# Comparing `tmp/esptool-4.8.dev3.tar.gz` & `tmp/esptool-4.8.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esptool-4.8.dev3.tar", last modified: Tue Mar 19 16:04:36 2024, max compression
+gzip compressed data, was "esptool-4.8.dev4.tar", last modified: Thu May 30 11:22:02 2024, max compression
```

## Comparing `esptool-4.8.dev3.tar` & `esptool-4.8.dev4.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.714456 esptool-4.8.dev3/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-03-19 16:04:24.000000 esptool-4.8.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-19 16:04:24.000000 esptool-4.8.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-03-19 16:04:36.710456 esptool-4.8.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-19 16:04:24.000000 esptool-4.8.dev3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)    10513 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esp_rfc2217_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.690456 esptool-4.8.dev3/espefuse/
--rwxr-xr-x   0 runner    (1001) docker     (127)    10566 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.690456 esptool-4.8.dev3/espefuse/efuse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/base_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    27243 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/base_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/emulate_efuse_controller_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.690456 esptool-4.8.dev3/espefuse/efuse/esp32/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    17243 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12519 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.694456 esptool-4.8.dev3/espefuse/efuse/esp32c2/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c2/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    14791 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c2/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c2/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11998 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c2/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.694456 esptool-4.8.dev3/espefuse/efuse/esp32c3/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c3/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    18098 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c3/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c3/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    14044 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c3/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.694456 esptool-4.8.dev3/espefuse/efuse/esp32c5/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c5/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    18793 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c5/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c5/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    13190 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c5/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.694456 esptool-4.8.dev3/espefuse/efuse/esp32c5beta3/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c5beta3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c5beta3/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    18813 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c5beta3/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c5beta3/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    13196 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c5beta3/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.694456 esptool-4.8.dev3/espefuse/efuse/esp32c6/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c6/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    18660 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c6/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c6/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c6/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.698456 esptool-4.8.dev3/espefuse/efuse/esp32c61/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c61/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c61/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    19111 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c61/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c61/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    15770 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32c61/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.698456 esptool-4.8.dev3/espefuse/efuse/esp32h2/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32h2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32h2/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    18856 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32h2/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32h2/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    15391 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32h2/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.698456 esptool-4.8.dev3/espefuse/efuse/esp32h2beta1/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32h2beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32h2beta1/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    18765 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32h2beta1/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32h2beta1/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32h2beta1/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.698456 esptool-4.8.dev3/espefuse/efuse/esp32p4/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32p4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32p4/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    18146 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32p4/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32p4/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    15591 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32p4/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.698456 esptool-4.8.dev3/espefuse/efuse/esp32s2/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32s2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32s2/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    19971 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32s2/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32s2/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    18647 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32s2/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.702456 esptool-4.8.dev3/espefuse/efuse/esp32s3/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32s3/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    19184 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32s3/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32s3/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    18570 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32s3/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.702456 esptool-4.8.dev3/espefuse/efuse/esp32s3beta2/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32s3beta2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32s3beta2/emulate_efuse_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    19198 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32s3beta2/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32s3beta2/mem_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    18577 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/esp32s3beta2/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/mem_definition_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.702456 esptool-4.8.dev3/espefuse/efuse_defs/
--rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse_defs/esp32.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15595 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse_defs/esp32c2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    34635 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse_defs/esp32c3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    29236 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse_defs/esp32c5.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    29236 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse_defs/esp32c5beta3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35331 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse_defs/esp32c6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    23139 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse_defs/esp32c61.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    33638 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse_defs/esp32h2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35358 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse_defs/esp32p4.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35820 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse_defs/esp32s2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    41844 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse/efuse_defs/esp32s3.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1180 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espefuse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.702456 esptool-4.8.dev3/espsecure/
--rwxr-xr-x   0 runner    (1001) docker     (127)    63495 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espsecure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espsecure/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.706456 esptool-4.8.dev3/espsecure/esp_hsm_sign/
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espsecure/esp_hsm_sign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espsecure/esp_hsm_sign/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1185 2024-03-19 16:04:24.000000 esptool-4.8.dev3/espsecure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.706456 esptool-4.8.dev3/esptool/
--rw-r--r--   0 runner    (1001) docker     (127)    40699 2024-03-19 16:04:34.000000 esptool-4.8.dev3/esptool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51676 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/bin_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    52027 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    63327 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/reset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.710456 esptool-4.8.dev3/esptool/targets/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16755 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/esp32.py
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/esp32c2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/esp32c3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/esp32c5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/esp32c5beta3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7430 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/esp32c6.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/esp32c61.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/esp32c6beta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/esp32h2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/esp32h2beta1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/esp32h2beta2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/esp32p4.py
--rw-r--r--   0 runner    (1001) docker     (127)    11562 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/esp32s2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14224 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/esp32s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/esp32s3beta2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/esp8266.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.710456 esptool-4.8.dev3/esptool/targets/stub_flasher/
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32.json
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32c2.json
--rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32c3.json
--rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32c5beta3.json
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32c6.json
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32c6beta.json
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32h2.json
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32h2beta1.json
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32h2beta2.json
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32p4.json
--rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32s2.json
--rw-r--r--   0 runner    (1001) docker     (127)     7540 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32s3.json
--rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32s3beta2.json
--rw-r--r--   0 runner    (1001) docker     (127)    12172 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_8266.json
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/uf2_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:04:36.706456 esptool-4.8.dev3/esptool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-03-19 16:04:36.000000 esptool-4.8.dev3/esptool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-03-19 16:04:36.000000 esptool-4.8.dev3/esptool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 16:04:36.000000 esptool-4.8.dev3/esptool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-19 16:04:36.000000 esptool-4.8.dev3/esptool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-19 16:04:36.000000 esptool-4.8.dev3/esptool.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1175 2024-03-19 16:04:24.000000 esptool-4.8.dev3/esptool.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 16:04:36.714456 esptool-4.8.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-03-19 16:04:24.000000 esptool-4.8.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.602161 esptool-4.8.dev4/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-30 11:21:50.000000 esptool-4.8.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-30 11:21:50.000000 esptool-4.8.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-30 11:22:02.602161 esptool-4.8.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-30 11:21:50.000000 esptool-4.8.dev4/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10513 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esp_rfc2217_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.578161 esptool-4.8.dev4/espefuse/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10566 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.582161 esptool-4.8.dev4/espefuse/efuse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35865 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/base_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28392 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/base_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/emulate_efuse_controller_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.582161 esptool-4.8.dev4/espefuse/efuse/esp32/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32/emulate_efuse_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17243 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32/mem_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12519 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.582161 esptool-4.8.dev4/espefuse/efuse/esp32c2/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c2/emulate_efuse_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14791 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c2/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c2/mem_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11998 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c2/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.582161 esptool-4.8.dev4/espefuse/efuse/esp32c3/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c3/emulate_efuse_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18098 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c3/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c3/mem_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14044 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c3/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.582161 esptool-4.8.dev4/espefuse/efuse/esp32c5/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c5/emulate_efuse_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18793 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c5/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c5/mem_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c5/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.586161 esptool-4.8.dev4/espefuse/efuse/esp32c5beta3/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c5beta3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c5beta3/emulate_efuse_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18813 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c5beta3/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c5beta3/mem_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c5beta3/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.586161 esptool-4.8.dev4/espefuse/efuse/esp32c6/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c6/emulate_efuse_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18660 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c6/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c6/mem_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c6/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.586161 esptool-4.8.dev4/espefuse/efuse/esp32c61/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c61/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c61/emulate_efuse_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19111 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c61/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c61/mem_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15769 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32c61/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.586161 esptool-4.8.dev4/espefuse/efuse/esp32h2/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32h2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32h2/emulate_efuse_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18856 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32h2/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32h2/mem_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15391 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32h2/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.586161 esptool-4.8.dev4/espefuse/efuse/esp32h2beta1/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32h2beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32h2beta1/emulate_efuse_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18765 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32h2beta1/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32h2beta1/mem_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32h2beta1/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.590161 esptool-4.8.dev4/espefuse/efuse/esp32p4/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32p4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32p4/emulate_efuse_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18146 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32p4/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32p4/mem_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15591 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32p4/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.590161 esptool-4.8.dev4/espefuse/efuse/esp32s2/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32s2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32s2/emulate_efuse_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19971 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32s2/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32s2/mem_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18647 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32s2/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.590161 esptool-4.8.dev4/espefuse/efuse/esp32s3/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32s3/emulate_efuse_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19184 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32s3/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32s3/mem_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18570 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32s3/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.590161 esptool-4.8.dev4/espefuse/efuse/esp32s3beta2/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32s3beta2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32s3beta2/emulate_efuse_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19198 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32s3beta2/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32s3beta2/mem_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18577 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/esp32s3beta2/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/mem_definition_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.594161 esptool-4.8.dev4/espefuse/efuse_defs/
+-rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse_defs/esp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15595 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse_defs/esp32c2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    34635 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse_defs/esp32c3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    29236 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse_defs/esp32c5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    29236 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse_defs/esp32c5beta3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35331 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse_defs/esp32c6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    23139 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse_defs/esp32c61.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    33638 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse_defs/esp32h2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35358 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse_defs/esp32p4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35820 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse_defs/esp32s2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    41844 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse/efuse_defs/esp32s3.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1180 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espefuse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.594161 esptool-4.8.dev4/espsecure/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    63495 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espsecure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espsecure/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.594161 esptool-4.8.dev4/espsecure/esp_hsm_sign/
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espsecure/esp_hsm_sign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espsecure/esp_hsm_sign/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1185 2024-05-30 11:21:50.000000 esptool-4.8.dev4/espsecure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.594161 esptool-4.8.dev4/esptool/
+-rw-r--r--   0 runner    (1001) docker     (127)    40728 2024-05-30 11:22:00.000000 esptool-4.8.dev4/esptool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52257 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/bin_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54160 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63854 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/reset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.598161 esptool-4.8.dev4/esptool/targets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16755 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/esp32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/esp32c2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/esp32c3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/esp32c5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/esp32c5beta3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7430 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/esp32c6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/esp32c61.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/esp32c6beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/esp32h2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/esp32h2beta1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/esp32h2beta2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/esp32p4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11562 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/esp32s2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14707 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/esp32s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/esp32s3beta2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/esp8266.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.602161 esptool-4.8.dev4/esptool/targets/stub_flasher/
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32c2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32c3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32c5beta3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32c6.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32c6beta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32h2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32h2beta1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32h2beta2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32p4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32s2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7540 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32s3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32s3beta2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12172 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_8266.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/uf2_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:22:02.598161 esptool-4.8.dev4/esptool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-30 11:22:02.000000 esptool-4.8.dev4/esptool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-05-30 11:22:02.000000 esptool-4.8.dev4/esptool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:22:02.000000 esptool-4.8.dev4/esptool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-30 11:22:02.000000 esptool-4.8.dev4/esptool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 11:22:02.000000 esptool-4.8.dev4/esptool.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1175 2024-05-30 11:21:50.000000 esptool-4.8.dev4/esptool.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 11:22:02.602161 esptool-4.8.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-30 11:21:50.000000 esptool-4.8.dev4/setup.py
```

### Comparing `esptool-4.8.dev3/LICENSE` & `esptool-4.8.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/PKG-INFO` & `esptool-4.8.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esptool
-Version: 4.8.dev3
+Version: 4.8.dev4
 Summary: A serial utility to communicate & flash code to Espressif chips.
 Home-page: https://github.com/espressif/esptool/
 Author: Fredrik Ahlberg (themadinventor) & Angus Gratton (projectgus) & Espressif Systems
 Author-email: 
 License: GPLv2+
 Project-URL: Documentation, https://docs.espressif.com/projects/esptool/
 Project-URL: Source, https://github.com/espressif/esptool/
