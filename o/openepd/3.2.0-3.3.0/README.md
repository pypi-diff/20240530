# Comparing `tmp/openepd-3.2.0.tar.gz` & `tmp/openepd-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openepd-3.2.0.tar", max compression
+gzip compressed data, was "openepd-3.3.0.tar", max compression
```

## Comparing `openepd-3.2.0.tar` & `openepd-3.3.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0    11357 2024-05-27 14:03:07.508798 openepd-3.2.0/LICENSE
--rw-r--r--   0        0        0     6786 2024-05-27 14:03:07.508798 openepd-3.2.0/README.md
--rw-r--r--   0        0        0     3147 2024-05-27 14:03:07.508798 openepd-3.2.0/pyproject.toml
--rw-r--r--   0        0        0      837 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/__init__.py
--rw-r--r--   0        0        0      855 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/__version__.py
--rw-r--r--   0        0        0      837 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/__init__.py
--rw-r--r--   0        0        0    21142 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/base_sync_client.py
--rw-r--r--   0        0        0      837 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/category/__init__.py
--rw-r--r--   0        0        0     1067 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/category/dto.py
--rw-r--r--   0        0        0     1588 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/category/sync_api.py
--rw-r--r--   0        0        0     8681 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/common.py
--rw-r--r--   0        0        0      837 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/dto/__init__.py
--rw-r--r--   0        0        0     1250 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/dto/base.py
--rw-r--r--   0        0        0     4705 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/dto/common.py
--rw-r--r--   0        0        0     2377 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/dto/meta.py
--rw-r--r--   0        0        0     2211 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/dto/mf.py
--rw-r--r--   0        0        0      837 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/dto/params.py
--rw-r--r--   0        0        0      837 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/epd/__init__.py
--rw-r--r--   0        0        0     5091 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/epd/dto.py
--rw-r--r--   0        0        0     4391 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/epd/sync_api.py
--rw-r--r--   0        0        0     2376 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/errors.py
--rw-r--r--   0        0        0      837 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/pcr/__init__.py
--rw-r--r--   0        0        0     1649 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/pcr/dto.py
--rw-r--r--   0        0        0     1805 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/pcr/sync_api.py
--rw-r--r--   0        0        0     2504 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/sync_client.py
--rw-r--r--   0        0        0      837 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/api/test/__init__.py
--rw-r--r--   0        0        0      837 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/bundle/__init__.py
--rw-r--r--   0        0        0     7086 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/bundle/base.py
--rw-r--r--   0        0        0     2663 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/bundle/model.py
--rw-r--r--   0        0        0     6904 2024-05-27 14:03:07.508798 openepd-3.2.0/src/openepd/bundle/reader.py
--rw-r--r--   0        0        0     8353 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/bundle/writer.py
--rw-r--r--   0        0        0      837 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/compat/__init__.py
--rw-r--r--   0        0        0     1051 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/compat/compat_functional_validators.py
--rw-r--r--   0        0        0     1363 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/compat/pydantic.py
--rw-r--r--   0        0        0      837 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/__init__.py
--rw-r--r--   0        0        0     9154 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/base.py
--rw-r--r--   0        0        0     1856 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/category.py
--rw-r--r--   0        0        0     5659 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/common.py
--rw-r--r--   0        0        0    14299 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/epd.py
--rw-r--r--   0        0        0     1918 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/factory.py
--rw-r--r--   0        0        0    17165 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/lcia.py
--rw-r--r--   0        0        0     4013 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/org.py
--rw-r--r--   0        0        0     4620 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/pcr.py
--rw-r--r--   0        0        0      862 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/README.md
--rw-r--r--   0        0        0     5176 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/__init__.py
--rw-r--r--   0        0        0     3549 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/asphalt.py
--rw-r--r--   0        0        0     2697 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/base.py
--rw-r--r--   0        0        0     9810 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/concrete.py
--rw-r--r--   0        0        0      837 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/__init__.py
--rw-r--r--   0        0        0     2230 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/accessories.py
--rw-r--r--   0        0        0     3161 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/aggregates.py
--rw-r--r--   0        0        0     2630 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/aluminium.py
--rw-r--r--   0        0        0     3369 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/asphalt.py
--rw-r--r--   0        0        0     1092 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/bulk_materials.py
--rw-r--r--   0        0        0     1172 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/cast_decks_and_underlayment.py
--rw-r--r--   0        0        0     6779 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/cladding.py
--rw-r--r--   0        0        0     2011 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/cmu.py
--rw-r--r--   0        0        0     1117 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/common.py
--rw-r--r--   0        0        0     7204 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/concrete.py
--rw-r--r--   0        0        0     2034 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/conveying_equipment.py
--rw-r--r--   0        0        0    10972 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/electrical.py
--rw-r--r--   0        0        0     2195 2024-05-27 14:03:07.512798 openepd-3.2.0/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py
--rw-r--r--   0        0        0     1040 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/electricity.py
--rw-r--r--   0        0        0    58546 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/enums.py
--rw-r--r--   0        0        0    21338 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/finishes.py
--rw-r--r--   0        0        0     3285 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/fire_and_smoke_protection.py
--rw-r--r--   0        0        0     2798 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/furnishings.py
--rw-r--r--   0        0        0     1151 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/grouting.py
--rw-r--r--   0        0        0     5320 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/manufacturing_inputs.py
--rw-r--r--   0        0        0     3286 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/masonry.py
--rw-r--r--   0        0        0     1491 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/material_handling.py
--rw-r--r--   0        0        0     9494 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/mechanical.py
--rw-r--r--   0        0        0     1834 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/mechanical_insulation.py
--rw-r--r--   0        0        0     8374 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/network_infrastructure.py
--rw-r--r--   0        0        0    19035 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/openings.py
--rw-r--r--   0        0        0     1031 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/other_electrical_equipment.py
--rw-r--r--   0        0        0     3715 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/other_materials.py
--rw-r--r--   0        0        0     4795 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/plumbing.py
--rw-r--r--   0        0        0     2529 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/precast_concrete.py
--rw-r--r--   0        0        0     3853 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/sheathing.py
--rw-r--r--   0        0        0    10118 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/steel.py
--rw-r--r--   0        0        0     8422 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/thermal_moisture_protection.py
--rw-r--r--   0        0        0     2710 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/utility_piping.py
--rw-r--r--   0        0        0     6756 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/wood.py
--rw-r--r--   0        0        0     2079 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/specs/generated/wood_joists.py
--rw-r--r--   0        0        0     1535 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/standard.py
--rw-r--r--   0        0        0      837 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/validation/__init__.py
--rw-r--r--   0        0        0     2652 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/validation/common.py
--rw-r--r--   0        0        0     1105 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/validation/numbers.py
--rw-r--r--   0        0        0     7402 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/validation/quantity.py
--rw-r--r--   0        0        0     4690 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/model/versioning.py
--rw-r--r--   0        0        0        0 2024-05-27 14:03:07.516798 openepd-3.2.0/src/openepd/py.typed
--rw-r--r--   0        0        0     7790 1970-01-01 00:00:00.000000 openepd-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-30 11:02:26.077691 openepd-3.3.0/LICENSE
+-rw-r--r--   0        0        0     6786 2024-05-30 11:02:26.077691 openepd-3.3.0/README.md
+-rw-r--r--   0        0        0     3147 2024-05-30 11:02:26.077691 openepd-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/__init__.py
+-rw-r--r--   0        0        0      855 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/__version__.py
+-rw-r--r--   0        0        0      837 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/__init__.py
+-rw-r--r--   0        0        0    21142 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/base_sync_client.py
+-rw-r--r--   0        0        0      837 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/category/__init__.py
+-rw-r--r--   0        0        0     1067 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/category/dto.py
+-rw-r--r--   0        0        0     1588 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/category/sync_api.py
+-rw-r--r--   0        0        0     8681 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/common.py
+-rw-r--r--   0        0        0      837 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/dto/__init__.py
+-rw-r--r--   0        0        0     1250 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/dto/base.py
+-rw-r--r--   0        0        0     4705 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/dto/common.py
+-rw-r--r--   0        0        0     2377 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/dto/meta.py
+-rw-r--r--   0        0        0     2211 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/dto/mf.py
+-rw-r--r--   0        0        0      837 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/dto/params.py
+-rw-r--r--   0        0        0      837 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/epd/__init__.py
+-rw-r--r--   0        0        0     5091 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/epd/dto.py
+-rw-r--r--   0        0        0     4391 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/epd/sync_api.py
+-rw-r--r--   0        0        0     2376 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/errors.py
+-rw-r--r--   0        0        0      837 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/pcr/__init__.py
+-rw-r--r--   0        0        0     1649 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/pcr/dto.py
+-rw-r--r--   0        0        0     1805 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/pcr/sync_api.py
+-rw-r--r--   0        0        0     2504 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/sync_client.py
+-rw-r--r--   0        0        0      837 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/api/test/__init__.py
+-rw-r--r--   0        0        0      837 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/bundle/__init__.py
+-rw-r--r--   0        0        0     7086 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/bundle/base.py
+-rw-r--r--   0        0        0     2663 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/bundle/model.py
+-rw-r--r--   0        0        0     6904 2024-05-30 11:02:26.077691 openepd-3.3.0/src/openepd/bundle/reader.py
+-rw-r--r--   0        0        0     8353 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/bundle/writer.py
+-rw-r--r--   0        0        0      837 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/compat/__init__.py
+-rw-r--r--   0        0        0     1051 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/compat/compat_functional_validators.py
+-rw-r--r--   0        0        0     1363 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/compat/pydantic.py
+-rw-r--r--   0        0        0      837 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/__init__.py
+-rw-r--r--   0        0        0     9154 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/base.py
+-rw-r--r--   0        0        0     1856 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/category.py
+-rw-r--r--   0        0        0     5659 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/common.py
+-rw-r--r--   0        0        0    14299 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/epd.py
+-rw-r--r--   0        0        0     1918 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/factory.py
+-rw-r--r--   0        0        0    17165 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/lcia.py
+-rw-r--r--   0        0        0     4013 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/org.py
+-rw-r--r--   0        0        0     4620 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/pcr.py
+-rw-r--r--   0        0        0      862 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/specs/README.md
+-rw-r--r--   0        0        0     5176 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/specs/__init__.py
+-rw-r--r--   0        0        0     3549 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/specs/asphalt.py
+-rw-r--r--   0        0        0     2697 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/specs/base.py
+-rw-r--r--   0        0        0     9810 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/specs/concrete.py
+-rw-r--r--   0        0        0      837 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/specs/generated/__init__.py
+-rw-r--r--   0        0        0     2230 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/specs/generated/accessories.py
+-rw-r--r--   0        0        0     3161 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/specs/generated/aggregates.py
+-rw-r--r--   0        0        0     2630 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/specs/generated/aluminium.py
+-rw-r--r--   0        0        0     3369 2024-05-30 11:02:26.081692 openepd-3.3.0/src/openepd/model/specs/generated/asphalt.py
+-rw-r--r--   0        0        0     1092 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/bulk_materials.py
+-rw-r--r--   0        0        0     1172 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/cast_decks_and_underlayment.py
+-rw-r--r--   0        0        0     6779 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/cladding.py
+-rw-r--r--   0        0        0     2011 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/cmu.py
+-rw-r--r--   0        0        0     1117 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/common.py
+-rw-r--r--   0        0        0     7204 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/concrete.py
+-rw-r--r--   0        0        0     2034 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/conveying_equipment.py
+-rw-r--r--   0        0        0    10972 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/electrical.py
+-rw-r--r--   0        0        0     2195 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py
+-rw-r--r--   0        0        0     1040 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/electricity.py
+-rw-r--r--   0        0        0    58546 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/enums.py
+-rw-r--r--   0        0        0    21338 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/finishes.py
+-rw-r--r--   0        0        0     3285 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/fire_and_smoke_protection.py
+-rw-r--r--   0        0        0     2798 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/furnishings.py
+-rw-r--r--   0        0        0     1151 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/grouting.py
+-rw-r--r--   0        0        0     5320 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/manufacturing_inputs.py
+-rw-r--r--   0        0        0     3286 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/masonry.py
+-rw-r--r--   0        0        0     1491 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/material_handling.py
+-rw-r--r--   0        0        0     9494 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/mechanical.py
+-rw-r--r--   0        0        0     1834 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/mechanical_insulation.py
+-rw-r--r--   0        0        0     8374 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/network_infrastructure.py
+-rw-r--r--   0        0        0    19035 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/openings.py
+-rw-r--r--   0        0        0     1031 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/other_electrical_equipment.py
+-rw-r--r--   0        0        0     3715 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/other_materials.py
+-rw-r--r--   0        0        0     4795 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/plumbing.py
+-rw-r--r--   0        0        0     7544 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/precast_concrete.py
+-rw-r--r--   0        0        0     3853 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/sheathing.py
+-rw-r--r--   0        0        0    10118 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/steel.py
+-rw-r--r--   0        0        0     8422 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/thermal_moisture_protection.py
+-rw-r--r--   0        0        0     2710 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/utility_piping.py
+-rw-r--r--   0        0        0     6756 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/wood.py
+-rw-r--r--   0        0        0     2079 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/specs/generated/wood_joists.py
+-rw-r--r--   0        0        0     1535 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/standard.py
+-rw-r--r--   0        0        0      837 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/validation/__init__.py
+-rw-r--r--   0        0        0     2652 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/validation/common.py
+-rw-r--r--   0        0        0     1105 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/validation/numbers.py
+-rw-r--r--   0        0        0     7402 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/validation/quantity.py
+-rw-r--r--   0        0        0     4690 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/model/versioning.py
+-rw-r--r--   0        0        0        0 2024-05-30 11:02:26.085692 openepd-3.3.0/src/openepd/py.typed
+-rw-r--r--   0        0        0     7790 1970-01-01 00:00:00.000000 openepd-3.3.0/PKG-INFO
```

### Comparing `openepd-3.2.0/LICENSE` & `openepd-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/README.md` & `openepd-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/pyproject.toml` & `openepd-3.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openepd"
-version = "3.2.0"
+version = "3.3.0"
 license = "Apache-2.0"
 description = "Python library to work with OpenEPD format"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <open-source@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/openepd"
 keywords = []
 classifiers = [
```

### Comparing `openepd-3.2.0/src/openepd/__init__.py` & `openepd-3.3.0/src/openepd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/__version__.py` & `openepd-3.3.0/src/openepd/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "3.2.0"
+VERSION = "3.3.0"
```

### Comparing `openepd-3.2.0/src/openepd/api/__init__.py` & `openepd-3.3.0/src/openepd/api/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/api/base_sync_client.py` & `openepd-3.3.0/src/openepd/api/base_sync_client.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/api/category/__init__.py` & `openepd-3.3.0/src/openepd/api/category/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/api/category/dto.py` & `openepd-3.3.0/src/openepd/api/category/dto.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/api/category/sync_api.py` & `openepd-3.3.0/src/openepd/api/category/sync_api.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/api/common.py` & `openepd-3.3.0/src/openepd/api/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/api/dto/__init__.py` & `openepd-3.3.0/src/openepd/api/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/api/dto/base.py` & `openepd-3.3.0/src/openepd/api/dto/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/api/dto/common.py` & `openepd-3.3.0/src/openepd/api/dto/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/api/dto/meta.py` & `openepd-3.3.0/src/openepd/api/dto/meta.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/api/dto/mf.py` & `openepd-3.3.0/src/openepd/api/dto/mf.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/api/dto/params.py` & `openepd-3.3.0/src/openepd/api/dto/params.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/api/epd/__init__.py` & `openepd-3.3.0/src/openepd/api/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/api/epd/dto.py` & `openepd-3.3.0/src/openepd/api/epd/dto.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/api/epd/sync_api.py` & `openepd-3.3.0/src/openepd/api/epd/sync_api.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/api/errors.py` & `openepd-3.3.0/src/openepd/api/errors.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/api/pcr/__init__.py` & `openepd-3.3.0/src/openepd/api/pcr/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/api/pcr/dto.py` & `openepd-3.3.0/src/openepd/api/pcr/dto.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/api/pcr/sync_api.py` & `openepd-3.3.0/src/openepd/api/pcr/sync_api.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/api/sync_client.py` & `openepd-3.3.0/src/openepd/api/sync_client.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/api/test/__init__.py` & `openepd-3.3.0/src/openepd/api/test/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/bundle/__init__.py` & `openepd-3.3.0/src/openepd/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/bundle/base.py` & `openepd-3.3.0/src/openepd/bundle/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/bundle/model.py` & `openepd-3.3.0/src/openepd/bundle/model.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/bundle/reader.py` & `openepd-3.3.0/src/openepd/bundle/reader.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/bundle/writer.py` & `openepd-3.3.0/src/openepd/bundle/writer.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/compat/__init__.py` & `openepd-3.3.0/src/openepd/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/compat/compat_functional_validators.py` & `openepd-3.3.0/src/openepd/compat/compat_functional_validators.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/compat/pydantic.py` & `openepd-3.3.0/src/openepd/compat/pydantic.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/__init__.py` & `openepd-3.3.0/src/openepd/model/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/base.py` & `openepd-3.3.0/src/openepd/model/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/category.py` & `openepd-3.3.0/src/openepd/model/category.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/common.py` & `openepd-3.3.0/src/openepd/model/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/epd.py` & `openepd-3.3.0/src/openepd/model/epd.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/factory.py` & `openepd-3.3.0/src/openepd/model/factory.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/lcia.py` & `openepd-3.3.0/src/openepd/model/lcia.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/org.py` & `openepd-3.3.0/src/openepd/model/org.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/pcr.py` & `openepd-3.3.0/src/openepd/model/pcr.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/README.md` & `openepd-3.3.0/src/openepd/model/specs/README.md`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/__init__.py` & `openepd-3.3.0/src/openepd/model/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/asphalt.py` & `openepd-3.3.0/src/openepd/model/specs/asphalt.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/base.py` & `openepd-3.3.0/src/openepd/model/specs/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/concrete.py` & `openepd-3.3.0/src/openepd/model/specs/concrete.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/__init__.py` & `openepd-3.3.0/src/openepd/model/specs/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/accessories.py` & `openepd-3.3.0/src/openepd/model/specs/generated/accessories.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/aggregates.py` & `openepd-3.3.0/src/openepd/model/specs/generated/aggregates.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/aluminium.py` & `openepd-3.3.0/src/openepd/model/specs/generated/aluminium.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/asphalt.py` & `openepd-3.3.0/src/openepd/model/specs/generated/asphalt.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/bulk_materials.py` & `openepd-3.3.0/src/openepd/model/specs/generated/bulk_materials.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/cast_decks_and_underlayment.py` & `openepd-3.3.0/src/openepd/model/specs/generated/cast_decks_and_underlayment.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/cladding.py` & `openepd-3.3.0/src/openepd/model/specs/generated/cladding.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/cmu.py` & `openepd-3.3.0/src/openepd/model/specs/generated/cmu.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/common.py` & `openepd-3.3.0/src/openepd/model/specs/generated/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/concrete.py` & `openepd-3.3.0/src/openepd/model/specs/generated/concrete.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/conveying_equipment.py` & `openepd-3.3.0/src/openepd/model/specs/generated/conveying_equipment.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/electrical.py` & `openepd-3.3.0/src/openepd/model/specs/generated/electrical.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py` & `openepd-3.3.0/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/electricity.py` & `openepd-3.3.0/src/openepd/model/specs/generated/electricity.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/enums.py` & `openepd-3.3.0/src/openepd/model/specs/generated/enums.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/finishes.py` & `openepd-3.3.0/src/openepd/model/specs/generated/finishes.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/fire_and_smoke_protection.py` & `openepd-3.3.0/src/openepd/model/specs/generated/fire_and_smoke_protection.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/furnishings.py` & `openepd-3.3.0/src/openepd/model/specs/generated/furnishings.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/grouting.py` & `openepd-3.3.0/src/openepd/model/specs/generated/grouting.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/manufacturing_inputs.py` & `openepd-3.3.0/src/openepd/model/specs/generated/manufacturing_inputs.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/masonry.py` & `openepd-3.3.0/src/openepd/model/specs/generated/masonry.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/material_handling.py` & `openepd-3.3.0/src/openepd/model/specs/generated/material_handling.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/mechanical.py` & `openepd-3.3.0/src/openepd/model/specs/generated/mechanical.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/mechanical_insulation.py` & `openepd-3.3.0/src/openepd/model/specs/generated/mechanical_insulation.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/network_infrastructure.py` & `openepd-3.3.0/src/openepd/model/specs/generated/network_infrastructure.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/openings.py` & `openepd-3.3.0/src/openepd/model/specs/generated/openings.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/other_electrical_equipment.py` & `openepd-3.3.0/src/openepd/model/specs/generated/other_electrical_equipment.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/other_materials.py` & `openepd-3.3.0/src/openepd/model/specs/generated/other_materials.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/plumbing.py` & `openepd-3.3.0/src/openepd/model/specs/generated/plumbing.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/sheathing.py` & `openepd-3.3.0/src/openepd/model/specs/generated/sheathing.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/steel.py` & `openepd-3.3.0/src/openepd/model/specs/generated/steel.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/thermal_moisture_protection.py` & `openepd-3.3.0/src/openepd/model/specs/generated/thermal_moisture_protection.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/utility_piping.py` & `openepd-3.3.0/src/openepd/model/specs/generated/utility_piping.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/wood.py` & `openepd-3.3.0/src/openepd/model/specs/generated/wood.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/specs/generated/wood_joists.py` & `openepd-3.3.0/src/openepd/model/specs/generated/wood_joists.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/standard.py` & `openepd-3.3.0/src/openepd/model/standard.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/validation/__init__.py` & `openepd-3.3.0/src/openepd/model/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/validation/common.py` & `openepd-3.3.0/src/openepd/model/validation/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/validation/numbers.py` & `openepd-3.3.0/src/openepd/model/validation/numbers.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/validation/quantity.py` & `openepd-3.3.0/src/openepd/model/validation/quantity.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/src/openepd/model/versioning.py` & `openepd-3.3.0/src/openepd/model/versioning.py`

 * *Files identical despite different names*

### Comparing `openepd-3.2.0/PKG-INFO` & `openepd-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openepd
-Version: 3.2.0
+Version: 3.3.0
 Summary: Python library to work with OpenEPD format
 Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: open-source@c-change-labs.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openepd Version: 3.2.0 Summary: Python library to
+Metadata-Version: 2.1 Name: openepd Version: 3.3.0 Summary: Python library to
 work with OpenEPD format Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0 Author: C-Change Labs Author-email: support@c-change-
 labs.com Maintainer: C-Change Labs Maintainer-email: open-source@c-change-
 labs.com Requires-Python: >=3.11,<4.0 Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

