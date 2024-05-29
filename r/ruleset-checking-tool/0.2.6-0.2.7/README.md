# Comparing `tmp/ruleset_checking_tool-0.2.6.tar.gz` & `tmp/ruleset_checking_tool-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruleset_checking_tool-0.2.6.tar", max compression
+gzip compressed data, was "ruleset_checking_tool-0.2.7.tar", max compression
```

## Comparing `ruleset_checking_tool-0.2.6.tar` & `ruleset_checking_tool-0.2.7.tar`

### file list

```diff
@@ -1,875 +1,875 @@
--rw-r--r--   0        0        0     1852 2024-05-22 15:09:38.499692 ruleset_checking_tool-0.2.6/LICENSE
--rw-r--r--   0        0        0    10670 2024-05-22 15:09:38.499692 ruleset_checking_tool-0.2.6/README.md
--rw-r--r--   0        0        0     1027 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/pyproject.toml
--rwxr-xr-x   0        0        0       22 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/__init__.py
--rw-r--r--   0        0        0     5960 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/cli.py
--rw-r--r--   0        0        0        0 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/report_engine/__init__.py
--rw-r--r--   0        0        0     5795 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/report_engine/rct_report.py
--rw-r--r--   0        0        0     1201 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/reports/__init__.py
--rw-r--r--   0        0        0      323 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/reports/ashrae9012019/__init__.py
--rw-r--r--   0        0        0     4519 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/reports/ashrae9012019/ashrae901_2019_detail_report.py
--rw-r--r--   0        0        0     3285 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/reports/ashrae9012019/ashrae901_2019_software_test_report.py
--rw-r--r--   0        0        0     9198 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/reports/ashrae9012019/ashrae901_2019_summary_report.py
--rw-r--r--   0        0        0      301 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/reports/general/__init__.py
--rw-r--r--   0        0        0     2097 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/reports/general/engine_raw_output.py
--rw-r--r--   0        0        0     3686 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/reports/general/engine_raw_summary.py
--rw-r--r--   0        0        0     1959 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/reports/project_report.py
--rw-r--r--   0        0        0     3293 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/reports/utils.py
--rwxr-xr-x   0        0        0        0 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/rule_engine/__init__.py
--rw-r--r--   0        0        0     8584 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/rule_engine/engine.py
--rw-r--r--   0        0        0      269 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/rule_engine/memoize.py
--rw-r--r--   0        0        0     3670 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/rule_engine/partial_rule_definition.py
--rw-r--r--   0        0        0     1267 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/rule_engine/partial_rule_definition_test.py
--rw-r--r--   0        0        0      184 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/rule_engine/rct_outcome_label.py
--rw-r--r--   0        0        0    24854 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/rule_engine/rule_base.py
--rw-r--r--   0        0        0     7043 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/rule_engine/rule_base_test.py
--rw-r--r--   0        0        0     6759 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/rule_engine/rule_list_base.py
--rw-r--r--   0        0        0     7106 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/rule_engine/rule_list_indexed_base.py
--rw-r--r--   0        0        0     1932 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/rule_engine/ruleset_model_factory.py
--rw-r--r--   0        0        0      420 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/rule_engine/rulesets.py
--rw-r--r--   0        0        0      621 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/rule_engine/tests/test_engine.py
--rw-r--r--   0        0        0      682 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/rule_engine/tests/test_rules.py
--rw-r--r--   0        0        0     1480 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/rule_engine/utils.py
--rw-r--r--   0        0        0        0 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/ruleset_functions.py
--rw-r--r--   0        0        0     3030 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/rulesets/__init__.py
--rw-r--r--   0        0        0     1108 2024-05-22 15:09:38.575691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/__init__.py
--rw-r--r--   0        0        0   316614 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ASHRAE229.9012019.extra.schema.json
--rw-r--r--   0        0        0      442 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/__init__.py
--rw-r--r--   0        0        0     1101 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_lighting_space_type_BPF_area_type.json
--rw-r--r--   0        0        0     5485 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_lighting_space_type_bpf_bat.json
--rw-r--r--   0        0        0     1328 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_lighting_to_hvac_map.json
--rw-r--r--   0        0        0     1712 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.boilers.json
--rw-r--r--   0        0        0     3550 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.chillers.json
--rw-r--r--   0        0        0     4304 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.climate_zone_sets.json
--rw-r--r--   0        0        0   416731 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.construction_properties.json
--rw-r--r--   0        0        0     6532 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.construction_sets.json
--rw-r--r--   0        0        0     3875 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.heat_pumps.json
--rw-r--r--   0        0        0     4376 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.heat_pumps_heating.json
--rw-r--r--   0        0        0      322 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.heat_rejection.json
--rw-r--r--   0        0        0    14051 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.lpd_space_type.json
--rw-r--r--   0        0        0     7043 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.motors.json
--rw-r--r--   0        0        0    11969 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_baseline_hvac.json
--rw-r--r--   0        0        0    22063 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_constructions.json
--rw-r--r--   0        0        0     5606 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_economizers.json
--rw-r--r--   0        0        0     3222 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_heat_type.json
--rw-r--r--   0        0        0      677 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_hvac_bldg_type.json
--rw-r--r--   0        0        0    56059 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_interior_lighting.json
--rw-r--r--   0        0        0     5344 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_swh_bldg_type.json
--rw-r--r--   0        0        0     1915 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_wwr_bldg_type.json
--rw-r--r--   0        0        0     5070 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.unitary_acs.json
--rw-r--r--   0        0        0     5358 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.water_heaters.json
--rw-r--r--   0        0        0     3772 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_chillers.json
--rw-r--r--   0        0        0     3072 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_transformers.json
--rw-r--r--   0        0        0     5760 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_space_lighting_to_hvac_map.json
--rw-r--r--   0        0        0     1098 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_3_2.json
--rw-r--r--   0        0        0    23223 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_4_2_1_1.json
--rw-r--r--   0        0        0     2584 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_9_5_1.json
--rw-r--r--   0        0        0      331 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_9_6_1.json
--rw-r--r--   0        0        0      483 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_1_3_11.json
--rw-r--r--   0        0        0     1639 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_5_1.json
--rw-r--r--   0        0        0     3068 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_5_2.json
--rw-r--r--   0        0        0     1603 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_5_3.json
--rw-r--r--   0        0        0      541 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_5_4.json
--rw-r--r--   0        0        0     1011 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_5_5.json
--rw-r--r--   0        0        0     3819 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_6.json
--rw-r--r--   0        0        0        0 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/__init__.py
--rw-r--r--   0        0        0     6979 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/extra_schema_fns.py
--rw-r--r--   0        0        0     9342 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/extra_schema_fns_test.py
--rw-r--r--   0        0        0     2085 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_3_1_3_11_fns.py
--rw-r--r--   0        0        0      711 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_3_1_3_11_fns_test.py
--rw-r--r--   0        0        0     1681 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_3_2_fns.py
--rw-r--r--   0        0        0     2075 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_3_2_fns_test.py
--rw-r--r--   0        0        0     2476 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_4_2_1_1_fns.py
--rw-r--r--   0        0        0     1713 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_4_2_1_1_fns_test.py
--rw-r--r--   0        0        0     3167 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_8_4_4_fns.py
--rw-r--r--   0        0        0     2733 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_8_4_4_fns_test.py
--rw-r--r--   0        0        0     2679 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_9_5_1_fns.py
--rw-r--r--   0        0        0     1268 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_9_5_1_fns_test.py
--rw-r--r--   0        0        0     1188 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_9_6_1_fns.py
--rw-r--r--   0        0        0     5914 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_9_6_1_fns_test.py
--rw-r--r--   0        0        0     2250 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_111_fns.py
--rw-r--r--   0        0        0     2853 2024-05-22 15:09:38.579692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_111_fns_test.py
--rw-r--r--   0        0        0     8357 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_4_fns.py
--rw-r--r--   0        0        0     2991 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_4_fns_test.py
--rw-r--r--   0        0        0     2180 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_1_fns.py
--rw-r--r--   0        0        0     1598 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_1_fns_test.py
--rw-r--r--   0        0        0     3548 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_2_fns.py
--rw-r--r--   0        0        0     4270 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_2_fns_test.py
--rw-r--r--   0        0        0     3068 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_3_fns.py
--rw-r--r--   0        0        0     2037 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_3_fns_test.py
--rw-r--r--   0        0        0     1466 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_4_fns.py
--rw-r--r--   0        0        0      974 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_4_fns_test.py
--rw-r--r--   0        0        0     2946 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_5_fns.py
--rw-r--r--   0        0        0     1836 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_5_fns_test.py
--rw-r--r--   0        0        0     3289 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_6_fns.py
--rw-r--r--   0        0        0     5601 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_6_fns_test.py
--rw-r--r--   0        0        0     9102 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_7_fns.py
--rw-r--r--   0        0        0     1642 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_7_fns_test.py
--rw-r--r--   0        0        0     3035 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_8_fns.py
--rw-r--r--   0        0        0     1818 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_8_fns_test.py
--rw-r--r--   0        0        0     3002 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_9_1_fins.py
--rw-r--r--   0        0        0      667 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_9_1_fins_test.py
--rw-r--r--   0        0        0      495 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_lighting_space_type_BPF_area_type_map.py
--rw-r--r--   0        0        0      767 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_lighting_space_type_BPF_area_type_map_test.py
--rw-r--r--   0        0        0      466 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_lighting_space_type_to_bpf_bat.py
--rw-r--r--   0        0        0     1088 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_lighting_space_type_to_bpf_bat_test.py
--rw-r--r--   0        0        0      753 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_lighting_to_hvac_bat_map_fns.py
--rw-r--r--   0        0        0      407 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_lighting_to_hvac_bat_map_fns_test.py
--rw-r--r--   0        0        0     4972 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_utils.py
--rw-r--r--   0        0        0      570 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_utils_test.py
--rw-r--r--   0        0        0        0 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/__init__.py
--rw-r--r--   0        0        0     2430 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/aggregate_min_OA_schedule_across_zones.py
--rw-r--r--   0        0        0     1238 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/aggregate_min_OA_schedule_across_zones_test.py
--rw-r--r--   0        0        0     1846 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/are_all_hvac_sys_fan_objects_autosized.py
--rw-r--r--   0        0        0     8025 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/are_all_hvac_sys_fan_objects_autosized_test.py
--rw-r--r--   0        0        0     2251 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_system_type_compare.py
--rw-r--r--   0        0        0     1502 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_system_type_compare_test.py
--rw-r--r--   0        0        0        0 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/__init__.py
--rw-r--r--   0        0        0     2061 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_chw_loops_purcahsed_cooling.py
--rw-r--r--   0        0        0     1078 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_cool_sources_chilled_water.py
--rw-r--r--   0        0        0     1241 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_cool_sources_none_or_null.py
--rw-r--r--   0        0        0     1147 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_fan_configs_parallel.py
--rw-r--r--   0        0        0     1032 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_fans_null.py
--rw-r--r--   0        0        0     1022 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_heat_sources_electric.py
--rw-r--r--   0        0        0     1362 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_heat_sources_hot_water.py
--rw-r--r--   0        0        0     1258 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_heat_sources_none_or_null.py
--rw-r--r--   0        0        0     1980 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_heating_loops_attached_to_boiler.py
--rw-r--r--   0        0        0     2216 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_heating_loops_purchased_heating.py
--rw-r--r--   0        0        0     1295 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_supplies_ducted.py
--rw-r--r--   0        0        0     1362 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_types_CAV.py
--rw-r--r--   0        0        0     1141 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_types_CAV_with_none_equal_to_null.py
--rw-r--r--   0        0        0     1201 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_types_VAV.py
--rw-r--r--   0        0        0      849 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/do_all_terminals_have_one_fan.py
--rw-r--r--   0        0        0      942 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/does_each_zone_have_only_one_terminal.py
--rw-r--r--   0        0        0      540 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/does_hvac_system_serve_single_zone.py
--rw-r--r--   0        0        0      898 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/get_dict_with_terminal_units_and_zones.py
--rw-r--r--   0        0        0      924 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_cooling_type_DX.py
--rw-r--r--   0        0        0     1260 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_cooling_type_fluid_loop.py
--rw-r--r--   0        0        0     1050 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_cooling_type_none.py
--rw-r--r--   0        0        0     1153 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_cooling_type_none_or_non_mechanical.py
--rw-r--r--   0        0        0     1019 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fan_sys_CV.py
--rw-r--r--   0        0        0     1167 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fan_sys_VSD.py
--rw-r--r--   0        0        0     1444 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fluid_loop_attached_to_boiler.py
--rw-r--r--   0        0        0     2193 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fluid_loop_attached_to_chiller.py
--rw-r--r--   0        0        0     1524 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fluid_loop_purchased_CHW.py
--rw-r--r--   0        0        0     1633 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fluid_loop_purchased_heating.py
--rw-r--r--   0        0        0     1017 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_heating_type_elec_resistance.py
--rw-r--r--   0        0        0     1251 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_heating_type_fluid_loop.py
--rw-r--r--   0        0        0     1020 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_heating_type_furnace.py
--rw-r--r--   0        0        0     1064 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_heating_type_heat_pump.py
--rw-r--r--   0        0        0     1453 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_preheat_fluid_loop_attached_to_boiler.py
--rw-r--r--   0        0        0     1539 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_preheat_fluid_loop_purchased_heating.py
--rw-r--r--   0        0        0     1054 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_preheating_type_elec_resistance.py
--rw-r--r--   0        0        0     1309 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_preheating_type_fluid_loop.py
--rw-r--r--   0        0        0      445 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_system_multizone.py
--rw-r--r--   0        0        0     2030 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_chw_loops_purchased_cooling.py
--rw-r--r--   0        0        0     1677 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_cool_sources_chilled_water.py
--rw-r--r--   0        0        0     1735 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_cool_sources_none_or_null.py
--rw-r--r--   0        0        0     1768 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_fan_configs_parallel.py
--rw-r--r--   0        0        0     1673 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_fans_null.py
--rw-r--r--   0        0        0     1716 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_heat_sources_electric.py
--rw-r--r--   0        0        0     1815 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_heat_sources_hot_water.py
--rw-r--r--   0        0        0     1731 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_heat_sources_none_or_null.py
--rw-r--r--   0        0        0     2209 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_heating_loops_attached_to_boiler.py
--rw-r--r--   0        0        0     2938 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_heating_loops_purchased_heating.py
--rw-r--r--   0        0        0     1679 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_supplies_ducted.py
--rw-r--r--   0        0        0     2367 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_types_CAV.py
--rw-r--r--   0        0        0     1626 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_types_VAV.py
--rw-r--r--   0        0        0     1894 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_do_all_terminals_have_one_fan.py
--rw-r--r--   0        0        0     2444 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_does_each_zone_have_only_one_terminal.py
--rw-r--r--   0        0        0    12083 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_get_dict_with_terminal_units_and_zones.py
--rw-r--r--   0        0        0     1735 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_cooling_type_DX.py
--rw-r--r--   0        0        0     2392 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_cooling_type_fluid_loop.py
--rw-r--r--   0        0        0     2336 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_cooling_type_none.py
--rw-r--r--   0        0        0     2963 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_cooling_type_none_or_non_mechanical.py
--rw-r--r--   0        0        0     2104 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fan_sys_CV.py
--rw-r--r--   0        0        0     2123 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fan_sys_vsd.py
--rw-r--r--   0        0        0     3147 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fluid_loop_attached_to_boiler.py
--rw-r--r--   0        0        0     2676 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fluid_loop_attached_to_chiller.py
--rw-r--r--   0        0        0     2552 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fluid_loop_purchased_chw.py
--rw-r--r--   0        0        0     3146 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fluid_loop_purchased_heating.py
--rw-r--r--   0        0        0     2471 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_heating_type_elec_resistance.py
--rw-r--r--   0        0        0     2489 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_heating_type_fluid_loop.py
--rw-r--r--   0        0        0     2423 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_heating_type_furnace.py
--rw-r--r--   0        0        0     2504 2024-05-22 15:09:38.583691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_heating_type_heat_pump.py
--rw-r--r--   0        0        0     3243 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_preheat_fluid_loop_attached_to_boiler.py
--rw-r--r--   0        0        0     3228 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_preheat_fluid_loop_purchased_heating.py
--rw-r--r--   0        0        0     2489 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_preheating_type_elec_resistance.py
--rw-r--r--   0        0        0     2504 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_preheating_type_fluid_loop.py
--rw-r--r--   0        0        0     6516 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_test_util.py
--rw-r--r--   0        0        0     1970 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_system_util.py
--rw-r--r--   0        0        0     6054 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_1.py
--rw-r--r--   0        0        0     6162 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_10.py
--rw-r--r--   0        0        0     6129 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_11_1.py
--rw-r--r--   0        0        0     4955 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_11_2.py
--rw-r--r--   0        0        0     5920 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_12.py
--rw-r--r--   0        0        0     5010 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_13.py
--rw-r--r--   0        0        0     3930 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_1_a.py
--rw-r--r--   0        0        0     3909 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_1_c.py
--rw-r--r--   0        0        0     4263 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_2.py
--rw-r--r--   0        0        0     6113 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_3.py
--rw-r--r--   0        0        0     4273 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_4.py
--rw-r--r--   0        0        0     5629 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_5.py
--rw-r--r--   0        0        0     5866 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_6.py
--rw-r--r--   0        0        0     6978 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_7.py
--rw-r--r--   0        0        0     6908 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_8.py
--rw-r--r--   0        0        0     4599 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_9.py
--rw-r--r--   0        0        0     3940 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_9b.py
--rw-r--r--   0        0        0    12699 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_1.py
--rw-r--r--   0        0        0     6708 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_10.py
--rw-r--r--   0        0        0    20538 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_11_1.py
--rw-r--r--   0        0        0    13207 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_11_2.py
--rw-r--r--   0        0        0    18622 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_12.py
--rw-r--r--   0        0        0    11871 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_13.py
--rw-r--r--   0        0        0     3766 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_2.py
--rw-r--r--   0        0        0    15515 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_3.py
--rw-r--r--   0        0        0     3854 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_4.py
--rw-r--r--   0        0        0    11711 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_5.py
--rw-r--r--   0        0        0    11183 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_6.py
--rw-r--r--   0        0        0    25141 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_7.py
--rw-r--r--   0        0        0    28077 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_8.py
--rw-r--r--   0        0        0     7117 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_9.py
--rw-r--r--   0        0        0     4524 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/check_purchased_chw_hhw_status_dict.py
--rw-r--r--   0        0        0    13931 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/check_purchased_chw_hhw_status_dict_test.py
--rw-r--r--   0        0        0     3003 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/compare_schedules.py
--rw-r--r--   0        0        0     2748 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/compare_schedules_test.py
--rw-r--r--   0        0        0        0 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/__init__.py
--rw-r--r--   0        0        0     6274 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1c.py
--rw-r--r--   0        0        0    21213 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1c_test.py
--rw-r--r--   0        0        0     5630 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1d.py
--rw-r--r--   0        0        0     3262 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1d_test.py
--rw-r--r--   0        0        0     2636 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1e.py
--rw-r--r--   0        0        0     4974 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1e_test.py
--rw-r--r--   0        0        0      850 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1f.py
--rw-r--r--   0        0        0     1200 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1g.py
--rw-r--r--   0        0        0     4594 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1g_test.py
--rw-r--r--   0        0        0        0 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/__init__.py
--rw-r--r--   0        0        0     7111 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/expected_system_type_from_table_g311a_dict.py
--rw-r--r--   0        0        0     6567 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/expected_system_type_from_table_g311a_dict_test.py
--rw-r--r--   0        0        0      964 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_building_lab_zones_list.py
--rw-r--r--   0        0        0     3075 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_building_lab_zones_list_test.py
--rw-r--r--   0        0        0     1313 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_building_total_lab_exhaust_from_zone_exhaust_fans.py
--rw-r--r--   0        0        0     3522 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_building_total_lab_exhaust_from_zone_exhaust_fans_test.py
--rw-r--r--   0        0        0     1103 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_computer_zones_peak_cooling_load.py
--rw-r--r--   0        0        0     3143 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_computer_zones_peak_cooling_load_test.py
--rw-r--r--   0        0        0     8214 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_hvac_building_area_types_and_zones_dict.py
--rw-r--r--   0        0        0     6987 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_hvac_building_area_types_and_zones_dict_test.py
--rw-r--r--   0        0        0     2883 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_number_of_floors.py
--rw-r--r--   0        0        0     6540 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_number_of_floors_test.py
--rw-r--r--   0        0        0     1457 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_predominant_hvac_building_area_type.py
--rw-r--r--   0        0        0     5785 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_predominant_hvac_building_area_type_test.py
--rw-r--r--   0        0        0     5972 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_eflh.py
--rw-r--r--   0        0        0     5670 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_eflh_test.py
--rw-r--r--   0        0        0     1552 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_hvac_bat.py
--rw-r--r--   0        0        0     2695 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_hvac_bat_test.py
--rw-r--r--   0        0        0     3548 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_peak_internal_load_floor_area_dict.py
--rw-r--r--   0        0        0     7874 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_peak_internal_load_floor_area_dict_test.py
--rw-r--r--   0        0        0     2588 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zones_computer_rooms.py
--rw-r--r--   0        0        0     3519 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zones_computer_rooms_test.py
--rw-r--r--   0        0        0     1094 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zones_on_same_floor_list.py
--rw-r--r--   0        0        0     1597 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zones_on_same_floor_list_test.py
--rw-r--r--   0        0        0     1998 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_space_a_computer_room.py
--rw-r--r--   0        0        0     3999 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_space_a_computer_room_test.py
--rw-r--r--   0        0        0     4077 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_likely_a_vestibule.py
--rw-r--r--   0        0        0     5148 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_likely_a_vestibule_test.py
--rw-r--r--   0        0        0     2909 2024-05-22 15:09:38.587691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_mechanically_cooled.py
--rw-r--r--   0        0        0     3681 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_mechanically_cooled_test.py
--rw-r--r--   0        0        0     2315 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_mechanically_heated_and_not_cooled.py
--rw-r--r--   0        0        0     6099 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_mechanically_heated_and_not_cooled_test.py
--rw-r--r--   0        0        0     5162 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_BPF_building_area_types_and_zones.py
--rw-r--r--   0        0        0     6302 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_BPF_building_area_types_and_zones_test.py
--rw-r--r--   0        0        0     2840 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_aggregated_zone_hvac_fan_operating_schedule.py
--rw-r--r--   0        0        0     4366 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_aggregated_zone_hvac_fan_operating_schedule_test.py
--rw-r--r--   0        0        0     4078 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_area_type_window_wall_area_dict.py
--rw-r--r--   0        0        0    28034 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_area_type_window_wall_area_dict_test.py
--rw-r--r--   0        0        0     1220 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_avg_zone_height.py
--rw-r--r--   0        0        0      444 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_avg_zone_height_test.py
--rw-r--r--   0        0        0     5090 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_baseline_system_types.py
--rw-r--r--   0        0        0    14126 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_baseline_system_types_test.py
--rw-r--r--   0        0        0     4804 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_scc_skylight_roof_ratios_dict.py
--rw-r--r--   0        0        0    35707 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_scc_skylight_roof_ratios_dict_test.py
--rw-r--r--   0        0        0     4652 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_scc_window_wall_ratios_dict.py
--rw-r--r--   0        0        0     7395 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_scc_window_wall_ratios_dict_test.py
--rw-r--r--   0        0        0     2166 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_segment_lighting_status_type_dict.py
--rw-r--r--   0        0        0     6583 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_segment_lighting_status_type_dict_test.py
--rw-r--r--   0        0        0     3809 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_segment_skylight_roof_areas_dict.py
--rw-r--r--   0        0        0     7906 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_segment_skylight_roof_areas_dict_test.py
--rw-r--r--   0        0        0     3058 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_dict_of_zones_and_terminal_units_served_by_hvac_sys.py
--rw-r--r--   0        0        0     4529 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_dict_of_zones_and_terminal_units_served_by_hvac_sys_test.py
--rw-r--r--   0        0        0     1645 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_dict_of_zones_hvac_sys_serving_specific_floor.py
--rw-r--r--   0        0        0     3191 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_dict_of_zones_hvac_sys_serving_specific_floor_test.py
--rw-r--r--   0        0        0     1905 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_fan_object_electric_power.py
--rw-r--r--   0        0        0     9193 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_fan_object_electric_power_test.py
--rw-r--r--   0        0        0     3172 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_fan_system_object_supply_return_exhaust_relief_total_power_flow.py
--rw-r--r--   0        0        0     9009 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_fan_system_object_supply_return_exhaust_relief_total_power_flow_test.py
--rw-r--r--   0        0        0     1177 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_heat_rejection_loops_connected_to_baseline_systems.py
--rw-r--r--   0        0        0     7324 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_heat_rejection_loops_connected_to_baseline_systems_test.py
--rw-r--r--   0        0        0     4057 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_sys_and_assoc_zones_largest_exhaust_source.py
--rw-r--r--   0        0        0    10446 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_sys_and_assoc_zones_largest_exhaust_source_test.py
--rw-r--r--   0        0        0     2912 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_5_6_serving_multiple_floors.py
--rw-r--r--   0        0        0     5260 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_5_6_serving_multiple_floors_test.py
--rw-r--r--   0        0        0     2652 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_primarily_serving_comp_room.py
--rw-r--r--   0        0        0     4313 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_primarily_serving_comp_room_test.py
--rw-r--r--   0        0        0     3178 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_serving_zone_health_safety_vent_reqs.py
--rw-r--r--   0        0        0     4161 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_serving_zone_health_safety_vent_reqs_test.py
--rw-r--r--   0        0        0     3523 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_zone_list_w_area_dict.py
--rw-r--r--   0        0        0     3100 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_zone_list_w_area_dict_test.py
--rw-r--r--   0        0        0     4605 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hw_loop_zone_list_w_area_dict.py
--rw-r--r--   0        0        0    10193 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hw_loop_zone_list_w_area_dict_test.py
--rw-r--r--   0        0        0     2653 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_lab_zone_hvac_systems.py
--rw-r--r--   0        0        0    24709 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_lab_zone_hvac_systems_test.py
--rw-r--r--   0        0        0     1055 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_list_hvac_systems_associated_with_zone.py
--rw-r--r--   0        0        0     2114 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_list_hvac_systems_associated_with_zone_test.py
--rw-r--r--   0        0        0     3824 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_min_oa_cfm_sch_zone.py
--rw-r--r--   0        0        0     3851 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_min_oa_cfm_sch_zone_test.py
--rw-r--r--   0        0        0     1691 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_most_used_weekday_hourly_schedule.py
--rw-r--r--   0        0        0     3621 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_most_used_weekday_hourly_schedule_test.py
--rw-r--r--   0        0        0     2241 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_opaque_surface_type.py
--rw-r--r--   0        0        0     1279 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_opaque_surface_type_test.py
--rw-r--r--   0        0        0     3261 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_primary_secondary_loops_dict.py
--rw-r--r--   0        0        0     5591 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_primary_secondary_loops_dict_test.py
--rw-r--r--   0        0        0     2697 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_proposed_hvac_modeled_with_virtual_cooling.py
--rw-r--r--   0        0        0     4407 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_proposed_hvac_modeled_with_virtual_cooling_test.py
--rw-r--r--   0        0        0     3545 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_proposed_hvac_modeled_with_virtual_heating.py
--rw-r--r--   0        0        0     8449 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_proposed_hvac_modeled_with_virtual_heating_test.py
--rw-r--r--   0        0        0     6402 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_surface_conditioning_category_dict.py
--rw-r--r--   0        0        0     1546 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_BPF_BAT.py
--rw-r--r--   0        0        0     4273 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_BPF_BAT_test.py
--rw-r--r--   0        0        0    18860 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_conditioning_category_dict.py
--rw-r--r--   0        0        0    38896 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_conditioning_category_dict_test.py
--rw-r--r--   0        0        0     3444 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_peak_internal_load_floor_area_dict.py
--rw-r--r--   0        0        0     7838 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_peak_internal_load_floor_area_dict_test.py
--rw-r--r--   0        0        0     8606 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_supply_return_exhaust_relief_terminal_fan_power_dict.py
--rw-r--r--   0        0        0    16330 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_supply_return_exhaust_relief_terminal_fan_power_dict_test.py
--rw-r--r--   0        0        0     9236 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_target_baseline_system.py
--rw-r--r--   0        0        0    36803 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_target_baseline_system_test.py
--rw-r--r--   0        0        0      881 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/is_cz_0_to_3a_bool.py
--rw-r--r--   0        0        0     1951 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/is_economizer_modeled_in_proposed.py
--rw-r--r--   0        0        0     9547 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/is_economizer_modeled_in_proposed_test.py
--rw-r--r--   0        0        0     5298 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/normalize_interior_lighting_schedules.py
--rw-r--r--   0        0        0     5071 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/normalize_interior_lighting_schedules_test.py
--rw-r--r--   0        0        0      452 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section1/__init__.py
--rw-r--r--   0        0        0     5946 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section1/section1rule1.py
--rw-r--r--   0        0        0     4518 2024-05-22 15:09:38.591691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section1/section1rule2.py
--rw-r--r--   0        0        0     5681 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section1/section1rule3.py
--rw-r--r--   0        0        0     3341 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section1/section1rule4.py
--rw-r--r--   0        0        0     7317 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section1/section1rule5.py
--rw-r--r--   0        0        0     1660 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section1/section1rule6.py
--rw-r--r--   0        0        0     1699 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section1/section1rule7.py
--rw-r--r--   0        0        0      350 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section10/__init__.py
--rw-r--r--   0        0        0    22013 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section10/section10rule14.py
--rw-r--r--   0        0        0    12015 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section10/section10rule7.py
--rw-r--r--   0        0        0      371 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section12/__init__.py
--rw-r--r--   0        0        0     1931 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section12/section12rule1.py
--rw-r--r--   0        0        0     1929 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section12/section12rule2.py
--rw-r--r--   0        0        0     2432 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section12/section12rule3.py
--rw-r--r--   0        0        0      437 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section15/__init__.py
--rw-r--r--   0        0        0     1264 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section15/section15rule1.py
--rw-r--r--   0        0        0     1262 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section15/section15rule2.py
--rw-r--r--   0        0        0     1865 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section15/section15rule3.py
--rw-r--r--   0        0        0     1964 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section15/section15rule4.py
--rw-r--r--   0        0        0     3825 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section15/section15rule5.py
--rw-r--r--   0        0        0     2943 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section15/section15rule6.py
--rw-r--r--   0        0        0      371 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section18/__init__.py
--rw-r--r--   0        0        0    11675 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section18/section18rule1.py
--rw-r--r--   0        0        0    17207 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section18/section18rule2.py
--rw-r--r--   0        0        0     2832 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section18/section18rule3.py
--rw-r--r--   0        0        0     1124 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/__init__.py
--rw-r--r--   0        0        0     7594 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule1.py
--rw-r--r--   0        0        0    14069 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule10.py
--rw-r--r--   0        0        0     3354 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule11.py
--rw-r--r--   0        0        0     4168 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule12.py
--rw-r--r--   0        0        0    12793 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule13.py
--rw-r--r--   0        0        0    11238 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule14.py
--rw-r--r--   0        0        0    10527 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule15.py
--rw-r--r--   0        0        0     6898 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule16.py
--rw-r--r--   0        0        0     5947 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule17.py
--rw-r--r--   0        0        0    14589 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule18.py
--rw-r--r--   0        0        0    13082 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule19.py
--rw-r--r--   0        0        0     9747 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule2.py
--rw-r--r--   0        0        0    10232 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule20.py
--rw-r--r--   0        0        0    24073 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule21.py
--rw-r--r--   0        0        0     2547 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule22.py
--rw-r--r--   0        0        0    25140 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule23.py
--rw-r--r--   0        0        0     4017 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule24.py
--rw-r--r--   0        0        0     5445 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule25.py
--rw-r--r--   0        0        0     4208 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule26.py
--rw-r--r--   0        0        0     4184 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule27.py
--rw-r--r--   0        0        0     3899 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule28.py
--rw-r--r--   0        0        0     3921 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule29.py
--rw-r--r--   0        0        0     2549 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule3.py
--rw-r--r--   0        0        0     3213 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule30.py
--rw-r--r--   0        0        0     3845 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule31.py
--rw-r--r--   0        0        0     3606 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule32.py
--rw-r--r--   0        0        0     4298 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule33.py
--rw-r--r--   0        0        0     5479 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule34.py
--rw-r--r--   0        0        0    11267 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule35.py
--rw-r--r--   0        0        0     5256 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule36.py
--rw-r--r--   0        0        0    20009 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule4.py
--rw-r--r--   0        0        0     3278 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule5.py
--rw-r--r--   0        0        0     3281 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule6.py
--rw-r--r--   0        0        0    19179 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule7.py
--rw-r--r--   0        0        0     6145 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule8.py
--rw-r--r--   0        0        0     4034 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule9.py
--rw-r--r--   0        0        0      710 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/__init__.py
--rw-r--r--   0        0        0     2602 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule1.py
--rw-r--r--   0        0        0     5019 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule10.py
--rw-r--r--   0        0        0     3540 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule11.py
--rw-r--r--   0        0        0     4287 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule12.py
--rw-r--r--   0        0        0     4145 2024-05-22 15:09:38.595692 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule13.py
--rw-r--r--   0        0        0     2345 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule14.py
--rw-r--r--   0        0        0     2328 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule15.py
--rw-r--r--   0        0        0     2740 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule16.py
--rw-r--r--   0        0        0     4835 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule17.py
--rw-r--r--   0        0        0     3839 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule18.py
--rw-r--r--   0        0        0     2309 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule2.py
--rw-r--r--   0        0        0     3517 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule3.py
--rw-r--r--   0        0        0     3176 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule4.py
--rw-r--r--   0        0        0     7604 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule5.py
--rw-r--r--   0        0        0     6391 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule6.py
--rw-r--r--   0        0        0     5061 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule7.py
--rw-r--r--   0        0        0     9095 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule8.py
--rw-r--r--   0        0        0     4159 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule9.py
--rw-r--r--   0        0        0     1239 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/__init__.py
--rw-r--r--   0        0        0     4595 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule1.py
--rw-r--r--   0        0        0     7954 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule10.py
--rw-r--r--   0        0        0     5315 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule11.py
--rw-r--r--   0        0        0     3712 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule12.py
--rw-r--r--   0        0        0     3292 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule13.py
--rw-r--r--   0        0        0     3635 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule14.py
--rw-r--r--   0        0        0     3484 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule15.py
--rw-r--r--   0        0        0     5261 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule16.py
--rw-r--r--   0        0        0     6472 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule17.py
--rw-r--r--   0        0        0     2895 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule18.py
--rw-r--r--   0        0        0     3913 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule19.py
--rw-r--r--   0        0        0     4597 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule2.py
--rw-r--r--   0        0        0     4398 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule20.py
--rw-r--r--   0        0        0     4270 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule21.py
--rw-r--r--   0        0        0     4038 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule22.py
--rw-r--r--   0        0        0     3130 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule23.py
--rw-r--r--   0        0        0     4040 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule24.py
--rw-r--r--   0        0        0     5089 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule25.py
--rw-r--r--   0        0        0     4545 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule26.py
--rw-r--r--   0        0        0     3256 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule27.py
--rw-r--r--   0        0        0     3567 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule28.py
--rw-r--r--   0        0        0     4791 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule29.py
--rw-r--r--   0        0        0     4224 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule3.py
--rw-r--r--   0        0        0     4139 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule30.py
--rw-r--r--   0        0        0     3425 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule31.py
--rw-r--r--   0        0        0     4735 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule32.py
--rw-r--r--   0        0        0     3095 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule33.py
--rw-r--r--   0        0        0     4022 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule34.py
--rw-r--r--   0        0        0     2240 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule35.py
--rw-r--r--   0        0        0     5416 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule36.py
--rw-r--r--   0        0        0     2274 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule37.py
--rw-r--r--   0        0        0     2304 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule38.py
--rw-r--r--   0        0        0     2293 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule39.py
--rw-r--r--   0        0        0     8949 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule4.py
--rw-r--r--   0        0        0     3230 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule40.py
--rw-r--r--   0        0        0     1441 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule41.py
--rw-r--r--   0        0        0     4010 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule5.py
--rw-r--r--   0        0        0     4682 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule6.py
--rw-r--r--   0        0        0     2480 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule7.py
--rw-r--r--   0        0        0     7284 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule8.py
--rw-r--r--   0        0        0     5729 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule9.py
--rw-r--r--   0        0        0      664 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/__init__.py
--rw-r--r--   0        0        0     6509 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule1.py
--rw-r--r--   0        0        0     4511 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule10.py
--rw-r--r--   0        0        0     6197 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule11.py
--rw-r--r--   0        0        0     1900 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule12.py
--rw-r--r--   0        0        0     5456 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule13.py
--rw-r--r--   0        0        0     5471 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule14.py
--rw-r--r--   0        0        0     5369 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule15.py
--rw-r--r--   0        0        0     7363 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule16.py
--rw-r--r--   0        0        0     5020 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule2.py
--rw-r--r--   0        0        0     4870 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule3.py
--rw-r--r--   0        0        0     3953 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule4.py
--rw-r--r--   0        0        0     3597 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule5.py
--rw-r--r--   0        0        0     4840 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule6.py
--rw-r--r--   0        0        0     4100 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule7.py
--rw-r--r--   0        0        0     6507 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule8.py
--rw-r--r--   0        0        0     6592 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule9.py
--rw-r--r--   0        0        0      391 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section4/__init__.py
--rw-r--r--   0        0        0     9893 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section4/section4rule1.py
--rw-r--r--   0        0        0    12790 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section4/section4rule11.py
--rw-r--r--   0        0        0     5258 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section4/section4rule14.py
--rw-r--r--   0        0        0    12964 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section4/section4rule2.py
--rw-r--r--   0        0        0     1255 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/archive/__init__.py
--rw-r--r--   0        0        0     2572 2024-05-22 15:09:38.599691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/archive/section5rule2.py
--rw-r--r--   0        0        0     5510 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/archive/section5rule45.py
--rw-r--r--   0        0        0    12911 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule1.py
--rw-r--r--   0        0        0     6192 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule10.py
--rw-r--r--   0        0        0     3855 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule11.py
--rw-r--r--   0        0        0     6989 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule12.py
--rw-r--r--   0        0        0     7996 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule13.py
--rw-r--r--   0        0        0     8371 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule14.py
--rw-r--r--   0        0        0     5670 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule15.py
--rw-r--r--   0        0        0     8058 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule16.py
--rw-r--r--   0        0        0     3259 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule17.py
--rw-r--r--   0        0        0     2595 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule18.py
--rw-r--r--   0        0        0    13122 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule19.py
--rw-r--r--   0        0        0     2560 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule2.py
--rw-r--r--   0        0        0    12795 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule20.py
--rw-r--r--   0        0        0     6377 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule21.py
--rw-r--r--   0        0        0     5202 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule22.py
--rw-r--r--   0        0        0     5354 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule23.py
--rw-r--r--   0        0        0     5309 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule24.py
--rw-r--r--   0        0        0     5172 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule25.py
--rw-r--r--   0        0        0     9147 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule26.py
--rw-r--r--   0        0        0    12014 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule27.py
--rw-r--r--   0        0        0    10811 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule28.py
--rw-r--r--   0        0        0     4023 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule29.py
--rw-r--r--   0        0        0     3819 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule3.py
--rw-r--r--   0        0        0     6214 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule30.py
--rw-r--r--   0        0        0     4013 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule31.py
--rw-r--r--   0        0        0     6286 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule32.py
--rw-r--r--   0        0        0     2425 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule33.py
--rw-r--r--   0        0        0     3346 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule34.py
--rw-r--r--   0        0        0     5016 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule35.py
--rw-r--r--   0        0        0     4104 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule36.py
--rw-r--r--   0        0        0     7794 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule37.py
--rw-r--r--   0        0        0     2636 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule38.py
--rw-r--r--   0        0        0    11390 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule39.py
--rw-r--r--   0        0        0     6173 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule4.py
--rw-r--r--   0        0        0     5775 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule40.py
--rw-r--r--   0        0        0     3778 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule5.py
--rw-r--r--   0        0        0     6418 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule6.py
--rw-r--r--   0        0        0     3789 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule7.py
--rw-r--r--   0        0        0     6172 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule8.py
--rw-r--r--   0        0        0     4145 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule9.py
--rw-r--r--   0        0        0      494 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/archive/__init__.py
--rw-r--r--   0        0        0     3062 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/archive/section6rule1_archive.py
--rw-r--r--   0        0        0     6870 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/section6rule1.py
--rw-r--r--   0        0        0     4863 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/section6rule2.py
--rw-r--r--   0        0        0     5247 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/section6rule3.py
--rw-r--r--   0        0        0     7707 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/section6rule4.py
--rw-r--r--   0        0        0     8765 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/section6rule5.py
--rw-r--r--   0        0        0     2422 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/section6rule6.py
--rw-r--r--   0        0        0     5381 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/section6rule7.py
--rw-r--r--   0        0        0     8400 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/section6rule8.py
--rw-r--r--   0        0        0     9177 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/section6rule9.py
--rw-r--r--   0        0        0    21344 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/Ruletest_JSON_Generation_Guide.md
--rw-r--r--   0        0        0    31094 2024-05-22 15:09:38.603691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_engine.py
--rw-r--r--   0        0        0 32998400 2024-05-22 15:09:38.643691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/airside_hvac_master.json
--rw-r--r--   0        0        0   116907 2024-05-22 15:09:38.647691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/airside_hvac_tests.json
--rw-r--r--   0        0        0   659490 2024-05-22 15:09:38.647691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/boiler_tcd_master.json
--rw-r--r--   0        0        0   299816 2024-05-22 15:09:38.647691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/boiler_tests.json
--rw-r--r--   0        0        0  1517314 2024-05-22 15:09:38.651691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/chiller_tcd_master.json
--rw-r--r--   0        0        0   586660 2024-05-22 15:09:38.651691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/chiller_tests.json
--rw-r--r--   0        0        0  1117107 2024-05-22 15:09:38.651691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/envelope_tcd_master.json
--rw-r--r--   0        0        0  2205088 2024-05-22 15:09:38.667691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/envelope_tests.json
--rw-r--r--   0        0        0 32996103 2024-05-22 15:09:38.711691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/hvac_airside_tcd_master.json
--rw-r--r--   0        0        0 19170731 2024-05-22 15:09:38.735691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/lighting_tcd_master.json
--rw-r--r--   0        0        0 14770206 2024-05-22 15:09:38.755691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/lighting_tests.json
--rw-r--r--   0        0        0    80929 2024-05-22 15:09:38.755691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/receptacle_tcd_master.json
--rw-r--r--   0        0        0    39152 2024-05-22 15:09:38.755691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/receptacle_tests.json
--rw-r--r--   0        0        0  2292360 2024-05-22 15:09:38.767691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/ruletest_spreadsheets/chiller_tcd_master.xlsx
--rw-r--r--   0        0        0    40737 2024-05-22 15:09:38.767691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_1.json
--rw-r--r--   0        0        0    41538 2024-05-22 15:09:38.767691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_2.json
--rw-r--r--   0        0        0    59369 2024-05-22 15:09:38.767691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_3.json
--rw-r--r--   0        0        0    39462 2024-05-22 15:09:38.767691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_4.json
--rw-r--r--   0        0        0    48906 2024-05-22 15:09:38.767691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_5.json
--rw-r--r--   0        0        0  5891602 2024-05-22 15:09:38.775691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_6.json
--rw-r--r--   0        0        0  5888042 2024-05-22 15:09:38.787691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_7.json
--rw-r--r--   0        0        0    96794 2024-05-22 15:09:38.787691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section10/rule_10_14.json
--rw-r--r--   0        0        0    30950 2024-05-22 15:09:38.787691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section10/rule_10_7.json
--rw-r--r--   0        0        0    15260 2024-05-22 15:09:38.787691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_1.json
--rw-r--r--   0        0        0    15254 2024-05-22 15:09:38.787691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_2.json
--rw-r--r--   0        0        0     9368 2024-05-22 15:09:38.787691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_3.json
--rw-r--r--   0        0        0     9372 2024-05-22 15:09:38.787691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_4.json
--rw-r--r--   0        0        0    10785 2024-05-22 15:09:38.787691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_5.json
--rw-r--r--   0        0        0    10278 2024-05-22 15:09:38.787691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_6.json
--rw-r--r--   0        0        0    10624 2024-05-22 15:09:38.787691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_7.json
--rw-r--r--   0        0        0     5995 2024-05-22 15:09:38.787691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_1.json
--rw-r--r--   0        0        0     5989 2024-05-22 15:09:38.787691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_2.json
--rw-r--r--   0        0        0     3660 2024-05-22 15:09:38.787691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_3.json
--rw-r--r--   0        0        0     3664 2024-05-22 15:09:38.787691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_4.json
--rw-r--r--   0        0        0     8796 2024-05-22 15:09:38.787691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_5.json
--rw-r--r--   0        0        0     5944 2024-05-22 15:09:38.787691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_6.json
--rw-r--r--   0        0        0  1524506 2024-05-22 15:09:38.791691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section18/rule_18_1.json
--rw-r--r--   0        0        0   244279 2024-05-22 15:09:38.791691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section18/rule_18_2.json
--rw-r--r--   0        0        0    79607 2024-05-22 15:09:38.791691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section18/rule_18_3.json
--rw-r--r--   0        0        0    22542 2024-05-22 15:09:38.791691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_1.json
--rw-r--r--   0        0        0   112870 2024-05-22 15:09:38.791691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_10.json
--rw-r--r--   0        0        0    18811 2024-05-22 15:09:38.791691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_11.json
--rw-r--r--   0        0        0    23723 2024-05-22 15:09:38.791691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_12.json
--rw-r--r--   0        0        0    85619 2024-05-22 15:09:38.791691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_13.json
--rw-r--r--   0        0        0    83590 2024-05-22 15:09:38.791691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_14.json
--rw-r--r--   0        0        0    51803 2024-05-22 15:09:38.791691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_15.json
--rw-r--r--   0        0        0    27379 2024-05-22 15:09:38.791691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_16.json
--rw-r--r--   0        0        0    21628 2024-05-22 15:09:38.791691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_17.json
--rw-r--r--   0        0        0    48645 2024-05-22 15:09:38.791691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_18.json
--rw-r--r--   0        0        0    42409 2024-05-22 15:09:38.791691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_19.json
--rw-r--r--   0        0        0    16103 2024-05-22 15:09:38.791691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_2.json
--rw-r--r--   0        0        0    35260 2024-05-22 15:09:38.791691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_20.json
--rw-r--r--   0        0        0  8288791 2024-05-22 15:09:38.803691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_21.json
--rw-r--r--   0        0        0    12655 2024-05-22 15:09:38.803691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_22.json
--rw-r--r--   0        0        0  6615439 2024-05-22 15:09:38.807691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_23.json
--rw-r--r--   0        0        0    43490 2024-05-22 15:09:38.807691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_24.json
--rw-r--r--   0        0        0    73936 2024-05-22 15:09:38.811691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_25.json
--rw-r--r--   0        0        0    16507 2024-05-22 15:09:38.811691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_26.json
--rw-r--r--   0        0        0    16456 2024-05-22 15:09:38.811691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_27.json
--rw-r--r--   0        0        0    14210 2024-05-22 15:09:38.811691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_28.json
--rw-r--r--   0        0        0    14161 2024-05-22 15:09:38.811691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_29.json
--rw-r--r--   0        0        0     9836 2024-05-22 15:09:38.811691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_3.json
--rw-r--r--   0        0        0    20090 2024-05-22 15:09:38.811691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_30.json
--rw-r--r--   0        0        0     9875 2024-05-22 15:09:38.811691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_31.json
--rw-r--r--   0        0        0     9843 2024-05-22 15:09:38.811691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_32.json
--rw-r--r--   0        0        0    27391 2024-05-22 15:09:38.811691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_33.json
--rw-r--r--   0        0        0    28337 2024-05-22 15:09:38.811691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_34.json
--rw-r--r--   0        0        0  3154605 2024-05-22 15:09:38.815691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_35.json
--rw-r--r--   0        0        0    31855 2024-05-22 15:09:38.815691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_36.json
--rw-r--r--   0        0        0  5816940 2024-05-22 15:09:38.819691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_4.json
--rw-r--r--   0        0        0    20414 2024-05-22 15:09:38.819691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_5.json
--rw-r--r--   0        0        0    20425 2024-05-22 15:09:38.819691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_6.json
--rw-r--r--   0        0        0  8138975 2024-05-22 15:09:38.827691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_7.json
--rw-r--r--   0        0        0    10604 2024-05-22 15:09:38.827691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_8.json
--rw-r--r--   0        0        0    13253 2024-05-22 15:09:38.827691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_9.json
--rw-r--r--   0        0        0    31359 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_1.json
--rw-r--r--   0        0        0    41011 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_10.json
--rw-r--r--   0        0        0    33002 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_11.json
--rw-r--r--   0        0        0    44857 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_12.json
--rw-r--r--   0        0        0    33163 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_13.json
--rw-r--r--   0        0        0    35885 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_16.json
--rw-r--r--   0        0        0    69811 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_17.json
--rw-r--r--   0        0        0    44303 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_18.json
--rw-r--r--   0        0        0    30887 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_2.json
--rw-r--r--   0        0        0    35154 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_3.json
--rw-r--r--   0        0        0    34560 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_4.json
--rw-r--r--   0        0        0    47111 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_5.json
--rw-r--r--   0        0        0    52419 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_6.json
--rw-r--r--   0        0        0    54422 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_7.json
--rw-r--r--   0        0        0    33612 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_8.json
--rw-r--r--   0        0        0    31414 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_9.json
--rw-r--r--   0        0        0    38016 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_1.json
--rw-r--r--   0        0        0    46003 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_10.json
--rw-r--r--   0        0        0    32354 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_11.json
--rw-r--r--   0        0        0    43483 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_12.json
--rw-r--r--   0        0        0    25993 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_13.json
--rw-r--r--   0        0        0    40407 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_14.json
--rw-r--r--   0        0        0    26350 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_15.json
--rw-r--r--   0        0        0    50504 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_16.json
--rw-r--r--   0        0        0    30506 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_17.json
--rw-r--r--   0        0        0    25272 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_18.json
--rw-r--r--   0        0        0    39459 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_19.json
--rw-r--r--   0        0        0    38727 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_2.json
--rw-r--r--   0        0        0    42840 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_20.json
--rw-r--r--   0        0        0    40769 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_21.json
--rw-r--r--   0        0        0    33361 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_22.json
--rw-r--r--   0        0        0    47776 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_23.json
--rw-r--r--   0        0        0    40404 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_24.json
--rw-r--r--   0        0        0    37088 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_25.json
--rw-r--r--   0        0        0    32602 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_26.json
--rw-r--r--   0        0        0    34653 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_27.json
--rw-r--r--   0        0        0    22587 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_28.json
--rw-r--r--   0        0        0    36184 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_29.json
--rw-r--r--   0        0        0    41205 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_3.json
--rw-r--r--   0        0        0    34583 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_30.json
--rw-r--r--   0        0        0    60737 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_31.json
--rw-r--r--   0        0        0    58309 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_32.json
--rw-r--r--   0        0        0    49199 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_33.json
--rw-r--r--   0        0        0    38235 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_34.json
--rw-r--r--   0        0        0    23563 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_35.json
--rw-r--r--   0        0        0    33713 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_36.json
--rw-r--r--   0        0        0    23345 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_37.json
--rw-r--r--   0        0        0    23819 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_38.json
--rw-r--r--   0        0        0    23607 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_39.json
--rw-r--r--   0        0        0    55361 2024-05-22 15:09:38.831691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_4.json
--rw-r--r--   0        0        0    47740 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_40.json
--rw-r--r--   0        0        0    23775 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_41.json
--rw-r--r--   0        0        0    26924 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_5.json
--rw-r--r--   0        0        0    35749 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_6.json
--rw-r--r--   0        0        0    35575 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_7.json
--rw-r--r--   0        0        0    38284 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_8.json
--rw-r--r--   0        0        0    38333 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_9.json
--rw-r--r--   0        0        0    23554 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_1.json
--rw-r--r--   0        0        0    20738 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_10.json
--rw-r--r--   0        0        0    18913 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_11.json
--rw-r--r--   0        0        0    14305 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_12.json
--rw-r--r--   0        0        0    16867 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_13.json
--rw-r--r--   0        0        0    16920 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_14.json
--rw-r--r--   0        0        0    16767 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_15.json
--rw-r--r--   0        0        0    17148 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_16.json
--rw-r--r--   0        0        0    25209 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_2.json
--rw-r--r--   0        0        0    26699 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_3.json
--rw-r--r--   0        0        0    22741 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_4.json
--rw-r--r--   0        0        0    29046 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_5.json
--rw-r--r--   0        0        0    14166 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_6.json
--rw-r--r--   0        0        0    12884 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_7.json
--rw-r--r--   0        0        0    23981 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_8.json
--rw-r--r--   0        0        0    19380 2024-05-22 15:09:38.835691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_9.json
--rw-r--r--   0        0        0  2960310 2024-05-22 15:09:38.839691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section4/rule_4_1.json
--rw-r--r--   0        0        0  2954872 2024-05-22 15:09:38.847691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section4/rule_4_11.json
--rw-r--r--   0        0        0   728912 2024-05-22 15:09:38.847691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section4/rule_4_14.json
--rw-r--r--   0        0        0  2213466 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section4/rule_4_2.json
--rw-r--r--   0        0        0    74747 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_17_19.json
--rw-r--r--   0        0        0    37237 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_26.json
--rw-r--r--   0        0        0     7503 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_27.json
--rw-r--r--   0        0        0    39596 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_13_15.json
--rw-r--r--   0        0        0     7675 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_16.json
--rw-r--r--   0        0        0    94101 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_17_19.json
--rw-r--r--   0        0        0    37237 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_26.json
--rw-r--r--   0        0        0    64847 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_2_8.json
--rw-r--r--   0        0        0    25181 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_33_44_46.json
--rw-r--r--   0        0        0    33024 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_9_12.json
--rw-r--r--   0        0        0     6064 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_example_tcds.json
--rw-r--r--   0        0        0    69636 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_20_25.json
--rw-r--r--   0        0        0    45859 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_28.json
--rw-r--r--   0        0        0    45859 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_28_31.json
--rw-r--r--   0        0        0   125061 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_34.json
--rw-r--r--   0        0        0   125061 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_34_39.json
--rw-r--r--   0        0        0    28853 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_45.json
--rw-r--r--   0        0        0    28853 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_47.json
--rw-r--r--   0        0        0    38501 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_49.json
--rw-r--r--   0        0        0    73721 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_53.json
--rw-r--r--   0        0        0     8650 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/rule_5_2.json
--rw-r--r--   0        0        0     8578 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/rule_5_3.json
--rw-r--r--   0        0        0    51135 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_1.json
--rw-r--r--   0        0        0    46233 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_10.json
--rw-r--r--   0        0        0     9687 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_11.json
--rw-r--r--   0        0        0    46780 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_12.json
--rw-r--r--   0        0        0    89032 2024-05-22 15:09:38.851691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_13.json
--rw-r--r--   0        0        0    29544 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_14.json
--rw-r--r--   0        0        0    41570 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_15.json
--rw-r--r--   0        0        0    29095 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_16.json
--rw-r--r--   0        0        0    12227 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_17.json
--rw-r--r--   0        0        0    11846 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_18.json
--rw-r--r--   0        0        0    47969 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_19.json
--rw-r--r--   0        0        0     8891 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_2.json
--rw-r--r--   0        0        0    48863 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_20.json
--rw-r--r--   0        0        0    43570 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_21.json
--rw-r--r--   0        0        0    18438 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_22.json
--rw-r--r--   0        0        0    10521 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_23.json
--rw-r--r--   0        0        0    21899 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_24.json
--rw-r--r--   0        0        0    21940 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_25.json
--rw-r--r--   0        0        0    24709 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_26.json
--rw-r--r--   0        0        0    46494 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_27.json
--rw-r--r--   0        0        0    18070 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_28.json
--rw-r--r--   0        0        0     9711 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_29.json
--rw-r--r--   0        0        0     9486 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_3.json
--rw-r--r--   0        0        0    36872 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_30.json
--rw-r--r--   0        0        0    10473 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_31.json
--rw-r--r--   0        0        0    36932 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_32.json
--rw-r--r--   0        0        0     7049 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_33.json
--rw-r--r--   0        0        0     8255 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_34.json
--rw-r--r--   0        0        0    50106 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_35.json
--rw-r--r--   0        0        0    14532 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_36.json
--rw-r--r--   0        0        0    26886 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_37.json
--rw-r--r--   0        0        0    14749 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_38.json
--rw-r--r--   0        0        0    23862 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_39.json
--rw-r--r--   0        0        0    45956 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_4.json
--rw-r--r--   0        0        0    22417 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_40.json
--rw-r--r--   0        0        0     9641 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_5.json
--rw-r--r--   0        0        0    46014 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_6.json
--rw-r--r--   0        0        0     9663 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_7.json
--rw-r--r--   0        0        0    46418 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_8.json
--rw-r--r--   0        0        0     9649 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_9.json
--rw-r--r--   0        0        0    32706 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_1.json
--rw-r--r--   0        0        0    33236 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_2.json
--rw-r--r--   0        0        0    26598 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_3.json
--rw-r--r--   0        0        0    33889 2024-05-22 15:09:38.855691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_4.json
--rw-r--r--   0        0        0  4357841 2024-05-22 15:09:38.867691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_5.json
--rw-r--r--   0        0        0     6295 2024-05-22 15:09:38.867691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_6.json
--rw-r--r--   0        0        0    23933 2024-05-22 15:09:38.867691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_7.json
--rw-r--r--   0        0        0 10236497 2024-05-22 15:09:38.879691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_8.json
--rw-r--r--   0        0        0  4419752 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_9.json
--rw-r--r--   0        0        0     4463 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System 12_CAV_SZ_HW.json
--rw-r--r--   0        0        0     4116 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System 12a_CAV_SZ_HW.json
--rw-r--r--   0        0        0     4485 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System 12b_CAV_SZ_HW.json
--rw-r--r--   0        0        0     3879 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System 13_CAV_SZ_ER.json
--rw-r--r--   0        0        0     3532 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System 13a_CAV_SZ_ER.json
--rw-r--r--   0        0        0     2163 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_10_Warm_Air_Furnace_Elec.json
--rw-r--r--   0        0        0     3891 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.1_VAV_SZ.json
--rw-r--r--   0        0        0     3544 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.1a_VAV_SZ.json
--rw-r--r--   0        0        0     4497 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.1b_VAV_SZ.json
--rw-r--r--   0        0        0     4096 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.1c_VAV_SZ.json
--rw-r--r--   0        0        0     4475 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.2_VAV_SZ.json
--rw-r--r--   0        0        0     4128 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.2a_VAV_SZ.json
--rw-r--r--   0        0        0     2994 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_1_PTAC.json
--rw-r--r--   0        0        0     2842 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_1a_PTAC.json
--rw-r--r--   0        0        0     3017 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_1b_PTAC.json
--rw-r--r--   0        0        0     2811 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_1c_PTAC.json
--rw-r--r--   0        0        0     2557 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_2_PTHP.json
--rw-r--r--   0        0        0     2815 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_3_PSZ_AC_Gas_Furnace.json
--rw-r--r--   0        0        0     3298 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_3a_PSZ_AC_Gas_Furnace.json
--rw-r--r--   0        0        0     3290 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_3b_PSZ_AC_Gas_Furnace.json
--rw-r--r--   0        0        0     3676 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_3c_PSZ_AC_Gas_Furnace.json
--rw-r--r--   0        0        0     2812 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_4_PSZ_HP.json
--rw-r--r--   0        0        0     4659 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_5_PVAV_HW_Reheat.json
--rw-r--r--   0        0        0     4696 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_5b_PVAV_HW_Reheat.json
--rw-r--r--   0        0        0     4306 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_6_PVAV_Elec_Reheat.json
--rw-r--r--   0        0        0     5174 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_6b_PVAV_Elec_Reheat.json
--rw-r--r--   0        0        0     5633 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_7_VAV_HW_Reheat.json
--rw-r--r--   0        0        0     5286 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_7a_VAV_HW_Reheat.json
--rw-r--r--   0        0        0     5670 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_7b_VAV_HW_Reheat.json
--rw-r--r--   0        0        0     5269 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_7c_VAV_HW_Reheat.json
--rw-r--r--   0        0        0     6043 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_8_PFP_Reheat.json
--rw-r--r--   0        0        0     5696 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_8a_PFP_Reheat.json
--rw-r--r--   0        0        0     6148 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_8b_PFP_Reheat.json
--rw-r--r--   0        0        0     5747 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_8c_PFP_Reheat.json
--rw-r--r--   0        0        0     2661 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_9_Warm_Air_Furnace_Gas.json
--rw-r--r--   0        0        0     2567 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_9b_Warm_Air_Furnace_Gas.json
--rw-r--r--   0        0        0   165706 2024-05-22 15:09:38.883691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types.json
--rw-r--r--   0        0        0  1886320 2024-05-22 15:09:38.887691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_zone_assignment_tcd_master.json
--rw-r--r--   0        0        0    34038 2024-05-22 15:09:38.887691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/transformer_tcd_master.json
--rw-r--r--   0        0        0    32588 2024-05-22 15:09:38.887691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/transformer_tests.json
--rw-r--r--   0        0        0     1465 2024-05-22 15:09:38.887691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/user_baseline_rmr.json
--rw-r--r--   0        0        0      138 2024-05-22 15:09:38.887691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/scripts/Pipfile
--rw-r--r--   0        0        0      453 2024-05-22 15:09:38.887691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/scripts/Pipfile.lock
--rw-r--r--   0        0        0      460 2024-05-22 15:09:38.887691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/scripts/disaggregate_master_test_json.py
--rw-r--r--   0        0        0     9756 2024-05-22 15:09:38.887691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/scripts/excel_generation_utilities.py
--rw-r--r--   0        0        0     1384 2024-05-22 15:09:38.887691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/scripts/excel_to_test_json.py
--rw-r--r--   0        0        0    44559 2024-05-22 15:09:38.887691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/scripts/excel_to_test_json_utilities.py
--rw-r--r--   0        0        0      314 2024-05-22 15:09:38.887691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/scripts/generate_rule_test_documentation.py
--rw-r--r--   0        0        0     2305 2024-05-22 15:09:38.887691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/scripts/generate_schedule_json.py
--rw-r--r--   0        0        0    21928 2024-05-22 15:09:38.887691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/scripts/json_generation_utilities.py
--rw-r--r--   0        0        0     3263 2024-05-22 15:09:38.887691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/scripts/resources/json_pointer_enumerations.json
--rw-r--r--   0        0        0   349657 2024-05-22 15:09:38.887691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/scripts/resources/schedule_library.json
--rw-r--r--   0        0        0      274 2024-05-22 15:09:38.887691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/scripts/run_json_schema_validation.py
--rw-r--r--   0        0        0     3063 2024-05-22 15:09:38.887691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_rmd_factory.py
--rw-r--r--   0        0        0     5976 2024-05-22 15:09:38.887691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/run_ruletests.py
--rw-r--r--   0        0        0      853 2024-05-22 15:09:38.887691 ruleset_checking_tool-0.2.6/rct229/ruletest_engine/tests/test_ruletest_templates.py
--rw-r--r--   0        0        0   248871 2024-05-22 15:09:38.887691 ruleset_checking_tool-0.2.6/rct229/schema/ASHRAE229.schema.json
--rw-r--r--   0        0        0    48852 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/schema/Enumerations2019ASHRAE901.schema.json
--rw-r--r--   0        0        0     4711 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/schema/Enumerations2019T24.schema.json
--rw-r--r--   0        0        0     1462 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/schema/EnumerationsRESNET.schema.json
--rw-r--r--   0        0        0    15302 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/schema/Output2019ASHRAE901.schema.json
--rw-r--r--   0        0        0    10012 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/schema/RCT_project_output_test_report.schema.json
--rw-r--r--   0        0        0    10095 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/schema/RCT_software_output_test_report.schema.json
--rw-r--r--   0        0        0        0 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/schema/__init__.py
--rw-r--r--   0        0        0      407 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/schema/config.py
--rw-r--r--   0        0        0     2079 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/schema/config_functions.py
--rw-r--r--   0        0        0     1949 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/schema/resources/unit_conventions.json
--rw-r--r--   0        0        0     7939 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/schema/resources/unit_registry.txt
--rw-r--r--   0        0        0     3229 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/schema/schema_enums.py
--rw-r--r--   0        0        0      986 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/schema/schema_store.py
--rw-r--r--   0        0        0     8332 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/schema/schema_utils.py
--rw-r--r--   0        0        0     1747 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/schema/schema_utils_test.py
--rw-r--r--   0        0        0    21025 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/schema/validate.py
--rw-r--r--   0        0        0     3863 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/schema/validate_test.py
--rw-r--r--   0        0        0     2771 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/assertions.py
--rw-r--r--   0        0        0     1117 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/assertions_test.py
--rw-r--r--   0        0        0     1719 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/compare_standard_val.py
--rw-r--r--   0        0        0      859 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/compare_standard_val_test.py
--rw-r--r--   0        0        0      214 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/file.py
--rw-r--r--   0        0        0      502 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/json_utils.py
--rw-r--r--   0        0        0      315 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/json_utils_test.py
--rw-r--r--   0        0        0     2233 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/jsonpath_utils.py
--rw-r--r--   0        0        0     1573 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/jsonpath_utils_test.py
--rw-r--r--   0        0        0      707 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/logging_config.py
--rw-r--r--   0        0        0      573 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/masks.py
--rw-r--r--   0        0        0      241 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/masks_test.py
--rw-r--r--   0        0        0     1457 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/match_lists.py
--rw-r--r--   0        0        0      794 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/match_lists_test.py
--rw-r--r--   0        0        0      517 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/natural_sort.py
--rw-r--r--   0        0        0     4526 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/pint_utils.py
--rw-r--r--   0        0        0      946 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/pint_utils_test.py
--rw-r--r--   0        0        0     1134 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/schedule_utils.py
--rw-r--r--   0        0        0     1017 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/std_comparisons.py
--rw-r--r--   0        0        0     4242 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/std_comparisons_test.py
--rw-r--r--   0        0        0     5881 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/utils/utility_functions.py
--rw-r--r--   0        0        0     6662 2024-05-22 15:09:38.891691 ruleset_checking_tool-0.2.6/rct229/web_application.py
--rw-r--r--   0        0        0    11759 1970-01-01 00:00:00.000000 ruleset_checking_tool-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1852 2024-05-29 22:20:42.722924 ruleset_checking_tool-0.2.7/LICENSE
+-rw-r--r--   0        0        0    10670 2024-05-29 22:20:42.726924 ruleset_checking_tool-0.2.7/README.md
+-rw-r--r--   0        0        0     1027 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/pyproject.toml
+-rwxr-xr-x   0        0        0       22 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/__init__.py
+-rw-r--r--   0        0        0     5960 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/cli.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/report_engine/__init__.py
+-rw-r--r--   0        0        0     5795 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/report_engine/rct_report.py
+-rw-r--r--   0        0        0     1201 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/reports/__init__.py
+-rw-r--r--   0        0        0      323 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/reports/ashrae9012019/__init__.py
+-rw-r--r--   0        0        0     4519 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/reports/ashrae9012019/ashrae901_2019_detail_report.py
+-rw-r--r--   0        0        0     3285 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/reports/ashrae9012019/ashrae901_2019_software_test_report.py
+-rw-r--r--   0        0        0     9198 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/reports/ashrae9012019/ashrae901_2019_summary_report.py
+-rw-r--r--   0        0        0      301 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/reports/general/__init__.py
+-rw-r--r--   0        0        0     2097 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/reports/general/engine_raw_output.py
+-rw-r--r--   0        0        0     3686 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/reports/general/engine_raw_summary.py
+-rw-r--r--   0        0        0     1959 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/reports/project_report.py
+-rw-r--r--   0        0        0     3293 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/reports/utils.py
+-rwxr-xr-x   0        0        0        0 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/rule_engine/__init__.py
+-rw-r--r--   0        0        0     8726 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/rule_engine/engine.py
+-rw-r--r--   0        0        0      269 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/rule_engine/memoize.py
+-rw-r--r--   0        0        0     3670 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/rule_engine/partial_rule_definition.py
+-rw-r--r--   0        0        0     1267 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/rule_engine/partial_rule_definition_test.py
+-rw-r--r--   0        0        0      184 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/rule_engine/rct_outcome_label.py
+-rw-r--r--   0        0        0    24854 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/rule_engine/rule_base.py
+-rw-r--r--   0        0        0     7043 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/rule_engine/rule_base_test.py
+-rw-r--r--   0        0        0     6759 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/rule_engine/rule_list_base.py
+-rw-r--r--   0        0        0     7106 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/rule_engine/rule_list_indexed_base.py
+-rw-r--r--   0        0        0     1932 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/rule_engine/ruleset_model_factory.py
+-rw-r--r--   0        0        0      420 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/rule_engine/rulesets.py
+-rw-r--r--   0        0        0      621 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/rule_engine/tests/test_engine.py
+-rw-r--r--   0        0        0      682 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/rule_engine/tests/test_rules.py
+-rw-r--r--   0        0        0     1480 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/rule_engine/utils.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/ruleset_functions.py
+-rw-r--r--   0        0        0     3030 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/rulesets/__init__.py
+-rw-r--r--   0        0        0     1108 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/__init__.py
+-rw-r--r--   0        0        0   316614 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ASHRAE229.9012019.extra.schema.json
+-rw-r--r--   0        0        0      442 2024-05-29 22:20:42.802924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/__init__.py
+-rw-r--r--   0        0        0     1101 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_lighting_space_type_BPF_area_type.json
+-rw-r--r--   0        0        0     5485 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_lighting_space_type_bpf_bat.json
+-rw-r--r--   0        0        0     1328 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_lighting_to_hvac_map.json
+-rw-r--r--   0        0        0     1712 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.boilers.json
+-rw-r--r--   0        0        0     3550 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.chillers.json
+-rw-r--r--   0        0        0     4304 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.climate_zone_sets.json
+-rw-r--r--   0        0        0   416731 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.construction_properties.json
+-rw-r--r--   0        0        0     6532 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.construction_sets.json
+-rw-r--r--   0        0        0     3875 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.heat_pumps.json
+-rw-r--r--   0        0        0     4376 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.heat_pumps_heating.json
+-rw-r--r--   0        0        0      322 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.heat_rejection.json
+-rw-r--r--   0        0        0    14051 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.lpd_space_type.json
+-rw-r--r--   0        0        0     7043 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.motors.json
+-rw-r--r--   0        0        0    11969 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_baseline_hvac.json
+-rw-r--r--   0        0        0    22063 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_constructions.json
+-rw-r--r--   0        0        0     5606 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_economizers.json
+-rw-r--r--   0        0        0     3222 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_heat_type.json
+-rw-r--r--   0        0        0      677 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_hvac_bldg_type.json
+-rw-r--r--   0        0        0    56059 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_interior_lighting.json
+-rw-r--r--   0        0        0     5344 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_swh_bldg_type.json
+-rw-r--r--   0        0        0     1915 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_wwr_bldg_type.json
+-rw-r--r--   0        0        0     5070 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.unitary_acs.json
+-rw-r--r--   0        0        0     5358 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.water_heaters.json
+-rw-r--r--   0        0        0     3772 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_chillers.json
+-rw-r--r--   0        0        0     3072 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_transformers.json
+-rw-r--r--   0        0        0     5760 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_space_lighting_to_hvac_map.json
+-rw-r--r--   0        0        0     1098 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_3_2.json
+-rw-r--r--   0        0        0    23223 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_4_2_1_1.json
+-rw-r--r--   0        0        0     2584 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_9_5_1.json
+-rw-r--r--   0        0        0      331 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_9_6_1.json
+-rw-r--r--   0        0        0      483 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_1_3_11.json
+-rw-r--r--   0        0        0     1639 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_5_1.json
+-rw-r--r--   0        0        0     3068 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_5_2.json
+-rw-r--r--   0        0        0     1603 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_5_3.json
+-rw-r--r--   0        0        0      541 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_5_4.json
+-rw-r--r--   0        0        0     1011 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_5_5.json
+-rw-r--r--   0        0        0     3819 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_6.json
+-rw-r--r--   0        0        0        0 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/__init__.py
+-rw-r--r--   0        0        0     6979 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/extra_schema_fns.py
+-rw-r--r--   0        0        0     9342 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/extra_schema_fns_test.py
+-rw-r--r--   0        0        0     2085 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_3_1_3_11_fns.py
+-rw-r--r--   0        0        0      711 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_3_1_3_11_fns_test.py
+-rw-r--r--   0        0        0     1681 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_3_2_fns.py
+-rw-r--r--   0        0        0     2075 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_3_2_fns_test.py
+-rw-r--r--   0        0        0     2476 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_4_2_1_1_fns.py
+-rw-r--r--   0        0        0     1713 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_4_2_1_1_fns_test.py
+-rw-r--r--   0        0        0     3167 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_8_4_4_fns.py
+-rw-r--r--   0        0        0     2733 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_8_4_4_fns_test.py
+-rw-r--r--   0        0        0     2679 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_9_5_1_fns.py
+-rw-r--r--   0        0        0     1268 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_9_5_1_fns_test.py
+-rw-r--r--   0        0        0     1188 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_9_6_1_fns.py
+-rw-r--r--   0        0        0     5914 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_9_6_1_fns_test.py
+-rw-r--r--   0        0        0     2250 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_111_fns.py
+-rw-r--r--   0        0        0     2853 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_111_fns_test.py
+-rw-r--r--   0        0        0     8357 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_4_fns.py
+-rw-r--r--   0        0        0     2991 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_4_fns_test.py
+-rw-r--r--   0        0        0     2180 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_1_fns.py
+-rw-r--r--   0        0        0     1598 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_1_fns_test.py
+-rw-r--r--   0        0        0     3548 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_2_fns.py
+-rw-r--r--   0        0        0     4270 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_2_fns_test.py
+-rw-r--r--   0        0        0     3068 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_3_fns.py
+-rw-r--r--   0        0        0     2037 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_3_fns_test.py
+-rw-r--r--   0        0        0     1466 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_4_fns.py
+-rw-r--r--   0        0        0      974 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_4_fns_test.py
+-rw-r--r--   0        0        0     2946 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_5_fns.py
+-rw-r--r--   0        0        0     1836 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_5_fns_test.py
+-rw-r--r--   0        0        0     3289 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_6_fns.py
+-rw-r--r--   0        0        0     5601 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_6_fns_test.py
+-rw-r--r--   0        0        0     9102 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_7_fns.py
+-rw-r--r--   0        0        0     1642 2024-05-29 22:20:42.806923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_7_fns_test.py
+-rw-r--r--   0        0        0     3035 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_8_fns.py
+-rw-r--r--   0        0        0     1818 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_8_fns_test.py
+-rw-r--r--   0        0        0     3002 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_9_1_fins.py
+-rw-r--r--   0        0        0      667 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_9_1_fins_test.py
+-rw-r--r--   0        0        0      495 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_lighting_space_type_BPF_area_type_map.py
+-rw-r--r--   0        0        0      767 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_lighting_space_type_BPF_area_type_map_test.py
+-rw-r--r--   0        0        0      466 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_lighting_space_type_to_bpf_bat.py
+-rw-r--r--   0        0        0     1088 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_lighting_space_type_to_bpf_bat_test.py
+-rw-r--r--   0        0        0      753 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_lighting_to_hvac_bat_map_fns.py
+-rw-r--r--   0        0        0      407 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_lighting_to_hvac_bat_map_fns_test.py
+-rw-r--r--   0        0        0     4972 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_utils.py
+-rw-r--r--   0        0        0      570 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_utils_test.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/__init__.py
+-rw-r--r--   0        0        0     2430 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/aggregate_min_OA_schedule_across_zones.py
+-rw-r--r--   0        0        0     1238 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/aggregate_min_OA_schedule_across_zones_test.py
+-rw-r--r--   0        0        0     1846 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/are_all_hvac_sys_fan_objects_autosized.py
+-rw-r--r--   0        0        0     8025 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/are_all_hvac_sys_fan_objects_autosized_test.py
+-rw-r--r--   0        0        0     2251 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_system_type_compare.py
+-rw-r--r--   0        0        0     1502 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_system_type_compare_test.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/__init__.py
+-rw-r--r--   0        0        0     2061 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_chw_loops_purcahsed_cooling.py
+-rw-r--r--   0        0        0     1078 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_cool_sources_chilled_water.py
+-rw-r--r--   0        0        0     1241 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_cool_sources_none_or_null.py
+-rw-r--r--   0        0        0     1147 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_fan_configs_parallel.py
+-rw-r--r--   0        0        0     1032 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_fans_null.py
+-rw-r--r--   0        0        0     1022 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_heat_sources_electric.py
+-rw-r--r--   0        0        0     1362 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_heat_sources_hot_water.py
+-rw-r--r--   0        0        0     1258 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_heat_sources_none_or_null.py
+-rw-r--r--   0        0        0     1980 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_heating_loops_attached_to_boiler.py
+-rw-r--r--   0        0        0     2216 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_heating_loops_purchased_heating.py
+-rw-r--r--   0        0        0     1295 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_supplies_ducted.py
+-rw-r--r--   0        0        0     1362 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_types_CAV.py
+-rw-r--r--   0        0        0     1141 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_types_CAV_with_none_equal_to_null.py
+-rw-r--r--   0        0        0     1201 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_types_VAV.py
+-rw-r--r--   0        0        0      849 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/do_all_terminals_have_one_fan.py
+-rw-r--r--   0        0        0      942 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/does_each_zone_have_only_one_terminal.py
+-rw-r--r--   0        0        0      540 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/does_hvac_system_serve_single_zone.py
+-rw-r--r--   0        0        0      898 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/get_dict_with_terminal_units_and_zones.py
+-rw-r--r--   0        0        0      924 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_cooling_type_DX.py
+-rw-r--r--   0        0        0     1260 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_cooling_type_fluid_loop.py
+-rw-r--r--   0        0        0     1050 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_cooling_type_none.py
+-rw-r--r--   0        0        0     1153 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_cooling_type_none_or_non_mechanical.py
+-rw-r--r--   0        0        0     1019 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fan_sys_CV.py
+-rw-r--r--   0        0        0     1167 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fan_sys_VSD.py
+-rw-r--r--   0        0        0     1444 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fluid_loop_attached_to_boiler.py
+-rw-r--r--   0        0        0     2193 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fluid_loop_attached_to_chiller.py
+-rw-r--r--   0        0        0     1524 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fluid_loop_purchased_CHW.py
+-rw-r--r--   0        0        0     1633 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fluid_loop_purchased_heating.py
+-rw-r--r--   0        0        0     1017 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_heating_type_elec_resistance.py
+-rw-r--r--   0        0        0     1251 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_heating_type_fluid_loop.py
+-rw-r--r--   0        0        0     1020 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_heating_type_furnace.py
+-rw-r--r--   0        0        0     1064 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_heating_type_heat_pump.py
+-rw-r--r--   0        0        0     1453 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_preheat_fluid_loop_attached_to_boiler.py
+-rw-r--r--   0        0        0     1539 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_preheat_fluid_loop_purchased_heating.py
+-rw-r--r--   0        0        0     1054 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_preheating_type_elec_resistance.py
+-rw-r--r--   0        0        0     1309 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_preheating_type_fluid_loop.py
+-rw-r--r--   0        0        0      445 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_system_multizone.py
+-rw-r--r--   0        0        0     2030 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_chw_loops_purchased_cooling.py
+-rw-r--r--   0        0        0     1677 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_cool_sources_chilled_water.py
+-rw-r--r--   0        0        0     1735 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_cool_sources_none_or_null.py
+-rw-r--r--   0        0        0     1768 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_fan_configs_parallel.py
+-rw-r--r--   0        0        0     1673 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_fans_null.py
+-rw-r--r--   0        0        0     1716 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_heat_sources_electric.py
+-rw-r--r--   0        0        0     1815 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_heat_sources_hot_water.py
+-rw-r--r--   0        0        0     1731 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_heat_sources_none_or_null.py
+-rw-r--r--   0        0        0     2209 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_heating_loops_attached_to_boiler.py
+-rw-r--r--   0        0        0     2938 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_heating_loops_purchased_heating.py
+-rw-r--r--   0        0        0     1679 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_supplies_ducted.py
+-rw-r--r--   0        0        0     2367 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_types_CAV.py
+-rw-r--r--   0        0        0     1626 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_types_VAV.py
+-rw-r--r--   0        0        0     1894 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_do_all_terminals_have_one_fan.py
+-rw-r--r--   0        0        0     2444 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_does_each_zone_have_only_one_terminal.py
+-rw-r--r--   0        0        0    12083 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_get_dict_with_terminal_units_and_zones.py
+-rw-r--r--   0        0        0     1735 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_cooling_type_DX.py
+-rw-r--r--   0        0        0     2392 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_cooling_type_fluid_loop.py
+-rw-r--r--   0        0        0     2336 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_cooling_type_none.py
+-rw-r--r--   0        0        0     2963 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_cooling_type_none_or_non_mechanical.py
+-rw-r--r--   0        0        0     2104 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fan_sys_CV.py
+-rw-r--r--   0        0        0     2123 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fan_sys_vsd.py
+-rw-r--r--   0        0        0     3147 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fluid_loop_attached_to_boiler.py
+-rw-r--r--   0        0        0     2676 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fluid_loop_attached_to_chiller.py
+-rw-r--r--   0        0        0     2552 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fluid_loop_purchased_chw.py
+-rw-r--r--   0        0        0     3146 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fluid_loop_purchased_heating.py
+-rw-r--r--   0        0        0     2471 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_heating_type_elec_resistance.py
+-rw-r--r--   0        0        0     2489 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_heating_type_fluid_loop.py
+-rw-r--r--   0        0        0     2423 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_heating_type_furnace.py
+-rw-r--r--   0        0        0     2504 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_heating_type_heat_pump.py
+-rw-r--r--   0        0        0     3243 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_preheat_fluid_loop_attached_to_boiler.py
+-rw-r--r--   0        0        0     3228 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_preheat_fluid_loop_purchased_heating.py
+-rw-r--r--   0        0        0     2489 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_preheating_type_elec_resistance.py
+-rw-r--r--   0        0        0     2504 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_preheating_type_fluid_loop.py
+-rw-r--r--   0        0        0     6516 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_test_util.py
+-rw-r--r--   0        0        0     1970 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_system_util.py
+-rw-r--r--   0        0        0     6054 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_1.py
+-rw-r--r--   0        0        0     6162 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_10.py
+-rw-r--r--   0        0        0     6129 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_11_1.py
+-rw-r--r--   0        0        0     4955 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_11_2.py
+-rw-r--r--   0        0        0     5920 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_12.py
+-rw-r--r--   0        0        0     5010 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_13.py
+-rw-r--r--   0        0        0     3930 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_1_a.py
+-rw-r--r--   0        0        0     3909 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_1_c.py
+-rw-r--r--   0        0        0     4263 2024-05-29 22:20:42.810923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_2.py
+-rw-r--r--   0        0        0     6113 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_3.py
+-rw-r--r--   0        0        0     4273 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_4.py
+-rw-r--r--   0        0        0     5629 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_5.py
+-rw-r--r--   0        0        0     5866 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_6.py
+-rw-r--r--   0        0        0     6978 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_7.py
+-rw-r--r--   0        0        0     6908 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_8.py
+-rw-r--r--   0        0        0     4599 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_9.py
+-rw-r--r--   0        0        0     3940 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_9b.py
+-rw-r--r--   0        0        0    12699 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_1.py
+-rw-r--r--   0        0        0     6708 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_10.py
+-rw-r--r--   0        0        0    20538 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_11_1.py
+-rw-r--r--   0        0        0    13207 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_11_2.py
+-rw-r--r--   0        0        0    18622 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_12.py
+-rw-r--r--   0        0        0    11871 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_13.py
+-rw-r--r--   0        0        0     3766 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_2.py
+-rw-r--r--   0        0        0    15515 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_3.py
+-rw-r--r--   0        0        0     3854 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_4.py
+-rw-r--r--   0        0        0    11711 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_5.py
+-rw-r--r--   0        0        0    11183 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_6.py
+-rw-r--r--   0        0        0    25141 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_7.py
+-rw-r--r--   0        0        0    28077 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_8.py
+-rw-r--r--   0        0        0     7117 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_9.py
+-rw-r--r--   0        0        0     4524 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/check_purchased_chw_hhw_status_dict.py
+-rw-r--r--   0        0        0    13931 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/check_purchased_chw_hhw_status_dict_test.py
+-rw-r--r--   0        0        0     3003 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/compare_schedules.py
+-rw-r--r--   0        0        0     2748 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/compare_schedules_test.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/__init__.py
+-rw-r--r--   0        0        0     6274 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1c.py
+-rw-r--r--   0        0        0    21213 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1c_test.py
+-rw-r--r--   0        0        0     5630 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1d.py
+-rw-r--r--   0        0        0     3262 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1d_test.py
+-rw-r--r--   0        0        0     2636 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1e.py
+-rw-r--r--   0        0        0     4974 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1e_test.py
+-rw-r--r--   0        0        0      850 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1f.py
+-rw-r--r--   0        0        0     1200 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1g.py
+-rw-r--r--   0        0        0     4594 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1g_test.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/__init__.py
+-rw-r--r--   0        0        0     7111 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/expected_system_type_from_table_g311a_dict.py
+-rw-r--r--   0        0        0     6567 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/expected_system_type_from_table_g311a_dict_test.py
+-rw-r--r--   0        0        0      964 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_building_lab_zones_list.py
+-rw-r--r--   0        0        0     3075 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_building_lab_zones_list_test.py
+-rw-r--r--   0        0        0     1313 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_building_total_lab_exhaust_from_zone_exhaust_fans.py
+-rw-r--r--   0        0        0     3522 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_building_total_lab_exhaust_from_zone_exhaust_fans_test.py
+-rw-r--r--   0        0        0     1103 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_computer_zones_peak_cooling_load.py
+-rw-r--r--   0        0        0     3143 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_computer_zones_peak_cooling_load_test.py
+-rw-r--r--   0        0        0     8214 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_hvac_building_area_types_and_zones_dict.py
+-rw-r--r--   0        0        0     6987 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_hvac_building_area_types_and_zones_dict_test.py
+-rw-r--r--   0        0        0     2883 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_number_of_floors.py
+-rw-r--r--   0        0        0     6540 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_number_of_floors_test.py
+-rw-r--r--   0        0        0     1457 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_predominant_hvac_building_area_type.py
+-rw-r--r--   0        0        0     5785 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_predominant_hvac_building_area_type_test.py
+-rw-r--r--   0        0        0     5972 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_eflh.py
+-rw-r--r--   0        0        0     5670 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_eflh_test.py
+-rw-r--r--   0        0        0     1552 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_hvac_bat.py
+-rw-r--r--   0        0        0     2695 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_hvac_bat_test.py
+-rw-r--r--   0        0        0     3548 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_peak_internal_load_floor_area_dict.py
+-rw-r--r--   0        0        0     7874 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_peak_internal_load_floor_area_dict_test.py
+-rw-r--r--   0        0        0     2588 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zones_computer_rooms.py
+-rw-r--r--   0        0        0     3519 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zones_computer_rooms_test.py
+-rw-r--r--   0        0        0     1094 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zones_on_same_floor_list.py
+-rw-r--r--   0        0        0     1597 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zones_on_same_floor_list_test.py
+-rw-r--r--   0        0        0     1998 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_space_a_computer_room.py
+-rw-r--r--   0        0        0     3999 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_space_a_computer_room_test.py
+-rw-r--r--   0        0        0     4077 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_likely_a_vestibule.py
+-rw-r--r--   0        0        0     5148 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_likely_a_vestibule_test.py
+-rw-r--r--   0        0        0     2909 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_mechanically_cooled.py
+-rw-r--r--   0        0        0     3681 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_mechanically_cooled_test.py
+-rw-r--r--   0        0        0     2315 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_mechanically_heated_and_not_cooled.py
+-rw-r--r--   0        0        0     6099 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_mechanically_heated_and_not_cooled_test.py
+-rw-r--r--   0        0        0     5162 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_BPF_building_area_types_and_zones.py
+-rw-r--r--   0        0        0     6302 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_BPF_building_area_types_and_zones_test.py
+-rw-r--r--   0        0        0     2840 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_aggregated_zone_hvac_fan_operating_schedule.py
+-rw-r--r--   0        0        0     4366 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_aggregated_zone_hvac_fan_operating_schedule_test.py
+-rw-r--r--   0        0        0     4078 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_area_type_window_wall_area_dict.py
+-rw-r--r--   0        0        0    28034 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_area_type_window_wall_area_dict_test.py
+-rw-r--r--   0        0        0     1220 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_avg_zone_height.py
+-rw-r--r--   0        0        0      444 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_avg_zone_height_test.py
+-rw-r--r--   0        0        0     5090 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_baseline_system_types.py
+-rw-r--r--   0        0        0    14126 2024-05-29 22:20:42.814924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_baseline_system_types_test.py
+-rw-r--r--   0        0        0     4804 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_scc_skylight_roof_ratios_dict.py
+-rw-r--r--   0        0        0    35707 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_scc_skylight_roof_ratios_dict_test.py
+-rw-r--r--   0        0        0     4652 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_scc_window_wall_ratios_dict.py
+-rw-r--r--   0        0        0     7395 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_scc_window_wall_ratios_dict_test.py
+-rw-r--r--   0        0        0     2166 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_segment_lighting_status_type_dict.py
+-rw-r--r--   0        0        0     6583 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_segment_lighting_status_type_dict_test.py
+-rw-r--r--   0        0        0     3809 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_segment_skylight_roof_areas_dict.py
+-rw-r--r--   0        0        0     7906 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_segment_skylight_roof_areas_dict_test.py
+-rw-r--r--   0        0        0     3058 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_dict_of_zones_and_terminal_units_served_by_hvac_sys.py
+-rw-r--r--   0        0        0     4529 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_dict_of_zones_and_terminal_units_served_by_hvac_sys_test.py
+-rw-r--r--   0        0        0     1645 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_dict_of_zones_hvac_sys_serving_specific_floor.py
+-rw-r--r--   0        0        0     3191 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_dict_of_zones_hvac_sys_serving_specific_floor_test.py
+-rw-r--r--   0        0        0     1905 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_fan_object_electric_power.py
+-rw-r--r--   0        0        0     9193 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_fan_object_electric_power_test.py
+-rw-r--r--   0        0        0     3172 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_fan_system_object_supply_return_exhaust_relief_total_power_flow.py
+-rw-r--r--   0        0        0     9009 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_fan_system_object_supply_return_exhaust_relief_total_power_flow_test.py
+-rw-r--r--   0        0        0     1177 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_heat_rejection_loops_connected_to_baseline_systems.py
+-rw-r--r--   0        0        0     7324 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_heat_rejection_loops_connected_to_baseline_systems_test.py
+-rw-r--r--   0        0        0     4057 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_sys_and_assoc_zones_largest_exhaust_source.py
+-rw-r--r--   0        0        0    10446 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_sys_and_assoc_zones_largest_exhaust_source_test.py
+-rw-r--r--   0        0        0     2912 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_5_6_serving_multiple_floors.py
+-rw-r--r--   0        0        0     5260 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_5_6_serving_multiple_floors_test.py
+-rw-r--r--   0        0        0     2652 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_primarily_serving_comp_room.py
+-rw-r--r--   0        0        0     4313 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_primarily_serving_comp_room_test.py
+-rw-r--r--   0        0        0     3178 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_serving_zone_health_safety_vent_reqs.py
+-rw-r--r--   0        0        0     4161 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_serving_zone_health_safety_vent_reqs_test.py
+-rw-r--r--   0        0        0     3523 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_zone_list_w_area_dict.py
+-rw-r--r--   0        0        0     3100 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_zone_list_w_area_dict_test.py
+-rw-r--r--   0        0        0     4605 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hw_loop_zone_list_w_area_dict.py
+-rw-r--r--   0        0        0    10193 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hw_loop_zone_list_w_area_dict_test.py
+-rw-r--r--   0        0        0     2653 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_lab_zone_hvac_systems.py
+-rw-r--r--   0        0        0    24709 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_lab_zone_hvac_systems_test.py
+-rw-r--r--   0        0        0     1055 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_list_hvac_systems_associated_with_zone.py
+-rw-r--r--   0        0        0     2114 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_list_hvac_systems_associated_with_zone_test.py
+-rw-r--r--   0        0        0     3824 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_min_oa_cfm_sch_zone.py
+-rw-r--r--   0        0        0     3851 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_min_oa_cfm_sch_zone_test.py
+-rw-r--r--   0        0        0     1691 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_most_used_weekday_hourly_schedule.py
+-rw-r--r--   0        0        0     3621 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_most_used_weekday_hourly_schedule_test.py
+-rw-r--r--   0        0        0     2241 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_opaque_surface_type.py
+-rw-r--r--   0        0        0     1279 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_opaque_surface_type_test.py
+-rw-r--r--   0        0        0     3261 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_primary_secondary_loops_dict.py
+-rw-r--r--   0        0        0     5591 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_primary_secondary_loops_dict_test.py
+-rw-r--r--   0        0        0     2697 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_proposed_hvac_modeled_with_virtual_cooling.py
+-rw-r--r--   0        0        0     4407 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_proposed_hvac_modeled_with_virtual_cooling_test.py
+-rw-r--r--   0        0        0     3545 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_proposed_hvac_modeled_with_virtual_heating.py
+-rw-r--r--   0        0        0     8449 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_proposed_hvac_modeled_with_virtual_heating_test.py
+-rw-r--r--   0        0        0     6402 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_surface_conditioning_category_dict.py
+-rw-r--r--   0        0        0     1546 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_BPF_BAT.py
+-rw-r--r--   0        0        0     4273 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_BPF_BAT_test.py
+-rw-r--r--   0        0        0    18860 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_conditioning_category_dict.py
+-rw-r--r--   0        0        0    38896 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_conditioning_category_dict_test.py
+-rw-r--r--   0        0        0     3444 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_peak_internal_load_floor_area_dict.py
+-rw-r--r--   0        0        0     7838 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_peak_internal_load_floor_area_dict_test.py
+-rw-r--r--   0        0        0     8606 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_supply_return_exhaust_relief_terminal_fan_power_dict.py
+-rw-r--r--   0        0        0    16330 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_supply_return_exhaust_relief_terminal_fan_power_dict_test.py
+-rw-r--r--   0        0        0     9236 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_target_baseline_system.py
+-rw-r--r--   0        0        0    36803 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_target_baseline_system_test.py
+-rw-r--r--   0        0        0      881 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/is_cz_0_to_3a_bool.py
+-rw-r--r--   0        0        0     1951 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/is_economizer_modeled_in_proposed.py
+-rw-r--r--   0        0        0     9547 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/is_economizer_modeled_in_proposed_test.py
+-rw-r--r--   0        0        0     5298 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/normalize_interior_lighting_schedules.py
+-rw-r--r--   0        0        0     5071 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/normalize_interior_lighting_schedules_test.py
+-rw-r--r--   0        0        0      452 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section1/__init__.py
+-rw-r--r--   0        0        0     5946 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section1/section1rule1.py
+-rw-r--r--   0        0        0     4518 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section1/section1rule2.py
+-rw-r--r--   0        0        0     5681 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section1/section1rule3.py
+-rw-r--r--   0        0        0     3341 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section1/section1rule4.py
+-rw-r--r--   0        0        0     7317 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section1/section1rule5.py
+-rw-r--r--   0        0        0     1951 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section1/section1rule6.py
+-rw-r--r--   0        0        0     1986 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section1/section1rule7.py
+-rw-r--r--   0        0        0      350 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section10/__init__.py
+-rw-r--r--   0        0        0    22013 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section10/section10rule14.py
+-rw-r--r--   0        0        0    12015 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section10/section10rule7.py
+-rw-r--r--   0        0        0      371 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section12/__init__.py
+-rw-r--r--   0        0        0     1931 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section12/section12rule1.py
+-rw-r--r--   0        0        0     1929 2024-05-29 22:20:42.818924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section12/section12rule2.py
+-rw-r--r--   0        0        0     2432 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section12/section12rule3.py
+-rw-r--r--   0        0        0      437 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section15/__init__.py
+-rw-r--r--   0        0        0     1264 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section15/section15rule1.py
+-rw-r--r--   0        0        0     1262 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section15/section15rule2.py
+-rw-r--r--   0        0        0     1865 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section15/section15rule3.py
+-rw-r--r--   0        0        0     1964 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section15/section15rule4.py
+-rw-r--r--   0        0        0     3825 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section15/section15rule5.py
+-rw-r--r--   0        0        0     2943 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section15/section15rule6.py
+-rw-r--r--   0        0        0      371 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section18/__init__.py
+-rw-r--r--   0        0        0    11675 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section18/section18rule1.py
+-rw-r--r--   0        0        0    17207 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section18/section18rule2.py
+-rw-r--r--   0        0        0     2832 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section18/section18rule3.py
+-rw-r--r--   0        0        0     1124 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/__init__.py
+-rw-r--r--   0        0        0     7594 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule1.py
+-rw-r--r--   0        0        0    14069 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule10.py
+-rw-r--r--   0        0        0     3354 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule11.py
+-rw-r--r--   0        0        0     4168 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule12.py
+-rw-r--r--   0        0        0    12793 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule13.py
+-rw-r--r--   0        0        0    11238 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule14.py
+-rw-r--r--   0        0        0    10527 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule15.py
+-rw-r--r--   0        0        0     6898 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule16.py
+-rw-r--r--   0        0        0     5947 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule17.py
+-rw-r--r--   0        0        0    14589 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule18.py
+-rw-r--r--   0        0        0    13082 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule19.py
+-rw-r--r--   0        0        0     9747 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule2.py
+-rw-r--r--   0        0        0    10232 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule20.py
+-rw-r--r--   0        0        0    24073 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule21.py
+-rw-r--r--   0        0        0     2547 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule22.py
+-rw-r--r--   0        0        0    25140 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule23.py
+-rw-r--r--   0        0        0     4017 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule24.py
+-rw-r--r--   0        0        0     5445 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule25.py
+-rw-r--r--   0        0        0     4208 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule26.py
+-rw-r--r--   0        0        0     4184 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule27.py
+-rw-r--r--   0        0        0     3899 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule28.py
+-rw-r--r--   0        0        0     3921 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule29.py
+-rw-r--r--   0        0        0     2549 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule3.py
+-rw-r--r--   0        0        0     3213 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule30.py
+-rw-r--r--   0        0        0     3845 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule31.py
+-rw-r--r--   0        0        0     3606 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule32.py
+-rw-r--r--   0        0        0     4298 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule33.py
+-rw-r--r--   0        0        0     5479 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule34.py
+-rw-r--r--   0        0        0    11267 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule35.py
+-rw-r--r--   0        0        0     5256 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule36.py
+-rw-r--r--   0        0        0    20009 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule4.py
+-rw-r--r--   0        0        0     3278 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule5.py
+-rw-r--r--   0        0        0     3281 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule6.py
+-rw-r--r--   0        0        0    19179 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule7.py
+-rw-r--r--   0        0        0     6145 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule8.py
+-rw-r--r--   0        0        0     4034 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule9.py
+-rw-r--r--   0        0        0      710 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/__init__.py
+-rw-r--r--   0        0        0     2602 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule1.py
+-rw-r--r--   0        0        0     5019 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule10.py
+-rw-r--r--   0        0        0     3540 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule11.py
+-rw-r--r--   0        0        0     4287 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule12.py
+-rw-r--r--   0        0        0     4145 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule13.py
+-rw-r--r--   0        0        0     2345 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule14.py
+-rw-r--r--   0        0        0     2328 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule15.py
+-rw-r--r--   0        0        0     2740 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule16.py
+-rw-r--r--   0        0        0     4835 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule17.py
+-rw-r--r--   0        0        0     3839 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule18.py
+-rw-r--r--   0        0        0     2309 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule2.py
+-rw-r--r--   0        0        0     3517 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule3.py
+-rw-r--r--   0        0        0     3176 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule4.py
+-rw-r--r--   0        0        0     7604 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule5.py
+-rw-r--r--   0        0        0     6391 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule6.py
+-rw-r--r--   0        0        0     5061 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule7.py
+-rw-r--r--   0        0        0     9095 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule8.py
+-rw-r--r--   0        0        0     4159 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule9.py
+-rw-r--r--   0        0        0     1239 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/__init__.py
+-rw-r--r--   0        0        0     4595 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule1.py
+-rw-r--r--   0        0        0     7954 2024-05-29 22:20:42.822924 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule10.py
+-rw-r--r--   0        0        0     5315 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule11.py
+-rw-r--r--   0        0        0     3712 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule12.py
+-rw-r--r--   0        0        0     3292 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule13.py
+-rw-r--r--   0        0        0     3635 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule14.py
+-rw-r--r--   0        0        0     3484 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule15.py
+-rw-r--r--   0        0        0     5261 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule16.py
+-rw-r--r--   0        0        0     6472 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule17.py
+-rw-r--r--   0        0        0     2895 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule18.py
+-rw-r--r--   0        0        0     3913 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule19.py
+-rw-r--r--   0        0        0     4597 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule2.py
+-rw-r--r--   0        0        0     4398 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule20.py
+-rw-r--r--   0        0        0     4270 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule21.py
+-rw-r--r--   0        0        0     4038 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule22.py
+-rw-r--r--   0        0        0     3130 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule23.py
+-rw-r--r--   0        0        0     4040 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule24.py
+-rw-r--r--   0        0        0     5089 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule25.py
+-rw-r--r--   0        0        0     4545 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule26.py
+-rw-r--r--   0        0        0     3256 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule27.py
+-rw-r--r--   0        0        0     3567 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule28.py
+-rw-r--r--   0        0        0     4791 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule29.py
+-rw-r--r--   0        0        0     4224 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule3.py
+-rw-r--r--   0        0        0     4139 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule30.py
+-rw-r--r--   0        0        0     3425 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule31.py
+-rw-r--r--   0        0        0     4735 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule32.py
+-rw-r--r--   0        0        0     3095 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule33.py
+-rw-r--r--   0        0        0     4022 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule34.py
+-rw-r--r--   0        0        0     2240 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule35.py
+-rw-r--r--   0        0        0     5416 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule36.py
+-rw-r--r--   0        0        0     2274 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule37.py
+-rw-r--r--   0        0        0     2304 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule38.py
+-rw-r--r--   0        0        0     2293 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule39.py
+-rw-r--r--   0        0        0     8949 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule4.py
+-rw-r--r--   0        0        0     3230 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule40.py
+-rw-r--r--   0        0        0     1441 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule41.py
+-rw-r--r--   0        0        0     4010 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule5.py
+-rw-r--r--   0        0        0     4682 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule6.py
+-rw-r--r--   0        0        0     2480 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule7.py
+-rw-r--r--   0        0        0     7284 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule8.py
+-rw-r--r--   0        0        0     5729 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule9.py
+-rw-r--r--   0        0        0      664 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/__init__.py
+-rw-r--r--   0        0        0     6509 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule1.py
+-rw-r--r--   0        0        0     4511 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule10.py
+-rw-r--r--   0        0        0     6197 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule11.py
+-rw-r--r--   0        0        0     1900 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule12.py
+-rw-r--r--   0        0        0     5456 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule13.py
+-rw-r--r--   0        0        0     5471 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule14.py
+-rw-r--r--   0        0        0     5369 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule15.py
+-rw-r--r--   0        0        0     7363 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule16.py
+-rw-r--r--   0        0        0     5020 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule2.py
+-rw-r--r--   0        0        0     4870 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule3.py
+-rw-r--r--   0        0        0     3953 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule4.py
+-rw-r--r--   0        0        0     3597 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule5.py
+-rw-r--r--   0        0        0     4840 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule6.py
+-rw-r--r--   0        0        0     4100 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule7.py
+-rw-r--r--   0        0        0     6507 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule8.py
+-rw-r--r--   0        0        0     6592 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule9.py
+-rw-r--r--   0        0        0      391 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section4/__init__.py
+-rw-r--r--   0        0        0     9893 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section4/section4rule1.py
+-rw-r--r--   0        0        0    12790 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section4/section4rule11.py
+-rw-r--r--   0        0        0     5258 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section4/section4rule14.py
+-rw-r--r--   0        0        0    12964 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section4/section4rule2.py
+-rw-r--r--   0        0        0     1255 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/archive/__init__.py
+-rw-r--r--   0        0        0     2572 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/archive/section5rule2.py
+-rw-r--r--   0        0        0     5510 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/archive/section5rule45.py
+-rw-r--r--   0        0        0    12911 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule1.py
+-rw-r--r--   0        0        0     6192 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule10.py
+-rw-r--r--   0        0        0     3855 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule11.py
+-rw-r--r--   0        0        0     6989 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule12.py
+-rw-r--r--   0        0        0     7996 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule13.py
+-rw-r--r--   0        0        0     8371 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule14.py
+-rw-r--r--   0        0        0     5670 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule15.py
+-rw-r--r--   0        0        0     8058 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule16.py
+-rw-r--r--   0        0        0     3259 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule17.py
+-rw-r--r--   0        0        0     2595 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule18.py
+-rw-r--r--   0        0        0    13122 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule19.py
+-rw-r--r--   0        0        0     2560 2024-05-29 22:20:42.826923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule2.py
+-rw-r--r--   0        0        0    12795 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule20.py
+-rw-r--r--   0        0        0     6377 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule21.py
+-rw-r--r--   0        0        0     5202 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule22.py
+-rw-r--r--   0        0        0     5354 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule23.py
+-rw-r--r--   0        0        0     5309 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule24.py
+-rw-r--r--   0        0        0     5172 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule25.py
+-rw-r--r--   0        0        0     9147 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule26.py
+-rw-r--r--   0        0        0    12014 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule27.py
+-rw-r--r--   0        0        0    10811 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule28.py
+-rw-r--r--   0        0        0     4023 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule29.py
+-rw-r--r--   0        0        0     3819 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule3.py
+-rw-r--r--   0        0        0     6214 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule30.py
+-rw-r--r--   0        0        0     4013 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule31.py
+-rw-r--r--   0        0        0     6286 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule32.py
+-rw-r--r--   0        0        0     2425 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule33.py
+-rw-r--r--   0        0        0     3346 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule34.py
+-rw-r--r--   0        0        0     5016 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule35.py
+-rw-r--r--   0        0        0     4104 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule36.py
+-rw-r--r--   0        0        0     7794 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule37.py
+-rw-r--r--   0        0        0     2636 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule38.py
+-rw-r--r--   0        0        0    11390 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule39.py
+-rw-r--r--   0        0        0     6173 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule4.py
+-rw-r--r--   0        0        0     5775 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule40.py
+-rw-r--r--   0        0        0     3778 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule5.py
+-rw-r--r--   0        0        0     6418 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule6.py
+-rw-r--r--   0        0        0     3789 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule7.py
+-rw-r--r--   0        0        0     6172 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule8.py
+-rw-r--r--   0        0        0     4145 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule9.py
+-rw-r--r--   0        0        0      494 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/archive/__init__.py
+-rw-r--r--   0        0        0     3062 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/archive/section6rule1_archive.py
+-rw-r--r--   0        0        0     6870 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/section6rule1.py
+-rw-r--r--   0        0        0     4863 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/section6rule2.py
+-rw-r--r--   0        0        0     5247 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/section6rule3.py
+-rw-r--r--   0        0        0     7707 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/section6rule4.py
+-rw-r--r--   0        0        0     8765 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/section6rule5.py
+-rw-r--r--   0        0        0     2422 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/section6rule6.py
+-rw-r--r--   0        0        0     5381 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/section6rule7.py
+-rw-r--r--   0        0        0     8400 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/section6rule8.py
+-rw-r--r--   0        0        0     9177 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/section6rule9.py
+-rw-r--r--   0        0        0    21344 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/Ruletest_JSON_Generation_Guide.md
+-rw-r--r--   0        0        0    31094 2024-05-29 22:20:42.830923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_engine.py
+-rw-r--r--   0        0        0 32998400 2024-05-29 22:20:42.870923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/airside_hvac_master.json
+-rw-r--r--   0        0        0   116907 2024-05-29 22:20:42.874923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/airside_hvac_tests.json
+-rw-r--r--   0        0        0   659490 2024-05-29 22:20:42.874923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/boiler_tcd_master.json
+-rw-r--r--   0        0        0   299816 2024-05-29 22:20:42.874923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/boiler_tests.json
+-rw-r--r--   0        0        0  1517314 2024-05-29 22:20:42.878923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/chiller_tcd_master.json
+-rw-r--r--   0        0        0   586660 2024-05-29 22:20:42.878923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/chiller_tests.json
+-rw-r--r--   0        0        0  1117107 2024-05-29 22:20:42.878923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/envelope_tcd_master.json
+-rw-r--r--   0        0        0  2205088 2024-05-29 22:20:42.894923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/envelope_tests.json
+-rw-r--r--   0        0        0 32996103 2024-05-29 22:20:42.934923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/hvac_airside_tcd_master.json
+-rw-r--r--   0        0        0 19170731 2024-05-29 22:20:42.958923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/lighting_tcd_master.json
+-rw-r--r--   0        0        0 14770206 2024-05-29 22:20:42.978923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/lighting_tests.json
+-rw-r--r--   0        0        0    80929 2024-05-29 22:20:42.978923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/receptacle_tcd_master.json
+-rw-r--r--   0        0        0    39152 2024-05-29 22:20:42.978923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/receptacle_tests.json
+-rw-r--r--   0        0        0  2292360 2024-05-29 22:20:42.986923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/ruletest_spreadsheets/chiller_tcd_master.xlsx
+-rw-r--r--   0        0        0    40737 2024-05-29 22:20:42.986923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_1.json
+-rw-r--r--   0        0        0    41538 2024-05-29 22:20:42.986923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_2.json
+-rw-r--r--   0        0        0    59369 2024-05-29 22:20:42.986923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_3.json
+-rw-r--r--   0        0        0    39462 2024-05-29 22:20:42.986923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_4.json
+-rw-r--r--   0        0        0    48906 2024-05-29 22:20:42.986923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_5.json
+-rw-r--r--   0        0        0  5891602 2024-05-29 22:20:42.998923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_6.json
+-rw-r--r--   0        0        0  5888042 2024-05-29 22:20:43.006923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_7.json
+-rw-r--r--   0        0        0    96794 2024-05-29 22:20:43.010923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section10/rule_10_14.json
+-rw-r--r--   0        0        0    30950 2024-05-29 22:20:43.010923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section10/rule_10_7.json
+-rw-r--r--   0        0        0    15260 2024-05-29 22:20:43.010923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_1.json
+-rw-r--r--   0        0        0    15254 2024-05-29 22:20:43.010923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_2.json
+-rw-r--r--   0        0        0     9368 2024-05-29 22:20:43.010923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_3.json
+-rw-r--r--   0        0        0     9372 2024-05-29 22:20:43.010923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_4.json
+-rw-r--r--   0        0        0    10785 2024-05-29 22:20:43.010923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_5.json
+-rw-r--r--   0        0        0    10278 2024-05-29 22:20:43.010923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_6.json
+-rw-r--r--   0        0        0    10624 2024-05-29 22:20:43.010923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_7.json
+-rw-r--r--   0        0        0     5995 2024-05-29 22:20:43.010923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_1.json
+-rw-r--r--   0        0        0     5989 2024-05-29 22:20:43.010923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_2.json
+-rw-r--r--   0        0        0     3660 2024-05-29 22:20:43.010923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_3.json
+-rw-r--r--   0        0        0     3664 2024-05-29 22:20:43.010923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_4.json
+-rw-r--r--   0        0        0     8796 2024-05-29 22:20:43.010923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_5.json
+-rw-r--r--   0        0        0     5944 2024-05-29 22:20:43.010923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_6.json
+-rw-r--r--   0        0        0  1524506 2024-05-29 22:20:43.010923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section18/rule_18_1.json
+-rw-r--r--   0        0        0   244279 2024-05-29 22:20:43.010923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section18/rule_18_2.json
+-rw-r--r--   0        0        0    79607 2024-05-29 22:20:43.010923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section18/rule_18_3.json
+-rw-r--r--   0        0        0    22542 2024-05-29 22:20:43.010923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_1.json
+-rw-r--r--   0        0        0   112870 2024-05-29 22:20:43.014923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_10.json
+-rw-r--r--   0        0        0    18811 2024-05-29 22:20:43.014923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_11.json
+-rw-r--r--   0        0        0    23723 2024-05-29 22:20:43.014923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_12.json
+-rw-r--r--   0        0        0    85619 2024-05-29 22:20:43.014923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_13.json
+-rw-r--r--   0        0        0    83590 2024-05-29 22:20:43.014923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_14.json
+-rw-r--r--   0        0        0    51803 2024-05-29 22:20:43.014923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_15.json
+-rw-r--r--   0        0        0    27379 2024-05-29 22:20:43.014923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_16.json
+-rw-r--r--   0        0        0    21628 2024-05-29 22:20:43.014923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_17.json
+-rw-r--r--   0        0        0    48645 2024-05-29 22:20:43.014923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_18.json
+-rw-r--r--   0        0        0    42409 2024-05-29 22:20:43.014923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_19.json
+-rw-r--r--   0        0        0    16103 2024-05-29 22:20:43.014923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_2.json
+-rw-r--r--   0        0        0    35260 2024-05-29 22:20:43.014923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_20.json
+-rw-r--r--   0        0        0  8288791 2024-05-29 22:20:43.022923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_21.json
+-rw-r--r--   0        0        0    12655 2024-05-29 22:20:43.022923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_22.json
+-rw-r--r--   0        0        0  6615439 2024-05-29 22:20:43.030923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_23.json
+-rw-r--r--   0        0        0    43490 2024-05-29 22:20:43.030923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_24.json
+-rw-r--r--   0        0        0    73936 2024-05-29 22:20:43.030923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_25.json
+-rw-r--r--   0        0        0    16507 2024-05-29 22:20:43.030923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_26.json
+-rw-r--r--   0        0        0    16456 2024-05-29 22:20:43.030923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_27.json
+-rw-r--r--   0        0        0    14210 2024-05-29 22:20:43.030923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_28.json
+-rw-r--r--   0        0        0    14161 2024-05-29 22:20:43.030923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_29.json
+-rw-r--r--   0        0        0     9836 2024-05-29 22:20:43.030923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_3.json
+-rw-r--r--   0        0        0    20090 2024-05-29 22:20:43.030923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_30.json
+-rw-r--r--   0        0        0     9875 2024-05-29 22:20:43.030923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_31.json
+-rw-r--r--   0        0        0     9843 2024-05-29 22:20:43.030923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_32.json
+-rw-r--r--   0        0        0    27391 2024-05-29 22:20:43.030923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_33.json
+-rw-r--r--   0        0        0    28337 2024-05-29 22:20:43.030923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_34.json
+-rw-r--r--   0        0        0  3154605 2024-05-29 22:20:43.034923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_35.json
+-rw-r--r--   0        0        0    31855 2024-05-29 22:20:43.034923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_36.json
+-rw-r--r--   0        0        0  5816940 2024-05-29 22:20:43.042923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_4.json
+-rw-r--r--   0        0        0    20414 2024-05-29 22:20:43.042923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_5.json
+-rw-r--r--   0        0        0    20425 2024-05-29 22:20:43.042923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_6.json
+-rw-r--r--   0        0        0  8138975 2024-05-29 22:20:43.050922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_7.json
+-rw-r--r--   0        0        0    10604 2024-05-29 22:20:43.050922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_8.json
+-rw-r--r--   0        0        0    13253 2024-05-29 22:20:43.050922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_9.json
+-rw-r--r--   0        0        0    31359 2024-05-29 22:20:43.050922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_1.json
+-rw-r--r--   0        0        0    41011 2024-05-29 22:20:43.050922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_10.json
+-rw-r--r--   0        0        0    33002 2024-05-29 22:20:43.050922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_11.json
+-rw-r--r--   0        0        0    44857 2024-05-29 22:20:43.050922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_12.json
+-rw-r--r--   0        0        0    33163 2024-05-29 22:20:43.050922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_13.json
+-rw-r--r--   0        0        0    35885 2024-05-29 22:20:43.050922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_16.json
+-rw-r--r--   0        0        0    69811 2024-05-29 22:20:43.050922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_17.json
+-rw-r--r--   0        0        0    44303 2024-05-29 22:20:43.050922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_18.json
+-rw-r--r--   0        0        0    30887 2024-05-29 22:20:43.050922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_2.json
+-rw-r--r--   0        0        0    35154 2024-05-29 22:20:43.050922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_3.json
+-rw-r--r--   0        0        0    34560 2024-05-29 22:20:43.050922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_4.json
+-rw-r--r--   0        0        0    47111 2024-05-29 22:20:43.050922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_5.json
+-rw-r--r--   0        0        0    52419 2024-05-29 22:20:43.050922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_6.json
+-rw-r--r--   0        0        0    54422 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_7.json
+-rw-r--r--   0        0        0    33612 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_8.json
+-rw-r--r--   0        0        0    31414 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_9.json
+-rw-r--r--   0        0        0    38016 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_1.json
+-rw-r--r--   0        0        0    46003 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_10.json
+-rw-r--r--   0        0        0    32354 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_11.json
+-rw-r--r--   0        0        0    43483 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_12.json
+-rw-r--r--   0        0        0    25993 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_13.json
+-rw-r--r--   0        0        0    40407 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_14.json
+-rw-r--r--   0        0        0    26350 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_15.json
+-rw-r--r--   0        0        0    50504 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_16.json
+-rw-r--r--   0        0        0    30506 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_17.json
+-rw-r--r--   0        0        0    25272 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_18.json
+-rw-r--r--   0        0        0    39459 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_19.json
+-rw-r--r--   0        0        0    38727 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_2.json
+-rw-r--r--   0        0        0    42840 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_20.json
+-rw-r--r--   0        0        0    40769 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_21.json
+-rw-r--r--   0        0        0    33361 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_22.json
+-rw-r--r--   0        0        0    47776 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_23.json
+-rw-r--r--   0        0        0    40404 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_24.json
+-rw-r--r--   0        0        0    37088 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_25.json
+-rw-r--r--   0        0        0    32602 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_26.json
+-rw-r--r--   0        0        0    34653 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_27.json
+-rw-r--r--   0        0        0    22587 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_28.json
+-rw-r--r--   0        0        0    36184 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_29.json
+-rw-r--r--   0        0        0    41205 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_3.json
+-rw-r--r--   0        0        0    34583 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_30.json
+-rw-r--r--   0        0        0    60737 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_31.json
+-rw-r--r--   0        0        0    58309 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_32.json
+-rw-r--r--   0        0        0    49199 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_33.json
+-rw-r--r--   0        0        0    38235 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_34.json
+-rw-r--r--   0        0        0    23563 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_35.json
+-rw-r--r--   0        0        0    33713 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_36.json
+-rw-r--r--   0        0        0    23345 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_37.json
+-rw-r--r--   0        0        0    23819 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_38.json
+-rw-r--r--   0        0        0    23607 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_39.json
+-rw-r--r--   0        0        0    55361 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_4.json
+-rw-r--r--   0        0        0    47740 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_40.json
+-rw-r--r--   0        0        0    23775 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_41.json
+-rw-r--r--   0        0        0    26924 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_5.json
+-rw-r--r--   0        0        0    35749 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_6.json
+-rw-r--r--   0        0        0    35575 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_7.json
+-rw-r--r--   0        0        0    38284 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_8.json
+-rw-r--r--   0        0        0    38333 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_9.json
+-rw-r--r--   0        0        0    23554 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_1.json
+-rw-r--r--   0        0        0    20738 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_10.json
+-rw-r--r--   0        0        0    18913 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_11.json
+-rw-r--r--   0        0        0    14305 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_12.json
+-rw-r--r--   0        0        0    16867 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_13.json
+-rw-r--r--   0        0        0    16920 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_14.json
+-rw-r--r--   0        0        0    16767 2024-05-29 22:20:43.054922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_15.json
+-rw-r--r--   0        0        0    17148 2024-05-29 22:20:43.058922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_16.json
+-rw-r--r--   0        0        0    25209 2024-05-29 22:20:43.058922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_2.json
+-rw-r--r--   0        0        0    26699 2024-05-29 22:20:43.058922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_3.json
+-rw-r--r--   0        0        0    22741 2024-05-29 22:20:43.058922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_4.json
+-rw-r--r--   0        0        0    29046 2024-05-29 22:20:43.058922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_5.json
+-rw-r--r--   0        0        0    14166 2024-05-29 22:20:43.058922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_6.json
+-rw-r--r--   0        0        0    12884 2024-05-29 22:20:43.058922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_7.json
+-rw-r--r--   0        0        0    23981 2024-05-29 22:20:43.058922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_8.json
+-rw-r--r--   0        0        0    19380 2024-05-29 22:20:43.058922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_9.json
+-rw-r--r--   0        0        0  2960310 2024-05-29 22:20:43.062923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section4/rule_4_1.json
+-rw-r--r--   0        0        0  2954872 2024-05-29 22:20:43.066923 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section4/rule_4_11.json
+-rw-r--r--   0        0        0   728912 2024-05-29 22:20:43.070922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section4/rule_4_14.json
+-rw-r--r--   0        0        0  2213466 2024-05-29 22:20:43.070922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section4/rule_4_2.json
+-rw-r--r--   0        0        0    74747 2024-05-29 22:20:43.070922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_17_19.json
+-rw-r--r--   0        0        0    37237 2024-05-29 22:20:43.070922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_26.json
+-rw-r--r--   0        0        0     7503 2024-05-29 22:20:43.070922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_27.json
+-rw-r--r--   0        0        0    39596 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_13_15.json
+-rw-r--r--   0        0        0     7675 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_16.json
+-rw-r--r--   0        0        0    94101 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_17_19.json
+-rw-r--r--   0        0        0    37237 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_26.json
+-rw-r--r--   0        0        0    64847 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_2_8.json
+-rw-r--r--   0        0        0    25181 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_33_44_46.json
+-rw-r--r--   0        0        0    33024 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_9_12.json
+-rw-r--r--   0        0        0     6064 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_example_tcds.json
+-rw-r--r--   0        0        0    69636 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_20_25.json
+-rw-r--r--   0        0        0    45859 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_28.json
+-rw-r--r--   0        0        0    45859 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_28_31.json
+-rw-r--r--   0        0        0   125061 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_34.json
+-rw-r--r--   0        0        0   125061 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_34_39.json
+-rw-r--r--   0        0        0    28853 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_45.json
+-rw-r--r--   0        0        0    28853 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_47.json
+-rw-r--r--   0        0        0    38501 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_49.json
+-rw-r--r--   0        0        0    73721 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_53.json
+-rw-r--r--   0        0        0     8650 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/rule_5_2.json
+-rw-r--r--   0        0        0     8578 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/rule_5_3.json
+-rw-r--r--   0        0        0    51135 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_1.json
+-rw-r--r--   0        0        0    46233 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_10.json
+-rw-r--r--   0        0        0     9687 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_11.json
+-rw-r--r--   0        0        0    46780 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_12.json
+-rw-r--r--   0        0        0    89032 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_13.json
+-rw-r--r--   0        0        0    29544 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_14.json
+-rw-r--r--   0        0        0    41570 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_15.json
+-rw-r--r--   0        0        0    29095 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_16.json
+-rw-r--r--   0        0        0    12227 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_17.json
+-rw-r--r--   0        0        0    11846 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_18.json
+-rw-r--r--   0        0        0    47969 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_19.json
+-rw-r--r--   0        0        0     8891 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_2.json
+-rw-r--r--   0        0        0    48863 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_20.json
+-rw-r--r--   0        0        0    43570 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_21.json
+-rw-r--r--   0        0        0    18438 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_22.json
+-rw-r--r--   0        0        0    10521 2024-05-29 22:20:43.074922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_23.json
+-rw-r--r--   0        0        0    21899 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_24.json
+-rw-r--r--   0        0        0    21940 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_25.json
+-rw-r--r--   0        0        0    24709 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_26.json
+-rw-r--r--   0        0        0    46494 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_27.json
+-rw-r--r--   0        0        0    18070 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_28.json
+-rw-r--r--   0        0        0     9711 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_29.json
+-rw-r--r--   0        0        0     9486 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_3.json
+-rw-r--r--   0        0        0    36872 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_30.json
+-rw-r--r--   0        0        0    10473 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_31.json
+-rw-r--r--   0        0        0    36932 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_32.json
+-rw-r--r--   0        0        0     7049 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_33.json
+-rw-r--r--   0        0        0     8255 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_34.json
+-rw-r--r--   0        0        0    50106 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_35.json
+-rw-r--r--   0        0        0    14532 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_36.json
+-rw-r--r--   0        0        0    26886 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_37.json
+-rw-r--r--   0        0        0    14749 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_38.json
+-rw-r--r--   0        0        0    23862 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_39.json
+-rw-r--r--   0        0        0    45956 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_4.json
+-rw-r--r--   0        0        0    22417 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_40.json
+-rw-r--r--   0        0        0     9641 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_5.json
+-rw-r--r--   0        0        0    46014 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_6.json
+-rw-r--r--   0        0        0     9663 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_7.json
+-rw-r--r--   0        0        0    46418 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_8.json
+-rw-r--r--   0        0        0     9649 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_9.json
+-rw-r--r--   0        0        0    32706 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_1.json
+-rw-r--r--   0        0        0    33236 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_2.json
+-rw-r--r--   0        0        0    26598 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_3.json
+-rw-r--r--   0        0        0    33889 2024-05-29 22:20:43.078922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_4.json
+-rw-r--r--   0        0        0  4357841 2024-05-29 22:20:43.090922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_5.json
+-rw-r--r--   0        0        0     6295 2024-05-29 22:20:43.090922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_6.json
+-rw-r--r--   0        0        0    23933 2024-05-29 22:20:43.090922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_7.json
+-rw-r--r--   0        0        0 10236497 2024-05-29 22:20:43.098922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_8.json
+-rw-r--r--   0        0        0  4419752 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_9.json
+-rw-r--r--   0        0        0     4463 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System 12_CAV_SZ_HW.json
+-rw-r--r--   0        0        0     4116 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System 12a_CAV_SZ_HW.json
+-rw-r--r--   0        0        0     4485 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System 12b_CAV_SZ_HW.json
+-rw-r--r--   0        0        0     3879 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System 13_CAV_SZ_ER.json
+-rw-r--r--   0        0        0     3532 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System 13a_CAV_SZ_ER.json
+-rw-r--r--   0        0        0     2163 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_10_Warm_Air_Furnace_Elec.json
+-rw-r--r--   0        0        0     3891 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.1_VAV_SZ.json
+-rw-r--r--   0        0        0     3544 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.1a_VAV_SZ.json
+-rw-r--r--   0        0        0     4497 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.1b_VAV_SZ.json
+-rw-r--r--   0        0        0     4096 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.1c_VAV_SZ.json
+-rw-r--r--   0        0        0     4475 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.2_VAV_SZ.json
+-rw-r--r--   0        0        0     4128 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.2a_VAV_SZ.json
+-rw-r--r--   0        0        0     2994 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_1_PTAC.json
+-rw-r--r--   0        0        0     2842 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_1a_PTAC.json
+-rw-r--r--   0        0        0     3017 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_1b_PTAC.json
+-rw-r--r--   0        0        0     2811 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_1c_PTAC.json
+-rw-r--r--   0        0        0     2557 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_2_PTHP.json
+-rw-r--r--   0        0        0     2815 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_3_PSZ_AC_Gas_Furnace.json
+-rw-r--r--   0        0        0     3298 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_3a_PSZ_AC_Gas_Furnace.json
+-rw-r--r--   0        0        0     3290 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_3b_PSZ_AC_Gas_Furnace.json
+-rw-r--r--   0        0        0     3676 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_3c_PSZ_AC_Gas_Furnace.json
+-rw-r--r--   0        0        0     2812 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_4_PSZ_HP.json
+-rw-r--r--   0        0        0     4659 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_5_PVAV_HW_Reheat.json
+-rw-r--r--   0        0        0     4696 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_5b_PVAV_HW_Reheat.json
+-rw-r--r--   0        0        0     4306 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_6_PVAV_Elec_Reheat.json
+-rw-r--r--   0        0        0     5174 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_6b_PVAV_Elec_Reheat.json
+-rw-r--r--   0        0        0     5633 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_7_VAV_HW_Reheat.json
+-rw-r--r--   0        0        0     5286 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_7a_VAV_HW_Reheat.json
+-rw-r--r--   0        0        0     5670 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_7b_VAV_HW_Reheat.json
+-rw-r--r--   0        0        0     5269 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_7c_VAV_HW_Reheat.json
+-rw-r--r--   0        0        0     6043 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_8_PFP_Reheat.json
+-rw-r--r--   0        0        0     5696 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_8a_PFP_Reheat.json
+-rw-r--r--   0        0        0     6148 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_8b_PFP_Reheat.json
+-rw-r--r--   0        0        0     5747 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_8c_PFP_Reheat.json
+-rw-r--r--   0        0        0     2661 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_9_Warm_Air_Furnace_Gas.json
+-rw-r--r--   0        0        0     2567 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_9b_Warm_Air_Furnace_Gas.json
+-rw-r--r--   0        0        0   165706 2024-05-29 22:20:43.106922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types.json
+-rw-r--r--   0        0        0  1886320 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_zone_assignment_tcd_master.json
+-rw-r--r--   0        0        0    34038 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/transformer_tcd_master.json
+-rw-r--r--   0        0        0    32588 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/transformer_tests.json
+-rw-r--r--   0        0        0     1465 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/user_baseline_rmr.json
+-rw-r--r--   0        0        0      138 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/scripts/Pipfile
+-rw-r--r--   0        0        0      453 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/scripts/Pipfile.lock
+-rw-r--r--   0        0        0      460 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/scripts/disaggregate_master_test_json.py
+-rw-r--r--   0        0        0     9756 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/scripts/excel_generation_utilities.py
+-rw-r--r--   0        0        0     1384 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/scripts/excel_to_test_json.py
+-rw-r--r--   0        0        0    44559 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/scripts/excel_to_test_json_utilities.py
+-rw-r--r--   0        0        0      314 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/scripts/generate_rule_test_documentation.py
+-rw-r--r--   0        0        0     2305 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/scripts/generate_schedule_json.py
+-rw-r--r--   0        0        0    21928 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/scripts/json_generation_utilities.py
+-rw-r--r--   0        0        0     3263 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/scripts/resources/json_pointer_enumerations.json
+-rw-r--r--   0        0        0   349657 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/scripts/resources/schedule_library.json
+-rw-r--r--   0        0        0      274 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/scripts/run_json_schema_validation.py
+-rw-r--r--   0        0        0     3063 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_rmd_factory.py
+-rw-r--r--   0        0        0     5976 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/run_ruletests.py
+-rw-r--r--   0        0        0      853 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/ruletest_engine/tests/test_ruletest_templates.py
+-rw-r--r--   0        0        0   248871 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/schema/ASHRAE229.schema.json
+-rw-r--r--   0        0        0    48852 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/schema/Enumerations2019ASHRAE901.schema.json
+-rw-r--r--   0        0        0     4711 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/schema/Enumerations2019T24.schema.json
+-rw-r--r--   0        0        0     1462 2024-05-29 22:20:43.110922 ruleset_checking_tool-0.2.7/rct229/schema/EnumerationsRESNET.schema.json
+-rw-r--r--   0        0        0    15302 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/schema/Output2019ASHRAE901.schema.json
+-rw-r--r--   0        0        0    10012 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/schema/RCT_project_output_test_report.schema.json
+-rw-r--r--   0        0        0    10095 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/schema/RCT_software_output_test_report.schema.json
+-rw-r--r--   0        0        0        0 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/schema/__init__.py
+-rw-r--r--   0        0        0      407 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/schema/config.py
+-rw-r--r--   0        0        0     2079 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/schema/config_functions.py
+-rw-r--r--   0        0        0     1949 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/schema/resources/unit_conventions.json
+-rw-r--r--   0        0        0     7939 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/schema/resources/unit_registry.txt
+-rw-r--r--   0        0        0     3229 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/schema/schema_enums.py
+-rw-r--r--   0        0        0      986 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/schema/schema_store.py
+-rw-r--r--   0        0        0     8332 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/schema/schema_utils.py
+-rw-r--r--   0        0        0     1747 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/schema/schema_utils_test.py
+-rw-r--r--   0        0        0    21025 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/schema/validate.py
+-rw-r--r--   0        0        0     3863 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/schema/validate_test.py
+-rw-r--r--   0        0        0     2771 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/assertions.py
+-rw-r--r--   0        0        0     1117 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/assertions_test.py
+-rw-r--r--   0        0        0     1719 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/compare_standard_val.py
+-rw-r--r--   0        0        0      859 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/compare_standard_val_test.py
+-rw-r--r--   0        0        0      214 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/file.py
+-rw-r--r--   0        0        0      502 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/json_utils.py
+-rw-r--r--   0        0        0      315 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/json_utils_test.py
+-rw-r--r--   0        0        0     2233 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/jsonpath_utils.py
+-rw-r--r--   0        0        0     1573 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/jsonpath_utils_test.py
+-rw-r--r--   0        0        0      707 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/logging_config.py
+-rw-r--r--   0        0        0      573 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/masks.py
+-rw-r--r--   0        0        0      241 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/masks_test.py
+-rw-r--r--   0        0        0     1457 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/match_lists.py
+-rw-r--r--   0        0        0      794 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/match_lists_test.py
+-rw-r--r--   0        0        0      517 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/natural_sort.py
+-rw-r--r--   0        0        0     4526 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/pint_utils.py
+-rw-r--r--   0        0        0      946 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/pint_utils_test.py
+-rw-r--r--   0        0        0     1134 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/schedule_utils.py
+-rw-r--r--   0        0        0     4201 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/std_comparisons.py
+-rw-r--r--   0        0        0     6507 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/std_comparisons_test.py
+-rw-r--r--   0        0        0     5881 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/utils/utility_functions.py
+-rw-r--r--   0        0        0     6755 2024-05-29 22:20:43.114922 ruleset_checking_tool-0.2.7/rct229/web_application.py
+-rw-r--r--   0        0        0    11759 1970-01-01 00:00:00.000000 ruleset_checking_tool-0.2.7/PKG-INFO
```

### Comparing `ruleset_checking_tool-0.2.6/LICENSE` & `ruleset_checking_tool-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/README.md` & `ruleset_checking_tool-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/pyproject.toml` & `ruleset_checking_tool-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ruleset-checking-tool"
-version = "0.2.6"
+version = "0.2.7"
 description = "PNNL ruleset checking tool"
 authors = ["Weili Xu <weili.xu@pnnl.gov>", "Charlie Holly <charlie.holly@pnnl.gov>", "Juan Gonzalez <juan.gonzalez@pnnl.gov>", "Yun Joon Jung <yunjoon.jung@pnnl.gov>", "Jiarong Xie <jiarong.xie@pnnl.gov>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rct229"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ruleset_checking_tool-0.2.6/rct229/cli.py` & `ruleset_checking_tool-0.2.7/rct229/cli.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/report_engine/rct_report.py` & `ruleset_checking_tool-0.2.7/rct229/report_engine/rct_report.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/reports/__init__.py` & `ruleset_checking_tool-0.2.7/rct229/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/reports/ashrae9012019/ashrae901_2019_detail_report.py` & `ruleset_checking_tool-0.2.7/rct229/reports/ashrae9012019/ashrae901_2019_detail_report.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/reports/ashrae9012019/ashrae901_2019_software_test_report.py` & `ruleset_checking_tool-0.2.7/rct229/reports/ashrae9012019/ashrae901_2019_software_test_report.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/reports/ashrae9012019/ashrae901_2019_summary_report.py` & `ruleset_checking_tool-0.2.7/rct229/reports/ashrae9012019/ashrae901_2019_summary_report.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/reports/general/engine_raw_output.py` & `ruleset_checking_tool-0.2.7/rct229/reports/general/engine_raw_output.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/reports/general/engine_raw_summary.py` & `ruleset_checking_tool-0.2.7/rct229/reports/general/engine_raw_summary.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/reports/project_report.py` & `ruleset_checking_tool-0.2.7/rct229/reports/project_report.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/reports/utils.py` & `ruleset_checking_tool-0.2.7/rct229/reports/utils.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rule_engine/engine.py` & `ruleset_checking_tool-0.2.7/rct229/rule_engine/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         available_rules += [
             f for f in inspect.getmembers(module[1], inspect.isfunction)
         ]
 
     return available_rules
 
 
-def evaluate_all_rules_rpd(ruleset_project_descriptions):
+def evaluate_all_rules_rpd(ruleset_project_descriptions, session_id=""):
     # Get reference to rule functions in rules model
     available_rule_definitions = rulesets.__getrules__()
     ruleset_models = get_rmd_instance()
 
     # register all ruleset model list
     rpd_rmd_map_list = []
     for rpd_json in ruleset_project_descriptions:
@@ -45,15 +45,15 @@
                 "ruleset_model_type": model_type,
                 "file_name": rpd_json["id"],
             }
             rpd_rmd_map_list.append(rpd_rmd_map)
 
     print("Processing rules...")
     rules_list = [rule_def[1]() for rule_def in available_rule_definitions]