```

### Comparing `esptool-4.8.dev3/README.md` & `esptool-4.8.dev4/README.md`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esp_rfc2217_server.py` & `esptool-4.8.dev4/esp_rfc2217_server.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/__init__.py` & `esptool-4.8.dev4/espefuse/__init__.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/base_fields.py` & `esptool-4.8.dev4/espefuse/efuse/base_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import sys
 
 from bitstring import BitArray, BitStream, CreationError
 
 import esptool
 
 from . import util
+from typing import List
 
 
 class CheckArgValue(object):
     def __init__(self, efuses, name):
         self.efuses = efuses
         self.name = name
 
@@ -223,21 +224,22 @@
 
     def get_words(self):
         def get_offsets(self):
             return [x + self.rd_addr for x in range(0, self.get_block_len(), 4)]
 
         return [self.parent.read_reg(offs) for offs in get_offsets(self)]
 
-    def read(self):
+    def read(self, print_info=True):
         words = self.get_words()
         data = BitArray()
         for word in reversed(words):
             data.append("uint:32=%d" % word)
         self.bitarray.overwrite(data, pos=0)
-        self.print_block(self.bitarray, "read_regs")
+        if print_info:
+            self.print_block(self.bitarray, "read_regs")
 
     def print_block(self, bit_string, comment, debug=False):
         if self.parent.debug or debug:
             bit_string.pos = 0
             print(
                 "%-15s (%-16s) [%-2d] %s:"
                 % (self.name, " ".join(self.alias)[:16], self.id, comment),
@@ -381,14 +383,26 @@
                     print(
                         "Error in BLOCK%d, re-burn it again (#%d), to fix it. "
                         "fail_bit=%d, num_errors=%d"
                         % (self.id, burns, self.fail, self.num_errors)
                     )
                     break
             if not self.fail and self.num_errors == 0:
+                self.read(print_info=False)
+                if self.wr_bitarray & self.bitarray != self.wr_bitarray:
+                    # if the required bits are not set then we need to re-burn it again.
+                    if burns < 2:
+                        print(
+                            f"\nRepeat burning BLOCK{self.id} (#{burns + 2}) because not all bits were set"
+                        )
+                        continue
+                    else:
+                        print(
+                            f"\nAfter {burns + 1} attempts, the required data was not set to BLOCK{self.id}"
+                        )
                 break
 
     def burn(self):
         if self.wr_bitarray.all(False):
             # nothing to burn
             return
         before_burn_bitarray = self.bitarray[:]
@@ -437,16 +451,16 @@
 
 class EspEfusesBase(object):
     """
     Wrapper object to manage the efuse fields in a connected ESP bootloader
     """
 
     _esp = None
-    blocks = []
-    efuses = []
+    blocks: List[EfuseBlockBase] = []
+    efuses: List = []
     coding_scheme = None
     force_write_always = None
     batch_mode_cnt = 0
     postpone = False
 
     def __iter__(self):
         return self.efuses.__iter__()
```