-    report = evaluate_rules(rules_list, ruleset_models)
+    report = evaluate_rules(rules_list, ruleset_models, session_id=session_id)
     report["rpd_files"] = rpd_rmd_map_list
 
     return report
 
 
 # Functions for evaluating rules
 def evaluate_all_rules(ruleset_model_path_list):
@@ -131,26 +131,31 @@
         }
     """
 
     return evaluate_rules([rule], rmrs, test=test)
 
 
 def evaluate_rules(
-    rules_list: list, rmds: RuleSetModels, unit_system=UNIT_SYSTEM.IP, test=False
+    rules_list: list,
+    rmds: RuleSetModels,
+    unit_system=UNIT_SYSTEM.IP,
+    test=False,
+    session_id="",
 ):
     """Evaluates a list of rules against an RMDs
 
     Parameters
     ----------
     rules_list : list
         list of rule definitions
     rmds : RuleSetModels
         Object containing RPDs for ruleset evaluation
     test: Boolean
         Flag to indicate whether this run is for software testing workflow or not.
+    session_id: string
 
     Returns
     -------
     dict
         A dictionary of the form:
         {
             invalid_rmds: dict - The keys are the names of the invalid RMDs.
@@ -223,15 +228,15 @@
 
     rule_counter = 0
     # Evaluate the rules
     for rule in rules_list:
         rule_counter += 1
         if rule_counter in counting_steps:
             print(
-                f"Compliance evaluation progress: {round(rule_counter / total_num_rules * 100)}%"
+                f"Project Evaluation Session ID: #{session_id}# => Compliance evaluation progress: {round(rule_counter / total_num_rules * 100)}%"
             )
         print(f"Processing Rule {rule.id}")
         outcome = rule.evaluate(copied_rmds)
         outcomes.append(outcome)
 
     return {
         "invalid_rmrs": invalid_rmds,
```

### Comparing `ruleset_checking_tool-0.2.6/rct229/rule_engine/partial_rule_definition.py` & `ruleset_checking_tool-0.2.7/rct229/rule_engine/partial_rule_definition.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rule_engine/partial_rule_definition_test.py` & `ruleset_checking_tool-0.2.7/rct229/rule_engine/partial_rule_definition_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rule_engine/rule_base.py` & `ruleset_checking_tool-0.2.7/rct229/rule_engine/rule_base.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rule_engine/rule_base_test.py` & `ruleset_checking_tool-0.2.7/rct229/rule_engine/rule_base_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rule_engine/rule_list_base.py` & `ruleset_checking_tool-0.2.7/rct229/rule_engine/rule_list_base.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rule_engine/rule_list_indexed_base.py` & `ruleset_checking_tool-0.2.7/rct229/rule_engine/rule_list_indexed_base.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rule_engine/ruleset_model_factory.py` & `ruleset_checking_tool-0.2.7/rct229/rule_engine/ruleset_model_factory.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rule_engine/tests/test_engine.py` & `ruleset_checking_tool-0.2.7/rct229/rule_engine/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rule_engine/tests/test_rules.py` & `ruleset_checking_tool-0.2.7/rct229/rule_engine/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rule_engine/utils.py` & `ruleset_checking_tool-0.2.7/rct229/rule_engine/utils.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/__init__.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/__init__.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/__init__.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/__init__.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ASHRAE229.9012019.extra.schema.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ASHRAE229.9012019.extra.schema.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_lighting_space_type_BPF_area_type.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_lighting_space_type_BPF_area_type.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_lighting_space_type_bpf_bat.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_lighting_space_type_bpf_bat.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_lighting_to_hvac_map.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_lighting_to_hvac_map.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.boilers.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.boilers.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.chillers.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.chillers.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.climate_zone_sets.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.climate_zone_sets.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.construction_properties.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.construction_properties.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.construction_sets.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.construction_sets.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.heat_pumps.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.heat_pumps.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.heat_pumps_heating.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.heat_pumps_heating.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.lpd_space_type.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.lpd_space_type.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.motors.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.motors.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_baseline_hvac.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_baseline_hvac.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_constructions.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_constructions.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_economizers.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_economizers.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_heat_type.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_heat_type.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_hvac_bldg_type.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_hvac_bldg_type.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_interior_lighting.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_interior_lighting.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_swh_bldg_type.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_swh_bldg_type.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_wwr_bldg_type.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.prm_wwr_bldg_type.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.unitary_acs.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.unitary_acs.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.water_heaters.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_2019.water_heaters.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_chillers.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_chillers.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_transformers.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_prm_transformers.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_space_lighting_to_hvac_map.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_space_lighting_to_hvac_map.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_3_2.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_3_2.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_4_2_1_1.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_4_2_1_1.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_9_5_1.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_9_5_1.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_5_1.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_5_1.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_5_2.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_5_2.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_5_3.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_5_3.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_5_4.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_5_4.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_5_5.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_5_5.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_6.json` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data/ashrae_90_1_table_G3_6.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/extra_schema_fns.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/extra_schema_fns.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/extra_schema_fns_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/extra_schema_fns_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_3_1_3_11_fns.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_3_1_3_11_fns.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_3_1_3_11_fns_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_3_1_3_11_fns_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_3_2_fns.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_3_2_fns.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_3_2_fns_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_3_2_fns_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_4_2_1_1_fns.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_4_2_1_1_fns.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_4_2_1_1_fns_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_4_2_1_1_fns_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_8_4_4_fns.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_8_4_4_fns.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_8_4_4_fns_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_8_4_4_fns_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_9_5_1_fns.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_9_5_1_fns.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_9_5_1_fns_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_9_5_1_fns_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_9_6_1_fns.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_9_6_1_fns.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_9_6_1_fns_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_9_6_1_fns_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_111_fns.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_111_fns.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_111_fns_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_111_fns_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_4_fns.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_4_fns.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_4_fns_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_4_fns_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_1_fns.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_1_fns.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_1_fns_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_1_fns_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_2_fns.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_2_fns.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_2_fns_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_2_fns_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_3_fns.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_3_fns.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_3_fns_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_3_fns_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_4_fns.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_4_fns.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_4_fns_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_4_fns_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_5_fns.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_5_fns.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_5_fns_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_5_5_fns_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_6_fns.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_6_fns.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_6_fns_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_6_fns_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_7_fns.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_7_fns.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_7_fns_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_7_fns_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_8_fns.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_8_fns.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_8_fns_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_8_fns_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_9_1_fins.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_9_1_fins.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_G3_9_1_fins_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_G3_9_1_fins_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_lighting_space_type_BPF_area_type_map_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_lighting_space_type_BPF_area_type_map_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_lighting_space_type_to_bpf_bat_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_lighting_space_type_to_bpf_bat_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_lighting_to_hvac_bat_map_fns.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_lighting_to_hvac_bat_map_fns.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_utils.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_utils.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/data_fns/table_utils_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/data_fns/table_utils_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/aggregate_min_OA_schedule_across_zones.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/aggregate_min_OA_schedule_across_zones.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/aggregate_min_OA_schedule_across_zones_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/aggregate_min_OA_schedule_across_zones_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/are_all_hvac_sys_fan_objects_autosized.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/are_all_hvac_sys_fan_objects_autosized.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/are_all_hvac_sys_fan_objects_autosized_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/are_all_hvac_sys_fan_objects_autosized_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_system_type_compare.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_system_type_compare.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_system_type_compare_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_system_type_compare_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_chw_loops_purcahsed_cooling.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_chw_loops_purcahsed_cooling.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_cool_sources_chilled_water.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_cool_sources_chilled_water.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_cool_sources_none_or_null.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_cool_sources_none_or_null.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_fan_configs_parallel.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_fan_configs_parallel.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_fans_null.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_fans_null.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_heat_sources_electric.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_heat_sources_electric.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_heat_sources_hot_water.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_heat_sources_hot_water.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_heat_sources_none_or_null.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_heat_sources_none_or_null.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_heating_loops_attached_to_boiler.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_heating_loops_attached_to_boiler.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_heating_loops_purchased_heating.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_heating_loops_purchased_heating.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_supplies_ducted.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_supplies_ducted.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_types_CAV.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_types_CAV.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_types_CAV_with_none_equal_to_null.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_types_CAV_with_none_equal_to_null.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_types_VAV.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/are_all_terminal_types_VAV.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/do_all_terminals_have_one_fan.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/do_all_terminals_have_one_fan.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/does_each_zone_have_only_one_terminal.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/does_each_zone_have_only_one_terminal.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/does_hvac_system_serve_single_zone.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/does_hvac_system_serve_single_zone.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/get_dict_with_terminal_units_and_zones.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/get_dict_with_terminal_units_and_zones.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_cooling_type_DX.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_cooling_type_DX.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_cooling_type_fluid_loop.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_cooling_type_fluid_loop.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_cooling_type_none.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_cooling_type_none.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_cooling_type_none_or_non_mechanical.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_cooling_type_none_or_non_mechanical.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fan_sys_CV.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fan_sys_CV.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fan_sys_VSD.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fan_sys_VSD.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fluid_loop_attached_to_boiler.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fluid_loop_attached_to_boiler.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fluid_loop_attached_to_chiller.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fluid_loop_attached_to_chiller.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fluid_loop_purchased_CHW.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fluid_loop_purchased_CHW.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fluid_loop_purchased_heating.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_fluid_loop_purchased_heating.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_heating_type_elec_resistance.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_heating_type_elec_resistance.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_heating_type_fluid_loop.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_heating_type_fluid_loop.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_heating_type_furnace.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_heating_type_furnace.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_heating_type_heat_pump.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_heating_type_heat_pump.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_preheat_fluid_loop_attached_to_boiler.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_preheat_fluid_loop_attached_to_boiler.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_preheat_fluid_loop_purchased_heating.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_preheat_fluid_loop_purchased_heating.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_preheating_type_elec_resistance.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_preheating_type_elec_resistance.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_preheating_type_fluid_loop.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/is_hvac_sys_preheating_type_fluid_loop.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_chw_loops_purchased_cooling.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_chw_loops_purchased_cooling.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_cool_sources_chilled_water.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_cool_sources_chilled_water.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_cool_sources_none_or_null.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_cool_sources_none_or_null.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_fan_configs_parallel.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_fan_configs_parallel.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_fans_null.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_fans_null.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_heat_sources_electric.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_heat_sources_electric.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_heat_sources_hot_water.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_heat_sources_hot_water.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_heat_sources_none_or_null.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_heat_sources_none_or_null.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_heating_loops_attached_to_boiler.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_heating_loops_attached_to_boiler.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_heating_loops_purchased_heating.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_heating_loops_purchased_heating.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_supplies_ducted.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_supplies_ducted.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_types_CAV.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_types_CAV.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_types_VAV.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_are_all_terminal_types_VAV.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_do_all_terminals_have_one_fan.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_do_all_terminals_have_one_fan.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_does_each_zone_have_only_one_terminal.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_does_each_zone_have_only_one_terminal.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_get_dict_with_terminal_units_and_zones.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_get_dict_with_terminal_units_and_zones.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_cooling_type_DX.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_cooling_type_DX.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_cooling_type_fluid_loop.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_cooling_type_fluid_loop.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_cooling_type_none.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_cooling_type_none.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_cooling_type_none_or_non_mechanical.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_cooling_type_none_or_non_mechanical.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fan_sys_CV.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fan_sys_CV.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fan_sys_vsd.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fan_sys_vsd.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fluid_loop_attached_to_boiler.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fluid_loop_attached_to_boiler.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fluid_loop_attached_to_chiller.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fluid_loop_attached_to_chiller.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fluid_loop_purchased_chw.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fluid_loop_purchased_chw.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fluid_loop_purchased_heating.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_fluid_loop_purchased_heating.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_heating_type_elec_resistance.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_heating_type_elec_resistance.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_heating_type_fluid_loop.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_heating_type_fluid_loop.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_heating_type_furnace.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_heating_type_furnace.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_heating_type_heat_pump.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_heating_type_heat_pump.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_preheat_fluid_loop_attached_to_boiler.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_preheat_fluid_loop_attached_to_boiler.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_preheat_fluid_loop_purchased_heating.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_preheat_fluid_loop_purchased_heating.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_preheating_type_elec_resistance.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_preheating_type_elec_resistance.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_preheating_type_fluid_loop.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_sub_functions/test_is_hvac_sys_preheating_type_fluid_loop.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_test_util.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_hvac_test_util.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_system_util.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/baseline_system_util.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_1.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_1.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_10.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_10.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_11_1.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_11_1.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_11_2.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_11_2.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_12.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_12.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_13.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_13.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_1_a.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_1_a.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_1_c.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_1_c.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_2.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_2.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_3.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_3.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_4.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_4.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_5.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_5.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_6.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_6.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_7.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_7.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_8.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_8.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_9.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_9.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_9b.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/is_baseline_system_9b.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_1.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_1.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_10.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_10.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_11_1.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_11_1.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_11_2.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_11_2.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_12.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_12.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_13.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_13.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_2.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_2.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_3.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_3.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_4.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_4.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_5.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_5.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_6.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_6.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_7.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_7.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_8.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_8.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_9.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/baseline_systems/test_is_baseline_system_9.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/check_purchased_chw_hhw_status_dict.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/check_purchased_chw_hhw_status_dict.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/check_purchased_chw_hhw_status_dict_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/check_purchased_chw_hhw_status_dict_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/compare_schedules.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/compare_schedules.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/compare_schedules_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/compare_schedules_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1c.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1c.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1c_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1c_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1d.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1d.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1d_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1d_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1e.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1e.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1e_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1e_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1f.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1f.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1g.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1g.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1g_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/does_zone_meet_G3_1_1g_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/expected_system_type_from_table_g311a_dict.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/expected_system_type_from_table_g311a_dict.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/expected_system_type_from_table_g311a_dict_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/expected_system_type_from_table_g311a_dict_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_building_lab_zones_list.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_building_lab_zones_list.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_building_lab_zones_list_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_building_lab_zones_list_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_building_total_lab_exhaust_from_zone_exhaust_fans.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_building_total_lab_exhaust_from_zone_exhaust_fans.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_building_total_lab_exhaust_from_zone_exhaust_fans_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_building_total_lab_exhaust_from_zone_exhaust_fans_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_computer_zones_peak_cooling_load.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_computer_zones_peak_cooling_load.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_computer_zones_peak_cooling_load_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_computer_zones_peak_cooling_load_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_hvac_building_area_types_and_zones_dict.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_hvac_building_area_types_and_zones_dict.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_hvac_building_area_types_and_zones_dict_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_hvac_building_area_types_and_zones_dict_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_number_of_floors.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_number_of_floors.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_number_of_floors_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_number_of_floors_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_predominant_hvac_building_area_type.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_predominant_hvac_building_area_type.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_predominant_hvac_building_area_type_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_predominant_hvac_building_area_type_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_eflh.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_eflh.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_eflh_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_eflh_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_hvac_bat.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_hvac_bat.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_hvac_bat_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_hvac_bat_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_peak_internal_load_floor_area_dict.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_peak_internal_load_floor_area_dict.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_peak_internal_load_floor_area_dict_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zone_peak_internal_load_floor_area_dict_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zones_computer_rooms.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zones_computer_rooms.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zones_computer_rooms_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zones_computer_rooms_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zones_on_same_floor_list.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zones_on_same_floor_list.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zones_on_same_floor_list_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/get_zones_on_same_floor_list_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_space_a_computer_room.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_space_a_computer_room.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_space_a_computer_room_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_space_a_computer_room_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_likely_a_vestibule.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_likely_a_vestibule.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_likely_a_vestibule_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_likely_a_vestibule_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_mechanically_cooled.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_mechanically_cooled.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_mechanically_cooled_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_mechanically_cooled_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_mechanically_heated_and_not_cooled.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_mechanically_heated_and_not_cooled.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_mechanically_heated_and_not_cooled_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/g311_exceptions/g311_sub_functions/is_zone_mechanically_heated_and_not_cooled_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_BPF_building_area_types_and_zones.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_BPF_building_area_types_and_zones.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_BPF_building_area_types_and_zones_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_BPF_building_area_types_and_zones_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_aggregated_zone_hvac_fan_operating_schedule.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_aggregated_zone_hvac_fan_operating_schedule.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_aggregated_zone_hvac_fan_operating_schedule_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_aggregated_zone_hvac_fan_operating_schedule_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_area_type_window_wall_area_dict.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_area_type_window_wall_area_dict.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_area_type_window_wall_area_dict_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_area_type_window_wall_area_dict_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_avg_zone_height.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_avg_zone_height.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_baseline_system_types.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_baseline_system_types.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_baseline_system_types_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_baseline_system_types_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_scc_skylight_roof_ratios_dict.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_scc_skylight_roof_ratios_dict.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_scc_skylight_roof_ratios_dict_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_scc_skylight_roof_ratios_dict_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_scc_window_wall_ratios_dict.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_scc_window_wall_ratios_dict.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_scc_window_wall_ratios_dict_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_scc_window_wall_ratios_dict_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_segment_lighting_status_type_dict.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_segment_lighting_status_type_dict.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_segment_lighting_status_type_dict_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_segment_lighting_status_type_dict_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_segment_skylight_roof_areas_dict.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_segment_skylight_roof_areas_dict.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_segment_skylight_roof_areas_dict_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_building_segment_skylight_roof_areas_dict_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_dict_of_zones_and_terminal_units_served_by_hvac_sys.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_dict_of_zones_and_terminal_units_served_by_hvac_sys.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_dict_of_zones_and_terminal_units_served_by_hvac_sys_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_dict_of_zones_and_terminal_units_served_by_hvac_sys_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_dict_of_zones_hvac_sys_serving_specific_floor.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_dict_of_zones_hvac_sys_serving_specific_floor.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_dict_of_zones_hvac_sys_serving_specific_floor_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_dict_of_zones_hvac_sys_serving_specific_floor_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_fan_object_electric_power.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_fan_object_electric_power.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_fan_object_electric_power_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_fan_object_electric_power_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_fan_system_object_supply_return_exhaust_relief_total_power_flow.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_fan_system_object_supply_return_exhaust_relief_total_power_flow.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_fan_system_object_supply_return_exhaust_relief_total_power_flow_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_fan_system_object_supply_return_exhaust_relief_total_power_flow_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_heat_rejection_loops_connected_to_baseline_systems.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_heat_rejection_loops_connected_to_baseline_systems.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_heat_rejection_loops_connected_to_baseline_systems_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_heat_rejection_loops_connected_to_baseline_systems_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_sys_and_assoc_zones_largest_exhaust_source.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_sys_and_assoc_zones_largest_exhaust_source.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_sys_and_assoc_zones_largest_exhaust_source_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_sys_and_assoc_zones_largest_exhaust_source_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_5_6_serving_multiple_floors.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_5_6_serving_multiple_floors.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_5_6_serving_multiple_floors_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_5_6_serving_multiple_floors_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_primarily_serving_comp_room.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_primarily_serving_comp_room.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_primarily_serving_comp_room_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_primarily_serving_comp_room_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_serving_zone_health_safety_vent_reqs.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_serving_zone_health_safety_vent_reqs.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_serving_zone_health_safety_vent_reqs_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_systems_serving_zone_health_safety_vent_reqs_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_zone_list_w_area_dict.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_zone_list_w_area_dict.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_zone_list_w_area_dict_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hvac_zone_list_w_area_dict_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hw_loop_zone_list_w_area_dict.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hw_loop_zone_list_w_area_dict.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_hw_loop_zone_list_w_area_dict_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_hw_loop_zone_list_w_area_dict_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_lab_zone_hvac_systems.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_lab_zone_hvac_systems.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_lab_zone_hvac_systems_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_lab_zone_hvac_systems_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_list_hvac_systems_associated_with_zone.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_list_hvac_systems_associated_with_zone.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_list_hvac_systems_associated_with_zone_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_list_hvac_systems_associated_with_zone_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_min_oa_cfm_sch_zone.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_min_oa_cfm_sch_zone.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_min_oa_cfm_sch_zone_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_min_oa_cfm_sch_zone_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_most_used_weekday_hourly_schedule.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_most_used_weekday_hourly_schedule.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_most_used_weekday_hourly_schedule_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_most_used_weekday_hourly_schedule_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_opaque_surface_type.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_opaque_surface_type.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_opaque_surface_type_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_opaque_surface_type_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_primary_secondary_loops_dict.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_primary_secondary_loops_dict.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_primary_secondary_loops_dict_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_primary_secondary_loops_dict_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_proposed_hvac_modeled_with_virtual_cooling.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_proposed_hvac_modeled_with_virtual_cooling.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_proposed_hvac_modeled_with_virtual_cooling_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_proposed_hvac_modeled_with_virtual_cooling_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_proposed_hvac_modeled_with_virtual_heating.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_proposed_hvac_modeled_with_virtual_heating.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_proposed_hvac_modeled_with_virtual_heating_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_proposed_hvac_modeled_with_virtual_heating_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_surface_conditioning_category_dict.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_surface_conditioning_category_dict.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_BPF_BAT.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_BPF_BAT.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_BPF_BAT_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_BPF_BAT_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_conditioning_category_dict.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_conditioning_category_dict.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_conditioning_category_dict_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_conditioning_category_dict_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_peak_internal_load_floor_area_dict.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_peak_internal_load_floor_area_dict.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_peak_internal_load_floor_area_dict_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_peak_internal_load_floor_area_dict_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_supply_return_exhaust_relief_terminal_fan_power_dict.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_supply_return_exhaust_relief_terminal_fan_power_dict.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_supply_return_exhaust_relief_terminal_fan_power_dict_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_supply_return_exhaust_relief_terminal_fan_power_dict_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_target_baseline_system.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_target_baseline_system.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_target_baseline_system_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/get_zone_target_baseline_system_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/is_cz_0_to_3a_bool.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/is_cz_0_to_3a_bool.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/is_economizer_modeled_in_proposed.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/is_economizer_modeled_in_proposed.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/is_economizer_modeled_in_proposed_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/is_economizer_modeled_in_proposed_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/normalize_interior_lighting_schedules.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/normalize_interior_lighting_schedules.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/ruleset_functions/normalize_interior_lighting_schedules_test.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/ruleset_functions/normalize_interior_lighting_schedules_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section1/section1rule1.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section1/section1rule1.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section1/section1rule2.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section1/section1rule2.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section1/section1rule3.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section1/section1rule3.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section1/section1rule4.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section1/section1rule4.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section1/section1rule5.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section1/section1rule5.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section1/section1rule6.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section1/section1rule7.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 from rct229.rule_engine.rule_base import RuleDefinitionBase
+from rct229.rule_engine.rule_list_indexed_base import RuleDefinitionListIndexedBase
 from rct229.rule_engine.ruleset_model_factory import produce_ruleset_model_description
-from rct229.rulesets.ashrae9012019.data_fns.extra_schema_fns import (
-    baseline_equals_proposed,
-)
+from rct229.rulesets.ashrae9012019.data_fns.extra_schema_fns import proposed_equals_user
 
 
-class Section1Rule6(RuleDefinitionBase):
-    """Rule 6 of ASHRAE 90.1-2019 Appendix G Section 1 (Performance Calculation)"""
+class Section1Rule7(RuleDefinitionBase):
+    """Rule 7 of ASHRAE 90.1-2019 Appendix G Section 1 (Performance Calculation)"""
 
     def __init__(self):
-        super(Section1Rule6, self).__init__(
+        super(Section1Rule7, self).__init__(
             rmds_used=produce_ruleset_model_description(
-                USER=False, BASELINE_0=True, PROPOSED=True
+                USER=True, BASELINE_0=False, PROPOSED=True
             ),
-            id="1-6",
-            description="temp",
+            id="1-7",
+            description="The proposed design shall be the same as the user design for all data elements identified in the schema hosted at data.standards.ashrae {{https://github.com/open229/ruleset-model-description-schema/blob/main/docs229/ASHRAE229_extra.schema.json}}",
             ruleset_section_title="Performance Calculation",
-            standard_section="a",
+            standard_section="Table G3.1(1) Proposed Building Performance (a)",
             is_primary_rule=True,
             rmd_context="",
         )
 
     def is_applicable(self, context, data=None):
         proposed = context.PROPOSED
-        baseline = context.BASELINE_0
-        return proposed and baseline
+        user = context.USER
+        return proposed and user
 
     def get_calc_vals(self, context, data=None):
         proposed = context.PROPOSED
-        baseline = context.BASELINE_0
+        user = context.USER
         error_msg_list = []
 
-        comparison_result = baseline_equals_proposed(
-            index_context=baseline,
-            compare_context=proposed,
+        comparison_result = proposed_equals_user(
+            index_context=proposed,
+            compare_context=user,
             error_msg_list=error_msg_list,
         )
 
         return {
             "comparison_result": comparison_result,
             "error_msg_list": error_msg_list,
         }
```

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section1/section1rule7.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section12/section12rule2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 from rct229.rule_engine.rule_base import RuleDefinitionBase
 from rct229.rule_engine.rule_list_indexed_base import RuleDefinitionListIndexedBase
 from rct229.rule_engine.ruleset_model_factory import produce_ruleset_model_description
-from rct229.rulesets.ashrae9012019.data_fns.extra_schema_fns import proposed_equals_user
+from rct229.rulesets.ashrae9012019 import USER
+from rct229.utils.jsonpath_utils import find_all
 
 
-class Section1Rule7(RuleDefinitionBase):
-    """Rule 7 of ASHRAE 90.1-2019 Appendix G Section 1 (Performance Calculation)"""
+class Section12Rule2(RuleDefinitionListIndexedBase):
+    """Rule 2 of ASHRAE 90.1-2019 Appendix G Section 12 (Receptacle)"""
 
     def __init__(self):
-        super(Section1Rule7, self).__init__(
+        super(Section12Rule2, self).__init__(
             rmds_used=produce_ruleset_model_description(
                 USER=True, BASELINE_0=False, PROPOSED=True
             ),
-            id="1-7",
-            description="temp",
-            ruleset_section_title="Performance Calculation",
-            standard_section="a",
+            each_rule=Section12Rule2.BuildingRule(),
+            index_rmd=USER,
+            id="12-2",
+            description=(
+                "Number of spaces modeled in User RMD and Proposed RMD are the same"
+            ),
+            ruleset_section_title="Receptacle",
+            standard_section="Section Table G3.1-12 Modeling Requirements for the Proposed design",
             is_primary_rule=True,
-            rmd_context="",
-        )
-
-    def is_applicable(self, context, data=None):
-        proposed = context.PROPOSED
-        user = context.USER
-        return proposed and user
-
-    def get_calc_vals(self, context, data=None):
-        proposed = context.PROPOSED
-        user = context.USER
-        error_msg_list = []
-
-        comparison_result = proposed_equals_user(
-            index_context=proposed,
-            compare_context=user,
-            error_msg_list=error_msg_list,
+            rmd_context="ruleset_model_descriptions/0/buildings",
         )
 
-        return {
-            "comparison_result": comparison_result,
-            "error_msg_list": error_msg_list,
-        }
-
-    def rule_check(self, context, calc_vals=None, data=None):
-        result = calc_vals["comparison_result"]
-        return result
+    class BuildingRule(RuleDefinitionBase):
+        def __init__(self):
+            super(Section12Rule2.BuildingRule, self).__init__(
+                rmds_used=produce_ruleset_model_description(
+                    USER=True, BASELINE_0=False, PROPOSED=True
+                ),
+            )
+
+        def get_calc_vals(self, context, data=None):
+            user_spaces = find_all("$..spaces[*]", context.USER)
+            proposed_spaces = find_all("$..spaces[*]", context.PROPOSED)
+            return {
+                "num_user_spaces": len(user_spaces),
+                "num_proposed_spaces": len(proposed_spaces),
+            }
 
-    def get_fail_msg(self, context, calc_vals=None, data=None):
-        return calc_vals["error_msg_list"]
+        def rule_check(self, context, calc_vals=None, data=None):
+            return calc_vals["num_user_spaces"] == calc_vals["num_proposed_spaces"]
```

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section10/section10rule14.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section10/section10rule14.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section10/section10rule7.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section10/section10rule7.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section12/section12rule1.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section12/section12rule1.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section12/section12rule2.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section12/section12rule3.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 from rct229.rule_engine.rule_base import RuleDefinitionBase
 from rct229.rule_engine.rule_list_indexed_base import RuleDefinitionListIndexedBase
 from rct229.rule_engine.ruleset_model_factory import produce_ruleset_model_description
 from rct229.rulesets.ashrae9012019 import USER
 from rct229.utils.jsonpath_utils import find_all
 
 
-class Section12Rule2(RuleDefinitionListIndexedBase):
-    """Rule 2 of ASHRAE 90.1-2019 Appendix G Section 12 (Receptacle)"""
+class Section12Rule3(RuleDefinitionListIndexedBase):
+    """Rule 3 of ASHRAE 90.1-2019 Appendix G Section 12 (Receptacle)"""
 
     def __init__(self):
-        super(Section12Rule2, self).__init__(
+        super(Section12Rule3, self).__init__(
             rmds_used=produce_ruleset_model_description(
                 USER=True, BASELINE_0=False, PROPOSED=True
             ),
-            each_rule=Section12Rule2.BuildingRule(),
+            each_rule=Section12Rule3.BuildingRule(),
             index_rmd=USER,
-            id="12-2",
-            description=(
-                "Number of spaces modeled in User RMD and Proposed RMD are the same"
-            ),
+            id="12-3",
+            description="User RMD Space ID in Proposed RMD",
             ruleset_section_title="Receptacle",
-            standard_section="Section Table G3.1-12 Modeling Requirements for the Proposed design",
+            standard_section="Section Table G3.1-12 Receptacles: Modeling Requirements for the Proposed design",
             is_primary_rule=True,
             rmd_context="ruleset_model_descriptions/0/buildings",
         )
 
-    class BuildingRule(RuleDefinitionBase):
+    class BuildingRule(RuleDefinitionListIndexedBase):
         def __init__(self):
-            super(Section12Rule2.BuildingRule, self).__init__(
+            super(Section12Rule3.BuildingRule, self).__init__(
                 rmds_used=produce_ruleset_model_description(
                     USER=True, BASELINE_0=False, PROPOSED=True
                 ),
+                each_rule=Section12Rule3.BuildingRule.SpaceRule(),
+                index_rmd=USER,
+                list_path="$..spaces[*]",  # All spaces in the buliding
             )
 
-        def get_calc_vals(self, context, data=None):
-            user_spaces = find_all("$..spaces[*]", context.USER)
-            proposed_spaces = find_all("$..spaces[*]", context.PROPOSED)
-            return {
-                "num_user_spaces": len(user_spaces),
-                "num_proposed_spaces": len(proposed_spaces),
-            }
+        def create_data(self, context, data):
+            # Get the Proposed space id values
+            return {"proposed_space_ids": find_all("$..spaces[*].id", context.PROPOSED)}
+
+        class SpaceRule(RuleDefinitionBase):
+            def __init__(self):
+                super(Section12Rule3.BuildingRule.SpaceRule, self).__init__(
+                    # No longer need the proposed RMD
+                    rmds_used=produce_ruleset_model_description(
+                        USER=True, BASELINE_0=False, PROPOSED=False
+                    ),
+                )
+
+            def get_calc_vals(self, context, data=None):
+                return {
+                    "user_space_id": context.USER["id"],
+                }
 
-        def rule_check(self, context, calc_vals=None, data=None):
-            return calc_vals["num_user_spaces"] == calc_vals["num_proposed_spaces"]
+            def rule_check(self, context, calc_vals, data):
+                return calc_vals["user_space_id"] in data["proposed_space_ids"]
```

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section12/section12rule3.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule18.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,53 @@
-from rct229.rule_engine.rule_base import RuleDefinitionBase
+from rct229.rule_engine.partial_rule_definition import PartialRuleDefinition
 from rct229.rule_engine.rule_list_indexed_base import RuleDefinitionListIndexedBase
 from rct229.rule_engine.ruleset_model_factory import produce_ruleset_model_description
-from rct229.rulesets.ashrae9012019 import USER
-from rct229.utils.jsonpath_utils import find_all
+from rct229.rulesets.ashrae9012019 import PROPOSED
+from rct229.schema.schema_enums import SchemaEnums
 
+SUBSURFACE_DYNAMIC_GLAZING = SchemaEnums.schema_enums["SubsurfaceDynamicGlazingOptions"]
+UNDETERMINED_MSG = "SUBSURFACE INCLUDES MANUALLY CONTROLLED DYNAMIC GLAZING IN THE PROPOSED DESIGN. VERIFY THAT SHGC AND VT WERE MODELED AS THE AVERAGE OF THE MINIMUM AND MAXIMUM SHGC AND VT."
 
-class Section12Rule3(RuleDefinitionListIndexedBase):
-    """Rule 3 of ASHRAE 90.1-2019 Appendix G Section 12 (Receptacle)"""
+
+class Section5Rule18(RuleDefinitionListIndexedBase):
+    """Rule 18 of ASHRAE 90.1-2019 Appendix G Section 5 (Envelope)"""
 
     def __init__(self):
-        super(Section12Rule3, self).__init__(
+        super(Section5Rule18, self).__init__(
             rmds_used=produce_ruleset_model_description(
-                USER=True, BASELINE_0=False, PROPOSED=True
+                USER=False, BASELINE_0=False, PROPOSED=True
             ),
-            each_rule=Section12Rule3.BuildingRule(),
-            index_rmd=USER,
-            id="12-3",
-            description="User RMD Space ID in Proposed RMD",
-            ruleset_section_title="Receptacle",
-            standard_section="Section Table G3.1-12 Receptacles: Modeling Requirements for the Proposed design",
-            is_primary_rule=True,
-            rmd_context="ruleset_model_descriptions/0/buildings",
+            each_rule=Section5Rule18.SubsurfaceRule(),
+            index_rmd=PROPOSED,
+            id="5-18",
+            description="Manually controlled dynamic glazing shall use the average of the minimum and maximum SHGC and VT.",
+            ruleset_section_title="Envelope",
+            standard_section="Section G3.1-5(a)5 Building Envelope Modeling Requirements for the Proposed design",
+            is_primary_rule=False,
+            list_path="ruleset_model_descriptions[0].buildings[*].building_segments[*].zones[*].surfaces[*].subsurfaces[*]",
         )
 
-    class BuildingRule(RuleDefinitionListIndexedBase):
+    class SubsurfaceRule(PartialRuleDefinition):
         def __init__(self):
-            super(Section12Rule3.BuildingRule, self).__init__(
+            super(Section5Rule18.SubsurfaceRule, self).__init__(
                 rmds_used=produce_ruleset_model_description(
-                    USER=True, BASELINE_0=False, PROPOSED=True
+                    USER=False, BASELINE_0=False, PROPOSED=True
                 ),
-                each_rule=Section12Rule3.BuildingRule.SpaceRule(),
-                index_rmd=USER,
-                list_path="$..spaces[*]",  # All spaces in the buliding
+                required_fields={"$": ["dynamic_glazing_type"]},
+                manual_check_required_msg=UNDETERMINED_MSG,
             )
 
-        def create_data(self, context, data):
-            # Get the Proposed space id values
-            return {"proposed_space_ids": find_all("$..spaces[*].id", context.PROPOSED)}
-
-        class SpaceRule(RuleDefinitionBase):
-            def __init__(self):
-                super(Section12Rule3.BuildingRule.SpaceRule, self).__init__(
-                    # No longer need the proposed RMD
-                    rmds_used=produce_ruleset_model_description(
-                        USER=True, BASELINE_0=False, PROPOSED=False
-                    ),
-                )
-
-            def get_calc_vals(self, context, data=None):
-                return {
-                    "user_space_id": context.USER["id"],
-                }
-
-            def rule_check(self, context, calc_vals, data):
-                return calc_vals["user_space_id"] in data["proposed_space_ids"]
+        def get_calc_vals(self, context, data=None):
+            subsurface_p = context.PROPOSED
+            subsurface_dynamic_glazing_type_p = subsurface_p["dynamic_glazing_type"]
+            return {
+                "subsurface_dynamic_glazing_type_p": subsurface_dynamic_glazing_type_p
+            }
+
+        def applicability_check(self, context, calc_vals, data):
+            subsurface_dynamic_glazing_type_p = calc_vals[
+                "subsurface_dynamic_glazing_type_p"
+            ]
+            return (
+                subsurface_dynamic_glazing_type_p
+                == SUBSURFACE_DYNAMIC_GLAZING.MANUAL_DYNAMIC
+            )
```

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section15/section15rule1.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section15/section15rule1.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section15/section15rule2.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section15/section15rule2.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section15/section15rule3.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section15/section15rule3.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section15/section15rule4.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section15/section15rule4.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section15/section15rule5.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section15/section15rule5.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section15/section15rule6.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section15/section15rule6.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section18/section18rule1.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section18/section18rule1.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section18/section18rule2.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section18/section18rule2.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section18/section18rule3.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section18/section18rule3.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/__init__.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/__init__.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule1.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule1.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule10.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule10.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule11.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule11.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule12.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule12.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule13.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule13.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule14.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule14.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule15.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule15.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule16.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule16.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule17.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule17.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule18.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule18.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule19.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule19.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule2.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule2.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule20.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule20.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule21.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule21.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule22.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule22.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule23.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule23.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule24.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule24.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule25.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule25.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule26.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule26.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule27.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule27.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule28.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule28.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule29.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule29.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule3.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule3.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule30.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule30.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule31.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule31.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule32.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule32.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule33.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule33.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule34.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule34.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule35.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule35.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule36.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule36.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule4.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule4.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule5.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule5.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule6.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule6.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule7.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule7.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule8.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule8.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section19/section19rule9.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section19/section19rule9.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/__init__.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/__init__.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule1.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule1.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule10.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule10.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule11.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule11.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule12.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule12.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule13.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule13.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule14.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule14.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule15.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule15.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule16.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule16.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule17.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule17.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule18.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule18.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule2.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule2.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule3.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule3.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule4.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule4.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule5.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule5.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule6.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule6.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule7.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule7.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule8.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule8.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section21/section21rule9.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section21/section21rule9.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/__init__.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/__init__.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule1.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule1.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule10.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule10.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule11.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule11.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule12.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule12.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule13.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule13.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule14.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule14.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule15.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule15.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule16.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule16.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule17.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule17.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule18.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule18.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule19.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule19.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule2.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule2.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule20.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule20.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule21.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule21.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule22.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule22.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule23.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule23.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule24.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule24.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule25.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule25.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule26.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule26.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule27.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule27.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule28.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule28.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule29.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule29.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule3.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule3.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule30.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule30.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule31.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule31.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule32.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule32.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule33.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule33.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule34.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule34.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule35.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule35.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule36.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule36.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule37.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule37.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule38.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule38.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule39.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule39.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule4.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule4.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule40.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule40.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule41.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule41.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule5.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule5.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule6.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule6.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule7.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule7.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule8.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule8.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section22/section22rule9.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section22/section22rule9.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/__init__.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/__init__.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule1.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule1.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule10.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule10.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule11.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule11.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule12.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule12.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule13.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule13.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule14.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule14.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule15.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule15.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule16.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule16.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule2.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule2.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule3.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule3.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule4.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule4.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule5.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule5.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule6.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule6.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule7.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule7.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule8.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule8.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section23/section23rule9.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section23/section23rule9.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section4/section4rule1.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section4/section4rule1.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section4/section4rule11.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section4/section4rule11.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section4/section4rule14.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section4/section4rule14.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section4/section4rule2.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section4/section4rule2.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/__init__.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/__init__.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/archive/section5rule2.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/archive/section5rule2.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/archive/section5rule45.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/archive/section5rule45.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule1.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule1.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule10.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule10.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule11.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule11.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule12.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule12.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule13.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule13.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule14.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule14.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule15.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule15.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule16.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule16.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule17.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule17.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule19.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule19.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule2.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule2.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule20.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule20.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule21.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule21.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule22.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule22.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule23.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule23.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule24.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule24.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule25.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule25.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule26.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule26.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule27.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule27.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule28.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule28.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule29.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule29.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule3.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule3.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule30.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule30.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule31.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule31.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule32.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule32.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule33.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule33.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule34.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule34.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule35.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule35.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule36.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule36.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule37.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule37.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule38.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule38.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule39.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule39.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule4.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule4.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule40.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule40.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule5.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule5.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule6.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule6.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule7.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule7.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule8.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule8.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section5/section5rule9.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section5/section5rule9.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/archive/section6rule1_archive.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/archive/section6rule1_archive.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/section6rule1.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/section6rule1.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/section6rule2.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/section6rule2.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/section6rule3.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/section6rule3.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/section6rule4.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/section6rule4.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/section6rule5.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/section6rule5.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/section6rule6.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/section6rule6.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/section6rule7.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/section6rule7.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/section6rule8.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/section6rule8.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/rulesets/ashrae9012019/section6/section6rule9.py` & `ruleset_checking_tool-0.2.7/rct229/rulesets/ashrae9012019/section6/section6rule9.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/Ruletest_JSON_Generation_Guide.md` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/Ruletest_JSON_Generation_Guide.md`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_engine.py` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_engine.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/airside_hvac_master.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/airside_hvac_master.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/airside_hvac_tests.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/airside_hvac_tests.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/boiler_tcd_master.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/boiler_tcd_master.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/boiler_tests.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/boiler_tests.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/chiller_tcd_master.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/chiller_tcd_master.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/chiller_tests.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/chiller_tests.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/envelope_tcd_master.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/envelope_tcd_master.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/envelope_tests.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/envelope_tests.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/hvac_airside_tcd_master.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/hvac_airside_tcd_master.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/lighting_tcd_master.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/lighting_tcd_master.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/lighting_tests.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/lighting_tests.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/receptacle_tcd_master.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/receptacle_tcd_master.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/receptacle_tests.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/receptacle_tests.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/ruletest_spreadsheets/chiller_tcd_master.xlsx` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/ruletest_spreadsheets/chiller_tcd_master.xlsx`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_1.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_1.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_2.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_2.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_3.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_3.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_4.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_4.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_5.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_5.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_6.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_6.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_7.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section1/rule_1_7.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section10/rule_10_14.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section10/rule_10_14.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section10/rule_10_7.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section10/rule_10_7.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_1.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_1.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_2.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_2.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_3.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_3.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_4.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_4.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_5.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_5.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_6.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_6.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_7.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section12/rule_12_7.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_1.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_1.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_2.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_2.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_3.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_3.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_4.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_4.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_5.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_5.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_6.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section15/rule_15_6.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section18/rule_18_1.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section18/rule_18_1.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section18/rule_18_2.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section18/rule_18_2.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section18/rule_18_3.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section18/rule_18_3.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_1.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_1.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_10.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_10.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_11.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_11.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_12.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_12.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_13.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_13.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_14.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_14.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_15.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_15.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_16.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_16.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_17.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_17.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_18.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_18.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_19.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_19.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_2.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_2.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_20.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_20.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_21.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_21.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_22.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_22.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_23.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_23.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_24.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_24.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_25.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_25.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_26.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_26.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_27.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_27.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_28.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_28.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_29.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_29.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_3.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_3.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_30.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_30.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_31.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_31.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_32.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_32.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_33.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_33.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_34.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_34.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_35.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_35.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_36.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_36.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_4.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_4.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_5.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_5.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_6.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_6.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_7.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_7.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_8.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_8.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_9.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section19/rule_19_9.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_1.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_1.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_10.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_10.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_11.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_11.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_12.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_12.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_13.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_13.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_16.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_16.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_17.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_17.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_18.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_18.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_2.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_2.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_3.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_3.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_4.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_4.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_5.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_5.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_6.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_6.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_7.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_7.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_8.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_8.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_9.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section21/rule_21_9.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_1.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_1.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_10.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_10.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_11.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_11.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_12.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_12.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_13.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_13.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_14.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_14.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_15.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_15.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_16.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_16.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_17.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_17.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_18.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_18.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_19.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_19.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_2.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_2.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_20.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_20.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_21.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_21.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_22.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_22.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_23.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_23.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_24.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_24.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_25.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_25.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_26.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_26.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_27.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_27.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_28.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_28.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_29.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_29.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_3.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_3.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_30.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_30.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_31.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_31.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_32.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_32.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_33.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_33.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_34.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_34.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_35.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_35.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_36.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_36.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_37.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_37.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_38.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_38.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_39.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_39.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_4.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_4.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_40.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_40.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_41.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_41.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_5.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_5.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_6.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_6.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_7.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_7.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_8.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_8.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_9.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section22/rule_22_9.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_1.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_1.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_10.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_10.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_11.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_11.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_12.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_12.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_13.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_13.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_14.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_14.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_15.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_15.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_16.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_16.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_2.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_2.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_3.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_3.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_4.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_4.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_5.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_5.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_6.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_6.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_7.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_7.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_8.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_8.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_9.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section23/rule_23_9.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section4/rule_4_1.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section4/rule_4_1.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section4/rule_4_11.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section4/rule_4_11.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section4/rule_4_14.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section4/rule_4_14.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section4/rule_4_2.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section4/rule_4_2.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_17_19.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_17_19.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_26.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_26.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_27.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_27.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_13_15.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_13_15.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_16.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_16.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_17_19.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_17_19.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_26.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_26.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_2_8.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_2_8.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_33_44_46.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_33_44_46.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_9_12.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_5_9_12.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_example_tcds.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_example_tcds.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_20_25.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_20_25.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_28.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_28.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_28_31.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_28_31.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_34.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_34.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_34_39.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_34_39.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_45.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_45.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_47.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_47.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_49.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_49.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_53.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/envelope_tcd_5_53.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/rule_5_2.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/rule_5_2.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/rule_5_3.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/archive/rule_5_3.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_1.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_1.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_10.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_10.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_11.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_11.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_12.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_12.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_13.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_13.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_14.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_14.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_15.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_15.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_16.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_16.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_17.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_17.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_18.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_18.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_19.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_19.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_2.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_2.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_20.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_20.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_21.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_21.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_22.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_22.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_23.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_23.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_24.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_24.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_25.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_25.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_26.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_26.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_27.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_27.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_28.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_28.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_29.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_29.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_3.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_3.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_30.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_30.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_31.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_31.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_32.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_32.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_33.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_33.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_34.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_34.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_35.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_35.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_36.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_36.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_37.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_37.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_38.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_38.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_39.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_39.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_4.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_4.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_40.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_40.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_5.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_5.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_6.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_6.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_7.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_7.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_8.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_8.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_9.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section5/rule_5_9.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_1.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_1.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_2.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_2.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_3.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_3.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_4.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_4.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_5.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_5.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_6.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_6.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_7.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_7.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_8.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_8.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_9.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/section6/rule_6_9.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System 12_CAV_SZ_HW.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System 12_CAV_SZ_HW.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System 12a_CAV_SZ_HW.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System 12a_CAV_SZ_HW.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System 12b_CAV_SZ_HW.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System 12b_CAV_SZ_HW.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System 13_CAV_SZ_ER.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System 13_CAV_SZ_ER.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System 13a_CAV_SZ_ER.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System 13a_CAV_SZ_ER.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_10_Warm_Air_Furnace_Elec.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_10_Warm_Air_Furnace_Elec.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.1_VAV_SZ.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.1_VAV_SZ.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.1a_VAV_SZ.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.1a_VAV_SZ.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.1b_VAV_SZ.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.1b_VAV_SZ.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.1c_VAV_SZ.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.1c_VAV_SZ.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.2_VAV_SZ.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.2_VAV_SZ.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.2a_VAV_SZ.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_11.2a_VAV_SZ.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_1_PTAC.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_1_PTAC.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_1a_PTAC.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_1a_PTAC.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_1b_PTAC.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_1b_PTAC.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_1c_PTAC.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_1c_PTAC.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_2_PTHP.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_2_PTHP.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_3_PSZ_AC_Gas_Furnace.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_3_PSZ_AC_Gas_Furnace.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_3a_PSZ_AC_Gas_Furnace.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_3a_PSZ_AC_Gas_Furnace.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_3b_PSZ_AC_Gas_Furnace.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_3b_PSZ_AC_Gas_Furnace.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_3c_PSZ_AC_Gas_Furnace.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_3c_PSZ_AC_Gas_Furnace.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_4_PSZ_HP.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_4_PSZ_HP.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_5_PVAV_HW_Reheat.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_5_PVAV_HW_Reheat.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_5b_PVAV_HW_Reheat.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_5b_PVAV_HW_Reheat.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_6_PVAV_Elec_Reheat.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_6_PVAV_Elec_Reheat.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_6b_PVAV_Elec_Reheat.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_6b_PVAV_Elec_Reheat.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_7_VAV_HW_Reheat.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_7_VAV_HW_Reheat.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_7a_VAV_HW_Reheat.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_7a_VAV_HW_Reheat.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_7b_VAV_HW_Reheat.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_7b_VAV_HW_Reheat.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_7c_VAV_HW_Reheat.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_7c_VAV_HW_Reheat.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_8_PFP_Reheat.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_8_PFP_Reheat.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_8a_PFP_Reheat.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_8a_PFP_Reheat.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_8b_PFP_Reheat.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_8b_PFP_Reheat.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_8c_PFP_Reheat.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_8c_PFP_Reheat.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_9_Warm_Air_Furnace_Gas.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_9_Warm_Air_Furnace_Gas.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_9b_Warm_Air_Furnace_Gas.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types/System_9b_Warm_Air_Furnace_Gas.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_types.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_zone_assignment_tcd_master.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/system_zone_assignment_tcd_master.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/transformer_tcd_master.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/transformer_tcd_master.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/transformer_tests.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/transformer_tests.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/user_baseline_rmr.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/ashrae9012019/user_baseline_rmr.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/scripts/excel_generation_utilities.py` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/scripts/excel_generation_utilities.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/scripts/excel_to_test_json.py` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/scripts/excel_to_test_json.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/scripts/excel_to_test_json_utilities.py` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/scripts/excel_to_test_json_utilities.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/scripts/generate_schedule_json.py` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/scripts/generate_schedule_json.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/scripts/json_generation_utilities.py` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/scripts/json_generation_utilities.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/scripts/resources/json_pointer_enumerations.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/scripts/resources/json_pointer_enumerations.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_jsons/scripts/resources/schedule_library.json` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_jsons/scripts/resources/schedule_library.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/ruletest_rmd_factory.py` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/ruletest_rmd_factory.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/run_ruletests.py` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/run_ruletests.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/ruletest_engine/tests/test_ruletest_templates.py` & `ruleset_checking_tool-0.2.7/rct229/ruletest_engine/tests/test_ruletest_templates.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/schema/ASHRAE229.schema.json` & `ruleset_checking_tool-0.2.7/rct229/schema/ASHRAE229.schema.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/schema/Enumerations2019ASHRAE901.schema.json` & `ruleset_checking_tool-0.2.7/rct229/schema/Enumerations2019ASHRAE901.schema.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/schema/Enumerations2019T24.schema.json` & `ruleset_checking_tool-0.2.7/rct229/schema/Enumerations2019T24.schema.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/schema/EnumerationsRESNET.schema.json` & `ruleset_checking_tool-0.2.7/rct229/schema/EnumerationsRESNET.schema.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/schema/Output2019ASHRAE901.schema.json` & `ruleset_checking_tool-0.2.7/rct229/schema/Output2019ASHRAE901.schema.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/schema/RCT_project_output_test_report.schema.json` & `ruleset_checking_tool-0.2.7/rct229/schema/RCT_project_output_test_report.schema.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/schema/RCT_software_output_test_report.schema.json` & `ruleset_checking_tool-0.2.7/rct229/schema/RCT_software_output_test_report.schema.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/schema/config_functions.py` & `ruleset_checking_tool-0.2.7/rct229/schema/config_functions.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/schema/resources/unit_conventions.json` & `ruleset_checking_tool-0.2.7/rct229/schema/resources/unit_conventions.json`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/schema/resources/unit_registry.txt` & `ruleset_checking_tool-0.2.7/rct229/schema/resources/unit_registry.txt`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/schema/schema_enums.py` & `ruleset_checking_tool-0.2.7/rct229/schema/schema_enums.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/schema/schema_store.py` & `ruleset_checking_tool-0.2.7/rct229/schema/schema_store.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/schema/schema_utils.py` & `ruleset_checking_tool-0.2.7/rct229/schema/schema_utils.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/schema/schema_utils_test.py` & `ruleset_checking_tool-0.2.7/rct229/schema/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/schema/validate.py` & `ruleset_checking_tool-0.2.7/rct229/schema/validate.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/schema/validate_test.py` & `ruleset_checking_tool-0.2.7/rct229/schema/validate_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/utils/assertions.py` & `ruleset_checking_tool-0.2.7/rct229/utils/assertions.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/utils/assertions_test.py` & `ruleset_checking_tool-0.2.7/rct229/utils/assertions_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/utils/compare_standard_val.py` & `ruleset_checking_tool-0.2.7/rct229/utils/compare_standard_val.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/utils/compare_standard_val_test.py` & `ruleset_checking_tool-0.2.7/rct229/utils/compare_standard_val_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/utils/jsonpath_utils.py` & `ruleset_checking_tool-0.2.7/rct229/utils/jsonpath_utils.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/utils/jsonpath_utils_test.py` & `ruleset_checking_tool-0.2.7/rct229/utils/jsonpath_utils_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/utils/logging_config.py` & `ruleset_checking_tool-0.2.7/rct229/utils/logging_config.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/utils/masks.py` & `ruleset_checking_tool-0.2.7/rct229/utils/masks.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/utils/match_lists.py` & `ruleset_checking_tool-0.2.7/rct229/utils/match_lists.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/utils/match_lists_test.py` & `ruleset_checking_tool-0.2.7/rct229/utils/match_lists_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/utils/natural_sort.py` & `ruleset_checking_tool-0.2.7/rct229/utils/natural_sort.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/utils/pint_utils.py` & `ruleset_checking_tool-0.2.7/rct229/utils/pint_utils.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/utils/pint_utils_test.py` & `ruleset_checking_tool-0.2.7/rct229/utils/pint_utils_test.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/utils/schedule_utils.py` & `ruleset_checking_tool-0.2.7/rct229/utils/schedule_utils.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/utils/utility_functions.py` & `ruleset_checking_tool-0.2.7/rct229/utils/utility_functions.py`

 * *Files identical despite different names*

### Comparing `ruleset_checking_tool-0.2.6/rct229/web_application.py` & `ruleset_checking_tool-0.2.7/rct229/web_application.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,23 +117,26 @@
     if ruleset == RuleSet.ASHRAE9012019_RULESET:
         report_dir = generate_ashrae9012019_software_test_report(
             section, output_dir=saving_dir
         )
     return report_dir
 
 
-def run_project_evaluation(rpds, ruleset, reports=["RAW_OUTPUT"], saving_dir="./"):
+def run_project_evaluation(
+    rpds, ruleset, reports=["RAW_OUTPUT"], saving_dir="./", session_id=""
+):
     """
 
     Parameters
     ----------
     rpds: list[dict] list of dictionary
     ruleset: str ruleset key
     reports: list[str] list of strings and each string is the enum value of a report
     saving_dir: directory to save report.
+    session_id: a string representing a calculation session
 
     Returns
     -------
     report list: list of strings contain paths to the report
 
     """
     assert_(
@@ -157,15 +160,15 @@
         assert_(
             report_type in available_report_dict,
             f"Cannot find matching report type for {report_type}. Available ones are {available_report_str}.",
         )
 
     print("Test implementation of rule engine for ASHRAE Std 229 RCT.")
     print("")
-    report = evaluate_all_rules_rpd(rpds)
+    report = evaluate_all_rules_rpd(rpds, session_id)
 
     print(f"Saving reports to: {saving_dir}......")
     report_path_list = []
     for report_type in reports:
         report_module = available_report_dict[report_type]()
         report_module.generate(report, saving_dir)
         report_path_list.append(
```

### Comparing `ruleset_checking_tool-0.2.6/PKG-INFO` & `ruleset_checking_tool-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ruleset-checking-tool
-Version: 0.2.6
+Version: 0.2.7
 Summary: PNNL ruleset checking tool
 License: MIT
 Author: Weili Xu
 Author-email: weili.xu@pnnl.gov
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