### Comparing `esptool-4.8.dev3/espefuse/efuse/base_operations.py` & `esptool-4.8.dev4/espefuse/efuse/base_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,20 +61,19 @@
             setattr(namespace, self.dest, efuse_value_pairs)
 
     burn = subparsers.add_parser(
         "burn_efuse", help="Burn the efuse with the specified name"
     )
     burn.add_argument(
         "name_value_pairs",
-        help="Name of efuse register and New value pairs to burn",
+        help="Name of efuse field and new value pairs to burn. EFUSE_NAME: "
+        "[{}].".format(", ".join([e.name for e in efuses.efuses])),
         action=ActionEfuseValuePair,
         nargs="+",
-        metavar="[EFUSE_NAME VALUE] [{} VALUE".format(
-            " VALUE] [".join([e.name for e in efuses.efuses])
-        ),
+        metavar="[EFUSE_NAME VALUE]",
         efuse_choices=[e.name for e in efuses.efuses]
         + [name for e in efuses.efuses for name in e.alt_names if name != ""],
         efuses=efuses,
     )
 
     read_protect_efuse = subparsers.add_parser(
         "read_protect_efuse",
@@ -179,23 +178,28 @@
 
     summary_cmd = subparsers.add_parser(
         "summary", help="Print human-readable summary of efuse values"
     )
     summary_cmd.add_argument(
         "--format",
         help="Select the summary format",
-        choices=["summary", "json"],
+        choices=["summary", "json", "value_only"],
         default="summary",
     )
     summary_cmd.add_argument(
         "--file",
         help="File to save the efuse summary",
         type=argparse.FileType("w"),
         default=sys.stdout,
     )
+    summary_cmd.add_argument(
+        "efuses_to_show",
+        help="The efuses to show. If not provided, all efuses will be shown.",
+        nargs="*",
+    )
 
     execute_scripts = subparsers.add_parser(
         "execute_scripts", help="Executes scripts to burn at one time."
     )
     execute_scripts.add_argument(
         "scripts",
         help="The special format of python scripts.",
@@ -242,37 +246,43 @@
         "Enabled if --debug is used.",
         action="store_true",
         default=False,
     )
 
 
 def summary(esp, efuses, args):
-    """Print a human-readable summary of efuse contents"""
+    """Print a human-readable or json summary of efuse contents"""
     ROW_FORMAT = "%-50s %-50s%s = %s %s %s"
-    human_output = args.format == "summary"
+    human_output = args.format in ["summary", "value_only"]
+    value_only = args.format == "value_only"
+    if value_only and len(args.efuses_to_show) != 1:
+        raise esptool.FatalError(
+            "The 'value_only' format can be used exactly for one efuse."
+        )
+    do_filtering = bool(args.efuses_to_show)
     json_efuse = {}
+    summary_efuse = []
     if args.file != sys.stdout:
         print("Saving efuse values to " + args.file.name)
-    if human_output:
-        print(
+    if human_output and not value_only:
+        summary_efuse.append(
             ROW_FORMAT.replace("-50", "-12")
             % (
                 "EFUSE_NAME (Block)",
                 "Description",
                 "",
                 "[Meaningful Value]",
                 "[Readable/Writeable]",
                 "(Hex Value)",
-            ),
-            file=args.file,
+            )
         )
-        print("-" * 88, file=args.file)
+        summary_efuse.append("-" * 88)
     for category in sorted(set(e.category for e in efuses), key=lambda c: c.title()):
-        if human_output:
-            print("%s fuses:" % category.title(), file=args.file)
+        if human_output and not value_only:
+            summary_efuse.append(f"{category.title()} fuses:")
         for e in (e for e in efuses if e.category == category):
             if e.efuse_type.startswith("bytes"):
                 raw = ""
             else:
                 raw = "({})".format(e.get_bitstring())
             (readable, writeable) = (e.is_readable(), e.is_writeable())
             if readable and writeable:
@@ -293,62 +303,75 @@
                     v = [value[: (len(value) // 2)], value[(len(value) // 2) :]]
                     for i in range(count_read_disable_bits):
                         if not e.is_readable(blk_part=i):
                             v[i] = v[i].replace("0", "?")
                     value = "".join(v)
                 else:
                     value = value.replace("0", "?")
-            if human_output:
-                print(
+            if (
+                human_output
+                and (not do_filtering or e.name in args.efuses_to_show)
+                and not value_only
+            ):
+                summary_efuse.append(
                     ROW_FORMAT
                     % (
                         e.get_info(),
                         e.description[:50],
                         "\n  " if len(value) > 20 else "",
                         value,
                         perms,
                         raw,
-                    ),
-                    file=args.file,
+                    )
                 )
                 desc_len = len(e.description[50:])
                 if desc_len:
                     desc_len += 50
                     for i in range(50, desc_len, 50):
-                        print(
-                            "%-50s %-50s" % ("", e.description[i : (50 + i)]),
-                            file=args.file,
+                        summary_efuse.append(
+                            f"{'':<50} {e.description[i : (50 + i)]:<50}"
                         )
-            if args.format == "json":
+            elif human_output and value_only and e.name in args.efuses_to_show:
+                summary_efuse.append(f"{value}")
+            elif args.format == "json" and (
+                not do_filtering or e.name in args.efuses_to_show
+            ):
                 json_efuse[e.name] = {
                     "name": e.name,
                     "value": base_value if readable else value,
                     "readable": readable,
                     "writeable": writeable,
                     "description": e.description,
                     "category": e.category,
                     "block": e.block,
                     "word": e.word,
                     "pos": e.pos,
                     "efuse_type": e.efuse_type,
                     "bit_len": e.bit_len,
                 }
-        if human_output:
-            print("", file=args.file)
-    if human_output:
-        print(efuses.summary(), file=args.file)
+        if human_output and not value_only:
+            # Remove empty category if efuses are filtered and there are none to show
+            if do_filtering and summary_efuse[-1] == f"{category.title()} fuses:":
+                summary_efuse.pop()
+            else:
+                summary_efuse.append("")
+    if human_output and not value_only:
+        summary_efuse.append(efuses.summary())
         warnings = efuses.get_coding_scheme_warnings()
         if warnings:
-            print(
-                "WARNING: Coding scheme has encoding bit error warnings", file=args.file
+            summary_efuse.append(
+                "WARNING: Coding scheme has encoding bit error warnings"
             )
+    if human_output:
+        for line in summary_efuse:
+            print(line, file=args.file)
         if args.file != sys.stdout:
             args.file.close()
             print("Done")
-    if args.format == "json":
+    elif args.format == "json":
         json.dump(json_efuse, args.file, sort_keys=True, indent=4)
         print("")
 
 
 def dump(esp, efuses, args):
     """Dump raw efuse data registers"""
     # Using --debug option allows to print dump.
```

### Comparing `esptool-4.8.dev3/espefuse/efuse/emulate_efuse_controller_base.py` & `esptool-4.8.dev4/espefuse/efuse/emulate_efuse_controller_base.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32/emulate_efuse_controller.py` & `esptool-4.8.dev4/espefuse/efuse/esp32/emulate_efuse_controller.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32/fields.py` & `esptool-4.8.dev4/espefuse/efuse/esp32/fields.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32/mem_definition.py` & `esptool-4.8.dev4/espefuse/efuse/esp32/mem_definition.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32/operations.py` & `esptool-4.8.dev4/espefuse/efuse/esp32/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c2/emulate_efuse_controller.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c2/emulate_efuse_controller.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c2/fields.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c2/fields.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c2/mem_definition.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c2/mem_definition.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c2/operations.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c2/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c3/emulate_efuse_controller.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c3/emulate_efuse_controller.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c3/fields.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c3/fields.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c3/mem_definition.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c3/mem_definition.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c3/operations.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c3/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c5/emulate_efuse_controller.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c5/emulate_efuse_controller.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c5/fields.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c5/fields.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c5/mem_definition.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c5beta3/mem_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# This file describes eFuses fields and registers for ESP32-C5 chip
+# This file describes eFuses fields and registers for ESP32-C5 beta3 chip
 #
-# SPDX-FileCopyrightText: 2024 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2023 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import os
 
 import yaml
```

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c5/operations.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c5/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,22 +232,29 @@
             raise esptool.FatalError("Unknown block name - %s" % (block_name))
         num_bytes = efuse.bit_len // 8
 
         block_num = efuses.get_index_block_by_name(block_name)
         block = efuses.blocks[block_num]
 
         if digest is None:
-            data = datafile.read()
+            if keypurpose == "ECDSA_KEY":
+                sk = espsecure.load_ecdsa_signing_key(datafile)
+                data = sk.to_string()
+                if len(data) == 24:
+                    # the private key is 24 bytes long for NIST192p, and 8 bytes of padding
+                    data = b"\x00" * 8 + data
+            else:
+                data = datafile.read()
         else:
             data = datafile
 
         print(" - %s" % (efuse.name), end=" ")
         revers_msg = None
         if efuses[block.key_purpose_name].need_reverse(keypurpose):
-            revers_msg = "\tReversing byte order for AES-XTS hardware peripheral"
+            revers_msg = f"\tReversing byte order for {keypurpose} hardware peripheral"
             data = data[::-1]
         print(
             "-> [{}]".format(
                 util.hexify(data, " ")
                 if args.show_sensitive_info
                 else " ".join(["??"] * len(data))
             )
```

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c5beta3/emulate_efuse_controller.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c5beta3/emulate_efuse_controller.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c5beta3/fields.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c5beta3/fields.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c5beta3/mem_definition.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c5/mem_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# This file describes eFuses fields and registers for ESP32-C5 beta3 chip
+# This file describes eFuses fields and registers for ESP32-C5 chip
 #
-# SPDX-FileCopyrightText: 2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2024 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import os
 
 import yaml
 
@@ -16,15 +16,15 @@
 )
 
 
 class EfuseDefineRegisters(EfuseRegistersBase):
     EFUSE_MEM_SIZE = 0x01FC + 4
 
     # EFUSE registers & command/conf values
-    DR_REG_EFUSE_BASE = 0x600B0800
+    DR_REG_EFUSE_BASE = 0x600B4800
     EFUSE_PGM_DATA0_REG = DR_REG_EFUSE_BASE
     EFUSE_CHECK_VALUE0_REG = DR_REG_EFUSE_BASE + 0x020
     EFUSE_CLK_REG = DR_REG_EFUSE_BASE + 0x1C8
     EFUSE_CONF_REG = DR_REG_EFUSE_BASE + 0x1CC
     EFUSE_STATUS_REG = DR_REG_EFUSE_BASE + 0x1D0
     EFUSE_CMD_REG = DR_REG_EFUSE_BASE + 0x1D4
     EFUSE_RD_RS_ERR0_REG = DR_REG_EFUSE_BASE + 0x1C0
```

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c5beta3/operations.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c5beta3/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,22 +232,29 @@
             raise esptool.FatalError("Unknown block name - %s" % (block_name))
         num_bytes = efuse.bit_len // 8
 
         block_num = efuses.get_index_block_by_name(block_name)
         block = efuses.blocks[block_num]
 
         if digest is None:
-            data = datafile.read()
+            if keypurpose == "ECDSA_KEY":
+                sk = espsecure.load_ecdsa_signing_key(datafile)
+                data = sk.to_string()
+                if len(data) == 24:
+                    # the private key is 24 bytes long for NIST192p, and 8 bytes of padding
+                    data = b"\x00" * 8 + data
+            else:
+                data = datafile.read()
         else:
             data = datafile
 
         print(" - %s" % (efuse.name), end=" ")
         revers_msg = None
         if efuses[block.key_purpose_name].need_reverse(keypurpose):
-            revers_msg = "\tReversing byte order for AES-XTS hardware peripheral"
+            revers_msg = f"\tReversing byte order for {keypurpose} hardware peripheral"
             data = data[::-1]
         print(
             "-> [{}]".format(
                 util.hexify(data, " ")
                 if args.show_sensitive_info
                 else " ".join(["??"] * len(data))
             )
```

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c6/emulate_efuse_controller.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c6/emulate_efuse_controller.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c6/fields.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c6/fields.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c6/mem_definition.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c6/mem_definition.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c6/operations.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c6/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c61/emulate_efuse_controller.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c61/emulate_efuse_controller.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c61/fields.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c61/fields.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c61/mem_definition.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c61/mem_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file describes eFuses fields and registers for ESP32-C61 chip
 #
 # SPDX-FileCopyrightText: 2024 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import os
+from typing import List
 
 import yaml
 
 from ..mem_definition_base import (
     EfuseBlocksBase,
     EfuseFieldsBase,
     EfuseRegistersBase,
@@ -115,15 +116,15 @@
         self.EFUSES = []
 
         self.KEYBLOCKS = []
 
         # if BLK_VERSION_MINOR is 1, these efuse fields are in BLOCK2
         self.BLOCK2_CALIBRATION_EFUSES = []
 
-        self.CALC = []
+        self.CALC: List = []
 
         dir_name = os.path.dirname(os.path.abspath(__file__))
         dir_name, file_name = os.path.split(dir_name)
         file_name = file_name + ".yaml"
         dir_name, _ = os.path.split(dir_name)
         efuse_file = os.path.join(dir_name, "efuse_defs", file_name)
         with open(f"{efuse_file}", "r") as r_file:
```

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32c61/operations.py` & `esptool-4.8.dev4/espefuse/efuse/esp32c61/operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,15 +300,15 @@
         num_bytes = efuse.bit_len // 8
 
         block_num = efuses.get_index_block_by_name(block_name)
         block = efuses.blocks[block_num]
 
         if digest is None:
             if keypurpose == "ECDSA_KEY":
-                sk = espsecure._load_ecdsa_signing_key(datafile)
+                sk = espsecure.load_ecdsa_signing_key(datafile)
                 data = sk.to_string()
                 if len(data) == 24:
                     # the private key is 24 bytes long for NIST192p, and 8 bytes of padding
                     data = b"\x00" * 8 + data
             else:
                 data = datafile.read()
         else:
```

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32h2/emulate_efuse_controller.py` & `esptool-4.8.dev4/espefuse/efuse/esp32h2/emulate_efuse_controller.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32h2/fields.py` & `esptool-4.8.dev4/espefuse/efuse/esp32h2/fields.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32h2/mem_definition.py` & `esptool-4.8.dev4/espefuse/efuse/esp32h2/mem_definition.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32h2/operations.py` & `esptool-4.8.dev4/espefuse/efuse/esp32h2/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32h2beta1/emulate_efuse_controller.py` & `esptool-4.8.dev4/espefuse/efuse/esp32h2beta1/emulate_efuse_controller.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32h2beta1/fields.py` & `esptool-4.8.dev4/espefuse/efuse/esp32h2beta1/fields.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32h2beta1/mem_definition.py` & `esptool-4.8.dev4/espefuse/efuse/esp32h2beta1/mem_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import os
 
 import yaml
 
 from ..mem_definition_base import EfuseBlocksBase, EfuseFieldsBase, EfuseRegistersBase
+from typing import List
 
 
 class EfuseDefineRegisters(EfuseRegistersBase):
     EFUSE_MEM_SIZE = 0x01FC + 4
 
     # EFUSE registers & command/conf values
     DR_REG_EFUSE_BASE = 0x6001A000
@@ -111,15 +112,15 @@
         self.EFUSES = []
 
         self.KEYBLOCKS = []
 
         # if BLK_VERSION_MAJOR is 1, these efuse fields are in BLOCK2
         self.BLOCK2_CALIBRATION_EFUSES = []
 
-        self.CALC = []
+        self.CALC: List = []
 
         dir_name = os.path.dirname(os.path.abspath(__file__))
         dir_name, file_name = os.path.split(dir_name)
         file_name = file_name + ".yaml"
         dir_name, _ = os.path.split(dir_name)
         efuse_file = os.path.join(dir_name, "efuse_defs", file_name)
         efuse_file = efuse_file.replace("esp32h2beta1", "esp32h2")
```

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32h2beta1/operations.py` & `esptool-4.8.dev4/espefuse/efuse/esp32h2beta1/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32p4/emulate_efuse_controller.py` & `esptool-4.8.dev4/espefuse/efuse/esp32p4/emulate_efuse_controller.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32p4/fields.py` & `esptool-4.8.dev4/espefuse/efuse/esp32p4/fields.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32p4/mem_definition.py` & `esptool-4.8.dev4/espefuse/efuse/esp32p4/mem_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import yaml
 
 from ..mem_definition_base import (
     EfuseBlocksBase,
     EfuseFieldsBase,
     EfuseRegistersBase,
 )
+from typing import List
 
 
 class EfuseDefineRegisters(EfuseRegistersBase):
     EFUSE_MEM_SIZE = 0x01FC + 4
 
     # EFUSE registers & command/conf values
     DR_REG_EFUSE_BASE = 0x5012D000
@@ -115,15 +116,15 @@
         self.EFUSES = []
 
         self.KEYBLOCKS = []
 
         # if BLK_VERSION_MINOR is 1, these efuse fields are in BLOCK2
         self.BLOCK2_CALIBRATION_EFUSES = []
 
-        self.CALC = []
+        self.CALC: List = []
 
         dir_name = os.path.dirname(os.path.abspath(__file__))
         dir_name, file_name = os.path.split(dir_name)
         file_name = file_name + ".yaml"
         dir_name, _ = os.path.split(dir_name)
         efuse_file = os.path.join(dir_name, "efuse_defs", file_name)
         with open(f"{efuse_file}", "r") as r_file:
```

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32p4/operations.py` & `esptool-4.8.dev4/espefuse/efuse/esp32p4/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32s2/emulate_efuse_controller.py` & `esptool-4.8.dev4/espefuse/efuse/esp32s2/emulate_efuse_controller.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32s2/fields.py` & `esptool-4.8.dev4/espefuse/efuse/esp32s2/fields.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32s2/mem_definition.py` & `esptool-4.8.dev4/espefuse/efuse/esp32s2/mem_definition.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32s2/operations.py` & `esptool-4.8.dev4/espefuse/efuse/esp32s2/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32s3/emulate_efuse_controller.py` & `esptool-4.8.dev4/espefuse/efuse/esp32s3/emulate_efuse_controller.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32s3/fields.py` & `esptool-4.8.dev4/espefuse/efuse/esp32s3/fields.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32s3/mem_definition.py` & `esptool-4.8.dev4/espefuse/efuse/esp32s3/mem_definition.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32s3/operations.py` & `esptool-4.8.dev4/espefuse/efuse/esp32s3/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32s3beta2/emulate_efuse_controller.py` & `esptool-4.8.dev4/espefuse/efuse/esp32s3beta2/emulate_efuse_controller.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32s3beta2/fields.py` & `esptool-4.8.dev4/espefuse/efuse/esp32s3beta2/fields.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32s3beta2/mem_definition.py` & `esptool-4.8.dev4/espefuse/efuse/esp32s3beta2/mem_definition.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/esp32s3beta2/operations.py` & `esptool-4.8.dev4/espefuse/efuse/esp32s3beta2/operations.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse/mem_definition_base.py` & `esptool-4.8.dev4/espefuse/efuse/mem_definition_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # This file describes eFuses fields and registers for ESP32 chip
 #
 # SPDX-FileCopyrightText: 2020-2022 Espressif Systems (Shanghai) CO LTD
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 from collections import namedtuple
+from typing import Optional, List
 
 
 class EfuseRegistersBase(object):
     # Coding Scheme values
     CODING_SCHEME_NONE = 0
     CODING_SCHEME_34 = 1
     CODING_SCHEME_REPEAT = 2
     CODING_SCHEME_NONE_RECOVERY = 3
     CODING_SCHEME_RS = 4
 
     EFUSE_BURN_TIMEOUT = 0.250  # seconds
 
 
 class EfuseBlocksBase(object):
-    BLOCKS = None
+    BLOCKS: Optional[List] = None
     NamedtupleBlock = namedtuple(
-        "Block",
+        "NamedtupleBlock",
         "name alias id rd_addr wr_addr write_disable_bit "
         "read_disable_bit len key_purpose",
     )
 
     @staticmethod
     def get(tuple_block):
         return EfuseBlocksBase.NamedtupleBlock._make(tuple_block)
@@ -45,27 +46,27 @@
 
 class Field:
     name = ""
     block = 0
     word = None
     pos = None
     bit_len = 0
-    alt_names = []
+    alt_names: List[str] = []
     type = ""
     write_disable_bit = None
     read_disable_bit = None
     category = "config"
     class_type = ""
     description = ""
     dictionary = None
 
 
 class EfuseFieldsBase(object):
     def __init__(self, e_desc) -> None:
-        self.ALL_EFUSES = []
+        self.ALL_EFUSES: List = []
 
         def set_category_and_class_type(efuse, name):
             def includes(name, names):
                 return any([word in name for word in names])
 
             if name.startswith("SPI_PAD_CONFIG"):
                 efuse.category = "spi pad"
```

### Comparing `esptool-4.8.dev3/espefuse/efuse/util.py` & `esptool-4.8.dev4/espefuse/efuse/util.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse_defs/esp32.yaml` & `esptool-4.8.dev4/espefuse/efuse_defs/esp32.yaml`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse_defs/esp32c2.yaml` & `esptool-4.8.dev4/espefuse/efuse_defs/esp32c2.yaml`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse_defs/esp32c3.yaml` & `esptool-4.8.dev4/espefuse/efuse_defs/esp32c3.yaml`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse_defs/esp32c5.yaml` & `esptool-4.8.dev4/espefuse/efuse_defs/esp32c5.yaml`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse_defs/esp32c5beta3.yaml` & `esptool-4.8.dev4/espefuse/efuse_defs/esp32c5beta3.yaml`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse_defs/esp32c6.yaml` & `esptool-4.8.dev4/espefuse/efuse_defs/esp32c6.yaml`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse_defs/esp32c61.yaml` & `esptool-4.8.dev4/espefuse/efuse_defs/esp32c61.yaml`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse_defs/esp32h2.yaml` & `esptool-4.8.dev4/espefuse/efuse_defs/esp32h2.yaml`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse_defs/esp32p4.yaml` & `esptool-4.8.dev4/espefuse/efuse_defs/esp32p4.yaml`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse_defs/esp32s2.yaml` & `esptool-4.8.dev4/espefuse/efuse_defs/esp32s2.yaml`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse/efuse_defs/esp32s3.yaml` & `esptool-4.8.dev4/espefuse/efuse_defs/esp32s3.yaml`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espefuse.py` & `esptool-4.8.dev4/espefuse.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espsecure/__init__.py` & `esptool-4.8.dev4/espsecure/__init__.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espsecure/esp_hsm_sign/__init__.py` & `esptool-4.8.dev4/espsecure/esp_hsm_sign/__init__.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espsecure/esp_hsm_sign/exceptions.py` & `esptool-4.8.dev4/espsecure/esp_hsm_sign/exceptions.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/espsecure.py` & `esptool-4.8.dev4/espsecure.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/__init__.py` & `esptool-4.8.dev4/esptool/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "verify_flash",
     "version",
     "write_flash",
     "write_flash_status",
     "write_mem",
 ]
 
-__version__ = "4.8.dev3"
+__version__ = "4.8.dev4"
 
 import argparse
 import inspect
 import os
 import shlex
 import sys
 import time
@@ -492,15 +492,15 @@
     parser_elf2image.add_argument(
         "--ram-only-header",
         help="Order segments of the output so IRAM and DRAM are placed at the "
         "beginning and force the main header segment number to RAM segments "
         "quantity. This will make the other segments invisible to the ROM "
         "loader. Use this argument with care because the ROM loader will load "
         "only the RAM segments although the other segments being present in "
-        "the output.",
+        "the output. Implies --dont-append-digest",
         action="store_true",
         default=None,
     )
 
     add_spi_flash_subparsers(parser_elf2image, allow_keep=False, auto_detect=False)
 
     subparsers.add_parser("read_mac", help="Read MAC address from OTP ROM")
```

### Comparing `esptool-4.8.dev3/esptool/bin_image.py` & `esptool-4.8.dev4/esptool/bin_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import copy
 import hashlib
 import io
 import os
 import re
 import struct
 import tempfile
-from typing import BinaryIO, Optional
+from typing import IO, Optional
 
 from intelhex import HexRecordError, IntelHex
 
 from .loader import ESPLoader
 from .targets import (
     ESP32C2ROM,
     ESP32C3ROM,
@@ -39,15 +39,15 @@
 
 def align_file_position(f, size):
     """Align the position in the file to the next block of specified size"""
     align = (size - 1) - (f.tell() % size)
     f.seek(align, 1)
 
 
-def intel_hex_to_bin(file: BinaryIO, start_addr: Optional[int] = None) -> BinaryIO:
+def intel_hex_to_bin(file: IO[bytes], start_addr: Optional[int] = None) -> IO[bytes]:
     """Convert IntelHex file to temp binary file with padding from start_addr
     If hex file was detected return temp bin file object; input file otherwise"""
     INTEL_HEX_MAGIC = b":"
     magic = file.read(1)
     file.seek(0)
     try:
         if magic == INTEL_HEX_MAGIC:
@@ -111,18 +111,19 @@
     return select_image_class(image_file, chip)
 
 
 class ImageSegment(object):
     """Wrapper class for a segment in an ESP image
     (very similar to a section in an ELFImage also)"""
 
-    def __init__(self, addr, data, file_offs=None):
+    def __init__(self, addr, data, file_offs=None, flags=0):
         self.addr = addr
         self.data = data
         self.file_offs = file_offs
+        self.flags = flags
         self.include_in_checksum = True
         if self.addr != 0:
             self.pad_to_alignment(
                 4
             )  # pad all "real" ImageSegments 4 byte aligned length
 
     def copy_with_new_addr(self, new_addr):
@@ -163,25 +164,28 @@
         self.data = pad_to(self.data, alignment, b"\x00")
 
 
 class ELFSection(ImageSegment):
     """Wrapper class for a section in an ELF image, has a section
     name as well as the common properties of an ImageSegment."""
 
-    def __init__(self, name, addr, data):
-        super(ELFSection, self).__init__(addr, data)
+    def __init__(self, name, addr, data, flags):
+        super(ELFSection, self).__init__(addr, data, flags=flags)
         self.name = name.decode("utf-8")
 
     def __repr__(self):
         return "%s %s" % (self.name, super(ELFSection, self).__repr__())
 
 
 class BaseFirmwareImage(object):
     SEG_HEADER_LEN = 8
     SHA256_DIGEST_LEN = 32
+    ELF_FLAG_WRITE = 0x1
+    ELF_FLAG_READ = 0x2
+    ELF_FLAG_EXEC = 0x4
 
     """ Base class with common firmware image functions """
 
     def __init__(self):
         self.segments = []
         self.entrypoint = 0
         self.elf_sha256 = None
@@ -348,14 +352,19 @@
             return irom_segments[0]
         return None
 
     def get_non_irom_segments(self):
         irom_segment = self.get_irom_segment()
         return [s for s in self.segments if s != irom_segment]
 
+    def sort_segments(self):
+        if not self.segments:
+            return  # nothing to sort
+        self.segments = sorted(self.segments, key=lambda s: s.addr)
+
     def merge_adjacent_segments(self):
         if not self.segments:
             return  # nothing to merge
 
         segments = []
         # The easiest way to merge the sections is the browse them backward.
         for i in range(len(self.segments) - 1, 0, -1):
@@ -364,14 +373,16 @@
             elem = self.segments[i - 1]
             next_elem = self.segments[i]
             if all(
                 (
                     elem.get_memory_type(self) == next_elem.get_memory_type(self),
                     elem.include_in_checksum == next_elem.include_in_checksum,
                     next_elem.addr == elem.addr + len(elem.data),
+                    next_elem.flags & self.ELF_FLAG_EXEC
+                    == elem.flags & self.ELF_FLAG_EXEC,
                 )
             ):
                 # Merge any segment that ends where the next one starts,
                 # without spanning memory types
                 #
                 # (don't 'pad' any gaps here as they may be excluded from the image
                 # due to 'noinit' or other reasons.)
@@ -751,16 +762,18 @@
                     # Some chips have a non-zero load offset (eg. 0x1000)
                     # therefore we shift the ROM segments "-load_offset"
                     # so it will be aligned properly after it is flashed
                     align_min = (
                         self.ROM_LOADER.BOOTLOADER_FLASH_OFFSET - self.SEG_HEADER_LEN
                     )
                     if pad_len < align_min:
-                        print("Unable to align the segment!")
-                        break
+                        # in case pad_len does not fit minimum alignment,
+                        # pad it to next aligned boundary
+                        pad_len += self.IROM_ALIGN
+
                     pad_len -= self.ROM_LOADER.BOOTLOADER_FLASH_OFFSET
                     pad_segment = ImageSegment(0, b"\x00" * pad_len, f.tell())
                     self.save_segment(f, pad_segment)
                     total_segments += 1
                     # check the alignment
                     assert (f.tell() + 8 + self.ROM_LOADER.BOOTLOADER_FLASH_OFFSET) % (
                         self.IROM_ALIGN
@@ -1265,24 +1278,24 @@
         # walk through the section header and extract all sections
         section_header_offsets = range(0, len(section_header), self.LEN_SEC_HEADER)
 
         def read_section_header(offs):
             name_offs, sec_type, _flags, lma, sec_offs, size = struct.unpack_from(
                 "<LLLLLL", section_header[offs:]
             )
-            return (name_offs, sec_type, lma, size, sec_offs)
+            return (name_offs, sec_type, lma, size, sec_offs, _flags)
 
         all_sections = [read_section_header(offs) for offs in section_header_offsets]
         prog_sections = [s for s in all_sections if s[1] in ELFFile.PROG_SEC_TYPES]
         nobits_secitons = [s for s in all_sections if s[1] == ELFFile.SEC_TYPE_NOBITS]
 
         # search for the string table section
         if (shstrndx * self.LEN_SEC_HEADER) not in section_header_offsets:
             raise FatalError("ELF file has no STRTAB section at shstrndx %d" % shstrndx)
-        _, sec_type, _, sec_size, sec_offs = read_section_header(
+        _, sec_type, _, sec_size, sec_offs, _ = read_section_header(
             shstrndx * self.LEN_SEC_HEADER
         )
         if sec_type != ELFFile.SEC_TYPE_STRTAB:
             print(
                 "WARNING: ELF file has incorrect STRTAB section type 0x%02x" % sec_type
             )
         f.seek(sec_offs)
@@ -1296,22 +1309,22 @@
             return raw[: raw.index(b"\x00")]
 
         def read_data(offs, size):
             f.seek(offs)
             return f.read(size)
 
         prog_sections = [
-            ELFSection(lookup_string(n_offs), lma, read_data(offs, size))
-            for (n_offs, _type, lma, size, offs) in prog_sections
+            ELFSection(lookup_string(n_offs), lma, read_data(offs, size), flags=_flags)
+            for (n_offs, _type, lma, size, offs, _flags) in prog_sections
             if lma != 0 and size > 0
         ]
         self.sections = prog_sections
         self.nobits_sections = [
-            ELFSection(lookup_string(n_offs), lma, b"")
-            for (n_offs, _type, lma, size, offs) in nobits_secitons
+            ELFSection(lookup_string(n_offs), lma, b"", flags=_flags)
+            for (n_offs, _type, lma, size, offs, _flags) in nobits_secitons
             if lma != 0 and size > 0
         ]
 
     def _read_segments(self, f, segment_header_offs, segment_header_count, shstrndx):
         f.seek(segment_header_offs)
         len_bytes = segment_header_count * self.LEN_SEG_HEADER
         segment_header = f.read(len_bytes)
@@ -1336,26 +1349,26 @@
                 _vaddr,
                 lma,
                 size,
                 _memsize,
                 _flags,
                 _align,
             ) = struct.unpack_from("<LLLLLLLL", segment_header[offs:])
-            return (seg_type, lma, size, seg_offs)
+            return (seg_type, lma, size, seg_offs, _flags)
 
         all_segments = [read_segment_header(offs) for offs in segment_header_offsets]
         prog_segments = [s for s in all_segments if s[0] == ELFFile.SEG_TYPE_LOAD]
 
         def read_data(offs, size):
             f.seek(offs)
             return f.read(size)
 
         prog_segments = [
-            ELFSection(b"PHDR", lma, read_data(offs, size))
-            for (_type, lma, size, offs) in prog_segments
+            ELFSection(b"PHDR", lma, read_data(offs, size), flags=_flags)
+            for (_type, lma, size, offs, _flags) in prog_segments
             if lma != 0 and size > 0
         ]
         self.segments = prog_segments
 
     def sha256(self):
         # return SHA256 hash of the input ELF file
         sha256 = hashlib.sha256()
```

### Comparing `esptool-4.8.dev3/esptool/cmds.py` & `esptool-4.8.dev4/esptool/cmds.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import struct
 import sys
 import time
 import zlib
 import itertools
 
 from intelhex import IntelHex
+from serial import SerialException
 
 from .bin_image import ELFFile, ImageSegment, LoadFirmwareImage
 from .bin_image import (
     ESP8266ROMFirmwareImage,
     ESP8266V2FirmwareImage,
     ESP8266V3FirmwareImage,
 )
@@ -112,15 +113,15 @@
                 except UnsupportedCommandError:
                     inst.secure_download_mode = True
                 inst._post_connect()
                 break
         else:
             err_msg = f"Unexpected chip ID value {chip_id}."
     except (UnsupportedCommandError, struct.error, FatalError) as e:
-        # UnsupportedCommmanddError: ESP8266/ESP32 ROM
+        # UnsupportedCommandError: ESP8266/ESP32 ROM
         # struct.error: ESP32-S2
         # FatalError: ESP8266/ESP32 STUB
         print(" Unsupported detection protocol, switching and trying again...")
         try:
             # ESP32/ESP8266 are reset after an unsupported command, need to reconnect
             # (not needed on ESP32-S2)
             if not isinstance(e, struct.error):
@@ -575,64 +576,97 @@
                 "WARNING: Security features enabled, so not changing any flash settings."
             )
         calcmd5 = hashlib.md5(image).hexdigest()
         uncsize = len(image)
         if compress:
             uncimage = image
             image = zlib.compress(uncimage, 9)
-            # Decompress the compressed binary a block at a time,
-            # to dynamically calculate the timeout based on the real write size
-            decompress = zlib.decompressobj()
-            blocks = esp.flash_defl_begin(uncsize, len(image), address)
-        else:
-            blocks = esp.flash_begin(uncsize, address, begin_rom_encrypted=encrypted)
-        argfile.seek(0)  # in case we need it again
-        seq = 0
-        bytes_sent = 0  # bytes sent on wire
-        bytes_written = 0  # bytes written to flash
-        t = time.time()
-
-        timeout = DEFAULT_TIMEOUT
-
-        while len(image) > 0:
-            print_overwrite(
-                "Writing at 0x%08x... (%d %%)"
-                % (address + bytes_written, 100 * (seq + 1) // blocks)
-            )
-            sys.stdout.flush()
-            block = image[0 : esp.FLASH_WRITE_SIZE]
-            if compress:
-                # feeding each compressed block into the decompressor lets us
-                # see block-by-block how much will be written
-                block_uncompressed = len(decompress.decompress(block))
-                bytes_written += block_uncompressed
-                block_timeout = max(
-                    DEFAULT_TIMEOUT,
-                    timeout_per_mb(ERASE_WRITE_TIMEOUT_PER_MB, block_uncompressed),
-                )
-                if not esp.IS_STUB:
-                    timeout = (
-                        block_timeout  # ROM code writes block to flash before ACKing
+        original_image = image  # Save the whole image in case retry is needed
+        # Try again if reconnect was successful
+        for attempt in range(1, esp.WRITE_FLASH_ATTEMPTS + 1):
+            try:
+                if compress:
+                    # Decompress the compressed binary a block at a time,
+                    # to dynamically calculate the timeout based on the real write size
+                    decompress = zlib.decompressobj()
+                    blocks = esp.flash_defl_begin(uncsize, len(image), address)
+                else:
+                    blocks = esp.flash_begin(
+                        uncsize, address, begin_rom_encrypted=encrypted
                     )
-                esp.flash_defl_block(block, seq, timeout=timeout)
-                if esp.IS_STUB:
-                    # Stub ACKs when block is received,
-                    # then writes to flash while receiving the block after it
-                    timeout = block_timeout
-            else:
-                # Pad the last block
-                block = block + b"\xff" * (esp.FLASH_WRITE_SIZE - len(block))
-                if encrypted:
-                    esp.flash_encrypt_block(block, seq)
+                argfile.seek(0)  # in case we need it again
+                seq = 0
+                bytes_sent = 0  # bytes sent on wire
+                bytes_written = 0  # bytes written to flash
+                t = time.time()
+
+                timeout = DEFAULT_TIMEOUT
+
+                while len(image) > 0:
+                    print_overwrite(
+                        "Writing at 0x%08x... (%d %%)"
+                        % (address + bytes_written, 100 * (seq + 1) // blocks)
+                    )
+                    sys.stdout.flush()
+                    block = image[0 : esp.FLASH_WRITE_SIZE]
+                    if compress:
+                        # feeding each compressed block into the decompressor lets us
+                        # see block-by-block how much will be written
+                        block_uncompressed = len(decompress.decompress(block))
+                        bytes_written += block_uncompressed
+                        block_timeout = max(
+                            DEFAULT_TIMEOUT,
+                            timeout_per_mb(
+                                ERASE_WRITE_TIMEOUT_PER_MB, block_uncompressed
+                            ),
+                        )
+                        if not esp.IS_STUB:
+                            timeout = block_timeout  # ROM code writes block to flash before ACKing
+                        esp.flash_defl_block(block, seq, timeout=timeout)
+                        if esp.IS_STUB:
+                            # Stub ACKs when block is received,
+                            # then writes to flash while receiving the block after it
+                            timeout = block_timeout
+                    else:
+                        # Pad the last block
+                        block = block + b"\xff" * (esp.FLASH_WRITE_SIZE - len(block))
+                        if encrypted:
+                            esp.flash_encrypt_block(block, seq)
+                        else:
+                            esp.flash_block(block, seq)
+                        bytes_written += len(block)
+                    bytes_sent += len(block)
+                    image = image[esp.FLASH_WRITE_SIZE :]
+                    seq += 1
+                break
+            except SerialException:
+                if attempt == esp.WRITE_FLASH_ATTEMPTS or encrypted:
+                    # Already retried once or encrypted mode is disabled because of security reasons
+                    raise
+                print("\nLost connection, retrying...")
+                esp._port.close()
+                print("Waiting for the chip to reconnect", end="")
+                for _ in range(DEFAULT_CONNECT_ATTEMPTS):
+                    try:
+                        time.sleep(1)
+                        esp._port.open()
+                        print()  # Print new line which was suppressed by print(".")
+                        esp.connect()
+                        if esp.IS_STUB:
+                            # Hack to bypass the stub overwrite check
+                            esp.IS_STUB = False
+                            # Reflash stub because chip was reset
+                            esp = esp.run_stub()
+                        image = original_image
+                        break
+                    except SerialException:
+                        print(".", end="")
+                        sys.stdout.flush()
                 else:
-                    esp.flash_block(block, seq)
-                bytes_written += len(block)
-            bytes_sent += len(block)
-            image = image[esp.FLASH_WRITE_SIZE :]
-            seq += 1
+                    raise  # Reconnect limit reached
 
         if esp.IS_STUB:
             # Stub only writes each block to flash after 'ack'ing the receive,
             # so do a final dummy operation which will not be 'ack'ed
             # until the last block has actually been written out to flash
             esp.read_reg(ESPLoader.CHIP_DETECT_MAGIC_REG_ADDR, timeout=timeout)
 
@@ -659,15 +693,15 @@
             try:
                 res = esp.flash_md5sum(address, uncsize)
                 if res != calcmd5:
                     print("File  md5: %s" % calcmd5)
                     print("Flash md5: %s" % res)
                     print(
                         "MD5 of 0xFF is %s"
-                        % (hashlib.md5(b"\xFF" * uncsize).hexdigest())
+                        % (hashlib.md5(b"\xff" * uncsize).hexdigest())
                     )
                     raise FatalError("MD5 of file does not match data in flash!")
                 else:
                     print("Hash of data verified.")
             except NotImplementedInROMError:
                 pass
 
@@ -1001,28 +1035,29 @@
 
 def elf2image(args):
     e = ELFFile(args.input)
     if args.chip == "auto":  # Default to ESP8266 for backwards compatibility
         args.chip = "esp8266"
 
     print("Creating {} image...".format(args.chip))
-    if args.ram_only_header:
-        print("ROM segments hidden - only RAM segments are visible to the ROM loader!")
 
     if args.chip != "esp8266":
         image = CHIP_DEFS[args.chip].BOOTLOADER_IMAGE()
         if args.chip == "esp32" and args.secure_pad:
             image.secure_pad = "1"
         if args.secure_pad_v2:
             image.secure_pad = "2"
         image.min_rev = args.min_rev
         image.min_rev_full = args.min_rev_full
         image.max_rev_full = args.max_rev_full
         image.ram_only_header = args.ram_only_header
-        image.append_digest = args.append_digest
+        if image.ram_only_header:
+            image.append_digest = False
+        else:
+            image.append_digest = args.append_digest
     elif args.version == "1":  # ESP8266
         image = ESP8266ROMFirmwareImage()
     elif args.version == "2":
         image = ESP8266V2FirmwareImage()
     else:
         image = ESP8266V3FirmwareImage()
     image.entrypoint = e.entrypoint
@@ -1038,14 +1073,21 @@
     image.flash_size_freq = image.ROM_LOADER.parse_flash_size_arg(args.flash_size)
     image.flash_size_freq += image.ROM_LOADER.parse_flash_freq_arg(args.flash_freq)
 
     if args.elf_sha256_offset:
         image.elf_sha256 = e.sha256()
         image.elf_sha256_offset = args.elf_sha256_offset
 
+    if args.ram_only_header:
+        print(
+            "Image has only RAM segments visible. "
+            "ROM segments are hidden and SHA256 digest is not appended."
+        )
+        image.sort_segments()
+
     before = len(image.segments)
     image.merge_adjacent_segments()
     if len(image.segments) != before:
         delta = before - len(image.segments)
         print("Merged %d ELF section%s" % (delta, "s" if delta > 1 else ""))
 
     image.verify()
@@ -1343,15 +1385,15 @@
         )
 
     elif args.format == "raw":
         with open(args.output, "wb") as of:
 
             def pad_to(flash_offs):
                 # account for output file offset if there is any
-                of.write(b"\xFF" * (flash_offs - args.target_offset - of.tell()))
+                of.write(b"\xff" * (flash_offs - args.target_offset - of.tell()))
 
             for addr, argfile in input_files:
                 pad_to(addr)
                 image = argfile.read()
                 image = _update_image_flash_params(chip_class, addr, args, image)
                 of.write(image)
             if args.fill_flash_size:
```

### Comparing `esptool-4.8.dev3/esptool/config.py` & `esptool-4.8.dev4/esptool/config.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/loader.py` & `esptool-4.8.dev4/esptool/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import json
 import os
 import re
 import string
 import struct
 import sys
 import time
+from typing import Optional
+
 
 from .config import load_config_file
 from .reset import (
     ClassicReset,
     CustomReset,
     DEFAULT_RESET_DELAY,
     HardReset,
@@ -55,15 +57,15 @@
 
 try:
     import serial.tools.list_ports as list_ports
 except ImportError:
     print(
         "The installed version (%s) of pyserial appears to be too old for esptool.py "
         "(Python interpreter %s). Check the README for installation instructions."
-        % (sys.VERSION, sys.executable)
+        % (serial.VERSION, sys.executable)
     )
     raise
 except Exception:
     if sys.platform == "darwin":
         # swallow the exception, this is a known issue in pyserial+macOS Big Sur preview
         # ref https://github.com/espressif/esptool/issues/540
         list_ports = None
@@ -175,20 +177,23 @@
 
 class ESPLoader(object):
     """Base class providing access to ESP ROM & software stub bootloaders.
     Subclasses provide ESP8266 & ESP32 Family specific functionality.
 
     Don't instantiate this base class directly, either instantiate a subclass or
     call cmds.detect_chip() which will interrogate the chip and return the
-    appropriate subclass instance.
+    appropriate subclass instance. You can also use a context manager as
+    "with detect_chip() as esp:" to ensure the serial port is closed when done.
 
     """
 
     CHIP_NAME = "Espressif device"
     IS_STUB = False
+    STUB_CLASS: Optional[object] = None
+    BOOTLOADER_IMAGE: Optional[object] = None
 
     DEFAULT_PORT = "/dev/ttyUSB0"
 
     USES_RFC2217 = False
 
     # Commands supported by ESP8266 ROM bootloader
     ESP_FLASH_BEGIN = 0x02
@@ -269,19 +274,23 @@
 
     # Device PIDs
     USB_JTAG_SERIAL_PID = 0x1001
 
     # Chip IDs that are no longer supported by esptool
     UNSUPPORTED_CHIPS = {6: "ESP32-S3(beta 3)"}
 
+    # Number of attempts to write flash data
+    WRITE_FLASH_ATTEMPTS = 2
+
     def __init__(self, port=DEFAULT_PORT, baud=ESP_ROM_BAUD, trace_enabled=False):
         """Base constructor for ESPLoader bootloader interaction
 
         Don't call this constructor, either instantiate a specific
-        ROM class directly, or use cmds.detect_chip().
+        ROM class directly, or use cmds.detect_chip(). You can use the with
+        statement to ensure the serial port is closed when done.
 
         This base class has all of the instance methods for bootloader
         functionality supported across various chips & stub
         loaders. Subclasses replace the functions they don't support
         with ones which throw NotImplementedInROMError().
 
         """
@@ -357,14 +366,20 @@
         try:
             self._port.write_timeout = DEFAULT_SERIAL_WRITE_TIMEOUT
         except NotImplementedError:
             # no write timeout for RFC2217 ports
             # need to set the property back to None or it will continue to fail
             self._port.write_timeout = None
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        self._port.close()
+
     @property
     def serial_port(self):
         return self._port.port
 
     def _set_port_baudrate(self, baud):
         try:
             self._port.baudrate = baud
```

### Comparing `esptool-4.8.dev3/esptool/reset.py` & `esptool-4.8.dev4/esptool/reset.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/__init__.py` & `esptool-4.8.dev4/esptool/targets/__init__.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/esp32.py` & `esptool-4.8.dev4/esptool/targets/esp32.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/esp32c2.py` & `esptool-4.8.dev4/esptool/targets/esp32c2.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/esp32c3.py` & `esptool-4.8.dev4/esptool/targets/esp32c3.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/esp32c5.py` & `esptool-4.8.dev4/esptool/targets/esp32c5.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from ..loader import ESPLoader
 
 
 class ESP32C5ROM(ESP32C6ROM):
     CHIP_NAME = "ESP32-C5"
     IMAGE_CHIP_ID = 23
 
+    EFUSE_BASE = 0x600B4800
+
     IROM_MAP_START = 0x42000000
     IROM_MAP_END = 0x42800000
     DROM_MAP_START = 0x42800000
     DROM_MAP_END = 0x43000000
 
     PCR_SYSCLK_CONF_REG = 0x60096110
     PCR_SYSCLK_XTAL_FREQ_V = 0x7F << 24
```

### Comparing `esptool-4.8.dev3/esptool/targets/esp32c5beta3.py` & `esptool-4.8.dev4/esptool/targets/esp32c5beta3.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/esp32c6.py` & `esptool-4.8.dev4/esptool/targets/esp32c6.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/esp32c61.py` & `esptool-4.8.dev4/esptool/targets/esp32c61.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/esp32c6beta.py` & `esptool-4.8.dev4/esptool/targets/esp32c6beta.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/esp32h2.py` & `esptool-4.8.dev4/esptool/targets/esp32h2.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/esp32h2beta1.py` & `esptool-4.8.dev4/esptool/targets/esp32h2beta1.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import struct
 
 from .esp32c3 import ESP32C3ROM
 from ..util import FatalError, NotImplementedInROMError
 
+from typing import List
+
 
 class ESP32H2BETA1ROM(ESP32C3ROM):
     CHIP_NAME = "ESP32-H2(beta1)"
     IMAGE_CHIP_ID = 10
 
     IROM_MAP_START = 0x42000000
     IROM_MAP_END = 0x42800000
@@ -62,15 +64,15 @@
 
     PURPOSE_VAL_XTS_AES128_KEY = 4
 
     SUPPORTS_ENCRYPTED_FLASH = True
 
     FLASH_ENCRYPTED_WRITE_ALIGN = 16
 
-    MEMORY_MAP = []
+    MEMORY_MAP: List = []
 
     FLASH_FREQUENCY = {
         "48m": 0xF,
         "24m": 0x0,
         "16m": 0x1,
         "12m": 0x2,
     }
```

### Comparing `esptool-4.8.dev3/esptool/targets/esp32h2beta2.py` & `esptool-4.8.dev4/esptool/targets/esp32h2beta2.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/esp32p4.py` & `esptool-4.8.dev4/esptool/targets/esp32p4.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/esp32s2.py` & `esptool-4.8.dev4/esptool/targets/esp32s2.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/esp32s3.py` & `esptool-4.8.dev4/esptool/targets/esp32s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -348,14 +348,24 @@
             raise SystemExit(1)
 
     def hard_reset(self):
         uses_usb_otg = self.uses_usb_otg()
         if uses_usb_otg:
             self._check_if_can_reset()
 
+        try:
+            # Clear force download boot mode to avoid the chip being stuck in download mode after reset
+            # workaround for issue: https://github.com/espressif/arduino-esp32/issues/6762
+            self.write_reg(
+                self.RTC_CNTL_OPTION1_REG, 0, self.RTC_CNTL_FORCE_DOWNLOAD_BOOT_MASK
+            )
+        except Exception:
+            # Skip if response was not valid and proceed to reset; e.g. when monitoring while resetting
+            pass
+
         print("Hard resetting via RTS pin...")
         HardReset(self._port, uses_usb_otg)()
 
     def change_baud(self, baud):
         ESPLoader.change_baud(self, baud)
 
     def check_spi_connection(self, spi_connection):
```

### Comparing `esptool-4.8.dev3/esptool/targets/esp32s3beta2.py` & `esptool-4.8.dev4/esptool/targets/esp32s3beta2.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/esp8266.py` & `esptool-4.8.dev4/esptool/targets/esp8266.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32.json` & `esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32.json`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32c2.json` & `esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32c2.json`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32c3.json` & `esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32c3.json`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32c5beta3.json` & `esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32c5beta3.json`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32c6.json` & `esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32c6.json`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32c6beta.json` & `esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32c6beta.json`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32h2.json` & `esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32h2.json`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32h2beta1.json` & `esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32h2beta1.json`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32h2beta2.json` & `esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32h2beta2.json`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32p4.json` & `esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32p4.json`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32s2.json` & `esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32s2.json`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32s3.json` & `esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32s3.json`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_32s3beta2.json` & `esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_32s3beta2.json`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/targets/stub_flasher/stub_flasher_8266.json` & `esptool-4.8.dev4/esptool/targets/stub_flasher/stub_flasher_8266.json`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/uf2_writer.py` & `esptool-4.8.dev4/esptool/uf2_writer.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool/util.py` & `esptool-4.8.dev4/esptool/util.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool.egg-info/PKG-INFO` & `esptool-4.8.dev4/esptool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esptool
-Version: 4.8.dev3
+Version: 4.8.dev4
 Summary: A serial utility to communicate & flash code to Espressif chips.
 Home-page: https://github.com/espressif/esptool/
 Author: Fredrik Ahlberg (themadinventor) & Angus Gratton (projectgus) & Espressif Systems
 Author-email: 
 License: GPLv2+
 Project-URL: Documentation, https://docs.espressif.com/projects/esptool/
 Project-URL: Source, https://github.com/espressif/esptool/
```

### Comparing `esptool-4.8.dev3/esptool.egg-info/SOURCES.txt` & `esptool-4.8.dev4/esptool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/esptool.py` & `esptool-4.8.dev4/esptool.py`

 * *Files identical despite different names*

### Comparing `esptool-4.8.dev3/setup.py` & `esptool-4.8.dev4/setup.py`

 * *Files identical despite different names*

