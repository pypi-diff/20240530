# Comparing `tmp/chipsec-1.4.4.0.tar.gz` & `tmp/chipsec-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chipsec-1.4.4.tar", last modified: Mon Dec  2 23:04:05 2019, max compression
+gzip compressed data, was "dist/chipsec-1.5.1.tar", last modified: Sat May 30 01:38:32 2020, max compression
```

## Comparing `chipsec-1.4.4.0.tar` & `chipsec-1.5.1.tar`

### file list

```diff
@@ -1,268 +1,278 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/
--rw-rw-r--   0 user      (1000) user      (1000)     1564 2019-11-21 00:27:16.000000 chipsec-1.4.4/README
--rw-rw-r--   0 user      (1000) user      (1000)     2814 2019-12-02 23:04:05.000000 chipsec-1.4.4/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/drivers/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/drivers/linux/
--rw-rw-r--   0 user      (1000) user      (1000)      205 2019-11-21 00:27:16.000000 chipsec-1.4.4/drivers/linux/AUTHORS
--rw-rw-r--   0 user      (1000) user      (1000)     2866 2019-11-21 00:27:16.000000 chipsec-1.4.4/drivers/linux/README
--rw-rw-r--   0 user      (1000) user      (1000)      855 2019-11-21 00:27:16.000000 chipsec-1.4.4/drivers/linux/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)      238 2019-11-21 00:27:16.000000 chipsec-1.4.4/drivers/linux/dkms.conf
--rw-rw-r--   0 user      (1000) user      (1000)    47067 2019-11-21 00:27:16.000000 chipsec-1.4.4/drivers/linux/chipsec_km.c
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/drivers/linux/include/
--rw-rw-r--   0 user      (1000) user      (1000)     3551 2019-11-21 00:27:16.000000 chipsec-1.4.4/drivers/linux/include/chipsec.h
--rw-rw-r--   0 user      (1000) user      (1000)    17935 2019-11-21 00:27:16.000000 chipsec-1.4.4/drivers/linux/COPYING
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/drivers/linux/amd64/
--rw-rw-r--   0 user      (1000) user      (1000)    15986 2019-11-21 00:27:16.000000 chipsec-1.4.4/drivers/linux/amd64/cpu.asm
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/drivers/linux/i386/
--rw-rw-r--   0 user      (1000) user      (1000)    12845 2019-11-21 00:27:16.000000 chipsec-1.4.4/drivers/linux/i386/cpu.asm
--rw-rw-r--   0 user      (1000) user      (1000)     1181 2019-11-21 00:27:16.000000 chipsec-1.4.4/drivers/linux/WARNING.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/
--rw-rw-r--   0 user      (1000) user      (1000)     3244 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/result_deltas.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/utilcmd/
--rw-rw-r--   0 user      (1000) user      (1000)     4111 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/spd_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     3974 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/ucode_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     3683 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/cmos_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)    15799 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/uefi_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     6862 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/cpu_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     5036 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/ec_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     1581 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/chipset_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     3276 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/io_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     9357 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/mem_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     3881 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/iommu_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     5261 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/interrupts_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     1630 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/spidesc_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     6548 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/spi_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     8068 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/pci_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     3272 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/acpi_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     4353 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/smbios_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     5467 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/vmm_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     2967 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/msr_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     4156 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/msgbus_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     2772 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/deltas_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     5211 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/decode_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     3247 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/desc_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     3260 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/mmcfg_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     8323 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/vmem_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)      776 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3093 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/smbus_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     3399 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/mmio_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     2851 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/tpm_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     4373 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/igd_cmd.py
--rw-rw-r--   0 user      (1000) user      (1000)     4727 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/utilcmd/reg_cmd.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/cfg/
--rw-rw-r--   0 user      (1000) user      (1000)     1565 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/jkt.xml
--rw-rw-r--   0 user      (1000) user      (1000)     9749 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/skx.xml
--rw-rw-r--   0 user      (1000) user      (1000)    11324 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/apl.xml
--rw-rw-r--   0 user      (1000) user      (1000)     1435 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/bdw.xml
--rw-rw-r--   0 user      (1000) user      (1000)     1482 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/hsw.xml
--rw-rw-r--   0 user      (1000) user      (1000)    47348 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/common.xml
--rw-rw-r--   0 user      (1000) user      (1000)    19692 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/kbl.xml
--rw-rw-r--   0 user      (1000) user      (1000)    19884 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/skl.xml
--rw-rw-r--   0 user      (1000) user      (1000)    19732 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/pch_2xx.xml
--rw-rw-r--   0 user      (1000) user      (1000)    12667 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/byt.xml
--rw-rw-r--   0 user      (1000) user      (1000)    16716 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/cfl.xml
--rw-rw-r--   0 user      (1000) user      (1000)     8279 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/common.py
--rw-rw-r--   0 user      (1000) user      (1000)     2164 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/whl.xml
--rw-rw-r--   0 user      (1000) user      (1000)     2191 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/qrk.xml
--rw-rw-r--   0 user      (1000) user      (1000)     2027 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/pch_c60x.xml
--rw-rw-r--   0 user      (1000) user      (1000)    16572 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/pch_3xx.xml
--rw-rw-r--   0 user      (1000) user      (1000)     1733 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/avn.xml
--rw-rw-r--   0 user      (1000) user      (1000)    25489 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/iommu.xml
--rw-rw-r--   0 user      (1000) user      (1000)     3174 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/template.xml
--rw-rw-r--   0 user      (1000) user      (1000)     9953 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/dnv.xml
--rw-rw-r--   0 user      (1000) user      (1000)     2147 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/pch_c61x.xml
--rw-rw-r--   0 user      (1000) user      (1000)    20151 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/glk.xml
--rw-rw-r--   0 user      (1000) user      (1000)     2458 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/cml.xml
--rw-rw-r--   0 user      (1000) user      (1000)    20108 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/pch_1xx.xml
--rw-rw-r--   0 user      (1000) user      (1000)    12770 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/hsx.xml
--rw-rw-r--   0 user      (1000) user      (1000)    12742 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/bdx.xml
--rw-rw-r--   0 user      (1000) user      (1000)    17532 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/pch_495.xml
--rw-rw-r--   0 user      (1000) user      (1000)    17505 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/pch_4xxlp.xml
--rw-rw-r--   0 user      (1000) user      (1000)      894 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     8183 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/chipsec_cfg.xsd
--rw-rw-r--   0 user      (1000) user      (1000)     1561 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/ivt.xml
--rw-rw-r--   0 user      (1000) user      (1000)    13736 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/cht.xml
--rw-rw-r--   0 user      (1000) user      (1000)    23633 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/cfg/pch_c620.xml
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/fuzzing/
--rw-rw-r--   0 user      (1000) user      (1000)    32238 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/fuzzing/primitives.py
--rw-rw-r--   0 user      (1000) user      (1000)      849 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/fuzzing/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3619 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/module_common.py
--rw-rw-r--   0 user      (1000) user      (1000)    14647 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1247 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/command.py
--rw-rw-r--   0 user      (1000) user      (1000)     4628 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/module.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/helper/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/helper/dal/
--rw-rw-r--   0 user      (1000) user      (1000)    16654 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/helper/dal/dalhelper.py
--rw-rw-r--   0 user      (1000) user      (1000)     1220 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/helper/dal/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     6963 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/helper/basehelper.py
--rw-rw-r--   0 user      (1000) user      (1000)    23773 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/helper/oshelper.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/helper/file/
--rw-rw-r--   0 user      (1000) user      (1000)    10756 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/helper/file/filehelper.py
--rw-rw-r--   0 user      (1000) user      (1000)      880 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/helper/file/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/helper/linux/
--rw-rw-r--   0 user      (1000) user      (1000)     1932 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/helper/linux/cores.c
--rw-rw-r--   0 user      (1000) user      (1000)     1211 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/helper/linux/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    48829 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/helper/linux/linuxhelper.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/helper/win/
--rw-rw-r--   0 user      (1000) user      (1000)    45277 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/helper/win/win32helper.py
--rw-rw-r--   0 user      (1000) user      (1000)     1216 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/helper/win/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/helper/rwe/
--rw-rw-r--   0 user      (1000) user      (1000)    43569 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/helper/rwe/rwehelper.py
--rw-rw-r--   0 user      (1000) user      (1000)     1025 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/helper/rwe/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/helper/efi/
--rw-rw-r--   0 user      (1000) user      (1000)    13035 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/helper/efi/efihelper.py
--rw-rw-r--   0 user      (1000) user      (1000)     1231 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/helper/efi/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1179 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/helper/helpers.py
--rw-rw-r--   0 user      (1000) user      (1000)      899 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/helper/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/helper/osx/
--rw-rw-r--   0 user      (1000) user      (1000)    18177 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/helper/osx/osxhelper.py
--rw-rw-r--   0 user      (1000) user      (1000)      759 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/helper/osx/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     5033 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/defines.py
--rw-rw-r--   0 user      (1000) user      (1000)     8679 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/testcase.py
--rw-rw-r--   0 user      (1000) user      (1000)        5 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/VERSION
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/hal/
--rw-rw-r--   0 user      (1000) user      (1000)     3988 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/io.py
--rw-rw-r--   0 user      (1000) user      (1000)     7093 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/iobar.py
--rw-rw-r--   0 user      (1000) user      (1000)     5360 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/virtmem.py
--rw-rw-r--   0 user      (1000) user      (1000)     4985 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/tpm12_commands.py
--rw-rw-r--   0 user      (1000) user      (1000)     5575 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/physmem.py
--rw-rw-r--   0 user      (1000) user      (1000)    84097 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/uefi_common.py
--rw-rw-r--   0 user      (1000) user      (1000)   114000 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/acpi_tables.py
--rw-rw-r--   0 user      (1000) user      (1000)     5426 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/ucode.py
--rw-rw-r--   0 user      (1000) user      (1000)     6270 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/tpm_eventlog.py
--rw-rw-r--   0 user      (1000) user      (1000)   911943 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/pcidb.py
--rw-rw-r--   0 user      (1000) user      (1000)     5934 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/vmm.py
--rw-rw-r--   0 user      (1000) user      (1000)     6188 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/ec.py
--rw-rw-r--   0 user      (1000) user      (1000)    17781 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/spd.py
--rw-rw-r--   0 user      (1000) user      (1000)     3285 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/cmos.py
--rw-rw-r--   0 user      (1000) user      (1000)     8399 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/iommu.py
--rw-rw-r--   0 user      (1000) user      (1000)    10340 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/smbus.py
--rw-rw-r--   0 user      (1000) user      (1000)     9040 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/msgbus.py
--rw-rw-r--   0 user      (1000) user      (1000)     8331 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/igd.py
--rw-rw-r--   0 user      (1000) user      (1000)    18717 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/pci.py
--rw-rw-r--   0 user      (1000) user      (1000)    29909 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/uefi.py
--rw-rw-r--   0 user      (1000) user      (1000)    21452 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/mmio.py
--rw-rw-r--   0 user      (1000) user      (1000)    21939 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/tpm.py
--rw-rw-r--   0 user      (1000) user      (1000)     7398 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/uefi_search.py
--rw-rw-r--   0 user      (1000) user      (1000)    27987 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/spi_uefi.py
--rw-rw-r--   0 user      (1000) user      (1000)     1254 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/spi_jedec_ids.py
--rw-rw-r--   0 user      (1000) user      (1000)     1767 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/cpuid.py
--rw-rw-r--   0 user      (1000) user      (1000)    58299 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/uefi_platform.py
--rw-rw-r--   0 user      (1000) user      (1000)      897 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    21482 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/smbios.py
--rw-rw-r--   0 user      (1000) user      (1000)    29732 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/spi.py
--rw-rw-r--   0 user      (1000) user      (1000)     8895 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/cpu.py
--rw-rw-r--   0 user      (1000) user      (1000)     5968 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/interrupts.py
--rw-rw-r--   0 user      (1000) user      (1000)     7073 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/msr.py
--rw-rw-r--   0 user      (1000) user      (1000)    23656 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/paging.py
--rw-rw-r--   0 user      (1000) user      (1000)      950 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/hal_base.py
--rw-rw-r--   0 user      (1000) user      (1000)    23072 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/acpi.py
--rw-rw-r--   0 user      (1000) user      (1000)    10949 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/hal/spi_descriptor.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/modules/
--rw-rw-r--   0 user      (1000) user      (1000)     5376 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/debugenabled.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/modules/bdw/
--rw-rw-r--   0 user      (1000) user      (1000)      776 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/bdw/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3306 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/memconfig.py
--rw-rw-r--   0 user      (1000) user      (1000)     6190 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/remap.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/modules/snb/
--rw-rw-r--   0 user      (1000) user      (1000)      776 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/snb/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     5017 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/smm_dma.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/modules/byt/
--rw-rw-r--   0 user      (1000) user      (1000)      776 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/byt/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/modules/hsw/
--rw-rw-r--   0 user      (1000) user      (1000)      776 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/hsw/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/modules/ivb/
--rw-rw-r--   0 user      (1000) user      (1000)      776 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/ivb/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      776 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/modules/common/
--rw-rw-r--   0 user      (1000) user      (1000)     3795 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/spi_access.py
--rw-rw-r--   0 user      (1000) user      (1000)     2876 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/spi_desc.py
--rw-rw-r--   0 user      (1000) user      (1000)     2283 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/spi_fdopss.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/modules/common/uefi/
--rw-rw-r--   0 user      (1000) user      (1000)     8662 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/uefi/access_uefispec.py
--rw-rw-r--   0 user      (1000) user      (1000)     9261 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/uefi/s3bootscript.py
--rw-rw-r--   0 user      (1000) user      (1000)      776 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/uefi/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     8266 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/bios_wp.py
--rw-rw-r--   0 user      (1000) user      (1000)     5202 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/bios_smi.py
--rw-rw-r--   0 user      (1000) user      (1000)     7779 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/smrr.py
--rw-rw-r--   0 user      (1000) user      (1000)     2673 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/spd_wd.py
--rw-rw-r--   0 user      (1000) user      (1000)     3571 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/smm.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/modules/common/cpu/
--rw-rw-r--   0 user      (1000) user      (1000)    11923 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/cpu/spectre_v2.py
--rw-rw-r--   0 user      (1000) user      (1000)     3022 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/cpu/cpu_info.py
--rw-rw-r--   0 user      (1000) user      (1000)      520 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/cpu/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2753 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/rtclock.py
--rw-rw-r--   0 user      (1000) user      (1000)     3038 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/spi_lock.py
--rw-rw-r--   0 user      (1000) user      (1000)    19845 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/sgx_check.py
--rw-rw-r--   0 user      (1000) user      (1000)     3388 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/memlock.py
--rw-rw-r--   0 user      (1000) user      (1000)     2405 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/ia32cfg.py
--rw-rw-r--   0 user      (1000) user      (1000)     3979 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/bios_kbrd_buffer.py
--rwxr-xr-x   0 user      (1000) user      (1000)     3582 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/me_mfg_mode.py
--rw-rw-r--   0 user      (1000) user      (1000)      776 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2867 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/bios_ts.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/modules/common/secureboot/
--rw-rw-r--   0 user      (1000) user      (1000)     7971 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/secureboot/variables.py
--rw-rw-r--   0 user      (1000) user      (1000)      776 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/common/secureboot/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/modules/tools/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/modules/tools/uefi/
--rw-rw-r--   0 user      (1000) user      (1000)    21304 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/uefi/s3script_modify.py
--rw-rw-r--   0 user      (1000) user      (1000)     3699 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/uefi/blacklist.json
--rw-rw-r--   0 user      (1000) user      (1000)     7263 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/uefi/blacklist.py
--rw-rw-r--   0 user      (1000) user      (1000)     8006 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/uefi/uefivar_fuzz.py
--rw-rw-r--   0 user      (1000) user      (1000)     9853 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/uefi/whitelist.py
--rw-rw-r--   0 user      (1000) user      (1000)      776 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/uefi/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/modules/tools/cpu/
--rw-rw-r--   0 user      (1000) user      (1000)     5292 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/cpu/sinkhole.py
--rw-rw-r--   0 user      (1000) user      (1000)      870 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/cpu/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/modules/tools/smm/
--rw-rw-r--   0 user      (1000) user      (1000)      155 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/smm/smm_config.ini
--rw-rw-r--   0 user      (1000) user      (1000)     9368 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/smm/rogue_mmio_bar.py
--rw-rw-r--   0 user      (1000) user      (1000)    25381 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/smm/smm_ptr.py
--rw-rw-r--   0 user      (1000) user      (1000)      870 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/smm/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/
--rw-rw-r--   0 user      (1000) user      (1000)     4285 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/msr_fuzz.py
--rw-rw-r--   0 user      (1000) user      (1000)     7150 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/hypercallfuzz.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/vbox/
--rw-rw-r--   0 user      (1000) user      (1000)     1953 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/vbox/vbox_crash_apicbase.py
--rw-rw-r--   0 user      (1000) user      (1000)      776 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/vbox/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/xen/
--rw-rw-r--   0 user      (1000) user      (1000)    10512 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/xen/define.py
--rw-rw-r--   0 user      (1000) user      (1000)     5775 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/xen/hypercallfuzz.py
--rw-rw-r--   0 user      (1000) user      (1000)     1702 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/xen/xsa188.py
--rw-rw-r--   0 user      (1000) user      (1000)      776 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/xen/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    10541 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/xen/hypercall.py
--rw-rw-r--   0 user      (1000) user      (1000)     4979 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/iofuzz.py
--rw-rw-r--   0 user      (1000) user      (1000)     9169 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/common.py
--rw-rw-r--   0 user      (1000) user      (1000)     4291 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/cpuid_fuzz.py
--rw-rw-r--   0 user      (1000) user      (1000)     1603 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/venom.py
--rw-rw-r--   0 user      (1000) user      (1000)     8365 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/pcie_fuzz.py
--rw-rw-r--   0 user      (1000) user      (1000)      776 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/hv/
--rw-rw-r--   0 user      (1000) user      (1000)     6689 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/hv/vmbusfuzz.py
--rw-rw-r--   0 user      (1000) user      (1000)    23154 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/hv/define.py
--rw-rw-r--   0 user      (1000) user      (1000)     5539 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/hv/hypercallfuzz.py
--rw-rw-r--   0 user      (1000) user      (1000)     5858 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/hv/synth_kbd.py
--rw-rw-r--   0 user      (1000) user      (1000)    30817 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/hv/vmbus.py
--rw-rw-r--   0 user      (1000) user      (1000)     5846 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/hv/synth_dev.py
--rw-rw-r--   0 user      (1000) user      (1000)     1504 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/hv/initial_data.json
--rw-rw-r--   0 user      (1000) user      (1000)      776 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/hv/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    19680 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/hv/hypercall.py
--rw-rw-r--   0 user      (1000) user      (1000)     7355 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/vmm/pcie_overlap_fuzz.py
--rw-rw-r--   0 user      (1000) user      (1000)      870 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec/modules/tools/secureboot/
--rw-rw-r--   0 user      (1000) user      (1000)       19 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/secureboot/te.cfg
--rw-rw-r--   0 user      (1000) user      (1000)    21657 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/secureboot/te.py
--rw-rw-r--   0 user      (1000) user      (1000)      870 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/modules/tools/secureboot/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    65146 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/chipset.py
--rw-rw-r--   0 user      (1000) user      (1000)      854 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1181 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/WARNING.txt
--rw-rw-r--   0 user      (1000) user      (1000)     2830 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec/file.py
--rwxr-xr-x   0 user      (1000) user      (1000)    11810 2019-12-02 23:03:57.000000 chipsec-1.4.4/setup.py
--rw-rw-r--   0 user      (1000) user      (1000)  1398825 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec-manual.pdf
--rw-rw-r--   0 user      (1000) user      (1000)      298 2019-12-02 23:04:05.000000 chipsec-1.4.4/README.NO_KERNEL_DRIVER
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec_tools/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-12-02 23:04:05.000000 chipsec-1.4.4/chipsec_tools/windows/
--rw-rw-r--   0 user      (1000) user      (1000)      854 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec_tools/windows/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      854 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec_tools/__init__.py
--rwxr-xr-x   0 user      (1000) user      (1000)    22896 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec_main.py
--rwxr-xr-x   0 user      (1000) user      (1000)     8531 2019-11-21 00:27:16.000000 chipsec-1.4.4/chipsec_util.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.193034 chipsec-1.5.1/
+-rw-rw-r--   0 user      (1000) user      (1000)     2666 2020-05-30 01:38:32.193034 chipsec-1.5.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1564 2020-05-28 20:41:29.894467 chipsec-1.5.1/README
+-rw-rw-r--   0 user      (1000) user      (1000)      298 2020-05-30 01:38:32.193034 chipsec-1.5.1/README.NO_KERNEL_DRIVER
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.153033 chipsec-1.5.1/chipsec/
+-rw-rw-r--   0 user      (1000) user      (1000)        5 2020-05-30 01:28:58.462144 chipsec-1.5.1/chipsec/VERSION
+-rw-rw-r--   0 user      (1000) user      (1000)     1181 2020-05-28 20:41:30.079469 chipsec-1.5.1/chipsec/WARNING.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      854 2020-05-28 20:41:30.079469 chipsec-1.5.1/chipsec/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.154034 chipsec-1.5.1/chipsec/cfg/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.160034 chipsec-1.5.1/chipsec/cfg/8086/
+-rw-rw-r--   0 user      (1000) user      (1000)    15468 2020-05-28 20:41:30.079469 chipsec-1.5.1/chipsec/cfg/8086/apl.xml
+-rw-rw-r--   0 user      (1000) user      (1000)     3216 2020-05-28 20:41:30.079469 chipsec-1.5.1/chipsec/cfg/8086/avn.xml
+-rw-rw-r--   0 user      (1000) user      (1000)     2369 2020-05-28 20:41:30.080469 chipsec-1.5.1/chipsec/cfg/8086/bdw.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    13156 2020-05-28 20:41:30.080469 chipsec-1.5.1/chipsec/cfg/8086/bdx.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    13027 2020-05-28 20:41:30.080469 chipsec-1.5.1/chipsec/cfg/8086/byt.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    18841 2020-05-28 20:41:30.080469 chipsec-1.5.1/chipsec/cfg/8086/cfl.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    14092 2020-05-28 20:41:30.080469 chipsec-1.5.1/chipsec/cfg/8086/cht.xml
+-rw-rw-r--   0 user      (1000) user      (1000)     3227 2020-05-28 20:41:30.081469 chipsec-1.5.1/chipsec/cfg/8086/cml.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    47900 2020-05-28 20:41:30.081469 chipsec-1.5.1/chipsec/cfg/8086/common.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    12419 2020-05-28 20:41:30.081469 chipsec-1.5.1/chipsec/cfg/8086/dnv.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    20240 2020-05-28 20:41:30.082469 chipsec-1.5.1/chipsec/cfg/8086/glk.xml
+-rw-rw-r--   0 user      (1000) user      (1000)     2797 2020-05-28 20:41:30.082469 chipsec-1.5.1/chipsec/cfg/8086/hsw.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    13187 2020-05-28 20:41:30.082469 chipsec-1.5.1/chipsec/cfg/8086/hsx.xml
+-rw-rw-r--   0 user      (1000) user      (1000)     5495 2020-05-30 01:28:58.463144 chipsec-1.5.1/chipsec/cfg/8086/icl.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    25489 2020-05-28 20:41:30.082469 chipsec-1.5.1/chipsec/cfg/8086/iommu.xml
+-rw-rw-r--   0 user      (1000) user      (1000)     2181 2020-05-28 20:41:30.082469 chipsec-1.5.1/chipsec/cfg/8086/ivb.xml
+-rw-rw-r--   0 user      (1000) user      (1000)     1963 2020-05-28 20:41:30.082469 chipsec-1.5.1/chipsec/cfg/8086/ivt.xml
+-rw-rw-r--   0 user      (1000) user      (1000)     1969 2020-05-28 20:41:30.082469 chipsec-1.5.1/chipsec/cfg/8086/jkt.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    20874 2020-05-28 20:41:30.083469 chipsec-1.5.1/chipsec/cfg/8086/kbl.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    22542 2020-05-28 20:41:30.083469 chipsec-1.5.1/chipsec/cfg/8086/pch_1xx.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    20629 2020-05-28 20:41:30.083469 chipsec-1.5.1/chipsec/cfg/8086/pch_2xx.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    17953 2020-05-28 20:41:30.083469 chipsec-1.5.1/chipsec/cfg/8086/pch_3xx.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    17646 2020-05-28 20:41:30.083469 chipsec-1.5.1/chipsec/cfg/8086/pch_3xxlp.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    17151 2020-05-28 20:41:30.083469 chipsec-1.5.1/chipsec/cfg/8086/pch_3xxop.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    18040 2020-05-30 01:28:58.463144 chipsec-1.5.1/chipsec/cfg/8086/pch_495.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    18564 2020-05-28 20:41:30.084469 chipsec-1.5.1/chipsec/cfg/8086/pch_4xxh.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    18115 2020-05-28 20:41:30.084469 chipsec-1.5.1/chipsec/cfg/8086/pch_4xxlp.xml
+-rw-rw-r--   0 user      (1000) user      (1000)     2377 2020-05-28 20:41:30.084469 chipsec-1.5.1/chipsec/cfg/8086/pch_c60x.xml
+-rw-rw-r--   0 user      (1000) user      (1000)     2721 2020-05-28 20:41:30.084469 chipsec-1.5.1/chipsec/cfg/8086/pch_c61x.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    25986 2020-05-28 20:41:30.084469 chipsec-1.5.1/chipsec/cfg/8086/pch_c620.xml
+-rw-rw-r--   0 user      (1000) user      (1000)     2552 2020-05-28 20:41:30.084469 chipsec-1.5.1/chipsec/cfg/8086/qrk.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    15355 2020-05-28 20:41:30.085469 chipsec-1.5.1/chipsec/cfg/8086/sfdp.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    21040 2020-05-28 20:41:30.085469 chipsec-1.5.1/chipsec/cfg/8086/skl.xml
+-rw-rw-r--   0 user      (1000) user      (1000)     3092 2020-05-28 20:41:30.085469 chipsec-1.5.1/chipsec/cfg/8086/skx.xml
+-rw-rw-r--   0 user      (1000) user      (1000)     2570 2020-05-28 20:41:30.085469 chipsec-1.5.1/chipsec/cfg/8086/snb.xml
+-rw-rw-r--   0 user      (1000) user      (1000)     3177 2020-05-28 20:41:30.085469 chipsec-1.5.1/chipsec/cfg/8086/whl.xml
+-rw-rw-r--   0 user      (1000) user      (1000)      894 2020-05-28 20:41:30.085469 chipsec-1.5.1/chipsec/cfg/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8183 2020-05-28 20:41:30.085469 chipsec-1.5.1/chipsec/cfg/chipsec_cfg.xsd
+-rw-rw-r--   0 user      (1000) user      (1000)     3174 2020-05-28 20:41:30.085469 chipsec-1.5.1/chipsec/cfg/template.xml
+-rw-rw-r--   0 user      (1000) user      (1000)    47784 2020-05-28 20:41:30.086470 chipsec-1.5.1/chipsec/chipset.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1247 2020-05-28 20:41:30.086470 chipsec-1.5.1/chipsec/command.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5081 2020-05-28 20:41:30.086470 chipsec-1.5.1/chipsec/defines.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2830 2020-05-28 20:41:30.086470 chipsec-1.5.1/chipsec/file.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.160034 chipsec-1.5.1/chipsec/fuzzing/
+-rw-rw-r--   0 user      (1000) user      (1000)      849 2020-05-28 20:41:30.087469 chipsec-1.5.1/chipsec/fuzzing/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    32238 2020-05-28 20:41:30.087469 chipsec-1.5.1/chipsec/fuzzing/primitives.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.167034 chipsec-1.5.1/chipsec/hal/
+-rw-rw-r--   0 user      (1000) user      (1000)      897 2020-05-28 20:41:30.087469 chipsec-1.5.1/chipsec/hal/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    22794 2020-05-28 20:41:30.088469 chipsec-1.5.1/chipsec/hal/acpi.py
+-rw-rw-r--   0 user      (1000) user      (1000)   112018 2020-05-28 20:41:30.089470 chipsec-1.5.1/chipsec/hal/acpi_tables.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3246 2020-05-28 20:41:30.089470 chipsec-1.5.1/chipsec/hal/cmos.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8556 2020-05-28 20:41:30.089470 chipsec-1.5.1/chipsec/hal/cpu.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1461 2020-05-28 20:41:30.090469 chipsec-1.5.1/chipsec/hal/cpuid.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6190 2020-05-28 20:41:30.090469 chipsec-1.5.1/chipsec/hal/ec.py
+-rw-rw-r--   0 user      (1000) user      (1000)      950 2020-05-28 20:41:30.090469 chipsec-1.5.1/chipsec/hal/hal_base.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8301 2020-05-28 20:41:30.090469 chipsec-1.5.1/chipsec/hal/igd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7613 2020-05-28 20:41:30.090469 chipsec-1.5.1/chipsec/hal/interrupts.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3947 2020-05-28 20:41:30.090469 chipsec-1.5.1/chipsec/hal/io.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7055 2020-05-28 20:41:30.090469 chipsec-1.5.1/chipsec/hal/iobar.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8470 2020-05-28 20:41:30.091469 chipsec-1.5.1/chipsec/hal/iommu.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15935 2020-05-28 20:41:30.091469 chipsec-1.5.1/chipsec/hal/mmio.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8759 2020-05-28 20:41:30.091469 chipsec-1.5.1/chipsec/hal/msgbus.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7177 2020-05-28 20:41:30.091469 chipsec-1.5.1/chipsec/hal/msr.py
+-rw-rw-r--   0 user      (1000) user      (1000)    23634 2020-05-28 20:41:30.092470 chipsec-1.5.1/chipsec/hal/paging.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18408 2020-05-28 20:41:30.092470 chipsec-1.5.1/chipsec/hal/pci.py
+-rw-rw-r--   0 user      (1000) user      (1000)   911943 2020-05-28 20:41:30.099470 chipsec-1.5.1/chipsec/hal/pcidb.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5469 2020-05-28 20:41:30.099470 chipsec-1.5.1/chipsec/hal/physmem.py
+-rw-rw-r--   0 user      (1000) user      (1000)    23216 2020-05-28 20:41:30.099470 chipsec-1.5.1/chipsec/hal/smbios.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10399 2020-05-28 20:41:30.099470 chipsec-1.5.1/chipsec/hal/smbus.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17541 2020-05-30 01:28:58.463144 chipsec-1.5.1/chipsec/hal/spd.py
+-rw-rw-r--   0 user      (1000) user      (1000)    37194 2020-05-28 20:41:30.100470 chipsec-1.5.1/chipsec/hal/spi.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10677 2020-05-28 20:41:30.100470 chipsec-1.5.1/chipsec/hal/spi_descriptor.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1254 2020-05-28 20:41:30.101470 chipsec-1.5.1/chipsec/hal/spi_jedec_ids.py
+-rw-rw-r--   0 user      (1000) user      (1000)    29221 2020-05-28 20:41:30.101470 chipsec-1.5.1/chipsec/hal/spi_uefi.py
+-rw-rw-r--   0 user      (1000) user      (1000)    22275 2020-05-28 20:41:30.101470 chipsec-1.5.1/chipsec/hal/tpm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4857 2020-05-28 20:41:30.101470 chipsec-1.5.1/chipsec/hal/tpm12_commands.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6228 2020-05-28 20:41:30.102470 chipsec-1.5.1/chipsec/hal/tpm_eventlog.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5053 2020-05-28 20:41:30.102470 chipsec-1.5.1/chipsec/hal/ucode.py
+-rw-rw-r--   0 user      (1000) user      (1000)    30647 2020-05-28 20:41:30.102470 chipsec-1.5.1/chipsec/hal/uefi.py
+-rw-rw-r--   0 user      (1000) user      (1000)    84086 2020-05-28 20:41:30.103470 chipsec-1.5.1/chipsec/hal/uefi_common.py
+-rw-rw-r--   0 user      (1000) user      (1000)    58112 2020-05-28 20:41:30.104470 chipsec-1.5.1/chipsec/hal/uefi_platform.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7441 2020-05-28 20:41:30.105470 chipsec-1.5.1/chipsec/hal/uefi_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5345 2020-05-28 20:41:30.105470 chipsec-1.5.1/chipsec/hal/virtmem.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5908 2020-05-28 20:41:30.105470 chipsec-1.5.1/chipsec/hal/vmm.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.168034 chipsec-1.5.1/chipsec/helper/
+-rw-rw-r--   0 user      (1000) user      (1000)      899 2020-05-28 20:41:30.105470 chipsec-1.5.1/chipsec/helper/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6963 2020-05-28 20:41:30.106470 chipsec-1.5.1/chipsec/helper/basehelper.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.168034 chipsec-1.5.1/chipsec/helper/dal/
+-rw-rw-r--   0 user      (1000) user      (1000)     1220 2020-05-28 20:41:30.106470 chipsec-1.5.1/chipsec/helper/dal/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16599 2020-05-28 20:41:30.106470 chipsec-1.5.1/chipsec/helper/dal/dalhelper.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.169034 chipsec-1.5.1/chipsec/helper/efi/
+-rw-rw-r--   0 user      (1000) user      (1000)     1231 2020-05-28 20:41:30.106470 chipsec-1.5.1/chipsec/helper/efi/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12938 2020-05-28 20:41:30.107470 chipsec-1.5.1/chipsec/helper/efi/efihelper.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.169034 chipsec-1.5.1/chipsec/helper/file/
+-rw-rw-r--   0 user      (1000) user      (1000)      880 2020-05-28 20:41:30.107470 chipsec-1.5.1/chipsec/helper/file/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10756 2020-05-28 20:41:30.107470 chipsec-1.5.1/chipsec/helper/file/filehelper.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1179 2020-05-28 20:41:30.107470 chipsec-1.5.1/chipsec/helper/helpers.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.169034 chipsec-1.5.1/chipsec/helper/linux/
+-rw-rw-r--   0 user      (1000) user      (1000)     1211 2020-05-28 20:41:30.108470 chipsec-1.5.1/chipsec/helper/linux/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1932 2020-05-28 20:41:30.108470 chipsec-1.5.1/chipsec/helper/linux/cores.c
+-rw-rw-r--   0 user      (1000) user      (1000)    48572 2020-05-28 20:41:30.108470 chipsec-1.5.1/chipsec/helper/linux/linuxhelper.py
+-rw-rw-r--   0 user      (1000) user      (1000)    23348 2020-05-28 20:41:30.109470 chipsec-1.5.1/chipsec/helper/oshelper.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.170034 chipsec-1.5.1/chipsec/helper/osx/
+-rw-rw-r--   0 user      (1000) user      (1000)      759 2020-05-28 20:41:30.109470 chipsec-1.5.1/chipsec/helper/osx/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17611 2020-05-28 20:41:30.109470 chipsec-1.5.1/chipsec/helper/osx/osxhelper.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.170034 chipsec-1.5.1/chipsec/helper/rwe/
+-rw-rw-r--   0 user      (1000) user      (1000)     1025 2020-05-28 20:41:30.109470 chipsec-1.5.1/chipsec/helper/rwe/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    41247 2020-05-28 20:41:30.110470 chipsec-1.5.1/chipsec/helper/rwe/rwehelper.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.170034 chipsec-1.5.1/chipsec/helper/win/
+-rw-rw-r--   0 user      (1000) user      (1000)     1216 2020-05-28 20:41:30.111470 chipsec-1.5.1/chipsec/helper/win/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    45076 2020-05-28 20:41:30.111470 chipsec-1.5.1/chipsec/helper/win/win32helper.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15749 2020-05-28 20:41:30.111470 chipsec-1.5.1/chipsec/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4905 2020-05-28 20:41:30.112470 chipsec-1.5.1/chipsec/module.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3582 2020-05-28 20:41:30.112470 chipsec-1.5.1/chipsec/module_common.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.171034 chipsec-1.5.1/chipsec/modules/
+-rw-rw-r--   0 user      (1000) user      (1000)      776 2020-05-28 20:41:30.112470 chipsec-1.5.1/chipsec/modules/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.171034 chipsec-1.5.1/chipsec/modules/bdw/
+-rw-rw-r--   0 user      (1000) user      (1000)      776 2020-05-28 20:41:30.112470 chipsec-1.5.1/chipsec/modules/bdw/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.172034 chipsec-1.5.1/chipsec/modules/byt/
+-rw-rw-r--   0 user      (1000) user      (1000)      776 2020-05-28 20:41:30.112470 chipsec-1.5.1/chipsec/modules/byt/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.175034 chipsec-1.5.1/chipsec/modules/common/
+-rw-rw-r--   0 user      (1000) user      (1000)      776 2020-05-28 20:41:30.112470 chipsec-1.5.1/chipsec/modules/common/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3976 2020-05-28 20:41:30.112470 chipsec-1.5.1/chipsec/modules/common/bios_kbrd_buffer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5137 2020-05-28 20:41:30.113470 chipsec-1.5.1/chipsec/modules/common/bios_smi.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2770 2020-05-28 20:41:30.113470 chipsec-1.5.1/chipsec/modules/common/bios_ts.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7488 2020-05-28 20:41:30.113470 chipsec-1.5.1/chipsec/modules/common/bios_wp.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.176034 chipsec-1.5.1/chipsec/modules/common/cpu/
+-rw-rw-r--   0 user      (1000) user      (1000)      520 2020-05-28 20:41:30.113470 chipsec-1.5.1/chipsec/modules/common/cpu/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3063 2020-05-28 20:41:30.113470 chipsec-1.5.1/chipsec/modules/common/cpu/cpu_info.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1774 2020-05-30 01:28:58.464145 chipsec-1.5.1/chipsec/modules/common/cpu/ia_untrusted.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11909 2020-05-28 20:41:30.114470 chipsec-1.5.1/chipsec/modules/common/cpu/spectre_v2.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2386 2020-05-28 20:41:30.114470 chipsec-1.5.1/chipsec/modules/common/ia32cfg.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     3609 2020-05-28 20:41:30.114470 chipsec-1.5.1/chipsec/modules/common/me_mfg_mode.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3338 2020-05-28 20:41:30.114470 chipsec-1.5.1/chipsec/modules/common/memlock.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4770 2020-05-30 01:28:58.464145 chipsec-1.5.1/chipsec/modules/common/rtclock.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.176034 chipsec-1.5.1/chipsec/modules/common/secureboot/
+-rw-rw-r--   0 user      (1000) user      (1000)      776 2020-05-28 20:41:30.115470 chipsec-1.5.1/chipsec/modules/common/secureboot/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8252 2020-05-28 20:41:30.115470 chipsec-1.5.1/chipsec/modules/common/secureboot/variables.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19902 2020-05-28 20:41:30.116470 chipsec-1.5.1/chipsec/modules/common/sgx_check.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3582 2020-05-28 20:41:30.116470 chipsec-1.5.1/chipsec/modules/common/smm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7486 2020-05-28 20:41:30.116470 chipsec-1.5.1/chipsec/modules/common/smrr.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2777 2020-05-28 20:41:30.116470 chipsec-1.5.1/chipsec/modules/common/spd_wd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4257 2020-05-28 20:41:30.116470 chipsec-1.5.1/chipsec/modules/common/spi_access.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2916 2020-05-28 20:41:30.116470 chipsec-1.5.1/chipsec/modules/common/spi_desc.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2317 2020-05-28 20:41:30.117470 chipsec-1.5.1/chipsec/modules/common/spi_fdopss.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3069 2020-05-28 20:41:30.117470 chipsec-1.5.1/chipsec/modules/common/spi_lock.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.177034 chipsec-1.5.1/chipsec/modules/common/uefi/
+-rw-rw-r--   0 user      (1000) user      (1000)      776 2020-05-28 20:41:30.117470 chipsec-1.5.1/chipsec/modules/common/uefi/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8899 2020-05-28 20:41:30.117470 chipsec-1.5.1/chipsec/modules/common/uefi/access_uefispec.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9086 2020-05-28 20:41:30.117470 chipsec-1.5.1/chipsec/modules/common/uefi/s3bootscript.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5376 2020-05-28 20:41:30.118470 chipsec-1.5.1/chipsec/modules/debugenabled.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.177034 chipsec-1.5.1/chipsec/modules/hsw/
+-rw-rw-r--   0 user      (1000) user      (1000)      776 2020-05-28 20:41:30.118470 chipsec-1.5.1/chipsec/modules/hsw/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.177034 chipsec-1.5.1/chipsec/modules/ivb/
+-rw-rw-r--   0 user      (1000) user      (1000)      776 2020-05-28 20:41:30.118470 chipsec-1.5.1/chipsec/modules/ivb/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4372 2020-05-30 01:28:58.464145 chipsec-1.5.1/chipsec/modules/memconfig.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6505 2020-05-30 01:28:58.465144 chipsec-1.5.1/chipsec/modules/remap.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5335 2020-05-30 01:28:58.465144 chipsec-1.5.1/chipsec/modules/smm_dma.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.177034 chipsec-1.5.1/chipsec/modules/snb/
+-rw-rw-r--   0 user      (1000) user      (1000)      776 2020-05-28 20:41:30.119470 chipsec-1.5.1/chipsec/modules/snb/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.177034 chipsec-1.5.1/chipsec/modules/tools/
+-rw-rw-r--   0 user      (1000) user      (1000)      870 2020-05-28 20:41:30.119470 chipsec-1.5.1/chipsec/modules/tools/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.178034 chipsec-1.5.1/chipsec/modules/tools/cpu/
+-rw-rw-r--   0 user      (1000) user      (1000)      870 2020-05-28 20:41:30.119470 chipsec-1.5.1/chipsec/modules/tools/cpu/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5324 2020-05-28 20:41:30.119470 chipsec-1.5.1/chipsec/modules/tools/cpu/sinkhole.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.178034 chipsec-1.5.1/chipsec/modules/tools/secureboot/
+-rw-rw-r--   0 user      (1000) user      (1000)      870 2020-05-28 20:41:30.128470 chipsec-1.5.1/chipsec/modules/tools/secureboot/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)       72 2020-05-28 20:41:30.128470 chipsec-1.5.1/chipsec/modules/tools/secureboot/te.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)    21831 2020-05-28 20:41:30.129470 chipsec-1.5.1/chipsec/modules/tools/secureboot/te.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.179034 chipsec-1.5.1/chipsec/modules/tools/smm/
+-rw-rw-r--   0 user      (1000) user      (1000)      870 2020-05-28 20:41:30.129470 chipsec-1.5.1/chipsec/modules/tools/smm/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9290 2020-05-28 20:41:30.129470 chipsec-1.5.1/chipsec/modules/tools/smm/rogue_mmio_bar.py
+-rw-rw-r--   0 user      (1000) user      (1000)      155 2020-05-28 20:41:30.129470 chipsec-1.5.1/chipsec/modules/tools/smm/smm_config.ini
+-rw-rw-r--   0 user      (1000) user      (1000)    25417 2020-05-28 20:41:30.130470 chipsec-1.5.1/chipsec/modules/tools/smm/smm_ptr.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.180034 chipsec-1.5.1/chipsec/modules/tools/uefi/
+-rw-rw-r--   0 user      (1000) user      (1000)      776 2020-05-28 20:41:30.130470 chipsec-1.5.1/chipsec/modules/tools/uefi/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3699 2020-05-28 20:41:30.130470 chipsec-1.5.1/chipsec/modules/tools/uefi/blacklist.json
+-rw-rw-r--   0 user      (1000) user      (1000)     7331 2020-05-28 20:41:30.130470 chipsec-1.5.1/chipsec/modules/tools/uefi/blacklist.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5930 2020-05-28 20:41:30.130470 chipsec-1.5.1/chipsec/modules/tools/uefi/reputation.py
+-rw-rw-r--   0 user      (1000) user      (1000)    21123 2020-05-28 20:41:30.131470 chipsec-1.5.1/chipsec/modules/tools/uefi/s3script_modify.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8014 2020-05-28 20:41:30.131470 chipsec-1.5.1/chipsec/modules/tools/uefi/uefivar_fuzz.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9860 2020-05-28 20:41:30.131470 chipsec-1.5.1/chipsec/modules/tools/uefi/whitelist.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.182034 chipsec-1.5.1/chipsec/modules/tools/vmm/
+-rw-rw-r--   0 user      (1000) user      (1000)      776 2020-05-28 20:41:30.131470 chipsec-1.5.1/chipsec/modules/tools/vmm/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9211 2020-05-28 20:41:30.132470 chipsec-1.5.1/chipsec/modules/tools/vmm/common.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4401 2020-05-28 20:41:30.132470 chipsec-1.5.1/chipsec/modules/tools/vmm/cpuid_fuzz.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9635 2020-05-28 20:41:30.132470 chipsec-1.5.1/chipsec/modules/tools/vmm/ept_finder.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.183034 chipsec-1.5.1/chipsec/modules/tools/vmm/hv/
+-rw-rw-r--   0 user      (1000) user      (1000)      776 2020-05-28 20:41:30.132470 chipsec-1.5.1/chipsec/modules/tools/vmm/hv/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    23154 2020-05-28 20:41:30.132470 chipsec-1.5.1/chipsec/modules/tools/vmm/hv/define.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19680 2020-05-28 20:41:30.133470 chipsec-1.5.1/chipsec/modules/tools/vmm/hv/hypercall.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5539 2020-05-28 20:41:30.133470 chipsec-1.5.1/chipsec/modules/tools/vmm/hv/hypercallfuzz.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1504 2020-05-28 20:41:30.133470 chipsec-1.5.1/chipsec/modules/tools/vmm/hv/initial_data.json
+-rw-rw-r--   0 user      (1000) user      (1000)     5846 2020-05-28 20:41:30.133470 chipsec-1.5.1/chipsec/modules/tools/vmm/hv/synth_dev.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5858 2020-05-28 20:41:30.133470 chipsec-1.5.1/chipsec/modules/tools/vmm/hv/synth_kbd.py
+-rw-rw-r--   0 user      (1000) user      (1000)    30817 2020-05-28 20:41:30.133470 chipsec-1.5.1/chipsec/modules/tools/vmm/hv/vmbus.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6689 2020-05-28 20:41:30.134470 chipsec-1.5.1/chipsec/modules/tools/vmm/hv/vmbusfuzz.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7157 2020-05-28 20:41:30.134470 chipsec-1.5.1/chipsec/modules/tools/vmm/hypercallfuzz.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4976 2020-05-28 20:41:30.134470 chipsec-1.5.1/chipsec/modules/tools/vmm/iofuzz.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4267 2020-05-28 20:41:30.134470 chipsec-1.5.1/chipsec/modules/tools/vmm/msr_fuzz.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8405 2020-05-28 20:41:30.134470 chipsec-1.5.1/chipsec/modules/tools/vmm/pcie_fuzz.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7392 2020-05-28 20:41:30.134470 chipsec-1.5.1/chipsec/modules/tools/vmm/pcie_overlap_fuzz.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.184034 chipsec-1.5.1/chipsec/modules/tools/vmm/vbox/
+-rw-rw-r--   0 user      (1000) user      (1000)      776 2020-05-28 20:41:30.135470 chipsec-1.5.1/chipsec/modules/tools/vmm/vbox/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1953 2020-05-28 20:41:30.135470 chipsec-1.5.1/chipsec/modules/tools/vmm/vbox/vbox_crash_apicbase.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1611 2020-05-28 20:41:30.135470 chipsec-1.5.1/chipsec/modules/tools/vmm/venom.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.185034 chipsec-1.5.1/chipsec/modules/tools/vmm/xen/
+-rw-rw-r--   0 user      (1000) user      (1000)      776 2020-05-28 20:41:30.135470 chipsec-1.5.1/chipsec/modules/tools/vmm/xen/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10512 2020-05-28 20:41:30.135470 chipsec-1.5.1/chipsec/modules/tools/vmm/xen/define.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10541 2020-05-28 20:41:30.135470 chipsec-1.5.1/chipsec/modules/tools/vmm/xen/hypercall.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5775 2020-05-28 20:41:30.136470 chipsec-1.5.1/chipsec/modules/tools/vmm/xen/hypercallfuzz.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1702 2020-05-28 20:41:30.136470 chipsec-1.5.1/chipsec/modules/tools/vmm/xen/xsa188.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3244 2020-05-28 20:41:30.136470 chipsec-1.5.1/chipsec/result_deltas.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9936 2020-05-28 20:41:30.136470 chipsec-1.5.1/chipsec/testcase.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.189034 chipsec-1.5.1/chipsec/utilcmd/
+-rw-rw-r--   0 user      (1000) user      (1000)      776 2020-05-28 20:41:30.136470 chipsec-1.5.1/chipsec/utilcmd/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3272 2020-05-28 20:41:30.137470 chipsec-1.5.1/chipsec/utilcmd/acpi_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1562 2020-05-28 20:41:30.137470 chipsec-1.5.1/chipsec/utilcmd/chipset_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3683 2020-05-28 20:41:30.137470 chipsec-1.5.1/chipsec/utilcmd/cmos_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6862 2020-05-28 20:41:30.137470 chipsec-1.5.1/chipsec/utilcmd/cpu_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5211 2020-05-28 20:41:30.137470 chipsec-1.5.1/chipsec/utilcmd/decode_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2773 2020-05-28 20:41:30.137470 chipsec-1.5.1/chipsec/utilcmd/deltas_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3247 2020-05-28 20:41:30.137470 chipsec-1.5.1/chipsec/utilcmd/desc_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5008 2020-05-28 20:41:30.138470 chipsec-1.5.1/chipsec/utilcmd/ec_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4351 2020-05-28 20:41:30.138470 chipsec-1.5.1/chipsec/utilcmd/igd_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6580 2020-05-28 20:41:30.138470 chipsec-1.5.1/chipsec/utilcmd/interrupts_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3288 2020-05-28 20:41:30.138470 chipsec-1.5.1/chipsec/utilcmd/io_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3881 2020-05-28 20:41:30.138470 chipsec-1.5.1/chipsec/utilcmd/iommu_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9250 2020-05-28 20:41:30.138470 chipsec-1.5.1/chipsec/utilcmd/mem_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3260 2020-05-28 20:41:30.138470 chipsec-1.5.1/chipsec/utilcmd/mmcfg_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3375 2020-05-28 20:41:30.139470 chipsec-1.5.1/chipsec/utilcmd/mmio_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4156 2020-05-28 20:41:30.139470 chipsec-1.5.1/chipsec/utilcmd/msgbus_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2947 2020-05-28 20:41:30.139470 chipsec-1.5.1/chipsec/utilcmd/msr_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8068 2020-05-28 20:41:30.139470 chipsec-1.5.1/chipsec/utilcmd/pci_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4727 2020-05-28 20:41:30.139470 chipsec-1.5.1/chipsec/utilcmd/reg_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4353 2020-05-28 20:41:30.140470 chipsec-1.5.1/chipsec/utilcmd/smbios_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3093 2020-05-28 20:41:30.140470 chipsec-1.5.1/chipsec/utilcmd/smbus_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4111 2020-05-28 20:41:30.140470 chipsec-1.5.1/chipsec/utilcmd/spd_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7801 2020-05-28 20:41:30.140470 chipsec-1.5.1/chipsec/utilcmd/spi_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1661 2020-05-28 20:41:30.140470 chipsec-1.5.1/chipsec/utilcmd/spidesc_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2852 2020-05-28 20:41:30.140470 chipsec-1.5.1/chipsec/utilcmd/tpm_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3974 2020-05-28 20:41:30.140470 chipsec-1.5.1/chipsec/utilcmd/ucode_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19747 2020-05-28 20:41:30.141470 chipsec-1.5.1/chipsec/utilcmd/uefi_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8323 2020-05-28 20:41:30.141470 chipsec-1.5.1/chipsec/utilcmd/vmem_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5467 2020-05-28 20:41:30.141470 chipsec-1.5.1/chipsec/utilcmd/vmm_cmd.py
+-rw-rw-r--   0 user      (1000) user      (1000)  1398825 2020-05-28 20:41:30.078469 chipsec-1.5.1/chipsec-manual.pdf
+-rwxr-xr-x   0 user      (1000) user      (1000)    23632 2020-05-28 23:09:08.504171 chipsec-1.5.1/chipsec_main.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.190034 chipsec-1.5.1/chipsec_tools/
+-rw-rw-r--   0 user      (1000) user      (1000)      854 2020-05-28 20:41:30.142470 chipsec-1.5.1/chipsec_tools/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.190034 chipsec-1.5.1/chipsec_tools/windows/
+-rw-rw-r--   0 user      (1000) user      (1000)      854 2020-05-28 20:41:30.205471 chipsec-1.5.1/chipsec_tools/windows/__init__.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     9328 2020-05-28 23:09:03.779106 chipsec-1.5.1/chipsec_util.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.150033 chipsec-1.5.1/drivers/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.192034 chipsec-1.5.1/drivers/linux/
+-rw-rw-r--   0 user      (1000) user      (1000)      205 2020-05-28 20:41:30.212471 chipsec-1.5.1/drivers/linux/AUTHORS
+-rw-rw-r--   0 user      (1000) user      (1000)    17935 2020-05-28 20:41:30.212471 chipsec-1.5.1/drivers/linux/COPYING
+-rw-rw-r--   0 user      (1000) user      (1000)      858 2020-05-28 20:41:30.212471 chipsec-1.5.1/drivers/linux/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)     2866 2020-05-28 20:41:30.212471 chipsec-1.5.1/drivers/linux/README
+-rw-rw-r--   0 user      (1000) user      (1000)     1181 2020-05-28 20:41:30.212471 chipsec-1.5.1/drivers/linux/WARNING.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.192034 chipsec-1.5.1/drivers/linux/amd64/
+-rw-rw-r--   0 user      (1000) user      (1000)    15986 2020-05-28 20:41:30.213471 chipsec-1.5.1/drivers/linux/amd64/cpu.asm
+-rw-rw-r--   0 user      (1000) user      (1000)    46393 2020-05-28 20:41:30.213471 chipsec-1.5.1/drivers/linux/chipsec_km.c
+-rw-rw-r--   0 user      (1000) user      (1000)      238 2020-05-28 20:41:30.214471 chipsec-1.5.1/drivers/linux/dkms.conf
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.192034 chipsec-1.5.1/drivers/linux/i386/
+-rw-rw-r--   0 user      (1000) user      (1000)    12845 2020-05-28 20:41:30.214471 chipsec-1.5.1/drivers/linux/i386/cpu.asm
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2020-05-30 01:38:32.192034 chipsec-1.5.1/drivers/linux/include/
+-rw-rw-r--   0 user      (1000) user      (1000)     3551 2020-05-28 20:41:30.214471 chipsec-1.5.1/drivers/linux/include/chipsec.h
+-rwxrwxr-x   0 user      (1000) user      (1000)    11678 2020-05-28 20:41:30.220471 chipsec-1.5.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `chipsec-1.4.4/README` & `chipsec-1.5.1/README`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/PKG-INFO` & `chipsec-1.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: chipsec
-Version: 1.4.4
+Version: 1.5.1
 Summary: CHIPSEC: Platform Security Assessment Framework
 Home-page: https://github.com/chipsec/chipsec
 Author: CHIPSEC Team
 Author-email: chipsec@intel.com
 License: GNU General Public License v2 (GPLv2)
 Download-URL: https://github.com/chipsec/chipsec
 Description: CHIPSEC: Platform Security Assessment Framework
@@ -43,12 +43,9 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Hardware
```

### Comparing `chipsec-1.4.4/drivers/linux/README` & `chipsec-1.5.1/drivers/linux/README`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/drivers/linux/Makefile` & `chipsec-1.5.1/drivers/linux/Makefile`

 * *Files 15% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 	@if [ ! -d $(KERNEL_SRC_DIR) ]; then \
 		echo "Unable to find the Linux source tree."; \
 		exit 1; \
 	fi
 
 chipsec: check_kernel_dir clean
 	nasm -f $(elf-size) -o $(asm-path)/cpu.o $(asm-path)/cpu.asm
-	@if [ `grep -c 'D efi' /proc/kallsyms` != "0" ]; then \
+	@if [ `grep -c 'efi_call' /proc/kallsyms` != "0" ]; then \
 	    make CFLAGS_MODULE=-DHAS_EFI=1 -C $(KERNEL_SRC_DIR) M=${CURDIR} modules; \
 	else \
 	    make -C $(KERNEL_SRC_DIR) M=${CURDIR} modules; \
 	fi
 
 clean: check_kernel_dir
 	make -C $(KERNEL_SRC_DIR) M=${CURDIR} clean
```

### Comparing `chipsec-1.4.4/drivers/linux/chipsec_km.c` & `chipsec-1.5.1/drivers/linux/chipsec_km.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-/* 
+/*
 CHIPSEC: Platform Security Assessment Framework
-Copyright (c) 2010-2018, Intel Corporation
- 
+Copyright (c) 2010-2020, Intel Corporation
+
 This program is free software; you can redistribute it and/or
 modify it under the terms of the GNU General Public License
 as published by the Free Software Foundation; Version 2.
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -13,15 +13,15 @@
 
 You should have received a copy of the GNU General Public License
 along with this program; if not, write to the Free Software
 Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 Contact information:
 chipsec@intel.com
-*/ 
+*/
 
 #include <linux/module.h>
 #include <linux/highmem.h>
 #include <linux/kallsyms.h>
 #include <linux/tty.h>
 #include <linux/ptrace.h>
 #include <linux/version.h>
@@ -32,20 +32,28 @@
 
 #include "include/chipsec.h"
 
 #ifdef HAS_EFI
     #include <linux/efi.h>
 #endif
 
-#define _GNU_SOURCE 
+#define _GNU_SOURCE
 #define CHIPSEC_VER_ 		1
 #define CHIPSEC_VER_MINOR	2
 
 MODULE_LICENSE("GPL");
 
+#if LINUX_VERSION_CODE >= KERNEL_VERSION(2, 6, 25)
+  /* 'ioremap_nocache' was deprecated in kernels >= 5.6, so instead we use 'ioremap' which
+  is no-cache by default since kernels 2.6.25. */
+#    define IOREMAP_NO_CACHE(address, size) ioremap(address, size)
+#else /* KERNEL_VERSION < 2.6.25 */
+#    define IOREMAP_NO_CACHE(address, size) ioremap_nocache(address, size)
+#endif
+
 // function page_is_ram is not exported 
 // for modules, but is available in kallsyms.
 // So we need determine this address using dirty tricks
 int (*guess_page_is_ram)(unsigned long pagenr);
 // same with phys_mem_accesss_prot
 pgprot_t (*guess_phys_mem_access_prot)(struct file *file, unsigned long pfn,
 				       unsigned long size, pgprot_t vma_prot);
@@ -299,15 +307,15 @@
 		        addr = kmap(pfn_to_page(pfn));	
 			return addr;
 		}
 		return __va(phys);
 	}
 
 	// Not RAM, so it is some device (can be bios for example)
-	addr = (void __force *)ioremap_nocache(start, PAGE_SIZE);
+	addr = (void __force *)IOREMAP_NO_CACHE(start, PAGE_SIZE);
     
     if (addr)
     {
         addr = (void *)((unsigned long)addr | (phys & ~PAGE_MASK));
         return addr;
     }
     
@@ -665,50 +673,14 @@
 #else
 	mutex_unlock(&file->f_path.dentry->d_inode->i_mutex);
 #endif 
 
 	return ret;
 }
 
-
-void * patch_apply_ucode(void * ucode_buf)
-{
-	unsigned long long ucode_start;
-
-	printk(KERN_INFO "[chipsec] [patch_apply_ucode] Applying patch in the processor id: %d", smp_processor_id());
-
-	ucode_start = (unsigned long long)ucode_buf;
-	asm volatile("wrmsr" :  : "c"(MSR_IA32_BIOS_UPDT_TRIG),"d"((unsigned int)((ucode_start >> 32) & 0xffffffff)),"a"((unsigned int)(ucode_start & 0xffffffff))); // lo is in eax
-
-
-	return NULL;
-}
-
-void * patch_bios_sign(void * ucode_buf)
-{
-	asm volatile("wrmsr" :  : "c"(MSR_IA32_BIOS_SIGN_ID),"a"((unsigned int)0),"d"((unsigned int)0));
-	return NULL;
-}
-
-void * patch_cpuid_0(void * CPUInfo)
-{
-	unsigned long *pointer;
-	pointer=(unsigned long *) CPUInfo;
-	asm volatile( "cpuid" : "=a"(pointer[0]),"=b"(pointer[1]),"=c"(pointer[2]),"=d"(pointer[3]) : "a"((unsigned int)(1)));
-	return NULL;
-}
-
-void * patch_read_msr(void * CPUInfo)
-{
-	unsigned long *pointer;
-	pointer=(unsigned long *) CPUInfo;
-	asm volatile("rdmsr" : "=a"(pointer[0]), "=d"(pointer[3]) : "c"(MSR_IA32_BIOS_SIGN_ID));
-	return NULL;
-}
-
 #ifdef EFI_NOT_READY
 void print_stat(efi_status_t stat)
 {
     switch (stat) {
         case EFI_SUCCESS:
             printk( KERN_DEBUG "EFI_SUCCESS\n");
             break;
@@ -758,15 +730,15 @@
 	unsigned long ptrbuf[16];
 	unsigned long *ptr = ptrbuf;
 	unsigned short ucode_size;
 	unsigned short thread_id;
 	char *ucode_buf;
 	//unsigned int counter;
 	char small_buffer[6]; //32 bits + char + \0
-	unsigned long CPUInfo[4]={-1};
+	unsigned long CPUInfo[4]={1,0,0,0};
 	void (*apply_ucode_patch_p)(void *info);
 
 	switch(ioctl_num)
 	{
 	case IOCTL_BASE:
 	{
 		return ((IOCTL_RDIO & 0xfffffff0) >> 4);
@@ -833,82 +805,66 @@
 #endif
 	}
 
 	case IOCTL_LOAD_UCODE_PATCH:
 	{
 
 #ifdef CONFIG_X86
+		unsigned long long ucode_start = 0;
+		u32 _eax[2] = {0}, _edx[2] = {0};
 		ucode_size=0;
 
 		printk(KERN_INFO "[chipsec][IOCTL_LOAD_UCODE_UPDATE] Initializing update routine\n");
 
-		/* we just check if the first bytes are in the ok range */
-#if LINUX_VERSION_CODE < KERNEL_VERSION(5,0,0)
-		if (!access_ok(VERIFY_READ, ioctl_param, sizeof(unsigned short))) 
-#else
-		if(!access_ok(ioctl_param,sizeof(unsigned short)))
-#endif	
-		{
-			printk("\n address not in user-mode\n");
-			return -EFAULT;
-		}
-	
 		/* first byte: thread_id */
 		memset(small_buffer, 0x00, 6);
 
 		if ( copy_from_user(&small_buffer, (char *) ioctl_param, sizeof(unsigned char)) > 0 )
 			return -EFAULT;
 
-		thread_id=(unsigned short) small_buffer[0];	
+		thread_id=(unsigned short) small_buffer[0];
 
 		memset(small_buffer, 0x00, 6);
 
 		if ( copy_from_user(&small_buffer, (unsigned char *)(ioctl_param+sizeof(unsigned char)), sizeof(unsigned short)) > 0 )
 			return -EFAULT;
 
 		ucode_size=(unsigned short) *((unsigned short *) small_buffer);
 
 		ucode_buf=kmalloc(ucode_size, GFP_KERNEL);
 		if (!ucode_buf)
 			return -EFAULT;
 
+		ucode_start = (unsigned long long) ucode_start;
 		memset(ucode_buf, 0, ucode_size);
-		
+
 		if ( copy_from_user(ucode_buf, (unsigned char *)(ioctl_param+sizeof(unsigned char)+sizeof(unsigned short)), ucode_size) > 0 )
 			return -EFAULT;
 
+		printk(KERN_INFO "[chipsec] [patch_apply_ucode] Checking current patch ID");
+		rdmsr_on_cpu(thread_id, MSR_IA32_BIOS_SIGN_ID, (u32*)&_eax[0], (u32*)&_edx[0]);
 
-		/* to confirm the received patch is correct, uncomment */
-		/*
-		printk(KERN_INFO "\n");
-		for (counter=0; counter<40; counter++)
-			printk(KERN_INFO "ucode_buf[%d] = 0x%x ",counter, (unsigned char) ucode_buf[counter]);
-		printk(KERN_INFO "\n");
-		printk(KERN_INFO "ucode_buf[%d] = 0x%x ",ucode_size-1, (unsigned char) ucode_buf[ucode_size-1]);
-		*/
+		printk(KERN_INFO "[chipsec] [patch_apply_ucode] Applying patch in the processor id: %d", thread_id);
+		wrmsr_on_cpu(thread_id, MSR_IA32_BIOS_UPDT_TRIG, (u32)ucode_start, (u32)((ucode_start >> 32) & 0xffffffff));
 
-		apply_ucode_patch_p=(void *) patch_apply_ucode;
-		smp_call_function_single(thread_id, apply_ucode_patch_p, ucode_buf, 0);
 		kfree(ucode_buf);
 
-		apply_ucode_patch_p=(void *)patch_bios_sign;
-		smp_call_function_single(thread_id, apply_ucode_patch_p, ucode_buf, 0);
-
-		apply_ucode_patch_p=(void *)patch_cpuid_0;
-		smp_call_function_single(thread_id, apply_ucode_patch_p, CPUInfo, 0);
+		printk(KERN_INFO "[chipsec] [patch_apply_ucode] checking ucode update was loaded..\n");
+		printk(KERN_INFO "[chipsec] [patch_apply_ucode] clear IA32_BIOS_SIGN_ID, CPUID EAX=1, read back IA32_BIOS_SIGN_ID\n" );
 
-		apply_ucode_patch_p=(void *)patch_read_msr;
-		smp_call_function_single(thread_id, apply_ucode_patch_p, CPUInfo, 0);
+		wrmsr_on_cpu(thread_id, MSR_IA32_BIOS_SIGN_ID, (u32)_eax[1], (u32)_edx[1]);
+		apply_ucode_patch_p=(void *)__cpuid__;
+		smp_call_function_single(thread_id, apply_ucode_patch_p, (CPUID_CTX *)CPUInfo,0);
+		rdmsr_on_cpu(thread_id, MSR_IA32_BIOS_SIGN_ID, (u32*)&_eax[1], (u32*)&_edx[1]);
 
-		if (0 != CPUInfo[3])
-			printk(KERN_INFO "[chipsec][IOCTL_LOAD_UCODE_UPDATE] Microcode update loaded (ID != 0)"); 
+		if (_edx[1] != _edx[0])
+			printk(KERN_INFO "[chipsec][IOCTL_LOAD_UCODE_UPDATE] Microcode update loaded (ID != %u)\n", _edx[0]);
 		else
 			printk(KERN_INFO "[chipsec][IOCTL_LOAD_UCODE_UPDATE] Microcode update failed"); 
 
-
 		break;
 #else
 		return -EFAULT;
 #endif
 	}
 
 	case IOCTL_RDMSR:
@@ -917,15 +873,16 @@
 		//OUT params: edx, eax
 #ifdef CONFIG_X86
 
 		numargs = 4;
 		if(copy_from_user((void*)ptrbuf, (void*)ioctl_param, (sizeof(long) * numargs)) > 0)
 			return -EFAULT;
 
-		_rdmsr(ptr[1],&ptr[3],&ptr[2]);
+		rdmsr_on_cpu(ptr[0], ptr[1], (u32*)&ptr[3], (u32*)&ptr[2]);
+		//_rdmsr(ptr[1],&ptr[3],&ptr[2]);
 
 		if(copy_to_user((void*)ioctl_param, (void*)ptrbuf, (sizeof(long) * numargs)) > 0)
 			return -EFAULT;
 		break;
 #else
 		return -EFAULT;
 #endif
@@ -935,15 +892,16 @@
 	{
 		//IN params: threadid, msr_addr, {e,r}dx, {e,r}ax
 #ifdef CONFIG_X86
 		numargs = 4;
 		if(copy_from_user((void*)ptrbuf, (void*)ioctl_param, (sizeof(long) * numargs)) > 0)
 			return -EFAULT;
 
-		_wrmsr(ptr[1],ptr[3],ptr[2]);
+		wrmsr_on_cpu(ptr[0], ptr[1], (u32)ptr[3], (u32)ptr[2]);
+		//_wrmsr(ptr[1],ptr[3],ptr[2]);
 
 		if(copy_to_user((void*)ioctl_param, (void*)ptrbuf, (sizeof(long) * numargs)) > 0)
 			return -EFAULT;
 		break;
 #else
 		return -EFAULT;
 #endif
```

### Comparing `chipsec-1.4.4/drivers/linux/include/chipsec.h` & `chipsec-1.5.1/drivers/linux/include/chipsec.h`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/drivers/linux/COPYING` & `chipsec-1.5.1/drivers/linux/COPYING`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/drivers/linux/amd64/cpu.asm` & `chipsec-1.5.1/drivers/linux/amd64/cpu.asm`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/drivers/linux/i386/cpu.asm` & `chipsec-1.5.1/drivers/linux/i386/cpu.asm`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/drivers/linux/WARNING.txt` & `chipsec-1.5.1/chipsec/WARNING.txt`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/result_deltas.py` & `chipsec-1.5.1/chipsec/result_deltas.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/utilcmd/spd_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/spd_cmd.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/utilcmd/ucode_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/ucode_cmd.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/utilcmd/cmos_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/cmos_cmd.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/utilcmd/cpu_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/cpu_cmd.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/utilcmd/ec_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/ec_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -106,28 +106,27 @@
     def write(self):
         self.logger.log( "[CHIPSEC] EC memory write: offset 0x{:X} = 0x{:X}".format(self.offset, self.wval) )
 
         if self.offset < 0x100: 
             self._ec.write_memory( self.offset, self.wval )
         else:
             self._ec.write_memory_extended( self.offset, self.wval )
-    
+
     def index(self):
 
         if self.offset:
             val = self._ec.read_idx(self.offset)
             self.logger.log( "[CHIPSEC] EC index I/O: reading memory offset 0x{:X}: 0x{:X}".format(self.offset, val) )
         else:
             self.logger.log( "[CHIPSEC] EC index I/O: dumping memory..." )
             mem =[]
             for off in range(0x10000):
                 mem.append(chr(self._ec.read_idx(off)))
             print_buffer(mem)
-            del mem
-    
+
     def run(self):
         t = time.time()
         try:
             self._ec = EC( self.cs )
         except BaseException as msg:
             print (msg)
             return
```

### Comparing `chipsec-1.4.4/chipsec/utilcmd/chipset_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/chipset_cmd.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2015, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 # 
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -17,21 +17,21 @@
 #
 #Contact information:
 #chipsec@intel.com
 #
 
 
 
-""" 
+"""
 usage as a standalone utility:
     >>> chipsec_util platform
 """
 
 from chipsec.command    import BaseCommand
-from chipsec.chipset    import UnknownChipsetError, print_supported_chipsets
+from chipsec.chipset    import UnknownChipsetError
 
 # ###################################################################
 #
 # Chipset/CPU Detection
 #
 # ###################################################################
 class PlatformCommand(BaseCommand):
@@ -40,15 +40,15 @@
     """
 
     def requires_driver(self):
         return True
 
     def run(self):
         try:
-            print_supported_chipsets()
+            self.cs.print_supported_chipsets()
             self.logger.log("")
             self.cs.print_chipset()
             self.cs.print_pch()
         except UnknownChipsetError as msg:
             self.logger.error( msg )
 
 commands = { 'platform': PlatformCommand }
```

### Comparing `chipsec-1.4.4/chipsec/utilcmd/io_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/io_cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -42,20 +42,20 @@
     >>> chipsec_util io list
     >>> chipsec_util io 0x61 1
     >>> chipsec_util io 0x430 byte 0x0
     """
 
     def requires_driver(self):
         # No driver required when printing the util documentation
-        if len(self.argv) < 3:
+        if self.argv[2] == '--help':
             return False
         return True
 
     def run(self):
-        if len(self.argv) < 3:
+        if self.argv[2] == '--help':
             print (PortIOCommand.__doc__)
             return
 
         try:
             _iobar = iobar.IOBAR( self.cs )
         except iobar.IOBARRuntimeError as msg:
             print (msg)
```

### Comparing `chipsec-1.4.4/chipsec/utilcmd/mem_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/mem_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 # 
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -64,15 +64,14 @@
         # No driver required when printing the util documentation
         if len(self.argv) < 3:
             return False
         return True
 
     def dump_region_to_path(self,path,pa_start,pa_end):
         if pa_start >= pa_end: return
-        pa = (pa_start + chipsec.defines.ALIGNED_4KB) & ~chipsec.defines.ALIGNED_4KB
         head_len = pa_start & chipsec.defines.ALIGNED_4KB
         tail_len = pa_end & chipsec.defines.ALIGNED_4KB
         pa = pa_start - head_len + chipsec.defines.ALIGNED_4KB + 1
         fname = os.path.join(path, "m{:016X}.bin".format(pa_start))
         f = open(fname, 'wb')
         end = pa_end - tail_len
 
@@ -85,16 +84,14 @@
 
         # read trailing bytes
         if (tail_len > 0):
             f.write(self.cs.mem.read_physical_mem(end, tail_len))
         f.close()
 
     def run(self):
-        size = 0x100
-
         if len(self.argv) < 3:
             print (MemCommand.__doc__)
             return
 
         op = self.argv[2]
         t = time.time()
```

### Comparing `chipsec-1.4.4/chipsec/utilcmd/iommu_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/iommu_cmd.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/utilcmd/interrupts_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/interrupts_cmd.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,30 +20,37 @@
 #
 
 
 import time
 
 from chipsec.command        import BaseCommand
 from chipsec.hal.interrupts import Interrupts
+import os
+
 
 # ###################################################################
 #
 # CPU Interrupts
 #
 # ###################################################################
+
+
+
 class SMICommand(BaseCommand):
     """
     >>> chipsec_util smi count
     >>> chipsec_util smi <thread_id> <SMI_code> <SMI_data> [RAX] [RBX] [RCX] [RDX] [RSI] [RDI]
+    >>> chipsec_util smi smmc <RT_code_start> <RT_code_end> <GUID> <payload_loc> <payload_file|payload_string>
 
     Examples:
 
     >>> chipsec_util smi count
     >>> chipsec_util smi 0x0 0xDE 0x0
     >>> chipsec_util smi 0x0 0xDE 0x0 0xAAAAAAAAAAAAAAAA ..
+    >>> chipsec_util.py smi smmc 0x79dfe000 0x79efdfff ed32d533-99e6-4209-9cc02d72cdd998a7 0x79dfaaaa payload.bin
     """
     def requires_driver(self):
         # No driver required when printing the util documentation
         if len(self.argv) < 3:
             return False
         return True
 
@@ -62,16 +69,41 @@
         t = time.time()
 
         if 'count' == op:
             self.logger.log( "[CHIPSEC] SMI count:" )
             for tid in range(self.cs.msr.get_cpu_thread_count()):
                 smi_cnt = self.cs.read_register_field('MSR_SMI_COUNT', 'Count', cpu_thread=tid)
                 self.logger.log( "  CPU{:d}: {:d}".format(tid,smi_cnt) )
+        elif 'smmc' == op:
+            if len(self.argv) < 8:
+                print (SMICommand.__doc__)
+                return
+
+            RTC_start = int(self.argv[3],16)
+            RTC_end = int(self.argv[4],16)
+            guid = self.argv[5]
+            payload_loc = int(self.argv[6],16)
+            payload = self.argv[7]
+            if os.path.isfile(payload):
+                f = open(payload,'rb')
+                payload = f.read()
+                f.close()
+
+            self.logger.log("Searching for \'smmc\' in range 0x{:x}-0x{:x}".format(RTC_start,RTC_end))
+            # scan for SMM_CORE_PRIVATE_DATA smmc signature
+            smmc_loc = interrupts.find_smmc(RTC_start,RTC_end)
+            if smmc_loc == 0:
+                self.logger.log(" Couldn't find smmc signature")
+                return
+            self.logger.log("Found \'smmc\' structure at 0x{:x}".format(smmc_loc))
+
+            ReturnStatus = interrupts.send_smmc_SMI(smmc_loc,guid,payload,payload_loc)
+            #TODO Translate ReturnStatus to EFI_STATUS enum
+            self.logger.log("ReturnStatus: {:x}".format(ReturnStatus))
         else:
-            SMI_code_port_value = 0xF
             SMI_data_port_value = 0x0
             if len(self.argv) > 4:
                 thread_id           = int(self.argv[2],16)
                 SMI_code_port_value = int(self.argv[3],16)
                 SMI_data_port_value = int(self.argv[4],16)
                 self.logger.log( "[CHIPSEC] Sending SW SMI (code: 0x{:02X}, data: 0x{:02X})..".format(SMI_code_port_value, SMI_data_port_value) )
                 if 5 == len(self.argv):
```

### Comparing `chipsec-1.4.4/chipsec/utilcmd/spidesc_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/spidesc_cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2015, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 # 
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -20,29 +20,29 @@
 #
 
 
 import time
 
 from chipsec.command            import BaseCommand
 from chipsec.file               import read_file
-from chipsec.hal.spi_descriptor import *
+from chipsec.hal.spi_descriptor import parse_spi_flash_descriptor
 
 class SPIDescCommand(BaseCommand):
     """
     >>> chipsec_util spidesc [rom]
 
     Examples:
 
     >>> chipsec_util spidesc spi.bin
     """
     def requires_driver(self):
         return False
 
     def run(self):
-        if len(self.argv) < 3:
+        if self.argv[2] == '--help':
             print (SPIDescCommand.__doc__)
             return
 
         fd_file = self.argv[2]
         self.logger.log( "[CHIPSEC] Parsing SPI Flash Descriptor from file '{}'\n".format(fd_file) )
 
         t = time.time()
```

### Comparing `chipsec-1.4.4/chipsec/utilcmd/spi_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/spi_cmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2018, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -47,14 +47,15 @@
     Examples:
 
     >>> chipsec_util spi info
     >>> chipsec_util spi dump rom.bin
     >>> chipsec_util spi read 0x700000 0x100000 bios.bin
     >>> chipsec_util spi write 0x0 flash_descriptor.bin
     >>> chipsec_util spi disable-wp
+    >>> chipsec_util spi sfdp
     >>> chipsec_util spi jedec
     >>> chipsec_util spi jedec decode
     """
     def requires_driver(self):
         # No driver required when printing the util documentation
         if len(self.argv) < 3:
             return False
@@ -69,40 +70,57 @@
             _spi = SPI( self.cs )
         except SpiRuntimeError as msg:
             print (msg)
             return
 
         spi_op = self.argv[2]
 
+        if spi_op in ['read', 'write','erase'] and len(self.argv) < 4:
+             print (SPICommand.__doc__)
+             return
         t = time.time()
 
         _msg = "it may take a few minutes (use DEBUG or VERBOSE logger options to see progress)"
         if ( 'erase' == spi_op ):
             spi_fla = int(self.argv[3],16)
             self.logger.log( "[CHIPSEC] erasing SPI flash memory block at FLA = 0x{:X}".format(spi_fla) )
 
             ok = _spi.erase_spi_block( spi_fla )
             if ok: self.logger.log_result( "completed SPI flash memory erase" )
             else:  self.logger.warn( "SPI flash erase returned error (turn on VERBOSE)" )
         elif ( 'write' == spi_op and 5 == len(self.argv) ):
             spi_fla = int(self.argv[3],16)
-            filename = self.argv[4]
-            self.logger.log( "[CHIPSEC] writing to SPI flash memory at FLA = 0x{:X} from '{:64}'".format(spi_fla, filename) )
+            if 5 == len(self.argv):
+                filename = self.argv[4]
+                if not os.path.exists(filename):
+                    self.logger.error( "File {} doesn't exist".format(filename))
+                    return
+            else:
+                 print (SPICommand.__doc__)
+                 return
+            self.logger.log( "[CHIPSEC] writing to SPI flash memory at FLA = 0x{:X} from '{:64s}'".format(spi_fla, filename) )
 
             ok = _spi.write_spi_from_file( spi_fla, filename )
             if ok: self.logger.log( "[CHIPSEC] completed SPI flash memory write" )
             else:  self.logger.warn( "SPI flash write returned error (turn on VERBOSE)" )
         elif ( 'read' == spi_op ):
             spi_fla = int(self.argv[3],16)
-            length = int(self.argv[4],16)
-            self.logger.log( "[CHIPSEC] reading 0x{:X} bytes from SPI Flash starting at FLA = 0x{:X}".format(length, spi_fla) )
+            if 5 == len(self.argv):
+                length = int(self.argv[4],16)
+            else:
+                length = 0x4
+            self.logger.log( "[CHIPSEC] reading 0x{:x} bytes from SPI Flash starting at FLA = 0x{:X}".format(length, spi_fla) )
             self.logger.log( "[CHIPSEC] {}".format(_msg) )
             out_file = None
             if 6 == len(self.argv):
-                out_file = self.argv[5]
+                if os.path.exists(self.argv[5]):
+                    out_file = self.argv[5]
+                else:
+                    self.logger.error( "File {} doesn't exist".format(self.argv[5]))
+                    return
             buf = _spi.read_spi_to_file( spi_fla, length, out_file )
             if (buf is None): self.logger.error( "SPI flash read didn't return any data (turn on VERBOSE)" )
             else: self.logger.log( "[CHIPSEC] completed SPI flash memory read" )
         elif ( 'info' == spi_op ):
             self.logger.log( "[CHIPSEC] SPI flash memory information\n" )
             _spi.display_SPI_map()
         elif ( 'dump' == spi_op ):
@@ -127,22 +145,34 @@
             #
             if _spi.disable_BIOS_write_protection():
                 self.logger.log_good( "BIOS region write protection is disabled in SPI flash" )
             else:
                 self.logger.log_bad( "couldn't disable BIOS region write protection in SPI flash" )
         elif ( 'jedec' == spi_op ):
             if ( len(self.argv) < 4 ):
-                self.logger.log( '    JEDEC ID: 0x{:06X}'.format(_spi.get_SPI_JEDEC_ID()) )
-                self.logger.log( '' )
+                jedec_id = _spi.get_SPI_JEDEC_ID()
+                if jedec_id is not False:
+                    self.logger.log( '    JEDEC ID: 0x{:06X}'.format(jedec_id) )
+                else:
+                    self.logger.log( ' JEDEC ID command is not supported ')
             else:
-                (jedec, man, part) = _spi.get_SPI_JEDEC_ID_decoded()
-                self.logger.log( '    JEDEC ID     : 0x{:06X}'.format(jedec) )
-                self.logger.log( '    Manufacturer : 0x{:02X}     - {}'.format( (jedec >> 16) & 0xFF , man) )
-                self.logger.log( '    Device       : 0x{:04X}   - {}'.format(jedec & 0xFFFF, part) )
-                self.logger.log( '' )
+                if 'decode' == self.argv[3]:
+                    (jedec, man, part) = _spi.get_SPI_JEDEC_ID_decoded()
+                    if jedec is not False:
+                        self.logger.log( '    JEDEC ID     : 0x{:06X}'.format(jedec) )
+                        self.logger.log( '    Manufacturer : 0x{:02X}     - {}'.format( (jedec >> 16) & 0xFF , man) )
+                        self.logger.log( '    Device       : 0x{:04X}   - {}'.format(jedec & 0xFFFF, part) )
+                        self.logger.log( '' )
+                    else:
+                        self.logger.log( ' JEDEC ID command is not supported ')
+                else:
+                    print (SPICommand.__doc__)
+                    return
+        elif ( 'sfdp' == spi_op):
+            _spi.get_SPI_SFDP()
         else:
             print (SPICommand.__doc__)
             return
 
         self.logger.log( "[CHIPSEC] (spi {}) time elapsed {:.3f}".format(spi_op, time.time()-t) )
 
 commands = { 'spi': SPICommand }
```

### Comparing `chipsec-1.4.4/chipsec/utilcmd/pci_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/pci_cmd.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/utilcmd/acpi_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/acpi_cmd.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/utilcmd/smbios_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/smbios_cmd.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/utilcmd/vmm_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/vmm_cmd.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/utilcmd/msr_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/msr_cmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2015, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 # 
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -37,24 +37,23 @@
     Examples:
 
     >>> chipsec_util msr 0x3A
     >>> chipsec_util msr 0x8B 0x0 0x0 0
     """
     def requires_driver(self):
         # No driver required when printing the util documentation
-        if len(self.argv) < 3:
+        if self.argv[2] == '--help':
             return False
         return True
 
     def run(self):
-        if len(self.argv) < 3:
+        if self.argv[2] == '--help':
             print (MSRCommand.__doc__)
             return
 
-        #msr = Msr( os_helper )
         msr_addr = int(self.argv[2],16)
 
         if (3 == len(self.argv)):
             for tid in range(self.cs.msr.get_cpu_thread_count()):
                 (eax, edx) = self.cs.msr.read_msr( tid, msr_addr )
                 val64 = ((edx << 32) | eax)
                 self.logger.log( "[CHIPSEC] CPU{:d}: RDMSR( 0x{:x} ) = {:016X} (EAX={:08X}, EDX={:08X})".format(tid, msr_addr, val64, eax, edx) )
```

### Comparing `chipsec-1.4.4/chipsec/utilcmd/msgbus_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/msgbus_cmd.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/utilcmd/deltas_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/deltas_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,17 @@
     >>> chipsec_util deltas run1.json run2.json
 
     """
 
     def requires_driver(self):
         parser = ArgumentParser(usage=DeltasCommand.__doc__)
         parser.add_argument('_prev_log', metavar='<previous>', help='previous log file')
-        parser.add_argument('_cur_log', metavar='<current', help='current log file')
-        parser.add_argument('_out-format', metavar='out-format', choices=['JSON','XML'], default='JSON', help='output format')
-        parser.add_argument('_out-name', metavar='out-name', nargs='?', default=None, help='output filename')
+        parser.add_argument('_cur_log', metavar='<current>', help='current log file')
+        parser.add_argument('_out_format', metavar='out-format', choices=['JSON','XML'], default='JSON', help='output format')
+        parser.add_argument('_out_name', metavar='out-name', nargs='?', default=None, help='output filename')
         parser.parse_args(self.argv[2:], namespace=self)
         return False
 
     def run(self):
         start_time = time()
 
         # Read files and determine deltas
```

### Comparing `chipsec-1.4.4/chipsec/utilcmd/decode_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/decode_cmd.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/utilcmd/desc_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/desc_cmd.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/utilcmd/mmcfg_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/mmcfg_cmd.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/utilcmd/vmem_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/vmem_cmd.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/utilcmd/__init__.py` & `chipsec-1.5.1/chipsec/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/utilcmd/smbus_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/smbus_cmd.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/utilcmd/mmio_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/mmio_cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2015, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 # 
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -55,15 +55,14 @@
     def requires_driver(self):
         # No driver required when printing the util documentation
         if len(self.argv) < 3:
             return False
         return True
 
     def run(self):
-        t = time.time()
         _mmio = mmio.MMIO(self.cs)
 
         if len(self.argv) < 3:
             print (MMIOCommand.__doc__)
             return
 
         op = self.argv[2]
```

### Comparing `chipsec-1.4.4/chipsec/utilcmd/tpm_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/tpm_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,23 +52,24 @@
         if len(self.argv) < 4:
             return False
         if self.argv[2] in self.no_driver_cmd:
             return False
         return True
 
     def run(self):
+        if len(self.argv) < 4:
+            print (TPMCommand.__doc__)
+            return
+
         try:
             _tpm = tpm.TPM(self.cs)
         except tpm.TpmRuntimeError as msg:
             print(msg)
             return
 
-        if len(self.argv) < 4:
-            print (TPMCommand.__doc__)
-            return
         op = self.argv[2]
         if ( 'parse_log' == op ):
             log = open(self.argv[3],'rb')
             tpm_eventlog.parse(log)
         elif ('command' == op ):
             if len(self.argv) < 5:
                 print (TPMCommand.__doc__)
```

### Comparing `chipsec-1.4.4/chipsec/utilcmd/igd_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/igd_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2017, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 # 
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -50,16 +50,14 @@
     def requires_driver(self):
         # No driver required when printing the util documentation
         if len(self.argv) < 3:
             return False
         return True
 
     def run(self):
-        size = 0x100
-
         if len(self.argv) < 3:
             print (IgdCommand.__doc__)
             return
 
         if not self.cs.igd.is_device_enabled():
             self.logger.log( '[CHIPSEC] Looks like internal graphics device is not enabled' )
             return
```

### Comparing `chipsec-1.4.4/chipsec/utilcmd/reg_cmd.py` & `chipsec-1.5.1/chipsec/utilcmd/reg_cmd.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/cfg/jkt.xml` & `chipsec-1.5.1/chipsec/cfg/8086/jkt.xml`

 * *Files 13% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/jkt.xml` & `chipsec-1.5.1/chipsec/cfg/8086/jkt.xml`

```diff
@@ -1,12 +1,20 @@
 <?xml version="1.0" encoding="utf-8"?>
 <configuration platform="JKT">
   <!--
 XML configuration file for Jaketown (Sandy Bridge-E) based platforms
 -->
+  <!-- #################################### -->
+  <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info family="xeon">
+    <sku did="0x3C00" name="Jaketown" code="JKT" longname="Server 2nd Generation Core Processor (Jaketown CPU / Patsburg PCH)"/>
+  </info>
   <registers>
     <!-- B:D.F 00:12.6 -->
     <register name="PCI0.0.0_SMRAMC" type="pcicfg" bus="0" dev="12" fun="6" offset="0x4c" size="1" desc="System Management RAM Control">
       <field name="D_OPEN" bit="6" size="1"/>
       <field name="D_CLS" bit="5" size="1"/>
       <field name="D_LCK" bit="4" size="1"/>
       <field name="G_SMRAME" bit="3" size="1"/>
```

### Comparing `chipsec-1.4.4/chipsec/cfg/skx.xml` & `chipsec-1.5.1/chipsec/cfg/8086/bdx.xml`

 * *Files 19% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/skx.xml` & `chipsec-1.5.1/chipsec/cfg/8086/bdx.xml`

```diff
@@ -1,151 +1,189 @@
 <?xml version="1.0" encoding="utf-8"?>
-<configuration platform="SKX">
+<configuration platform="BDX">
   <!--
-XML configuration file for Skylake/Purely Server
-Intel (c) Xeon Processor Scalable Family datasheet Vol. 2
-Intel (c) C620 Series Chipset Platform Controller Hub datasheet
+XML configuration file for Broadwell Server based platforms
+Intel (c) Xeon Processor E5 v4 Product Family datasheet Vol. 2
+Intel (c) Xeon Processor E7 v4 Product Family datasheet Vol. 2
+Intel (c) C600 Series Chipset and Intel (c) X79 Express Chipset datasheet
+Intel (c) C600 Series Chipset and Intel (c) X79 Express Chipset Specification Update
+Intel (c) C610 Series Chipset and Intel (c) X99 Chipset Platform Controller Hub (PCH) datasheet
 -->
+  <!-- #################################### -->
+  <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info family="xeon">
+    <sku did="0x6F00" name="Broadwell Server" code="BDX" longname="Intel Xeon Processor E5/E7 v4 (Broadwell Server CPU / Wellsburg PCH)"/>
+  </info>
   <pci>
-    <device name="P2SBC" bus="0" dev="0x1F" fun="1" vid="0x8086" did="0xA220,0xA1A0"/>
-    <device name="PMC" bus="0" dev="0x1F" fun="2" vid="0x8086" did="0xA221,0xA1A1"/>
-    <device name="SMBUS" bus="0" dev="0x1F" fun="4" vid="0x8086" did="0xA223,0xA1A3"/>
-    <device name="SPI" bus="0" dev="0x1F" fun="5" vid="0x8086" did="0xA224,0xA1A4"/>
+    <device name="VTD_MEM_SM" bus="0" dev="0x5" fun="0" vid="0x8086" did="0x2F28"/>
+    <device name="LPC" bus="0" dev="0x1F" fun="0" vid="0x8086" did="0x8D44,0x8D47,0x1D41"/>
+    <device name="IMC0_MAIN_SMBUS" bus="0x17" dev="0x13" fun="0" vid="0x8086" did="0x2FA8"/>
+    <device name="IMC1_MAIN_SMBUS" bus="0x17" dev="0x16" fun="0" vid="0x8086" did="0x2F68"/>
   </pci>
   <mmio>
     <bar name="MMCFG" bus="0" dev="5" fun="0" reg="0x90" width="8" mask="0x7FFFFFC000000" size="0x1000" desc="PCI Express Register Range"/>
     <bar name="DMIBAR" bus="0" dev="0" fun="0" reg="0x50" width="4" mask="0xFFFFF000" size="0x1000" enable_bit="0" desc="Root Complex Register Range"/>
-    <bar name="PWRMBASE" bus="0" dev="0x1F" fun="2" reg="0x48" width="4" mask="0xFFFFF000" size="0x1000" desc="PM Base Address"/>
-    <bar name="TCO_BAR" bus="0" dev="0x1F" fun="4" reg="0x50" width="4" mask="0xFFE0" size="0x1000" desc="TCO Base Register Register Range"/>
-    <bar name="SPIBAR" bus="0" dev="0x1F" fun="5" reg="0x10" width="4" mask="0xFFFFF000" size="0x1000" desc="SPI Controller Register Range"/>
-    <bar name="SBREGBAR" register="SBREG_BAR" base_field="RBA" size="0x1000000" desc="Sideband Register Access BAR"/>
   </mmio>
   <io/>
   <memory/>
   <registers>
-    <!-- PCH -->
-    <register name="ABAR" type="pcicfg" bus="0" dev="0x17" fun="0" offset="0x24" size="4" desc="AHCI Base Address">
-      <field name="BA" bit="19" size="13" desc="Base Address"/>
+    <!-- Host Controller -->
+    <register name="DMIRCBAR" type="pcicfg" bus="0" dev="0" fun="0" offset="0x50" size="4" desc="DMI Root Complex Register Block Base Address">
+      <field name="dmircbaren" bit="0" size="1" desc="Enable DMIRCBAR"/>
+      <field name="dmircbar" bit="12" size="20" desc="Base address DMI Root Complex register space"/>
     </register>
-    <register name="SATAGC" type="pcicfg" bus="0" dev="0x17" fun="0" offset="0x9C" size="4" desc="SATA General Configuration">
-      <field name="ASSEL" bit="0" size="3" desc="ABAR Size Select"/>
-    </register>
-    <!-- Sideband Register Access Registers -->
-    <register name="SBREG_BAR" type="pcicfg" device="P2SBC" offset="0x10" size="4" desc="Sideband Register Access BAR">
-      <field name="RBA" bit="24" size="8" desc="Register Base Address"/>
-    </register>
-    <register name="SBREG_BARH" type="pcicfg" device="P2SBC" offset="0x14" size="4" desc="Sideband Register Access BAR High DWORD">
-      <field name="RBAH" bit="0" size="32" desc="Register Base Address"/>
-    </register>
-    <register name="P2SBC" type="pcicfg" device="P2SBC" offset="0xE0" size="4" desc="P2SB Configuration Register">
-      <field name="HIDE" bit="8" size="1" desc="Hide SBREG_BAR"/>
-    </register>
-    <register name="P2SB_HIDE" type="pcicfg" device="P2SBC" offset="0xE1" size="1" desc="P2SB Configuration Register hide-unhide">
-      <field name="HIDE" bit="0" size="1" desc="Hide SBREG_BAR"/>
-    </register>
-    <!-- MMCFG -->
-    <register name="MMCFG_BASE" type="pcicfg" bus="0" dev="5" fun="0" offset="0x90" size="8" desc="MMCFG Address Base">
-      <field name="mmcfg_base_addr" bit="26" size="25" desc="MMCFG Base Address"/>
-    </register>
-    <register name="MMCFG_LIMIT" type="pcicfg" bus="0" dev="5" fun="0" offset="0x98" size="8" desc="MMCFG Address Limit">
-      <field name="mmcfg_limit_addr" bit="26" size="25" desc="MMCFG Limit Address"/>
-    </register>
-    <register name="TSEG" type="pcicfg" bus="0" dev="5" fun="0" offset="0xA8" size="8" desc="TSEG Memory">
+    <register name="TSEG" type="pcicfg" device="VTD_MEM_SM" offset="0xA8" size="8" desc="TSEG Memory">
       <field name="base" bit="20" size="12" desc="Base address"/>
       <field name="limit" bit="52" size="12" desc="Limit address"/>
     </register>
-    <register name="TSEG_BASE" type="pcicfg" bus="0" dev="5" fun="0" offset="0xA8" size="4" desc="TSEG Memory Base">
+    <register name="TSEG_BASE" type="pcicfg" device="VTD_MEM_SM" offset="0xA8" size="4" desc="TSEG Memory Base">
       <field name="base" bit="20" size="12" desc="Base address"/>
     </register>
-    <register name="TSEG_LIMIT" type="pcicfg" bus="0" dev="5" fun="0" offset="0xAC" size="4" desc="TSEG Memory Limit">
+    <register name="TSEG_LIMIT" type="pcicfg" device="VTD_MEM_SM" offset="0xAC" size="4" desc="TSEG Memory Limit">
       <field name="limit" bit="20" size="12" desc="Limit address"/>
     </register>
-    <register name="TOLM" type="pcicfg" bus="0" dev="5" fun="0" offset="0xD0" size="4" desc="Top of Low Memory">
-      <field name="addr" bit="26" size="6" desc="TOLM address"/>
-    </register>
-    <register name="TOHM" type="pcicfg" bus="0" dev="5" fun="0" offset="0xD8" size="8" desc="Top of High Memory">
-      <field name="addr" bit="26" size="38" desc="TOHM address"/>
+    <register name="VTBAR" type="mmcfg" device="VTD_MEM_SM" offset="0x180" size="4" desc="VT BAR Register">
+      <field name="Enable" bit="0" size="1" desc="Enable"/>
+      <field name="Base" bit="13" size="19" desc="VTD Base Address"/>
+    </register>
+    <register name="VTGENCTRL" type="mmcfg" device="VTD_MEM_SM" offset="0x184" size="4" desc="VTGENCTRL Register">
+      <field name="gpa_limit" bit="0" size="4" desc="Guest virtual addressing limit"/>
+      <field name="hpa_limit" bit="4" size="4" desc="Host processor addressing limit"/>
+      <field name="lockvtd" bit="15" size="1" desc="lockvtd"/>
+    </register>
+    <register name="LTDPR" type="mmcfg" device="VTD_MEM_SM" offset="0x290" size="4" desc="Intel TXT DMA Protected Range Register">
+      <field name="lock" bit="0" size="1" desc="Lock LTDPR register"/>
+      <field name="protregsts" bit="1" size="1" desc="Protection enabled in HW"/>
+      <field name="commandbit" bit="2" size="1" desc="Command bit"/>
+      <field name="size" bit="4" size="8" desc="Size of memory"/>
+      <field name="topofdpr" bit="20" size="12" desc="Top address +1 of DPR"/>
+    </register>
+    <!-- GENPROTRANGE Registers -->
+    <register name="GENPROTRANGE1_BASE" type="pcicfg" device="VTD_MEM_SM" offset="0xB0" size="8" desc="Generic Protected Memory Range 1 Base Address">
+      <field name="base_address" bit="16" size="35" desc="GENPROTRANGE 1 base address"/>
+    </register>
+    <register name="GENPROTRANGE1_LIMIT" type="pcicfg" device="VTD_MEM_SM" offset="0xB8" size="8" desc="Generic Protected Memory Range 1 Limit Address">
+      <field name="limit_address" bit="16" size="35" desc="GENPROTRANGE 1 limit address"/>
+    </register>
+    <register name="GENPROTRANGE2_BASE" type="pcicfg" device="VTD_MEM_SM" offset="0xC0" size="8" desc="Generic Protected Memory Range 2 Base Address">
+      <field name="base_address" bit="16" size="35" desc="GENPROTRANGE 2 base address"/>
+    </register>
+    <register name="GENPROTRANGE2_LIMIT" type="pcicfg" device="VTD_MEM_SM" offset="0xC8" size="8" desc="Generic Protected Memory Range 2 Limit Address">
+      <field name="limit_address" bit="16" size="35" desc="GENPROTRANGE 2 limit address"/>
+    </register>
+    <register name="GENPROTRANGE0_BASE" type="mmcfg" device="VTD_MEM_SM" offset="0x120" size="8" desc="Generic Protected Memory Range 0 Base Address">
+      <field name="base_address" bit="16" size="35" desc="GENPROTRANGE 0 base address"/>
+    </register>
+    <register name="GENPROTRANGE0_LIMIT" type="mmcfg" device="VTD_MEM_SM" offset="0x128" size="8" desc="Generic Protected Memory Range 0 Limit Address">
+      <field name="limit_address" bit="16" size="35" desc="GENPROTRANGE 0 limit address"/>
+    </register>
+    <!-- Integrated Memory Controller 0 -->
+    <register name="IMC0_SMBSTAT_0" type="mmcfg" device="IMC0_MAIN_SMBUS" offset="0x180" size="4" desc="SMBus Host Status">
+      <field name="RDATA" bit="0" size="16" desc="Read Data"/>
+      <field name="TSOD_SA" bit="24" size="4" desc="Last Issued TSOD Slave Address"/>
+      <field name="BUSY" bit="28" size="1" desc="SMBus Busy"/>
+      <field name="SBE" bit="29" size="1" desc="SMBus Error/Failed"/>
+      <field name="WOD" bit="30" size="1" desc="Write Operation Done"/>
+      <field name="RDO" bit="31" size="1" desc="Read Data Valid"/>
+    </register>
+    <register name="IMC0_SMBCMD_0" type="mmcfg" device="IMC0_MAIN_SMBUS" offset="0x184" size="4" desc="SMBus Host Command">
+      <field name="WDATA" bit="0" size="16" desc="Write Data"/>
+      <field name="BA" bit="16" size="8" desc="Bus Transaction Address"/>
+      <field name="SA" bit="24" size="3" desc="Slave Address"/>
+      <field name="WRT_CMD" bit="27" size="1" desc="Read/Write Command"/>
+      <field name="WRT_PNTR" bit="28" size="1" desc="Write Pointer"/>
+      <field name="WORD_ACCESS" bit="29" size="1" desc="Word Access"/>
+      <field name="PNTR_SEL" bit="30" size="1" desc="Pointer Select"/>
+      <field name="CMD_TRIGGER" bit="31" size="1" desc="Start/Trigger"/>
+    </register>
+    <register name="IMC0_SMBCNTL_0" type="mmcfg" device="IMC0_MAIN_SMBUS" offset="0x188" size="4" desc="SMBus Host Control">
+      <field name="DTI" bit="28" size="4" desc="Device Type Identifier"/>
+    </register>
+    <register name="IMC0_SMBSTAT_1" type="mmcfg" device="IMC0_MAIN_SMBUS" offset="0x190" size="4" desc="SMBus Host Status 1">
+      <field name="RDATA" bit="0" size="16" desc="Read Data"/>
+      <field name="TSOD_SA" bit="24" size="4" desc="Last Issued TSOD Slave Address"/>
+      <field name="BUSY" bit="28" size="1" desc="SMBus Busy"/>
+      <field name="SBE" bit="29" size="1" desc="SMBus Error/Failed"/>
+      <field name="WOD" bit="30" size="1" desc="Write Operation Done"/>
+      <field name="RDO" bit="31" size="1" desc="Read Data Valid"/>
+    </register>
+    <register name="IMC0_SMBCMD_1" type="mmcfg" device="IMC0_MAIN_SMBUS" offset="0x194" size="4" desc="SMBus Host Command 1">
+      <field name="WDATA" bit="0" size="16" desc="Write Data"/>
+      <field name="BA" bit="16" size="8" desc="Bus Transaction Address"/>
+      <field name="SA" bit="24" size="3" desc="Slave Address"/>
+      <field name="WRT_CMD" bit="27" size="1" desc="Read/Write Command"/>
+      <field name="WRT_PNTR" bit="28" size="1" desc="Write Pointer"/>
+      <field name="WORD_ACCESS" bit="29" size="1" desc="Word Access"/>
+      <field name="PNTR_SEL" bit="30" size="1" desc="Pointer Select"/>
+      <field name="CMD_TRIGGER" bit="31" size="1" desc="Start/Trigger"/>
+    </register>
+    <register name="IMC0_SMBCNTL_1" type="mmcfg" device="IMC0_MAIN_SMBUS" offset="0x198" size="4" desc="SMBus Host Control 1">
+      <field name="DTI" bit="28" size="4" desc="Device Type Identifier"/>
+    </register>
+    <!-- Integrated Memory Controller 1 -->
+    <register name="IMC1_SMBSTAT_0" type="mmcfg" device="IMC1_MAIN_SMBUS" offset="0x180" size="4" desc="SMBus Host Status">
+      <field name="RDATA" bit="0" size="16" desc="Read Data"/>
+      <field name="TSOD_SA" bit="24" size="4" desc="Last Issued TSOD Slave Address"/>
+      <field name="BUSY" bit="28" size="1" desc="SMBus Busy"/>
+      <field name="SBE" bit="29" size="1" desc="SMBus Error/Failed"/>
+      <field name="WOD" bit="30" size="1" desc="Write Operation Done"/>
+      <field name="RDO" bit="31" size="1" desc="Read Data Valid"/>
+    </register>
+    <register name="IMC1_SMBCMD_0" type="mmcfg" device="IMC1_MAIN_SMBUS" offset="0x184" size="4" desc="SMBus Host Command">
+      <field name="WDATA" bit="0" size="16" desc="Write Data"/>
+      <field name="BA" bit="16" size="8" desc="Bus Transaction Address"/>
+      <field name="SA" bit="24" size="3" desc="Slave Address"/>
+      <field name="WRT_CMD" bit="27" size="1" desc="Read/Write Command"/>
+      <field name="WRT_PNTR" bit="28" size="1" desc="Write Pointer"/>
+      <field name="WORD_ACCESS" bit="29" size="1" desc="Word Access"/>
+      <field name="PNTR_SEL" bit="30" size="1" desc="Pointer Select"/>
+      <field name="CMD_TRIGGER" bit="31" size="1" desc="Start/Trigger"/>
+    </register>
+    <register name="IMC1_SMBCNTL_0" type="mmcfg" device="IMC1_MAIN_SMBUS" offset="0x188" size="4" desc="SMBus Host Control">
+      <field name="DTI" bit="28" size="4" desc="Device Type Identifier"/>
+    </register>
+    <register name="IMC1_SMBSTAT_1" type="mmcfg" device="IMC1_MAIN_SMBUS" offset="0x190" size="4" desc="SMBus Host Status 1">
+      <field name="RDATA" bit="0" size="16" desc="Read Data"/>
+      <field name="TSOD_SA" bit="24" size="4" desc="Last Issued TSOD Slave Address"/>
+      <field name="BUSY" bit="28" size="1" desc="SMBus Busy"/>
+      <field name="SBE" bit="29" size="1" desc="SMBus Error/Failed"/>
+      <field name="WOD" bit="30" size="1" desc="Write Operation Done"/>
+      <field name="RDO" bit="31" size="1" desc="Read Data Valid"/>
+    </register>
+    <register name="IMC1_SMBCMD_1" type="mmcfg" device="IMC1_MAIN_SMBUS" offset="0x194" size="4" desc="SMBus Host Command 1">
+      <field name="WDATA" bit="0" size="16" desc="Write Data"/>
+      <field name="BA" bit="16" size="8" desc="Bus Transaction Address"/>
+      <field name="SA" bit="24" size="3" desc="Slave Address"/>
+      <field name="WRT_CMD" bit="27" size="1" desc="Read/Write Command"/>
+      <field name="WRT_PNTR" bit="28" size="1" desc="Write Pointer"/>
+      <field name="WORD_ACCESS" bit="29" size="1" desc="Word Access"/>
+      <field name="PNTR_SEL" bit="30" size="1" desc="Pointer Select"/>
+      <field name="CMD_TRIGGER" bit="31" size="1" desc="Start/Trigger"/>
     </register>
-    <register name="VTBAR" type="mmcfg" bus="0" dev="5" fun="0" offset="0x180" size="4" desc="VT BAR Register">
-      <field name="Base" bit="13" size="19" desc="Intel VT-d Base Address"/>
-      <field name="Enable" bit="0" size="1" desc="VTBAR enable"/>
+    <register name="IMC1_SMBCNTL_1" type="mmcfg" device="IMC1_MAIN_SMBUS" offset="0x198" size="4" desc="SMBus Host Control 1">
+      <field name="DTI" bit="28" size="4" desc="Device Type Identifier"/>
     </register>
     <!-- PCH ABASE (PMBASE) I/O registers -->
-    <register name="ABASE" type="pcicfg" device="PMC" offset="0x40" size="4" desc="ACPI Base Address">
-      <field name="Base" bit="8" size="24" desc="Base Address"/>
-    </register>
-    <register name="GEN_PMCON_1" type="pcicfg" device="PMC" offset="0xA0" size="2" desc="General PM Configuration 1">
-      <field name="SMI_LOCK" bit="4" size="1" desc="SMI Lock"/>
-    </register>
-    <register name="GEN_PMCON_B" type="pcicfg" device="PMC" offset="0xA4" size="4" desc="General Power Management Configuration Lock">
-      <field name="ACPI_BASE_LOCK" bit="17" size="1" desc="Lock down ACPI Base Address (ABASE)"/>
-    </register>
-    <!-- SPI Flash Controller MMIO registers -->
-    <register name="HSFS" type="mmio" bar="SPIBAR" offset="0x04" size="4" desc="Hardware Sequencing Flash Status Register">
-      <field name="FDONE" bit="0" size="1" desc="Flash Cycle Done"/>
-      <field name="FCERR" bit="1" size="1" desc="Flash Cycle Error"/>
-      <field name="AEL" bit="2" size="1" desc="Access Error Log"/>
-      <field name="SAF_ERROR" bit="3" size="1" desc="SAF Error"/>
-      <field name="SAF_DLE" bit="4" size="1" desc="SAF Data Length Error"/>
-      <field name="SCIP" bit="5" size="1" desc="SPI cycle in progress"/>
-      <field name="WRSDIS" bit="11" size="1" desc="Write status disable"/>
-      <field name="PR34LKD" bit="12" size="1" desc="PRR3 PRR4 Lock-Down"/>
-      <field name="FDOPSS" bit="13" size="1" desc="Flash Descriptor Override Pin-Strap Status"/>
-      <field name="FDV" bit="14" size="1" desc="Flash Descriptor Valid"/>
-      <field name="FLOCKDN" bit="15" size="1" desc="Flash Configuration Lock-Down"/>
-      <field name="FGO" bit="16" size="1" desc="Flash cycle go"/>
-      <field name="FCYCLE" bit="17" size="4" desc="Flash Cycle Type"/>
-      <field name="WET" bit="21" size="1" desc="Write Enable Type"/>
-      <field name="FDBC" bit="24" size="6" desc="Flash Data Byte Count"/>
-      <field name="FSMIE" bit="31" size="1" desc="Flash SPI SMI Enable"/>
-    </register>
-    <!-- SMBus Host Controller -->
-    <register name="SMBUS_VID" type="pcicfg" device="SMBUS" offset="0x00" size="2" desc="VID"/>
-    <register name="SMBUS_DID" type="pcicfg" device="SMBUS" offset="0x02" size="2" desc="DID"/>
-    <register name="SMBUS_CMD" type="pcicfg" device="SMBUS" offset="0x04" size="2" desc="CMD"/>
-    <register name="SMBUS_HCFG" type="pcicfg" device="SMBUS" offset="0x40" size="1" desc="Host Configuration">
-      <field name="HST_EN" bit="0" size="1"/>
-      <field name="SMB_SMI_EN" bit="1" size="1"/>
-      <field name="I2C_EN" bit="2" size="2"/>
-      <field name="SSRESET" bit="3" size="1"/>
-      <field name="SPD_WD" bit="4" size="1"/>
-    </register>
-    <register name="TCOBASE" type="pcicfg" device="SMBUS" offset="0x50" size="4" desc="TCO Base Address">
-      <field name="IOS" bit="0" size="1" desc="I/O space"/>
-      <field name="TCOBA" bit="5" size="11" desc="TCO Base Address"/>
-    </register>
-    <register name="TCOCTL" type="pcicfg" device="SMBUS" offset="0x54" size="4" desc="TCO Control">
-      <field name="TCO_BASE_LOCK" bit="0" size="1" desc="TCO Base Lock"/>
-      <field name="TCO_BASE_EN" bit="8" size="1" desc="TCO Base Enable"/>
-    </register>
     <register name="SMI_EN" type="iobar" bar="ABASE" offset="0x30" size="4" desc="SMI Control and Enable">
-      <field name="GBL_SMI_EN" bit="0" size="1" desc="Global SMI Enable"/>
-      <field name="TCO_EN" bit="13" size="1" desc="TCO Enable"/>
-      <field name="GPIO_UNLOCK_SMI_EN" bit="27" size="1" desc="GPIO Unlock SMI Enable"/>
-    </register>
-    <register name="TCO1_CNT" type="iobar" bar="TCOBAR" offset="0x8" size="2" desc="TCO1 Control">
-      <field name="TCO_LOCK" bit="12" size="1" desc="TCO Lock"/>
-    </register>
-    <!-- SPI Interface Controller -->
-    <register name="BC" type="pcicfg" device="SPI" offset="0xDC" size="4" desc="BIOS Control">
-      <field name="BIOSWE" bit="0" size="1" desc="BIOS Write Enable"/>
-      <!-- WPD -->
-      <field name="BLE" bit="1" size="1" desc="BIOS Lock Enable"/>
-      <!-- LE -->
-      <field name="TSS" bit="4" size="1" desc="Top Swap Status"/>
-      <!-- TSS -->
-      <field name="SMM_BWP" bit="5" size="1" desc="SMM BIOS Write Protection"/>
-      <!-- EISS -->
-      <field name="BILD" bit="7" size="1" desc="BIOS Interface Lock Down"/>
-      <!-- BILD -->
-    </register>
-    <!-- DCI registers -->
-    <register name="ECTRL" type="mm_msgbus" port="0xB8" offset="0x0004" size="4" desc="DCI Control Register">
-      <field name="ENABLE" bit="4" size="1"/>
+      <field name="GBL_SMI_EN" bit="0" size="1"/>
+      <field name="EOS" bit="1" size="1"/>
+      <field name="BIOS_EN" bit="2" size="1"/>
+      <field name="LEGACY_USB_EN" bit="3" size="1"/>
+      <field name="SLP_SMI_EN" bit="4" size="1"/>
+      <field name="APMC_EN" bit="5" size="1"/>
+      <field name="SWSMI_TMR_EN" bit="6" size="1"/>
+      <field name="BIOS_RLS" bit="7" size="1"/>
+      <field name="MCSMI_EN" bit="11" size="1"/>
+      <field name="TCO_EN" bit="13" size="1"/>
+      <field name="PERIODIC_EN" bit="14" size="1"/>
+      <field name="LEGACY_USB2_EN" bit="17" size="1"/>
+      <field name="INTEL_USB2_EN" bit="18" size="1"/>
+      <field name="GPIO_UNLOCK_SMI_EN" bit="27" size="1"/>
+      <field name="ME_SMI_EN" bit="30" size="1"/>
+      <field name="xHCI_SMI_EN" bit="31" size="1"/>
     </register>
+    <!-- CPU Model Specific Registers -->
   </registers>
-  <controls>
-    <control name="BiosInterfaceLockDown" register="BC" field="BILD" desc="BIOS Interface Lock-Down"/>
-    <control name="SpiWriteStatusDis" register="HSFS" field="WRSDIS" desc="Write Status Disable"/>
-    <control name="TcoCtlLock" register="TCOCTL" field="TCO_BASE_LOCK" desc="TCO Base Lock"/>
-  </controls>
 </configuration>
```

### Comparing `chipsec-1.4.4/chipsec/cfg/apl.xml` & `chipsec-1.5.1/chipsec/cfg/8086/apl.xml`

 * *Files 13% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/apl.xml` & `chipsec-1.5.1/chipsec/cfg/8086/apl.xml`

```diff
@@ -1,47 +1,76 @@
 <?xml version="1.0" encoding="utf-8"?>
 <configuration platform="APL">
   <!--
 XML configuration for Apollo Lake based SoCs
 -->
   <!-- #################################### -->
   <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info family="atom">
+    <sku did="0x5AF0" name="Apollo Lake" code="APL" longname="Apollo Lake"/>
+  </info>
+  <!-- #################################### -->
+  <!--                                      -->
   <!-- Memory Mapped I/O spaces (MMIO BARs) -->
   <!--                                      -->
   <!-- #################################### -->
   <mmio>
-    <bar name="SPIBAR" bus="0" dev="0x0D" fun="2" reg="0x10" width="4" mask="0xFFFFFE00" size="0x200" enable_bit="1" desc="SPI Controller Register Range"/>
+    <bar name="SPIBAR" bus="0" dev="0x0D" fun="2" reg="0x10" width="4" mask="0xFFFFF000" size="0x200" enable_bit="1" desc="SPI Controller Register Range"/>
     <bar name="GTTMMADR" bus="0" dev="0x02" fun="0" reg="0x10" width="8" mask="0x7FF000000" desc="Graphics Translation Table Range"/>
+    <bar name="PWRMBASE" register="PWRMBASE" base_field="BA" size="0x1000" desc="Power Management Register Range"/>
+    <bar name="SBREGBAR" register="SBREG_BAR" base_field="RBA" size="0x1000000" fixed_address="0xFD000000" desc="Sideband Register Access BAR"/>
   </mmio>
   <!-- #################################### -->
   <!--                                      -->
+  <!-- I/O spaces (I/O BARs)                -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <io>
+    <bar name="ABASE" register="ABASE" base_field="BA" size="0x100" fixed_address="0x400" desc="ACPI Base Address"/>
+    <bar name="PMBASE" register="ABASE" base_field="BA" size="0x100" fixed_address="0x400" desc="ACPI Base Address"/>
+  </io>
+  <!-- #################################### -->
+  <!--                                      -->
   <!-- Configuration registers              -->
   <!--                                      -->
   <!-- #################################### -->
   <registers>
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- PCIe Configuration registers -->
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
-    <!-- GFx PCI device registers -->
-    <register name="PCI0.0.0_GGC" type="pcicfg" bus="0" dev="0x2" fun="0" offset="0x50" size="4" desc="GMCH Graphics Control">
-      <field name="GGCLOCK" bit="0" size="1"/>
-    </register>
-    <register name="PCI0.0.0_BDSM" type="pcicfg" bus="0" dev="0x2" fun="0" offset="0x5C" size="4" desc="Base of Data Stolen Memory">
-      <field name="LOCK" bit="0" size="1"/>
+    <!-- Sideband Register Access Registers -->
+    <register name="SBREG_BAR" type="pcicfg" bus="0" dev="0xD" fun="0" offset="0x10" size="4" desc="Sideband Register Access BAR">
+      <field name="RBA" bit="24" size="8" desc="Register Base Address"/>
     </register>
-    <register name="PCI0.0.0_BGSM" type="pcicfg" bus="0" dev="0x2" fun="0" offset="0x70" size="4" desc="Base of Graphics Stolen Memory">
-      <field name="LOCK" bit="0" size="1"/>
+    <register name="P2SBC" type="pcicfg" bus="0" dev="0xD" fun="0" offset="0xE0" size="4" desc="P2SB Configuration Register">
+      <field name="HIDE" bit="8" size="1" desc="Hide SBREG_BAR"/>
     </register>
-    <register name="PCI0.0.0_PAVPC" type="pcicfg" bus="0" dev="0x2" fun="0" offset="0x74" size="4" desc="PAVP Control">
-      <field name="PAVPLCK" bit="2" size="1"/>
+    <register name="P2SB_HIDE" type="pcicfg" bus="0" dev="0xD" fun="0" offset="0xE1" size="1" desc="P2SB Configuration Register hide-unhide">
+      <field name="HIDE" bit="0" size="1" desc="Hide SBREG_BAR"/>
     </register>
     <!-- Misc PCI registers -->
     <register name="IADBGCTRL" type="pcicfg" bus="0" dev="0x1A" fun="0" offset="0xB0" desc="Debug Control">
       <field name="IADBGCTRL_LOCK" bit="30" size="1"/>
     </register>
+    <register name="PWRMBASE" type="pcicfg" bus="0" dev="0x0D" fun="1" offset="0x10" size="8" desc="PM Base Address">
+      <field name="STYPE" bit="1" size="2" desc="Space Type (if 0 - 32bit, 10 - 64bit)"/>
+      <field name="BA" bit="12" size="52" desc="Base Address"/>
+    </register>
+    <register name="ABASE" type="pcicfg" bus="0" dev="0x0D" fun="1" offset="0x20" size="4" desc="ACPI Base Address">
+      <field name="BA" bit="2" size="30" desc="Base Address"/>
+    </register>
+    <register name="TCOBASE" type="pcicfg" bus="0" dev="0x1f" fun="1" offset="0x50" size="4" desc="TCO Base Address">
+      <field name="TCOBA" bit="5" size="11" desc="TCO Base Address"/>
+    </register>
+    <register name="TCOCTL" type="pcicfg" bus="0" dev="0x1f" fun="1" offset="0x54" size="4" desc="TCO Control">
+      <field name="TCO_BASE_EN" bit="8" size="1" desc="TCO Base Enable"/>
+    </register>
     <!-- SPI Controller Registers -->
     <register name="BC" type="pcicfg" bus="0" dev="0x0D" fun="2" offset="0xDC" size="4" desc="BIOS Control Register (BCR)">
       <field name="BIOSWE" bit="0" size="1" desc="BIOS Write Enable"/>
       <field name="BLE" bit="1" size="1" desc="BIOS Lock Enable"/>
       <field name="SRC" bit="2" size="2" desc="SPI Read Configuration"/>
       <field name="TSS" bit="4" size="1" desc="Top Swap Status"/>
       <field name="SMM_BWP" bit="5" size="1" desc="SMM BIOS Write Protect"/>
@@ -163,14 +192,49 @@
       <field name="PRL" bit="16" size="15"/>
       <field name="WPE" bit="31" size="1"/>
     </register>
     <!-- GFx MMIO registers -->
     <register name="PCBR" type="mmio" bar="GTTMMADR" offset="0x182120" desc="PCBR">
       <field name="PCBR_LOCK" bit="0" size="1"/>
     </register>
+    <!-- Power Management Registers -->
+    <register name="GEN_PMCON_1" type="mmio" bar="PWRMBASE" offset="0x1020" size="4" desc="General PM Configuration 1"/>
+    <register name="GEN_PMCON_2" type="mmio" bar="PWRMBASE" offset="0x1024" size="4" desc="General PM Configuration 2">
+      <field name="SMI_LOCK" bit="4" size="1"/>
+    </register>
+    <!-- PCH TCOBASE (SMBus TCO) I/O registers -->
+    <register name="TCO1_CNT" type="iobar" bar="ABASE" offset="0x68" size="4" desc="TCO1 Control">
+      <field name="TCO_LOCK" bit="12" size="1" desc="TCO Lock"/>
+    </register>
+    <!-- PCH ABASE (PMBASE) -->
+    <register name="SMI_EN" type="iobar" bar="ABASE" offset="0x40" size="4" desc="SMI Control and Enable">
+      <field name="GBL_SMI_EN" bit="0" size="1"/>
+      <field name="EOS" bit="1" size="1"/>
+      <field name="BIOS_EN" bit="2" size="1"/>
+      <field name="LEGACY_USB_EN" bit="3" size="1"/>
+      <field name="SLP_SMI_EN" bit="4" size="1"/>
+      <field name="APMC_EN" bit="5" size="1"/>
+      <field name="SWSMI_TMR_EN" bit="6" size="1"/>
+      <field name="BIOS_RLS" bit="7" size="1"/>
+      <field name="GPIO_UNLOCK_SMI_EN" bit="10" size="1"/>
+      <field name="GPIO_UNLOCK_SSMI_EN" bit="11" size="1"/>
+      <field name="MCSMI_EN" bit="12" size="1"/>
+      <field name="TCO_EN" bit="13" size="1"/>
+      <field name="PERIODIC_EN" bit="14" size="1"/>
+      <field name="SERIRQ_SMI_EN" bit="15" size="1"/>
+      <field name="SMBUS_SMI_EN" bit="16" size="1"/>
+      <field name="xHCI_SMI_EN" bit="17" size="1"/>
+      <field name="HOST_SMBUS_SMI_EN" bit="18" size="1"/>
+      <field name="SCS_SMI_EN" bit="19" size="1"/>
+      <field name="PCIE_SMI_EN" bit="20" size="1"/>
+      <field name="SCC2_SMI_EN" bit="21" size="1"/>
+      <field name="SPI_SSMI_EN" bit="25" size="1"/>
+      <field name="SPI_SMI_EN" bit="26" size="1"/>
+      <field name="OCP_SMI_EN" bit="27" size="1"/>
+    </register>
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- CPU MSRs                     -->
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <register name="MSR_POWER_MISC" type="msr" msr="0x120" desc="MISC"/>
   </registers>
   <!-- #################################### -->
   <!--                                      -->
@@ -178,9 +242,10 @@
   <!--                                      -->
   <!-- #################################### -->
   <controls>
     <control name="BiosInterfaceLockDown" register="BC" field="BILD" desc="BIOS Interface Lock-Down"/>
     <control name="SpiWriteStatusDis" register="HSFS" field="WRSDIS" desc="Write Status Disable"/>
     <control name="TopSwapStatus" register="BC" field="TSS" desc="Top Swap Status"/>
     <control name="TopSwap" register="BC" field="TSS" desc="Top Swap Status"/>
+    <control name="SMILock" register="GEN_PMCON_2" field="SMI_LOCK" desc="SMI Global Configuration Lock"/>
   </controls>
 </configuration>
```

### Comparing `chipsec-1.4.4/chipsec/cfg/hsw.xml` & `chipsec-1.5.1/chipsec/cfg/8086/bdw.xml`

 * *Files 23% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/hsw.xml` & `chipsec-1.5.1/chipsec/cfg/8086/bdw.xml`

```diff
@@ -1,14 +1,26 @@
 <?xml version="1.0" encoding="utf-8"?>
-<configuration platform="HSW">
+<configuration platform="BDW">
   <!--
-XML configuration file for Haswell based platforms
+XML configuration for Broadwell based platforms
 -->
   <!-- #################################### -->
   <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info family="core">
+    <sku did="0x1600" name="Broadwell" code="BDW" longname="Desktop 5th Generation Core Processor (Broadwell CPU / Wildcat Point PCH)"/>
+    <sku did="0x1604" name="Broadwell" code="BDW" longname="Mobile 5th Generation Core Processor (Broadwell M/H / Wildcat Point PCH)"/>
+    <sku did="0x1610" name="Broadwell" code="BDW" longname="Desktop 5th Generation Core Processor (Broadwell H / Wildcat Point PCH)"/>
+    <sku did="0x1614" name="Broadwell" code="BDW" longname="Mobile 5th Generation Core Processor (Broadwell H / Wildcat Point PCH)"/>
+    <sku did="0x1618" name="Broadwell Server" code="BDW" longname="Intel Xeon Processor E3 v4 (Broadwell CPU)"/>
+  </info>
+  <!-- #################################### -->
+  <!--                                      -->
   <!-- Integrated devices                   -->
   <!--                                      -->
   <!-- #################################### -->
   <pci/>
   <!-- #################################### -->
   <!--                                      -->
   <!-- Memory Mapped I/O spaces (MMIO BARs) -->
```

### Comparing `chipsec-1.4.4/chipsec/cfg/common.xml` & `chipsec-1.5.1/chipsec/cfg/8086/common.xml`

 * *Files 1% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/common.xml` & `chipsec-1.5.1/chipsec/cfg/8086/common.xml`

```diff
@@ -42,15 +42,15 @@
   <!--                                      -->
   <!-- Memory Mapped I/O spaces (MMIO BARs) -->
   <!--                                      -->
   <!-- #################################### -->
   <mmio>
     <bar name="PXPEPBAR" bus="0" dev="0" fun="0" reg="0x40" width="8" mask="0x7FFFFFF000" size="0x1000" enable_bit="0" desc="PCI Express Egress Port Register Range"/>
     <bar name="MCHBAR" bus="0" dev="0" fun="0" reg="0x48" width="8" mask="0x7FFFFF8000" size="0x8000" enable_bit="0" desc="Host Memory Mapped Register Range"/>
-    <bar name="MMCFG" bus="0" dev="0" fun="0" reg="0x60" width="8" mask="0x7FFFFFF000" size="0x1000" enable_bit="0" desc="PCI Express Register Range"/>
+    <bar name="MMCFG" bus="0" dev="0" fun="0" reg="0x60" width="8" mask="0x7FFC000000" size="0x1000" enable_bit="0" desc="PCI Express Register Range"/>
     <bar name="DMIBAR" bus="0" dev="0" fun="0" reg="0x68" width="8" mask="0x7FFFFFF000" size="0x1000" enable_bit="0" desc="Root Complex Register Range"/>
     <bar name="GTTMMADR" bus="0" dev="2" fun="0" reg="0x10" width="8" mask="0x7FFFC00000" desc="Graphics Translation Table Range"/>
     <bar name="GMADR" bus="0" dev="2" fun="0" reg="0x18" width="8" mask="0x7FF8000000" desc="Graphics Memory Range"/>
     <bar name="HDABAR" bus="0" dev="3" fun="0" reg="0x10" width="8" mask="0x7FFFFFF000" size="0x1000" desc="HD Audio Controller Register Range"/>
     <bar name="HDBAR" bus="0" dev="0x1B" fun="0" reg="0x10" width="8" mask="0x7FFFFFC000" size="0x1000" desc="PCH HD Audio Controller Register Range"/>
     <bar name="RCBA" bus="0" dev="0x1F" fun="0" reg="0xF0" width="4" mask="0xFFFFC000" size="0x4000" enable_bit="0" desc="PCH Root Complex Register Range"/>
     <bar name="SPIBAR" bus="0" dev="0x1F" fun="0" reg="0xF0" width="4" mask="0xFFFFC000" size="0x200" enable_bit="0" desc="SPI Controller Register Range" offset="0x3800"/>
@@ -358,14 +358,16 @@
     <register name="UVSCC" type="mmio" bar="SPIBAR" offset="0xC8" size="4" desc="Host Upper Vendor Specific Component Capabilities">
       <field name="UBES" bit="0" size="2" desc="Upper Block/Sector Erase Size"/>
       <field name="UWG" bit="2" size="1" desc="Upper Write Granularity"/>
       <field name="UWSR" bit="3" size="1" desc="Upper Write Status Required"/>
       <field name="UWEWS" bit="4" size="1" desc="Write Enable on Write Status"/>
       <field name="UEO" bit="8" size="8" desc="Upper Erase Opcode"/>
     </register>
+    <register name="BIOS_PTINX" type="mmio" bar="SPIBAR" offset="0xCC" size="4" desc="Parameter Table Index"/>
+    <register name="BIOS_PTDATA" type="mmio" bar="SPIBAR" offset="0xD0" size="4" desc="Parameter Table Data"/>
     <!-- SPI Flash Descriptor registers -->
     <register name="FLMAP0" type="mmio" bar="FDBAR" offset="0x14" size="4" desc="Flash Map 0 Register">
       <field name="FCBA" bit="0" size="8" desc="Flash Component Base Address"/>
       <field name="NC" bit="8" size="2" desc="Number of Components"/>
       <field name="FRBA" bit="16" size="8" desc="Flash Region Base Address"/>
       <field name="NR" bit="24" size="3" desc="Number of Regions"/>
     </register>
@@ -511,14 +513,18 @@
     <register name="SMBUS_HST_D0" type="iobar" bar="SMBUS_BASE" offset="0x05" size="1" desc="SMBus Host Data 0">
       <field name="Data" bit="0" size="8" desc="Data0/Count"/>
     </register>
     <register name="SMBUS_HST_D1" type="iobar" bar="SMBUS_BASE" offset="0x06" size="1" desc="SMBus Host Data 1">
       <field name="Data" bit="0" size="8" desc="Data1"/>
     </register>
     <!-- CPU Model Specific Registers (MSR) -->
+    <register name="IA32_MSR_CORE_THREAD_COUNT" type="msr" msr="0x35" desc="Core Thread Count">
+      <field name="Thread_Count" bit="0" size="16" desc="Number of Logical Processors currently enabled"/>
+      <field name="Core_Count" bit="16" size="16" desc="Number of Processor Cores currently enabled"/>
+    </register>
     <register name="IA32_BIOS_SIGN_ID" type="msr" msr="0x8B" desc="Microcode Update Signature Register">
       <field name="Microcode" bit="32" size="32" desc="Microcode update signature"/>
     </register>
     <register name="IA32_SMRR_PHYSBASE" type="msr" msr="0x1F2" desc="SMRR Base Address MSR">
       <field name="Type" bit="0" size="8" desc="SMRR memory type"/>
       <field name="PhysBase" bit="12" size="20" desc="SMRR physical base address"/>
     </register>
```

### Comparing `chipsec-1.4.4/chipsec/cfg/kbl.xml` & `chipsec-1.5.1/chipsec/cfg/8086/pch_2xx.xml`

 * *Files 2% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/kbl.xml` & `chipsec-1.5.1/chipsec/cfg/8086/pch_2xx.xml`

```diff
@@ -1,60 +1,64 @@
 <?xml version="1.0" encoding="utf-8"?>
-<configuration platform="KBL">
+<configuration platform="PCH_2xx">
   <!--
-XML configuration file for Kaby Lake based platforms
+XML configuration file for 200 series PCH based platforms
 
-http://www.intel.com/content/www/us/en/processors/core/core-technical-resources.html
-
-* 7th Generation Intel(R) Processor Families for U/Y-Platforms
-
-* 7th Generation Intel(R) Processor Families I/O for U/Y-Platforms
+* Intel(R) 200 Series Chipset Family Platform Controller Hub (PCH)
+  http://www.intel.com/content/www/us/en/processors/core/core-technical-resources.html
 -->
   <!-- #################################### -->
   <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info>
+    <sku did="0xA2C4" name="H270" code="PCH_2xx" longname="Intel H270 (200 series) PCH"/>
+    <sku did="0xA2C5" name="Z270" code="PCH_2xx" longname="Intel Z270 (200 series) PCH"/>
+    <sku did="0xA2C6" name="Q270" code="PCH_2xx" longname="Intel Q270 (200 series) PCH"/>
+    <sku did="0xA2C7" name="Q250" code="PCH_2xx" longname="Intel Q250 (200 series) PCH"/>
+    <sku did="0xA2C8" name="B250" code="PCH_2xx" longname="Intel B250 (200 series) PCH"/>
+    <sku did="0xA2C9" name="Z370" code="PCH_2xx" longname="Intel Z370 (200 series) PCH"/>
+    <sku did="0xA2D2" name="X299" code="PCH_2xx" longname="Intel X299 (200 series) PCH"/>
+  </info>
+  <!-- #################################### -->
+  <!--                                      -->
   <!-- Integrated devices                   -->
   <!--                                      -->
   <!-- #################################### -->
   <pci>
     <device name="P2SBC" bus="0" dev="0x1F" fun="1" vid="0x8086"/>
     <device name="SMBUS" bus="0" dev="0x1F" fun="4" vid="0x8086"/>
     <device name="SPI" bus="0" dev="0x1F" fun="5" vid="0x8086"/>
   </pci>
   <!-- #################################### -->
   <!--                                      -->
   <!-- Memory Mapped I/O spaces (MMIO BARs) -->
   <!--                                      -->
   <!-- #################################### -->
   <mmio>
-    <bar name="GTTMMADR" bus="0" dev="2" fun="0" reg="0x10" width="8" mask="0x7FFF000000" desc="Graphics Translation Table Range"/>
     <bar name="HDABAR" bus="0" dev="0x1F" fun="3" reg="0x10" width="8" mask="0xFFFFFFFFFFFFC000" size="0x1000" desc="HD Audio Base"/>
     <bar name="SPIBAR" bus="0" dev="0x1F" fun="5" reg="0x10" width="4" mask="0xFFFFF000" size="0x1000" desc="SPI Controller Register Range" offset="0x0"/>
     <bar name="PWRMBASE" register="PWRMBASE" base_field="BA" size="0x1000" fixed_address="0xFE000000" desc="Power Management Register Range"/>
     <bar name="SBREGBAR" register="SBREG_BAR" base_field="RBA" size="0x1000000" fixed_address="0xFD000000" desc="Sideband Register Access BAR"/>
   </mmio>
   <!-- #################################### -->
   <!--                                      -->
   <!-- I/O spaces (I/O BARs)                -->
   <!--                                      -->
   <!-- #################################### -->
   <io>
-    <bar name="ABASE" register="ABASE" base_field="BA" size="0x100" desc="ACPI Base Address"/>
-    <bar name="PMBASE" register="ABASE" base_field="BA" size="0x100" desc="ACPI Base Address"/>
+    <bar name="ABASE" register="ABASE" base_field="BA" size="0x100" fixed_address="0x1800" desc="ACPI Base Address"/>
+    <bar name="PMBASE" register="ABASE" base_field="BA" size="0x100" fixed_address="0x1800" desc="ACPI Base Address"/>
     <bar name="TCOBASE" register="TCOBASE" base_field="TCOBA" size="0x20" desc="TCO Base Address"/>
     <!-- old definition -->
     <bar name="SMBUS_BASE" bus="0" dev="0x1F" fun="4" reg="0x20" mask="0xFFE0" size="0x80" desc="SMBus Base Address"/>
   </io>
   <!-- #################################### -->
   <!--                                      -->
-  <!-- Memory ranges                        -->
-  <!--                                      -->
-  <!-- #################################### -->
-  <memory/>
-  <!-- #################################### -->
-  <!--                                      -->
   <!-- Configuration registers              -->
   <!--                                      -->
   <!-- #################################### -->
   <registers>
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- PCIe Configuration registers -->
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
@@ -130,14 +134,21 @@
       <field name="FLOCKDN" bit="15" size="1" desc="Flash Configuration Lock-Down"/>
       <field name="FGO" bit="16" size="1" desc="Flash cycle go"/>
       <field name="FCYCLE" bit="17" size="4" desc="Flash Cycle Type"/>
       <field name="WET" bit="21" size="1" desc="Write Enable Type"/>
       <field name="FDBC" bit="24" size="6" desc="Flash Data Byte Count"/>
       <field name="FSMIE" bit="31" size="1" desc="Flash SPI SMI# Enable"/>
     </register>
+    <register name="HSFC" type="mmio" bar="SPIBAR" offset="0x06" size="2" desc="Hardware Sequencing Flash Control Register">
+      <field name="FGO" bit="0" size="1" desc="Flash Cycle GO"/>
+      <field name="FCYCLE" bit="1" size="4" desc="Flash Cycle"/>
+      <field name="WET" bit="5" size="1" desc="Write Enable Type"/>
+      <field name="FDBC" bit="8" size="6" desc="Flash Data Byte Count, Count = FDBC + 1"/>
+      <field name="FSMIE" bit="15" size="1" desc="Flash SPI SMI Enable"/>
+    </register>
     <register name="FREG0_FLASHD" type="mmio" bar="SPIBAR" offset="0x54" size="4" desc="Flash Region 0 (Flash Descriptor)">
       <field name="RB" bit="0" size="15" desc="Region Base"/>
       <field name="RL" bit="16" size="15" desc="Region Limit"/>
     </register>
     <register name="FREG1_BIOS" type="mmio" bar="SPIBAR" offset="0x58" size="4" desc="Flash Region 1 (BIOS)">
       <field name="RB" bit="0" size="15" desc="Region Base"/>
       <field name="RL" bit="16" size="15" desc="Region Limit"/>
@@ -233,15 +244,15 @@
       <field name="LL" bit="3" size="1" desc="Lower 128 Byte Lock"/>
       <field name="UL" bit="4" size="1" desc="Upper 128 Byte Lock"/>
       <field name="BILD" bit="31" size="1" desc="BIOS Interface Lock-Down"/>
     </register>
     <register name="BUC" type="mm_msgbus" port="0xC3" offset="0x3414" size="4" desc="Backed Up Control">
       <field name="TS" bit="0" size="1" desc="Top Swap"/>
     </register>
-    <!-- PMC MMIO registers (7th Generation Intel(R) Processor Families I/O for U/Y-Platforms, Vol. 2, section 4.3) -->
+    <!-- PMC MMIO registers (7th/8th Generation Intel(R) Processor Families I/O for U/Y-Platforms, Vol. 2, section 4.3) -->
     <register name="PM_CFG" type="mmio" bar="PWRMBASE" offset="0x18" size="4" desc="Power Management Configuration Reg 1"/>
     <!-- SPI Flash Descriptor registers -->
     <register name="FLMAP0" type="mmio" bar="FDBAR" offset="0x14" size="4" desc="Flash Map 0 Register">
       <field name="FCBA" bit="0" size="8" desc="Flash Component Base Address"/>
       <field name="NC" bit="8" size="2" desc="Number of Components"/>
       <field name="FRBA" bit="16" size="8" desc="Flash Region Base Address"/>
     </register>
```

### Comparing `chipsec-1.4.4/chipsec/cfg/skl.xml` & `chipsec-1.5.1/chipsec/cfg/8086/kbl.xml`

 * *Files 1% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/skl.xml` & `chipsec-1.5.1/chipsec/cfg/8086/kbl.xml`

```diff
@@ -1,26 +1,35 @@
 <?xml version="1.0" encoding="utf-8"?>
-<configuration platform="SKL">
+<configuration platform="KBL">
   <!--
-XML configuration file for Skylake based platforms
+XML configuration file for Kaby Lake based platforms
 
 http://www.intel.com/content/www/us/en/processors/core/core-technical-resources.html
 
-* 6th Generation Intel(R) Processor Datasheet for U/Y-Platforms
+* 7th Generation Intel(R) Processor Families for U/Y-Platforms
 
-* 6th Generation Intel(R) Processor I/O Datasheet for U/Y-Platforms
-
-* 6th Generation Intel(R) Processor Datasheet for S-Platforms
-
-* 6th Generation Intel(R) Processor Datasheet for H-Platforms
-
-* Intel(R) 100 Series Chipset Family Platform Controller Hub (PCH)
+* 7th Generation Intel(R) Processor Families I/O for U/Y-Platforms
 -->
   <!-- #################################### -->
   <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info family="core">
+    <sku did="0x5900" name="Kabylake" code="KBL" longname="Mobile 7th Generation Core Processor (Kabylake H)"/>
+    <sku did="0x5904" name="Kabylake" code="KBL" longname="Mobile 7th Generation Core Processor (Kabylake U)"/>
+    <sku did="0x590C" name="Kabylake" code="KBL" longname="Mobile 7th Generation Core Processor (Kabylake Y)"/>
+    <sku did="0x590F" name="Kabylake" code="KBL" longname="Desktop 7th Generation Core Processor (Kabylake S)"/>
+    <sku did="0x5910" name="Kabylake" code="KBL" longname="Mobile 7th Generation Core Processor (Kabylake H)"/>
+    <sku did="0x5914" name="Kabylake" code="KBL" longname="Mobile 8th Generation Core Processor (Kabylake U-Quad Core)"/>
+    <sku did="0x591F" name="Kabylake" code="KBL" longname="Desktop 7th Generation Core Processor (Kabylake S)"/>
+    <sku did="0x5918" name="Kabylake" code="KBL" longname="Intel Xeon Processor E3 v6 (Kabylake CPU)"/>
+  </info>
+  <!-- #################################### -->
+  <!--                                      -->
   <!-- Integrated devices                   -->
   <!--                                      -->
   <!-- #################################### -->
   <pci>
     <device name="P2SBC" bus="0" dev="0x1F" fun="1" vid="0x8086"/>
     <device name="SMBUS" bus="0" dev="0x1F" fun="4" vid="0x8086"/>
     <device name="SPI" bus="0" dev="0x1F" fun="5" vid="0x8086"/>
@@ -134,15 +143,15 @@
       <field name="FDOPSS" bit="13" size="1" desc="Flash Descriptor Override Pin-Strap Status"/>
       <field name="FDV" bit="14" size="1" desc="Flash Descriptor Valid"/>
       <field name="FLOCKDN" bit="15" size="1" desc="Flash Configuration Lock-Down"/>
       <field name="FGO" bit="16" size="1" desc="Flash cycle go"/>
       <field name="FCYCLE" bit="17" size="4" desc="Flash Cycle Type"/>
       <field name="WET" bit="21" size="1" desc="Write Enable Type"/>
       <field name="FDBC" bit="24" size="6" desc="Flash Data Byte Count"/>
-      <field name="FSMIE" bit="31" size="1" desc="Flash SPI SMI Enable"/>
+      <field name="FSMIE" bit="31" size="1" desc="Flash SPI SMI# Enable"/>
     </register>
     <register name="FREG0_FLASHD" type="mmio" bar="SPIBAR" offset="0x54" size="4" desc="Flash Region 0 (Flash Descriptor)">
       <field name="RB" bit="0" size="15" desc="Region Base"/>
       <field name="RL" bit="16" size="15" desc="Region Limit"/>
     </register>
     <register name="FREG1_BIOS" type="mmio" bar="SPIBAR" offset="0x58" size="4" desc="Flash Region 1 (BIOS)">
       <field name="RB" bit="0" size="15" desc="Region Base"/>
@@ -239,15 +248,15 @@
       <field name="LL" bit="3" size="1" desc="Lower 128 Byte Lock"/>
       <field name="UL" bit="4" size="1" desc="Upper 128 Byte Lock"/>
       <field name="BILD" bit="31" size="1" desc="BIOS Interface Lock-Down"/>
     </register>
     <register name="BUC" type="mm_msgbus" port="0xC3" offset="0x3414" size="4" desc="Backed Up Control">
       <field name="TS" bit="0" size="1" desc="Top Swap"/>
     </register>
-    <!-- PMC MMIO registers (6th Generation Intel(R) Processor I/O Datasheet for U/Y-Platforms, Vol. 2, section 4.3) -->
+    <!-- PMC MMIO registers (7th Generation Intel(R) Processor Families I/O for U/Y-Platforms, Vol. 2, section 4.3) -->
     <register name="PM_CFG" type="mmio" bar="PWRMBASE" offset="0x18" size="4" desc="Power Management Configuration Reg 1"/>
     <!-- SPI Flash Descriptor registers -->
     <register name="FLMAP0" type="mmio" bar="FDBAR" offset="0x14" size="4" desc="Flash Map 0 Register">
       <field name="FCBA" bit="0" size="8" desc="Flash Component Base Address"/>
       <field name="NC" bit="8" size="2" desc="Number of Components"/>
       <field name="FRBA" bit="16" size="8" desc="Flash Region Base Address"/>
     </register>
```

### Comparing `chipsec-1.4.4/chipsec/cfg/pch_2xx.xml` & `chipsec-1.5.1/chipsec/cfg/8086/skl.xml`

 * *Files 8% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/pch_2xx.xml` & `chipsec-1.5.1/chipsec/cfg/8086/skl.xml`

```diff
@@ -1,50 +1,80 @@
 <?xml version="1.0" encoding="utf-8"?>
-<configuration platform="PCH_2xx">
+<configuration platform="SKL">
   <!--
-XML configuration file for 200 series PCH based platforms
+XML configuration file for Skylake based platforms
 
-* Intel(R) 200 Series Chipset Family Platform Controller Hub (PCH)
-  http://www.intel.com/content/www/us/en/processors/core/core-technical-resources.html
+http://www.intel.com/content/www/us/en/processors/core/core-technical-resources.html
+
+* 6th Generation Intel(R) Processor Datasheet for U/Y-Platforms
+
+* 6th Generation Intel(R) Processor I/O Datasheet for U/Y-Platforms
+
+* 6th Generation Intel(R) Processor Datasheet for S-Platforms
+
+* 6th Generation Intel(R) Processor Datasheet for H-Platforms
+
+* Intel(R) 100 Series Chipset Family Platform Controller Hub (PCH)
 -->
   <!-- #################################### -->
   <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info family="core">
+    <sku did="0x1904" name="Skylake" code="SKL" longname="Mobile 6th Generation Core Processor (Skylake U)"/>
+    <sku did="0x190C" name="Skylake" code="SKL" longname="Mobile 6th Generation Core Processor (Skylake Y)"/>
+    <sku did="0x1900" name="Skylake" code="SKL" longname="Mobile 6th Generation Core Processor Dual Core (Skylake H)"/>
+    <sku did="0x1910" name="Skylake" code="SKL" longname="Mobile 6th Generation Core Processor Quad Core (Skylake H)"/>
+    <sku did="0x190F" name="Skylake" code="SKL" longname="Desktop 6th Generation Core Processor Dual Core (Skylake CPU / Sunrise Point PCH)"/>
+    <sku did="0x191F" name="Skylake" code="SKL" longname="Desktop 6th Generation Core Processor Quad Core (Skylake CPU / Sunrise Point PCH)"/>
+    <sku did="0x1918" name="Skylake Server" code="SKL" longname="Intel Xeon Processor E3 v5 (Skylake CPU / Sunrise Point PCH)"/>
+  </info>
+  <!-- #################################### -->
+  <!--                                      -->
   <!-- Integrated devices                   -->
   <!--                                      -->
   <!-- #################################### -->
   <pci>
     <device name="P2SBC" bus="0" dev="0x1F" fun="1" vid="0x8086"/>
     <device name="SMBUS" bus="0" dev="0x1F" fun="4" vid="0x8086"/>
     <device name="SPI" bus="0" dev="0x1F" fun="5" vid="0x8086"/>
   </pci>
   <!-- #################################### -->
   <!--                                      -->
   <!-- Memory Mapped I/O spaces (MMIO BARs) -->
   <!--                                      -->
   <!-- #################################### -->
   <mmio>
+    <bar name="GTTMMADR" bus="0" dev="2" fun="0" reg="0x10" width="8" mask="0x7FFF000000" desc="Graphics Translation Table Range"/>
     <bar name="HDABAR" bus="0" dev="0x1F" fun="3" reg="0x10" width="8" mask="0xFFFFFFFFFFFFC000" size="0x1000" desc="HD Audio Base"/>
     <bar name="SPIBAR" bus="0" dev="0x1F" fun="5" reg="0x10" width="4" mask="0xFFFFF000" size="0x1000" desc="SPI Controller Register Range" offset="0x0"/>
     <bar name="PWRMBASE" register="PWRMBASE" base_field="BA" size="0x1000" fixed_address="0xFE000000" desc="Power Management Register Range"/>
     <bar name="SBREGBAR" register="SBREG_BAR" base_field="RBA" size="0x1000000" fixed_address="0xFD000000" desc="Sideband Register Access BAR"/>
   </mmio>
   <!-- #################################### -->
   <!--                                      -->
   <!-- I/O spaces (I/O BARs)                -->
   <!--                                      -->
   <!-- #################################### -->
   <io>
-    <bar name="ABASE" register="ABASE" base_field="BA" size="0x100" fixed_address="0x1800" desc="ACPI Base Address"/>
-    <bar name="PMBASE" register="ABASE" base_field="BA" size="0x100" fixed_address="0x1800" desc="ACPI Base Address"/>
+    <bar name="ABASE" register="ABASE" base_field="BA" size="0x100" desc="ACPI Base Address"/>
+    <bar name="PMBASE" register="ABASE" base_field="BA" size="0x100" desc="ACPI Base Address"/>
     <bar name="TCOBASE" register="TCOBASE" base_field="TCOBA" size="0x20" desc="TCO Base Address"/>
     <!-- old definition -->
     <bar name="SMBUS_BASE" bus="0" dev="0x1F" fun="4" reg="0x20" mask="0xFFE0" size="0x80" desc="SMBus Base Address"/>
   </io>
   <!-- #################################### -->
   <!--                                      -->
+  <!-- Memory ranges                        -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <memory/>
+  <!-- #################################### -->
+  <!--                                      -->
   <!-- Configuration registers              -->
   <!--                                      -->
   <!-- #################################### -->
   <registers>
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- PCIe Configuration registers -->
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
@@ -118,22 +148,15 @@
       <field name="FDOPSS" bit="13" size="1" desc="Flash Descriptor Override Pin-Strap Status"/>
       <field name="FDV" bit="14" size="1" desc="Flash Descriptor Valid"/>
       <field name="FLOCKDN" bit="15" size="1" desc="Flash Configuration Lock-Down"/>
       <field name="FGO" bit="16" size="1" desc="Flash cycle go"/>
       <field name="FCYCLE" bit="17" size="4" desc="Flash Cycle Type"/>
       <field name="WET" bit="21" size="1" desc="Write Enable Type"/>
       <field name="FDBC" bit="24" size="6" desc="Flash Data Byte Count"/>
-      <field name="FSMIE" bit="31" size="1" desc="Flash SPI SMI# Enable"/>
-    </register>
-    <register name="HSFC" type="mmio" bar="SPIBAR" offset="0x06" size="2" desc="Hardware Sequencing Flash Control Register">
-      <field name="FGO" bit="0" size="1" desc="Flash Cycle GO"/>
-      <field name="FCYCLE" bit="1" size="4" desc="Flash Cycle"/>
-      <field name="WET" bit="5" size="1" desc="Write Enable Type"/>
-      <field name="FDBC" bit="8" size="6" desc="Flash Data Byte Count, Count = FDBC + 1"/>
-      <field name="FSMIE" bit="15" size="1" desc="Flash SPI SMI Enable"/>
+      <field name="FSMIE" bit="31" size="1" desc="Flash SPI SMI Enable"/>
     </register>
     <register name="FREG0_FLASHD" type="mmio" bar="SPIBAR" offset="0x54" size="4" desc="Flash Region 0 (Flash Descriptor)">
       <field name="RB" bit="0" size="15" desc="Region Base"/>
       <field name="RL" bit="16" size="15" desc="Region Limit"/>
     </register>
     <register name="FREG1_BIOS" type="mmio" bar="SPIBAR" offset="0x58" size="4" desc="Flash Region 1 (BIOS)">
       <field name="RB" bit="0" size="15" desc="Region Base"/>
@@ -230,15 +253,15 @@
       <field name="LL" bit="3" size="1" desc="Lower 128 Byte Lock"/>
       <field name="UL" bit="4" size="1" desc="Upper 128 Byte Lock"/>
       <field name="BILD" bit="31" size="1" desc="BIOS Interface Lock-Down"/>
     </register>
     <register name="BUC" type="mm_msgbus" port="0xC3" offset="0x3414" size="4" desc="Backed Up Control">
       <field name="TS" bit="0" size="1" desc="Top Swap"/>
     </register>
-    <!-- PMC MMIO registers (7th/8th Generation Intel(R) Processor Families I/O for U/Y-Platforms, Vol. 2, section 4.3) -->
+    <!-- PMC MMIO registers (6th Generation Intel(R) Processor I/O Datasheet for U/Y-Platforms, Vol. 2, section 4.3) -->
     <register name="PM_CFG" type="mmio" bar="PWRMBASE" offset="0x18" size="4" desc="Power Management Configuration Reg 1"/>
     <!-- SPI Flash Descriptor registers -->
     <register name="FLMAP0" type="mmio" bar="FDBAR" offset="0x14" size="4" desc="Flash Map 0 Register">
       <field name="FCBA" bit="0" size="8" desc="Flash Component Base Address"/>
       <field name="NC" bit="8" size="2" desc="Number of Components"/>
       <field name="FRBA" bit="16" size="8" desc="Flash Region Base Address"/>
     </register>
```

### Comparing `chipsec-1.4.4/chipsec/cfg/byt.xml` & `chipsec-1.5.1/chipsec/cfg/8086/byt.xml`

 * *Files 4% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/byt.xml` & `chipsec-1.5.1/chipsec/cfg/8086/byt.xml`

```diff
@@ -4,14 +4,22 @@
 XML configuration for Bay Trail based platforms
 
 * Intel(R) Atom(TM) Processor E3800 Product Family Datasheet, May 2016, Revision 4.0
   http://www.intel.com/content/www/us/en/embedded/products/bay-trail/atom-e3800-family-datasheet.html
 -->
   <!-- #################################### -->
   <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info family="atom">
+    <sku did="0x0F00" name="Baytrail" code="BYT" longname="Bay Trail SoC"/>
+  </info>
+  <!-- #################################### -->
+  <!--                                      -->
   <!-- Memory Mapped I/O spaces (MMIO BARs) -->
   <!--                                      -->
   <!-- #################################### -->
   <mmio>
     <!-- Section 14.9.5-14.9.6 -->
     <bar name="GTTMMADR" bus="0" dev="0x02" fun="0" reg="0x10" width="8" mask="0xFFFFFFF0FFC00000" desc="Graphics Translation Table Range"/>
     <!-- Section 35.6 -->
```

### Comparing `chipsec-1.4.4/chipsec/cfg/cfl.xml` & `chipsec-1.5.1/chipsec/cfg/8086/pch_3xxop.xml`

 * *Files 5% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/cfl.xml` & `chipsec-1.5.1/chipsec/cfg/8086/pch_3xxop.xml`

```diff
@@ -1,45 +1,52 @@
 <?xml version="1.0" encoding="utf-8"?>
-<configuration platform="CFL">
+<configuration platform="PCH_3xxOP">
   <!--
-XML configuration file for Coffee Lake
-
-* 8th Generation Intel(R) Processor Family for S-Processor Platforms
-  https://www.intel.com/content/www/us/en/processors/core/core-technical-resources.html
+XML configuration file for the 300 series On Package PCH
+https://www.intel.com/content/www/us/en/products/docs/chipsets/300-series-chipset-on-package-pch-datasheet-vol-2.html
+337868-002
 -->
   <!-- #################################### -->
   <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info>
+    <sku did="0x9D84" name="PCH-U" code="PCH_3xxOP" longname="Intel 300 series On-Package PCH"/>
+  </info>
+  <!-- #################################### -->
+  <!--                                      -->
   <!-- Integrated devices                   -->
   <!--                                      -->
   <!-- #################################### -->
   <pci>
     <device name="P2SBC" bus="0" dev="0x1F" fun="1" vid="0x8086"/>
+    <device name="PMC" bus="0" dev="0x1F" fun="2" vid="0x8086"/>
     <device name="SMBUS" bus="0" dev="0x1F" fun="4" vid="0x8086"/>
     <device name="SPI" bus="0" dev="0x1F" fun="5" vid="0x8086"/>
   </pci>
   <!-- #################################### -->
   <!--                                      -->
   <!-- Memory Mapped I/O spaces (MMIO BARs) -->
   <!--                                      -->
   <!-- #################################### -->
   <mmio>
-    <bar name="GTTMMADR" bus="0" dev="2" fun="0" reg="0x10" width="8" mask="0x7FFF000000" desc="Graphics Translation Table Range"/>
     <bar name="HDABAR" bus="0" dev="0x1F" fun="3" reg="0x10" width="8" mask="0xFFFFFFFFFFFFC000" size="0x1000" desc="HD Audio Base"/>
     <bar name="SPIBAR" bus="0" dev="0x1F" fun="5" reg="0x10" width="4" mask="0xFFFFF000" size="0x1000" desc="SPI Controller Register Range" offset="0x0"/>
     <bar name="PWRMBASE" register="PWRMBASE" base_field="BA" size="0x1000" fixed_address="0xFE000000" desc="Power Management Register Range"/>
     <bar name="SBREGBAR" register="SBREG_BAR" base_field="RBA" size="0x1000000" fixed_address="0xFD000000" desc="Sideband Register Access BAR"/>
   </mmio>
   <!-- #################################### -->
   <!--                                      -->
   <!-- I/O spaces (I/O BARs)                -->
   <!--                                      -->
   <!-- #################################### -->
   <io>
-    <bar name="ABASE" register="ABASE" base_field="BA" size="0x100" desc="ACPI Base Address"/>
-    <bar name="PMBASE" register="ABASE" base_field="BA" size="0x100" desc="ACPI Base Address"/>
+    <bar name="ABASE" register="ABASE" base_field="BA" size="0x100" fixed_address="0x1800" desc="ACPI Base Address"/>
+    <bar name="PMBASE" register="ABASE" base_field="BA" size="0x100" fixed_address="0x1800" desc="ACPI Base Address"/>
     <bar name="TCOBASE" register="TCOBASE" base_field="TCOBA" size="0x20" desc="TCO Base Address"/>
     <!-- old definition -->
     <bar name="SMBUS_BASE" bus="0" dev="0x1F" fun="4" reg="0x20" mask="0xFFE0" size="0x80" desc="SMBus Base Address"/>
   </io>
   <!-- #################################### -->
   <!--                                      -->
   <!-- Memory ranges                        -->
@@ -66,26 +73,26 @@
       <field name="HIDE" bit="0" size="1" desc="Hide SBREG_BAR"/>
     </register>
     <!-- Power Management Controller -->
     <register name="ABASE" type="pcicfg" bus="0" dev="0x1f" fun="2" offset="0x40" size="4" desc="ACPI Base Address">
       <field name="STYPE" bit="0" size="1" desc="Space Type (always 1 - I/O space)"/>
       <field name="BA" bit="8" size="8" desc="Base Address"/>
     </register>
-    <register name="ACTL" type="pcicfg" bus="0" dev="0x1f" fun="2" offset="0x44" size="4" desc="ACPI Control">
-      <field name="SCIS" bit="0" size="2" desc="SCI IRQ Select"/>
-      <field name="EN" bit="7" size="1" desc="ACPI Enable"/>
-      <field name="PWRM_EN" bit="8" size="1" desc="PWRM Enable"/>
-    </register>
-    <register name="PWRMBASE" type="pcicfg" bus="0" dev="0x1f" fun="2" offset="0x48" size="4" desc="PM Base Address">
+    <register name="PWRMBASE" type="pcicfg" bus="0" dev="0x1f" fun="2" offset="0x10" size="8" desc="PM Base Address">
       <field name="STYPE" bit="0" size="1" desc="Space Type (always 0 - memory space)"/>
-      <field name="BA" bit="12" size="20" desc="Base Address"/>
+      <field name="BA" bit="12" size="52" desc="Base Address"/>
     </register>
-    <register name="GEN_PMCON_1" type="pcicfg" bus="0" dev="0x1f" fun="2" offset="0xA0" size="2" desc="General PM Configuration A">
+    <register name="GEN_PMCON_1" type="mmio" bar="PWRMBASE" offset="0x1020" size="4" desc="General PM Configuration A"/>
+    <register name="GEN_PMCON_2" type="mmio" bar="PWRMBASE" offset="0x1024" size="4" desc="General PM Configuration B">
       <field name="SMI_LOCK" bit="4" size="1"/>
     </register>
+    <register name="ACTL" type="mmio" bar="PWRMBASE" offset="0x1BD8" size="4" desc="ACPI Control">
+      <field name="SCIS" bit="0" size="3" desc="SCI IRQ Select"/>
+    </register>
+    <register name="PM_CFG" type="mmio" bar="PWRMBASE" offset="0x1818" size="4" desc="Power Management Configuration Reg 1"/>
     <!-- SMBus Host Controller -->
     <register name="SMBUS_VID" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x00" size="2" desc="VID"/>
     <register name="SMBUS_DID" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x02" size="2" desc="DID"/>
     <register name="SMBUS_CMD" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x04" size="2" desc="CMD"/>
     <register name="SMBUS_HCFG" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x40" size="1" desc="Host Configuration">
       <field name="HST_EN" bit="0" size="1"/>
       <field name="SMB_SMI_EN" bit="1" size="1"/>
@@ -153,39 +160,39 @@
     </register>
     <register name="FREG5" type="mmio" bar="SPIBAR" offset="0x68" size="4" desc="Flash Region 5">
       <field name="RB" bit="0" size="15" desc="Region Base"/>
       <field name="RL" bit="16" size="15" desc="Region Limit"/>
     </register>
     <register name="FREG6" undef="Flash Region 6 not defined for this platform"/>
     <register name="PR0" type="mmio" bar="SPIBAR" offset="0x84" size="4" desc="Protected Range 0">
-      <field name="PRB" bit="0" size="13"/>
+      <field name="PRB" bit="0" size="15"/>
       <field name="RPE" bit="15" size="1"/>
       <field name="PRL" bit="16" size="15"/>
       <field name="WPE" bit="31" size="1"/>
     </register>
     <register name="PR1" type="mmio" bar="SPIBAR" offset="0x88" size="4" desc="Protected Range 1">
-      <field name="PRB" bit="0" size="13"/>
+      <field name="PRB" bit="0" size="15"/>
       <field name="RPE" bit="15" size="1"/>
       <field name="PRL" bit="16" size="15"/>
       <field name="WPE" bit="31" size="1"/>
     </register>
     <register name="PR2" type="mmio" bar="SPIBAR" offset="0x8C" size="4" desc="Protected Range 2">
-      <field name="PRB" bit="0" size="13"/>
+      <field name="PRB" bit="0" size="15"/>
       <field name="RPE" bit="15" size="1"/>
       <field name="PRL" bit="16" size="15"/>
       <field name="WPE" bit="31" size="1"/>
     </register>
     <register name="PR3" type="mmio" bar="SPIBAR" offset="0x90" size="4" desc="Protected Range 3">
-      <field name="PRB" bit="0" size="13"/>
+      <field name="PRB" bit="0" size="15"/>
       <field name="RPE" bit="15" size="1"/>
       <field name="PRL" bit="16" size="15"/>
       <field name="WPE" bit="31" size="1"/>
     </register>
     <register name="PR4" type="mmio" bar="SPIBAR" offset="0x94" size="4" desc="Protected Range 4">
-      <field name="PRB" bit="0" size="13"/>
+      <field name="PRB" bit="0" size="15"/>
       <field name="RPE" bit="15" size="1"/>
       <field name="PRL" bit="16" size="15"/>
       <field name="WPE" bit="31" size="1"/>
     </register>
     <register name="FDOC" type="mmio" bar="SPIBAR" offset="0xB4" size="4" desc="Flash Descriptor Observability Control Register">
       <field name="FDSI" bit="2" size="10" desc="Flash Descriptor Section Index"/>
       <field name="FDSS" bit="12" size="3" desc="Flash Descriptor Section Select"/>
@@ -230,15 +237,14 @@
       <field name="LL" bit="3" size="1" desc="Lower 128 Byte Lock"/>
       <field name="UL" bit="4" size="1" desc="Upper 128 Byte Lock"/>
       <field name="BILD" bit="31" size="1" desc="BIOS Interface Lock-Down"/>
     </register>
     <register name="BUC" type="mm_msgbus" port="0xC3" offset="0x3414" size="4" desc="Backed Up Control">
       <field name="TS" bit="0" size="1" desc="Top Swap"/>
     </register>
-    <register name="PM_CFG" type="mmio" bar="PWRMBASE" offset="0x18" size="4" desc="Power Management Configuration Reg 1"/>
     <!-- DCI registers -->
     <register name="ECTRL" type="mm_msgbus" port="0xB8" offset="0x0004" size="4" desc="DCI Control Register">
       <field name="ENABLE" bit="4" size="1"/>
     </register>
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- I/O registers (I/O ports)    -->
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
@@ -251,9 +257,10 @@
   <!--                                      -->
   <!-- 'Controls'                           -->
   <!--                                      -->
   <!-- #################################### -->
   <controls>
     <control name="BiosInterfaceLockDown" register="BC" field="BILD" desc="BIOS Interface Lock-Down"/>
     <control name="SpiWriteStatusDis" register="HSFS" field="WRSDIS" desc="Write Status Disable"/>
+    <control name="SMILock" register="GEN_PMCON_2" field="SMI_LOCK" desc="SMI Global Configuration Lock"/>
   </controls>
 </configuration>
```

### Comparing `chipsec-1.4.4/chipsec/cfg/whl.xml` & `chipsec-1.5.1/chipsec/cfg/8086/whl.xml`

 * *Files 27% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/whl.xml` & `chipsec-1.5.1/chipsec/cfg/8086/whl.xml`

```diff
@@ -5,14 +5,23 @@
 
 * 8th Generation Intel(R) Processor Family for U-Processor Platforms
   https://www.intel.com/content/www/us/en/processors/core/core-technical-resources.html
   https://www.intel.com/content/dam/www/public/us/en/documents/technical-specifications/300-series-chipset-on-package-pch-datasheet-vol-1.pdf
 -->
   <!-- #################################### -->
   <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info family="core">
+    <sku did="0x3E34" name="Whiskey Lake" code="WHL" longname="Mobile 8th Generation Core Processor (Whiskey Lake U 4 Cores)" detection_value="806EA"/>
+    <sku did="0x3E34" name="Whiskey Lake" code="WHL" longname="Mobile 8th Generation Core Processor (Whiskey Lake U 4 Cores)" detection_value="806EB"/>
+  </info>
+  <!-- #################################### -->
+  <!--                                      -->
   <!-- Integrated devices                   -->
   <!--                                      -->
   <!-- #################################### -->
   <pci/>
   <!-- #################################### -->
   <!--                                      -->
   <!-- Memory Mapped I/O spaces (MMIO BARs) -->
@@ -34,15 +43,22 @@
   <!-- #################################### -->
   <memory/>
   <!-- #################################### -->
   <!--                                      -->
   <!-- Configuration registers              -->
   <!--                                      -->
   <!-- #################################### -->
-  <registers/>
+  <registers>
+    <register name="PCI0.0.0_PCIEXBAR" type="pcicfg" device="HOSTCTRL" offset="0x60" size="8" desc="PCIe MMCFG Base Address">
+      <field name="PCIEXBAREN" bit="0" size="1" desc="Enable"/>
+      <Field name="LENGTH" bit="1" size="2" desc="Length of region"/>
+      <Field name="RESERVED" bit="3" size="23" desc="Reserved"/>
+      <Field name="PCIEXBAR" bit="26" size="13" desc="Base Address for PCI Express"/>
+    </register>
+  </registers>
   <!-- #################################### -->
   <!--                                      -->
   <!-- 'Controls'                           -->
   <!--                                      -->
   <!-- #################################### -->
   <controls/>
 </configuration>
```

### Comparing `chipsec-1.4.4/chipsec/cfg/qrk.xml` & `chipsec-1.5.1/chipsec/cfg/8086/qrk.xml`

 * *Files 4% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/qrk.xml` & `chipsec-1.5.1/chipsec/cfg/8086/qrk.xml`

```diff
@@ -1,14 +1,22 @@
 <?xml version="1.0" encoding="utf-8"?>
 <configuration platform="QRK">
   <!--
 XML configuration for Quark based platforms
 -->
   <!-- #################################### -->
   <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info family="quark">
+    <sku did="0x0958" name="Galileo " code="QRK" longname="Intel Quark SoC X1000"/>
+  </info>
+  <!-- #################################### -->
+  <!--                                      -->
   <!-- Memory Mapped I/O spaces (MMIO BARs) -->
   <!--                                      -->
   <!-- #################################### -->
   <mmio>
     <bar name="MMCFG" register="BECREG" base_field="ECBASE" size="0x10000000" enable_bit="ECENABLE" desc="PCI Express Register Range"/>
   </mmio>
   <!-- #################################### -->
```

### Comparing `chipsec-1.4.4/chipsec/cfg/pch_c60x.xml` & `chipsec-1.5.1/chipsec/cfg/8086/pch_c60x.xml`

 * *Files 23% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/pch_c60x.xml` & `chipsec-1.5.1/chipsec/cfg/8086/pch_c60x.xml`

```diff
@@ -1,15 +1,23 @@
 <?xml version="1.0" encoding="utf-8"?>
-<configuration platform="PCH_C60X">
+<configuration platform="PCH_C60x">
   <!--
 XML configuration file for C600 series PCH
   Intel (c) C600 Series Chipset and Intel (c) X79 Express Chipset datasheet
   Intel (c) C600 Series Chipset and Intel (c) X79 Express Chipset Specification Update
   https://ark.intel.com/products/series/98463/Intel-C600-Series-Chipsets
 -->
+  <!-- #################################### -->
+  <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info>
+    <sku did="0x1D41" name="C600" code="PCH_C60x" longname="Intel C600/X79 series PCH"/>
+  </info>
   <pci>
     <device name="LPC" bus="0" dev="0x1F" fun="0" vid="0x8086" did="0x1D41"/>
   </pci>
   <registers>
     <!-- LPC Interface Bridge -->
     <register name="GEN_PMCON_LOCK" type="pcicfg" device="LPC" offset="0xA6" size="1" desc="General Power Management Configuration Lock">
       <field name="ACPI_BASE_LOCK" bit="1" size="1" desc="Lock down ACPI Base Address (ABASE)"/>
```

### Comparing `chipsec-1.4.4/chipsec/cfg/pch_3xx.xml` & `chipsec-1.5.1/chipsec/cfg/8086/pch_4xxlp.xml`

 * *Files 4% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/pch_3xx.xml` & `chipsec-1.5.1/chipsec/cfg/8086/pch_4xxlp.xml`

```diff
@@ -1,19 +1,29 @@
 <?xml version="1.0" encoding="utf-8"?>
-<configuration platform="PCH_3xx">
+<configuration platform="PCH_4xxLP">
   <!--
-XML configuration file for the 300 series PCH
+XML configuration file for the 400 series LP (U/H) PCH
 -->
   <!-- #################################### -->
   <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info>
+    <sku did="0x0284" name="PCH-LP-Prem" code="PCH_4xxLP" longname="Intel 400 series PCH-LP Prem-U"/>
+    <sku did="0x0285" name="PCH-LP" code="PCH_4xxLP" longname="Intel 400 series PCH-LP Base-U"/>
+  </info>
+  <!-- #################################### -->
+  <!--                                      -->
   <!-- Integrated devices                   -->
   <!--                                      -->
   <!-- #################################### -->
   <pci>
     <device name="P2SBC" bus="0" dev="0x1F" fun="1" vid="0x8086"/>
+    <device name="PMC" bus="0" dev="0x1F" fun="2" vid="0x8086"/>
     <device name="SMBUS" bus="0" dev="0x1F" fun="4" vid="0x8086"/>
     <device name="SPI" bus="0" dev="0x1F" fun="5" vid="0x8086"/>
   </pci>
   <!-- #################################### -->
   <!--                                      -->
   <!-- Memory Mapped I/O spaces (MMIO BARs) -->
   <!--                                      -->
@@ -48,73 +58,85 @@
   <!--                                      -->
   <!-- #################################### -->
   <registers>
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- PCIe Configuration registers -->
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- Sideband Register Access Registers -->
-    <register name="SBREG_BAR" type="pcicfg" bus="0" dev="0x1F" fun="1" offset="0x10" size="4" desc="Sideband Register Access BAR">
+    <register name="SBREG_BAR" type="pcicfg" device="P2SBC" offset="0x10" size="4" desc="Sideband Register Access BAR">
       <field name="RBA" bit="24" size="8" desc="Register Base Address"/>
     </register>
-    <register name="P2SBC" type="pcicfg" bus="0" dev="0x1F" fun="1" offset="0xE0" size="2" desc="P2SB Configuration Register">
+    <register name="P2SBC" type="pcicfg" device="P2SBC" offset="0xE0" size="2" desc="P2SB Configuration Register">
       <field name="HIDE" bit="8" size="1" desc="Hide SBREG_BAR"/>
     </register>
-    <register name="P2SB_HIDE" type="pcicfg" bus="0" dev="0x1F" fun="1" offset="0xE1" size="1" desc="P2SB Configuration Register hide-unhide">
+    <register name="P2SB_HIDE" type="pcicfg" device="P2SBC" offset="0xE1" size="1" desc="P2SB Configuration Register hide-unhide">
       <field name="HIDE" bit="0" size="1" desc="Hide SBREG_BAR"/>
     </register>
     <!-- Power Management Controller -->
-    <register name="ABASE" type="pcicfg" bus="0" dev="0x1f" fun="2" offset="0x40" size="4" desc="ACPI Base Address">
+    <register name="ABASE" type="pcicfg" device="PMC" offset="0x20" size="4" desc="ACPI Base Address">
       <field name="STYPE" bit="0" size="1" desc="Space Type (always 1 - I/O space)"/>
-      <field name="BA" bit="8" size="8" desc="Base Address"/>
+      <field name="BA" bit="7" size="25" desc="Base Address"/>
     </register>
-    <register name="PWRMBASE" type="pcicfg" bus="0" dev="0x1f" fun="2" offset="0x10" size="8" desc="PM Base Address">
+    <register name="PWRMBASE" type="pcicfg" device="PMC" offset="0x10" size="4" desc="PM Base Address">
       <field name="STYPE" bit="0" size="1" desc="Space Type (always 0 - memory space)"/>
-      <field name="BA" bit="13" size="51" desc="Base Address"/>
+      <field name="BA" bit="13" size="19" desc="Base Address"/>
+    </register>
+    <register name="GEN_PMCON_1" type="mmio" bar="PWRMBASE" offset="0x1020" size="4" desc="General PM Configuration A">
+      <field name="ESPI_SMI_LOCK" bit="8" size="1" desc="ESPI_SMI_LOCK"/>
     </register>
-    <register name="GEN_PMCON_1" type="mmio" bar="PWRMBASE" offset="0x1020" size="4" desc="General PM Configuration A"/>
     <register name="GEN_PMCON_2" type="mmio" bar="PWRMBASE" offset="0x1024" size="4" desc="General PM Configuration B">
       <field name="SMI_LOCK" bit="4" size="1"/>
     </register>
+    <register name="PM_CFG" type="mmio" bar="PWRMBASE" offset="0x1818" size="4" desc="Power Management Configuration Reg 1"/>
     <register name="ACTL" type="mmio" bar="PWRMBASE" offset="0x1BD8" size="4" desc="ACPI Control">
       <field name="SCIS" bit="0" size="3" desc="SCI IRQ Select"/>
     </register>
     <!-- SMBus Host Controller -->
-    <register name="SMBUS_VID" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x00" size="2" desc="VID"/>
-    <register name="SMBUS_DID" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x02" size="2" desc="DID"/>
-    <register name="SMBUS_CMD" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x04" size="2" desc="CMD"/>
-    <register name="SMBUS_HCFG" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x40" size="1" desc="Host Configuration">
+    <register name="SMBUS_VID" type="pcicfg" device="SMBUS" offset="0x00" size="2" desc="VID"/>
+    <register name="SMBUS_DID" type="pcicfg" device="SMBUS" offset="0x02" size="2" desc="DID"/>
+    <register name="SMBUS_CMD" type="pcicfg" device="SMBUS" offset="0x04" size="2" desc="CMD"/>
+    <register name="SMBUS_HCFG" type="pcicfg" device="SMBUS" offset="0x40" size="1" desc="Host Configuration">
       <field name="HST_EN" bit="0" size="1"/>
       <field name="SMB_SMI_EN" bit="1" size="1"/>
-      <field name="I2C_EN" bit="2" size="2"/>
+      <field name="I2C_EN" bit="2" size="1"/>
       <field name="SSRESET" bit="3" size="1"/>
       <field name="SPD_WD" bit="4" size="1"/>
     </register>
-    <register name="TCOBASE" type="pcicfg" bus="0" dev="0x1f" fun="4" offset="0x50" size="4" desc="TCO Base Address">
+    <register name="SMBBASE" type="pcicfg" device="SMBUS" offset="0x20" size="4" desc="SMB Base Address">
+      <field name="IOS" bit="0" size="1" desc="I/O space"/>
+      <field name="SMBBA" bit="5" size="11" desc="SMB Base Address"/>
+    </register>
+    <register name="TCOBASE" type="pcicfg" device="SMBUS" offset="0x50" size="4" desc="TCO Base Address">
       <field name="IOS" bit="0" size="1" desc="I/O space"/>
       <field name="TCOBA" bit="5" size="11" desc="TCO Base Address"/>
     </register>
-    <register name="TCOCTL" type="pcicfg" bus="0" dev="0x1f" fun="4" offset="0x54" size="4" desc="TCO Control">
+    <register name="TCOCTL" type="pcicfg" device="SMBUS" offset="0x54" size="4" desc="TCO Control">
       <field name="TCO_BASE_LOCK" bit="0" size="1" desc="TCO Base Lock"/>
       <field name="TCO_BASE_EN" bit="8" size="1" desc="TCO Base Enable"/>
     </register>
     <!-- SPI Interface Controller -->
-    <register name="BC" type="pcicfg" bus="0" dev="0x1F" fun="5" offset="0xDC" size="4" desc="BIOS Control">
+    <register name="BC" type="pcicfg" device="SPI" offset="0xDC" size="4" desc="BIOS Control">
       <field name="BIOSWE" bit="0" size="1" desc="BIOS Write Enable"/>
       <field name="BLE" bit="1" size="1" desc="BIOS Lock Enable"/>
       <field name="SRC" bit="2" size="2" desc="SPI Read Configuration"/>
       <field name="TSS" bit="4" size="1" desc="Top Swap Status"/>
       <field name="SMM_BWP" bit="5" size="1" desc="SMM BIOS Write Protection"/>
       <field name="BBS" bit="6" size="1" desc="Boot BIOS Strap"/>
       <field name="BILD" bit="7" size="1" desc="BIOS Interface Lock Down"/>
+      <field name="ASE_BWP" bit="11" size="1" desc="Async SMI Enable for BIOS Write Protection"/>
     </register>
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- MMIO registers               -->
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- PCH SPIBAR registers -->
-    <register name="HSFS" type="mmio" bar="SPIBAR" offset="0x04" size="4" desc="Hardware Sequencing Flash Status Register">
+    <register name="BFPR" type="mmio" bar="SPIBAR" offset="0x00" size="4" desc="BIOS Flash Primary Region Register (= FREG1)">
+      <field name="PRB" bit="0" size="15" desc="BIOS Flash Primary Region Base"/>
+      <field name="PRL" bit="16" size="15" desc="BIOS Flash Primary Region Limit"/>
+    </register>
+    <register name="HSFS" type="mmio" bar="SPIBAR" offset="0x4" size="4" desc="Hardware Sequencing Flash Status Register">
       <field name="FDONE" bit="0" size="1" desc="Flash Cycle Done"/>
       <field name="FCERR" bit="1" size="1" desc="Flash Cycle Error"/>
       <field name="AEL" bit="2" size="1" desc="Access Error Log"/>
       <field name="SCIP" bit="5" size="1" desc="SPI cycle in progress"/>
       <field name="WRSDIS" bit="11" size="1" desc="Write status disable"/>
       <field name="PR34LKD" bit="12" size="1" desc="PRR3 PRR4 Lock-Down"/>
       <field name="FDOPSS" bit="13" size="1" desc="Flash Descriptor Override Pin-Strap Status"/>
@@ -146,15 +168,14 @@
       <field name="RB" bit="0" size="15" desc="Region Base"/>
       <field name="RL" bit="16" size="15" desc="Region Limit"/>
     </register>
     <register name="FREG5" type="mmio" bar="SPIBAR" offset="0x68" size="4" desc="Flash Region 5">
       <field name="RB" bit="0" size="15" desc="Region Base"/>
       <field name="RL" bit="16" size="15" desc="Region Limit"/>
     </register>
-    <register name="FREG6" undef="Flash Region 6 not defined for this platform"/>
     <register name="PR0" type="mmio" bar="SPIBAR" offset="0x84" size="4" desc="Protected Range 0">
       <field name="PRB" bit="0" size="15"/>
       <field name="RPE" bit="15" size="1"/>
       <field name="PRL" bit="16" size="15"/>
       <field name="WPE" bit="31" size="1"/>
     </register>
     <register name="PR1" type="mmio" bar="SPIBAR" offset="0x88" size="4" desc="Protected Range 1">
@@ -225,31 +246,37 @@
       <field name="LL" bit="3" size="1" desc="Lower 128 Byte Lock"/>
       <field name="UL" bit="4" size="1" desc="Upper 128 Byte Lock"/>
       <field name="BILD" bit="31" size="1" desc="BIOS Interface Lock-Down"/>
     </register>
     <register name="BUC" type="mm_msgbus" port="0xC3" offset="0x3414" size="4" desc="Backed Up Control">
       <field name="TS" bit="0" size="1" desc="Top Swap"/>
     </register>
-    <register name="PM_CFG" type="mmio" bar="PWRMBASE" offset="0x1818" size="4" desc="Power Management Configuration Reg 1"/>
     <!-- DCI registers -->
     <register name="ECTRL" type="mm_msgbus" port="0xB8" offset="0x0004" size="4" desc="DCI Control Register">
+      <field name="LOCK" bit="0" size="1"/>
       <field name="ENABLE" bit="4" size="1"/>
     </register>
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- I/O registers (I/O ports)    -->
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- PCH TCOBASE (SMBus TCO) I/O registers -->
     <register name="TCO1_CNT" type="iobar" bar="TCOBASE" offset="0x8" size="2" desc="TCO1 Control">
       <field name="TCO_LOCK" bit="12" size="1" desc="TCO Lock"/>
     </register>
+    <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
+    <!--      Undefined Registers     -->
+    <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
+    <register name="GC" undef="Not defined for platform"/>
   </registers>
   <!-- #################################### -->
   <!--                                      -->
   <!-- 'Controls'                           -->
   <!--                                      -->
   <!-- #################################### -->
   <controls>
     <control name="BiosInterfaceLockDown" register="BC" field="BILD" desc="BIOS Interface Lock-Down"/>
+    <control name="TopSwap" register="BC" field="TSS" desc="Top Swap Status"/>
     <control name="SpiWriteStatusDis" register="HSFS" field="WRSDIS" desc="Write Status Disable"/>
     <control name="SMILock" register="GEN_PMCON_2" field="SMI_LOCK" desc="SMI Global Configuration Lock"/>
+    <control name="TcoCtlLock" register="TCOCTL" field="TCO_BASE_LOCK" desc="TCO Base Lock"/>
   </controls>
 </configuration>
```

### Comparing `chipsec-1.4.4/chipsec/cfg/iommu.xml` & `chipsec-1.5.1/chipsec/cfg/8086/iommu.xml`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/cfg/template.xml` & `chipsec-1.5.1/chipsec/cfg/template.xml`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/cfg/dnv.xml` & `chipsec-1.5.1/chipsec/cfg/8086/dnv.xml`

 * *Files 18% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/dnv.xml` & `chipsec-1.5.1/chipsec/cfg/8086/dnv.xml`

```diff
@@ -1,25 +1,43 @@
 <?xml version="1.0" encoding="utf-8"?>
 <configuration platform="DNV">
   <!--
 XML configuration file for Denverton
 
 * Intel Atom(R) Processor C3000 Product Family
   https://www.intel.com/content/www/us/en/processors/atom/atom-technical-resources.html
+  337018-002
 -->
+  <!-- #################################### -->
+  <info family="atom">
+    <sku did="0x1980" name="Denverton" code="DNV" longname="Intel Atom Processor C3000 Product Family"/>
+  </info>
   <pci/>
   <mmio>
     <bar name="SPIBAR" bus="0" dev="0x1F" fun="5" reg="0x10" width="4" mask="0xFFFFC000" size="0x200" desc="SPI Controller Register Range"/>
   </mmio>
   <io>
     <bar name="ABASE" register="ABASE" base_field="Base" size="0x100" desc="ACPI Base Address"/>
     <bar name="TCOBASE" register="TCOBASE" base_field="Base" size="0x20" desc="TCO Base Address"/>
   </io>
   <memory/>
   <registers>
+    <register name="P2SBC" type="pcicfg" bus="0" dev="0x1F" fun="1" offset="0xE0" size="4" desc="P2SB Control">
+      <field name="MASKLOCK" bit="17" size="12" desc="Base address"/>
+    </register>
+    <register name="SMBUS_HCFG" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x40" size="1" desc="Host Configuration">
+      <field name="SPD_WD" bit="4" size="1" desc="SPD Write Disable"/>
+    </register>
+    <register name="SMI_EN" type="iobar" bar="ABASE" offset="0x30" size="4" desc="SMI Control and Enable">
+      <field name="GBL_SMI_EN" bit="0" size="1"/>
+      <field name="TCO_EN" bit="13" size="1"/>
+    </register>
+    <register name="TCO1_CNT" type="iobar" bar="TCOBASE" offset="0x8" size="4" desc="SMI Control and Enable">
+      <field name="TCO_LOCK" bit="12" size="1"/>
+    </register>
     <register name="BC" type="pcicfg" bus="0" dev="0x1F" fun="5" offset="0xDC" size="1" desc="BIOS Control">
       <field name="BIOSWE" bit="0" size="1" desc="Write Protect Disable"/>
       <field name="BLE" bit="1" size="1" desc="BIOS Lock Enable"/>
       <field name="SRC" bit="2" size="2" desc="SPI Read Configuration"/>
       <field name="TSS" bit="4" size="1" desc="Top Swap Status"/>
       <field name="SMM_BWP" bit="5" size="1" desc="Enable InSMM.STS"/>
       <field name="BILD" bit="7" size="1" desc="BIOS Interface Lock-Down"/>
@@ -135,13 +153,27 @@
       <field name="UWEWS" bit="4" size="1" desc="Write Enable on Write Status"/>
       <field name="EO_4k" bit="8" size="8" desc="4k Erase Opcode"/>
       <field name="EO_64k" bit="16" size="8" desc="64k Erase Opcode"/>
       <field name="EO_4k_VALID" bit="28" size="1" desc="4k Erase Valid"/>
       <field name="EO_64k_VALID" bit="29" size="1" desc="64k Erase Valid"/>
       <field name="CPPTV" bit="31" size="1" desc="Component Property Parameter Table Valid"/>
     </register>
+    <!-- ME Host Firmware Status https://github.com/coreboot/coreboot/blob/master/src/southbridge/intel/*/{pch,me}.h -->
+    <register name="HFS" type="pcicfg" bus="0" dev="0x18" fun="0" offset="0x40" size="4" desc="ME Host Firmware Status">
+      <field name="MFG_MODE" bit="4" size="1" desc="ME Manufacturing Mode"/>
+      <field name="FW_INIT_COMPLETE" bit="9" size="1" desc="ME Firmware Initialization Complete"/>
+      <field name="UPDATE_IN_PROGRESS" bit="11" size="1" desc="ME Update In Progress"/>
+    </register>
   </registers>
   <controls>
     <control name="FlashLockDown" register="HSFS" field="FLOCKDN" desc="Flash Configuration Lock-Down"/>
     <control name="SpiWriteStatusDis" register="HSFS" field="WRSDIS" desc="Write Status Disable"/>
+    <control name="SmmBiosWriteProtection" register="BC" field="SMM_BWP" desc="SMM BIOS Write Protection"/>
+    <control name="BiosLockEnable" register="BC" field="BLE" desc="BIOS Lock Enable"/>
+    <control name="BiosWriteEnable" register="BC" field="BIOSWE" desc="BIOS Write Enable"/>
+    <control name="TopSwapStatus" register="BC" field="TSS" desc="Top Swap Status"/>
+    <control name="BiosInterfaceLockDown" register="BC" field="BILD" desc="BIOS Interface Lock-Down"/>
+    <control name="GlobalSMIEnable" register="SMI_EN" field="GBL_SMI_EN" desc="Global SMI Enable"/>
+    <control name="TCOSMILock" register="TCO1_CNT" field="TCO_LOCK" desc="TCO SMI Lock"/>
+    <control name="TCOSMIEnable" register="SMI_EN" field="TCO_EN" desc="TCO SMI Enable"/>
   </controls>
 </configuration>
```

### Comparing `chipsec-1.4.4/chipsec/cfg/pch_c61x.xml` & `chipsec-1.5.1/chipsec/cfg/8086/pch_c61x.xml`

 * *Files 22% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/pch_c61x.xml` & `chipsec-1.5.1/chipsec/cfg/8086/pch_c61x.xml`

```diff
@@ -1,14 +1,24 @@
 <?xml version="1.0" encoding="utf-8"?>
-<configuration platform="PCH_C61X">
+<configuration platform="PCH_C61x">
   <!--
 XML configuration file for C610 series PCH
   Intel (c) C610 Series Chipset and Intel (c) X99 Chipset Platform Controller Hub (PCH) datasheet
   https://ark.intel.com/products/series/98915/Intel-C610-Series-Chipsets
 -->
+  <!-- #################################### -->
+  <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info>
+    <sku did="0x8D40" name="C610" code="PCH_C61x" longname="Intel Wellsburg (C610/X99 series) PCH"/>
+    <sku did="0x8D44" name="C610-G" code="PCH_C61x" longname="Intel Wellsburg-G (C610/X99 series) PCH"/>
+    <sku did="0x8D47" name="C610-X" code="PCH_C61x" longname="Intel Wellsburg-X (C610/X99 series) PCH"/>
+  </info>
   <pci>
     <device name="LPC" bus="0" dev="0x1F" fun="0" vid="0x8086" did="0x8D44,0x8D47"/>
   </pci>
   <registers>
     <!-- LPC Interface Bridge -->
     <register name="GEN_PMCON_LOCK" type="pcicfg" device="LPC" offset="0xA6" size="1" desc="General Power Management Configuration Lock">
       <field name="ACPI_BASE_LOCK" bit="1" size="1" desc="Lock down ACPI Base Address (ABASE)"/>
```

### Comparing `chipsec-1.4.4/chipsec/cfg/glk.xml` & `chipsec-1.5.1/chipsec/cfg/8086/glk.xml`

 * *Files 4% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/glk.xml` & `chipsec-1.5.1/chipsec/cfg/8086/glk.xml`

```diff
@@ -1,14 +1,23 @@
 <?xml version="1.0" encoding="utf-8"?>
 <configuration platform="GLK">
   <!-- XML configuration for GLK
   Document ID: 336561-001
 -->
   <!-- #################################### -->
   <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info family="atom">
+    <sku did="0x3180" name="Gemini Lake" code="GLK" longname="Gemini Lake"/>
+    <sku did="0x31F0" name="Gemini Lake" code="GLK" longname="Gemini Lake"/>
+  </info>
+  <!-- #################################### -->
+  <!--                                      -->
   <!-- Integrated devices                   -->
   <!--                                      -->
   <!-- #################################### -->
   <pci>
     <device name="P2SBC" bus="0" dev="0x0D" fun="0" vid="0x8086"/>
     <device name="MEI1" bus="0" dev="0x0F" fun="0" vid="0x8086"/>
     <device name="MEI2" bus="0" dev="0x0F" fun="1" vid="0x8086"/>
@@ -18,26 +27,26 @@
   </pci>
   <!-- #################################### -->
   <!--                                      -->
   <!-- Memory Mapped I/O spaces (MMIO BARs) -->
   <!--                                      -->
   <!-- #################################### -->
   <mmio>
-    <bar name="SPIBAR" bus="0" dev="0xD" fun="0x2" reg="0x10" width="4" mask="0xFFFFFE00" size="0x200" enable_bit="1" desc="SPI Controller Register Range"/>
+    <bar name="SPIBAR" bus="0" dev="0xD" fun="0x2" reg="0x10" width="4" mask="0xFFFFF000" size="0x200" enable_bit="1" desc="SPI Controller Register Range"/>
     <bar name="GTTMMADR" bus="0" dev="0x02" fun="0" reg="0x10" width="8" mask="0x7FF000000" desc="Graphics Translation Table Range"/>
-    <bar name="PWRMBASE" register="PWRMBASE" base_field="BA" size="0x1000" desc="Power Management Register Range"/>
+    <bar name="PWRMBASE" register="PWRMBASE" base_field="BA" size="0x1000" fixed_address="0xFE042000" desc="Power Management Register Range"/>
     <bar name="SBREGBAR" register="SBREG_BAR" base_field="RBA" size="0x1000000" fixed_address="0xFD000000" desc="Sideband Register Access BAR"/>
+    <bar name="TCOBASE" register="TCOBASE" base_field="TCOBA" size="0x20" desc="TCO Base Address"/>
   </mmio>
   <!-- #################################### -->
   <!--                                      -->
   <!-- I/O spaces (I/O BARs)                -->
   <!--                                      -->
   <!-- #################################### -->
   <io>
-    <bar name="TCOBASE" register="TCOBASE" base_field="TCOBA" size="0x20" desc="TCO Base Address"/>
     <bar name="ABASE" register="ABASE" base_field="BA" size="0x100" fixed_address="0x400" desc="ACPI Base Address"/>
     <bar name="PMBASE" register="ABASE" base_field="BA" size="0x100" fixed_address="0x400" desc="ACPI Base Address"/>
     <bar name="SMBUS_BASE" bus="0" dev="0x1F" fun="1" reg="0x20" mask="0xFFE0" size="0x80" desc="SMBus Base Address"/>
   </io>
   <!-- #################################### -->
   <!--                                      -->
   <!-- Configuration registers              -->
@@ -47,45 +56,32 @@
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- PCIe Configuration registers -->
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- Sideband Register Access Registers -->
     <register name="SBREG_BAR" type="pcicfg" bus="0" dev="0xD" fun="0" offset="0x10" size="4" desc="Sideband Register Access BAR">
       <field name="RBA" bit="24" size="8" desc="Register Base Address"/>
     </register>
-    <register name="P2SBC" type="pcicfg" bus="0" dev="0xD" fun="0" offset="0xE0" size="2" desc="P2SB Configuration Register">
+    <register name="P2SBC" type="pcicfg" bus="0" dev="0xD" fun="0" offset="0xE0" size="4" desc="P2SB Configuration Register">
       <field name="HIDE" bit="8" size="1" desc="Hide SBREG_BAR"/>
     </register>
     <register name="P2SB_HIDE" type="pcicfg" bus="0" dev="0xD" fun="0" offset="0xE1" size="1" desc="P2SB Configuration Register hide-unhide">
       <field name="HIDE" bit="0" size="1" desc="Hide SBREG_BAR"/>
     </register>
     <!-- ME Host Firmware Status https://github.com/coreboot/coreboot/blob/master/src/southbridge/intel/*/{pch,me}.h -->
     <register name="HFS" type="pcicfg" bus="0" dev="0x0F" fun="0" offset="0x40" size="4" desc="ME Host Firmware Status">
       <field name="MFG_MODE" bit="4" size="1" desc="ME Manufacturing Mode"/>
       <field name="FW_INIT_COMPLETE" bit="9" size="1" desc="ME Firmware Initialization Complete"/>
       <field name="UPDATE_IN_PROGRESS" bit="11" size="1" desc="ME Update In Progress"/>
     </register>
-    <!-- GFx PCI device registers -->
-    <register name="PCI0.0.0_GGC" type="pcicfg" bus="0" dev="0" fun="0" offset="0x50" size="4" desc="GMCH Graphics Control">
-      <field name="GGCLCK" bit="0" size="1"/>
-    </register>
-    <register name="PCI0.0.0_BDSM" type="pcicfg" bus="0" dev="0" fun="0" offset="0xB0" size="4" desc="Base of Data Stolen Memory">
-      <field name="BDSM_LOCK" bit="0" size="1"/>
-    </register>
-    <register name="PCI0.0.0_BGSM" type="pcicfg" bus="0" dev="0" fun="0" offset="0xB4" size="4" desc="Base of Graphics Stolen Memory">
-      <field name="BGSM_LOCK" bit="0" size="1"/>
-    </register>
-    <register name="PCI0.0.0_PAVPC" type="pcicfg" bus="0" dev="0" fun="0" offset="0x58" size="4" desc="PAVP Control">
-      <field name="PAVPC_LOCK" bit="2" size="1"/>
-    </register>
     <register name="PWRMBASE" type="pcicfg" bus="0" dev="0x0D" fun="1" offset="0x10" size="8" desc="PM Base Address">
-      <field name="STYPE" bit="2" size="1" desc="Space Type (if 0 - 32bit, 1 - 64bit)"/>
+      <field name="STYPE" bit="1" size="2" desc="Space Type (if 0 - 32bit, 10 - 64bit)"/>
       <field name="BA" bit="12" size="52" desc="Base Address"/>
     </register>
-    <register name="ABASE" type="pcicfg" bus="0" dev="0x0D" fun="1" offset="0x20" size="2" desc="ACPI Base Address">
-      <field name="BA" bit="8" size="8" desc="Base Address"/>
+    <register name="ABASE" type="pcicfg" bus="0" dev="0x0D" fun="1" offset="0x20" size="4" desc="ACPI Base Address">
+      <field name="BA" bit="2" size="30" desc="Base Address"/>
     </register>
     <register name="RC" type="mm_msgbus" port="0xC3" offset="0x3400" size="4" desc="RTC Configuration">
       <field name="UE" bit="2" size="1" desc="Upper 128 Byte Enable"/>
       <field name="LL" bit="3" size="1" desc="Lower 128 Byte Lock"/>
       <field name="UL" bit="4" size="1" desc="Upper 128 Byte Lock"/>
       <field name="BILD" bit="31" size="1" desc="BIOS Interface Lock-Down"/>
     </register>
@@ -100,15 +96,14 @@
       <field name="HST_EN" bit="0" size="1"/>
       <field name="SMB_SMI_EN" bit="1" size="1"/>
       <field name="I2C_EN" bit="2" size="2"/>
       <field name="SSRESET" bit="3" size="1"/>
       <field name="SPD_WD" bit="4" size="1"/>
     </register>
     <register name="TCOBASE" type="pcicfg" bus="0" dev="0x1f" fun="1" offset="0x50" size="4" desc="TCO Base Address">
-      <field name="IOS" bit="0" size="1" desc="I/O space"/>
       <field name="TCOBA" bit="5" size="11" desc="TCO Base Address"/>
     </register>
     <register name="TCOCTL" type="pcicfg" bus="0" dev="0x1f" fun="1" offset="0x54" size="4" desc="TCO Control">
       <field name="TCO_BASE_EN" bit="8" size="1" desc="TCO Base Enable"/>
     </register>
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- MMIO registers               -->
@@ -276,22 +271,30 @@
       <field name="EOS" bit="1" size="1"/>
       <field name="BIOS_EN" bit="2" size="1"/>
       <field name="LEGACY_USB_EN" bit="3" size="1"/>
       <field name="SLP_SMI_EN" bit="4" size="1"/>
       <field name="APMC_EN" bit="5" size="1"/>
       <field name="SWSMI_TMR_EN" bit="6" size="1"/>
       <field name="BIOS_RLS" bit="7" size="1"/>
-      <field name="MCSMI_EN" bit="11" size="1"/>
+      <field name="GPIO_UNLOCK_SMI_EN" bit="10" size="1"/>
+      <field name="GPIO_UNLOCK_SSMI_EN" bit="11" size="1"/>
+      <field name="MCSMI_EN" bit="12" size="1"/>
       <field name="TCO_EN" bit="13" size="1"/>
       <field name="PERIODIC_EN" bit="14" size="1"/>
-      <field name="LEGACY_USB2_EN" bit="17" size="1"/>
-      <field name="INTEL_USB2_EN" bit="18" size="1"/>
-      <field name="GPIO_UNLOCK_SMI_EN" bit="27" size="1"/>
-      <field name="ME_SMI_EN" bit="30" size="1"/>
-      <field name="xHCI_SMI_EN" bit="31" size="1"/>
+      <field name="SERIRQ_SMI_EN" bit="15" size="1"/>
+      <field name="SMBUS_SMI_EN" bit="16" size="1"/>
+      <field name="xHCI_SMI_EN" bit="17" size="1"/>
+      <field name="HOST_SMBUS_SMI_EN" bit="18" size="1"/>
+      <field name="SCS_SMI_EN" bit="19" size="1"/>
+      <field name="PCIE_SMI_EN" bit="20" size="1"/>
+      <field name="SCC2_SMI_EN" bit="21" size="1"/>
+      <field name="SPI_SMI_EN" bit="26" size="1"/>
+      <field name="OCP_SMI_EN" bit="27" size="1"/>
+      <field name="ESPI_SMI_EN" bit="28" size="1"/>
+      <field name="CSE_SMI_EN" bit="29" size="1"/>
     </register>
   </registers>
   <!-- #################################### -->
   <!--                                      -->
   <!-- 'Controls'                           -->
   <!--                                      -->
   <!-- #################################### -->
```

### Comparing `chipsec-1.4.4/chipsec/cfg/pch_1xx.xml` & `chipsec-1.5.1/chipsec/cfg/8086/pch_495.xml`

 * *Files 5% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/pch_1xx.xml` & `chipsec-1.5.1/chipsec/cfg/8086/pch_495.xml`

```diff
@@ -1,22 +1,31 @@
 <?xml version="1.0" encoding="utf-8"?>
-<configuration platform="PCH_1xx">
+<configuration platform="PCH_495">
   <!--
-XML configuration file for 100 series PCH based platforms
-
-* Intel(R) 100 Series Chipset Family Platform Controller Hub (PCH)
-  http://www.intel.com/content/www/us/en/processors/core/core-technical-resources.html
+XML configuration file for the 495 series PCH
 -->
   <!-- #################################### -->
   <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info>
+    <sku did="0x3481" name="PCH-LP-U" code="PCH_495" longname="Intel 495 series PCH-LP U"/>
+    <sku did="0x3482" name="PCH-LP-UPrem" code="PCH_495" longname="Intel 495 series PCH-LP Prem-U"/>
+    <sku did="0x3486" name="PCH-LP-Y" code="PCH_495" longname="Intel 495 series PCH-LP Y"/>
+    <sku did="0x3487" name="PCH-LP-YPrem" code="PCH_495" longname="Intel 495 series PCH-LP Prem-Y"/>
+  </info>
+  <!-- #################################### -->
+  <!--                                      -->
   <!-- Integrated devices                   -->
   <!--                                      -->
   <!-- #################################### -->
   <pci>
     <device name="P2SBC" bus="0" dev="0x1F" fun="1" vid="0x8086"/>
+    <device name="PMC" bus="0" dev="0x1F" fun="2" vid="0x8086"/>
     <device name="SMBUS" bus="0" dev="0x1F" fun="4" vid="0x8086"/>
     <device name="SPI" bus="0" dev="0x1F" fun="5" vid="0x8086"/>
   </pci>
   <!-- #################################### -->
   <!--                                      -->
   <!-- Memory Mapped I/O spaces (MMIO BARs) -->
   <!--                                      -->
@@ -37,82 +46,97 @@
     <bar name="PMBASE" register="ABASE" base_field="BA" size="0x100" fixed_address="0x1800" desc="ACPI Base Address"/>
     <bar name="TCOBASE" register="TCOBASE" base_field="TCOBA" size="0x20" desc="TCO Base Address"/>
     <!-- old definition -->
     <bar name="SMBUS_BASE" bus="0" dev="0x1F" fun="4" reg="0x20" mask="0xFFE0" size="0x80" desc="SMBus Base Address"/>
   </io>
   <!-- #################################### -->
   <!--                                      -->
+  <!-- Memory ranges                        -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <memory/>
+  <!-- #################################### -->
+  <!--                                      -->
   <!-- Configuration registers              -->
   <!--                                      -->
   <!-- #################################### -->
   <registers>
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- PCIe Configuration registers -->
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- Sideband Register Access Registers -->
-    <register name="SBREG_BAR" type="pcicfg" bus="0" dev="0x1F" fun="1" offset="0x10" size="4" desc="Sideband Register Access BAR">
+    <register name="SBREG_BAR" type="pcicfg" device="P2SBC" offset="0x10" size="4" desc="Sideband Register Access BAR">
       <field name="RBA" bit="24" size="8" desc="Register Base Address"/>
     </register>
-    <register name="P2SBC" type="pcicfg" bus="0" dev="0x1F" fun="1" offset="0xE0" size="2" desc="P2SB Configuration Register">
+    <register name="P2SBC" type="pcicfg" device="P2SBC" offset="0xE0" size="2" desc="P2SB Configuration Register">
       <field name="HIDE" bit="8" size="1" desc="Hide SBREG_BAR"/>
     </register>
-    <register name="P2SB_HIDE" type="pcicfg" bus="0" dev="0x1F" fun="1" offset="0xE1" size="1" desc="P2SB Configuration Register hide-unhide">
+    <register name="P2SB_HIDE" type="pcicfg" device="P2SBC" offset="0xE1" size="1" desc="P2SB Configuration Register hide-unhide">
       <field name="HIDE" bit="0" size="1" desc="Hide SBREG_BAR"/>
     </register>
     <!-- Power Management Controller -->
-    <register name="ABASE" type="pcicfg" bus="0" dev="0x1f" fun="2" offset="0x40" size="4" desc="ACPI Base Address">
+    <register name="PWRMBASE" type="pcicfg" device="PMC" offset="0x10" size="4" desc="PM Base Address">
+      <field name="STYPE" bit="0" size="1" desc="Space Type (always 0 - memory space)"/>
+      <field name="BA" bit="13" size="19" desc="Base Address"/>
+    </register>
+    <register name="ABASE" type="pcicfg" device="PMC" offset="0x20" size="4" desc="ACPI Base Address">
       <field name="STYPE" bit="0" size="1" desc="Space Type (always 1 - I/O space)"/>
-      <field name="BA" bit="8" size="8" desc="Base Address"/>
+      <field name="BA" bit="7" size="25" desc="Base Address"/>
+    </register>
+    <register name="GEN_PMCON_1" type="mmio" bar="PWRMBASE" offset="0x1020" size="4" desc="General PM Configuration A">
+      <field name="ESPI_SMI_LOCK" bit="8" size="1" desc="ESPI_SMI_LOCK"/>
     </register>
-    <register name="ACTL" type="pcicfg" bus="0" dev="0x1f" fun="2" offset="0x44" size="4" desc="ACPI Control">
+    <register name="GEN_PMCON_2" type="mmio" bar="PWRMBASE" offset="0x1024" size="4" desc="General PM Configuration B">
+      <field name="SMI_LOCK" bit="4" size="1"/>
+    </register>
+    <register name="PM_CFG" type="mmio" bar="PWRMBASE" offset="0x1818" size="4" desc="Power Management Configuration Reg 1"/>
+    <register name="ACTL" type="mmio" bar="PWRMBASE" offset="0x1BD8" size="4" desc="ACPI Control">
       <field name="SCIS" bit="0" size="2" desc="SCI IRQ Select"/>
       <field name="EN" bit="7" size="1" desc="ACPI Enable"/>
       <field name="PWRM_EN" bit="8" size="1" desc="PWRM Enable"/>
     </register>
-    <register name="PWRMBASE" type="pcicfg" bus="0" dev="0x1f" fun="2" offset="0x48" size="4" desc="PM Base Address">
-      <field name="STYPE" bit="0" size="1" desc="Space Type (always 0 - memory space)"/>
-      <field name="BA" bit="12" size="20" desc="Base Address"/>
-    </register>
-    <register name="GEN_PMCON_1" type="pcicfg" bus="0" dev="0x1f" fun="2" offset="0xA0" size="2" desc="General PM Configuration A">
-      <field name="SMI_LOCK" bit="4" size="1"/>
-    </register>
     <!-- SMBus Host Controller -->
-    <register name="SMBUS_VID" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x00" size="2" desc="VID"/>
-    <register name="SMBUS_DID" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x02" size="2" desc="DID"/>
-    <register name="SMBUS_CMD" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x04" size="2" desc="CMD"/>
-    <register name="SMBUS_HCFG" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x40" size="1" desc="Host Configuration">
+    <register name="SMBUS_VID" type="pcicfg" device="SMBUS" offset="0x00" size="2" desc="VID"/>
+    <register name="SMBUS_DID" type="pcicfg" device="SMBUS" offset="0x02" size="2" desc="DID"/>
+    <register name="SMBUS_CMD" type="pcicfg" device="SMBUS" offset="0x04" size="2" desc="CMD"/>
+    <register name="SMBUS_HCFG" type="pcicfg" device="SMBUS" offset="0x40" size="1" desc="Host Configuration">
       <field name="HST_EN" bit="0" size="1"/>
       <field name="SMB_SMI_EN" bit="1" size="1"/>
-      <field name="I2C_EN" bit="2" size="2"/>
+      <field name="I2C_EN" bit="2" size="1"/>
       <field name="SSRESET" bit="3" size="1"/>
       <field name="SPD_WD" bit="4" size="1"/>
     </register>
-    <register name="TCOBASE" type="pcicfg" bus="0" dev="0x1f" fun="4" offset="0x50" size="4" desc="TCO Base Address">
+    <register name="TCOBASE" type="pcicfg" device="SMBUS" offset="0x50" size="4" desc="TCO Base Address">
       <field name="IOS" bit="0" size="1" desc="I/O space"/>
       <field name="TCOBA" bit="5" size="11" desc="TCO Base Address"/>
     </register>
-    <register name="TCOCTL" type="pcicfg" bus="0" dev="0x1f" fun="4" offset="0x54" size="4" desc="TCO Control">
+    <register name="TCOCTL" type="pcicfg" device="SMBUS" offset="0x54" size="4" desc="TCO Control">
       <field name="TCO_BASE_LOCK" bit="0" size="1" desc="TCO Base Lock"/>
       <field name="TCO_BASE_EN" bit="8" size="1" desc="TCO Base Enable"/>
     </register>
     <!-- SPI Interface Controller -->
-    <register name="BC" type="pcicfg" bus="0" dev="0x1F" fun="5" offset="0xDC" size="4" desc="BIOS Control">
+    <register name="BC" type="pcicfg" device="SPI" offset="0xDC" size="4" desc="BIOS Control">
       <field name="BIOSWE" bit="0" size="1" desc="BIOS Write Enable"/>
       <field name="BLE" bit="1" size="1" desc="BIOS Lock Enable"/>
       <field name="SRC" bit="2" size="2" desc="SPI Read Configuration"/>
       <field name="TSS" bit="4" size="1" desc="Top Swap Status"/>
       <field name="SMM_BWP" bit="5" size="1" desc="SMM BIOS Write Protection"/>
       <field name="BBS" bit="6" size="1" desc="Boot BIOS Strap"/>
       <field name="BILD" bit="7" size="1" desc="BIOS Interface Lock Down"/>
+      <field name="ASE_BWP" bit="11" size="1" desc="Async SMI Enable for BIOS Write Protection"/>
     </register>
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- MMIO registers               -->
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- PCH SPIBAR registers -->
-    <register name="HSFS" type="mmio" bar="SPIBAR" offset="0x04" size="4" desc="Hardware Sequencing Flash Status Register">
+    <register name="BFPR" type="mmio" bar="SPIBAR" offset="0x00" size="4" desc="BIOS Flash Primary Region Register (= FREG1)">
+      <field name="PRB" bit="0" size="15" desc="BIOS Flash Primary Region Base"/>
+      <field name="PRL" bit="16" size="15" desc="BIOS Flash Primary Region Limit"/>
+    </register>
+    <register name="HSFS" type="mmio" bar="SPIBAR" offset="0x4" size="4" desc="Hardware Sequencing Flash Status Register">
       <field name="FDONE" bit="0" size="1" desc="Flash Cycle Done"/>
       <field name="FCERR" bit="1" size="1" desc="Flash Cycle Error"/>
       <field name="AEL" bit="2" size="1" desc="Access Error Log"/>
       <field name="SCIP" bit="5" size="1" desc="SPI cycle in progress"/>
       <field name="WRSDIS" bit="11" size="1" desc="Write status disable"/>
       <field name="PR34LKD" bit="12" size="1" desc="PRR3 PRR4 Lock-Down"/>
       <field name="FDOPSS" bit="13" size="1" desc="Flash Descriptor Override Pin-Strap Status"/>
@@ -120,21 +144,14 @@
       <field name="FLOCKDN" bit="15" size="1" desc="Flash Configuration Lock-Down"/>
       <field name="FGO" bit="16" size="1" desc="Flash cycle go"/>
       <field name="FCYCLE" bit="17" size="4" desc="Flash Cycle Type"/>
       <field name="WET" bit="21" size="1" desc="Write Enable Type"/>
       <field name="FDBC" bit="24" size="6" desc="Flash Data Byte Count"/>
       <field name="FSMIE" bit="31" size="1" desc="Flash SPI SMI# Enable"/>
     </register>
-    <register name="HSFC" type="mmio" bar="SPIBAR" offset="0x06" size="2" desc="Hardware Sequencing Flash Control Register">
-      <field name="FGO" bit="0" size="1" desc="Flash Cycle GO"/>
-      <field name="FCYCLE" bit="1" size="4" desc="Flash Cycle"/>
-      <field name="WET" bit="5" size="1" desc="Write Enable Type"/>
-      <field name="FDBC" bit="8" size="6" desc="Flash Data Byte Count, Count = FDBC + 1"/>
-      <field name="FSMIE" bit="15" size="1" desc="Flash SPI SMI Enable"/>
-    </register>
     <register name="FREG0_FLASHD" type="mmio" bar="SPIBAR" offset="0x54" size="4" desc="Flash Region 0 (Flash Descriptor)">
       <field name="RB" bit="0" size="15" desc="Region Base"/>
       <field name="RL" bit="16" size="15" desc="Region Limit"/>
     </register>
     <register name="FREG1_BIOS" type="mmio" bar="SPIBAR" offset="0x58" size="4" desc="Flash Region 1 (BIOS)">
       <field name="RB" bit="0" size="15" desc="Region Base"/>
       <field name="RL" bit="16" size="15" desc="Region Limit"/>
@@ -151,41 +168,40 @@
       <field name="RB" bit="0" size="15" desc="Region Base"/>
       <field name="RL" bit="16" size="15" desc="Region Limit"/>
     </register>
     <register name="FREG5" type="mmio" bar="SPIBAR" offset="0x68" size="4" desc="Flash Region 5">
       <field name="RB" bit="0" size="15" desc="Region Base"/>
       <field name="RL" bit="16" size="15" desc="Region Limit"/>
     </register>
-    <register name="FREG6" undef="Flash Region 6 not defined for this platform"/>
     <register name="PR0" type="mmio" bar="SPIBAR" offset="0x84" size="4" desc="Protected Range 0">
-      <field name="PRB" bit="0" size="13"/>
+      <field name="PRB" bit="0" size="15"/>
       <field name="RPE" bit="15" size="1"/>
       <field name="PRL" bit="16" size="15"/>
       <field name="WPE" bit="31" size="1"/>
     </register>
     <register name="PR1" type="mmio" bar="SPIBAR" offset="0x88" size="4" desc="Protected Range 1">
-      <field name="PRB" bit="0" size="13"/>
+      <field name="PRB" bit="0" size="15"/>
       <field name="RPE" bit="15" size="1"/>
       <field name="PRL" bit="16" size="15"/>
       <field name="WPE" bit="31" size="1"/>
     </register>
     <register name="PR2" type="mmio" bar="SPIBAR" offset="0x8C" size="4" desc="Protected Range 2">
-      <field name="PRB" bit="0" size="13"/>
+      <field name="PRB" bit="0" size="15"/>
       <field name="RPE" bit="15" size="1"/>
       <field name="PRL" bit="16" size="15"/>
       <field name="WPE" bit="31" size="1"/>
     </register>
     <register name="PR3" type="mmio" bar="SPIBAR" offset="0x90" size="4" desc="Protected Range 3">
-      <field name="PRB" bit="0" size="13"/>
+      <field name="PRB" bit="0" size="15"/>
       <field name="RPE" bit="15" size="1"/>
       <field name="PRL" bit="16" size="15"/>
       <field name="WPE" bit="31" size="1"/>
     </register>
     <register name="PR4" type="mmio" bar="SPIBAR" offset="0x94" size="4" desc="Protected Range 4">
-      <field name="PRB" bit="0" size="13"/>
+      <field name="PRB" bit="0" size="15"/>
       <field name="RPE" bit="15" size="1"/>
       <field name="PRL" bit="16" size="15"/>
       <field name="WPE" bit="31" size="1"/>
     </register>
     <register name="FDOC" type="mmio" bar="SPIBAR" offset="0xB4" size="4" desc="Flash Descriptor Observability Control Register">
       <field name="FDSI" bit="2" size="10" desc="Flash Descriptor Section Index"/>
       <field name="FDSS" bit="12" size="3" desc="Flash Descriptor Section Select"/>
@@ -230,75 +246,36 @@
       <field name="LL" bit="3" size="1" desc="Lower 128 Byte Lock"/>
       <field name="UL" bit="4" size="1" desc="Upper 128 Byte Lock"/>
       <field name="BILD" bit="31" size="1" desc="BIOS Interface Lock-Down"/>
     </register>
     <register name="BUC" type="mm_msgbus" port="0xC3" offset="0x3414" size="4" desc="Backed Up Control">
       <field name="TS" bit="0" size="1" desc="Top Swap"/>
     </register>
-    <!-- PMC MMIO registers (6th Generation Intel(R) Processor I/O Datasheet for U/Y-Platforms, Vol. 2, section 4.3) -->
-    <register name="PM_CFG" type="mmio" bar="PWRMBASE" offset="0x18" size="4" desc="Power Management Configuration Reg 1"/>
-    <!-- SPI Flash Descriptor registers -->
-    <register name="FLMAP0" type="mmio" bar="FDBAR" offset="0x14" size="4" desc="Flash Map 0 Register">
-      <field name="FCBA" bit="0" size="8" desc="Flash Component Base Address"/>
-      <field name="NC" bit="8" size="2" desc="Number of Components"/>
-      <field name="FRBA" bit="16" size="8" desc="Flash Region Base Address"/>
-    </register>
-    <register name="FLMAP1" type="mmio" bar="FDBAR" offset="0x18" size="4" desc="Flash Map 1 Register">
-      <field name="FMBA" bit="0" size="8" desc="Flash Master Base Address"/>
-      <field name="NM" bit="8" size="3" desc="Number of Masters"/>
-      <field name="FPSBA" bit="16" size="8" desc="Flash PCH Strap Base Address"/>
-      <field name="PSL" bit="24" size="8" desc="PCH Strap Length"/>
-    </register>
-    <register name="FLMAP2" type="mmio" bar="FDBAR" offset="0x1C" size="4" desc="Flash Map 2 Register">
-      <field name="FCPUSBA" bit="0" size="8" desc="Flash CPU Strap Base Address"/>
-      <field name="CPUSL" bit="8" size="8" desc="CPU Strap Length"/>
-    </register>
-    <register name="FLREG0" type="mmio" bar="FRBA" offset="0x0" size="4" desc="Flash Region 0 (Flash Descriptor) Register">
-      <field name="RB" bit="0" size="15" desc="Region Base"/>
-      <field name="RL" bit="16" size="15" desc="Region Limit"/>
-    </register>
-    <register name="FLREG1" type="mmio" bar="FRBA" offset="0x4" size="4" desc="Flash Region 1 (BIOS) Register">
-      <field name="RB" bit="0" size="15" desc="Region Base"/>
-      <field name="RL" bit="16" size="15" desc="Region Limit"/>
-    </register>
-    <register name="FLREG2" type="mmio" bar="FRBA" offset="0x8" size="4" desc="Flash Region 2 (Intel ME) Register">
-      <field name="RB" bit="0" size="15" desc="Region Base"/>
-      <field name="RL" bit="16" size="15" desc="Region Limit"/>
-    </register>
-    <register name="FLREG3" type="mmio" bar="FRBA" offset="0xC" size="4" desc="Flash Region 3 (GBe) Register">
-      <field name="RB" bit="0" size="15" desc="Region Base"/>
-      <field name="RL" bit="16" size="15" desc="Region Limit"/>
-    </register>
-    <register name="FLREG4" type="mmio" bar="FRBA" offset="0x10" size="4" desc="Flash Region 4 (Platform Data) Register">
-      <field name="RB" bit="0" size="15" desc="Region Base"/>
-      <field name="RL" bit="16" size="15" desc="Region Limit"/>
-    </register>
-    <register name="FLREG8" type="mmio" bar="FRBA" offset="0x20" size="4" desc="Flash Region 8 (Embedded Controller) Register">
-      <field name="RB" bit="0" size="15" desc="Region Base"/>
-      <field name="RL" bit="16" size="15" desc="Region Limit"/>
-    </register>
-    <register name="FLMSTR1" type="mmio" bar="FMBA" offset="0x0" size="4" desc="Flash Master 1">
-      <field name="MRRA" bit="8" size="12" desc="Master Region Read Access"/>
-      <field name="MRWA" bit="20" size="12" desc="Master Region Write Access"/>
-    </register>
     <!-- DCI registers -->
     <register name="ECTRL" type="mm_msgbus" port="0xB8" offset="0x0004" size="4" desc="DCI Control Register">
+      <field name="LOCK" bit="0" size="1"/>
       <field name="ENABLE" bit="4" size="1"/>
     </register>
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- I/O registers (I/O ports)    -->
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- PCH TCOBASE (SMBus TCO) I/O registers -->
     <register name="TCO1_CNT" type="iobar" bar="TCOBASE" offset="0x8" size="2" desc="TCO1 Control">
       <field name="TCO_LOCK" bit="12" size="1" desc="TCO Lock"/>
     </register>
+    <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
+    <!--      Undefined Registers     -->
+    <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
+    <register name="GC" undef="Not defined for platform"/>
   </registers>
   <!-- #################################### -->
   <!--                                      -->
   <!-- 'Controls'                           -->
   <!--                                      -->
   <!-- #################################### -->
   <controls>
     <control name="BiosInterfaceLockDown" register="BC" field="BILD" desc="BIOS Interface Lock-Down"/>
+    <control name="TopSwap" register="BC" field="TSS" desc="Top Swap Status"/>
     <control name="SpiWriteStatusDis" register="HSFS" field="WRSDIS" desc="Write Status Disable"/>
+    <control name="SMILock" register="GEN_PMCON_2" field="SMI_LOCK" desc="SMI Global Configuration Lock"/>
   </controls>
 </configuration>
```

### Comparing `chipsec-1.4.4/chipsec/cfg/hsx.xml` & `chipsec-1.5.1/chipsec/cfg/8086/hsx.xml`

 * *Files 2% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/hsx.xml` & `chipsec-1.5.1/chipsec/cfg/8086/hsx.xml`

```diff
@@ -4,14 +4,22 @@
 XML configuration file for Haswell Server based platforms
 Intel (c) Xeon Processor E5-1600/2400/2600/4600 v3 Product Family datasheet Vol. 2
 Intel (c) Xeon Processor E7-8800/4800 v3 Product Family datasheet Vol. 2
 Intel (c) C600 Series Chipset and Intel (c) X79 Express Chipset datasheet
 Intel (c) C600 Series Chipset and Intel (c) X79 Express Chipset Specification Update
 Intel (c) C610 Series Chipset and Intel (c) X99 Chipset Platform Controller Hub (PCH) datasheet
 -->
+  <!-- #################################### -->
+  <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info family="xeon">
+    <sku did="0x2F00" name="Haswell Server" code="HSX" longname="Server 4th Generation Core Processor (Haswell Server CPU / Wellsburg PCH)"/>
+  </info>
   <pci>
     <device name="VTD_MEM_SM" bus="0" dev="0x5" fun="0" vid="0x8086" did="0x2F28"/>
     <device name="LPC" bus="0" dev="0x1F" fun="0" vid="0x8086" did="0x8D44,0x8D47,0x1D41"/>
     <device name="IMC0_MAIN_SMBUS" bus="0x17" dev="0x13" fun="0" vid="0x8086" did="0x2FA8"/>
     <device name="IMC1_MAIN_SMBUS" bus="0x17" dev="0x16" fun="0" vid="0x8086" did="0x2F68"/>
   </pci>
   <mmio>
```

### Comparing `chipsec-1.4.4/chipsec/cfg/bdx.xml` & `chipsec-1.5.1/chipsec/cfg/8086/cht.xml`

 * *Files 20% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/bdx.xml` & `chipsec-1.5.1/chipsec/cfg/8086/cht.xml`

```diff
@@ -1,181 +1,228 @@
 <?xml version="1.0" encoding="utf-8"?>
-<configuration platform="BDX">
+<configuration platform="CHT">
   <!--
-XML configuration file for Broadwell Server based platforms
-Intel (c) Xeon Processor E5 v4 Product Family datasheet Vol. 2
-Intel (c) Xeon Processor E7 v4 Product Family datasheet Vol. 2
-Intel (c) C600 Series Chipset and Intel (c) X79 Express Chipset datasheet
-Intel (c) C600 Series Chipset and Intel (c) X79 Express Chipset Specification Update
-Intel (c) C610 Series Chipset and Intel (c) X99 Chipset Platform Controller Hub (PCH) datasheet
+XML configuration for Cherry Trail and Braswell SoCs
+
+* Intel(R) Atom(TM) Processor Z8000 series datasheet
+  http://www.intel.com/content/www/us/en/processors/atom/atom-z8000-datasheet-vol-2.html
+
+* N-series Intel(R) Pentium(R) and Celeron(R) Processors Datasheet
+  http://www.intel.com/content/dam/www/public/us/en/documents/datasheets/pentium-celeron-n-series-datasheet-vol-2.pdf
 -->
-  <pci>
-    <device name="VTD_MEM_SM" bus="0" dev="0x5" fun="0" vid="0x8086" did="0x2F28"/>
-    <device name="LPC" bus="0" dev="0x1F" fun="0" vid="0x8086" did="0x8D44,0x8D47,0x1D41"/>
-    <device name="IMC0_MAIN_SMBUS" bus="0x17" dev="0x13" fun="0" vid="0x8086" did="0x2FA8"/>
-    <device name="IMC1_MAIN_SMBUS" bus="0x17" dev="0x16" fun="0" vid="0x8086" did="0x2F68"/>
-  </pci>
+  <!-- #################################### -->
+  <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info family="atom">
+    <sku did="0x2280" name="Braswell/Cherry Trail" code="CHT" longname="Braswell/Cherry Trail SoC"/>
+  </info>
+  <!-- #################################### -->
+  <!--                                      -->
+  <!-- Memory Mapped I/O spaces (MMIO BARs) -->
+  <!--                                      -->
+  <!-- #################################### -->
   <mmio>
-    <bar name="MMCFG" bus="0" dev="5" fun="0" reg="0x90" width="8" mask="0x7FFFFFC000000" size="0x1000" desc="PCI Express Register Range"/>
-    <bar name="DMIBAR" bus="0" dev="0" fun="0" reg="0x50" width="4" mask="0xFFFFF000" size="0x1000" enable_bit="0" desc="Root Complex Register Range"/>
+    <!-- Section 4.1.7-8 -->
+    <bar name="GTTMMADR" bus="0" dev="0x02" fun="0" reg="0x10" width="8" mask="0xFFFFFFF0FFC00000" desc="Graphics Translation Table Range"/>
+    <!-- Section 35.6 -->
+    <bar name="PMBASE" register="PBASE" base_field="Base" size="0x200" enable_field="Enable" desc="PM Base"/>
+    <bar name="IOBASE" register="IOBASE" base_field="Base" size="0x2000" enable_field="Enable" desc="I/O Controller Base"/>
+    <bar name="IBASE" register="IBASE" base_field="Base" size="0x200" enable_field="Enable" desc="iLB Base"/>
+    <bar name="MPBASE" register="MPBASE" base_field="Base" size="0x100000" enable_field="Enable" desc="MPHY Base"/>
+    <bar name="PUBASE" register="PUBASE" base_field="Base" size="0x800" enable_field="Enable" desc="PUnit Base"/>
+    <bar name="SPIBAR" register="SBASE" base_field="Base" size="0x200" enable_field="Enable" desc="SPI Base"/>
+    <bar name="MMCFG" register="BECREG" base_field="ECBASE" size="0x10000000" enable_bit="ECENABLE" desc="PCI Express Register Range"/>
   </mmio>
-  <io/>
-  <memory/>
+  <!-- #################################### -->
+  <!--                                      -->
+  <!-- I/O spaces (I/O BARs)                -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <io>
+    <!-- Section 10.20 -->
+    <bar name="ABASE" register="ABASE" base_field="Base" size="0x1000" enable_field="Enable" desc="ACPI Base Address"/>
+    <bar name="GBASE" register="GBASE" base_field="Base" size="0x100" enable_field="Enable" desc="GPIO Base Address"/>
+  </io>
+  <!-- #################################### -->
+  <!--                                      -->
+  <!-- Configuration registers              -->
+  <!--                                      -->
+  <!-- #################################### -->
   <registers>
-    <!-- Host Controller -->
-    <register name="DMIRCBAR" type="pcicfg" bus="0" dev="0" fun="0" offset="0x50" size="4" desc="DMI Root Complex Register Block Base Address">
-      <field name="dmircbaren" bit="0" size="1" desc="Enable DMIRCBAR"/>
-      <field name="dmircbar" bit="12" size="20" desc="Base address DMI Root Complex register space"/>
-    </register>
-    <register name="TSEG" type="pcicfg" device="VTD_MEM_SM" offset="0xA8" size="8" desc="TSEG Memory">
-      <field name="base" bit="20" size="12" desc="Base address"/>
-      <field name="limit" bit="52" size="12" desc="Limit address"/>
-    </register>
-    <register name="TSEG_BASE" type="pcicfg" device="VTD_MEM_SM" offset="0xA8" size="4" desc="TSEG Memory Base">
-      <field name="base" bit="20" size="12" desc="Base address"/>
-    </register>
-    <register name="TSEG_LIMIT" type="pcicfg" device="VTD_MEM_SM" offset="0xAC" size="4" desc="TSEG Memory Limit">
-      <field name="limit" bit="20" size="12" desc="Limit address"/>
-    </register>
-    <register name="VTBAR" type="mmcfg" device="VTD_MEM_SM" offset="0x180" size="4" desc="VT BAR Register">
-      <field name="Enable" bit="0" size="1" desc="Enable"/>
-      <field name="Base" bit="13" size="19" desc="VTD Base Address"/>
-    </register>
-    <register name="VTGENCTRL" type="mmcfg" device="VTD_MEM_SM" offset="0x184" size="4" desc="VTGENCTRL Register">
-      <field name="gpa_limit" bit="0" size="4" desc="Guest virtual addressing limit"/>
-      <field name="hpa_limit" bit="4" size="4" desc="Host processor addressing limit"/>
-      <field name="lockvtd" bit="15" size="1" desc="lockvtd"/>
-    </register>
-    <register name="LTDPR" type="mmcfg" device="VTD_MEM_SM" offset="0x290" size="4" desc="Intel TXT DMA Protected Range Register">
-      <field name="lock" bit="0" size="1" desc="Lock LTDPR register"/>
-      <field name="protregsts" bit="1" size="1" desc="Protection enabled in HW"/>
-      <field name="commandbit" bit="2" size="1" desc="Command bit"/>
-      <field name="size" bit="4" size="8" desc="Size of memory"/>
-      <field name="topofdpr" bit="20" size="12" desc="Top address +1 of DPR"/>
-    </register>
-    <!-- GENPROTRANGE Registers -->
-    <register name="GENPROTRANGE1_BASE" type="pcicfg" device="VTD_MEM_SM" offset="0xB0" size="8" desc="Generic Protected Memory Range 1 Base Address">
-      <field name="base_address" bit="16" size="35" desc="GENPROTRANGE 1 base address"/>
-    </register>
-    <register name="GENPROTRANGE1_LIMIT" type="pcicfg" device="VTD_MEM_SM" offset="0xB8" size="8" desc="Generic Protected Memory Range 1 Limit Address">
-      <field name="limit_address" bit="16" size="35" desc="GENPROTRANGE 1 limit address"/>
-    </register>
-    <register name="GENPROTRANGE2_BASE" type="pcicfg" device="VTD_MEM_SM" offset="0xC0" size="8" desc="Generic Protected Memory Range 2 Base Address">
-      <field name="base_address" bit="16" size="35" desc="GENPROTRANGE 2 base address"/>
-    </register>
-    <register name="GENPROTRANGE2_LIMIT" type="pcicfg" device="VTD_MEM_SM" offset="0xC8" size="8" desc="Generic Protected Memory Range 2 Limit Address">
-      <field name="limit_address" bit="16" size="35" desc="GENPROTRANGE 2 limit address"/>
-    </register>
-    <register name="GENPROTRANGE0_BASE" type="mmcfg" device="VTD_MEM_SM" offset="0x120" size="8" desc="Generic Protected Memory Range 0 Base Address">
-      <field name="base_address" bit="16" size="35" desc="GENPROTRANGE 0 base address"/>
-    </register>
-    <register name="GENPROTRANGE0_LIMIT" type="mmcfg" device="VTD_MEM_SM" offset="0x128" size="8" desc="Generic Protected Memory Range 0 Limit Address">
-      <field name="limit_address" bit="16" size="35" desc="GENPROTRANGE 0 limit address"/>
-    </register>
-    <!-- Integrated Memory Controller 0 -->
-    <register name="IMC0_SMBSTAT_0" type="mmcfg" device="IMC0_MAIN_SMBUS" offset="0x180" size="4" desc="SMBus Host Status">
-      <field name="RDATA" bit="0" size="16" desc="Read Data"/>
-      <field name="TSOD_SA" bit="24" size="4" desc="Last Issued TSOD Slave Address"/>
-      <field name="BUSY" bit="28" size="1" desc="SMBus Busy"/>
-      <field name="SBE" bit="29" size="1" desc="SMBus Error/Failed"/>
-      <field name="WOD" bit="30" size="1" desc="Write Operation Done"/>
-      <field name="RDO" bit="31" size="1" desc="Read Data Valid"/>
-    </register>
-    <register name="IMC0_SMBCMD_0" type="mmcfg" device="IMC0_MAIN_SMBUS" offset="0x184" size="4" desc="SMBus Host Command">
-      <field name="WDATA" bit="0" size="16" desc="Write Data"/>
-      <field name="BA" bit="16" size="8" desc="Bus Transaction Address"/>
-      <field name="SA" bit="24" size="3" desc="Slave Address"/>
-      <field name="WRT_CMD" bit="27" size="1" desc="Read/Write Command"/>
-      <field name="WRT_PNTR" bit="28" size="1" desc="Write Pointer"/>
-      <field name="WORD_ACCESS" bit="29" size="1" desc="Word Access"/>
-      <field name="PNTR_SEL" bit="30" size="1" desc="Pointer Select"/>
-      <field name="CMD_TRIGGER" bit="31" size="1" desc="Start/Trigger"/>
-    </register>
-    <register name="IMC0_SMBCNTL_0" type="mmcfg" device="IMC0_MAIN_SMBUS" offset="0x188" size="4" desc="SMBus Host Control">
-      <field name="DTI" bit="28" size="4" desc="Device Type Identifier"/>
-    </register>
-    <register name="IMC0_SMBSTAT_1" type="mmcfg" device="IMC0_MAIN_SMBUS" offset="0x190" size="4" desc="SMBus Host Status 1">
-      <field name="RDATA" bit="0" size="16" desc="Read Data"/>
-      <field name="TSOD_SA" bit="24" size="4" desc="Last Issued TSOD Slave Address"/>
-      <field name="BUSY" bit="28" size="1" desc="SMBus Busy"/>
-      <field name="SBE" bit="29" size="1" desc="SMBus Error/Failed"/>
-      <field name="WOD" bit="30" size="1" desc="Write Operation Done"/>
-      <field name="RDO" bit="31" size="1" desc="Read Data Valid"/>
-    </register>
-    <register name="IMC0_SMBCMD_1" type="mmcfg" device="IMC0_MAIN_SMBUS" offset="0x194" size="4" desc="SMBus Host Command 1">
-      <field name="WDATA" bit="0" size="16" desc="Write Data"/>
-      <field name="BA" bit="16" size="8" desc="Bus Transaction Address"/>
-      <field name="SA" bit="24" size="3" desc="Slave Address"/>
-      <field name="WRT_CMD" bit="27" size="1" desc="Read/Write Command"/>
-      <field name="WRT_PNTR" bit="28" size="1" desc="Write Pointer"/>
-      <field name="WORD_ACCESS" bit="29" size="1" desc="Word Access"/>
-      <field name="PNTR_SEL" bit="30" size="1" desc="Pointer Select"/>
-      <field name="CMD_TRIGGER" bit="31" size="1" desc="Start/Trigger"/>
-    </register>
-    <register name="IMC0_SMBCNTL_1" type="mmcfg" device="IMC0_MAIN_SMBUS" offset="0x198" size="4" desc="SMBus Host Control 1">
-      <field name="DTI" bit="28" size="4" desc="Device Type Identifier"/>
-    </register>
-    <!-- Integrated Memory Controller 1 -->
-    <register name="IMC1_SMBSTAT_0" type="mmcfg" device="IMC1_MAIN_SMBUS" offset="0x180" size="4" desc="SMBus Host Status">
-      <field name="RDATA" bit="0" size="16" desc="Read Data"/>
-      <field name="TSOD_SA" bit="24" size="4" desc="Last Issued TSOD Slave Address"/>
-      <field name="BUSY" bit="28" size="1" desc="SMBus Busy"/>
-      <field name="SBE" bit="29" size="1" desc="SMBus Error/Failed"/>
-      <field name="WOD" bit="30" size="1" desc="Write Operation Done"/>
-      <field name="RDO" bit="31" size="1" desc="Read Data Valid"/>
-    </register>
-    <register name="IMC1_SMBCMD_0" type="mmcfg" device="IMC1_MAIN_SMBUS" offset="0x184" size="4" desc="SMBus Host Command">
-      <field name="WDATA" bit="0" size="16" desc="Write Data"/>
-      <field name="BA" bit="16" size="8" desc="Bus Transaction Address"/>
-      <field name="SA" bit="24" size="3" desc="Slave Address"/>
-      <field name="WRT_CMD" bit="27" size="1" desc="Read/Write Command"/>
-      <field name="WRT_PNTR" bit="28" size="1" desc="Write Pointer"/>
-      <field name="WORD_ACCESS" bit="29" size="1" desc="Word Access"/>
-      <field name="PNTR_SEL" bit="30" size="1" desc="Pointer Select"/>
-      <field name="CMD_TRIGGER" bit="31" size="1" desc="Start/Trigger"/>
-    </register>
-    <register name="IMC1_SMBCNTL_0" type="mmcfg" device="IMC1_MAIN_SMBUS" offset="0x188" size="4" desc="SMBus Host Control">
-      <field name="DTI" bit="28" size="4" desc="Device Type Identifier"/>
-    </register>
-    <register name="IMC1_SMBSTAT_1" type="mmcfg" device="IMC1_MAIN_SMBUS" offset="0x190" size="4" desc="SMBus Host Status 1">
-      <field name="RDATA" bit="0" size="16" desc="Read Data"/>
-      <field name="TSOD_SA" bit="24" size="4" desc="Last Issued TSOD Slave Address"/>
-      <field name="BUSY" bit="28" size="1" desc="SMBus Busy"/>
-      <field name="SBE" bit="29" size="1" desc="SMBus Error/Failed"/>
-      <field name="WOD" bit="30" size="1" desc="Write Operation Done"/>
-      <field name="RDO" bit="31" size="1" desc="Read Data Valid"/>
-    </register>
-    <register name="IMC1_SMBCMD_1" type="mmcfg" device="IMC1_MAIN_SMBUS" offset="0x194" size="4" desc="SMBus Host Command 1">
-      <field name="WDATA" bit="0" size="16" desc="Write Data"/>
-      <field name="BA" bit="16" size="8" desc="Bus Transaction Address"/>
-      <field name="SA" bit="24" size="3" desc="Slave Address"/>
-      <field name="WRT_CMD" bit="27" size="1" desc="Read/Write Command"/>
-      <field name="WRT_PNTR" bit="28" size="1" desc="Write Pointer"/>
-      <field name="WORD_ACCESS" bit="29" size="1" desc="Word Access"/>
-      <field name="PNTR_SEL" bit="30" size="1" desc="Pointer Select"/>
-      <field name="CMD_TRIGGER" bit="31" size="1" desc="Start/Trigger"/>
-    </register>
-    <register name="IMC1_SMBCNTL_1" type="mmcfg" device="IMC1_MAIN_SMBUS" offset="0x198" size="4" desc="SMBus Host Control 1">
-      <field name="DTI" bit="28" size="4" desc="Device Type Identifier"/>
-    </register>
-    <!-- PCH ABASE (PMBASE) I/O registers -->
+    <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
+    <!-- PCIe Configuration registers -->
+    <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
+    <!-- Sections 1.6 -->
+    <register name="MSG_CTRL_REG" type="pcicfg" bus="0" dev="0" fun="0" offset="0xD0" desc="Message Bus Control Register">
+      <field name="MESSAGE_WR_BYTE_ENABLES" bit="4" size="4" desc="Message write byte enable"/>
+      <field name="MESSAGE_ADDRESS_OFFSET" bit="8" size="8" desc="Message register address"/>
+      <field name="MESSAGE_PORT" bit="16" size="8" desc="Message port"/>
+      <field name="MESSAGE_OPCODE" bit="24" size="8" desc="Message opcode"/>
+    </register>
+    <register name="MSG_DATA_REG" type="pcicfg" bus="0" dev="0" fun="0" offset="0xD4" desc="Message Bus Data Register">
+      <field name="MESSAGE_DATA" bit="0" size="32" desc="Message data"/>
+    </register>
+    <register name="MSG_CTRL_REG_EXT" type="pcicfg" bus="0" dev="0" fun="0" offset="0xD8" desc="Message Bus Control Register Extension">
+      <field name="MESSAGE_ADDRESS_OFFSET_EXT" bit="8" size="24" desc="Message register address extension"/>
+    </register>
+    <!-- Graphics -->
+    <!-- Section 4.1.13 -->
+    <register name="PCI0.0.0_GGC" type="pcicfg" bus="0" dev="0x2" fun="0" offset="0x50" size="4" desc="GMCH Graphics Control">
+      <field name="GGCLOCK" bit="0" size="1" desc="GGC Lock"/>
+      <field name="VGA_DISABLE" bit="1" size="1" desc="VGA Disable"/>
+      <field name="GMS" bit="3" size="7" desc="Graphics Mode Select"/>
+      <field name="GGMS" bit="8" size="2" desc="GTT Graphics Memory Size"/>
+      <field name="VAMEN" bit="14" size="1" desc="Versatile Acceleration"/>
+    </register>
+    <!-- Section 4.1.14 -->
+    <register name="PCI0.0.0_BDSM" type="pcicfg" bus="0" dev="0x2" fun="0" offset="0x5C" size="4" desc="Base of Data Stolen Memory">
+      <field name="LOCK" bit="0" size="1" desc="BDSM Lock"/>
+      <field name="BDSM" bit="20" size="12" desc="GFx Base of Data Stolen Memory"/>
+    </register>
+    <!-- Section 4.1.16 -->
+    <register name="PCI0.0.0_BGSM" type="pcicfg" bus="0" dev="0x2" fun="0" offset="0x70" size="4" desc="Base of Graphics Stolen Memory">
+      <field name="LOCK" bit="0" size="1" desc="BGSM Lock"/>
+      <field name="BGSM" bit="20" size="12" desc="GFx Base of GTT Stolen Memory"/>
+    </register>
+    <!-- iLB LPC Bridge -->
+    <!-- Section 10.20 PCU -->
+    <register name="ABASE" type="pcicfg" bus="0" dev="0x1F" fun="0" offset="0x40" size="4" desc="ACPI Base Address">
+      <field name="MEMI" bit="0" size="1" desc="Memory Space Indication"/>
+      <field name="Enable" bit="1" size="1" desc="Enable"/>
+      <field name="Base" bit="7" size="9" desc="Base Address"/>
+    </register>
+    <register name="PBASE" type="pcicfg" bus="0" dev="0x1F" fun="0" offset="0x44" size="4" desc="PMC Base Address">
+      <field name="MEMI" bit="0" size="1" desc="Memory Space Indication"/>
+      <field name="Enable" bit="1" size="1" desc="Enable"/>
+      <field name="ADDRNG" bit="2" size="1" desc="Address Range"/>
+      <field name="PREF" bit="3" size="1" desc="Prefetchable"/>
+      <field name="Base" bit="9" size="23" desc="Base Address"/>
+    </register>
+    <register name="GBASE" type="pcicfg" bus="0" dev="0x1F" fun="0" offset="0x48" size="4" desc="GPIO Base Address">
+      <field name="MEMI" bit="0" size="1" desc="Memory Space Indication"/>
+      <field name="Enable" bit="1" size="1" desc="Enable"/>
+      <field name="Base" bit="8" size="8" desc="Base Address"/>
+    </register>
+    <register name="IOBASE" type="pcicfg" bus="0" dev="0x1F" fun="0" offset="0x4C" size="4" desc="I/O Controller Base Address">
+      <field name="MEMI" bit="0" size="1" desc="Memory Space Indication"/>
+      <field name="Enable" bit="1" size="1" desc="Enable"/>
+      <field name="ADDRNG" bit="2" size="1" desc="Address Range"/>
+      <field name="PREF" bit="3" size="1" desc="Prefetchable"/>
+      <field name="Base" bit="14" size="18" desc="Base Address"/>
+    </register>
+    <register name="IBASE" type="pcicfg" bus="0" dev="0x1F" fun="0" offset="0x50" size="4" desc="ILB Base Address">
+      <field name="MEMI" bit="0" size="1" desc="Memory Space Indication"/>
+      <field name="Enable" bit="1" size="1" desc="Enable"/>
+      <field name="ADDRNG" bit="2" size="1" desc="Address Range"/>
+      <field name="PREF" bit="3" size="1" desc="Prefetchable"/>
+      <field name="Base" bit="9" size="23" desc="Base Address"/>
+    </register>
+    <register name="SBASE" type="pcicfg" bus="0" dev="0x1F" fun="0" offset="0x54" size="4" desc="SPI Base Address">
+      <field name="MEMI" bit="0" size="1" desc="Memory Space Indication"/>
+      <field name="Enable" bit="1" size="1" desc="Enable"/>
+      <field name="ADDRNG" bit="2" size="1" desc="Address Range"/>
+      <field name="PREF" bit="3" size="1" desc="Prefetchable"/>
+      <field name="Base" bit="9" size="23" desc="Base Address"/>
+    </register>
+    <register name="MPBASE" type="pcicfg" bus="0" dev="0x1F" fun="0" offset="0x58" size="4" desc="MPHY Base Address">
+      <field name="MEMI" bit="0" size="1" desc="Memory Space Indication"/>
+      <field name="Enable" bit="1" size="1" desc="Enable"/>
+      <field name="ADDRNG" bit="2" size="1" desc="Address Range"/>
+      <field name="PREF" bit="3" size="1" desc="Prefetchable"/>
+      <field name="Base" bit="20" size="12" desc="Base Address"/>
+    </register>
+    <register name="PUBASE" type="pcicfg" bus="0" dev="0x1F" fun="0" offset="0x5C" size="4" desc="PUnit Base Address">
+      <field name="MEMI" bit="0" size="1" desc="Memory Space Indication"/>
+      <field name="Enable" bit="1" size="1" desc="Enable"/>
+      <field name="ADDRNG" bit="2" size="1" desc="Address Range"/>
+      <field name="PREF" bit="3" size="1" desc="Prefetchable"/>
+      <field name="Base" bit="11" size="21" desc="Base Address"/>
+    </register>
+    <register name="BIOS_DECODE_EN" type="pcicfg" bus="0" dev="0x1F" fun="0" offset="0xD8" size="2" desc="BIOS Decode Enable">
+      <field name="E40" bit="0" size="1" desc="40-4F Enable"/>
+      <field name="E50" bit="1" size="1" desc="50-5F Enable"/>
+      <field name="E60" bit="2" size="1" desc="60-6F Enable"/>
+      <field name="E70" bit="3" size="1" desc="70-7F Enable"/>
+      <field name="LEE" bit="6" size="1" desc="Legacy E Segment Enable"/>
+      <field name="LFE" bit="7" size="1" desc="Legacy F Segment Enable"/>
+      <field name="EC0" bit="8" size="1" desc="C0-C8 Enable"/>
+      <field name="EC8" bit="9" size="1" desc="C8-CF Enable"/>
+      <field name="ED0" bit="10" size="1" desc="D0-D8 Enable"/>
+      <field name="ED8" bit="11" size="1" desc="D8-DF Enable"/>
+      <field name="EE0" bit="12" size="1" desc="E0-E8 Enable"/>
+      <field name="EE8" bit="13" size="1" desc="E8-EF Enable"/>
+      <field name="EF0" bit="14" size="1" desc="F0-F8 Enable"/>
+      <field name="EF8" bit="15" size="1" desc="F8-FF Enable"/>
+    </register>
+    <!-- Section 10.12.1 -->
+    <register name="GCS" type="mmio" bar="RCBA" offset="0x0" size="4" desc="General Control and Status">
+      <field name="BILD" bit="0" size="1" desc="BIOS Interface Lock Down"/>
+      <field name="TS" bit="1" size="1" desc="Top Swap"/>
+      <field name="BBS" bit="10" size="2" desc="Boot BIOS Straps"/>
+      <field name="BBSize" bit="29" size="2" desc="Boot Block Size"/>
+    </register>
+    <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
+    <!-- MMIO registers               -->
+    <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
+    <!-- Section 10.9.48 -->
+    <register name="BC" type="mmio" bar="SPIBAR" offset="0xFC" size="4" desc="BIOS Control Register (BCR)">
+      <field name="BIOSWE" bit="0" size="1" desc="BIOS Write Enable"/>
+      <field name="BLE" bit="1" size="1" desc="BIOS Lock Enable"/>
+      <field name="SRC" bit="2" size="2" desc="SPI Read Configuration"/>
+      <field name="SMM_BWP" bit="5" size="1" desc="SMM BIOS Write Protect"/>
+    </register>
+    <!-- PMBASE MMIO registers -->
+    <!-- Section 10.2.9 -->
+    <register name="GEN_PMCON2" type="mmio" bar="PMBASE" offset="0x24" size="4" desc="General PM Configuration 2">
+      <field name="PER_SMI_SEL" bit="0" size="2" desc="Period SMI Select"/>
+      <field name="SMI_LOCK" bit="4" size="1" desc="SMI Lock"/>
+    </register>
+    <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
+    <!-- I/O registers                -->
+    <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
+    <!-- ABASE I/O registers -->
+    <!-- Section 10.17.6 -->
     <register name="SMI_EN" type="iobar" bar="ABASE" offset="0x30" size="4" desc="SMI Control and Enable">
       <field name="GBL_SMI_EN" bit="0" size="1"/>
       <field name="EOS" bit="1" size="1"/>
       <field name="BIOS_EN" bit="2" size="1"/>
-      <field name="LEGACY_USB_EN" bit="3" size="1"/>
       <field name="SLP_SMI_EN" bit="4" size="1"/>
       <field name="APMC_EN" bit="5" size="1"/>
       <field name="SWSMI_TMR_EN" bit="6" size="1"/>
       <field name="BIOS_RLS" bit="7" size="1"/>
-      <field name="MCSMI_EN" bit="11" size="1"/>
       <field name="TCO_EN" bit="13" size="1"/>
       <field name="PERIODIC_EN" bit="14" size="1"/>
-      <field name="LEGACY_USB2_EN" bit="17" size="1"/>
-      <field name="INTEL_USB2_EN" bit="18" size="1"/>
-      <field name="GPIO_UNLOCK_SMI_EN" bit="27" size="1"/>
-      <field name="ME_SMI_EN" bit="30" size="1"/>
-      <field name="xHCI_SMI_EN" bit="31" size="1"/>
+      <field name="USB_SMI_EN" bit="17" size="1"/>
+      <field name="USB_IS_SMI_EN" bit="18" size="1"/>
+    </register>
+    <!-- Section 10.17.14 -->
+    <register name="TCO1_CNT" type="iobar" bar="ABASE" offset="0x68" size="4" desc="TCO Timer Control">
+      <field name="TCO_TMR_HALT" bit="11" size="1" desc="TCO Timre Halt"/>
+      <field name="TCO_LOCK" bit="12" size="1" desc="TCO Lock"/>
+      <field name="OS_POLICY" bit="20" size="2" desc="OS Policy"/>
+    </register>
+    <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
+    <!-- CPU MSRs                     -->
+    <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
+    <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
+    <!-- Message Bus registers        -->
+    <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
+    <!-- B-unit -->
+    <register name="BECREG" type="msgbus" port="0x3" offset="0x27" size="4" desc="Extended Configuration Space Base">
+      <field name="ECENABLE" bit="0" size="1" desc="EC Enable"/>
+      <field name="ECBASE" bit="28" size="4" desc="EC Boundary"/>
     </register>
-    <!-- CPU Model Specific Registers -->
   </registers>
+  <!-- #################################### -->
+  <!--                                      -->
+  <!-- 'Controls'                           -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <controls>
+    <control name="TopSwapStatus" register="GCS" field="TS" desc="Top Swap Status"/>
+    <control name="TopSwap" register="GCS" field="TS" desc="Top Swap"/>
+    <control name="BiosInterfaceLockDown" register="GCS" field="BILD" desc="BIOS Interface Lock-Down"/>
+    <control name="SMILock" register="GEN_PMCON2" field="SMI_LOCK" desc="SMI Global Configuration Lock"/>
+  </controls>
 </configuration>
```

### Comparing `chipsec-1.4.4/chipsec/cfg/pch_495.xml` & `chipsec-1.5.1/chipsec/cfg/8086/pch_3xxlp.xml`

 * *Files 8% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/pch_495.xml` & `chipsec-1.5.1/chipsec/cfg/8086/pch_3xxlp.xml`

```diff
@@ -1,14 +1,29 @@
 <?xml version="1.0" encoding="utf-8"?>
-<configuration platform="PCH_495">
+<configuration platform="PCH_3xxLP">
   <!--
-XML configuration file for the 495 series PCH
+XML configuration file for the 300 series LP (U/Y) PCH
+https://www.intel.com/content/www/us/en/products/docs/processors/core/7th-and-8th-gen-core-family-mobile-u-y-processor-lines-i-o-datasheet-vol-2.html
+334659-005
 -->
   <!-- #################################### -->
   <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info>
+    <sku did="0x9D4B" name="PCH-U" code="PCH_3xxLP" longname="PCH-Y with iHDCP 2.2 Premium"/>
+    <sku did="0x9D4E" name="PCH-U" code="PCH_3xxLP" longname="PCH-U with iHDCP 2.2 Premium"/>
+    <sku did="0x9D50" name="PCH-U" code="PCH_3xxLP" longname="PCH-U with iHDCP 2.2 Base"/>
+    <sku did="0x9D53" name="PCH-U" code="PCH_3xxLP" longname="PCH-U Base"/>
+    <sku did="0x9D56" name="PCH-Y" code="PCH_3xxLP" longname="PCH-Y Premium"/>
+    <sku did="0x9D58" name="PCH-U" code="PCH_3xxLP" longname="PCH-U Premium"/>
+  </info>
+  <!-- #################################### -->
+  <!--                                      -->
   <!-- Integrated devices                   -->
   <!--                                      -->
   <!-- #################################### -->
   <pci>
     <device name="P2SBC" bus="0" dev="0x1F" fun="1" vid="0x8086"/>
     <device name="PMC" bus="0" dev="0x1F" fun="2" vid="0x8086"/>
     <device name="SMBUS" bus="0" dev="0x1F" fun="4" vid="0x8086"/>
@@ -16,15 +31,14 @@
   </pci>
   <!-- #################################### -->
   <!--                                      -->
   <!-- Memory Mapped I/O spaces (MMIO BARs) -->
   <!--                                      -->
   <!-- #################################### -->
   <mmio>
-    <bar name="GTTMMADR" bus="0" dev="2" fun="0" reg="0x10" width="8" mask="0x7FFF000000" desc="Graphics Translation Table Range"/>
     <bar name="HDABAR" bus="0" dev="0x1F" fun="3" reg="0x10" width="8" mask="0xFFFFFFFFFFFFC000" size="0x1000" desc="HD Audio Base"/>
     <bar name="SPIBAR" bus="0" dev="0x1F" fun="5" reg="0x10" width="4" mask="0xFFFFF000" size="0x1000" desc="SPI Controller Register Range" offset="0x0"/>
     <bar name="PWRMBASE" register="PWRMBASE" base_field="BA" size="0x1000" fixed_address="0xFE000000" desc="Power Management Register Range"/>
     <bar name="SBREGBAR" register="SBREG_BAR" base_field="RBA" size="0x1000000" fixed_address="0xFD000000" desc="Sideband Register Access BAR"/>
   </mmio>
   <!-- #################################### -->
   <!--                                      -->
@@ -50,83 +64,74 @@
   <!--                                      -->
   <!-- #################################### -->
   <registers>
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- PCIe Configuration registers -->
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- Sideband Register Access Registers -->
-    <register name="SBREG_BAR" type="pcicfg" device="P2SBC" offset="0x10" size="4" desc="Sideband Register Access BAR">
+    <register name="SBREG_BAR" type="pcicfg" bus="0" dev="0x1F" fun="1" offset="0x10" size="4" desc="Sideband Register Access BAR">
       <field name="RBA" bit="24" size="8" desc="Register Base Address"/>
     </register>
-    <register name="P2SBC" type="pcicfg" device="P2SBC" offset="0xE0" size="2" desc="P2SB Configuration Register">
+    <register name="P2SBC" type="pcicfg" bus="0" dev="0x1F" fun="1" offset="0xE0" size="2" desc="P2SB Configuration Register">
       <field name="HIDE" bit="8" size="1" desc="Hide SBREG_BAR"/>
     </register>
-    <register name="P2SB_HIDE" type="pcicfg" device="P2SBC" offset="0xE1" size="1" desc="P2SB Configuration Register hide-unhide">
+    <register name="P2SB_HIDE" type="pcicfg" bus="0" dev="0x1F" fun="1" offset="0xE1" size="1" desc="P2SB Configuration Register hide-unhide">
       <field name="HIDE" bit="0" size="1" desc="Hide SBREG_BAR"/>
     </register>
     <!-- Power Management Controller -->
-    <register name="PWRMBASE" type="pcicfg" device="PMC" offset="0x10" size="4" desc="PM Base Address">
-      <field name="STYPE" bit="0" size="1" desc="Space Type (always 0 - memory space)"/>
-      <field name="BA" bit="13" size="19" desc="Base Address"/>
-    </register>
-    <register name="ABASE" type="pcicfg" device="PMC" offset="0x20" size="4" desc="ACPI Base Address">
+    <register name="ABASE" type="pcicfg" bus="0" dev="0x1f" fun="2" offset="0x40" size="4" desc="ACPI Base Address">
       <field name="STYPE" bit="0" size="1" desc="Space Type (always 1 - I/O space)"/>
-      <field name="BA" bit="7" size="25" desc="Base Address"/>
+      <field name="BA" bit="8" size="24" desc="Base Address"/>
     </register>
-    <register name="GEN_PMCON_1" type="mmio" bar="PWRMBASE" offset="0x1020" size="4" desc="General PM Configuration A">
-      <field name="ESPI_SMI_LOCK" bit="8" size="1" desc="ESPI_SMI_LOCK"/>
+    <register name="PWRMBASE" type="pcicfg" bus="0" dev="0x1f" fun="2" offset="0x10" size="4" desc="PM Base Address">
+      <field name="STYPE" bit="0" size="1" desc="Space Type (always 0 - memory space)"/>
+      <field name="BA" bit="14" size="18" desc="Base Address"/>
     </register>
-    <register name="GEN_PMCON_2" type="mmio" bar="PWRMBASE" offset="0x1024" size="4" desc="General PM Configuration B">
+    <register name="GEN_PMCON_1" type="pcicfg" bus="0" dev="0x1f" fun="2" offset="0xA0" size="4" desc="General PM Configuration A">
       <field name="SMI_LOCK" bit="4" size="1"/>
     </register>
-    <register name="PM_CFG" type="mmio" bar="PWRMBASE" offset="0x1818" size="4" desc="Power Management Configuration Reg 1"/>
-    <register name="ACTL" type="mmio" bar="PWRMBASE" offset="0x1BD8" size="4" desc="ACPI Control">
-      <field name="SCIS" bit="0" size="2" desc="SCI IRQ Select"/>
-      <field name="EN" bit="7" size="1" desc="ACPI Enable"/>
-      <field name="PWRM_EN" bit="8" size="1" desc="PWRM Enable"/>
+    <register name="GEN_PMCON_2" type="pcicfg" bus="0" dev="0x1f" fun="2" offset="0xA4" size="4" desc="General PM Configuration B"/>
+    <register name="ACTL" type="pcicfg" bus="0" dev="0x1f" fun="2" offset="0x44" size="4" desc="ACPI Control">
+      <field name="SCIS" bit="0" size="3" desc="SCI IRQ Select"/>
     </register>
+    <register name="PM_CFG" type="mmio" bar="PWRMBASE" offset="0x18" size="4" desc="Power Management Configuration Reg 1"/>
     <!-- SMBus Host Controller -->
-    <register name="SMBUS_VID" type="pcicfg" device="SMBUS" offset="0x00" size="2" desc="VID"/>
-    <register name="SMBUS_DID" type="pcicfg" device="SMBUS" offset="0x02" size="2" desc="DID"/>
-    <register name="SMBUS_CMD" type="pcicfg" device="SMBUS" offset="0x04" size="2" desc="CMD"/>
-    <register name="SMBUS_HCFG" type="pcicfg" device="SMBUS" offset="0x40" size="1" desc="Host Configuration">
+    <register name="SMBUS_VID" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x00" size="2" desc="VID"/>
+    <register name="SMBUS_DID" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x02" size="2" desc="DID"/>
+    <register name="SMBUS_CMD" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x04" size="2" desc="CMD"/>
+    <register name="SMBUS_HCFG" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x40" size="1" desc="Host Configuration">
       <field name="HST_EN" bit="0" size="1"/>
       <field name="SMB_SMI_EN" bit="1" size="1"/>
-      <field name="I2C_EN" bit="2" size="1"/>
+      <field name="I2C_EN" bit="2" size="2"/>
       <field name="SSRESET" bit="3" size="1"/>
       <field name="SPD_WD" bit="4" size="1"/>
     </register>
-    <register name="TCOBASE" type="pcicfg" device="SMBUS" offset="0x50" size="4" desc="TCO Base Address">
+    <register name="TCOBASE" type="pcicfg" bus="0" dev="0x1f" fun="4" offset="0x50" size="4" desc="TCO Base Address">
       <field name="IOS" bit="0" size="1" desc="I/O space"/>
       <field name="TCOBA" bit="5" size="11" desc="TCO Base Address"/>
     </register>
-    <register name="TCOCTL" type="pcicfg" device="SMBUS" offset="0x54" size="4" desc="TCO Control">
+    <register name="TCOCTL" type="pcicfg" bus="0" dev="0x1f" fun="4" offset="0x54" size="4" desc="TCO Control">
       <field name="TCO_BASE_LOCK" bit="0" size="1" desc="TCO Base Lock"/>
       <field name="TCO_BASE_EN" bit="8" size="1" desc="TCO Base Enable"/>
     </register>
     <!-- SPI Interface Controller -->
-    <register name="BC" type="pcicfg" device="SPI" offset="0xDC" size="4" desc="BIOS Control">
+    <register name="BC" type="pcicfg" bus="0" dev="0x1F" fun="5" offset="0xDC" size="4" desc="BIOS Control">
       <field name="BIOSWE" bit="0" size="1" desc="BIOS Write Enable"/>
       <field name="BLE" bit="1" size="1" desc="BIOS Lock Enable"/>
       <field name="SRC" bit="2" size="2" desc="SPI Read Configuration"/>
       <field name="TSS" bit="4" size="1" desc="Top Swap Status"/>
       <field name="SMM_BWP" bit="5" size="1" desc="SMM BIOS Write Protection"/>
       <field name="BBS" bit="6" size="1" desc="Boot BIOS Strap"/>
       <field name="BILD" bit="7" size="1" desc="BIOS Interface Lock Down"/>
-      <field name="ASE_BWP" bit="11" size="1" desc="Async SMI Enable for BIOS Write Protection"/>
     </register>
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- MMIO registers               -->
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- PCH SPIBAR registers -->
-    <register name="BFPR" type="mmio" bar="SPIBAR" offset="0x00" size="4" desc="BIOS Flash Primary Region Register (= FREG1)">
-      <field name="PRB" bit="0" size="15" desc="BIOS Flash Primary Region Base"/>
-      <field name="PRL" bit="16" size="15" desc="BIOS Flash Primary Region Limit"/>
-    </register>
-    <register name="HSFS" type="mmio" bar="SPIBAR" offset="0x4" size="4" desc="Hardware Sequencing Flash Status Register">
+    <register name="HSFS" type="mmio" bar="SPIBAR" offset="0x04" size="4" desc="Hardware Sequencing Flash Status Register">
       <field name="FDONE" bit="0" size="1" desc="Flash Cycle Done"/>
       <field name="FCERR" bit="1" size="1" desc="Flash Cycle Error"/>
       <field name="AEL" bit="2" size="1" desc="Access Error Log"/>
       <field name="SCIP" bit="5" size="1" desc="SPI cycle in progress"/>
       <field name="WRSDIS" bit="11" size="1" desc="Write status disable"/>
       <field name="PR34LKD" bit="12" size="1" desc="PRR3 PRR4 Lock-Down"/>
       <field name="FDOPSS" bit="13" size="1" desc="Flash Descriptor Override Pin-Strap Status"/>
@@ -158,14 +163,15 @@
       <field name="RB" bit="0" size="15" desc="Region Base"/>
       <field name="RL" bit="16" size="15" desc="Region Limit"/>
     </register>
     <register name="FREG5" type="mmio" bar="SPIBAR" offset="0x68" size="4" desc="Flash Region 5">
       <field name="RB" bit="0" size="15" desc="Region Base"/>
       <field name="RL" bit="16" size="15" desc="Region Limit"/>
     </register>
+    <register name="FREG6" undef="Flash Region 6 not defined for this platform"/>
     <register name="PR0" type="mmio" bar="SPIBAR" offset="0x84" size="4" desc="Protected Range 0">
       <field name="PRB" bit="0" size="15"/>
       <field name="RPE" bit="15" size="1"/>
       <field name="PRL" bit="16" size="15"/>
       <field name="WPE" bit="31" size="1"/>
     </register>
     <register name="PR1" type="mmio" bar="SPIBAR" offset="0x88" size="4" desc="Protected Range 1">
@@ -238,34 +244,28 @@
       <field name="BILD" bit="31" size="1" desc="BIOS Interface Lock-Down"/>
     </register>
     <register name="BUC" type="mm_msgbus" port="0xC3" offset="0x3414" size="4" desc="Backed Up Control">
       <field name="TS" bit="0" size="1" desc="Top Swap"/>
     </register>
     <!-- DCI registers -->
     <register name="ECTRL" type="mm_msgbus" port="0xB8" offset="0x0004" size="4" desc="DCI Control Register">
-      <field name="LOCK" bit="0" size="1"/>
       <field name="ENABLE" bit="4" size="1"/>
     </register>
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- I/O registers (I/O ports)    -->
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- PCH TCOBASE (SMBus TCO) I/O registers -->
     <register name="TCO1_CNT" type="iobar" bar="TCOBASE" offset="0x8" size="2" desc="TCO1 Control">
       <field name="TCO_LOCK" bit="12" size="1" desc="TCO Lock"/>
     </register>
-    <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
-    <!--      Undefined Registers     -->
-    <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
-    <register name="GC" undef="Not defined for platform"/>
   </registers>
   <!-- #################################### -->
   <!--                                      -->
   <!-- 'Controls'                           -->
   <!--                                      -->
   <!-- #################################### -->
   <controls>
     <control name="BiosInterfaceLockDown" register="BC" field="BILD" desc="BIOS Interface Lock-Down"/>
-    <control name="TopSwap" register="BC" field="TSS" desc="Top Swap Status"/>
     <control name="SpiWriteStatusDis" register="HSFS" field="WRSDIS" desc="Write Status Disable"/>
-    <control name="SMILock" register="GEN_PMCON_2" field="SMI_LOCK" desc="SMI Global Configuration Lock"/>
+    <control name="SMILock" register="GEN_PMCON_1" field="SMI_LOCK" desc="SMI Global Configuration Lock"/>
   </controls>
 </configuration>
```

### Comparing `chipsec-1.4.4/chipsec/cfg/pch_4xxlp.xml` & `chipsec-1.5.1/chipsec/cfg/8086/cfl.xml`

 * *Files 8% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/pch_4xxlp.xml` & `chipsec-1.5.1/chipsec/cfg/8086/cfl.xml`

```diff
@@ -1,42 +1,66 @@
 <?xml version="1.0" encoding="utf-8"?>
-<configuration platform="PCH_4xxLP">
+<configuration platform="CFL">
   <!--
-XML configuration file for the 300 series PCH
+XML configuration file for Coffee Lake
+
+* 8th Generation Intel(R) Processor Family for S-Processor Platforms
+  https://www.intel.com/content/www/us/en/processors/core/core-technical-resources.html
 -->
   <!-- #################################### -->
   <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info family="core">
+    <sku did="0x3E0F" name="CoffeeLake" code="CFL" longname="Desktop 8th Generation Core Processor (CoffeeLake S 2 Cores)"/>
+    <sku did="0x3E1F" name="CoffeeLake" code="CFL" longname="Desktop 8th Generation Core Processor (Coffeelake S 4 Cores)"/>
+    <sku did="0x3EC2" name="CoffeeLake" code="CFL" longname="Desktop 8th Generation Core Processor (Coffeelake S 6 Cores)"/>
+    <sku did="0x3E30" name="CoffeeLake" code="CFL" longname="Desktop 8th Generation Core Processor (CoffeeLake S 8 Cores)"/>
+    <sku did="0x3ECC" name="CoffeeLake" code="CFL" longname="Desktop 8th Generation Core Processor (CoffeeLake U 2 Cores)"/>
+    <sku did="0x3ED0" name="CoffeeLake" code="CFL" longname="Desktop 8th Generation Core Processor (CoffeeLake U 4 Cores)"/>
+    <sku did="0x3E10" name="CoffeeLake" code="CFL" longname="Desktop 8th Generation Core Processor (CoffeeLake H 4 Cores)"/>
+    <sku did="0x3EC4" name="CoffeeLake" code="CFL" longname="Desktop 8th Generation Core Processor (CoffeeLake H 6 Cores)"/>
+    <sku did="0x3E18" name="CoffeeLake" code="CFL" longname="Desktop 8th Generation Core Processor (CoffeeLake Workstation 4 Cores)"/>
+    <sku did="0x3EC6" name="CoffeeLake" code="CFL" longname="Desktop 8th Generation Core Processor (CoffeeLake Workstation 6 Cores)"/>
+    <sku did="0x3E31" name="CoffeeLake" code="CFL" longname="Desktop 8th Generation Core Processor (CoffeeLake Workstation 8 Cores)"/>
+    <sku did="0x3E33" name="CoffeeLake" code="CFL" longname="Desktop 8th Generation Core Processor (CoffeeLake Server 4 Cores)" detection_value="906EA"/>
+    <sku did="0x3ECA" name="CoffeeLake" code="CFL" longname="Desktop 8th Generation Core Processor (CoffeeLake Server 6 Cores)"/>
+    <sku did="0x3E32" name="CoffeeLake" code="CFL" longname="Desktop 8th Generation Core Processor (CoffeeLake Server 8 Cores)"/>
+  </info>
+  <!-- #################################### -->
+  <!--                                      -->
   <!-- Integrated devices                   -->
   <!--                                      -->
   <!-- #################################### -->
   <pci>
     <device name="P2SBC" bus="0" dev="0x1F" fun="1" vid="0x8086"/>
-    <device name="PMC" bus="0" dev="0x1F" fun="2" vid="0x8086"/>
     <device name="SMBUS" bus="0" dev="0x1F" fun="4" vid="0x8086"/>
     <device name="SPI" bus="0" dev="0x1F" fun="5" vid="0x8086"/>
   </pci>
   <!-- #################################### -->
   <!--                                      -->
   <!-- Memory Mapped I/O spaces (MMIO BARs) -->
   <!--                                      -->
   <!-- #################################### -->
   <mmio>
+    <bar name="GTTMMADR" bus="0" dev="2" fun="0" reg="0x10" width="8" mask="0x7FFF000000" desc="Graphics Translation Table Range"/>
     <bar name="HDABAR" bus="0" dev="0x1F" fun="3" reg="0x10" width="8" mask="0xFFFFFFFFFFFFC000" size="0x1000" desc="HD Audio Base"/>
     <bar name="SPIBAR" bus="0" dev="0x1F" fun="5" reg="0x10" width="4" mask="0xFFFFF000" size="0x1000" desc="SPI Controller Register Range" offset="0x0"/>
     <bar name="PWRMBASE" register="PWRMBASE" base_field="BA" size="0x1000" fixed_address="0xFE000000" desc="Power Management Register Range"/>
     <bar name="SBREGBAR" register="SBREG_BAR" base_field="RBA" size="0x1000000" fixed_address="0xFD000000" desc="Sideband Register Access BAR"/>
   </mmio>
   <!-- #################################### -->
   <!--                                      -->
   <!-- I/O spaces (I/O BARs)                -->
   <!--                                      -->
   <!-- #################################### -->
   <io>
-    <bar name="ABASE" register="ABASE" base_field="BA" size="0x100" fixed_address="0x1800" desc="ACPI Base Address"/>
-    <bar name="PMBASE" register="ABASE" base_field="BA" size="0x100" fixed_address="0x1800" desc="ACPI Base Address"/>
+    <bar name="ABASE" register="ABASE" base_field="BA" size="0x100" desc="ACPI Base Address"/>
+    <bar name="PMBASE" register="ABASE" base_field="BA" size="0x100" desc="ACPI Base Address"/>
     <bar name="TCOBASE" register="TCOBASE" base_field="TCOBA" size="0x20" desc="TCO Base Address"/>
     <!-- old definition -->
     <bar name="SMBUS_BASE" bus="0" dev="0x1F" fun="4" reg="0x20" mask="0xFFE0" size="0x80" desc="SMBus Base Address"/>
   </io>
   <!-- #################################### -->
   <!--                                      -->
   <!-- Memory ranges                        -->
@@ -49,85 +73,74 @@
   <!--                                      -->
   <!-- #################################### -->
   <registers>
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- PCIe Configuration registers -->
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- Sideband Register Access Registers -->
-    <register name="SBREG_BAR" type="pcicfg" device="P2SBC" offset="0x10" size="4" desc="Sideband Register Access BAR">
+    <register name="SBREG_BAR" type="pcicfg" bus="0" dev="0x1F" fun="1" offset="0x10" size="4" desc="Sideband Register Access BAR">
       <field name="RBA" bit="24" size="8" desc="Register Base Address"/>
     </register>
-    <register name="P2SBC" type="pcicfg" device="P2SBC" offset="0xE0" size="2" desc="P2SB Configuration Register">
+    <register name="P2SBC" type="pcicfg" bus="0" dev="0x1F" fun="1" offset="0xE0" size="2" desc="P2SB Configuration Register">
       <field name="HIDE" bit="8" size="1" desc="Hide SBREG_BAR"/>
     </register>
-    <register name="P2SB_HIDE" type="pcicfg" device="P2SBC" offset="0xE1" size="1" desc="P2SB Configuration Register hide-unhide">
+    <register name="P2SB_HIDE" type="pcicfg" bus="0" dev="0x1F" fun="1" offset="0xE1" size="1" desc="P2SB Configuration Register hide-unhide">
       <field name="HIDE" bit="0" size="1" desc="Hide SBREG_BAR"/>
     </register>
     <!-- Power Management Controller -->
-    <register name="ABASE" type="pcicfg" device="PMC" offset="0x20" size="4" desc="ACPI Base Address">
+    <register name="ABASE" type="pcicfg" bus="0" dev="0x1f" fun="2" offset="0x40" size="4" desc="ACPI Base Address">
       <field name="STYPE" bit="0" size="1" desc="Space Type (always 1 - I/O space)"/>
-      <field name="BA" bit="7" size="25" desc="Base Address"/>
+      <field name="BA" bit="8" size="8" desc="Base Address"/>
     </register>
-    <register name="PWRMBASE" type="pcicfg" device="PMC" offset="0x10" size="4" desc="PM Base Address">
-      <field name="STYPE" bit="0" size="1" desc="Space Type (always 0 - memory space)"/>
-      <field name="BA" bit="13" size="19" desc="Base Address"/>
+    <register name="ACTL" type="pcicfg" bus="0" dev="0x1f" fun="2" offset="0x44" size="4" desc="ACPI Control">
+      <field name="SCIS" bit="0" size="2" desc="SCI IRQ Select"/>
+      <field name="EN" bit="7" size="1" desc="ACPI Enable"/>
+      <field name="PWRM_EN" bit="8" size="1" desc="PWRM Enable"/>
     </register>
-    <register name="GEN_PMCON_1" type="mmio" bar="PWRMBASE" offset="0x1020" size="4" desc="General PM Configuration A">
-      <field name="ESPI_SMI_LOCK" bit="8" size="1" desc="ESPI_SMI_LOCK"/>
+    <register name="PWRMBASE" type="pcicfg" bus="0" dev="0x1f" fun="2" offset="0x48" size="4" desc="PM Base Address">
+      <field name="STYPE" bit="0" size="1" desc="Space Type (always 0 - memory space)"/>
+      <field name="BA" bit="12" size="20" desc="Base Address"/>
     </register>
-    <register name="GEN_PMCON_2" type="mmio" bar="PWRMBASE" offset="0x1024" size="4" desc="General PM Configuration B">
+    <register name="GEN_PMCON_1" type="pcicfg" bus="0" dev="0x1f" fun="2" offset="0xA0" size="2" desc="General PM Configuration A">
       <field name="SMI_LOCK" bit="4" size="1"/>
     </register>
-    <register name="PM_CFG" type="mmio" bar="PWRMBASE" offset="0x1818" size="4" desc="Power Management Configuration Reg 1"/>
-    <register name="ACTL" type="mmio" bar="PWRMBASE" offset="0x1BD8" size="4" desc="ACPI Control">
-      <field name="SCIS" bit="0" size="3" desc="SCI IRQ Select"/>
-    </register>
     <!-- SMBus Host Controller -->
-    <register name="SMBUS_VID" type="pcicfg" device="SMBUS" offset="0x00" size="2" desc="VID"/>
-    <register name="SMBUS_DID" type="pcicfg" device="SMBUS" offset="0x02" size="2" desc="DID"/>
-    <register name="SMBUS_CMD" type="pcicfg" device="SMBUS" offset="0x04" size="2" desc="CMD"/>
-    <register name="SMBUS_HCFG" type="pcicfg" device="SMBUS" offset="0x40" size="1" desc="Host Configuration">
+    <register name="SMBUS_VID" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x00" size="2" desc="VID"/>
+    <register name="SMBUS_DID" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x02" size="2" desc="DID"/>
+    <register name="SMBUS_CMD" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x04" size="2" desc="CMD"/>
+    <register name="SMBUS_HCFG" type="pcicfg" bus="0" dev="0x1F" fun="4" offset="0x40" size="1" desc="Host Configuration">
       <field name="HST_EN" bit="0" size="1"/>
       <field name="SMB_SMI_EN" bit="1" size="1"/>
-      <field name="I2C_EN" bit="2" size="1"/>
+      <field name="I2C_EN" bit="2" size="2"/>
       <field name="SSRESET" bit="3" size="1"/>
       <field name="SPD_WD" bit="4" size="1"/>
     </register>
-    <register name="SMBBASE" type="pcicfg" device="SMBUS" offset="0x20" size="4" desc="SMB Base Address">
-      <field name="IOS" bit="0" size="1" desc="I/O space"/>
-      <field name="SMBBA" bit="5" size="11" desc="SMB Base Address"/>
-    </register>
-    <register name="TCOBASE" type="pcicfg" device="SMBUS" offset="0x50" size="4" desc="TCO Base Address">
+    <register name="TCOBASE" type="pcicfg" bus="0" dev="0x1f" fun="4" offset="0x50" size="4" desc="TCO Base Address">
       <field name="IOS" bit="0" size="1" desc="I/O space"/>
       <field name="TCOBA" bit="5" size="11" desc="TCO Base Address"/>
     </register>
-    <register name="TCOCTL" type="pcicfg" device="SMBUS" offset="0x54" size="4" desc="TCO Control">
+    <register name="TCOCTL" type="pcicfg" bus="0" dev="0x1f" fun="4" offset="0x54" size="4" desc="TCO Control">
       <field name="TCO_BASE_LOCK" bit="0" size="1" desc="TCO Base Lock"/>
       <field name="TCO_BASE_EN" bit="8" size="1" desc="TCO Base Enable"/>
     </register>
     <!-- SPI Interface Controller -->
-    <register name="BC" type="pcicfg" device="SPI" offset="0xDC" size="4" desc="BIOS Control">
+    <register name="BC" type="pcicfg" bus="0" dev="0x1F" fun="5" offset="0xDC" size="4" desc="BIOS Control">
       <field name="BIOSWE" bit="0" size="1" desc="BIOS Write Enable"/>
       <field name="BLE" bit="1" size="1" desc="BIOS Lock Enable"/>
       <field name="SRC" bit="2" size="2" desc="SPI Read Configuration"/>
       <field name="TSS" bit="4" size="1" desc="Top Swap Status"/>
       <field name="SMM_BWP" bit="5" size="1" desc="SMM BIOS Write Protection"/>
       <field name="BBS" bit="6" size="1" desc="Boot BIOS Strap"/>
       <field name="BILD" bit="7" size="1" desc="BIOS Interface Lock Down"/>
-      <field name="ASE_BWP" bit="11" size="1" desc="Async SMI Enable for BIOS Write Protection"/>
     </register>
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- MMIO registers               -->
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- PCH SPIBAR registers -->
-    <register name="BFPR" type="mmio" bar="SPIBAR" offset="0x00" size="4" desc="BIOS Flash Primary Region Register (= FREG1)">
-      <field name="PRB" bit="0" size="15" desc="BIOS Flash Primary Region Base"/>
-      <field name="PRL" bit="16" size="15" desc="BIOS Flash Primary Region Limit"/>
-    </register>
-    <register name="HSFS" type="mmio" bar="SPIBAR" offset="0x4" size="4" desc="Hardware Sequencing Flash Status Register">
+    <register name="HSFS" type="mmio" bar="SPIBAR" offset="0x04" size="4" desc="Hardware Sequencing Flash Status Register">
       <field name="FDONE" bit="0" size="1" desc="Flash Cycle Done"/>
       <field name="FCERR" bit="1" size="1" desc="Flash Cycle Error"/>
       <field name="AEL" bit="2" size="1" desc="Access Error Log"/>
       <field name="SCIP" bit="5" size="1" desc="SPI cycle in progress"/>
       <field name="WRSDIS" bit="11" size="1" desc="Write status disable"/>
       <field name="PR34LKD" bit="12" size="1" desc="PRR3 PRR4 Lock-Down"/>
       <field name="FDOPSS" bit="13" size="1" desc="Flash Descriptor Override Pin-Strap Status"/>
@@ -159,40 +172,41 @@
       <field name="RB" bit="0" size="15" desc="Region Base"/>
       <field name="RL" bit="16" size="15" desc="Region Limit"/>
     </register>
     <register name="FREG5" type="mmio" bar="SPIBAR" offset="0x68" size="4" desc="Flash Region 5">
       <field name="RB" bit="0" size="15" desc="Region Base"/>
       <field name="RL" bit="16" size="15" desc="Region Limit"/>
     </register>
+    <register name="FREG6" undef="Flash Region 6 not defined for this platform"/>
     <register name="PR0" type="mmio" bar="SPIBAR" offset="0x84" size="4" desc="Protected Range 0">
-      <field name="PRB" bit="0" size="15"/>
+      <field name="PRB" bit="0" size="13"/>
       <field name="RPE" bit="15" size="1"/>
       <field name="PRL" bit="16" size="15"/>
       <field name="WPE" bit="31" size="1"/>
     </register>
     <register name="PR1" type="mmio" bar="SPIBAR" offset="0x88" size="4" desc="Protected Range 1">
-      <field name="PRB" bit="0" size="15"/>
+      <field name="PRB" bit="0" size="13"/>
       <field name="RPE" bit="15" size="1"/>
       <field name="PRL" bit="16" size="15"/>
       <field name="WPE" bit="31" size="1"/>
     </register>
     <register name="PR2" type="mmio" bar="SPIBAR" offset="0x8C" size="4" desc="Protected Range 2">
-      <field name="PRB" bit="0" size="15"/>
+      <field name="PRB" bit="0" size="13"/>
       <field name="RPE" bit="15" size="1"/>
       <field name="PRL" bit="16" size="15"/>
       <field name="WPE" bit="31" size="1"/>
     </register>
     <register name="PR3" type="mmio" bar="SPIBAR" offset="0x90" size="4" desc="Protected Range 3">
-      <field name="PRB" bit="0" size="15"/>
+      <field name="PRB" bit="0" size="13"/>
       <field name="RPE" bit="15" size="1"/>
       <field name="PRL" bit="16" size="15"/>
       <field name="WPE" bit="31" size="1"/>
     </register>
     <register name="PR4" type="mmio" bar="SPIBAR" offset="0x94" size="4" desc="Protected Range 4">
-      <field name="PRB" bit="0" size="15"/>
+      <field name="PRB" bit="0" size="13"/>
       <field name="RPE" bit="15" size="1"/>
       <field name="PRL" bit="16" size="15"/>
       <field name="WPE" bit="31" size="1"/>
     </register>
     <register name="FDOC" type="mmio" bar="SPIBAR" offset="0xB4" size="4" desc="Flash Descriptor Observability Control Register">
       <field name="FDSI" bit="2" size="10" desc="Flash Descriptor Section Index"/>
       <field name="FDSS" bit="12" size="3" desc="Flash Descriptor Section Select"/>
@@ -237,36 +251,30 @@
       <field name="LL" bit="3" size="1" desc="Lower 128 Byte Lock"/>
       <field name="UL" bit="4" size="1" desc="Upper 128 Byte Lock"/>
       <field name="BILD" bit="31" size="1" desc="BIOS Interface Lock-Down"/>
     </register>
     <register name="BUC" type="mm_msgbus" port="0xC3" offset="0x3414" size="4" desc="Backed Up Control">
       <field name="TS" bit="0" size="1" desc="Top Swap"/>
     </register>
+    <register name="PM_CFG" type="mmio" bar="PWRMBASE" offset="0x18" size="4" desc="Power Management Configuration Reg 1"/>
     <!-- DCI registers -->
     <register name="ECTRL" type="mm_msgbus" port="0xB8" offset="0x0004" size="4" desc="DCI Control Register">
-      <field name="LOCK" bit="0" size="1"/>
       <field name="ENABLE" bit="4" size="1"/>
     </register>
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- I/O registers (I/O ports)    -->
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- PCH TCOBASE (SMBus TCO) I/O registers -->
     <register name="TCO1_CNT" type="iobar" bar="TCOBASE" offset="0x8" size="2" desc="TCO1 Control">
       <field name="TCO_LOCK" bit="12" size="1" desc="TCO Lock"/>
     </register>
-    <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
-    <!--      Undefined Registers     -->
-    <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
-    <register name="GC" undef="Not defined for platform"/>
   </registers>
   <!-- #################################### -->
   <!--                                      -->
   <!-- 'Controls'                           -->
   <!--                                      -->
   <!-- #################################### -->
   <controls>
     <control name="BiosInterfaceLockDown" register="BC" field="BILD" desc="BIOS Interface Lock-Down"/>
-    <control name="TopSwap" register="BC" field="TSS" desc="Top Swap Status"/>
     <control name="SpiWriteStatusDis" register="HSFS" field="WRSDIS" desc="Write Status Disable"/>
-    <control name="SMILock" register="GEN_PMCON_2" field="SMI_LOCK" desc="SMI Global Configuration Lock"/>
   </controls>
 </configuration>
```

### Comparing `chipsec-1.4.4/chipsec/cfg/__init__.py` & `chipsec-1.5.1/chipsec/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/cfg/chipsec_cfg.xsd` & `chipsec-1.5.1/chipsec/cfg/chipsec_cfg.xsd`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/cfg/ivt.xml` & `chipsec-1.5.1/chipsec/cfg/8086/ivt.xml`

 * *Files 7% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/ivt.xml` & `chipsec-1.5.1/chipsec/cfg/8086/ivt.xml`

```diff
@@ -1,12 +1,20 @@
 <?xml version="1.0" encoding="utf-8"?>
 <configuration platform="IVT">
   <!--
 XML configuration file for Ivytown (Ivy Bridge-E) based platforms
 -->
+  <!-- #################################### -->
+  <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info family="xeon">
+    <sku did="0x0E00" name="Ivytown" code="IVT" longname="Server 3rd Generation Core Procesor (Ivytown CPU / Patsburg PCH)"/>
+  </info>
   <registers>
     <!-- B:D.F 00:12.6 -->
     <register name="PCI0.0.0_SMRAMC" type="pcicfg" bus="0" dev="12" fun="6" offset="0x4c" size="1" desc="System Management RAM Control">
       <field name="D_OPEN" bit="6" size="1"/>
       <field name="D_CLS" bit="5" size="1"/>
       <field name="D_LCK" bit="4" size="1"/>
       <field name="G_SMRAME" bit="3" size="1"/>
```

### Comparing `chipsec-1.4.4/chipsec/cfg/pch_c620.xml` & `chipsec-1.5.1/chipsec/cfg/8086/pch_c620.xml`

 * *Files 3% similar despite different names*

#### Comparing `chipsec-1.4.4/chipsec/cfg/pch_c620.xml` & `chipsec-1.5.1/chipsec/cfg/8086/pch_c620.xml`

```diff
@@ -4,14 +4,34 @@
 XML configuration file for
 
 * Intel(R) C620 Series Chipset Family Platform Controller Hub
   https://www.intel.com/content/dam/www/public/us/en/documents/datasheets/c620-series-chipset-datasheet.pdf
 -->
   <!-- #################################### -->
   <!--                                      -->
+  <!-- Information                          -->
+  <!--                                      -->
+  <!-- #################################### -->
+  <info>
+    <sku did="0xA1C1" name="C621" code="PCH_C620" longname="Intel C621 (C620 series) PCH"/>
+    <sku did="0xA1C2" name="C622" code="PCH_C620" longname="Intel C622 (C620 series) PCH"/>
+    <sku did="0xA1C3" name="C624" code="PCH_C620" longname="Intel C624 (C620 series) PCH"/>
+    <sku did="0xA1C4" name="C625" code="PCH_C620" longname="Intel C625 (C620 series) PCH"/>
+    <sku did="0xA1C5" name="C626" code="PCH_C620" longname="Intel C626 (C620 series) PCH"/>
+    <sku did="0xA1C6" name="C627" code="PCH_C620" longname="Intel C627 (C620 series) PCH"/>
+    <sku did="0xA1C7" name="C628" code="PCH_C620" longname="Intel C628 (C620 series) PCH"/>
+    <sku did="0xA1CA" name="C629" code="PCH_C620" longname="Intel C629 (C620 series) PCH"/>
+    <sku did="0xA242" name="C624" code="PCH_C620" longname="Intel C624 (C620 series) PCH"/>
+    <sku did="0xA243" name="C627" code="PCH_C620" longname="Intel C627 (C620 series) PCH"/>
+    <sku did="0xA244" name="C621" code="PCH_C620" longname="Intel C621 (C620 series) PCH"/>
+    <sku did="0xA245" name="C627" code="PCH_C620" longname="Intel C627 (C620 series) PCH"/>
+    <sku did="0xA246" name="C628" code="PCH_C620" longname="Intel C628 (C620 series) PCH"/>
+  </info>
+  <!-- #################################### -->
+  <!--                                      -->
   <!-- Integrated devices                   -->
   <!--                                      -->
   <!-- #################################### -->
   <pci>
     <device name="SATA" bus="0" dev="0x17" fun="0" vid="0x8086" did="0xA182,0xA186,0xA202,0xA206,0x2822,0x2826"/>
     <device name="P2SBC" bus="0" dev="0x1F" fun="1" vid="0x8086" did="0xA220,0xA1A0"/>
     <device name="PMC" bus="0" dev="0x1F" fun="2" vid="0x8086" did="0xA221,0xA1A1"/>
@@ -73,15 +93,15 @@
     </register>
     <!-- Power Management Controller -->
     <register name="ABASE" type="pcicfg" device="PMC" offset="0x40" size="4" desc="ACPI Base Address">
       <field name="Base" bit="8" size="24" desc="Base Address"/>
       <field name="STYPE" bit="0" size="1" desc="Space Type (always 1 - I/O space)"/>
     </register>
     <register name="ACTL" type="pcicfg" device="PMC" offset="0x44" size="4" desc="ACPI Control">
-      <field name="SCIS" bit="0" size="2" desc="SCI IRQ Select"/>
+      <field name="SCIS" bit="0" size="3" desc="SCI IRQ Select"/>
       <field name="EN" bit="7" size="1" desc="ACPI Enable"/>
       <field name="PWRM_EN" bit="8" size="1" desc="PWRM Enable"/>
     </register>
     <register name="PWRMBASE" type="pcicfg" device="PMC" offset="0x48" size="4" desc="PM Base Address">
       <field name="STYPE" bit="0" size="1" desc="Space Type (always 0 - memory space)"/>
       <field name="BA" bit="12" size="20" desc="Base Address"/>
     </register>
@@ -192,42 +212,42 @@
       <field name="RL" bit="16" size="15" desc="Region Limit"/>
     </register>
     <register name="FREG11" type="mmio" bar="SPIBAR" offset="0x80" size="4" desc="Flash Region 11">
       <field name="RB" bit="0" size="15" desc="Region Base"/>
       <field name="RL" bit="16" size="15" desc="Region Limit"/>
     </register>
     <register name="PR0" type="mmio" bar="SPIBAR" offset="0x84" size="4" desc="Protected Range 0">
-      <field name="PRB" bit="0" size="13"/>
-      <field name="RPE" bit="15" size="1"/>
-      <field name="PRL" bit="16" size="15"/>
-      <field name="WPE" bit="31" size="1"/>
+      <field name="PRB" bit="0" size="15" desc="Protected Range Base"/>
+      <field name="RPE" bit="15" size="1" desc="Read Protection Enabled"/>
+      <field name="PRL" bit="16" size="15" desc="Protected Range Limit"/>
+      <field name="WPE" bit="31" size="1" desc="Write Protection Enabled"/>
     </register>
     <register name="PR1" type="mmio" bar="SPIBAR" offset="0x88" size="4" desc="Protected Range 1">
-      <field name="PRB" bit="0" size="13"/>
-      <field name="RPE" bit="15" size="1"/>
-      <field name="PRL" bit="16" size="15"/>
-      <field name="WPE" bit="31" size="1"/>
+      <field name="PRB" bit="0" size="15" desc="Protected Range Base"/>
+      <field name="RPE" bit="15" size="1" desc="Read Protection Enabled"/>
+      <field name="PRL" bit="16" size="15" desc="Protected Range Limit"/>
+      <field name="WPE" bit="31" size="1" desc="Write Protection Enabled"/>
     </register>
     <register name="PR2" type="mmio" bar="SPIBAR" offset="0x8C" size="4" desc="Protected Range 2">
-      <field name="PRB" bit="0" size="13"/>
-      <field name="RPE" bit="15" size="1"/>
-      <field name="PRL" bit="16" size="15"/>
-      <field name="WPE" bit="31" size="1"/>
+      <field name="PRB" bit="0" size="15" desc="Protected Range Base"/>
+      <field name="RPE" bit="15" size="1" desc="Read Protection Enabled"/>
+      <field name="PRL" bit="16" size="15" desc="Protected Range Limit"/>
+      <field name="WPE" bit="31" size="1" desc="Write Protection Enabled"/>
     </register>
     <register name="PR3" type="mmio" bar="SPIBAR" offset="0x90" size="4" desc="Protected Range 3">
-      <field name="PRB" bit="0" size="13"/>
-      <field name="RPE" bit="15" size="1"/>
-      <field name="PRL" bit="16" size="15"/>
-      <field name="WPE" bit="31" size="1"/>
+      <field name="PRB" bit="0" size="15" desc="Protected Range Base"/>
+      <field name="RPE" bit="15" size="1" desc="Read Protection Enabled"/>
+      <field name="PRL" bit="16" size="15" desc="Protected Range Limit"/>
+      <field name="WPE" bit="31" size="1" desc="Write Protection Enabled"/>
     </register>
     <register name="PR4" type="mmio" bar="SPIBAR" offset="0x94" size="4" desc="Protected Range 4">
-      <field name="PRB" bit="0" size="13"/>
-      <field name="RPE" bit="15" size="1"/>
-      <field name="PRL" bit="16" size="15"/>
-      <field name="WPE" bit="31" size="1"/>
+      <field name="PRB" bit="0" size="15" desc="Protected Range Base"/>
+      <field name="RPE" bit="15" size="1" desc="Read Protection Enabled"/>
+      <field name="PRL" bit="16" size="15" desc="Protected Range Limit"/>
+      <field name="WPE" bit="31" size="1" desc="Write Protection Enabled"/>
     </register>
     <register name="FDOC" type="mmio" bar="SPIBAR" offset="0xB4" size="4" desc="Flash Descriptor Observability Control Register">
       <field name="FDSI" bit="2" size="10" desc="Flash Descriptor Section Index"/>
       <field name="FDSS" bit="12" size="3" desc="Flash Descriptor Section Select"/>
     </register>
     <register name="FDOD" type="mmio" bar="SPIBAR" offset="0xB8" size="4" desc="Flash Descriptor Observability Data Register">
       <field name="FDSD" bit="0" size="32" desc="Flash Descriptor Section Data"/>
@@ -346,19 +366,23 @@
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- I/O registers (I/O ports)    -->
     <!-- ~~~~~~~~~~~~~~~~~~~~~~~~~~~~ -->
     <!-- PCH TCOBASE (SMBus TCO) I/O registers -->
     <register name="TCO1_CNT" type="iobar" bar="TCOBASE" offset="0x8" size="2" desc="TCO1 Control">
       <field name="TCO_LOCK" bit="12" size="1" desc="TCO Lock"/>
     </register>
+    <register name="ECTRL" type="mm_msgbus" port="0xB8" offset="0x0004" size="4" desc="DCI Control Register">
+      <field name="ENABLE" bit="4" size="1"/>
+    </register>
   </registers>
   <!-- #################################### -->
   <!--                                      -->
   <!-- 'Controls'                           -->
   <!--                                      -->
   <!-- #################################### -->
   <controls>
     <control name="BiosInterfaceLockDown" register="BC" field="BILD" desc="BIOS Interface Lock-Down"/>
     <control name="SpiWriteStatusDis" register="HSFS" field="WRSDIS" desc="Write Status Disable"/>
     <control name="ACPIBaseLock" register="GEN_PMCON_B" field="ACPI_BASE_LOCK" desc="Lock Down ACPI Base Address"/>
+    <control name="TcoCtlLock" register="TCOCTL" field="TCO_BASE_LOCK" desc="TCO Base Lock"/>
   </controls>
 </configuration>
```

### Comparing `chipsec-1.4.4/chipsec/fuzzing/primitives.py` & `chipsec-1.5.1/chipsec/fuzzing/primitives.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/fuzzing/__init__.py` & `chipsec-1.5.1/chipsec/fuzzing/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/module_common.py` & `chipsec-1.5.1/chipsec/module_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -68,15 +68,14 @@
     def is_supported(self):
         """
         This method should be overwritten by the module returning True or False
         depending whether or not this module is supported in the currently running
         platform.
         To access the currently running platform use
 
-        >>> self.cs.get_chipset_id()
         """
         return True
 
     def update_res(self, value):
         if self.res == ModuleResult.WARNING:
             if value == ModuleResult.FAILED \
             or value == ModuleResult.ERROR:
```

### Comparing `chipsec-1.4.4/chipsec/logger.py` & `chipsec-1.5.1/chipsec/logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -21,17 +21,19 @@
 
 """
 Logging functions
 """
 import logging as pyLogging
 import platform
 import string
+import binascii
 import sys
 import os
 from time import localtime, strftime
+import atexit
 
 from chipsec.testcase import TestCase, ChipsecResults
 import traceback
 try:
     import WConio
     has_WConio = True
 except ImportError:
@@ -68,18 +70,19 @@
             pyLogging.CRITICAL: BLUE,
             pyLogging.ERROR: RED
             }
 
             def log_color ( self, message, record ):
                 """ Testing """
                 if record.levelno in self.LEVEL_ID:
-                    old_setting = WConio.gettextinfo()[4] & 0x00FF
                     WConio.textcolor( self.LEVEL_ID[record.levelno] )
                     return message
-                WConio.textcolor( old_setting )
+
+            old_setting = WConio.gettextinfo()[4] & 0x00FF
+            atexit.register(WConio.textcolor, old_setting)
 
         else:
             def log_color( self, message, record ):
                 return message
 
     elif "linux" == platform.system().lower():
         ENDC = '\033[0m'
@@ -93,27 +96,27 @@
         GRAY   = 0
         RED    = 1
         GREEN  = 2
         YELLOW = 3
         BLUE   = 4
         PURPLE = 5
         CYAN   = 6
-        LIGHT_GRAY  = 7 
+        LIGHT_GRAY  = 7
         NORMAL = 8
         WHITE = 9
         csi = '\x1b['
         reset = '\x1b[0m'
 
         LEVEL_ID = {
             pyLogging.DEBUG: GREEN,
             pyLogging.INFO: WHITE,
             pyLogging.WARNING: YELLOW,
             pyLogging.CRITICAL: BLUE,
             pyLogging.ERROR: RED
-            }  
+            }
 
         def log_color( self, message, record) :
             if record.levelno in self.LEVEL_ID:
                 color = self.LEVEL_ID[record.levelno]
                 params = []
                 params.append(str(color + 30))
                 message = ''.join((self.csi, ';'.join(params),
@@ -129,15 +132,14 @@
 
 class Logger:
 
     """Class for logging to console, text file, XML."""
 
     def __init__( self ):
         """The Constructor."""
-        pass
         self.mytime = localtime()
         self.logfile = None
         self.debug = pyLogging.DEBUG
         self.info = pyLogging.INFO
         self.rootLogger = pyLogging.getLogger(__name__)
         self.rootLogger.setLevel(self.debug)
         self.ALWAYS_FLUSH = False
@@ -204,40 +206,40 @@
                 self.rootLogger.addHandler(self.logfile)
             except Exception:
                 self.disable()
 
     def set_always_flush( self, val ):
         self.ALWAYS_FLUSH = val
 
-    def log( self, text):
+    def log( self, text, level=pyLogging.INFO):
         """Sends plain text to logging."""
         if self.Results.get_current() is not None:
             self.Results.get_current().add_output(text)
         if self.LOG_TO_FILE: self._save_to_log_file( text )
         else:
             if self.rootLogger:
-                self.rootLogger.info(text)
+                self.rootLogger.log(level, text)
                 if self.ALWAYS_FLUSH: sys.stdout.flush()
             else:
                 print(text)
 
     def error( self, text ):
         """Logs an Error message"""
         text = "ERROR: " + text
-        self.rootLogger.error(text)
+        self.log(text, pyLogging.ERROR)
 
     def warn( self, text ):
         """Logs an Warning message"""
         text = "WARNING: " + text
-        self.rootLogger.warning(text)
+        self.log(text, pyLogging.WARNING)
 
     def verbose_log( self, text):
         """Logs an Verbose message"""
         if self.VERBOSE:
-            self.rootLogger.log(self.verbose, text )
+            self.log(text, self.verbose)
 
     def log_passed_check( self, text ):
         """Logs a Test as PASSED"""
         self.log_passed(text)
 
     def log_failed_check( self, text ):
         """Logs a Test as FAILED"""
@@ -262,94 +264,94 @@
     def log_not_applicable_check( self, text):
         """Logs a Test as Not Applicable"""
         self.log_not_applicable(text)
 
     def log_passed( self, text ):
         """Logs a passed message."""
         text = "[+] PASSED: " + text
-        self.rootLogger.debug(text)
+        self.log(text, pyLogging.DEBUG)
 
     def log_failed( self, text ):
         """Logs a failed message."""
         text = "[-] FAILED: " + text
-        self.rootLogger.error(text)
+        self.log(text, pyLogging.ERROR)
 
     def log_warning( self, text ):
         """Logs a Warning message"""
         text = "[!] WARNING: " + text
-        self.rootLogger.warning(text)
+        self.log(text, pyLogging.WARNING)
 
     def log_skipped( self, text ):
         """Logs a NOT IMPLEMENTED message."""
         text = "[*] NOT IMPLEMENTED: " + text
-        self.rootLogger.warning(text)
+        self.log(text, pyLogging.WARNING)
 
     def log_not_applicable(self, text):
         """Logs a NOT APPLICABLE message."""
         text = "[*] NOT APPLICABLE: " + text
-        self.rootLogger.warning(text)
+        self.log(text, pyLogging.WARNING)
 
     def log_heading( self, text ):
         """Logs a heading message."""
-        self.rootLogger.critical(text)
+        self.log(text, pyLogging.CRITICAL)
 
     def log_important( self, text ):
         """Logs a important message."""
         text = "[!] " + text
-        self.rootLogger.error(text)
+        self.log(text, pyLogging.ERROR)
 
     def log_result( self, text ):
         """Logs a result message."""
         text = "[+] " + text
-        self.rootLogger.debug(text)
+        self.log(text, pyLogging.DEBUG)
 
     def log_bad( self, text ):
         """Logs a bad message, so it calls attention in the information displayed."""
         text = "[-] " + text
-        self.rootLogger.error(text)
+        self.log(text, pyLogging.ERROR)
 
     def log_good( self, text ):
         """Logs a message, if colors available, displays in green."""
         text = "[+] " + text
-        self.rootLogger.debug(text)
+        self.log(text, pyLogging.DEBUG)
 
     def log_unknown( self, text ):
         """Logs a message with a question mark."""
         text = "[?] " + text
-        self.rootLogger.info(text)
+        self.log(text, pyLogging.INFO)
 
     def log_information( self, text):
         """Logs a message with information message"""
         text = "[#] INFORMATION: " + text
-        self.rootLogger.debug(text)
+        self.log(text, pyLogging.DEBUG)
 
     def start_test( self, test_name ):
         """Logs the start point of a Test"""
         text =        "[x][ =======================================================================\n"
         text = text + "[x][ Module: " + test_name + "\n"
         text = text + "[x][ ======================================================================="
-        self.rootLogger.critical(text)
+        self.log(text, pyLogging.CRITICAL)
 
     def start_module( self, module_name ):
         """Displays a banner for the module name provided."""
         text = "\n[*] running module: {}".format(module_name)
-        self.rootLogger.info(text)
+        self.log(text, pyLogging.INFO)
         if self.Results.get_current() is not None:
             self.Results.get_current().add_desc(module_name)
             self.Results.get_current().set_time()
 
 
     def end_module( self, module_name ):
         if self.Results.get_current() is not None:
             self.Results.get_current().set_time()
         #text = "\n[-] *** Done *** %s" % module_name
         #self._log(text, None, None)
 
     def _write_log( self, text, filename ):
-        self.rootLogger.log(self.info,text) #writes text to defined log file
+        self.rootLogger.log(self.info, text) #writes text to defined log file
         if self.ALWAYS_FLUSH:
             # not sure why flush doesn't work as excpected
             # self.logfile.flush()
             # close and re-open log file
             try:
                 self.logfile.close()
                 self.logfile = open( self.LOG_FILE_NAME, 'a+' )
@@ -377,97 +379,113 @@
     return _logger
 
 
 ##################################################################################
 # Hex dump functions
 ##################################################################################
 
-def dump_buffer( arr, length = 8 ):
-    """Dumps the buffer."""
-    tmp=[]
-    tmp_str=[]
-    i=1
-    for c in arr:
-        tmp+=["{:02x} ".format(ord(c))]
-        if c in string.whitespace or c not in string.printable:
-            ch = " "
+def hex_to_text( value ):
+    '''Generate text string based on bytestrings'''
+    text = binascii.unhexlify('{:x}'.format(value))[::-1]
+    if isinstance( text, str ):
+        return text   # Python 2.x
+    else:
+        return text.decode( 'latin-1' )   # Python 3.x
+
+
+def bytes2string( buffer, length=16 ):
+    '''Generate text string based on str with ASCII side panel'''
+    output       = []
+    num_string   = []
+    ascii_string = []
+    index        = 1
+    for c in buffer:
+        num_string += ['{:02X} '.format(ord(c))]
+        if ( not (c in string.printable) or (c in string.whitespace) ):
+            ascii_string += ['{}'.format(' ')]
         else:
-            ch = ord(c)
-        tmp_str+=["%c"%ch]
-        if i%length==0:
-            tmp+=["| "]
-            tmp+=tmp_str
-            tmp+=["\n"]
-            tmp_str=[]
-        i+=1
-    if 0 != len(arr)%length:
-        tmp+=[ (length - len(arr)%length) * 3*" " ]
-        tmp+=["| "]
-        tmp+=tmp_str
-        tmp+=["\n"]
-    return "".join(tmp)
+            ascii_string += ['{}'.format(c)]
+        if index%length == 0:
+            num_string += ['| ']
+            num_string += ascii_string
+            output.append( ''.join(num_string) )
+            ascii_string = []
+            num_string   = []
+        index += 1
+    if 0 != len(buffer)%length:
+        num_string += [ (length - len(buffer)%length) * 3*' ' ]
+        num_string += ['| ']
+        num_string += ascii_string
+        output.append( ''.join(num_string) )
+    return '\n'.join(output)
+
+
+def dump_buffer( arr, length = 8 ):
+    """Dumps the buffer (str) with ASCII"""
+    return bytes2string( arr, length )
+
 
 def print_buffer( arr, length = 16 ):
-    """Prints the buffer."""
-    tmp=[]
-    tmp_str=[]
-    i=1
-    for c in arr:
-        tmp+=["{:2x} ".format(ord(c))]
-        if (not c in string.printable) or (c in string.whitespace):
-            ch = " "
-        else:
-            ch = ord(c)
-        tmp_str+=["%c"%ch]
-        if i%length==0:
-            tmp+=["| "]
-            tmp+=tmp_str
-            tmp_s = "".join(tmp)
-            logger().log( tmp_s )
-            tmp_str=[]
-            tmp=[]
-        i+=1
+    """Prints the buffer (str) with ASCII"""
+    prt_str = bytes2string( arr, length )
+    logger().log( prt_str )
 
-    if 0 != len(arr)%length:
-        tmp+=[ (length - len(arr)%length) * 3*" " ]
-        tmp+=["| "]
-        tmp+=tmp_str
-        tmp_s = "".join(tmp)
-        logger().log( tmp_s )
 
-def print_buffer_bytes( arr, length = 16 ):
-    """Prints the buffer."""
-    tmp=[]
-    tmp_str=[]
-    i=1
+def dump_buffer_bytes( arr, length = 8):
+    """Dumps the buffer (bytes, bytearray) with ASCII"""
+    output       = []
+    num_string   = []
+    ascii_string = []
+    index        = 1
     for c in arr:
-        tmp+=["{:2x} ".format(c)]
-        if (not chr(c) in string.printable) or (chr(c) in string.whitespace):
-            ch = " "
+        num_string += ['{:02X} '.format(c)]
+        if ( not (chr(c) in string.printable) or (chr(c) in string.whitespace) ):
+            ascii_string += ['{}'.format(' ')]
         else:
-            ch = c
-        tmp_str+=["%c"%ch]
-        if i%length==0:
-            tmp+=["| "]
-            tmp+=tmp_str
-            tmp_s = "".join(tmp)
-            logger().log( tmp_s )
-            tmp_str=[]
-            tmp=[]
-        i+=1
-
+            ascii_string += [chr(c)]
+        if index%length == 0:
+            num_string += ['| ']
+            num_string += ascii_string
+            output.append( ''.join(num_string) )
+            ascii_string = []
+            num_string   = []
+        index += 1
     if 0 != len(arr)%length:
-        tmp+=[ (length - len(arr)%length) * 3*" " ]
-        tmp+=["| "]
-        tmp+=tmp_str
-        tmp_s = "".join(tmp)
-        logger().log( tmp_s )
+        num_string += [ (length - len(arr)%length) * 3*' ' ]
+        num_string += ['| ']
+        num_string += ascii_string
+        output.append( ''.join(num_string) )
+    return output
+    return '\n'.join(output)
+
+
+def print_buffer_bytes( arr, length = 16 ):
+    """Prints the buffer (bytes, bytearray) with ASCII"""
+    prt_str = dump_buffer_bytes( arr, length )
+    logger().log( prt_str )
 
 
 def pretty_print_hex_buffer( arr, length = 16 ):
+    """Prints the buffer (bytes, bytearray) in a grid"""
     _str = ["    _"]
     for n in range(length):
-        _str += ["%02X__" % n]
+        _str += ["{:02X}__".format(n)]
     for n in range(len(arr)):
         if n%length == 0: _str += ["\n{:02X} | ".format(n)]
         _str += ["{:02X}  ".format(arr[n])]
     logger().log( ''.join(_str) )
+
+
+def dump_data( data, length = 16 ):
+    """Dumps the buffer with ASCII"""
+    if isinstance( data, str ):
+        dump_buffer( data, length )
+    else:
+        dump_buffer_bytes( data, length )
+
+
+def print_data( data, length = 16 ):
+    """Prints the buffer with ASCII"""
+    if isinstance( data, str ):
+        print_buffer( data, length )
+    else:
+        print_buffer_bytes( data, length )
```

### Comparing `chipsec-1.4.4/chipsec/command.py` & `chipsec-1.5.1/chipsec/command.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/module.py` & `chipsec-1.5.1/chipsec/module.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -37,14 +37,25 @@
 class Module():
     def __init__(self,name):
         self.logger = chipsec.logger.logger()
         self.name = name
         self.module = None
         self.mod_obj = None
 
+    def __lt__(self, other):
+        return self.name < other.name
+
+    def __le__(self, other):
+        return self.name <= other.name
+    
+    def __gt__(self, other):
+        return self.name > other.name
+
+    def __ge__(self, other):
+        return self.name >= other.name
 
     def get_name(self):
         return self.name
 
     def do_import(self):
         loaded = False
         if not MODPATH_RE.match(self.get_name()):
```

### Comparing `chipsec-1.4.4/chipsec/helper/dal/dalhelper.py` & `chipsec-1.5.1/chipsec/helper/dal/dalhelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # CHIPSEC: Platform Security Assessment Framework
-# Copyright (c) 2010-2019, Intel Corporation
+# Copyright (c) 2010-2020, Intel Corporation
 #
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; Version 2.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -24,15 +24,14 @@
 Intel DFx Abstraction Layer (DAL) helper
 
 From the Intel(R) DFx Abstraction Layer Python* Command Line Interface User Guide
 
 """
 
 import struct
-import sys
 
 from chipsec.logger import logger
 import itpii
 from ctypes import *
 from chipsec.helper.basehelper import Helper
 
 SYSTEM_HALTED = True
@@ -134,26 +133,24 @@
         config_addr |= (bus & 0xFF) << 16
         config_addr |= (device & 0x1F) << 11
         config_addr |= (function & 0x07) << 8
         config_addr |= (offset & 0xFF) << 0
         return config_addr
 
     def read_pci_reg( self, bus, device, function, address, size ):
-        value = 0xFFFFFFFF
         ie_thread = self.find_thread()
         self.base.threads[ie_thread].dport(0xCF8, self.pci_addr(bus, device, function, address))
         value = (self.base.threads[ie_thread].dport(0xCFC) >> ((address % 4) * 8))
         if 1 == size:
             value &= 0xFF
         elif 2 == size:
             value &= 0xFFFF
         return value.ToUInt32()
 
     def write_pci_reg( self, bus, device, function, address, dword_value, size ):
-        old_value = 0xFFFFFFFF
         ie_thread = self.find_thread()
         self.base.threads[ie_thread].dport(0xCF8, self.pci_addr(bus, device, function, address))
         old_value = self.base.threads[ie_thread].dport(0xCFC)
         self.base.threads[ie_thread].dport(0xCFC, dword_value)
         return old_value
 
     #
@@ -169,30 +166,30 @@
         ptr = 0
         format = {1: 'B', 2: 'H', 4: 'L', 8:'Q'}
         while width >= 1 :
             while (length - ptr) >= width :
                 v = self.base.threads[self.find_thread()].mem(itpii.Address((phys_address + ptr),itpii.AddressType.physical), width)
                 struct.pack_into(format[width], out_buf, ptr, v.ToUInt64())
                 ptr += width
-            width = width / 2
+            width = width // 2
         return ''.join(out_buf)
 
     def write_physical_mem( self, phys_address, length, buf, bytewise=False ):
         if bytewise :
             width = 1
         else :
             width = 8
         ptr = 0
         format = {1: 'B', 2: 'H', 4: 'L', 8:'Q'}
         while width >= 1 :
             while (length - ptr) >= width :
                 v = struct.unpack_from(format[width], buf, ptr)
                 self.base.threads[self.find_thread()].mem(itpii.Address((phys_address + ptr),itpii.AddressType.physical), width, v[0])
                 ptr += width
-            width = width / 2
+            width = width // 2
         return
 
     def read_phys_mem( self, phys_address_hi, phys_address_lo, length ) :
         return self.read_physical_mem((phys_address_hi << 32) | phys_address_lo, length)
 
     def write_phys_mem( self, phys_address_hi, phys_address_lo, length, buf ) :
         self.write_physical_mem((phys_address_hi << 32) | phys_address_lo, length, buf)
@@ -400,15 +397,15 @@
         if logger().DEBUG: logger().error( '[DAL] API get_ACPI_SDT() is not supported' )
         return None, None
 
     def native_get_ACPI_table( self, table_name ):
         if logger().DEBUG: logger().error( '[DAL] API native_get_ACPI_table() is not supported' )
         return None
 
-    def get_ACPI_table( self ):
+    def get_ACPI_table( self, table_name ):
         if logger().DEBUG: logger().error( '[DAL] API get_ACPI_table() is not supported' )
         return None
 
     #
     # IOSF Message Bus access
     #
     def msgbus_send_read_message( self, mcr, mcrx ):
```

### Comparing `chipsec-1.4.4/chipsec/helper/dal/__init__.py` & `chipsec-1.5.1/chipsec/helper/dal/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/helper/basehelper.py` & `chipsec-1.5.1/chipsec/helper/basehelper.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/helper/oshelper.py` & `chipsec-1.5.1/chipsec/helper/oshelper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -15,45 +15,26 @@
 #along with this program; if not, write to the Free Software
 #Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
 #Contact information:
 #chipsec@intel.com
 #
 
-
-
-# -------------------------------------------------------------------------------
-#
-# CHIPSEC: Platform Hardware Security Assessment Framework
-# (c) 2010-2019 Intel Corporation
-#
-# -------------------------------------------------------------------------------
-
 """
 Abstracts support for various OS/environments, wrapper around platform specific code that invokes kernel driver
 """
 
 import os
-import fnmatch
 import re
 import errno
-import shutil
 import traceback
 import sys
 
 import chipsec.file
-from chipsec.logger import *
-from chipsec.helper.basehelper import Helper
-
-_importlib = True
-try:
-    import importlib
-
-except ImportError:
-    _importlib = False
+from chipsec.logger import logger
 
 avail_helpers = []
 
 ZIP_HELPER_RE = re.compile("^chipsec\/helper\/\w+\/\w+\.pyc$", re.IGNORECASE)
 def f_mod_zip(x):
     return ( x.find('__init__') == -1 and ZIP_HELPER_RE.match(x) )
 def map_modname_zip(x):
@@ -112,15 +93,15 @@
     def start(self, start_driver, driver_exists=None, to_file=None, from_file=False):
         if not to_file is None:
             from chipsec.helper.file.filehelper import FileCmds
             self.filecmds = FileCmds(to_file)
         if not driver_exists is None:
             for name in avail_helpers:
                 if name == driver_exists:
-                    self.helper = getattr(chiphelpers,helper).get_helper()
+                    self.helper = getattr(chiphelpers,name).get_helper()
         try:
             if not self.helper.create( start_driver ):
                 raise OsHelperError("failed to create OS helper",1)
             if not self.helper.start( start_driver, from_file ):
                 raise OsHelperError("failed to start OS helper",1)
         except Exception as msg:
             if logger().DEBUG: logger().log_bad(traceback.format_exc())
```

### Comparing `chipsec-1.4.4/chipsec/helper/file/filehelper.py` & `chipsec-1.5.1/chipsec/helper/file/filehelper.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/helper/file/__init__.py` & `chipsec-1.5.1/chipsec/helper/file/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/helper/linux/cores.c` & `chipsec-1.5.1/chipsec/helper/linux/cores.c`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/helper/linux/__init__.py` & `chipsec-1.5.1/chipsec/helper/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/helper/linux/linuxhelper.py` & `chipsec-1.5.1/chipsec/helper/linux/linuxhelper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -15,49 +15,40 @@
 #along with this program; if not, write to the Free Software
 #Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
 #Contact information:
 #chipsec@intel.com
 #
 
-# -------------------------------------------------------------------------------
-#
-# CHIPSEC: Platform Hardware Security Assessment Framework
-# (c) 2010-2018 Intel Corporation
-#
-# -------------------------------------------------------------------------------
-
 """
 Linux helper
 """
 
 import array
 import ctypes
 import errno
 import fcntl
 import fnmatch
 import mmap
 import os
-import os.path
 import platform
 import resource
 import struct
 import subprocess
 import sys
 import shutil
 
 from chipsec import defines
 from chipsec.helper.oshelper import OsHelperError, HWAccessViolationError, UnimplementedAPIError, UnimplementedNativeAPIError, get_tools_path
 from chipsec.helper.basehelper import Helper
-from chipsec.logger import logger, print_buffer
+from chipsec.logger import logger
 import chipsec.file
 from chipsec.hal.uefi_common import EFI_VARIABLE_NON_VOLATILE, EFI_VARIABLE_BOOTSERVICE_ACCESS, EFI_VARIABLE_RUNTIME_ACCESS
 from chipsec.hal.uefi_common import EFI_VARIABLE_HARDWARE_ERROR_RECORD, EFI_VARIABLE_AUTHENTICATED_WRITE_ACCESS
 from chipsec.hal.uefi_common import EFI_VARIABLE_TIME_BASED_AUTHENTICATED_WRITE_ACCESS, EFI_VARIABLE_APPEND_WRITE
-from chipsec.defines import bytestostring
 
 MSGBUS_MDR_IN_MASK  = 0x1
 MSGBUS_MDR_OUT_MASK = 0x2
 
 IOCTL_BASE                     = 0x0
 IOCTL_RDIO                     = 0x1
 IOCTL_WRIO                     = 0x2
@@ -160,21 +151,25 @@
                 if logger().DEBUG:
                     logger().log("Cannot find symbol 'phys_mem_access_prot'")
             else:
                 a2 = "a2=0x{}".format(phys_mem_access_prot)
 
         driver_path = os.path.join(chipsec.file.get_main_dir(), "chipsec", "helper" ,"linux", "chipsec.ko" )
         if not os.path.exists(driver_path):
-            #check DKMS modules location
-            try:
-                driver_path = self.get_dkms_module_location()
-            except Exception:
-                pass
+            driver_path += ".xz"
             if not os.path.exists(driver_path):
-                raise Exception("Cannot find chipsec.ko module")
+                #check DKMS modules location
+                try:
+                    driver_path = self.get_dkms_module_location()
+                except Exception:
+                    pass
+                if not os.path.exists(driver_path):
+                    driver_path += ".xz"
+                    if not os.path.exists(driver_path):
+                        raise Exception("Cannot find chipsec.ko module")
         try:
             subprocess.check_output( [ "insmod", driver_path, a1, a2 ] )
         except Exception as err:
             raise Exception("Could not start Linux Helper, are you running as Admin/root?\n\t{}.format(err)")
         uid = gid = 0
         os.chown(self.DEVICE_NAME, uid, gid)
         os.chmod(self.DEVICE_NAME, 600)
@@ -245,15 +240,14 @@
             self.dev_mem = os.open(self.DEV_MEM, os.O_RDWR)
             return True
         except IOError as err:
             raise OsHelperError("Unable to open /dev/mem.\n"
                                 "This command requires access to /dev/mem.\n"
                                 "Are you running this command as root?\n"
                                 "{}".format(str(err)), err.errno)
-        return False
 
 
     def devport_available(self):
         """Check if /dev/port is usable.
 
            In case the driver is not loaded, we might be able to perform the
            requested operation via /dev/port. Returns True if /dev/port is
@@ -457,15 +451,14 @@
     def load_ucode_update( self, cpu_thread_id, ucode_update_buf):
         cpu_ucode_thread_id = ctypes.c_int(cpu_thread_id)
 
         in_buf = struct.pack('=BH', cpu_thread_id, len(ucode_update_buf)) + ucode_update_buf
         in_buf_final = array.array("c", in_buf)
         #print_buffer(in_buf)
         out_length=0
-        out_buf=(ctypes.c_char * out_length)()
         try:
             out_buf = self.ioctl(IOCTL_LOAD_UCODE_PATCH, in_buf_final)
         except IOError:
             if logger().DEBUG: logger().error("IOError IOCTL Load Patch\n")
             return None
 
         return True
@@ -619,15 +612,15 @@
 
     def get_ACPI_SDT( self ):
         raise UnimplementedAPIError( "get_ACPI_SDT" )
     # @TODO: implement ACPI access in native mode through file system
     def native_get_ACPI_table( self ):
         raise UnimplementedNativeAPIError( "native_get_ACPI_table" )
     # ACPI access is implemented through ACPI HAL rather than through kernel module
-    def get_ACPI_table( self ):
+    def get_ACPI_table( self, table_name ):
         raise UnimplementedAPIError( "get_ACPI_table" )
 
     #
     # IOSF Message Bus access
     #
     def msgbus_send_read_message( self, mcr, mcrx ):
         mdr_out = 0
@@ -668,15 +661,15 @@
             f = open('/proc/cpuinfo', 'r')
             for line in f:
                 if "processor" in line:
                     numCpus += 1
             f.close()
         except:
             numCpus = 1;
-            pass
+
         errno = ctypes.c_int( 0 )
         if 0 == CORES.getaffinity( numCpus,ctypes.byref( mask ),ctypes.byref( errno ) ):
             AffinityString = " GetAffinity: "
             for i in range( 0, numCpus ):
                 if mask[i] == 1:
                     AffinityString += "{} ".format(i)
             if logger().DEBUG: logger().log( AffinityString )
@@ -799,15 +792,14 @@
     def kern_get_EFI_variable(self, name, guid):
         (off, buf, hdr, data, guid, attr) = self.kern_get_EFI_variable_full(name, guid)
         return data
 
     def kern_list_EFI_variables(self):
         varlist = []
         off = 0
-        buf = list()
         hdr = 0
         attr = 0
         try:
             if os.path.isdir('/sys/firmware/efi/efivars'):
                 varlist = os.listdir('/sys/firmware/efi/efivars')
             elif os.path.isdir('/sys/firmware/efi/vars'):
                 varlist = os.listdir('/sys/firmware/efi/vars')
@@ -1169,12 +1161,12 @@
             return False
         return True
 
     #
     # Logical CPU count
     #
     def get_threads_count ( self ):
-        import subprocess
-        return int(subprocess.check_output("grep -c process /proc/cpuinfo", shell=True))
+        import multiprocessing
+        return multiprocessing.cpu_count()
 
 def get_helper():
     return LinuxHelper()
```

### Comparing `chipsec-1.4.4/chipsec/helper/win/win32helper.py` & `chipsec-1.5.1/chipsec/helper/win/win32helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -15,57 +15,45 @@
 #along with this program; if not, write to the Free Software
 #Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
 #Contact information:
 #chipsec@intel.com
 #
 
-
-
-
-# -------------------------------------------------------------------------------
-#
-# CHIPSEC: Platform Hardware Security Assessment Framework
-# (c) 2010-2019 Intel Corporation
-#
-# -------------------------------------------------------------------------------
-
 """
 Management and communication with Windows kernel mode driver which provides access to hardware resources
 
-.. note:: 
+.. note::
     On Windows you need to install pywin32 Python extension corresponding to your Python version:
     http://sourceforge.net/projects/pywin32/
 """
 
 import os.path
 import struct
 import sys
 import platform
-import re
 import errno
-import traceback
-import time
 import shutil
-from threading import Lock
 from collections import namedtuple
 from ctypes import *
 import subprocess
+import codecs
 
 import pywintypes
 import win32service #win32serviceutil, win32api, win32con
 import winerror
 from win32file import FILE_SHARE_READ, FILE_SHARE_WRITE, OPEN_EXISTING, FILE_ATTRIBUTE_NORMAL, FILE_FLAG_OVERLAPPED, INVALID_HANDLE_VALUE
 import win32api, win32process, win32security, win32file, win32serviceutil
 
-from chipsec.helper.oshelper import OsHelperError, HWAccessViolationError, UnimplementedAPIError, UnimplementedNativeAPIError, get_tools_path
+from chipsec.helper.oshelper import OsHelperError, HWAccessViolationError, UnimplementedAPIError, UnimplementedNativeAPIError
 from chipsec.helper.basehelper import Helper
-from chipsec.logger import logger, print_buffer
+from chipsec.logger import logger
 import chipsec.file
-import chipsec.defines
+from chipsec.defines import bytestostring
+from chipsec.hal.uefi_common import EFI_GUID
 
 
 class PCI_BDF(Structure):
     _fields_ = [("BUS",  c_ushort, 16),  # Bus
                 ("DEV",  c_ushort, 16),  # Device
                 ("FUNC", c_ushort, 16),  # Function
                 ("OFF",  c_ushort, 16)]  # Offset
@@ -171,47 +159,44 @@
 PyLong_AsByteArray.argtypes = [py_object,
                                c_char_p,
                                c_size_t,
                                c_int,
                                c_int]
 
 def packl_ctypes( lnum, bitlength ):
-    length = (bitlength + 7)/8
+    if sys.version_info.major == 2:
+        lnum = long(lnum)
+    length = (bitlength + 7)//8
     a = create_string_buffer( length )
     PyLong_AsByteArray(lnum, a, len(a), 1, 1) # 4th param is for endianness 0 - big, non 0 - little
     return a.raw
 
 #
 # Firmware Table Provider Signatures
 #
 FirmwareTableProviderSignature_ACPI = 0x41435049 # 'ACPI' - The ACPI firmware table provider
 FirmwareTableProviderSignature_FIRM = 0x4649524D # 'FIRM' - The raw firmware table provider
 FirmwareTableProviderSignature_RSMB = 0x52534D42 # 'RSMB' - The raw SMBIOS firmware table provider
 
 FirmwareTableID_RSDT = 0x54445352
 FirmwareTableID_XSDT = 0x54445358
 
-#
-# Windows 8 NtEnumerateSystemEnvironmentValuesEx (infcls = 2)
-#
-def guid_str(guid0, guid1, guid2, guid3):
-    return ( "{:08X}-{:04X}-{:04X}-{:4}-{:6}".format(guid0, guid1, guid2, guid3[:2].encode('hex').upper(), guid3[-6::].encode('hex').upper()) )
 
 class EFI_HDR_WIN( namedtuple('EFI_HDR_WIN', 'Size DataOffset DataSize Attributes guid0 guid1 guid2 guid3') ):
     __slots__ = ()
     def __str__(self):
         return """
 Header (Windows)
 ----------------
 VendorGuid= {{{:08X}-{:04X}-{:04X}-{:4}-{:6}}}
 Size      = 0x{:08X}
 DataOffset= 0x{:08X}
 DataSize  = 0x{:08X}
 Attributes= 0x{:08X}
-""".format( self.guid0, self.guid1, self.guid2, self.guid3[:2].encode('hex').upper(), self.guid3[-6::].encode('hex').upper(), self.Size, self.DataOffset, self.DataSize, self.Attributes )
+""".format( self.guid0, self.guid1, self.guid2, bytestostring(codecs.encode(self.guid3[:2],'hex')).upper(), bytestostring(codecs.encode(self.guid3[-6::],'hex')).upper(), self.Size, self.DataOffset, self.DataSize, self.Attributes )
 
 def getEFIvariables_NtEnumerateSystemEnvironmentValuesEx2( nvram_buf ):
     start = 0
     buffer = nvram_buf
     bsize = len(buffer)
     header_fmt = "<IIIIIHH8s"
     header_size = struct.calcsize( header_fmt )
@@ -231,15 +216,15 @@
             efi_var_name = unicode(s, "utf-16-le", errors="replace").split(u'\u0000')[0]
         else:
             efi_var_name = str(s, "utf-16-le", errors="replace").split(u'\u0000')[0]
 
         if efi_var_name not in variables.keys():
             variables[efi_var_name] = []
         #                                off, buf,         hdr,         data,         guid,                                                                                 attrs
-        variables[efi_var_name].append( (off, efi_var_buf, efi_var_hdr, efi_var_data, guid_str(efi_var_hdr.guid0, efi_var_hdr.guid1, efi_var_hdr.guid2, efi_var_hdr.guid3), efi_var_hdr.Attributes) )
+        variables[efi_var_name].append( (off, efi_var_buf, efi_var_hdr, efi_var_data, EFI_GUID(efi_var_hdr.guid0, efi_var_hdr.guid1, efi_var_hdr.guid2, efi_var_hdr.guid3), efi_var_hdr.Attributes) )
 
         if 0 == efi_var_hdr.Size: break
         off = next_var_offset
 
     return variables
 #    return ( start, next_var_offset, efi_var_buf, efi_var_hdr, efi_var_name, efi_var_data, guid_str(efi_var_hdr.guid0, efi_var_hdr.guid1, efi_var_hdr.guid2, efi_var_hdr.guid3), efi_var_hdr.Attributes )
 
@@ -255,15 +240,14 @@
 
     decompression_oder_type1 = [chipsec.defines.COMPRESSION_TYPE_TIANO,chipsec.defines.COMPRESSION_TYPE_UEFI]
     decompression_oder_type2 = [chipsec.defines.COMPRESSION_TYPE_TIANO,chipsec.defines.COMPRESSION_TYPE_UEFI,chipsec.defines.COMPRESSION_TYPE_LZMA,chipsec.defines.COMPRESSION_TYPE_BROTLI]
 
     def __init__(self):
         super(Win32Helper, self).__init__()
 
-        import platform, os
         self.os_system  = platform.system()
         self.os_release = platform.release()
         self.os_version = platform.version()
         self.os_machine = platform.machine()
         self.os_uname   = platform.uname()
         self.name       = "Win32Helper"
         if "windows" == self.os_system.lower():
@@ -290,42 +274,38 @@
             self.GetFirmwareEnvironmentVariable.restype = c_int
             self.GetFirmwareEnvironmentVariable.argtypes = [c_wchar_p, c_wchar_p, c_void_p, c_int]
             self.SetFirmwareEnvironmentVariable = kernel32.SetFirmwareEnvironmentVariableW
             self.SetFirmwareEnvironmentVariable.restype = c_int
             self.SetFirmwareEnvironmentVariable.argtypes = [c_wchar_p, c_wchar_p, c_void_p, c_int]
         except AttributeError as msg:
             logger().warn( "G[S]etFirmwareEnvironmentVariableW function doesn't seem to exist" )
-            pass
 
         try:
             self.NtEnumerateSystemEnvironmentValuesEx = windll.ntdll.NtEnumerateSystemEnvironmentValuesEx
             self.NtEnumerateSystemEnvironmentValuesEx.restype = c_int
             self.NtEnumerateSystemEnvironmentValuesEx.argtypes = [c_int, c_void_p, c_void_p]
         except AttributeError as msg:
             logger().warn( "NtEnumerateSystemEnvironmentValuesEx function doesn't seem to exist" )
-            pass
 
         try:
             self.GetFirmwareEnvironmentVariableEx = kernel32.GetFirmwareEnvironmentVariableExW
             self.GetFirmwareEnvironmentVariableEx.restype = c_int
             self.GetFirmwareEnvironmentVariableEx.argtypes = [c_wchar_p, c_wchar_p, c_void_p, c_int, c_int_p]
             self.SetFirmwareEnvironmentVariableEx = kernel32.SetFirmwareEnvironmentVariableExW
             self.SetFirmwareEnvironmentVariableEx.restype = c_int
             self.SetFirmwareEnvironmentVariableEx.argtypes = [c_wchar_p, c_wchar_p, c_void_p, c_int, c_int]
         except AttributeError as msg:
             if logger().DEBUG: logger().warn( "G[S]etFirmwareEnvironmentVariableExW function doesn't seem to exist" )
-            pass
 
         try:
             self.GetSystemFirmwareTbl = kernel32.GetSystemFirmwareTable
             self.GetSystemFirmwareTbl.restype = c_int
             self.GetSystemFirmwareTbl.argtypes = [c_int, c_int, c_void_p, c_int]
         except AttributeError as msg:
             logger().warn( "GetSystemFirmwareTable function doesn't seem to exist" )
-            pass
 
         try:
             self.EnumSystemFirmwareTbls = kernel32.EnumSystemFirmwareTables 
             self.EnumSystemFirmwareTbls.restype = c_int
             self.EnumSystemFirmwareTbls.argtypes = [c_int, c_void_p, c_int]
         except AttributeError as msg:
             logger().warn( "GetSystemFirmwareTable function doesn't seem to exist" )
@@ -405,15 +385,15 @@
         finally:
             win32service.CloseServiceHandle( hs )
             win32service.CloseServiceHandle( hscm )
 
         return True
 
     #
-    # Remove (detele/unregister/uninstall) chipsec service
+    # Remove (delete/unregister/uninstall) chipsec service
     #
     def delete( self, start_driver ):
         if not start_driver: return True
         if self.use_existing_service: return True
 
         if win32serviceutil.QueryServiceStatus( SERVICE_NAME )[1] != win32service.SERVICE_STOPPED:
             logger().warn( "cannot delete service '{}' (not stopped)".format(SERVICE_NAME) )
@@ -545,36 +525,33 @@
 
 ###############################################################################################
 # Actual driver IOCTL functions to access HW resources
 ###############################################################################################
 
     def read_phys_mem( self, phys_address_hi, phys_address_lo, length ):
         out_length = length
-        out_buf = (c_char * out_length)()
         in_buf = struct.pack( '3I', phys_address_hi, phys_address_lo, length )
         out_buf = self._ioctl( IOCTL_READ_PHYSMEM, in_buf, out_length )
         return out_buf
 
     def native_read_phys_mem( self, phys_address_hi, phys_address_lo, length ):
         raise UnimplementedNativeAPIError( "native_read_phys_mem" )
 
     def write_phys_mem( self, phys_address_hi, phys_address_lo, length, buf ):
         in_length = length + 12
-        out_buf = (c_char * 4)()
         in_buf = struct.pack( '3I', phys_address_hi, phys_address_lo, length ) + buf
         out_buf = self._ioctl( IOCTL_WRITE_PHYSMEM, in_buf, 4 )
         return out_buf
 
     def native_write_phys_mem( self, phys_address_hi, phys_address_lo, length, buf ):
         raise UnimplementedNativeAPIError( "native_write_phys_mem" )
 
     # @TODO: Temporarily the same as read_phys_mem for compatibility 
     def read_mmio_reg( self, phys_address, size ):
         out_size = size
-        out_buf = (c_char * out_size)()
         in_buf = struct.pack( '3I', (phys_address>>32)&0xFFFFFFFF, phys_address&0xFFFFFFFF, size )
         out_buf = self._ioctl( IOCTL_READ_PHYSMEM, in_buf, out_size )
         if size == 8:
             value = struct.unpack( '=Q', out_buf )[0]
         elif size == 4:
             value = struct.unpack( '=I', out_buf )[0]
         elif size == 2:
@@ -588,28 +565,25 @@
         elif size == 4: buf = struct.pack( '=I', value&0xFFFFFFFF )
         elif size == 2: buf = struct.pack( '=H', value&0xFFFF )
         elif size == 1: buf = struct.pack( '=B', value&0xFF )
         else: return False
         return self.write_phys_mem( ((phys_address>>32)&0xFFFFFFFF), (phys_address&0xFFFFFFFF), size, buf )
 
     def alloc_phys_mem( self, length, max_pa ):
-        (va, pa) = (0,0)
         in_length  = 12
         out_length = 16
-        out_buf = (c_char * out_length)()
         in_buf = struct.pack( 'QI', max_pa, length )
         out_buf = self._ioctl( IOCTL_ALLOC_PHYSMEM, in_buf, out_length )
         (va, pa) = struct.unpack( '2Q', out_buf )
         return (va, pa)
 
     def va2pa( self, va ):
         error_code = 0
         in_length  = 8
         out_length = 8
-        out_buf = (c_char * out_length)()
         in_buf = struct.pack( 'Q', va )
         out_buf = self._ioctl( IOCTL_GET_PHYSADDR, in_buf, out_length )
         pa = struct.unpack( 'Q', out_buf )[0]
         return (pa,error_code)
 
     #
     # HYPERCALL
@@ -617,75 +591,67 @@
     def hypercall( self, rcx, rdx, r8, r9, r10, r11, rax, rbx, rdi, rsi, xmm_buffer ):
         if self.os_machine == 'AMD64':
             arg_type = 'Q'
             out_length = 8
         else:
             arg_type = 'I'
             out_length = 4
-        out_buf = (c_char * out_length)()
         in_buf  = struct.pack( '<11' + arg_type, rcx, rdx, r8, r9, r10, r11, rax, rbx, rdi, rsi, xmm_buffer )
         out_buf = self._ioctl( IOCTL_HYPERCALL, in_buf, out_length )
         return struct.unpack( '<' + arg_type, out_buf )[0]
 
     #
     # MAP_IO_SPACE
     #
     def map_io_space( self, physical_address, length, cache_type ):
         out_length = 8
-        out_buf = (c_char * out_length)()
         in_buf  = struct.pack( '<3Q', physical_address, length, cache_type )
         out_buf = self._ioctl( IOCTL_MAP_IO_SPACE, in_buf, out_length )
         virtual_address = struct.unpack( '<Q', out_buf )[0]
         return virtual_address
 
     #
     # FREE_PHYS_MEM
     #
     def free_phys_mem( self, physical_address ):
         out_length = 8
-        out_buf = (c_char * out_length)()
         in_buf  = struct.pack( '<Q', physical_address )
         out_buf = self._ioctl( IOCTL_FREE_PHYSMEM, in_buf, out_length )
         return
 
     def read_msr( self, cpu_thread_id, msr_addr ):
-        (eax,edx) = (0,0)
         out_length = 8
-        out_buf = (c_char * out_length)()
         in_buf = struct.pack( '=2I', cpu_thread_id, msr_addr )
         out_buf = self._ioctl( IOCTL_RDMSR, in_buf, out_length )
         (eax, edx) = struct.unpack( '2I', out_buf )
         return (eax, edx)
 
     def write_msr( self, cpu_thread_id, msr_addr, eax, edx ):
         out_length = 0
         out_buf = (c_char * out_length)()
         in_buf = struct.pack( '=4I', cpu_thread_id, msr_addr, eax, edx )
         out_buf = self._ioctl( IOCTL_WRMSR, in_buf, out_length )
         return
 
     def read_pci_reg( self, bus, device, function, address, size ):
-        value = 0xFFFFFFFF
         bdf = PCI_BDF( bus&0xFFFF, device&0xFFFF, function&0xFFFF, address&0xFFFF )
         out_length = size
-        out_buf = (c_char * out_length)()
         in_buf = struct.pack( '4HB', bdf.BUS, bdf.DEV, bdf.FUNC, bdf.OFF, size )
         out_buf = self._ioctl( READ_PCI_CFG_REGISTER, in_buf, out_length )
         if 1 == size:
             value = struct.unpack( 'B', out_buf )[0]
         elif 2 == size:
             value = struct.unpack( 'H', out_buf )[0]
         else:
             value = struct.unpack( 'I', out_buf )[0]
         return value
 
     def write_pci_reg( self, bus, device, function, address, value, size ):
         bdf = PCI_BDF( bus&0xFFFF, device&0xFFFF, function&0xFFFF, address&0xFFFF )
         out_length = 0
-        out_buf = (c_char * out_length)()
         in_buf = struct.pack( '4HIB', bdf.BUS, bdf.DEV, bdf.FUNC, bdf.OFF, value, size )
         out_buf = self._ioctl( WRITE_PCI_CFG_REGISTER, in_buf, out_length )
         return True
 
     def load_ucode_update( self, cpu_thread_id, ucode_update_buf ):
         in_length = len(ucode_update_buf) + 3
         out_length = 0
@@ -773,15 +739,15 @@
         (status, data, attributes) = self.get_EFI_variable_full( name, guid, attrs )
         return data
 
     def set_EFI_variable( self, name, guid, data, datasize, attrs ):
         var     = bytes(0) if data     is None else data
         var_len = len(var) if datasize is None else datasize
         if isinstance(attrs, (str,bytes)):
-            attrs = struct.unpack("Q","{messge:\x00<{fill}}".format(message=attrs,fill=8)[:8])[0]
+            attrs = struct.unpack("Q","{message:\x00<{fill}}".format(message=attrs,fill=8)[:8])[0]
 
         if attrs is None:
             if self.SetFirmwareEnvironmentVariable is not None:
                 if logger().DEBUG: logger().log( "[helper] -> SetFirmwareEnvironmentVariable( name='{}', GUID='{}', length=0x{:X} )..".format(name, "{{{}}}".format(guid), var_len) )
                 ntsts = self.SetFirmwareEnvironmentVariable( name, "{{{}}}".format(guid), var, var_len )
         else:
             if self.SetFirmwareEnvironmentVariableEx is not None:
@@ -797,39 +763,46 @@
 
     def delete_EFI_variable(self, name, guid):
         return self.set_EFI_variable( name, guid, None, datasize=0, attrs=None )
 
     def list_EFI_variables( self, infcls=2 ):
         if logger().DEBUG: logger().log( '[helper] -> NtEnumerateSystemEnvironmentValuesEx( infcls={:d} )..'.format(infcls) )
         efi_vars = create_string_buffer( EFI_VAR_MAX_BUFFER_SIZE )
-        length = packl_ctypes( long(EFI_VAR_MAX_BUFFER_SIZE), 32 )
+        length = packl_ctypes( EFI_VAR_MAX_BUFFER_SIZE, 32 )
         status = self.NtEnumerateSystemEnvironmentValuesEx( infcls, efi_vars, length )
         status = ( ((1 << 32) - 1) & status)
         if (0xC0000023 == status):
             retlength, = struct.unpack("<I", length)
             efi_vars = create_string_buffer( retlength )
             status = self.NtEnumerateSystemEnvironmentValuesEx( infcls, efi_vars, length )
         elif (0xC0000002 == status):
             if logger().DEBUG: logger().warn( 'NtEnumerateSystemEnvironmentValuesEx was not found (NTSTATUS = 0xC0000002)' )
             if logger().DEBUG: logger().log( '[*] Your Windows does not expose UEFI Runtime Variable API. It was likely installed as legacy boot.\nTo use UEFI variable functions, chipsec needs to run in OS installed with UEFI boot (enable UEFI Boot in BIOS before installing OS)' )
             return None
         if 0 != status:
-            if logger().DEBUG:
-                logger().error( 'NtEnumerateSystemEnvironmentValuesEx failed (GetLastError = 0x{:X})'.format(kernel32.GetLastError()) )
-                logger().error( '*** NTSTATUS: {:08X}'.format( ((1 << 32) - 1) & status) )
-            raise WinError()
+            lasterror = kernel32.GetLastError()
+            if (0xC0000001 == status and lasterror == 0x000003E6): # ERROR_NOACCESS: Invalid access to memory location.  https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-erref/18d8fbe8-a967-4f1c-ae50-99ca8e491d2d
+                if logger().DEBUG: logger().warn( 'NtEnumerateSystemEnvironmentValuesEx was not successful (NTSTATUS = 0xC0000001)' )
+                if logger().DEBUG: logger().log( '[*] Your Windows has restricted access to UEFI variables.\nTo use UEFI variable functions, chipsec needs to run in an older version of windows or in a different environment' )
+                return None
+            else:
+                if logger().DEBUG:
+                    logger().error( 'NtEnumerateSystemEnvironmentValuesEx failed (GetLastError = 0x{:X})'.format(lasterror) )
+                    logger().error( '*** NTSTATUS: {:08X}'.format(status) )
+                raise WinError()
         if logger().DEBUG: logger().log( '[helper] len(efi_vars) = 0x{:X} (should be 0x20000)'.format(len(efi_vars)) )
         return getEFIvariables_NtEnumerateSystemEnvironmentValuesEx2( efi_vars )
 
     #
     # Interrupts
     #
     def send_sw_smi( self, cpu_thread_id, SMI_code_data, _rax, _rbx, _rcx, _rdx, _rsi, _rdi ):
+        if (sys.maxsize < 2**32 and self.os_machine == 'AMD64') or (sys.maxsize > 2**32 and self.os_machine == 'i386'):
+            logger().log("[helper] Python architecture must match OS architecture.  Run with {} architecture of python".format(self.os_machine))
         out_length = struct.calcsize(_smi_msg_t_fmt)
-        out_buf = (c_char * out_length)()
         out_size = c_ulong(out_length)
         in_buf = struct.pack( _smi_msg_t_fmt, SMI_code_data, _rax, _rbx, _rcx, _rdx, _rsi, _rdi )
         out_buf = self._ioctl( IOCTL_SWSMI, in_buf, out_length )
         if out_buf:
             ret = struct.unpack( _smi_msg_t_fmt, out_buf)
         else:
             ret = None
@@ -868,15 +841,14 @@
             raise ValueError(e)
 
     #
     # CPUID
     #
     def cpuid( self, eax, ecx ):
         out_length = 16
-        out_buf = (c_char * out_length)()
         in_buf = struct.pack( '=2I', eax, ecx )
         out_buf = self._ioctl( IOCTL_CPUID, in_buf, out_length )
         (eax, ebx, ecx, edx) = struct.unpack( '4I', out_buf )
         return (eax, ebx, ecx, edx)
 
 
     def get_ACPI_SDT( self ):
@@ -895,15 +867,15 @@
         if retVal > table_size:
             table_size = retVal
             tBuffer    = create_string_buffer( table_size )
             retVal     = self.GetSystemFirmwareTbl( FirmwareTableProviderSignature_ACPI, tbl, tBuffer, table_size )
         return tBuffer[:retVal]
 
     # ACPI access is implemented through ACPI HAL rather than through kernel module
-    def get_ACPI_table( self ):
+    def get_ACPI_table( self, table_name ):
         raise UnimplementedAPIError( "get_ACPI_table" )
 
 
 
     #
     # IOSF Message Bus access
     #
```

### Comparing `chipsec-1.4.4/chipsec/helper/win/__init__.py` & `chipsec-1.5.1/chipsec/helper/win/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/helper/rwe/rwehelper.py` & `chipsec-1.5.1/chipsec/helper/rwe/rwehelper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -14,54 +14,44 @@
 #along with this program; if not, write to the Free Software
 #Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
 #Contact information:
 #chipsec@intel.com
 #
 
-# -------------------------------------------------------------------------------
-#
-# CHIPSEC: Platform Hardware Security Assessment Framework
-# (c) 2010-2018 Intel Corporation
-#
-# -------------------------------------------------------------------------------
-
 """
 Management and communication with Windows kernel mode driver which provides access to hardware resources
 
 .. note::
     On Windows you need to install pywin32 Python extension corresponding to your Python version:
     http://sourceforge.net/projects/pywin32/
 """
 
 import os.path
 import struct
 import sys
 import platform
-import re
 import errno
 import traceback
-import time
-from threading import Lock
 from collections import namedtuple
 from ctypes import *
 import shutil
 
 import pywintypes
 import win32service #win32serviceutil, win32api, win32con
 import winerror
 from win32file import FILE_SHARE_READ, FILE_SHARE_WRITE, OPEN_EXISTING, FILE_ATTRIBUTE_NORMAL, FILE_FLAG_OVERLAPPED, INVALID_HANDLE_VALUE
 import win32api, win32process, win32security, win32file, win32serviceutil
 
 from chipsec.helper.oshelper import OsHelperError, HWAccessViolationError, UnimplementedAPIError, UnimplementedNativeAPIError, get_tools_path
 from chipsec.helper.basehelper import Helper
 from chipsec.logger import logger, print_buffer
 import chipsec.file
-import chipsec.defines
-
+from chipsec.defines import bytestostring
+from chipsec.hal.uefi_common import EFI_GUID
 
 class PCI_BDF(Structure):
     _fields_ = [("BUS",  c_ushort, 16),  # Bus
                 ("DEV",  c_ushort, 16),  # Device
                 ("FUNC", c_ushort, 16),  # Function
                 ("OFF",  c_ushort, 16)]  # Offset
 
@@ -163,15 +153,15 @@
 PyLong_AsByteArray.argtypes = [py_object,
                                c_char_p,
                                c_size_t,
                                c_int,
                                c_int]
 
 def packl_ctypes( lnum, bitlength ):
-    length = (bitlength + 7)/8
+    length = (bitlength + 7)//8
     a = create_string_buffer( length )
     PyLong_AsByteArray(lnum, a, len(a), 1, 1) # 4th param is for endianness 0 - big, non 0 - little
     return a.raw
 
 #
 # Firmware Table Provider Signatures
 #
@@ -215,20 +205,23 @@
         next_var_offset = off + efi_var_hdr.Size
         efi_var_buf     = buffer[ off : next_var_offset ]
         efi_var_data    = buffer[ off + efi_var_hdr.DataOffset : off + efi_var_hdr.DataOffset + efi_var_hdr.DataSize ]
 
         #efi_var_name = "".join( buffer[ start + header_size : start + efi_var_hdr.DataOffset ] ).decode('utf-16-le')
         str_fmt = "{:d}s".format(efi_var_hdr.DataOffset - header_size)
         s, = struct.unpack( str_fmt, buffer[ off + header_size : off + efi_var_hdr.DataOffset ] )
-        efi_var_name = unicode(s, "utf-16-le", errors="replace").split(u'\u0000')[0]
+        if sys.version_info[0] < 3:
+            efi_var_name = unicode(s, "utf-16-le", errors="replace").split(u'\u0000')[0]
+        else:
+            efi_var_name = str(s, "utf-16-le", errors="replace").split(u'\u0000')[0]
 
         if efi_var_name not in variables.keys():
             variables[efi_var_name] = []
         #                                off, buf,         hdr,         data,         guid,                                                                                 attrs
-        variables[efi_var_name].append( (off, efi_var_buf, efi_var_hdr, efi_var_data, guid_str(efi_var_hdr.guid0, efi_var_hdr.guid1, efi_var_hdr.guid2, efi_var_hdr.guid3), efi_var_hdr.Attributes) )
+        variables[efi_var_name].append( (off, efi_var_buf, efi_var_hdr, efi_var_data, EFI_GUID(efi_var_hdr.guid0, efi_var_hdr.guid1, efi_var_hdr.guid2, efi_var_hdr.guid3), efi_var_hdr.Attributes) )
 
         if 0 == efi_var_hdr.Size: break
         off = next_var_offset
 
     return variables
 #    return ( start, next_var_offset, efi_var_buf, efi_var_hdr, efi_var_name, efi_var_data, guid_str(efi_var_hdr.guid0, efi_var_hdr.guid1, efi_var_hdr.guid2, efi_var_hdr.guid3), efi_var_hdr.Attributes )
 
@@ -238,16 +231,16 @@
     _handle_error( ("{} failed: {} ({:d})".format(fn, msg, hr)), hr )
 def _handle_error( err, hr=0 ):
     logger().error( err )
     raise OsHelperError( err, hr )
 
 
 _tools = {
-  chipsec.defines.ToolType.TIANO_COMPRESS: 'TianoCompress.exe',
-  chipsec.defines.ToolType.LZMA_COMPRESS : 'LzmaCompress.exe'
+  chipsec.defines.COMPRESSION_TYPE_TIANO: 'TianoCompress.exe',
+  chipsec.defines.COMPRESSION_TYPE_LZMA : 'LzmaCompress.exe'
 }
 
 class RweHelper(Helper):
 
     def __init__(self):
         super(RweHelper, self).__init__()
 
@@ -263,26 +256,27 @@
             if ("5" == self.os_release): win_ver = "winxp"
             if logger().DEBUG: logger().log( "[helper] OS: {} {} {}".format(self.os_system, self.os_release, self.os_version) )
 
         self.use_existing_service = False
 
         self.win_ver        = win_ver
         self.driver_handle  = None
-        self.device_file    = pywintypes.Unicode(DEVICE_FILE)
+        self.device_file    = str(DEVICE_FILE)
 
         # check DRIVER_FILE_PATHS for the DRIVER_FILE_NAME
         self.driver_path    = None
         for path in DRIVER_FILE_PATHS:
             driver_path = os.path.join(path, DRIVER_FILE_NAME)
             if os.path.isfile(driver_path): 
                 self.driver_path = driver_path
                 if logger().DEBUG: logger().log("[helper] found driver in {}".format(driver_path))
         if self.driver_path is None: 
-            if logger().DEBUG: logger().log("[helper] RWE Driver Not Found")
-            raise DriverNotFound
+            if logger().DEBUG:
+                logger().log("[helper] RWE Driver Not Found")
+            raise Exception("RWE Driver Not Found")
 
         c_int_p = POINTER(c_int)
 
         # enable required SeSystemEnvironmentPrivilege privilege
         privilege = win32security.LookupPrivilegeValue( None, 'SeSystemEnvironmentPrivilege' )
         token = win32security.OpenProcessToken( win32process.GetCurrentProcess(), win32security.TOKEN_READ|win32security.TOKEN_ADJUST_PRIVILEGES )
         win32security.AdjustTokenPrivileges( token, False, [(privilege, win32security.SE_PRIVILEGE_ENABLED)] )
@@ -293,42 +287,38 @@
             self.GetFirmwareEnvironmentVariable.restype = c_int
             self.GetFirmwareEnvironmentVariable.argtypes = [c_wchar_p, c_wchar_p, c_void_p, c_int]
             self.SetFirmwareEnvironmentVariable = kernel32.SetFirmwareEnvironmentVariableW
             self.SetFirmwareEnvironmentVariable.restype = c_int
             self.SetFirmwareEnvironmentVariable.argtypes = [c_wchar_p, c_wchar_p, c_void_p, c_int]
         except AttributeError as msg:
             if logger().DEBUG: logger().warn( "G[S]etFirmwareEnvironmentVariableW function doesn't seem to exist" )
-            pass
 
         try:
             self.NtEnumerateSystemEnvironmentValuesEx = windll.ntdll.NtEnumerateSystemEnvironmentValuesEx
             self.NtEnumerateSystemEnvironmentValuesEx.restype = c_int
             self.NtEnumerateSystemEnvironmentValuesEx.argtypes = [c_int, c_void_p, c_void_p]
         except AttributeError as msg:
             if logger().DEBUG: logger().warn( "NtEnumerateSystemEnvironmentValuesEx function doesn't seem to exist" )
-            pass
 
         try:
             self.GetFirmwareEnvironmentVariableEx = kernel32.GetFirmwareEnvironmentVariableExW
             self.GetFirmwareEnvironmentVariableEx.restype = c_int
             self.GetFirmwareEnvironmentVariableEx.argtypes = [c_wchar_p, c_wchar_p, c_void_p, c_int, c_int_p]
             self.SetFirmwareEnvironmentVariableEx = kernel32.SetFirmwareEnvironmentVariableExW
             self.SetFirmwareEnvironmentVariableEx.restype = c_int
             self.SetFirmwareEnvironmentVariableEx.argtypes = [c_wchar_p, c_wchar_p, c_void_p, c_int, c_int]
         except AttributeError as msg:
             if logger().DEBUG: logger().warn( "G[S]etFirmwareEnvironmentVariableExW function doesn't seem to exist" )
-            pass
 
         try:
             self.GetSystemFirmwareTbl = kernel32.GetSystemFirmwareTable
             self.GetSystemFirmwareTbl.restype = c_int
             self.GetSystemFirmwareTbl.argtypes = [c_int, c_int, c_void_p, c_int]
         except AttributeError as msg:
             if logger().DEBUG: logger().warn( "GetSystemFirmwareTable function doesn't seem to exist" )
-            pass
 
         try:
             self.EnumSystemFirmwareTbls = kernel32.EnumSystemFirmwareTables 
             self.EnumSystemFirmwareTbls.restype = c_int
             self.EnumSystemFirmwareTbls.argtypes = [c_int, c_void_p, c_int]
         except AttributeError as msg:
             if logger().DEBUG: logger().warn( "GetSystemFirmwareTable function doesn't seem to exist" )
@@ -364,15 +354,15 @@
 
         try:
             hscm = win32service.OpenSCManager( None, None, win32service.SC_MANAGER_ALL_ACCESS ) # SC_MANAGER_CREATE_SERVICE
         except win32service.error as err:
             _handle_winerror(err.args[1], err.args[2], err.args[0])
 
         if logger().DEBUG:
-            logger().log( "[helper] service control manager opened (handle = 0x{:08X})".format(hscm) )
+            logger().log( "[helper] service control manager opened (handle = {})".format(hscm) )
             logger().log( "[helper] driver path: '{}'".format(os.path.abspath(self.driver_path)) )
 
         try:
             hs = win32service.CreateService(
                  hscm,
                  SERVICE_NAME,
                  DISPLAY_NAME,
@@ -381,46 +371,46 @@
                  win32service.SERVICE_DEMAND_START,
                  win32service.SERVICE_ERROR_NORMAL,
                  os.path.abspath(self.driver_path),
                  None, 0, u"", None, None )
             if hs:
                 if logger().DEBUG: logger().log( "[helper] service '{}' created (handle = 0x{:08X})".format(SERVICE_NAME,hs) )
         except win32service.error as err:
-            if (winerror.ERROR_SERVICE_EXISTS == err[0]):
-                if logger().DEBUG: logger().log( "[helper] service '{}' already exists: {} ({:d})".format(SERVICE_NAME, err[2], err[0]) )
+            if (winerror.ERROR_SERVICE_EXISTS == err.args[0]):
+                if logger().DEBUG: logger().log( "[helper] service '{}' already exists: {} ({:d})".format(SERVICE_NAME, err.args[2], err.args[0]) )
                 try:
                     hs = win32service.OpenService( hscm, SERVICE_NAME, (win32service.SERVICE_QUERY_STATUS|win32service.SERVICE_START|win32service.SERVICE_STOP) ) # SERVICE_ALL_ACCESS
                 except win32service.error as err1:
-                    _handle_winerror(err1[1], err1[2], err1[0])
+                    _handle_winerror(err1.args[1], err1.args[2], err1.args[0])
             else:
-                _handle_winerror(err[1], err[2], err[0])
+                _handle_winerror(err.args[1], err.args[2], err.args[0])
 
         finally:
             win32service.CloseServiceHandle( hs )
             win32service.CloseServiceHandle( hscm )
 
         return True
 
     #
-    # Remove (detele/unregister/uninstall) chipsec service
+    # Remove (delete/unregister/uninstall) chipsec service
     #
     def delete( self, start_driver ):
         if not start_driver: return True
         if self.use_existing_service: return True
 
         if win32serviceutil.QueryServiceStatus( SERVICE_NAME )[1] != win32service.SERVICE_STOPPED:
             if logger().DEBUG: logger().warn( "cannot delete service '{}' (not stopped)".format(SERVICE_NAME) )
             return False
 
         if logger().DEBUG: logger().log( "[helper] deleting service '{}'...".format(SERVICE_NAME) )
         try:
             win32serviceutil.RemoveService( SERVICE_NAME )
             if logger().DEBUG: logger().log( "[helper] service '{}' deleted".format(SERVICE_NAME) )
         except win32service.error as err:
-            if logger().DEBUG: logger().warn( "RemoveService failed: {} ({:d})".format(err[2], err[0]) )
+            if logger().DEBUG: logger().warn( "RemoveService failed: {} ({:d})".format(err.args[2], err.args[0]) )
             return False
 
         return True
 
     #
     # Start chipsec service
     #
@@ -439,15 +429,15 @@
             #    _handle_error( "connecting to existing '{}' service failed (service is not running)".format(SERVICE_NAME) )
             try:
                 win32serviceutil.StartService( SERVICE_NAME )
                 win32serviceutil.WaitForServiceStatus( SERVICE_NAME, win32service.SERVICE_RUNNING, 1 )
                 self.driver_loaded = True
                 if logger().DEBUG: logger().log( "[helper] service '{}' started".format(SERVICE_NAME) )
             except pywintypes.error as err:
-                _handle_error( "service '{}' didn't start: {} ({:d})".format(SERVICE_NAME, err[2], err[0]), err[0] )
+                _handle_error( "service '{}' didn't start: {} ({:d})".format(SERVICE_NAME, err.args[2], err.args[0]), err.args[0] )
         self.driverpath = win32serviceutil.LocateSpecificServiceExe(SERVICE_NAME)
         return True
 
     #
     # Stop chipsec service
     #
     def stop( self, start_driver ):
@@ -456,24 +446,24 @@
 
         if logger().DEBUG: logger().log( "[helper] stopping service '{}'..".format(SERVICE_NAME) )
         try:
             win32api.CloseHandle( self.driver_handle )
             self.driver_handle = None
             win32serviceutil.StopService( SERVICE_NAME )
         except pywintypes.error as err:
-            if logger().DEBUG: logger().error( "StopService failed: {} ({:d})".format(err[2], err[0]) )
+            if logger().DEBUG: logger().error( "StopService failed: {} ({:d})".format(err.args[2], err.args[0]) )
             return False
         finally:
             self.driver_loaded = False
 
         try:
             win32serviceutil.WaitForServiceStatus( SERVICE_NAME, win32service.SERVICE_STOPPED, 1 )
             if logger().DEBUG: logger().log( "[helper] service '{}' stopped".format(SERVICE_NAME) )
         except pywintypes.error as err:
-            if logger().DEBUG: logger().warn( "service '{}' didn't stop: {} ({:d})".format(SERVICE_NAME, err[2], err[0]) )
+            if logger().DEBUG: logger().warn( "service '{}' didn't stop: {} ({:d})".format(SERVICE_NAME, err.args[2], err.args[0]) )
             return False
 
         return True
 
 
 
     def get_driver_handle( self ):
@@ -481,15 +471,15 @@
         if (self.driver_handle is not None) and (INVALID_HANDLE_VALUE != self.driver_handle):
             return self.driver_handle
 
         self.driver_handle = win32file.CreateFile( self.device_file, FILE_SHARE_READ | FILE_SHARE_WRITE, 0, None, OPEN_EXISTING, FILE_ATTRIBUTE_NORMAL | FILE_FLAG_OVERLAPPED, None )
         if (self.driver_handle is None) or (INVALID_HANDLE_VALUE == self.driver_handle):
             _handle_error( drv_hndl_error_msg, errno.ENXIO )
         else:
-            if logger().DEBUG: logger().log( "[helper] opened device '{:.64}' (handle: {:08X})".format(DEVICE_FILE, self.driver_handle) )
+            if logger().DEBUG: logger().log( "[helper] opened device '{:.64}' (handle: {:08X})".format(DEVICE_FILE, int(self.driver_handle)) )
         return self.driver_handle
 
     def check_driver_handle( self ):
         if (0x6 == kernel32.GetLastError()):
             #kernel32.CloseHandle( self.driver_handle )
             win32api.CloseHandle( self.driver_handle )
             self.driver_handle = None
@@ -518,25 +508,25 @@
     def _ioctl( self, ioctl_code, in_buf, out_length ):
 
         if not self.driver_loaded:
            _handle_error("chipsec kernel driver is not loaded (in native API mode?)")
 
         out_buf = (c_char * out_length)()
         self.get_driver_handle()
-        if logger().DEBUG: print_buffer( in_buf )
+        if logger().DEBUG: print_buffer( bytestostring(in_buf) )
         try:
             out_buf = win32file.DeviceIoControl( self.driver_handle, ioctl_code, in_buf, out_length, None )
         except pywintypes.error as _err:
-            err_status = _err[0] + 0x100000000
+            err_status = _err.args[0] + 0x100000000
             if STATUS_PRIVILEGED_INSTRUCTION == err_status:
                 err_msg = "HW Access Violation: DeviceIoControl returned STATUS_PRIVILEGED_INSTRUCTION (0x{:X})".format(err_status)
                 if logger().DEBUG: logger().error( err_msg )
                 raise HWAccessViolationError( err_msg, err_status )
             else:
-                _handle_error( "HW Access Error: DeviceIoControl returned status 0x{:X} ({})".format(err_status,_err[2]), err_status )
+                _handle_error( "HW Access Error: DeviceIoControl returned status 0x{:X} ({})".format(err_status,_err.args[2]), err_status )
 
         return out_buf
 
 ###############################################################################################
 # Actual driver IOCTL functions to access HW resources
 ###############################################################################################
 
@@ -587,98 +577,64 @@
         elif size == 2: buf = struct.pack( '=H', value&0xFFFF )
         elif size == 1: buf = struct.pack( '=B', value&0xFF )
         else: return False
         return self.write_phys_mem( ((phys_address>>32)&0xFFFFFFFF), (phys_address&0xFFFFFFFF), size, buf )
 
     def alloc_phys_mem( self, length, max_pa ):
         #raise UnimplementedNativeAPIError( "alloc_phys_mem" )
-        (va, pa) = (0,0)
         out_length = 16
-        out_buf = (c_char * out_length)()
         in_buf = struct.pack( '<I', length )
         out_buf = self._ioctl( IOCTL_ALLOC_PHYSMEM, in_buf, out_length )
         (size, pa, va) = struct.unpack( '<IIQ', out_buf )
         print (hex(va), hex(pa))
         return (va, pa)
 
     def va2pa( self, va ):
         raise UnimplementedNativeAPIError( "va2pa" )
-        error_code = 0
-        in_length  = 8
-        out_length = 8
-        out_buf = (c_char * out_length)()
-        in_buf = struct.pack( 'Q', va )
-        out_buf = self._ioctl( IOCTL_GET_PHYSADDR, in_buf, out_length )
-        pa = struct.unpack( 'Q', out_buf )[0]
-        return (pa,error_code)
 
     #
     # HYPERCALL
     #
     def hypercall( self, rcx, rdx, r8, r9, r10, r11, rax, rbx, rdi, rsi, xmm_buffer ):
         raise UnimplementedNativeAPIError( "hypercall" )
-        if self.os_machine == 'AMD64':
-            arg_type = 'Q'
-            out_length = 8
-        else:
-            arg_type = 'I'
-            out_length = 4
-        out_buf = (c_char * out_length)()
-        in_buf  = struct.pack( '<11' + arg_type, rcx, rdx, r8, r9, r10, r11, rax, rbx, rdi, rsi, xmm_buffer )
-        out_buf = self._ioctl( IOCTL_HYPERCALL, in_buf, out_length )
-        return struct.unpack( '<' + arg_type, out_buf )[0]
 
     #
     # MAP_IO_SPACE
     #
     def map_io_space( self, physical_address, length, cache_type ):
         raise UnimplementedNativeAPIError( "map_io_space" )
-        out_length = 8
-        out_buf = (c_char * out_length)()
-        in_buf  = struct.pack( '<3Q', physical_address, length, cache_type )
-        out_buf = self._ioctl( IOCTL_MAP_IO_SPACE, in_buf, out_length )
-        virtual_address = struct.unpack( '<Q', out_buf )[0]
-        return virtual_address
 
     #
     # FREE_PHYS_MEM
     #
     def free_phys_mem( self, physical_address ):
         raise UnimplementedNativeAPIError( "free_phys_mem" )
-        out_length = 8
-        out_buf = (c_char * out_length)()
-        in_buf  = struct.pack( '<QQ', 0, physical_address )
-        out_buf = self._ioctl( IOCTL_FREE_PHYSMEM, in_buf, out_length )
-        return
 
     def read_msr( self, cpu_thread_id, msr_addr ):
         (eax,ebx,ecx,edx) = (0,0,0,0)
         out_length = 16
-        out_buf = (c_char * out_length)()
         out_size = c_ulong(out_length)
         in_buf = struct.pack( '<4I', 0, 0, msr_addr, 0 )
         out_buf = self._ioctl( IOCTL_RDMSR, in_buf, out_length )
         try:
             (eax,ebx,ecx,edx) = struct.unpack( '<4I', out_buf )
         except:
             if logger().DEBUG: logger().error( 'DeviceIoControl did not return 4 DWORD values' )
 
         return (eax, edx)
 
     def write_msr( self, cpu_thread_id, msr_addr, eax, edx ):
         out_length = 0
-        out_buf = (c_char * out_length)()
         out_size = c_ulong(out_length)
         in_buf = struct.pack( '<4I', eax, 0, msr_addr, edx )
         out_buf = self._ioctl( IOCTL_WRMSR, in_buf, out_length )
 
         return
 
     def read_pci_reg( self, bus, device, function, address, size ):
-        value = 0xFFFFFFFF
         bdf = PCI_BDF( bus&0xFFFF, device&0xFFFF, function&0xFFFF, address&0xFFFF )
         cfg_addr = bdf.cfg_address()
         byte_off = address & 0x03
         self.write_io_port(0xCF8, cfg_addr, 4)
         value = self.read_io_port(0xCFC + byte_off, size)
         return value
 
@@ -688,20 +644,14 @@
         byte_off = address & 0x03
         self.write_io_port(0xCF8, cfg_addr, 4)
         self.write_io_port(0xCFC + byte_off, value, size)
         return True
 
     def load_ucode_update( self, cpu_thread_id, ucode_update_buf ):
         raise UnimplementedNativeAPIError( "load_ucode_update" )
-        in_length = len(ucode_update_buf) + 3
-        out_length = 0
-        out_buf = (c_char * out_length)()
-        in_buf = struct.pack( '=BH', cpu_thread_id, len(ucode_update_buf) ) + ucode_update_buf
-        out_buf = self._ioctl( IOCTL_LOAD_UCODE_PATCH, in_buf, out_length )
-        return True
 
     def read_io_port( self, io_port, size ):
         in_buf = struct.pack( '<II', io_port, 0 )
         mask = 0
         #print "[read_io_port] ", hex(io_port), size
         try:
             if 1 == size:
@@ -752,19 +702,14 @@
         return True
 
     #
     # IDTR/GDTR/LDTR
     #
     def get_descriptor_table( self, cpu_thread_id, desc_table_code  ):
         raise UnimplementedNativeAPIError( "get_descriptor_table" )
-        in_buf = struct.pack( 'BB', cpu_thread_id, desc_table_code )
-        out_buf = self._ioctl( IOCTL_GET_CPU_DESCRIPTOR_TABLE, in_buf, 18 )
-        (limit,base,pa) = struct.unpack( '=HQQ', out_buf )
-        return (limit,base,pa)
-
 
     #
     # EFI Variable API
     #
     def EFI_supported( self):
         # @TODO: use GetFirmwareType ?
         return ((self.GetFirmwareEnvironmentVariable is not None) or (self.GetFirmwareEnvironmentVariableEx is not None))
@@ -842,20 +787,14 @@
         return getEFIvariables_NtEnumerateSystemEnvironmentValuesEx2( efi_vars )
 
     #
     # Interrupts
     #
     def send_sw_smi( self, cpu_thread_id, SMI_code_data, _rax, _rbx, _rcx, _rdx, _rsi, _rdi ):
         raise UnimplementedNativeAPIError( "send_sw_smi" )
-        out_length = 0
-        out_buf = (c_char * out_length)()
-        out_size = c_ulong(out_length)
-        in_buf = struct.pack( '=H6Q', SMI_code_data, _rax, _rbx, _rcx, _rdx, _rsi, _rdi )
-        out_buf = self._ioctl( IOCTL_SWSMI, in_buf, out_length )
-        return
 
     def _get_handle_for_pid( self, pid=0, ro=True ):
         if pid == 0:
             pHandle = win32process.GetCurrentProcess()
         else:
             flags = win32con.PROCESS_QUERY_INFORMATION
             if not ro:
@@ -887,15 +826,14 @@
 
     #
     # CPUID
     #
     def cpuid( self, eax, ecx ):
         #raise UnimplementedNativeAPIError( "cpuid" )
         out_length = 16
-        out_buf = (c_char * out_length)()
         in_buf = struct.pack( '<2I', eax, ecx )
         out_buf = self._ioctl( IOCTL_CPUID, in_buf, out_length )
         (eax, ebx, ecx, edx) = struct.unpack( '<4I', out_buf )
         return (eax, ebx, ecx, edx)
 
 
     def get_ACPI_SDT( self ):
@@ -914,15 +852,15 @@
         if retVal > table_size:
             table_size = retVal
             tBuffer    = create_string_buffer( table_size )
             retVal     = self.GetSystemFirmwareTbl( FirmwareTableProviderSignature_ACPI, tbl, tBuffer, table_size )
         return tBuffer[:retVal]
 
     # ACPI access is implemented through ACPI HAL rather than through kernel module
-    def get_ACPI_table( self ):
+    def get_ACPI_table( self, table_name ):
         raise UnimplementedAPIError( "get_ACPI_table" )
 
 
 
     #
     # IOSF Message Bus access
     #
```

### Comparing `chipsec-1.4.4/chipsec/helper/rwe/__init__.py` & `chipsec-1.5.1/chipsec/helper/rwe/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/helper/efi/efihelper.py` & `chipsec-1.5.1/chipsec/helper/efi/efihelper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -116,15 +116,15 @@
     # Physical memory access
     #
 
     def read_phys_mem( self, phys_address_hi, phys_address_lo, length ):
         if logger().DEBUG:
             logger().log( '[efi] helper does not support 64b PA' )
         return self._read_phys_mem( phys_address_lo, length )
-          
+
     def _read_phys_mem( self, phys_address, length ):
         return edk2.readmem( phys_address, length )
 
     def write_phys_mem( self, phys_address_hi, phys_address_lo, length, buf ):
         if logger().DEBUG:
             logger().log( '[efi] helper does not support 64b PA' )
         return self._write_phys_mem( phys_address_lo, length, buf )
@@ -181,15 +181,15 @@
         if logger().DEBUG:
             logger().log( '[efi] helper does not support 64b PA' )
         if size == 4:
             return edk2.writemem_dword( phys_address, value )
         else:
             buf = struct.pack(size*"B", value)
             edk2.writemem( phys_address, buf, size )
-        
+
     #
     # PCIe configuration access
     #
 
     def read_pci_reg( self, bus, device, function, address, size ):
         if   (1 == size):
             return ( edk2.readpci( bus, device, function, address, size ) & 0xFF )
@@ -246,15 +246,15 @@
         if logger().DEBUG: logger().error( "[efi] load_ucode_update is not supported yet" )
         return 0
 
     def get_threads_count ( self ):
         if logger().DEBUG: logger().log_warning( "EFI helper hasn't implemented get_threads_count yet" )
         #print "OsHelper for %s does not support get_threads_count from OS API"%self.os_system.lower()
         return 0
-        
+
     def cpuid(self, eax, ecx):
         (reax, rebx, recx, redx)=edk2.cpuid(eax,ecx)
         return (reax, rebx, recx, redx)
 
     def get_descriptor_table( self, cpu_thread_id, desc_table_code ):
         if logger().DEBUG: logger().log_warning("EFI helper has not implemented get_descriptor_table yet")
         return 0
@@ -267,82 +267,81 @@
         tool_name = _tools[ tool_type ] if tool_type in _tools else None
         tool_path = os.path.join( get_tools_path(), self.os_system.lower() )
         return tool_name,tool_path
 
     def getcwd( self ):
         return os.getcwd()
 
-        
     #
     # EFI Variable API
     #
 
     def EFI_supported( self ):
         return True
 
     def get_EFI_variable_full(self, name, guidstr):
         guid = uuid.UUID(guidstr)
-        
+
         size = 100
         (Status, Attributes, newdata, DataSize) = edk2.GetVariable(unicode(name), guid.bytes, size)
-        
+
         if Status == 5:
             size = DataSize+1
             (Status, Attributes, newdata, DataSize) = edk2.GetVariable(unicode(name), guid.bytes, size) 
-        
+
         return (Status, newdata, Attributes)
-        
+
 
     def get_EFI_variable(self, name, guidstr):
         (status, data, attrs) = self.get_EFI_variable_full(name, guidstr)
         return data
-        
+
     def set_EFI_variable(self, name, guidstr, data, datasize=None, attrs=0x7):
-        
+
         guid = uuid.UUID(guidstr)
-        
+
         if data     is None: data = '\0'*4
         if datasize is None: datasize = len(data)
         if attrs is None:
             attrs=0x07
             if logger().VERBOSE: logger().log_warning("Setting attributes to: {:04X}".format(attrs))
 
         (Status, datasize, guidbytes) = edk2.SetVariable(unicode(name), guid.bytes, int(attrs), data, datasize)
-        
+
         return Status
-        
+
     def delete_EFI_variable(self, name, guid):
         return self.set_EFI_variable(name, guid, None, 0, 0)
-    
-    def list_EFI_variables(self):   
-                
+
+    def list_EFI_variables(self):
+
         off = 0
         buf = list()
         hdr = 0
         attr = 0
         variables = dict()
 
         status_dict = { 0:"EFI_SUCCESS", 1:"EFI_LOAD_ERROR", 2:"EFI_INVALID_PARAMETER", 3:"EFI_UNSUPPORTED", 4:"EFI_BAD_BUFFER_SIZE", 5:"EFI_BUFFER_TOO_SMALL", 6:"EFI_NOT_READY", 7:"EFI_DEVICE_ERROR", 8:"EFI_WRITE_PROTECTED", 9:"EFI_OUT_OF_RESOURCES", 14:"EFI_NOT_FOUND", 26:"EFI_SECURITY_VIOLATION" }
-        
+
         name = '\0'*200
-        
+
         randguid = uuid.uuid4()
-        
-        (status, name, size, guidbytes) = edk2.GetNextVariableName(200, unicode(name), randguid.bytes)     
-        
+
+        (status, name, size, guidbytes) = edk2.GetNextVariableName(200, unicode(name), randguid.bytes)
+
         if status == 5:
             if logger().DEBUG: logger().log("size was too small increasing to {:d}".format(size))
             name = '\0'*size
             (status, name, size, guidbytes) = edk2.GetNextVariableName(size, unicode(name), randguid.bytes)
 
         while status == 0:
             guid = uuid.UUID(bytes=guidbytes)
             name = name.encode('ascii','ignore')
             (status, data, attr) = self.get_EFI_variable_full(name, guid.hex)
-            
+
             if logger().DEBUG: logger().log("{:d}: Found variable {}".format(len(variables), name))
 
             var = (off, buf, hdr, data, str(guid), attr)
             if name in variables: 
                 if logger().DEBUG: logger().log("WARNING: found a second instance of name {}.".format(name))
 
             else: variables[name] = []
@@ -351,36 +350,39 @@
 
             (status, name, size, guidbytes) = edk2.GetNextVariableName(200, unicode(name), guid.bytes)
             if logger().DEBUG: logger().log("returned {}. status is {}".format(name, status_dict[status]))
 
             if status == 5:
                 if logger().DEBUG: logger().log("size was too small increasing to {:d}".format(size))
                 (status, name, size, guidbytes) = edk2.GetNextVariableName(size, unicode(name), guid.bytes)
-        return variables        
-        
+        return variables
+
     #
     # ACPI tables access
     #
 
     def get_ACPI_SDT( self ):
         if logger().DEBUG: logger().error( "[efi] ACPI is not supported yet" )
-        return 0        
+        return 0
 
     #
     # IOSF Message Bus access
     #
 
     def msgbus_send_read_message( self, mcr, mcrx ):
         if logger().DEBUG: logger().error( "[efi] Message Bus is not supported yet" )
-        return None        
+        return None
 
     def msgbus_send_write_message( self, mcr, mcrx, mdr ):
         if logger().DEBUG: logger().error( "[efi] Message Bus is not supported yet" )
-        return None        
+        return None
 
     def msgbus_send_message( self, mcr, mcrx, mdr=None ):
         if logger().DEBUG: logger().error( "[efi] Message Bus is not supported yet" )
-        return None        
-    
-        
+        return None
+
+    def set_affinity( self, value ):
+        if logger().DEBUG: logger().error( '[efi] API set_affinity() is not supported' )
+        return 0
+
 def get_helper():
     return EfiHelper( )
```

### Comparing `chipsec-1.4.4/chipsec/helper/efi/__init__.py` & `chipsec-1.5.1/chipsec/helper/efi/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/helper/helpers.py` & `chipsec-1.5.1/chipsec/helper/helpers.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/helper/__init__.py` & `chipsec-1.5.1/chipsec/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/helper/osx/osxhelper.py` & `chipsec-1.5.1/chipsec/helper/osx/osxhelper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # CHIPSEC: Platform Security Assessment Framework
 # Copyright (c) 2016, Google
 #
-# Copyright (c) 2010-2019, Intel Corporation
+# Copyright (c) 2010-2020, Intel Corporation
 #
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; Version 2.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -13,28 +13,26 @@
 # GNU General Public License for more details.
 #
 
 """
 OSX helper
 """
 
-import errno
 import fcntl
 import os
 import platform
 import struct
 import subprocess
-import sys
 import shutil
 
 import chipsec
 import chipsec.defines
 from chipsec.helper.oshelper import OsHelperError, HWAccessViolationError, UnimplementedAPIError, UnimplementedNativeAPIError
 from chipsec.helper.basehelper import Helper
-from chipsec.logger import logger, print_buffer
+from chipsec.logger import logger
 
 MSGBUS_MDR_IN_MASK          = 0x1
 MSGBUS_MDR_OUT_MASK         = 0x2
 
 IOCTL_RDPCI                 = 0xc00c7001
 IOCTL_WRPCI                 = 0xc00c7002
 IOCTL_RDMMIO                = 0xc0187003
@@ -441,23 +439,10 @@
         return ret
 
     def map_io_space(self, base, size, cache_type):
         raise NotImplementedError()
 
     def load_ucode_update(self, cpu_thread_id, ucode_update_buf):
         raise NotImplementedError()
-        '''cpu_ucode_thread_id = ctypes.c_int(cpu_thread_id)
-        in_buf = struct.pack(_ucodeh_msg_t_fmt, cpu_thread_id,len(ucode_update_buf))+ ucode_update_buf
-        in_buf_final = array.array("c",in_buf)
-        out_len = 0
-        out_buf = (ctypes.c_char * out_length)()
-        try:
-            out_buf = self.ioctl(IOCTL_LOAD_UCODE_PATCH, in_buf_final)
-        except IOError:
-            if logger().DEBUG:
-                logger().error("IOError IOCTL Load Patch\n")
-            return None
-
-        return True'''
 
 def get_helper():
     return OSXHelper()
```

### Comparing `chipsec-1.4.4/chipsec/helper/osx/__init__.py` & `chipsec-1.5.1/chipsec/helper/osx/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/testcase.py` & `chipsec-1.5.1/chipsec/testcase.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2018-2019, Intel Corporation
+#Copyright (c) 2018-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -64,17 +64,14 @@
 
     def add_properties(self,properties):
         self.properties = properties
 
     def add_testcase(self,test):
         self.test_cases.append(test)
 
-    def get_results(self):
-        return self.test_cases
-
     def get_current(self):
         if len(self.test_cases) == 0 or self.summary:
             return None
         return self.test_cases[len(self.test_cases)-1]
 
     def add_exception(self,name):
         self.exceptions.append(str(name))
@@ -206,27 +203,64 @@
         for test in self.test_cases:
             tc_element =  ET.SubElement(ts_element, "testcase", {'classname':test.name,'name':test.desc, 'time':'{}'.format("{:5f}".format(test.time)if test.time is not None else "0.0")})
             r_element =   ET.SubElement(tc_element, "pass", {"type":test.result})
             out_element = ET.SubElement(tc_element, "system-out")
             out_element.text = test.output
         return xml.dom.minidom.parseString(ET.tostring( xml_element, None, None )).toprettyxml()
 
+
+    def markdown_full(self, name):
+        passed = []
+        failed = []
+        error = []
+        warning = []
+        skipped = []
+        information = []
+        notapplicable = []
+        deprecated = []
+        destination = { 'Passed':        passed,
+                        'Failed':        failed,
+                        'Error':         error,
+                        'Warning':       warning,
+                        'Skipped':       skipped,
+                        'Information':   information,
+                        'NotApplicable': notapplicable,
+                        'Deprecated':    deprecated
+                        }
+
+        for test in self.test_cases:
+            # Test case as header level 4
+            out_string = '#### {:s}\n'.format(test.name.replace('chipsec.modules.',''))
+            for line in test.output.splitlines(True):
+                # Format output as code
+                out_string += '    {:s}'.format(line)
+            destination[test.result].append(out_string)
+
+        ret_string = ""
+        for result in destination:
+            # Category as header level 1
+            ret_string += '\n# {:s}:{:d}\n'.format(result, len(destination[result]))
+            ret_string += ''.join(destination[result])
+        return ret_string
+
+
 class TestCase():
     def __init__(self, name):
         self.name = name
         self.result = ''
         self.output = ''
         self.argv = ''
         self.desc = ''
         self.startTime = None
         self.endTime = None
         self.time = None
 
     def add_output(self, text):
         self.output += str(text)
+        self.output += "\n"
 
     def add_result(self, result):
         self.result = result
 
     def add_arg(self, arg):
         self.argv = arg
```

### Comparing `chipsec-1.4.4/chipsec/hal/io.py` & `chipsec-1.5.1/chipsec/hal/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -28,18 +28,14 @@
     >>> read_port_word( 0x61 )
     >>> read_port_dword( 0x61 )
     >>> write_port_byte( 0x71, 0 )
     >>> write_port_word( 0x71, 0 )
     >>> write_port_dword( 0x71, 0 )
 """
 
-import struct
-import sys
-import os.path
-
 from chipsec.logger import logger
 
 class PortIORuntimeError (RuntimeError):
     pass
 
 class PortIO:
```

### Comparing `chipsec-1.4.4/chipsec/hal/iobar.py` & `chipsec-1.5.1/chipsec/hal/iobar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -26,18 +26,14 @@
 usage:
     >>> get_IO_BAR_base_address( bar_name )
     >>> read_IO_BAR_reg( bar_name, offset, size )
     >>> write_IO_BAR_reg( bar_name, offset, size, value )
     >>> dump_IO_BAR( bar_name )
 """
 
-import struct
-import sys
-import time
-
 from chipsec.hal import hal_base
 from chipsec.logger import logger
 
 DEFAULT_IO_BAR_SIZE = 0x100
 
 class IOBARRuntimeError (RuntimeError):
     pass
```

### Comparing `chipsec-1.4.4/chipsec/hal/virtmem.py` & `chipsec-1.5.1/chipsec/hal/virtmem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -27,28 +27,27 @@
     >>> read_virtual_mem( 0xf0000, 0x100 )
     >>> write_virtual_mem( 0xf0000, 0x100, buffer )
     >>> write_virtual_mem_dowrd( 0xf0000, 0xdeadbeef )
     >>> read_virtual_mem_dowrd( 0xfed40000 )
 """
 
 import struct
-import sys
 
 from chipsec.logger import logger, print_buffer
 from chipsec.hal import hal_base
 
 class MemoryRuntimeError (RuntimeError):
     pass
 
 class MemoryAccessError (RuntimeError):
     pass
 
 class VirtMemory(hal_base.HALBase):
     def __init__( self, cs ):
-        hal_base.HALBase.__init__(VirtMemory,cs)
+        super(VirtMemory, self).__init__(cs)
         self.helper = cs.helper
 
     ####################################################################################
     #
     # virtual memory API using 64b virtual Address
     # (Same functions as below just using 64b PA instead of High and Low 32b parts of PA)
     #
```

### Comparing `chipsec-1.4.4/chipsec/hal/tpm12_commands.py` & `chipsec-1.5.1/chipsec/hal/tpm12_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2018, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -24,15 +24,15 @@
 Definition for TPMv1.2 commands to use with TPM HAL
 
 TCG PC Client TPM Specification
 TCG TPM v1.2 Specification
 """
 
 import struct
-from chipsec.logger import *
+from chipsec.logger import logger
 
 COMMAND_FORMAT = "=HIIIII"
 
 TPM_TAG_RQU_COMMAND = 0xc100
 TPM_TAG_RQU_AUTH1_COMMAND = 0xc200
 TPM_TAG_RQU_AUTH2_COMMAND = 0xC300
 TPM_TAG_RSP_COMMAND = 0xC400
@@ -89,97 +89,76 @@
   25:0x19000000,
   26:0x1a000000,
   27:0x1b000000,
   28:0x1c000000,
   29:0x1d000000,
   30:0x1e000000
 }
-    
+
 def pcrread( command_argv ):
     """
     The TPM_PCRRead operation provides non-cryptographic reporting  of the contents of a named PCR
-    """  
+    """
     Size = 0x0E000000
     try:
         Pcr = PCR[int(command_argv[0])]
     except:
         if logger().HAL: logger().log_bad("Invalid PCR value\n")
         return
     command = struct.pack( COMMAND_FORMAT, TPM_TAG_RQU_COMMAND, Size, TPM_ORD_PCRREAD, Pcr, 0, 0 )
     size = Size >> 0x18
     return ( command, size )
 
 def nvread( command_argv ):
     """
     Read a value from the NV store
     Index, Offset, Size
-    """  
+    """
     Size = 0x18000000
     command = struct.pack( COMMAND_FORMAT, TPM_TAG_RQU_COMMAND, Size, TPM_ORD_NV_READVALUE, int(command_argv[0], 16), int(command_argv[1], 16), int(command_argv[2], 16) )
     size = Size >> 0x18
     return ( command, size )
-    
+
 def startup( command_argv ):
     """
     Execute a tpm_startup command. TPM_Startup is always preceded by TPM_Init, which is the physical indication (a system wide reset) that TPM initialization is necessary
     Type of Startup to be used:
     1: TPM_ST_CLEAR
     2: TPM_ST_STATE
     3: TPM_ST_DEACTIVATED
-    """  
+    """
     try:
         startupType = STARTUP[int(command_argv[0])]
     except:
         if logger().HAL: logger().log_bad("Invalid startup type option value\n")
         return
     Size = 0x0E000000
     command = struct.pack( COMMAND_FORMAT, TPM_TAG_RQU_COMMAND, Size, TPM_ORD_STARTUP, startupType, 0, 0 )
     size = Size >> 0x18
-    return ( command, size )    
+    return ( command, size )
 
 def continueselftest( command_argv ):
     """
     TPM_ContinueSelfTest informs the TPM that it should complete self-test of all TPM functions. The TPM may return success immediately and then perform the self-test, or it may perform the self-test and then return success or failure.
     """
     Size = 0x0A000000
     command = struct.pack( COMMAND_FORMAT, TPM_TAG_RQU_COMMAND, Size, TPM_ORD_CONTINUESELFTEST, 0, 0, 0 )
     size = Size >> 0x18
-    return ( command, size )  
+    return ( command, size )
 
 def getcap( command_argv ):
     """
     Returns current information regarding the TPM
     CapArea    - Capabilities Area
     SubCapSize - Size of SubCapabilities
     SubCap     - Subcapabilities
-    """  
+    """
     Size = 0x18000000
     command = struct.pack( COMMAND_FORMAT, TPM_TAG_RQU_COMMAND, Size, TPM_ORD_GETCAPABILITY, int(command_argv[0], 16), int(command_argv[1], 16), int(command_argv[2], 16) )
     size = Size >> 0x18
     return ( command, size )
-   
+
 def forceclear( command_argv ):
     Size = 0x0A000000
     command = struct.pack( COMMAND_FORMAT, TPM_TAG_RQU_COMMAND, Size, TPM_ORD_FORCECLEAR, 0, 0, 0 )
     size = Size >> 0x18
-    return ( command, size )   
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
+    return ( command, size )
```

### Comparing `chipsec-1.4.4/chipsec/hal/physmem.py` & `chipsec-1.5.1/chipsec/hal/physmem.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2016, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -15,127 +15,119 @@
 #along with this program; if not, write to the Free Software
 #Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
 #Contact information:
 #chipsec@intel.com
 #
 
-
-
-# -------------------------------------------------------------------------------
-#
-# CHIPSEC: Platform Hardware Security Assessment Framework
-# (c) 2010-2012 Intel Corporation
-#
-# -------------------------------------------------------------------------------
-
 """
 Access to physical memory
 
 usage:
     >>> read_physical_mem( 0xf0000, 0x100 )
     >>> write_physical_mem( 0xf0000, 0x100, buffer )
     >>> write_physical_mem_dowrd( 0xf0000, 0xdeadbeef )
     >>> read_physical_mem_dowrd( 0xfed40000 )
 """
 
 import struct
 import sys
 
-from chipsec.logger import *
+from chipsec.hal.hal_base import HALBase
+from chipsec.logger import print_buffer
 
 class MemoryRuntimeError (RuntimeError):
     pass
 
 class MemoryAccessError (RuntimeError):
     pass
 
-class Memory:
+class Memory(HALBase):
     def __init__( self, cs ):
+        super(Memory, self).__init__(cs)
         self.helper = cs.helper
-        self.cs = cs
 
     ####################################################################################
     #
     # Physical memory API using 64b Physical Address
     # (Same functions as below just using 64b PA instead of High and Low 32b parts of PA)
     #
     ####################################################################################
 
     # Reading physical memory
 
     def read_physical_mem( self, phys_address, length ):
-        if logger().HAL: logger().log("[mem] 0x{:016X}".format(phys_address))
+        if self.logger.HAL: self.logger.log("[mem] 0x{:016X}".format(phys_address))
         return self.helper.read_physical_mem( phys_address, length )
 
     def read_physical_mem_dword( self, phys_address ):
         out_buf = self.read_physical_mem( phys_address, 4 )
         value = struct.unpack( '=I', out_buf )[0]
-        if logger().HAL: logger().log( '[mem] dword at PA = 0x{:016X}: 0x{:08X}'.format(phys_address, value) )
+        if self.logger.HAL: self.logger.log( '[mem] dword at PA = 0x{:016X}: 0x{:08X}'.format(phys_address, value) )
         return value
 
     def read_physical_mem_word( self, phys_address ):
         out_buf = self.read_physical_mem( phys_address, 2 )
         value = struct.unpack( '=H', out_buf )[0]
-        if logger().HAL: logger().log( '[mem] word at PA = 0x{:016X}: 0x{:04X}'.format(phys_address, value) )
+        if self.logger.HAL: self.logger.log( '[mem] word at PA = 0x{:016X}: 0x{:04X}'.format(phys_address, value) )
         return value
 
     def read_physical_mem_byte( self, phys_address ):
         out_buf = self.read_physical_mem( phys_address, 1 )
         value = struct.unpack( '=B', out_buf )[0]
-        if logger().HAL: logger().log( '[mem] byte at PA = 0x{:016X}: 0x{:02X}'.format(phys_address, value) )
+        if self.logger.HAL: self.logger.log( '[mem] byte at PA = 0x{:016X}: 0x{:02X}'.format(phys_address, value) )
         return value
 
     # Writing physical memory
 
     def write_physical_mem( self, phys_address, length, buf ):
-        if logger().HAL:
-            logger().log( '[mem] buffer len = 0x{:X} to PA = 0x{:016X}'.format(length, phys_address) )
+        if self.logger.HAL:
+            self.logger.log( '[mem] buffer len = 0x{:X} to PA = 0x{:016X}'.format(length, phys_address) )
             print_buffer( buf )
         return self.helper.write_physical_mem( phys_address, length, buf )
 
     def write_physical_mem_dword( self, phys_address, dword_value ):
-        if logger().HAL: logger().log( '[mem] dword to PA = 0x{:016X} <- 0x{:08X}'.format(phys_address, dword_value) )
+        if self.logger.HAL: self.logger.log( '[mem] dword to PA = 0x{:016X} <- 0x{:08X}'.format(phys_address, dword_value) )
         return self.write_physical_mem( phys_address, 4, struct.pack( 'I', dword_value ) )
 
     def write_physical_mem_word( self, phys_address, word_value ):
-        if logger().HAL: logger().log( '[mem] word to PA = 0x{:016X} <- 0x{:04X}'.format(phys_address, word_value) )
+        if self.logger.HAL: self.logger.log( '[mem] word to PA = 0x{:016X} <- 0x{:04X}'.format(phys_address, word_value) )
         return self.write_physical_mem( phys_address, 2, struct.pack( 'H', word_value ) )
 
     def write_physical_mem_byte( self, phys_address, byte_value ):
-        if logger().HAL: logger().log( '[mem] byte to PA = 0x{:016X} <- 0x{:02X}'.format(phys_address, byte_value) )
+        if self.logger.HAL: self.logger.log( '[mem] byte to PA = 0x{:016X} <- 0x{:02X}'.format(phys_address, byte_value) )
         return self.write_physical_mem( phys_address, 1, struct.pack( 'B', byte_value ) )
 
     # Allocate physical memory buffer
 
     def alloc_physical_mem( self, length, max_phys_address=0xFFFFFFFFFFFFFFFF ):
         (va, pa) = self.helper.alloc_physical_mem( length, max_phys_address )
-        if logger().HAL: logger().log( '[mem] Allocated: PA = 0x{:016X}, VA = 0x{:016X}'.format(pa, va) )
+        if self.logger.HAL: self.logger.log( '[mem] Allocated: PA = 0x{:016X}, VA = 0x{:016X}'.format(pa, va) )
         return (va, pa)
 
     def va2pa( self, va ):
         (pa, error_code) = self.helper.va2pa( va )
-        if logger().HAL: logger().log( '[mem] VA (0x{:016X}) -> PA (0x{:016X})'.format(va, pa) )
+        if self.logger.HAL: self.logger.log( '[mem] VA (0x{:016X}) -> PA (0x{:016X})'.format(va, pa) )
         if error_code:
-            if logger().HAL: logger().log( '[mem] Looks like VA (0x{:016X}) not mapped'.format(va) )
+            if self.logger.HAL: self.logger.log( '[mem] Looks like VA (0x{:016X}) not mapped'.format(va) )
             return 
         return pa
 
     # Map physical address to virtual
 
     def map_io_space(self, pa, length, cache_type):
         va = self.helper.map_io_space(pa, length, cache_type)
-        if logger().HAL: logger().log( '[mem] Mapped: PA = 0x{:016X}, VA = 0x{:016X}'.format(pa, va) )
+        if self.logger.HAL: self.logger.log( '[mem] Mapped: PA = 0x{:016X}, VA = 0x{:016X}'.format(pa, va) )
         return va
 
     # Free physical memory buffer
 
     def free_physical_mem(self, pa):
         ret = self.helper.free_physical_mem(pa)
-        if logger().HAL: logger().log( '[mem] Deallocated : PA = 0x{:016X}'.format(pa) )
+        if self.logger.HAL: self.logger.log( '[mem] Deallocated : PA = 0x{:016X}'.format(pa) )
         return True if ret == 1 else False
 
     def set_mem_bit(self, addr, bit):
         addr += bit >> 3
         byte = self.read_physical_mem_byte(addr)
         self.write_physical_mem_byte(addr, (byte | (0x1 << (bit & 0x7))))
         return byte
```

### Comparing `chipsec-1.4.4/chipsec/hal/uefi_common.py` & `chipsec-1.5.1/chipsec/hal/uefi_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -26,16 +26,16 @@
 
 import os
 import struct
 import codecs
 import uuid
 from collections import namedtuple
 
-from chipsec.file import *
-from chipsec.logger import *
+from chipsec.file import read_file, write_file
+from chipsec.logger import logger, dump_buffer
 from chipsec.defines import bytestostring
 
 #from chipsec.helper.oshelper import helper
 
 
 ################################################################################################
 #
@@ -507,15 +507,15 @@
     return ''
 
 def assemble_uefi_file(guid, image):
     EFI_FFS_FILE_HEADER = "<16sHBBL"
     FileHeaderSize      = struct.calcsize(EFI_FFS_FILE_HEADER)
 
     Type       = EFI_FV_FILETYPE_FREEFORM
-    CheckSum   = 0x0000;
+    CheckSum   = 0x0000
     Attributes = 0x40
     Size       = FileHeaderSize + len(image)
     State      = 0xF8
 
     SizeState  = (Size & 0x00FFFFFF) | (State << 24)
     FileHeader = struct.pack(EFI_FFS_FILE_HEADER, get_guid_bin(guid), CheckSum, Type, Attributes, (Size & 0x00FFFFFF))
 
@@ -856,15 +856,14 @@
         # prevent infinite loop when parsing malformed var
         if SignatureListSize == 0:
             logger().log_bad("db parsing failed!")
             return entries
 
         # Determine the signature type
         SignatureType = guid_str(SignatureType0, SignatureType1, SignatureType2, SignatureType3)
-        short_name = "UNKNOWN"
         sig_parse_f = None
         sig_size = 0
         if (SignatureType in sig_types.keys()):
             sig_name, sig_parse_f, sig_size, short_name = sig_types[SignatureType]
         else:
             logger().log_bad('Unknown signature type {}, skipping signature decode.'.format(SignatureType))
             dof += SignatureListSize
@@ -956,15 +955,14 @@
         name_size *= 2  # Name size is actually the number of CHAR16 in the name array
         tof = dof + AUTH_CERT_DB_DATA_size
         try:
             var_name = codecs.decode(db[tof:tof+name_size], 'utf-16')
         except UnicodeDecodeError:
             logger().warn("Unable to decode {}".format(db[tof:tof+name_size]))
             var_name = "CHIPSEC ERROR!"
-            pass
         tof += name_size
         sig_data = db[tof:tof+cert_data_size]
         entries.append(sig_data)
         sig_file_name = '{}-{}-{:02X}.bin'.format(vendor_guid, codecs.encode(var_name), nsig)
         sig_file_name = os.path.join(decode_dir, sig_file_name)
         write_file(sig_file_name, sig_data)
         dof += cert_node_size
```

### Comparing `chipsec-1.4.4/chipsec/hal/acpi_tables.py` & `chipsec-1.5.1/chipsec/hal/acpi_tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -18,34 +18,25 @@
 #Contact information:
 #chipsec@intel.com
 # Authors:
 #  Sarah Van Sickle, INTEL DCG RED team
 #
 
 
-
-
-# -------------------------------------------------------------------------------
-#
-# CHIPSEC: Platform Hardware Security Assessment Framework
-# (c) 2010-2012 Intel Corporation
-#
-# -------------------------------------------------------------------------------
-
 """
 HAL component decoding various ACPI tables
 """
 
 __version__ = '0.1'
 
 import struct
 from collections import namedtuple
 from uuid import UUID
 
-from chipsec.logger import *
+from chipsec.logger import logger
 from chipsec.hal.uefi_common import GUID,guid_str
 from chipsec.defines import bytestostring
 
 class ACPI_TABLE():
     def parse( self, table_content ):
         return
     def __str__( self ):
@@ -645,25 +636,25 @@
     def parse(self, table_content):
         self.Version = struct.unpack('<H', table_content[0:2])[0]
         self.Status = struct.unpack('<b', table_content[2:3])[0]
         self.ImageType = struct.unpack('<b', table_content[3:4])[0]
         self.ImageAddress = struct.unpack('<Q', table_content[4:12])[0]
         self.ImageOffsetX = struct.unpack('<I', table_content[12:16])[0]
         self.ImageOffsetY = struct.unpack('<I', table_content[16:20])[0]
-        if(self.Status is 0):
+        if self.Status == 0:
             self.OrientationOffset = '0 degrees'
-        elif(self.Status is 1):
+        elif self.Status == 1:
             self.OrientationOffset = '90 degrees'
-        elif(self.Status is 2):
+        elif self.Status == 2:
             self.OrientationOffset = '180 degrees'
-        elif(self.Status is 3):
+        elif self.Status == 3:
             self.OrientationOffset = '270 degrees'
         else:
             self.OrientationOffset = 'Reserved bits are used'
-        if(self.ImageType is 0):
+        if self.ImageType == 0:
             self.ImageTypeStr = ' - Bitmap'
         else:
             self.ImageTypeStr = 'Reserved'
 
     def __str__(self):
         return """
 ------------------------------------------------------------------
@@ -702,37 +693,37 @@
         # Intel VT for Directed I/O Specific DMAr Section:  {0x71761D37, 0x32B2, 0x45cd, {0xA7, 0xD0, 0xB0, 0xFE 0xDD, 0x93, 0xE8, 0xCF}}
         # IOMMU Specific DMAr Section: {0x036F84E1, 0x7F37, 0x428c, {0xA7, 0x9E, 0x57, 0x5F, 0xDF, 0xAA, 0x84, 0xEC}}
         val1 = struct.unpack('<L', table_content[0:4])[0]
         val2 = struct.unpack('<L', table_content[4:8])[0]
         val3 = struct.unpack('<L', table_content[8:12])[0]
         val4 = struct.unpack('<L', table_content[12:16])[0]
         results = '''0x{:08X} 0x{:08X} 0x{:08X} 0x{:08X} - '''.format( val1, val2, val3, val4 )
-        """if val1 is 0x9876CCAD and val2 is 0x47B4 and val3 is 0x4bdb and val4 in [0xB6, 0x5E, 0x16, 0xF1, 0x93, 0xC4, 0xF3, 0xDB]:
+        """if val1 == 0x9876CCAD and val2 == 0x47B4 and val3 == 0x4bdb and val4 in [0xB6, 0x5E, 0x16, 0xF1, 0x93, 0xC4, 0xF3, 0xDB]:
             return results + '''Generic Processor'''
-        elif val1 is 0xDC3EA0B0 and val2 is 0xA144 and val3 is 0x4797 and val4 in [0xB9, 0x5B, 0x53, 0xFA, 0x24, 0x2B, 0x6E, 0x1D]:
+        elif val1 == 0xDC3EA0B0 and val2 == 0xA144 and val3 == 0x4797 and val4 in [0xB9, 0x5B, 0x53, 0xFA, 0x24, 0x2B, 0x6E, 0x1D]:
             return results + '''Processor Specific: IA32/X64'''
-        elif val1 is 0xe429faf1 and val2 is 0x3cb7 and val3 is 0x11d4 and val4 in [0xb, 0xca, 0x7, 0x00, 0x80,0xc7, 0x3c, 0x88, 0x81]:
+        elif val1 == 0xe429faf1 and val2 == 0x3cb7 and val3 == 0x11d4 and val4 in [0xb, 0xca, 0x7, 0x00, 0x80,0xc7, 0x3c, 0x88, 0x81]:
             return results + '''Processor Specific: IPF'''
-        elif val1 is 0xE19E3D16 and val2 is 0xBC11 and val3 is 0x11E4 and val4 in [0x9C, 0xAA, 0xC2, 0x05,0x1D, 0x5D, 0x46, 0xB0]:
+        elif val1 == 0xE19E3D16 and val2 == 0xBC11 and val3 == 0x11E4 and val4 in [0x9C, 0xAA, 0xC2, 0x05,0x1D, 0x5D, 0x46, 0xB0]:
             return results + '''Processor Specific: ARM'''
-        elif val1 is 0xA5BC1114 and val2 is x6F64 and val3 is 0x4EDE and val4 in [0xB8, 0x63, 0x3E, 0x83, 0xED, 0x7C, 0x83, 0xB1]:
+        elif val1 == 0xA5BC1114 and val2 == 0x6F64 and val3 == 0x4EDE and val4 in [0xB8, 0x63, 0x3E, 0x83, 0xED, 0x7C, 0x83, 0xB1]:
             return results + '''Platform Memory'''
-        elif val1 is 0xD995E954 and val2 is 0xBBC1 and val3 is 0x430F and val4 in [0xAD, 0x91, 0xB4, 0x4D, 0xCB,0x3C, 0x6F, 0x35]:
+        elif val1 == 0xD995E954 and val2 == 0xBBC1 and val3 == 0x430F and val4 in [0xAD, 0x91, 0xB4, 0x4D, 0xCB,0x3C, 0x6F, 0x35]:
             return results + '''PCIe'''
-        elif val1 is 0x81212A96 and val2 is 0x09ED and val3 is 0x4996 and val4 in [0x94, 0x71, 0x8D, 0x72, 0x9C, 0x8E, 0x69, 0xED]:
+        elif val1 == 0x81212A96 and val2 == 0x09ED and val3 == 0x4996 and val4 in [0x94, 0x71, 0x8D, 0x72, 0x9C, 0x8E, 0x69, 0xED]:
             return results + '''Firmware Error Record Reference'''
-        elif val1 is 0xC5753963 and val2 is 0x3B84 and val3 is 0x4095 and val4 in [0xBF, 0x78, 0xED, 0xDA, 0xD3, 0xF9, 0xC9, 0xDD]:
+        elif val1 == 0xC5753963 and val2 == 0x3B84 and val3 == 0x4095 and val4 in [0xBF, 0x78, 0xED, 0xDA, 0xD3, 0xF9, 0xC9, 0xDD]:
             return results + '''PCI/PCI-X Bus'''
-        elif val1 0xEB5E4685 is and val2 is 0xCA66 and val3 is 0x4769 and val4 in [0xB6, 0xA2, 0x26, 0x06, 0x8B, 0x00, 0x13, 0x26]:
+        elif val1 == 0xEB5E4685 and val2 == 0xCA66 and val3 == 0x4769 and val4 in [0xB6, 0xA2, 0x26, 0x06, 0x8B, 0x00, 0x13, 0x26]:
             return results + '''PCI Component/Device'''
-        elif val1 is 0x5B51FEF7 and val2 is 0xC79D and val3 is 0x4434 and val4 in [0x8F, 0x1B, 0xAA, 0x62, 0xDE, 0x3E, 0x2C, 0x64]:
+        elif val1 == 0x5B51FEF7 and val2 == 0xC79D and val3 == 0x4434 and val4 in [0x8F, 0x1B, 0xAA, 0x62, 0xDE, 0x3E, 0x2C, 0x64]:
             return results + '''DMAr Generic'''
-        elif val1 is 0x71761D37 and val2 is 0x32B2 and val3 is 0x45cd and val4 in [0xA7, 0xD0, 0xB0, 0xFE, 0xDD, 0x93, 0xE8, 0xCF]:
+        elif val1 == 0x71761D37 and val2 == 0x32B2 and val3 == 0x45cd and val4 in [0xA7, 0xD0, 0xB0, 0xFE, 0xDD, 0x93, 0xE8, 0xCF]:
             return results + '''Intel VT for Directed I/O Specific DMAr Section'''
-        elif val1 is 0x036F84E1 and val2 is 0x7F37 and val3 is 0x428c and val4 in [0xA7, 0x9E, 0x57, 0x5F, 0xDF, 0xAA, 0x84, 0xEC]:
+        elif val1 == 0x036F84E1 and val2 == 0x7F37 and val3 == 0x428c and val4 in [0xA7, 0x9E, 0x57, 0x5F, 0xDF, 0xAA, 0x84, 0xEC]:
             return results + '''IOMMU Specific DMAr Section'''"""
         return results + '''Unknown'''
 
     def parseTime(self, table_content):
         seconds = struct.unpack('<B', table_content[0:1])[0]
         minutes = struct.unpack('<B', table_content[1:2])[0]
         hours = struct.unpack('<B', table_content[2:3])[0]
@@ -765,18 +756,18 @@
             data = str(struct.unpack('<P', table_content[72:errDataLen + 72])[0])
         else:
             data = 'None'
         errorSeverity_str = errorSeverities[4]
         if errorSeverity < 4:
             errorSeverity_str = errorSeverities[errorSeverity]
         revision_str = ''
-        if revision is not 3:
+        if revision != 3:
             revision_str = ' - Should be 0x003'
         FRU_Id_str = ''
-        if FRU_Id1 is 0 and FRU_Id2 is 0 and FRU_Id3 is 0 and FRU_Id4 is 0:
+        if FRU_Id1 == 0 and FRU_Id2 == 0 and FRU_Id3 == 0 and FRU_Id4 == 0:
             FRU_Id_str = ' - Default value, invalid FRU ID'
         return '''
       Section Type                                  : {}
       Error Severity                                : {} - {}
       Revision                                      : 0x{:04X}{}
       Validation Bits                               : 0x{:02X}
       Flags                                         : 0x{:02X}
@@ -862,29 +853,29 @@
         reserved = struct.unpack('<B', table_content[3:4])[0]
         injectionHeaderSz = struct.unpack('<L', table_content[0:4])[0]
         registerRegion = self.parseAddress(table_content[4:16])
         value = struct.unpack('<Q', table_content[16:24])[0]
         mask = struct.unpack('<Q', table_content[24:32])[0]
         if injectionAction < 10:
             injectionAction_str = errorInjectActions[injectionAction]
-        elif injectionAction is 255:
+        elif injectionAction == 255:
             injectionAction_str = 'TRIGGER_ERROR'
         else:
             injectionAction_str = errorInjectActions[10]
         if instruction < 5:
             instruction_str = injectionInstructions[instruction]
         else:
             instruction_str = injectionInstructions[5]
-        if flags is 1 and (instruction is 2 or instruction is 3):
+        if flags == 1 and (instruction == 2 or instruction == 3):
             flags_str = ' - PRESERVE_REGISTER'
-        elif flags is 0:
+        elif flags == 0:
             flags_str = ' - Ignore'
         else:
             flags_str = ''
-        if reserved is not 0:
+        if reserved != 0:
             reserved_str = ' - Error, must be 0'
         else:
             reserved_str = ''
         self.results_str += """
   Injection Instruction Entry
     Injection Action                                : 0x{:02X} ( {:d} ) - {}
     Instruction                                     : 0x{:02X} ( {:d} ) - {}
@@ -909,17 +900,17 @@
         reserved3 = struct.unpack('<B', table_content[7:8])[0]
         reserved3 = reserved3 << 16
         reserved2 = reserved2 << 8
         reserved = reserved3 | reserved2 | reserved1
         injectionEntryCount = struct.unpack('<L', table_content[8:12])[0]
         injection_str = ''
         reserved_str = ''
-        if injectionFlags is not 0:
+        if injectionFlags != 0:
             injection_str = ' - Error, this feild should be 0'
-        if reserved is not 0:
+        if reserved != 0:
             reserved_str = ' - Error, this field should be 0'
         self.results_str = """
 ------------------------------------------------------------------
   Injection Header Size                             : 0x{:016X} ( {:d} )
   Injection Flags                                   : 0x{:02X}{}
   Reserved                                          : 0x{:06X}{}
   Injection Entry Count                             : 0x{:08X} ( {:d} )
@@ -963,19 +954,19 @@
             serializationAction_str = serializationActions[serializationAction]
         else:
             serializationAction_str = 'Unknown'
         if instruction < 17:
             serializationInstr_str = serializationInstructions[instruction]
         else:
             serializationAction_str = 'Unknown'
-        if reserved is not 0:
+        if reserved != 0:
             reserved_str = ' - Error, this should be 0'
         else:
             reserved_str = ''
-        if flags is 1:
+        if flags == 1:
             flags_str = ' - PRESERVE_REGISTER'
         else:
             flags_str = ''
 		
         self.results_str += '''
     Serialization Intruction Entry
       Serialized Action                             : 0x{:02X} - {}
@@ -987,15 +978,15 @@
       Mask                                          : 0x{:016X}
     '''.format( serializationAction, serializationAction_str, instruction, serializationInstr_str, flags, flags_str, reserved, reserved_str, registerRegion, value, mask )
 
     def parse(self, table_content):
         headerSz = struct.unpack('<L', table_content[0:4])[0]
         reserved = struct.unpack('<L', table_content[4:8])[0]
         instrCountEntry = struct.unpack('<L', table_content[8:12])[0]
-        if reserved is not 0:
+        if reserved != 0:
             reserved_str = ' - Error, this should be 0'
         else:
             reserved_str = ''
         self.results_str = """
 ------------------------------------------------------------------
   Serialization Header Size                       : 0x{:08X} ( {:d} )
   Reserved                                        : 0x{:08X}{}
@@ -1015,23 +1006,23 @@
 
 class HEST (ACPI_TABLE):
     def __init__( self ):
         return
 
     def parseErrEntry(self, table_content):
         type = struct.unpack('<H', table_content[0:2])[0]
-        if(type is 0): #Arch Machine Check Execption Structure
+        if type == 0: #Arch Machine Check Execption Structure
             return self.parseAMCES(table_content)
-        elif(type is 1): #Arch Corrected Mach Check Structure or ArchitectureDeferred machine Check Structure
+        elif type == 1: #Arch Corrected Mach Check Structure or ArchitectureDeferred machine Check Structure
             return self.parseAMCS(table_content, type)
-        elif(type is 2): #NMI Error Structure
+        elif type == 2: #NMI Error Structure
             return self.parseNMIStructure(table_content)
-        elif(type is 6 or type is 7 or type is 8): #PCIe Root Port AER Structure or PCIe Device AER Structure or PCIe Bridge AER Structure
+        elif type == 6 or type == 7 or type == 8: #PCIe Root Port AER Structure or PCIe Device AER Structure or PCIe Bridge AER Structure
             return self.parsePCIe(table_content, type)
-        elif(type is 9 or type is 10): #Generic hardware Error Source Structure or Generic Hardware Error Source version 2
+        elif type == 9 or type == 10: #Generic hardware Error Source Structure or Generic Hardware Error Source version 2
             return self.parseGHESS(table_content, type)
         else:
             pass
 
     def parseNotify(self, table_content):
         types = ['Polled','External Interrupt', 'Local Interrupt', 'SCI', 'NMI', 'CMCI', 'MCE', 'GPI-Signal', 'ARMv8 SEA', 'ARMv8 SEI', 'External Interrupt - GSIV', 'Software Delicated Exception', 'Reserved']
         errorType = struct.unpack('<B', table_content[0:1])[0]
@@ -1046,15 +1037,15 @@
 	
         if errorType <= 12:
             typeStr = types[errorType]
         else:
             typeStr = types[12]
 
         vector_str = ''
-        if errorType is 10:
+        if errorType == 10:
             vector_str = 'Specifies the GSIV triggerd by error source'
 		
         return """Hardware Error Notification Structure
       Type                                        : {:d} - {}
       Length                                      : 0x{:02X}
       Configuration Write Enable                  : 0x{:04X}
         Type                                      : {:d}
@@ -1077,41 +1068,41 @@
         reserved1 = struct.unpack('<L', table_content[3:4])[0]
         controlRegMsrAddr = struct.unpack('<L', table_content[4:8])[0]
         controlInitData = struct.unpack('<L', table_content[8:16])[0]
         statusRegMSRAddr =struct.unpack('<L', table_content[16:20])[0]
         addrRegMSRAddr = struct.unpack('<L', table_content[20:24])[0]
         miscRegMSTAddr = struct.unpack('<L', table_content[24:28])[0]
 	
-        if clearStatus is 0:
+        if clearStatus == 0:
             clearStatus_str = 'Clear'
         else:
             clearStatus_str = "Don't Clear"
 		
         statusDataFormatStrList = ['IA-32 MCA', 'Intel 64 MCA',  'AMD64MCA', 'Reserved']
         if statusDataFormat < 3:
             statusDataFormat_str = statusDataFormatStrList[statusDataFormat]
         else:
             statusDataFormat_str = statusDataFormatStrList[3]
 
-        if controlRegMsrAddr is not 0:
+        if controlRegMsrAddr != 0:
             controlRegMsrAddr_str = ''
         else:
             controlRegMsrAddr_str = ' - Ignore'
 
-        if statusRegMSRAddr is not 0:
+        if statusRegMSRAddr != 0:
             statusRegMSRAddr_str = ''
         else:
             statusRegMSRAddr_str = ' - Ignore'
 
-        if addrRegMSRAddr is not 0:
+        if addrRegMSRAddr != 0:
             addrRegMSRAddr_str = ''
         else:
             addrRegMSRAddr_str = ' - Ignore'
 
-        if miscRegMSTAddr is not 0:
+        if miscRegMSTAddr != 0:
             miscRegMSTAddr_str = ''
         else:
             miscRegMSTAddr_str = ' - Ignore' 
 		
         self.resultsStr = self.resultsStr + ("""Machine Check Error Bank Structure
       Bank Number                                 : 0x{:04X}
       Clear Status On Initialization              : 0x{:04X} - {}
@@ -1140,29 +1131,29 @@
         reserved2_2 = struct.unpack('<B', table_content[34:35])[0]
         reserved2_3 = struct.unpack('<B', table_content[35:36])[0]
         reserved2_4 = struct.unpack('<B', table_content[36:37])[0]
         reserved2_5 = struct.unpack('<B', table_content[37:38])[0]
         reserved2_6 = struct.unpack('<B', table_content[38:39])[0]
         reserved2_7 = struct.unpack('<B', table_content[39:40])[0]
         
-        if(flags & 1 is 1):
+        if (flags & 1) == 1:
             firmware_first = 1
             firmware_first_str = 'System firmware handles errors from the source first'
         else:
             firmware_first = 0
             firmware_first_str = 'System firmware does not handle errors from the source first'
 		
-        if(flags & 4 is 4):
+        if (flags & 4) == 4:
             ghes_assist = 1
             ghes_assist_str = 'Additional information given'
         else:
             ghes_assist = 0
             ghes_assist_str = 'Additional information not given'
 		
-        if(firmware_first is 0):
+        if firmware_first == 0:
             ghes_assist_str = 'Bit is reserved'
 		
         self.resultsStr = self.resultsStr + ("""
   Architecture Machine Check Exception Structure
     Source ID                                     : 0x{:04X}
     Reserved                                      : 0x{:04X}
     Flags                                         : 0x{:02X}
@@ -1190,39 +1181,39 @@
         maxSectorsPerRecord = struct.unpack('<L', table_content[12:16])[0]
         notificationStructure = self.parseNotify(table_content[16:44])
         numHardwareBanks = struct.unpack('<B', table_content[44:45])[0]
         reserved2_1 = struct.unpack('<B', table_content[45:46])[0]
         reserved2_2 = struct.unpack('<B', table_content[46:47])[0]
         reserved2_3 = struct.unpack('<B', table_content[47:48])[0]
 		
-        if(flags & 1 is 1):
+        if (flags & 1) == 1:
             firmware_first = 1
             firmware_first_str = 'System firmware handles errors from the source first'
         else:
             firmware_first = 0
             firmware_first_str = 'System firmware does not handle errors from the source first'
 		
-        if(flags & 4 is 4):
+        if (flags & 4) == 4:
             ghes_assist = 1
             ghes_assist_str = 'Additional information given'
         else:
             ghes_assist = 0
             ghes_assist_str = 'Additional information not given'
 		
-        flags_str =''
-        if flags is not 1 and flags is not 4 and flags is not 5:
+        flags_str = ''
+        if flags != 1 and flags != 4 and flags != 5:
             flags_str = ' - Error, Reserved Bits are not 0'
 		
-        if(firmware_first is 0):
+        if firmware_first == 0:
             ghes_assist_str = 'Bit is reserved'
 			
-        if type is 1:
+        if type == 1:
             title = 'Architecture Corrected Machine Check Structure'
         else:
-            title ='Architecture Deferred Machine Check Structure'
+            title = 'Architecture Deferred Machine Check Structure'
 		
         self.resultsStr = self.resultsStr + ("""
     {}
     Source ID         				  : 0x{:04X}
     Reserved                                      : 0x{:04X}
     Flags                                         : 0x{:02X}{}
       FIRMWARE_FIRST                              : {} - {}
@@ -1243,15 +1234,15 @@
     def parseNMIStructure(self, table_content):
         sourceID = struct.unpack('<H', table_content[2:4])[0]
         reserved = struct.unpack('<L', table_content[4:8])[0]
         numRecordsToPreAllocate = struct.unpack('<L', table_content[8:12])[0]
         maxSectorsPerRecord = struct.unpack('<L', table_content[12:16])[0]
         maxRawDataLength = struct.unpack('<L', table_content[16:20])[0]
 		
-        if reserved is 0:
+        if reserved == 0:
             reserved_str = ''
         else:
             reserved_str = ' - Error, not 0'
 		
         self.resultsStr = self.resultsStr + ("""
   Architecture NMI Error Structure
     Source ID                                     : 0x{:04X}
@@ -1275,60 +1266,60 @@
         function = struct.unpack('<H', table_content[22:24])[0]
         deviceControl = struct.unpack('<H', table_content[24:26])[0]
         reserved2 = struct.unpack('<H', table_content[26:28])[0]
         uncorrectableErrorMask = struct.unpack('<L', table_content[28:32])[0]
         uncorrectableErrorServerity = struct.unpack('<L', table_content[32:36])[0]
         correctableErrorMask = struct.unpack('<L', table_content[36:40])[0]
         advancedErrorCapabilitiesAndControl = struct.unpack('<L', table_content[40:44])[0]
-        if type is 6:
+        if type == 6:
             title = 'PCI Express Root Port AER Structure'
             rootErrCommand = struct.unpack('<L', table_content[44:48])[0]
             extra_str = '''
     Root Error Command                            : 0x{:08X}'''.format( rootErrCommand )
             size = 48
-        elif type is 8:
+        elif type == 8:
             title = 'PCI Express Bridge AER Structure'
             secondaryUncorrErrMask = struct.unpack('<L', table_content[44:48])[0]
             secondaryUncorrErrServ = struct.unpack('<L', table_content[48:52])[0]
             secondaryAdvCapabAndControl = struct.unpack('<L', table_content[52:56])[0]
             extra_str = '''
     Secondary Uncorrectable Error Mask            : 0x{:08X}
     Secondary Uncorrectable Error Severity        : 0x{:08X}
     Secondary Advanced Capabilities and Control   : 0x{:08X}'''.format( secondaryUncorrErrMask, secondaryUncorrErrServ, secondaryAdvCapabAndControl )
             size = 56
         else:
             title = 'PCI Express Device AER Structure'
             extra_str = ''
             size = 44
 		
-        if (flags & 1 is 1):
+        if (flags & 1) == 1:
             firmware_first = 1
             firmware_first_str = 'System firmware handles errors from the source first'
         else:
             firmware_first = 0
             firmware_first_str = 'System firmware does not handle errors from the source first'
 		
-        if (flags & 2 is 2):
+        if (flags & 2) == 2:
             global_flag = 1
             global_flag_str = 'Settings in table are for all PCIe Devices'
         else:
             global_flag = 0
             global_flag_str = 'Settings in table are not for all PCIe Devices'
         flags_str = ''
         reserved2_str = ''
         isGlobal_str =''
         isFirmware_str =''
 	
         if flags >= 4:
             flags_str = 'Error, reserved bits are not 0'
-        if reserved2 is not 0:
+        if reserved2 != 0:
             reserved2_str = ' - Error, reserved bits should be 0'
-        if global_flag is not 0:
+        if global_flag != 0:
             isGlobal_str = ' - This field should be ignored since Global is set'
-        if firmware_first is not 0:
+        if firmware_first != 0:
             isFirmware_str = ' - This field should be ignored since FIRMWARE_FIRST is set'
 		    
         self.resultsStr = self.resultsStr + ("""
   {}
     Source ID                                     : 0x{:04X}
     Reserved                                      : 0x{:08X}
     Flags                                         : 0x{:02X}{}
@@ -1356,27 +1347,27 @@
         enabled = struct.unpack('<B', table_content[7:8])[0]
         numRecordsToPreAllocate = struct.unpack('<L', table_content[8:12])[0]
         maxSectorsPerRecord = struct.unpack('<L', table_content[12:16])[0]
         maxRawDataLength = struct.unpack('<L', table_content[16:20])[0]
         address_str = self.parseAddress(table_content[20:32])
         notification_str = self.parseNotify(table_content[32:60])
         errStatusBlockLen = struct.unpack('<L', table_content[60:64])[0]
-        if type is 9:
+        if type == 9:
             title = 'Generic Hardware Error Source Structure'
             extra_str = ''
         else:
             title = 'Generic Hardware Error Source Version 2'
             readAckReg_str = self.parseAddress(table_content[64:76])
             readAckPresv = struct.unpack('<Q', table_content[76:84])[0]
             readAckWr = struct.unpack('<Q', table_content[84:88])[0]
             extra_str = '''
     Read Ack Register - {}
     Read Ack Preserve                             : 0x{:016X}
     Read Ack Write                                : 0x{:016X}'''.format( readAckReg_str,  readAckPresv, readAckWr )
-        if relatedSourceID is 65535:
+        if relatedSourceID == 65535:
             relatedSourceID_str = 'Does not represent an alternate souce'
         else:
             relatedSourceID_str = ''
 		
         self.resultsStr = self.resultsStr + ("""
   {}
     Source ID                                     : 0x{:04X}
@@ -1443,49 +1434,49 @@
         interruptType = struct.unpack('<H', table_content[3:5])[0]
         gpe = struct.unpack('<B', table_content[5:6])[0]
         reserved2 = struct.unpack('<B', table_content[6:7])[0]
         pciDeviceFlag = struct.unpack('<B', table_content[7:8])[0]
         globalSysInter = struct.unpack('<L', table_content[8:12])[0]
         baseAdder = self.parseAddress(table_content[12:24])
         reserved3 = struct.unpack('<B', table_content[28:29])[0]
-        if interfaceType is 1:
+        if interfaceType == 1:
             intTypeStr = "Keyboard Controller Style (KCS)"
-        elif interfaceType is 2:
+        elif interfaceType == 2:
             intTypeStr = "Server Management Interface Chip (SMIC)"
-        elif interfaceType is 3:
+        elif interfaceType == 3:
             intTypeStr = "Block Transfer (BT)"
-        elif interfaceType is 4:
+        elif interfaceType == 4:
             intTypeStr = "SMBus System Interface (SSIF)"
         else:
             intTypeStr = "Reserved"
         specRevStr = ('0x{:02X}'.format(specRev))
         intType_0 = interruptType & 1
         intType_1 = interruptType & 2 >> 1
         intType_other = interruptType ^ 3 >> 2
-        if intType_0 is 1:
+        if intType_0 == 1:
             intTypeSCIGPE = "supported"
         else:
             intTypeSCIGPE = "not supported"
-        if intType_1 is 1:
+        if intType_1 == 1:
             intTypeIO = "supported"
         else:
             intTypeIO = "not supported"
         GPE_str = ''
-        if interruptType & 1 is not 1:
+        if (interruptType & 1) != 1:
             GPE_str = " - should be set to 00h"
         pciDeviceFlag_0 = pciDeviceFlag & 1
-        if pciDeviceFlag_0 is 1:
+        if pciDeviceFlag_0 == 1:
             pci_str = 'For PCi IPMI devices'
             otherStr = self.parseNonUID(table_content[25:28]) 
         else:
             pci_str = 'non-PCI device'
             otherStr = self.parseUID(table_content[25:28])
         pciDeviceFlag_reserved = 1 ^ pciDeviceFlag_0
         globalSysInt_str = ''
-        if intType_1 is not 1:
+        if intType_1 != 1:
             globalSysInt_str = ' - this field should be 0'
         self.results = '''==================================================================
   Service Processor Management Interface Description Table ( SPMI )
 ==================================================================
   Interface Type                                          : 0x{:02X} - {}
   Reserved                                                : 0x{:02X} - Must always be 01h to be compatible with any software implementing previous versions of the spec
   Specification Revision (version)                        : {} 
@@ -1560,17 +1551,17 @@
         length = struct.unpack('<B', table_content[1:2])[0]
         maxDomRangeL = struct.unpack('<L', table_content[2:6])[0]
         maxDomRangeH = struct.unpack('<L', table_content[6:10])[0]
         maxProcCap = struct.unpack('<L', table_content[10:14])[0]
         maxMemCap = struct.unpack('<Q', table_content[14:22])[0]
         maxProcCap_str = ''
         maxMemCap_str = ''
-        if maxProcCap is 0:
+        if maxProcCap == 0:
             maxProcCap_str = ' - Proximity domains do not contain a processor'
-        if maxMemCap is 0:
+        if maxMemCap == 0:
             maxMemCap_str = '- Proximity domains do not contain memory'
         return '''
     Maximum Proximity Domain Informaiton Structure[{:d}]
       Revision                                              : 0x{:02X} ( {:d} )
       Length                                                : 0x{:02X} ( {:d} )
       Proximity Domain Range (low)                          : 0x{:04X}
       Proximity Domain Range (high)                         : 0x{:04X}
@@ -1626,26 +1617,26 @@
         reserved1_3 = struct.unpack('<B', table_content[7:8])[0]
         capabilities = struct.unpack('<L', table_content[8:12])[0]
         cap1 = capabilities & 1
         cap2 = capabilities & 2
         cap3 = capabilities & 4
         capRes = capabilities & ~(7)
         reserved2 = struct.unpack('<L', table_content[12:16])[0]
-        if cap1 is 1:
+        if cap1 == 1:
             cap1_str = 'Platform ensures the entire CPU store data path is flushed to persistent memory on system power loss'
         else:
             cap1_str = 'Platform does not ensure the entire CPU store data path is flushed to persistent memory on system power loss'
-        if cap2 is 2:
+        if cap2 == 2:
             cap2_str = 'Platform provides mehanisms to automatically flush outstanding write data from the memory controller to persistent memory in the event of power loss'
         else:
-            if cap1 is 1:
+            if cap1 == 1:
                 cap2_str = 'Platform does not provides mehanisms to automatically flush outstanding write data from the memory controller to persistent memory in the event of power loss'
             else:
              cap2_str = 'This should be set to 1 - Platform does not support'
-        if cap3 is 4:
+        if cap3 == 4:
             cap3_str = 'Platform supports mirroring multiple byte addressable persistent memory regions together'
         else:
             cap3_str = 'Platform does not support mirroring multiple byte addressable persistent memory regions together'
         return '''
     Platform Capabilities Structure [Type 7]
       Length                                                      : 0x{:04X} ( {:d} bytes )
       Highest Valid Capability                                    : 0x{:02X}
@@ -1715,15 +1706,15 @@
         rfic2 = struct.unpack('<B', table_content[29:30])[0]
         rfic_r1 = rfic1 & 224
         rfic_fif = rfic1 & 31
         rfic_r2 = rfic2 & 224
         rfic_fcf = rfic2 & 31
         numBlockControlWindows = struct.unpack('<H', table_content[30:32])[0]
         cont_str = 'ERROR - Table is shorter than expected.'
-        if numBlockControlWindows is not 0:
+        if numBlockControlWindows != 0:
             szBlckControlWindow = struct.unpack('<Q', table_content[32:40])[0]
             commandRegOffset = struct.unpack('<Q', table_content[40:48])[0]
             szCommandReg = struct.unpack('<Q', table_content[48:56])[0]
             statusRegOffset = struct.unpack('<Q', table_content[56:64])[0]
             szStatus = struct.unpack('<Q', table_content[64:72])[0]
             nvdimmControlRegionFl = struct.unpack('<H', table_content[72:74])[0]
             reserved2_1 = struct.unpack('<B', table_content[74:75])[0]
@@ -1739,15 +1730,15 @@
       Size of Status Register in Block Control Windows            : 0x{:016X}
       NVDIMM Control Region Flag                                  : 0x{:04X}
       Reserved                                                    : 0x{:02X} 0x{:02X} 0x{:02X} 0x{:02X} 0x{:02X} 0x{:02X}
       {}'''.format( szBlckControlWindow, szBlckControlWindow, commandRegOffset, szCommandReg, statusRegOffset, szStatus, nvdimmControlRegionFl, reserved2_1, reserved2_2, reserved2_3, reserved2_4, reserved2_5, reserved2_6, cont_str )
         valid_0 = validFields & 1
         valid_str = ''
         valid_man_str = ''
-        if valid_0 is 0:
+        if valid_0 == 0:
             valid_str = 'System is compliant with ACPI 6.0 - Manufacturing Location & Date fields are invalid and should be ignored'
             valid_man_str = 'Value is invalid and should be ignored'
         return '''
     NVDIMM Control Region Structure [Type 4]
       Length                                                      : 0x{:04X} ( {:d} bytes )
       NVDIMM Control Region Structure Index                       : 0x{:04X}
       Vendor ID                                                   : 0x{:04X}
@@ -1775,43 +1766,16 @@
         reserved = struct.unpack('<L', table_content[4:8])[0]
         curPos = 8
         dataStr = ''
         return '''
     SMBIOS Management Information Structure [Type 3]
       Length                                                      : 0x{:04X} ( {:d} bytes )
       Reserved                                                    : 0x{:08X}
-----Infinite loop occurs here.  Unable to further parse without more work to program.----
+      ----Unable to further at this time.----
 '''.format( tableLen, tableLen, reserved)
-        while curPos < tableLen:
-            smbios_table_type = struct.unpack('<B', table_content[curPos:curPos+1])[0]
-            smbios_table_length = struct.unpack('<B', table_content[curPos + 1:curPos + 2])[0]
-            smbios_table_name = 'Unknown'
-            if smbios_table_type > 0 and smbios_table_type < 43:
-                smbios_table_name = smbios_tables[smbios_table_type]
-            elif smbios_table_type is 126:
-                smbios_table_name =  'Inactive'
-            elif smbios_table_type is 127:
-                smbios_table_name = 'End-of-Table'
-            cur_smbios_table_pos = 2
-            smbios_table_data_str = ''
-            while cur_smbios_table_pos < smbios_table_length:
-                entry = struct.unpack('<B', table_content[curPos + cur_smbios_table_pos:curPos + cur_smbios_table_pos + 1])[0]
-                smbios_table_data_str += '''0x{:02X} '''.format(entry)
-                cur_smbios_table_pos += 1
-            dataStr += '''
-      SMBIOS Table - {}
-        Table Type                                                : 0x{:02X} ( {:d} ) - {}
-        Table Length                                              : 0x{:02X} ( {:d} bytes )
-        Data
-          {}'''.format(smbios_table_name, smbios_table_type, smbios_table_type, smbios_table_name, smbios_table_length, smbios_table_length, smbios_table_data_str)
-        return '''
-    SMBIOS Management Information Structure
-      Length                                                      : 0x{:04X} ( {:d} bytes ){}
-      Reserved                                                    : 0x{:08X}
-'''.format( tableLen, tableLen, reserved, dataStr)
 
     def interleave(self, tableLen, table_content):
         interleaveStructureIndex = struct.unpack('<H', table_content[4:6])[0]
         reserved = struct.unpack('<H', table_content[6:8])[0]
         numLinesDescribed = struct.unpack('<L', table_content[8:12])[0]
         lineSz = struct.unpack('<L', table_content[12:16])[0]
         curLine = 0
@@ -1825,15 +1789,15 @@
     Interleave Structure [Type 2]
       Length                                                      : 0x{:04X} ( {:d} bytes )
       Reserved                                                    : 0x{:04X}
       Number of Lines Described                                   : 0x{:08X} ( {:d} )
       Line Size                                                   : 0x{:08X} ( {:d} bytes )
       Lines {}
 '''.format( tableLen, tableLen, reserved, numLinesDescribed, numLinesDescribed, lineSz, lineSz, lines)
-    
+
     def parseMAP(self, tableLen, table_content):
         nfitDeviceHandle = struct.unpack('<L', table_content[4:8])[0]
         nvdimmPhysID = struct.unpack('<H', table_content[8:10])[0]
         nvdimmRegionID = struct.unpack('<H', table_content[10:12])[0]
         spaRangeStructureIndex = struct.unpack('<H', table_content[12:14])[0]
         nvdimmControlRegionSz = struct.unpack('<H', table_content[14:16])[0]
         nvdimmRegionSz = struct.unpack('<Q', table_content[16:24])[0]
@@ -1887,46 +1851,45 @@
         addressRangeTypeGUID_9 = struct.unpack('<B', table_content[29:30])[0]
         addressRangeTypeGUID_10 = struct.unpack('<B', table_content[30:31])[0]
         addressRangeTypeGUID_11 = struct.unpack('<B', table_content[31:32])[0]
         systemPARangeBase = struct.unpack('<Q', table_content[32:40])[0]
         SPARLen = struct.unpack('<Q', table_content[40:48])[0]
         addrRangeMemMapAttr = struct.unpack('<Q', table_content[48:56])[0]
         spaRangeStructure_str = ''
-        if spaRangeStructure is 0:
+        if spaRangeStructure == 0:
             spaRangeStructure_str = ' - Value of 0 is reserved and shall not be used as an index'
-        if flag1 is 1:
+        if flag1 == 1:
             flag1_str = ' - Control region only for hot add/online operation'
         else:
             flag1_str = ' - Control region not only for hot add/online operation'
-        if flag2 is 1:
-            flag2str = ' - Data in proximity region is valid'
-        else:
+        if flag2 != 1:
             flag2_str = ' - Data in proximity region is not valid'
-        if addrRangeMemMapAttr & 1 is 1:
-            flag2str = 'EFI_MEMORY_UC'
-        elif addrRangeMemMapAttr & 2 is 2:
-            flag2str = 'EFI_MEMORY_WC'
-        elif addrRangeMemMapAttr & 4 is 4:
-            flag2str = 'EFI_MEMORY_WT'
-        elif addrRangeMemMapAttr & 8 is 8:
-            flag2str = 'EFI_MEMORY_WB'
-        elif addrRangeMemMapAttr & 16 is 16:
-            flag2str = 'EFI_MEMORY_UCE'
-        elif addrRangeMemMapAttr & 4096 is 4096:
-            flag2str = 'EFI_MEMORY_WP'
-        elif addrRangeMemMapAttr & 8192 is 8192:
-            flag2str = 'EFI_MEMORY_RP'
-        elif addrRangeMemMapAttr& 16384 is 16384:
-            flag2str = 'EFI_MEMORY_XP'
-        elif addrRangeMemMapAttr is 32768 is 32768:
-            flag2str = 'EFI_MEMORY_NV'
-        elif addrRangeMemMapAttr is 65536 is 65536:
-            flag2str = 'EFI_MEMORY_MORE_RELIABLE'
         else:
-            flag2_str = 'undefined'
+            if (addrRangeMemMapAttr & 1) == 1:
+                flag2_str = 'EFI_MEMORY_UC'
+            elif (addrRangeMemMapAttr & 2) == 2:
+                flag2_str = 'EFI_MEMORY_WC'
+            elif (addrRangeMemMapAttr & 4) == 4:
+                flag2_str = 'EFI_MEMORY_WT'
+            elif (addrRangeMemMapAttr & 8) == 8:
+                flag2_str = 'EFI_MEMORY_WB'
+            elif (addrRangeMemMapAttr & 16) == 16:
+                flag2_str = 'EFI_MEMORY_UCE'
+            elif (addrRangeMemMapAttr & 4096) == 4096:
+                flag2_str = 'EFI_MEMORY_WP'
+            elif (addrRangeMemMapAttr & 8192) == 8192:
+                flag2_str = 'EFI_MEMORY_RP'
+            elif (addrRangeMemMapAttr & 16384) == 16384:
+                flag2_str = 'EFI_MEMORY_XP'
+            elif (addrRangeMemMapAttr & 32768) == 32768:
+                flag2_str = 'EFI_MEMORY_NV'
+            elif (addrRangeMemMapAttr & 65536) == 65536:
+                flag2_str = 'EFI_MEMORY_MORE_RELIABLE'
+            else:
+                flag2_str = 'undefined'
         addressRangeTypeGUID = [ addressRangeTypeGUID_1, addressRangeTypeGUID_2, addressRangeTypeGUID_3, addressRangeTypeGUID_4, addressRangeTypeGUID_5, addressRangeTypeGUID_6, addressRangeTypeGUID_7, addressRangeTypeGUID_8, addressRangeTypeGUID_9, addressRangeTypeGUID_10, addressRangeTypeGUID_11]
         if addressRangeTypeGUID == volitileMemGUID:
             artg_str = 'Volitile Memory Region'
         elif addressRangeTypeGUID == byteAddrPMGUID:
             artg_str = 'Byte Addressable Persistent Memory (PM) Region'
         elif addressRangeTypeGUID == nvdimmControlRegionGUID:
             artg_str = 'NVDIMM Control Region'
@@ -1962,38 +1925,38 @@
         notFinished = True
         curPos = 0
         result = ''
         while notFinished:
             tableType = struct.unpack('<H', table_content[curPos:curPos+2])[0]
             tableLen = struct.unpack('<H', table_content[curPos+2:curPos+4])[0]
             result += ''' Length:                    {:d}'''.format(self.total_length)
-            if tableType is 0:
+            if tableType == 0:
                 result += self.parseSPA( tableLen, table_content[curPos:] )
                 curPos = curPos + tableLen
-            elif tableType is 1:
+            elif tableType == 1:
                 result += self.parseMAP( tableLen, table_content[curPos:] )
                 curPos = curPos + tableLen
-            elif tableType is 2:
+            elif tableType == 2:
                 sz, result_str = self.interleave( tableLen, table_content[curPos:] )
                 result += result_str
                 curPos = curPos + tableLen
-            elif tableType is 3:
+            elif tableType == 3:
                 result += self.smbiosManagementInfo( tableLen, table_content[curPos:] )
                 curPos = curPos + tableLen
-            elif tableType is 4:
+            elif tableType == 4:
                 result += self.nvdimmControlRegionStructMark( tableLen, table_content[curPos:] )
                 curPos += tableLen
-            elif tableType is 5:
+            elif tableType == 5:
                 result += self.nvdimmBlockDataWindowsRegionStruct( tableLen, table_content[curPos:] )
                 curPos = curPos + tableLen
-            elif tableType is 6:
+            elif tableType == 6:
                 sz, result_str = self.flushHintAddrStruct( tableLen, table_content[curPos:] )
                 result += result_str
                 curPos = curPos + tableLen
-            elif tableType is 7:
+            elif tableType == 7:
                 result += self.platCapStruct( tableLen, table_content[curPos:] )
                 curPos = curPos + tableLen
             else:
                 pass
             if curPos >= self.total_length:
                 notFinished = False
         return result
@@ -2075,27 +2038,27 @@
 class GAS:
     def __init__(self,table_content):
         self.addrSpaceID = struct.unpack('<B', table_content[0:1])[0]
         self.regBitWidth = struct.unpack('<B', table_content[1:2])[0]
         self.regBitOffset = struct.unpack('<B', table_content[2:3])[0]
         self.accessSize = struct.unpack('<B', table_content[3:4])[0]
         self.addr = struct.unpack('<Q', table_content[4:12])[0]
-        if self.addrSpaceID is 0:
+        if self.addrSpaceID == 0:
             self.addrSpaceID_str = 'System Memory Space'
-        elif self.addrSpaceID is 1:
+        elif self.addrSpaceID == 1:
             self.addrSpaceID_str = 'System I/O Space'
-        elif self.addrSpaceID is 2:
+        elif self.addrSpaceID == 2:
             self.addrSpaceID_str = 'PCI Configuration Space'
-        elif self.addrSpaceID is 3:
+        elif self.addrSpaceID == 3:
             self.addrSpaceID_str = 'Embedded Controller'
-        elif self.addrSpaceID is 4:
+        elif self.addrSpaceID == 4:
             self.addrSpaceID_str = 'SMBus'
-        elif self.addrSpaceID is 0x0A:
+        elif self.addrSpaceID == 0x0A:
             self.addrSpaceID_str = 'Platform Communications Channel (PCC)'
-        elif self.addrSpaceID is 0x7F:
+        elif self.addrSpaceID == 0x7F:
             self.addrSpaceID_str = 'Functional Fixed Hardware'
         elif self.addrSpaceID >= 0xC0 and self.addrSpaceID <= 0xFF:
             self.addrSpaceID_str = 'OEM Defined'
         else:
             self.addrSpaceID_str = 'Reserved'
         accessSizeList = ['Undefined (legacy reasons)', 'Byte Access', 'Word Access', 'Dword Access', 'QWord Access', 'Not a defined value, check if defined by Address Space ID']
         if self.accessSize < 6:
```

### Comparing `chipsec-1.4.4/chipsec/hal/ucode.py` & `chipsec-1.5.1/chipsec/hal/ucode.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2015, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -15,40 +15,29 @@
 #along with this program; if not, write to the Free Software
 #Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
 #Contact information:
 #chipsec@intel.com
 #
 
-
-
-# -------------------------------------------------------------------------------
-#
-# CHIPSEC: Platform Hardware Security Assessment Framework
-# (c) 2010-2018 Intel Corporation
-#
-# -------------------------------------------------------------------------------
-
 """
 Microcode update specific functionality (for each CPU thread)
 
 usage:
     >>> ucode_update_id( 0 )
     >>> load_ucode_update( 0, ucode_buf )
     >>> update_ucode_all_cpus( 'ucode.pdb' )
     >>> dump_ucode_update_header( 'ucode.pdb' )
 """
 
 import struct
-import sys
+import os
 
-from chipsec.logger import *
-from chipsec.hal.physmem import *
-from chipsec.hal.msr import *
-from chipsec.file import *
+from chipsec.logger import logger
+from chipsec.file import read_file
 
 IA32_MSR_BIOS_UPDT_TRIG      = 0x79
 IA32_MSR_BIOS_SIGN_ID        = 0x8B
 IA32_MSR_BIOS_SIGN_ID_STATUS = 0x1
 
 
 from collections import namedtuple
@@ -93,16 +82,16 @@
 class Ucode:
     def __init__( self, cs ):
         self.helper = cs.helper
         self.cs = cs
 
     # @TODO remove later/replace with msr.get_cpu_thread_count()
     def get_cpu_thread_count( self ):
-        (core_thread_count, dummy) = self.helper.read_msr( 0, Cfg.IA32_MSR_CORE_THREAD_COUNT )
-        return (core_thread_count & Cfg.IA32_MSR_CORE_THREAD_COUNT_THREADCOUNT_MASK)
+        thread_count = self.cs.read_register_field("IA32_MSR_CORE_THREAD_COUNT","Thread_Count")
+        return thread_count
 
     def ucode_update_id(self, cpu_thread_id):
         #self.helper.write_msr( cpu_thread_id, IA32_MSR_BIOS_SIGN_ID, 0, 0 )
         #self.helper.cpuid( cpu_thread_id, 0 )
         (bios_sign_id_lo, bios_sign_id_hi) = self.helper.read_msr( cpu_thread_id, IA32_MSR_BIOS_SIGN_ID )
         ucode_update_id = bios_sign_id_hi
```

### Comparing `chipsec-1.4.4/chipsec/hal/tpm_eventlog.py` & `chipsec-1.5.1/chipsec/hal/tpm_eventlog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # CHIPSEC: Platform Security Assessment Framework
 # Copyright (c) 2017, Google Inc
-# Copyright (c) 2019, Intel Corporation
+# Copyright (c) 2019-2020, Intel Corporation
 #
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; Version 2.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -27,18 +27,16 @@
 https://trustedcomputinggroup.org/wp-content/uploads/EFI-Protocol-Specification-rev13-160330final.pdf
 
 TCG PC Client Platform Firmware Profile Specification
 https://trustedcomputinggroup.org/wp-content/uploads/PC-ClientSpecific_Platform_Profile_for_TPM_2p0_Systems_v51.pdf
 """
 
 import binascii
-import collections
 import struct
 
-from chipsec import defines
 from chipsec.logger import logger
 
 
 class TcgPcrEvent(object):
     """An Event (TPM 1.2 format) as recorded in the SML."""
 
     _header_fmt = "II20sI"
```

### Comparing `chipsec-1.4.4/chipsec/hal/pcidb.py` & `chipsec-1.5.1/chipsec/hal/pcidb.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/hal/vmm.py` & `chipsec-1.5.1/chipsec/hal/vmm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -25,16 +25,14 @@
 2. Second-level Address Translation (SLAT)
 3. VirtIO devices
 4. ...
 
 """
 
 import struct
-import sys
-import os.path
 
 from chipsec.logger import logger, pretty_print_hex_buffer
 import chipsec.hal.pcidb
 
 class VMMRuntimeError (RuntimeError):
     pass
```

### Comparing `chipsec-1.4.4/chipsec/hal/ec.py` & `chipsec-1.5.1/chipsec/hal/ec.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2016, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -41,16 +41,15 @@
     >>> write_memory_extended( word_offset, data )
     >>> read_range( start_offset, size )
     >>> write_range( start_offset, buffer )
 
 """
 
 from chipsec.hal import hal_base
-from chipsec.logger import *
-from chipsec.cfg.common import *
+from chipsec.logger import print_buffer
 
 #
 # Embedded Controller ACPI ports
 #
 IO_PORT_EC_DATA        = 0x62
 IO_PORT_EC_COMMAND     = 0x66
 IO_PORT_EC_STATUS      = 0x66
@@ -140,37 +139,37 @@
             #self.write_data( start_offset + i )
             #buffer[i] = chr( self.read_data() )
             if start_offset + i < 0x100:
                 buffer[i] = chr( self.read_memory( start_offset + i ) )
             else:
                 buffer[i] = chr( self.read_memory_extended( start_offset + i ) )
 
-        if logger().HAL:
-            logger().log( "[ec] read EC memory from offset {:X} size {:X}:".format(start_offset, size) )
+        if self.logger.HAL:
+            self.logger.log( "[ec] read EC memory from offset {:X} size {:X}:".format(start_offset, size) )
             print_buffer( buffer )
         return buffer
 
     def write_range( self, start_offset, buffer ):
         size = len(buffer)
         for i in range(size):
             self.write_memory( start_offset + i, ord(buffer[i]) )
-        if logger().HAL:
-            logger().log( "[ec] write EC memory to offset {:X} size {:X}:".format(start_offset, size) )
+        if self.logger.HAL:
+            self.logger.log( "[ec] write EC memory to offset {:X} size {:X}:".format(start_offset, size) )
             print_buffer( buffer )
         return True
 
     #
     # EC Intex I/O access
     #
     def read_idx( self, offset ):
         self.cs.io.write_port_byte( IO_PORT_EC_INDEX_ADDRL, offset & 0xFF )
         self.cs.io.write_port_byte( IO_PORT_EC_INDEX_ADDRH, (offset>>8) & 0xFF )
         value = self.cs.io.read_port_byte( IO_PORT_EC_INDEX_DATA )
-        if logger().HAL: logger().log( "[ec] index read: offset 0x{:02X} > 0x{:02X}:".format(offset, value) )
+        if self.logger.HAL: self.logger.log( "[ec] index read: offset 0x{:02X} > 0x{:02X}:".format(offset, value) )
         return value
 
     def write_idx( self, offset, value ):
-        if logger().HAL: logger().log( "[ec] index write: offset 0x{:02X} < 0x{:02X}:".format(offset, value) )
+        if self.logger.HAL: self.logger.log( "[ec] index write: offset 0x{:02X} < 0x{:02X}:".format(offset, value) )
         self.cs.io.write_port_byte( IO_PORT_EC_INDEX_ADDRL, offset & 0xFF )
         self.cs.io.write_port_byte( IO_PORT_EC_INDEX_ADDRH, (offset>>8) & 0xFF )
         self.cs.io.write_port_byte( IO_PORT_EC_INDEX_DATA, value & 0xFF )
         return True
```

### Comparing `chipsec-1.4.4/chipsec/hal/spd.py` & `chipsec-1.5.1/chipsec/hal/spd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2016, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -15,23 +15,14 @@
 #along with this program; if not, write to the Free Software
 #Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
 #Contact information:
 #chipsec@intel.com
 #
 
-
-
-# -------------------------------------------------------------------------------
-#
-# CHIPSEC: Platform Hardware Security Assessment Framework
-# (c) 2010-2018 Intel Corporation
-#
-# -------------------------------------------------------------------------------
-
 """
 Access to Memory (DRAM) Serial Presence Detect (SPD) EEPROM
 
 References:
 
 http://www.jedec.org/sites/default/files/docs/4_01_02R19.pdf
 http://www.jedec.org/sites/default/files/docs/4_01_02_10R17.pdf
@@ -42,15 +33,15 @@
 http://www.simmtester.com/page/news/showpubnews.asp?num=101
 http://en.wikipedia.org/wiki/Serial_presence_detect
 """
 
 import struct
 from collections import namedtuple
 
-from chipsec.logger import *
+from chipsec.logger import logger, print_buffer
 
 SPD_SMBUS_ADDRESS = 0xA0 # A2, A4, A6, A8, AA, AC, AE
 SPD_SMBUS_ADDRESS_DIMM0 = SPD_SMBUS_ADDRESS
 SPD_SMBUS_ADDRESS_DIMM1 = SPD_SMBUS_ADDRESS + 0x2
 SPD_SMBUS_ADDRESS_DIMM2 = SPD_SMBUS_ADDRESS + 0x4
 SPD_SMBUS_ADDRESS_DIMM3 = SPD_SMBUS_ADDRESS + 0x6
 SPD_SMBUS_ADDRESS_DIMM4 = SPD_SMBUS_ADDRESS + 0x8
@@ -367,15 +358,15 @@
 
     def detect( self ):
         _dimms = []
         for d in SPD_DIMMS:
             if self.isSPDPresent( d ): _dimms.append( d )
         if logger().HAL:
             logger().log( "Detected the following SPD devices:" )
-            for _dimm in _dimms: logger().log( "%s: 0x%02X" % (SPD_DIMMS[_dimm],_dimm) )
+            for _dimm in _dimms: logger().log( "{}: 0x{:02X}".format(SPD_DIMMS[_dimm],_dimm) )
         return _dimms 
 
     def isSPDPresent( self, device=SPD_SMBUS_ADDRESS ):
         device_type = self.getDRAMDeviceType( device )
         is_spd_present = (device_type != 0xFF)
         if logger().HAL: logger().log( "[spd][0x{:02X}] Detecting SPD.. {}found (DRAM memory type = 0x{:X})".format(device,'' if is_spd_present else 'not ',device_type) )
         return is_spd_present
```

### Comparing `chipsec-1.4.4/chipsec/hal/cmos.py` & `chipsec-1.5.1/chipsec/hal/cmos.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -36,18 +36,14 @@
     >>> cmos.dump()
     >>> cmos.read_cmos_low( offset )
     >>> cmos.write_cmos_low( offset, value )
     >>> cmos.read_cmos_high( offset )
     >>> cmos.write_cmos_high( offset, value )
 """
 
-import struct
-import sys
-import time
-
 from chipsec.hal import hal_base
 import chipsec.logger
 
 class CmosRuntimeError (RuntimeError):
     pass
 class CmosAccessError (RuntimeError):
     pass
```

### Comparing `chipsec-1.4.4/chipsec/hal/iommu.py` & `chipsec-1.5.1/chipsec/hal/iommu.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2016, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -22,16 +22,14 @@
 
 
 
 """
 Access to IOMMU engines
 """
 
-from chipsec.logger import *
-
 from chipsec.hal import hal_base, mmio, paging
 
 IOMMU_ENGINE_DEFAULT = 'VTD'
 IOMMU_ENGINE_GFX     = 'GFXVTD'
 
 
 IOMMU_ENGINES = {
@@ -69,94 +67,94 @@
         return (1==tes)
 
     def set_IOMMU_Translation( self, iommu_engine, te ):
         return self.cs.write_register_field( IOMMU_ENGINES[ iommu_engine ] + '_GCMD', 'TE', te )
 
 
     def dump_IOMMU_configuration( self, iommu_engine ):
-        logger().log( "==================================================================" )
+        self.logger.log( "==================================================================" )
         vtd = IOMMU_ENGINES[ iommu_engine ]
-        logger().log( "[iommu] {} IOMMU Engine Configuration".format(iommu_engine) )
-        logger().log( "==================================================================" )
-        logger().log( "Base register (BAR)       : {}".format(vtd) )
+        self.logger.log( "[iommu] {} IOMMU Engine Configuration".format(iommu_engine) )
+        self.logger.log( "==================================================================" )
+        self.logger.log( "Base register (BAR)       : {}".format(vtd) )
         reg = self.cs.read_register( vtd )
-        logger().log( "BAR register value        : 0x{:X}".format(reg) )
+        self.logger.log( "BAR register value        : 0x{:X}".format(reg) )
         base    = self.get_IOMMU_Base_Address( iommu_engine )
-        logger().log( "MMIO base                 : 0x{:016X}".format(base) )
-        logger().log( "------------------------------------------------------------------" )
+        self.logger.log( "MMIO base                 : 0x{:016X}".format(base) )
+        self.logger.log( "------------------------------------------------------------------" )
         ver_min = self.cs.read_register_field( vtd + '_VER', 'MIN' )
         ver_max = self.cs.read_register_field( vtd + '_VER', 'MAX' )
-        logger().log( "Version                   : {:X}.{:X}".format(ver_max,ver_min) )
+        self.logger.log( "Version                   : {:X}.{:X}".format(ver_max,ver_min) )
         enabled = self.is_IOMMU_Engine_Enabled( iommu_engine )
-        logger().log( "Engine enabled            : {:d}".format(enabled) )
+        self.logger.log( "Engine enabled            : {:d}".format(enabled) )
         te      = self.is_IOMMU_Translation_Enabled( iommu_engine )
-        logger().log( "Translation enabled       : {:d}".format(te) )
+        self.logger.log( "Translation enabled       : {:d}".format(te) )
         rtaddr_rta = self.cs.read_register_field( vtd + '_RTADDR', 'RTA', True )
-        logger().log( "Root Table Address        : 0x{:016X}".format(rtaddr_rta) )
+        self.logger.log( "Root Table Address        : 0x{:016X}".format(rtaddr_rta) )
         irta = self.cs.read_register_field( vtd + '_IRTA', 'IRTA' )
-        logger().log( "Interrupt Remapping Table : 0x{:016X}".format(irta) )
-        logger().log( "------------------------------------------------------------------" )
-        logger().log( "Protected Memory:" )
+        self.logger.log( "Interrupt Remapping Table : 0x{:016X}".format(irta) )
+        self.logger.log( "------------------------------------------------------------------" )
+        self.logger.log( "Protected Memory:" )
         pmen_epm = self.cs.read_register_field( vtd + '_PMEN', 'EPM' )
         pmen_prs = self.cs.read_register_field( vtd + '_PMEN', 'PRS' )
-        logger().log( "  Enabled                 : {:d}".format(pmen_epm) )
-        logger().log( "  Status                  : {:d}".format(pmen_prs) )
+        self.logger.log( "  Enabled                 : {:d}".format(pmen_epm) )
+        self.logger.log( "  Status                  : {:d}".format(pmen_prs) )
         plmbase  = self.cs.read_register_field( vtd + '_PLMBASE', 'PLMB' )
         plmlimit = self.cs.read_register_field( vtd + '_PLMLIMIT', 'PLML' )
         phmbase  = self.cs.read_register_field( vtd + '_PHMBASE', 'PHMB' )
         phmlimit = self.cs.read_register_field( vtd + '_PHMLIMIT', 'PHML' )
-        logger().log( "  Low Memory Base         : 0x{:016X}".format(plmbase) )
-        logger().log( "  Low Memory Limit        : 0x{:016X}".format(plmlimit) )
-        logger().log( "  High Memory Base        : 0x{:016X}".format(phmbase) )
-        logger().log( "  High Memory Limit       : 0x{:016X}".format(phmlimit) )
-        logger().log( "------------------------------------------------------------------" )
-        logger().log( "Capabilities:\n" )
+        self.logger.log( "  Low Memory Base         : 0x{:016X}".format(plmbase) )
+        self.logger.log( "  Low Memory Limit        : 0x{:016X}".format(plmlimit) )
+        self.logger.log( "  High Memory Base        : 0x{:016X}".format(phmbase) )
+        self.logger.log( "  High Memory Limit       : 0x{:016X}".format(phmlimit) )
+        self.logger.log( "------------------------------------------------------------------" )
+        self.logger.log( "Capabilities:\n" )
         cap_reg = self.cs.read_register( vtd + '_CAP' )
         self.cs.print_register( vtd + '_CAP', cap_reg )
         ecap_reg = self.cs.read_register( vtd + '_ECAP' )
         self.cs.print_register( vtd + '_ECAP', ecap_reg )
-        logger().log( '' )
+        self.logger.log( '' )
 
 
     def dump_IOMMU_page_tables( self, iommu_engine ):
         vtd = IOMMU_ENGINES[ iommu_engine ]
         te  = self.is_IOMMU_Translation_Enabled( iommu_engine )
-        logger().log( "[iommu] Translation enabled    : {:d}".format(te) )
+        self.logger.log( "[iommu] Translation enabled    : {:d}".format(te) )
         rtaddr_reg = self.cs.read_register( vtd + '_RTADDR' )
         rtaddr_rta = self.cs.get_register_field( vtd + '_RTADDR', rtaddr_reg, 'RTA', True )
         rtaddr_rtt = self.cs.get_register_field( vtd + '_RTADDR', rtaddr_reg, 'RTT' )
         #rtaddr_rta = self.cs.read_register_field( vtd + '_RTADDR', 'RTA', True )
         #rtaddr_rtt = self.cs.read_register_field( vtd + '_RTADDR', 'RTT' )
-        logger().log( "[iommu] Root Table Address/Type: 0x{:016X}/{:X}".format(rtaddr_rta,rtaddr_rtt) )
+        self.logger.log( "[iommu] Root Table Address/Type: 0x{:016X}/{:X}".format(rtaddr_rta,rtaddr_rtt) )
 
         ecap_reg   = self.cs.read_register( vtd + '_ECAP' )
         ecs        = self.cs.get_register_field( vtd + '_ECAP', ecap_reg, 'ECS' )
         pasid      = self.cs.get_register_field( vtd + '_ECAP', ecap_reg, 'PASID' )
-        logger().log( '[iommu] PASID / ECS            : {:X} / {:X}'.format(pasid, ecs))
+        self.logger.log( '[iommu] PASID / ECS            : {:X} / {:X}'.format(pasid, ecs))
 
         if 0xFFFFFFFFFFFFFFFF != rtaddr_reg:
             if te:
-                logger().log( '[iommu] dumping VT-d page table hierarchy at 0x{:016X} (vtd_context_{:08X})..'.format(rtaddr_rta,rtaddr_rta) )
+                self.logger.log( '[iommu] dumping VT-d page table hierarchy at 0x{:016X} (vtd_context_{:08X})..'.format(rtaddr_rta,rtaddr_rta) )
                 paging_vtd = paging.c_vtd_page_tables( self.cs )
                 paging_vtd.read_vtd_context('vtd_context_{:08X}'.format(rtaddr_rta), rtaddr_rta)
-                logger().log( '[iommu] total VTd domains: {:d}'.format(len(paging_vtd.domains)))
+                self.logger.log( '[iommu] total VTd domains: {:d}'.format(len(paging_vtd.domains)))
                 for domain in paging_vtd.domains:
                     paging_vtd.read_pt_and_show_status('vtd_{:08X}'.format(domain), 'VTd', domain)
-                    #if paging_vtd.failure: logger().error( "couldn't dump VT-d page tables" )    
+                    #if paging_vtd.failure: self.logger.error( "couldn't dump VT-d page tables" )    
             else:
-                logger().log( "[iommu] translation via VT-d engine '{}' is not enabled".format(iommu_engine) )
+                self.logger.log( "[iommu] translation via VT-d engine '{}' is not enabled".format(iommu_engine) )
         else:
-            logger().error( "cannot access VT-d registers" )
+            self.logger.error( "cannot access VT-d registers" )
 
 
     def dump_IOMMU_status( self, iommu_engine ):
         vtd = IOMMU_ENGINES[ iommu_engine ]
-        logger().log( "==================================================================" )
-        logger().log( "[iommu] {} IOMMU Engine Status:".format(iommu_engine) )
-        logger().log( "==================================================================" )
+        self.logger.log( "==================================================================" )
+        self.logger.log( "[iommu] {} IOMMU Engine Status:".format(iommu_engine) )
+        self.logger.log( "==================================================================" )
         gsts_reg = self.cs.read_register( vtd + '_GSTS' )
         self.cs.print_register( vtd + '_GSTS', gsts_reg )
         fsts_reg = self.cs.read_register( vtd + '_FSTS' )
         self.cs.print_register( vtd + '_FSTS', fsts_reg )
         frcdl_reg = self.cs.read_register( vtd + '_FRCDL' )
         self.cs.print_register( vtd + '_FRCDL', frcdl_reg )
         frcdh_reg = self.cs.read_register( vtd + '_FRCDH' )
```

### Comparing `chipsec-1.4.4/chipsec/hal/smbus.py` & `chipsec-1.5.1/chipsec/hal/smbus.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -29,16 +29,14 @@
 
 """
 Access to SMBus Controller
 """
 
 from chipsec.hal import iobar, hal_base
 
-from chipsec.logger import *
-
 SMBUS_COMMAND_QUICK         = 0
 SMBUS_COMMAND_BYTE          = 1
 SMBUS_COMMAND_BYTE_DATA     = 2
 SMBUS_COMMAND_WORD_DATA     = 3
 SMBUS_COMMAND_PROCESS_CALL  = 4
 SMBUS_COMMAND_BLOCK         = 5
 SMBUS_COMMAND_I2C_READ      = 6
@@ -67,37 +65,37 @@
             return sba_base
         else:
             raise iobar.IOBARNotFoundError ('IOBARAccessError: SMBUS_BASE')
 
     def get_SMBus_HCFG( self ):
         if self.cs.is_register_defined( 'SMBUS_HCFG' ):
             reg_value = self.cs.read_register( 'SMBUS_HCFG' )
-            if logger().HAL: self.cs.print_register( 'SMBUS_HCFG', reg_value )
+            if self.logger.HAL: self.cs.print_register( 'SMBUS_HCFG', reg_value )
             return reg_value
         else:
             raise self.cs.RegisterNotFoundError ('RegisterNotFound: SMBUS_HCFG')
 
     def display_SMBus_info( self ):
-        if logger().HAL: logger().log( "[smbus] SMBus Base Address: 0x{:04X}".format(self.get_SMBus_Base_Address()) )
+        if self.logger.HAL: self.logger.log( "[smbus] SMBus Base Address: 0x{:04X}".format(self.get_SMBus_Base_Address()) )
         self.get_SMBus_HCFG()
 
     def is_SMBus_enabled( self ):
         return self.cs.is_device_enabled( 'SMBUS' )
 
     def is_SMBus_supported( self ):
         (did,vid) = self.cs.get_DeviceVendorID( 'SMBUS' )
-        if logger().HAL: logger().log( "[smbus] SMBus Controller (DID,VID) = (0x{:04X},0x{:04X})".format(did,vid) )
+        if self.logger.HAL: self.logger.log( "[smbus] SMBus Controller (DID,VID) = (0x{:04X},0x{:04X})".format(did,vid) )
         if (0x8086 == vid): return True
         else:
-            logger().error( "Unknown SMBus Controller (DID,VID) = (0x{:04X},0x{:04X})".format(did,vid) )
+            self.logger.error( "Unknown SMBus Controller (DID,VID) = (0x{:04X},0x{:04X})".format(did,vid) )
             return False
 
     def is_SMBus_host_controller_enabled( self ):
         hcfg = self.get_SMBus_HCFG()
-        return hcfg.CFG_REG_PCH_SMB_HCFG_HST_EN
+        return self.cs.get_register_field("SMBUS_HCFG", hcfg, "HST_EN")
 
     def enable_SMBus_host_controller( self ):
         # Enable SMBus Host Controller Interface in HCFG
         reg_value = self.cs.read_register( 'SMBUS_HCFG' )
         if 0 == (reg_value & 0x1): self.cs.write_register( 'SMBUS_HCFG', (reg_value|0x1) )
         # @TODO: check SBA is programmed
         sba = self.get_SMBus_Base_Address()
@@ -130,32 +128,32 @@
         for i in range(SMBUS_POLL_COUNT):
             #time.sleep( SMBUS_POLL_SLEEP_INTERVAL )
             sts    = self.cs.read_register( self.smb_reg_status )
             busy   = self.cs.get_register_field( self.smb_reg_status, sts, 'BUSY' )
             intr   = self.cs.get_register_field( self.smb_reg_status, sts, 'INTR' )
             failed = self.cs.get_register_field( self.smb_reg_status, sts, 'FAILED' )
             if 0 == busy and 1 == intr:
-                #if logger().HAL:
+                #if self.logger.HAL:
                 #    intr = chipsec.chipset.get_register_field( self.cs, self.smb_reg_status, sts, 'INTR' )
-                #    logger().log( "[smbus]: INTR = {:d}".format(intr) )
+                #    self.logger.log( "[smbus]: INTR = {:d}".format(intr) )
                 break
             elif 1 == failed:
                 #kill = 0
                 #if chipsec.chipset.register_has_field( self.cs, self.smb_reg_control, 'KILL' ):
                 #    kill = chipsec.chipset.read_register_field( self.cs, self.smb_reg_control, 'KILL' )
-                if logger().HAL: logger().error( "SMBus transaction failed (FAILED/ERROR bit = 1)" )
+                if self.logger.HAL: self.logger.error( "SMBus transaction failed (FAILED/ERROR bit = 1)" )
                 return False
             else:
                 if self.cs.register_has_field( self.smb_reg_status, 'DEV_ERR' ):
                     if 1 == self.cs.get_register_field( self.smb_reg_status, sts, 'DEV_ERR' ): 
-                        if logger().HAL: logger().error( "SMBus device error (invalid cmd, unclaimed cycle or time-out error)" )
+                        if self.logger.HAL: self.logger.error( "SMBus device error (invalid cmd, unclaimed cycle or time-out error)" )
                         return False
                 if self.cs.register_has_field( self.smb_reg_status, 'BUS_ERR' ):
                     if 1 == self.cs.get_register_field( self.smb_reg_status, sts, 'BUS_ERR' ):
-                        if logger().HAL: logger().error( "SMBus bus error" )
+                        if self.logger.HAL: self.logger.error( "SMBus bus error" )
                         return False
         return (0 == busy)
 
     def read_byte( self, target_address, offset ):
         # clear status bits
         self.cs.write_register( self.smb_reg_status, 0xFF )
 
@@ -177,15 +175,15 @@
         # read the data
         value = self.cs.read_register_field( self.smb_reg_data0, 'Data' )
         # clear status bits
         self.cs.write_register( self.smb_reg_status, 0xFF )
         # clear address/offset registers
         #chipsec.chipset.write_register( self.cs, self.smb_reg_address, 0x0 )
         #chipsec.chipset.write_register( self.cs, self.smb_reg_command, 0x0 )
-        if logger().HAL: logger().log( "[smbus] read device {:X} off {:X} = {:X}".format(target_address, offset, value) )
+        if self.logger.HAL: self.logger.log( "[smbus] read device {:X} off {:X} = {:X}".format(target_address, offset, value) )
         return value
 
     def write_byte( self, target_address, offset, value ):
         # clear status bits
         self.cs.write_register( self.smb_reg_status, 0xFF )
 
         # SMBus txn RW direction = Write, SMBus slave address = target_address
@@ -206,28 +204,28 @@
         # wait for cycle to complete
         if not self._wait_for_cycle(): return False
         # clear status bits
         self.cs.write_register( self.smb_reg_status, 0xFF )
         # clear address/offset registers
         #chipsec.chipset.write_register( self.cs, self.smb_reg_address, 0x0 )
         #chipsec.chipset.write_register( self.cs, self.smb_reg_command, 0x0 )
-        if logger().HAL: logger().log( "[smbus] write to device {:X} off {:X} = {:X}".format(target_address, offset, value) )
+        if self.logger.HAL: self.logger.log( "[smbus] write to device {:X} off {:X} = {:X}".format(target_address, offset, value) )
         return True
 
 
     def read_range( self, target_address, start_offset, size ):
         buffer = [chr(0xFF)]*size
         for i in range (size):
             buffer[i] = chr( self.read_byte( target_address, start_offset + i ) )
-        if logger().HAL:
-            logger().log( "[smbus] reading {:d} bytes from device 0x{:X} at offset {:X}".format(size, target_address, start_offset) )
+        if self.logger.HAL:
+            self.logger.log( "[smbus] reading {:d} bytes from device 0x{:X} at offset {:X}".format(size, target_address, start_offset) )
             #print_buffer( buffer )
         return buffer
 
     def write_range( self, target_address, start_offset, buffer ):
         size = len(buffer)
         for i in range(size):
             self.write_byte( target_address, start_offset + i, ord(buffer[i]) )
-        if logger().HAL:
-            logger().log( "[smbus] writing {:d} bytes to device 0x{:X} at offset {:X}".format(size, target_address, start_offset) )
+        if self.logger.HAL:
+            self.logger.log( "[smbus] writing {:d} bytes to device 0x{:X} at offset {:X}".format(size, target_address, start_offset) )
             #print_buffer( buffer )
         return True
```

### Comparing `chipsec-1.4.4/chipsec/hal/msgbus.py` & `chipsec-1.5.1/chipsec/hal/msgbus.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2018, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -16,22 +16,14 @@
 #Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
 #Contact information:
 #chipsec@intel.com
 #
 
 
-
-# -------------------------------------------------------------------------------
-#
-# CHIPSEC: Platform Hardware Security Assessment Framework
-# (c) 2010-2018 Intel Corporation
-#
-# -------------------------------------------------------------------------------
-
 """
 Access to message bus (IOSF sideband) interface registers on Intel SoCs
 
 References:
 
 - Intel(R) Atom(TM) Processor E3800 Product Family Datasheet, May 2016, Revision 4.0
   http://www.intel.com/content/www/us/en/embedded/products/bay-trail/atom-e3800-family-datasheet.html (sections 3.6 and 13.4.6 - 13.4.8)
@@ -43,20 +35,15 @@
     >>> msgbus_reg_read( port, register )
     >>> msgbus_reg_write( port, register, data )
     >>> msgbus_read_message( port, register, opcode )
     >>> msgbus_write_message( port, register, opcode, data )
     >>> msgbus_send_message( port, register, opcode, data )
 """
 
-import struct
-import sys
-import os.path
-
 from chipsec.hal import hal_base
-from chipsec.logger import logger
 
 #
 # IOSF Message bus message opcodes
 # Reference: http://lxr.free-electrons.com/source/arch/x86/include/asm/iosf_mbi.h
 #
 class MessageBusOpcode:
   MB_OPCODE_MMIO_READ   = 0x00
@@ -112,15 +99,15 @@
         mcr = self.cs.set_register_field( 'MSG_CTRL_REG', mcr, 'MESSAGE_ADDRESS_OFFSET', reg )
         mcr = self.cs.set_register_field( 'MSG_CTRL_REG', mcr, 'MESSAGE_PORT', port )
         mcr = self.cs.set_register_field( 'MSG_CTRL_REG', mcr, 'MESSAGE_OPCODE', opcode )
         return mcr
 
     def __MB_MESSAGE_MCRX(self, reg):
         mcrx = 0x0
-        mcrx = self.cs.set_register_field( 'MSG_CTRL_REG_EXT', mcrx, 'MESSAGE_ADDRESS_OFFSET_EXT', reg, preserve_field_position=True )
+        mcrx = self.cs.set_register_field( 'MSG_CTRL_REG_EXT', mcrx, 'MESSAGE_ADDRESS_OFFSET_EXT', (reg >> 8), preserve_field_position=True )
         return mcrx
 
     def __MB_MESSAGE_MDR(self, data):
         mdr = 0x0
         mdr = self.cs.set_register_field( 'MSG_DATA_REG', mdr, 'MESSAGE_DATA', data )
         return mdr
 
@@ -135,54 +122,54 @@
     #
     # Issues read message on the message bus
     #
     def msgbus_read_message( self, port, register, opcode ):
         mcr  = self.__MB_MESSAGE_MCR(port, register, opcode)
         mcrx = self.__MB_MESSAGE_MCRX(register)
 
-        if logger().HAL: 
-            logger().log( "[msgbus] read: port 0x{:02X} + 0x{:08X} (op = 0x{:02X})".format(port, register, opcode) )
-            logger().log( "[msgbus]       MCR = 0x{:08X}, MCRX = 0x{:08X}".format(mcr, mcrx) )
+        if self.logger.HAL: 
+            self.logger.log( "[msgbus] read: port 0x{:02X} + 0x{:08X} (op = 0x{:02X})".format(port, register, opcode) )
+            self.logger.log( "[msgbus]       MCR = 0x{:08X}, MCRX = 0x{:08X}".format(mcr, mcrx) )
 
         mdr_out = self.helper.msgbus_send_read_message( mcr, mcrx )
 
-        if logger().HAL: logger().log( "[msgbus]       < 0x{:08X}".format(mdr_out) )
+        if self.logger.HAL: self.logger.log( "[msgbus]       < 0x{:08X}".format(mdr_out) )
 
         return mdr_out
 
     #
     # Issues write message on the message bus
     #
     def msgbus_write_message( self, port, register, opcode, data ):
         mcr  = self.__MB_MESSAGE_MCR(port, register, opcode)
         mcrx = self.__MB_MESSAGE_MCRX(register)
         mdr  = self.__MB_MESSAGE_MDR (data)
 
-        if logger().HAL:
-            logger().log( "[msgbus] write: port 0x{:02X} + 0x{:08X} (op = 0x{:02X}) < data = 0x{:08X}".format(port, register, opcode, data) )
-            logger().log( "[msgbus]        MCR = 0x{:08X}, MCRX = 0x{:08X}, MDR = 0x{:08X}".format(mcr, mcrx, mdr) )
+        if self.logger.HAL:
+            self.logger.log( "[msgbus] write: port 0x{:02X} + 0x{:08X} (op = 0x{:02X}) < data = 0x{:08X}".format(port, register, opcode, data) )
+            self.logger.log( "[msgbus]        MCR = 0x{:08X}, MCRX = 0x{:08X}, MDR = 0x{:08X}".format(mcr, mcrx, mdr) )
 
         return self.helper.msgbus_send_write_message( mcr, mcrx, mdr )
 
     #
     # Issues generic message on the message bus
     #
     def msgbus_send_message( self, port, register, opcode, data=None ):
         mcr  = self.__MB_MESSAGE_MCR(port, register, opcode)
         mcrx = self.__MB_MESSAGE_MCRX(register)
         mdr  = None if data is None else self.__MB_MESSAGE_MDR(data)
 
-        if logger().HAL:
-            logger().log( "[msgbus] message: port 0x{:02X} + 0x{:08X} (op = 0x{:02X})".format(port, register, opcode) )
-            if data is not None: logger().log( "[msgbus]          data = 0x{:08X}".format(data) )
-            logger().log( "[msgbus]          MCR = 0x{:08X}, MCRX = 0x{:08X}, MDR = 0x{:08X}".format(mcr, mcrx, mdr) )
+        if self.logger.HAL:
+            self.logger.log( "[msgbus] message: port 0x{:02X} + 0x{:08X} (op = 0x{:02X})".format(port, register, opcode) )
+            if data is not None: self.logger.log( "[msgbus]          data = 0x{:08X}".format(data) )
+            self.logger.log( "[msgbus]          MCR = 0x{:08X}, MCRX = 0x{:08X}, MDR = 0x{:08X}".format(mcr, mcrx, mdr) )
 
         mdr_out = self.helper.msgbus_send_message( mcr, mcrx, mdr )
 
-        if logger().HAL: logger().log( "[msgbus]          < 0x{:08X}".format(mdr_out) )
+        if self.logger.HAL: self.logger.log( "[msgbus]          < 0x{:08X}".format(mdr_out) )
 
         return mdr_out
 
     #
     # Message bus register read/write
     #
 
@@ -211,17 +198,17 @@
         if self.cs.is_register_defined('P2SBC') and was_hidden:
             self.__hide_p2sb(True)
         return reg_val
 
     """
     # py implementation of msgbus -- doesn't seem to work properly becaise it's not atomic
     def msgbus_send_message( self, port, register, opcode, data=None ):
-        if logger().HAL:
-            logger().log( "[msgbus] message - port: 0x{:02X}, reg: 0x{:08X} (op: 0x{:02X})".format(port, register, opcode) )
-            if data is not None: logger().log( "[msgbus] message - data: 0x{:08X}".format(data) )
+        if self.logger.HAL:
+            self.logger.log( "[msgbus] message - port: 0x{:02X}, reg: 0x{:08X} (op: 0x{:02X})".format(port, register, opcode) )
+            if data is not None: self.logger.log( "[msgbus] message - data: 0x{:08X}".format(data) )
         if (register & 0xFFFFFF00):
             # write extended register address (bits [31:08]) to Message Control Register Extension (MCRX)
             chipsec.chipset.write_register_field( self.cs, 'MSG_CTRL_REG_EXT', 'MESSAGE_ADDRESS_OFFSET_EXT', register, preserve_field_position=True )
         res = None
         # write data to Message Data Register (MDR) for writes
         if data is not None: chipsec.chipset.write_register( self.cs, 'MSG_DATA_REG', data )
         # write message (byte enables, address bits [08:00], port and opcode) to Message Control Register (MCR)
```

### Comparing `chipsec-1.4.4/chipsec/hal/igd.py` & `chipsec-1.5.1/chipsec/hal/igd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -28,17 +28,14 @@
 """
 Working with Intel processor Integrated Graphics Device (IGD)
 
 usage:
     >>> gfx_aperture_dma_read(0x80000000, 0x100)
 """
 
-import struct
-import sys
-
 from chipsec.hal import hal_base
 from chipsec.logger import print_buffer
 from chipsec.defines import bytestostring
 
 class IGDRuntimeError (RuntimeError):
     pass
```

### Comparing `chipsec-1.4.4/chipsec/hal/pci.py` & `chipsec-1.5.1/chipsec/hal/pci.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -15,23 +15,14 @@
 #along with this program; if not, write to the Free Software
 #Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
 #Contact information:
 #chipsec@intel.com
 #
 
-
-
-# -------------------------------------------------------------------------------
-#
-# CHIPSEC: Platform Hardware Security Assessment Framework
-# (c) 2010-2018 Intel Corporation
-#
-# -------------------------------------------------------------------------------
-
 """
 Access to of PCI/PCIe device hierarchy
 - enumerating PCI/PCIe devices
 - read/write access to PCI configuration headers/registers
 - enumerating PCI expansion (option) ROMs
 - identifying PCI/PCIe devices MMIO and I/O ranges (BARs)
 
@@ -43,24 +34,21 @@
     >>> self.cs.pci.find_XROM( 2, 0, 0, True, True, 0xFED00000 )
     >>> self.cs.pci.get_device_bars( 2, 0, 0 )
     >>> self.cs.pci.get_DIDVID( 2, 0, 0 )
     >>> self.cs.pci.is_enabled( 2, 0, 0 )
 """
 
 import struct
-import sys
-import os.path
 from collections import namedtuple
 import itertools
 
 from chipsec import defines
 from chipsec.logger import logger, pretty_print_hex_buffer
 from chipsec.file import write_file
-from chipsec.cfg.common import *
-from chipsec.hal.pcidb import *
+from chipsec.hal.pcidb import VENDORS, DEVICES
 from chipsec.helper import oshelper
 
 
 class PciRuntimeError (RuntimeError):
     pass
 class PciDeviceNotFoundError (RuntimeError):
     pass
```

### Comparing `chipsec-1.4.4/chipsec/hal/uefi.py` & `chipsec-1.5.1/chipsec/hal/uefi.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -15,38 +15,34 @@
 #along with this program; if not, write to the Free Software
 #Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
 #Contact information:
 #chipsec@intel.com
 #
 
-
-
-
-# -------------------------------------------------------------------------------
-#
-# CHIPSEC: Platform Hardware Security Assessment Framework
-# (c) 2010-2019 Intel Corporation
-#
-# -------------------------------------------------------------------------------
-
 """
 Main UEFI component using platform specific and common UEFI functionality
 """
 
 import struct
 import sys
+import os
 
 from collections import namedtuple
 import collections
 
 from chipsec.hal import hal_base, mmio, spi, uefi_platform
-from chipsec.hal.uefi_common import *
-from chipsec.logger import *
-from chipsec.file import *
+from chipsec.hal.uefi_common import EFI_VENDOR_TABLE, EFI_VENDOR_TABLE_SIZE, EFI_VENDOR_TABLE_FORMAT, EFI_TABLE_HEADER_SIZE, EFI_TABLE_HEADER, EFI_TABLES,  MAX_EFI_TABLE_SIZE
+from chipsec.hal.uefi_common import S3BootScriptOpcode, S3_BOOTSCRIPT_VARIABLES, parse_efivar_file, EFI_REVISIONS, AUTH_SIG_VAR, ESAL_SIG_VAR
+from chipsec.hal.uefi_common import EFI_VARIABLE_AUTHENTICATED_WRITE_ACCESS, EFI_VARIABLE_TIME_BASED_AUTHENTICATED_WRITE_ACCESS, EFI_VARIABLE_APPEND_WRITE, EFI_VARIABLE_NON_VOLATILE
+from chipsec.hal.uefi_common import EFI_VARIABLE_BOOTSERVICE_ACCESS, EFI_VARIABLE_RUNTIME_ACCESS, EFI_VARIABLE_HARDWARE_ERROR_RECORD, SECURE_BOOT_SIG_VAR
+from chipsec.hal.uefi_common import IS_VARIABLE_ATTRIBUTE, EFI_TABLE_HEADER_FMT, EFI_SYSTEM_TABLE_SIGNATURE, EFI_RUNTIME_SERVICES_SIGNATURE, EFI_BOOT_SERVICES_SIGNATURE
+from chipsec.hal.uefi_common import EFI_DXE_SERVICES_TABLE_SIGNATURE, EFI_CONFIGURATION_TABLE, ACPI_VARIABLE_SET_STRUCT_SIZE
+from chipsec.logger import logger, print_buffer
+from chipsec.file import write_file, read_file
 from chipsec.defines import COMPRESSION_TYPES
 from chipsec.defines import bytestostring
 
 
 ########################################################################################################
 #
 # S3 Resume Boot-Script Parsing Functionality
@@ -71,15 +67,15 @@
         off += s3script_entry.length
 
     if log_script: logger().log( '[uefi] +++ End of S3 Resume Boot-Script +++' )
 
     if logger().HAL: logger().log( '[uefi] S3 Resume Boot-Script size: 0x{:X}'.format(off) )
     if logger().HAL: 
         logger().log( '\n[uefi] [++++++++++ S3 Resume Boot-Script Buffer ++++++++++]' )
-        print_buffer( script[ : off ] )
+        print_buffer( bytestostring(script[ : off ]) )
 
     return s3_boot_script_entries
 
 
 ########################################################################################################
 #
 # UEFI Variables Parsing Functionality
@@ -416,15 +412,15 @@
 
         for efivar_name in efivars:
             (off, buf, hdr, data, guid, attrs) = efivars[efivar_name][0]
             if efivar_name in S3_BOOTSCRIPT_VARIABLES:
                 if logger().HAL: logger().log( "[uefi] found: {} {{{}}} {} variable".format(efivar_name,guid,get_attr_string(attrs)) )
                 if logger().HAL:
                     logger().log('[uefi] {} variable data:'.format(efivar_name))
-                    print_buffer( data )
+                    print_buffer( bytestostring(data) )
 
                 varsz = len(data)
                 if   4 == varsz: AcpiGlobalAddr_fmt = '<L'
                 elif 8 == varsz: AcpiGlobalAddr_fmt = '<Q'
                 else:
                     logger().error( "Unrecognized format of '{}' UEFI variable (data size = 0x{:X})".format(efivar_name,varsz) )
                     break
@@ -433,15 +429,15 @@
                     logger().error( "Pointer to ACPI Global Data structure in {} variable is 0".format(efivar_name) )
                     break
                 if logger().HAL: logger().log( "[uefi] Pointer to ACPI Global Data structure: 0x{:016X}".format( AcpiGlobalAddr ) )
                 if logger().HAL: logger().log( "[uefi] Decoding ACPI Global Data structure.." )
                 AcpiVariableSet = self.helper.read_physical_mem( AcpiGlobalAddr, ACPI_VARIABLE_SET_STRUCT_SIZE )
                 if logger().HAL:
                     logger().log('[uefi] AcpiVariableSet structure:')
-                    print_buffer( AcpiVariableSet )
+                    print_buffer( bytestostring(AcpiVariableSet) )
                 AcpiVariableSet_fmt = '<6Q'
                 #if len(AcpiVariableSet) < struct.calcsize(AcpiVariableSet_fmt):
                 #    logger().error( 'Unrecognized format of AcpiVariableSet structure' )
                 #    return (False,0)
                 AcpiReservedMemoryBase, AcpiReservedMemorySize, S3ReservedLowMemoryBase, AcpiBootScriptTable, RuntimeScriptTableBase, AcpiFacsTable = struct.unpack_from( AcpiVariableSet_fmt, AcpiVariableSet )
                 if logger().HAL: logger().log( '[uefi] ACPI Boot-Script table base = 0x{:016X}'.format(AcpiBootScriptTable) )
                 found   = True
```

### Comparing `chipsec-1.4.4/chipsec/hal/mmio.py` & `chipsec-1.5.1/chipsec/hal/mmio.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -15,22 +15,14 @@
 #along with this program; if not, write to the Free Software
 #Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
 #Contact information:
 #chipsec@intel.com
 #
 
-
-# -------------------------------------------------------------------------------
-#
-# CHIPSEC: Platform Hardware Security Assessment Framework
-# (c) 2010-2018 Intel Corporation
-#
-# -------------------------------------------------------------------------------
-
 """
 Access to MMIO (Memory Mapped IO) BARs and Memory-Mapped PCI Configuration Space (MMCFG)
 
 usage:
     >>> read_MMIO_reg(cs, bar_base, 0x0, 4 )
     >>> write_MMIO_reg(cs, bar_base, 0x0, 0xFFFFFFFF, 4 )
     >>> read_MMIO( cs, bar_base, 0x1000 )
@@ -47,73 +39,33 @@
     >>> list_MMIO_BARs( cs )
 
     Access Memory Mapped Config Space:
 
     >>> get_MMCFG_base_address(cs)
     >>> read_mmcfg_reg( cs, 0, 0, 0, 0x10, 4 )
     >>> read_mmcfg_reg( cs, 0, 0, 0, 0x10, 4, 0xFFFFFFFF )
-
-    DEPRECATED: Access MMIO by BAR id:
-
-    >>> read_MMIOBAR_reg( cs, mmio.MMIO_BAR_MCHBAR, 0x0 )
-    >>> write_MMIOBAR_reg( cs, mmio.MMIO_BAR_MCHBAR, 0xFFFFFFFF )
-    >>> get_MMIO_base_address( cs, mmio.MMIO_BAR_MCHBAR )
 """
 
-import struct
-import sys
-
 from chipsec.hal import hal_base
-from chipsec.logger import logger
-
-from chipsec.cfg.common import *
-
-# CPU
-# Device 0
-MMIO_BAR_MCHBAR      = 1   # MCHBAR
-MMIO_BAR_DMIBAR      = 2   # DMIBAR
-MMIO_BAR_PCIEXBAR    = 3   # PCIEXBAR
-# Device 1
-# @TODO
-# Device 2
-MMIO_BAR_GTTMMADR    = 10  # GFx MMIO
-MMIO_BAR_GMADR       = 11  # GFx Aperture
-# Device 3 (Device 27)
-MMIO_BAR_HDABAR      = 20  # HD Audio MMIO BAR
-# PCH
-# @TODO
-# Device 31
-MMIO_BAR_LPCRCBA     = 100 # ICH LPC Interface Root Complex (RCBA)
-MMIO_BAR_LPCRCBA_SPI = 101 # RCBA SPIBASE
-
-MMIO_BAR_name = {
-    MMIO_BAR_MCHBAR      : "MCHBAR",
-    MMIO_BAR_DMIBAR      : "DMIBAR",
-    MMIO_BAR_PCIEXBAR    : "PCIEXBAR",
-    MMIO_BAR_GMADR       : "GMADR",
-    MMIO_BAR_GTTMMADR    : "GTTMMADR",
-    MMIO_BAR_HDABAR      : "HDABAR",
-    MMIO_BAR_LPCRCBA     : "RCBA"
-}
 
 DEFAULT_MMIO_BAR_SIZE = 0x1000
 
+PCI_PCIEXBAR_REG_LENGTH_256MB  = 0x0
+PCI_PCIEXBAR_REG_LENGTH_128MB  = 0x1
+PCI_PCIEXBAR_REG_LENGTH_64MB   = 0x2
+PCI_PCIEXBAR_REG_LENGTH_512MB  = 0x3
+PCI_PCIEXBAR_REG_LENGTH_1024MB = 0x4
+PCI_PCIEXBAR_REG_LENGTH_2048MB = 0x5
+PCI_PCIEXBAR_REG_LENGTH_4096MB = 0x6
+PCI_PCIEBAR_REG_MASK = 0x7FFC000000
+
 class MMIO(hal_base.HALBase):
 
     def __init__(self, cs):
         super(MMIO, self).__init__(cs)
-        self.MMIO_BAR_base = {
-            MMIO_BAR_MCHBAR      : self.get_MCHBAR_base_address,
-            MMIO_BAR_DMIBAR      : self.get_DMIBAR_base_address,
-            MMIO_BAR_PCIEXBAR    : self.get_PCIEXBAR_base_address,
-            MMIO_BAR_GMADR       : self.get_GMADR_base_address,
-            MMIO_BAR_GTTMMADR    : self.get_GTTMMADR_base_address,
-            MMIO_BAR_HDABAR      : self.get_HDAudioBAR_base_address,
-            MMIO_BAR_LPCRCBA     : self.get_LPC_RCBA_base_address
-        }
 
     ###########################################################################
     # Access to MMIO BAR defined by configuration files (chipsec/cfg/*.py)
     ###########################################################################
     #
     # To add your own MMIO bar:
     #   1. Add new MMIO BAR id (any)
@@ -121,170 +73,58 @@
     #      returns base addres of new bar
     #   3. Add a pointer to this function to MMIO_BAR_base map
     #   4. Don't touch read/write_MMIO_reg functions ;)
     #
     ###########################################################################
 
 
-    #
-    # Dev0 BARs: MCHBAR, DMIBAR
-    #
-    def get_MCHBAR_base_address(self):
-        base = self.cs.pci.read_dword(0, 0, 0, Cfg.PCI_MCHBAR_REG_OFF)
-        if (0 == base & 0x1):
-            logger().warn('MCHBAR is disabled')
-        base = base & 0xFFFFF000
-        if logger().HAL:
-            logger().log('[mmio] MCHBAR: 0x{:016X}'.format(base))
-        return base
-
-    def get_DMIBAR_base_address(self):
-        base_lo = self.cs.pci.read_dword(0, 0, 0, Cfg.PCI_DMIBAR_REG_OFF)
-        base_hi = self.cs.pci.read_dword(0, 0, 0, Cfg.PCI_DMIBAR_REG_OFF + 4)
-        if (0 == base_lo & 0x1) and logger().HAL:
-            logger().warn('DMIBAR is disabled')
-        base = (base_hi << 32) | (base_lo & 0xFFFFF000)
-        if logger().HAL:
-            logger().log( '[mmio] DMIBAR: 0x{:016X}'.format(base) )
-        return base
-
-    #
-    # PCH LPC Interface Root Complex base address (RCBA)
-    #
-    def get_LPC_RCBA_base_address(self):
-        reg_value = self.cs.pci.read_dword(0, 31, 0, Cfg.LPC_RCBA_REG_OFFSET)
-        #RcbaReg = LPC_RCBA_REG( (reg_value>>14)&0x3FFFF, (reg_value>>1)&0x1FFF, reg_value&0x1 )
-        #rcba_base = RcbaReg.BaseAddr << Cfg.RCBA_BASE_ADDR_SHIFT
-        rcba_base = (reg_value >> Cfg.RCBA_BASE_ADDR_SHIFT) << Cfg.RCBA_BASE_ADDR_SHIFT
-        if logger().HAL:
-            logger().log( "[mmio] LPC RCBA: 0x{:08X}".format(rcba_base) )
-        return rcba_base
-
-    #
-    # GFx MMIO: GMADR/GTTMMADR
-    #
-    def get_GFx_base_address(self, dev2_offset):
-        #bar = PCI_BDF(0, 2, 0, dev2_offset)
-        base_lo = self.cs.pci.read_dword(0, 2, 0, dev2_offset)
-        base_hi = self.cs.pci.read_dword(0, 2, 0, dev2_offset + 4)
-        base = base_hi | (base_lo & 0xFF000000)
-        return base
-
-    def get_GMADR_base_address(self):
-        base = self.get_GFx_base_address(Cfg.PCI_GMADR_REG_OFF)
-        if logger().HAL:
-            logger().log( '[mmio] GMADR: 0x{:016X}'.format(base) )
-        return base
-
-    def get_GTTMMADR_base_address(self):
-        base = self.get_GFx_base_address(Cfg.PCI_GTTMMADR_REG_OFF)
-        if logger().HAL:
-            logger().log( '[mmio] GTTMMADR: 0x{:016X}'.format(base) )
-        return base
-
-    #
-    # HD Audio MMIO
-    #
-    def get_HDAudioBAR_base_address(self):
-        base = self.cs.pci.read_dword( 0, Cfg.PCI_HDA_DEV, 0, Cfg.PCI_HDAUDIOBAR_REG_OFF )
-        base = base & (0xFFFFFFFF << 14)
-        if logger().HAL:
-            logger().log( '[mmio] HD Audio MMIO: 0x{:08X}'.format(base) )
-        return base
-
-    #
-    # PCIEXBAR - technically not MMIO but Memory-mapped CFG space (MMCFG)
-    # but defined by BAR similarly to MMIO BARs
-    #
-    def get_PCIEXBAR_base_address(self):
-        base_lo = self.cs.pci.read_dword( 0, 0, 0, Cfg.PCI_PCIEXBAR_REG_OFF )
-        base_hi = self.cs.pci.read_dword( 0, 0, 0, Cfg.PCI_PCIEXBAR_REG_OFF + 4 )
-        if (0 == base_lo & 0x1) and logger().HAL:
-            logger().warn('PCIEXBAR is disabled')
-
-        base_lo &= Cfg.PCI_PCIEXBAR_REG_ADMSK256
-        if (Cfg.PCI_PCIEXBAR_REG_LENGTH_128MB == (base_lo & Cfg.PCI_PCIEXBAR_REG_LENGTH_MASK) >> 1):
-            base_lo |= Cfg.PCI_PCIEXBAR_REG_ADMSK128
-        elif (Cfg.PCI_PCIEXBAR_REG_LENGTH_64MB == (base_lo & Cfg.PCI_PCIEXBAR_REG_LENGTH_MASK) >> 1):
-            base_lo |= (Cfg.PCI_PCIEXBAR_REG_ADMSK128|Cfg.PCI_PCIEXBAR_REG_ADMSK64)
-        base = (base_hi << 32) | base_lo
-        if logger().HAL:
-            logger().log( '[mmio] PCIEXBAR (MMCFG): 0x{:016X}'.format(base) )
-        return base
-
-    #
-    # Get base address of MMIO range by MMIO_BAR_* id
-    #
-    def get_MMIO_base_address(self, bar_id):
-        return self.MMIO_BAR_base[bar_id]
-
-    #
-    # Read MMIO register in MMIO BAR defined by MMIO_BAR_* id
-    #
-    def read_MMIOBAR_reg(self, bar_id, offset ):
-        bar_base  = self.MMIO_BAR_base[ bar_id ]
-        reg_addr  = bar_base + offset
-        reg_value = self.cs.helper.read_mmio_reg( bar_base, 4, offset )
-        if logger().HAL:
-            logger().log( '[mmio] {} + 0x{:08X} (0x{:08X}) = 0x{:08X}'.format(MMIO_BAR_name[bar_id], offset, reg_addr, reg_value) )
-        return reg_value
-
-    #
-    # Write MMIO register in MMIO BAR defined by MMIO_BAR_* id
-    #
-    def write_MMIOBAR_reg(self, bar_id, offset, dword_value):
-        bar_base  = self.MMIO_BAR_base[bar_id]
-        reg_addr  = bar_base + offset
-        if logger().HAL:
-            logger().log('[mmio] write {} + 0x{:08X} (0x{:08X}) = 0x{:08X}'.format(MMIO_BAR_name[bar_id], offset, reg_addr, dword_value) )
-        self.cs.helper.write_mmio_reg(reg_addr, 4, dword_value)
 
 
     #
     # Read MMIO register as an offset off of MMIO range base address
     #
     def read_MMIO_reg(self, bar_base, offset, size=4, bar_size=None ):
         if size > 8:
-            if logger().HAL: logger().warn("MMIO read cannot exceed 8")
+            if self.logger.HAL: self.logger.warn("MMIO read cannot exceed 8")
         reg_value = self.cs.helper.read_mmio_reg( bar_base, size, offset, bar_size )
-        if logger().HAL: logger().log( '[mmio] 0x{:08X} + 0x{:08X} = 0x{:08X}'.format(bar_base, offset, reg_value) )
+        if self.logger.HAL: self.logger.log( '[mmio] 0x{:08X} + 0x{:08X} = 0x{:08X}'.format(bar_base, offset, reg_value) )
         return reg_value
 
     def read_MMIO_reg_byte(self, bar_base, offset ):
         reg_value = self.cs.helper.read_mmio_reg( bar_base, 1, offset )
-        if logger().HAL: logger().log( '[mmio] 0x{:08X} + 0x{:08X} = 0x{:08X}'.format(bar_base, offset, reg_value) )
+        if self.logger.HAL: self.logger.log( '[mmio] 0x{:08X} + 0x{:08X} = 0x{:08X}'.format(bar_base, offset, reg_value) )
         return reg_value
 
     def read_MMIO_reg_word(self, bar_base, offset ):
         reg_value = self.cs.helper.read_mmio_reg( bar_base, 2, offset )
-        if logger().HAL: logger().log( '[mmio] 0x{:08X} + 0x{:08X} = 0x{:08X}'.format(bar_base, offset, reg_value) )
+        if self.logger.HAL: self.logger.log( '[mmio] 0x{:08X} + 0x{:08X} = 0x{:08X}'.format(bar_base, offset, reg_value) )
         return reg_value
 
     def read_MMIO_reg_dword(self, bar_base, offset ):
         reg_value = self.cs.helper.read_mmio_reg( bar_base, 4, offset )
-        if logger().HAL: logger().log( '[mmio] 0x{:08X} + 0x{:08X} = 0x{:08X}'.format(bar_base, offset, reg_value) )
+        if self.logger.HAL: self.logger.log( '[mmio] 0x{:08X} + 0x{:08X} = 0x{:08X}'.format(bar_base, offset, reg_value) )
         return reg_value
 
     #
     # Write MMIO register as an offset off of MMIO range base address
     #
     def write_MMIO_reg(self, bar_base, offset, value, size=4, bar_size=None ):
-        if logger().HAL: logger().log( '[mmio] write 0x{:08X} + 0x{:08X} = 0x{:08X}'.format(bar_base, offset, value) )
+        if self.logger.HAL: self.logger.log( '[mmio] write 0x{:08X} + 0x{:08X} = 0x{:08X}'.format(bar_base, offset, value) )
         self.cs.helper.write_mmio_reg( bar_base, size, value, offset, bar_size )
 
     def write_MMIO_reg_byte(self, bar_base, offset, value ):
-        if logger().HAL: logger().log( '[mmio] write 0x{:08X} + 0x{:08X} = 0x{:08X}'.format(bar_base, offset, value) )
+        if self.logger.HAL: self.logger.log( '[mmio] write 0x{:08X} + 0x{:08X} = 0x{:08X}'.format(bar_base, offset, value) )
         self.cs.helper.write_mmio_reg( bar_base, 1, value, offset )
 
     def write_MMIO_reg_word(self, bar_base, offset, value ):
-        if logger().HAL: logger().log( '[mmio] write 0x{:08X} + 0x{:08X} = 0x{:08X}'.format(bar_base, offset, value) )
+        if self.logger.HAL: self.logger.log( '[mmio] write 0x{:08X} + 0x{:08X} = 0x{:08X}'.format(bar_base, offset, value) )
         self.cs.helper.write_mmio_reg( bar_base, 2, value, offset )
 
     def write_MMIO_reg_dword(self, bar_base, offset, value ):
-        if logger().HAL: logger().log( '[mmio] write 0x{:08X} + 0x{:08X} = 0x{:08X}'.format(bar_base, offset, value) )
+        if self.logger.HAL: self.logger.log( '[mmio] write 0x{:08X} + 0x{:08X} = 0x{:08X}'.format(bar_base, offset, value) )
         self.cs.helper.write_mmio_reg( bar_base, 4, value, offset )
 
     #
     # Read MMIO registers as offsets off of MMIO range base address
     #
     def read_MMIO(self, bar_base, size):
         regs = []
@@ -293,18 +133,18 @@
             regs.append(self.read_MMIO_reg(bar_base, offset))
         return regs
 
     #
     # Dump MMIO range
     #
     def dump_MMIO(self, bar_base, size ):
-        logger().log("[mmio] MMIO register range [0x{:016X}:0x{:016X}+{:08X}]:".format(bar_base, bar_base, size))
+        self.logger.log("[mmio] MMIO register range [0x{:016X}:0x{:016X}+{:08X}]:".format(bar_base, bar_base, size))
         size -= size % 4
         for offset in range(0, size, 4):
-            logger().log( '+{:08X}: {:08X}'.format(offset, self.read_MMIO_reg(bar_base, offset)) )
+            self.logger.log( '+{:08X}: {:08X}'.format(offset, self.read_MMIO_reg(bar_base, offset)) )
 
 
     ###############################################################################
     # Access to MMIO BAR defined by XML configuration files (chipsec/cfg/*.xml)
     ###############################################################################
 
     #
@@ -321,15 +161,15 @@
                 elif ('bus' in _bar) and ('dev' in _bar) and ('fun' in _bar) and ('reg' in _bar):
                     # old definition
                     is_bar_defined = True
         except KeyError:
             pass
 
         if not is_bar_defined:
-            if logger().HAL: logger().warn( "'{}' MMIO BAR definition not found/correct in XML config".format(bar_name) )
+            if self.logger.HAL: self.logger.warn( "'{}' MMIO BAR definition not found/correct in XML config".format(bar_name) )
         return is_bar_defined
 
     #
     # Get base address of MMIO range by MMIO BAR name
     #
     def get_MMIO_BAR_base_address(self, bar_name):
         bar = self.cs.Cfg.MMIO_BARS[ bar_name ]
@@ -358,20 +198,20 @@
                 base_hi = self.cs.pci.read_dword( b, d, f, r + 4 )
                 base = (base_hi << 32) | base_lo
             else:
                 base = self.cs.pci.read_dword( b, d, f, r )
 
         if 'fixed_address' in bar and base == reg_mask:
             base = int(bar['fixed_address'],16)
-            if logger().HAL: logger().log('[mmio] Using fixed address for {}: 0x{:016X}'.format(bar_name, base))
+            if self.logger.HAL: self.logger.log('[mmio] Using fixed address for {}: 0x{:016X}'.format(bar_name, base))
         if 'mask' in bar: base &= int(bar['mask'],16)
         if 'offset' in bar: base = base + int(bar['offset'],16)
         size = int(bar['size'],16) if ('size' in bar) else DEFAULT_MMIO_BAR_SIZE
 
-        if logger().HAL: logger().log( '[mmio] {}: 0x{:016X} (size = 0x{:X})'.format(bar_name,base,size) )
+        if self.logger.HAL: self.logger.log( '[mmio] {}: 0x{:016X} (size = 0x{:X})'.format(bar_name,base,size) )
         return base, size
 
     #
     # Check if MMIO range is enabled by MMIO BAR name
     #
     def is_MMIO_BAR_enabled(self, bar_name):
         bar = self.cs.Cfg.MMIO_BARS[ bar_name ]
@@ -455,63 +295,72 @@
     # Dump MMIO range by MMIO BAR name
     #
     def dump_MMIO_BAR(self, bar_name):
         (bar_base,bar_size) = self.get_MMIO_BAR_base_address(bar_name)
         self.dump_MMIO(bar_base, bar_size)
 
     def list_MMIO_BARs(self):
-        logger().log('')
-        logger().log( '--------------------------------------------------------------------------------' )
-        logger().log( ' MMIO Range   | BAR Register   | Base             | Size     | En? | Description' )
-        logger().log( '--------------------------------------------------------------------------------' )
+        self.logger.log('')
+        self.logger.log( '--------------------------------------------------------------------------------' )
+        self.logger.log( ' MMIO Range   | BAR Register   | Base             | Size     | En? | Description' )
+        self.logger.log( '--------------------------------------------------------------------------------' )
         for _bar_name in self.cs.Cfg.MMIO_BARS:
             if not self.is_MMIO_BAR_defined( _bar_name ): continue
             _bar = self.cs.Cfg.MMIO_BARS[_bar_name]
             try:
                 (_base,_size) = self.get_MMIO_BAR_base_address(_bar_name)
             except:
-                if logger().HAL: logger().log("Unable to find MMIO BAR {}".format(_bar))
+                if self.logger.HAL: self.logger.log("Unable to find MMIO BAR {}".format(_bar))
                 continue
             _en = self.is_MMIO_BAR_enabled( _bar_name)
 
             if 'register' in _bar:
                 _s = _bar['register']
                 if 'offset' in _bar: _s += (' + 0x{:X}'.format(int(_bar['offset'],16)))
             else:
                 _s = '{:02X}:{:02X}.{:01X} + {}'.format( int(_bar['bus'],16),int(_bar['dev'],16),int(_bar['fun'],16),_bar['reg'] )
 
-            logger().log( ' {:12} | {:14} | {:016X} | {:08X} | {:d}   | {}'.format(_bar_name, _s, _base, _size, _en, _bar['desc']) )
+            self.logger.log( ' {:12} | {:14} | {:016X} | {:08X} | {:d}   | {}'.format(_bar_name, _s, _base, _size, _en, _bar['desc']) )
 
 
     ##################################################################################
     # Access to Memory Mapped PCIe Configuration Space
     ##################################################################################
 
     def get_MMCFG_base_address(self):
         (bar_base,bar_size)  = self.get_MMIO_BAR_base_address('MMCFG')
-        # @TODO: temporary w/a
-        #if (Cfg.PCI_PCIEXBAR_REG_LENGTH_256MB == (bar_base & Cfg.PCI_PCIEXBAR_REG_LENGTH_MASK) >> 1):
-        #    bar_base &= ~(Cfg.PCI_PCIEXBAR_REG_ADMSK128|Cfg.PCI_PCIEXBAR_REG_ADMSK64)
-        #elif (Cfg.PCI_PCIEXBAR_REG_LENGTH_128MB == (bar_base & Cfg.PCI_PCIEXBAR_REG_LENGTH_MASK) >> 1):
-        #    bar_base &= ~Cfg.PCI_PCIEXBAR_REG_ADMSK64
-        ##elif (Cfg.PCI_PCIEXBAR_REG_LENGTH_64MB == (bar_base & Cfg.PCI_PCIEXBAR_REG_LENGTH_MASK) >> 1):
-        ##   pass
-        if logger().HAL: logger().log( '[mmcfg] Memory Mapped CFG Base: 0x{:016X}'.format(bar_base) )
+        if self.cs.register_has_field("PCI0.0.0_PCIEXBAR", "LENGTH") and not self.cs.is_server():
+            len = self.cs.read_register_field("PCI0.0.0_PCIEXBAR", "LENGTH")
+            if len == PCI_PCIEXBAR_REG_LENGTH_256MB:
+                bar_base &= (PCI_PCIEBAR_REG_MASK << 2)
+            elif len == PCI_PCIEXBAR_REG_LENGTH_128MB:
+                bar_base &= (PCI_PCIEBAR_REG_MASK << 1)
+            if len == PCI_PCIEXBAR_REG_LENGTH_64MB:
+                bar_base &= (PCI_PCIEBAR_REG_MASK << 0)
+            if len == PCI_PCIEXBAR_REG_LENGTH_512MB:
+                bar_base &= (PCI_PCIEBAR_REG_MASK << 3)
+            if len == PCI_PCIEXBAR_REG_LENGTH_1024MB:
+                bar_base &= (PCI_PCIEBAR_REG_MASK << 4)
+            if len == PCI_PCIEXBAR_REG_LENGTH_2048MB:
+                bar_base &= (PCI_PCIEBAR_REG_MASK << 5)
+            if len == PCI_PCIEXBAR_REG_LENGTH_4096MB:
+                bar_base &= (PCI_PCIEBAR_REG_MASK << 6)
+        if self.logger.HAL: self.logger.log( '[mmcfg] Memory Mapped CFG Base: 0x{:016X}'.format(bar_base) )
         return bar_base, bar_size
 
     def read_mmcfg_reg(self, bus, dev, fun, off, size):
         pciexbar, pciexbar_sz = self.get_MMCFG_base_address()
         pciexbar_off = (bus * 32 * 8 + dev * 8 + fun) * 0x1000 + off
         value = self.read_MMIO_reg(pciexbar, pciexbar_off, 4, pciexbar_sz)
-        if logger().HAL: logger().log( "[mmcfg] reading {:02d}:{:02d}.{:d} + 0x{:02X} (MMCFG + 0x{:08X}): 0x{:08X}".format(bus, dev, fun, off, pciexbar_off, value) )
+        if self.logger.HAL: self.logger.log( "[mmcfg] reading {:02d}:{:02d}.{:d} + 0x{:02X} (MMCFG + 0x{:08X}): 0x{:08X}".format(bus, dev, fun, off, pciexbar_off, value) )
         if 1 == size:
             return (value & 0xFF)
         elif 2 == size:
             return (value & 0xFFFF)
         return value
 
     def write_mmcfg_reg(self, bus, dev, fun, off, size, value):
         pciexbar, pciexbar_sz = self.get_MMCFG_base_address()
         pciexbar_off = (bus * 32 * 8 + dev * 8 + fun) * 0x1000 + off
         self.write_MMIO_reg(pciexbar, pciexbar_off, (value&0xFFFFFFFF),4,pciexbar_sz)
-        if logger().HAL: logger().log( "[mmcfg] writing {:02d}:{:02d}.{:d} + 0x{:02X} (MMCFG + 0x{:08X}): 0x{:08X}".format(bus, dev, fun, off, pciexbar_off, value) )
+        if self.logger.HAL: self.logger.log( "[mmcfg] writing {:02d}:{:02d}.{:d} + 0x{:02X} (MMCFG + 0x{:08X}): 0x{:08X}".format(bus, dev, fun, off, pciexbar_off, value) )
         return True
```

### Comparing `chipsec-1.4.4/chipsec/hal/tpm.py` & `chipsec-1.5.1/chipsec/hal/tpm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -24,19 +24,17 @@
 Trusted Platform Module (TPM) HAL component
 
 https://trustedcomputinggroup.org
 """
 
 import struct
 import sys
-import time
 from collections import namedtuple
 
-from chipsec.logger import *
-from chipsec.file import *
+from chipsec.logger import print_buffer
 from chipsec.hal import hal_base
 
 import chipsec.hal.tpm12_commands
 
 class TpmRuntimeError (RuntimeError):
     pass
 
@@ -207,15 +205,15 @@
     def command( self, commandName, locality, command_argv ):
         """
         Send command to the TPM and receive data
         """
         try:
             Locality = LOCALITY[locality]
         except:
-            if logger().HAL: logger().log_bad("Invalid locality value\n")
+            if self.logger.HAL: self.logger.log_bad("Invalid locality value\n")
             return
 
         requestedUse = False
 
         #
         # Request locality use if needed
         #
@@ -227,17 +225,17 @@
         #
         # Build command (big endian) and send/receive 
         #
         ( command, size ) = COMMANDS[commandName]( command_argv )
         self._send_command( Locality, command, size )
 
         ( header, data, header_blob, data_blob ) = self._read_response( Locality )
-        logger().log( header )
+        self.logger.log( header )
         print_buffer( str(data_blob) )
-        logger().log( '\n' )
+        self.logger.log( '\n' )
 
         #
         # Release locality if needed
         #
         if requestedUse==True:
             self.helper.write_mmio_reg( access_address, 4, BEENSEIZED )
         self.helper.write_mmio_reg( access_address, 1, ACTIVELOCALITY )
@@ -262,15 +260,18 @@
             sts_value = self.helper.read_mmio_reg( sts_address, 1 )
 
         while count < size:
             sts_value = self.helper.read_mmio_reg( sts_address, 4 )
             burst_count = ( ( sts_value>>8 ) & 0xFFFFFF )
             burst_index = 0
             while ( burst_index < burst_count ) and ( count < size ):
-                self.helper.write_mmio_reg( datafifo_address, 1, struct.unpack("=B", command[count])[0] )
+                datafifo_value = command[count]
+                if sys.version_info.major == 2:
+                    datafifo_value = struct.unpack("=B", datafifo_value)[0]
+                self.helper.write_mmio_reg( datafifo_address, 1, datafifo_value )
                 count += 1
                 burst_index += 0x1
 
         self.helper.write_mmio_reg( sts_address, 1, TPMGO )
 
     def _read_response(self, Locality):
         """
@@ -327,142 +328,142 @@
     def dump_access( self, locality ):
         """
         View the contents of the register used to gain ownership of the TPM
         """
         try:
             Locality = LOCALITY[locality]
         except:
-            if logger().HAL: logger().log_bad("Invalid locality value\n")
+            if self.logger.HAL: self.logger.log_bad("Invalid locality value\n")
             return
 
         access_address = self.TPM_BASE | Locality| TPM_ACCESS 
         access_value = self.helper.read_mmio_reg( access_address, 1 )
 
-        logger().log( "================================================================" )
-        logger().log( "                        TPM Access" )
-        logger().log( "================================================================" )
-        logger().log( "\ttpmRegValidSts  : 0x{}".format(bin( access_value & ( 1<<7 ) )[2]) )
-        logger().log( "\treserved        : 0x{}".format(bin( access_value & ( 1<<6 ) )[2]) )
-        logger().log( "\tactiveLocality  : 0x{}".format(bin( access_value & ( 1<<5 ) )[2]) )
-        logger().log( "\tbeenSeized      : 0x{}".format(bin( access_value & ( 1<<4 ) )[2]) )
-        logger().log( "\tSeize           : 0x{}".format(bin( access_value & ( 1<<3 ) )[2]) )
-        logger().log( "\tpendingRequest  : 0x{}".format(bin( access_value & ( 1<<2 ) )[2]) )
-        logger().log( "\trequestUse      : 0x{}".format(bin( access_value & ( 1<<1 ) )[2]) )
-        logger().log( "\ttpmEstablishment: 0x{}".format(bin( access_value & ( 1<<0 ) )[2]) )
+        self.logger.log( "================================================================" )
+        self.logger.log( "                        TPM Access" )
+        self.logger.log( "================================================================" )
+        self.logger.log( "\ttpmRegValidSts  : 0x{}".format(bin( access_value & ( 1<<7 ) )[2]) )
+        self.logger.log( "\treserved        : 0x{}".format(bin( access_value & ( 1<<6 ) )[2]) )
+        self.logger.log( "\tactiveLocality  : 0x{}".format(bin( access_value & ( 1<<5 ) )[2]) )
+        self.logger.log( "\tbeenSeized      : 0x{}".format(bin( access_value & ( 1<<4 ) )[2]) )
+        self.logger.log( "\tSeize           : 0x{}".format(bin( access_value & ( 1<<3 ) )[2]) )
+        self.logger.log( "\tpendingRequest  : 0x{}".format(bin( access_value & ( 1<<2 ) )[2]) )
+        self.logger.log( "\trequestUse      : 0x{}".format(bin( access_value & ( 1<<1 ) )[2]) )
+        self.logger.log( "\ttpmEstablishment: 0x{}".format(bin( access_value & ( 1<<0 ) )[2]) )
 
     def dump_status( self, locality ):
         """
         View general status details
         """
         try:
             Locality = LOCALITY[locality]
         except:
-            if logger().HAL: logger().log_bad("Invalid locality value\n")
+            if self.logger.HAL: self.logger.log_bad("Invalid locality value\n")
             return
 
         sts_address = self.TPM_BASE | Locality| TPM_STS 
         sts_value = self.helper.read_mmio_reg( sts_address, 4 )
 
-        logger().log( "================================================================" )
-        logger().log( "                         TPM Status" )
-        logger().log( "================================================================" )
-        logger().log( "\tburstCount   : 0x{:x}".format( ( sts_value>>8 ) & 0xFFFFFF ) )
-        logger().log( "\tstsValid     : 0x{}".format(bin( sts_value & ( 1<<7 ) )[2]) )
-        logger().log( "\tcommandReady : 0x{}".format(bin( sts_value & ( 1<<6 ) )[2]) )
-        logger().log( "\ttpmGo        : 0x{}".format(bin( sts_value & ( 1<<5 ) )[2]) )
-        logger().log( "\tdataAvail    : 0x{}".format(bin( sts_value & ( 1<<4 ) )[2]) )
-        logger().log( "\tExpect       : 0x{}".format(bin( sts_value & ( 1<<3 ) )[2]) )
-        logger().log( "\tReserved     : 0x{}".format(bin( sts_value & ( 1<<2 ) )[2]) )
-        logger().log( "\tresponseRetry: 0x{}".format(bin( sts_value & ( 1<<1 ) )[2]) )
-        logger().log( "\tReserved     : 0x{}".format(bin( sts_value & ( 1<<0 ) )[2]) )
+        self.logger.log( "================================================================" )
+        self.logger.log( "                         TPM Status" )
+        self.logger.log( "================================================================" )
+        self.logger.log( "\tburstCount   : 0x{:x}".format( ( sts_value>>8 ) & 0xFFFFFF ) )
+        self.logger.log( "\tstsValid     : 0x{}".format(bin( sts_value & ( 1<<7 ) )[2]) )
+        self.logger.log( "\tcommandReady : 0x{}".format(bin( sts_value & ( 1<<6 ) )[2]) )
+        self.logger.log( "\ttpmGo        : 0x{}".format(bin( sts_value & ( 1<<5 ) )[2]) )
+        self.logger.log( "\tdataAvail    : 0x{}".format(bin( sts_value & ( 1<<4 ) )[2]) )
+        self.logger.log( "\tExpect       : 0x{}".format(bin( sts_value & ( 1<<3 ) )[2]) )
+        self.logger.log( "\tReserved     : 0x{}".format(bin( sts_value & ( 1<<2 ) )[2]) )
+        self.logger.log( "\tresponseRetry: 0x{}".format(bin( sts_value & ( 1<<1 ) )[2]) )
+        self.logger.log( "\tReserved     : 0x{}".format(bin( sts_value & ( 1<<0 ) )[2]) )
 
     def dump_didvid( self, locality ):
         """ 
         TPM's Vendor and Device ID
         """
         try:
             Locality = LOCALITY[locality]
         except:
-            if logger().HAL: logger().log_bad("Invalid locality value\n")
+            if self.logger.HAL: self.logger.log_bad("Invalid locality value\n")
             return
 
         didvid_address = self.TPM_BASE | Locality| TPM_DIDVID 
         didvid_value = self.helper.read_mmio_reg( didvid_address, 4 )
 
-        logger().log( "================================================================" )
-        logger().log( "                           TPM DID VID" )
-        logger().log( "================================================================" )
-        logger().log( "\tdid: 0x{:x}".format( ( didvid_value>>16 ) & 0xFFFF ) )
-        logger().log( "\tvid: 0x{:x}".format( didvid_value & 0xFFFF) )
+        self.logger.log( "================================================================" )
+        self.logger.log( "                           TPM DID VID" )
+        self.logger.log( "================================================================" )
+        self.logger.log( "\tdid: 0x{:x}".format( ( didvid_value>>16 ) & 0xFFFF ) )
+        self.logger.log( "\tvid: 0x{:x}".format( didvid_value & 0xFFFF) )
 
     def dump_rid( self, locality ):
         """
         TPM's Revision ID
         """
         try:
             Locality = LOCALITY[locality]
         except:
-            if logger().HAL: logger().log_bad("Invalid locality value\n")
+            if self.logger.HAL: self.logger.log_bad("Invalid locality value\n")
             return
 
         rid_address = self.TPM_BASE | Locality| TPM_RID 
         rid_value = self.helper.read_mmio_reg( rid_address, 1 )
 
-        logger().log( "================================================================" )
-        logger().log( "                             TPM RID" )
-        logger().log( "================================================================" )
-        logger().log( "\trid: 0x{:x}".format(rid_value) )
+        self.logger.log( "================================================================" )
+        self.logger.log( "                             TPM RID" )
+        self.logger.log( "================================================================" )
+        self.logger.log( "\trid: 0x{:x}".format(rid_value) )
 
     def dump_intcap( self, locality ):
         """
         Provides information of which interrupts that particular TPM supports
         """
         try:
             Locality = LOCALITY[locality]
         except:
-            if logger().HAL: logger().log_bad("Invalid locality value\n")
+            if self.logger.HAL: self.logger.log_bad("Invalid locality value\n")
             return
 
         intcap_address = self.TPM_BASE | Locality| TPM_INTCAP
         intcap_value = self.helper.read_mmio_reg( intcap_address, 4 )
 
-        logger().log( "================================================================" )
-        logger().log( "                     TPM INTF CAPABILITY" )
-        logger().log( "================================================================" )
-        logger().log( "\tReserved                : 0x{:x}".format( ( intcap_value>>8 ) & 0xFFFFFE ) )
-        logger().log( "\tBurstCountStatic        : 0x{}".format(bin( intcap_value & ( 1<<8 ) )[2]) )
-        logger().log( "\tCommandReadyIntSupport  : 0x{}".format(bin( intcap_value & ( 1<<7 ) )[2]) )
-        logger().log( "\tInterruptEdgeFalling    : 0x{}".format(bin( intcap_value & ( 1<<6 ) )[2]) )
-        logger().log( "\tInterruptEdgeRising     : 0x{}".format(bin( intcap_value & ( 1<<5 ) )[2]) )
-        logger().log( "\tInterruptLevelLow       : 0x{}".format(bin( intcap_value & ( 1<<4 ) )[2]) )
-        logger().log( "\tInterruptLevelHigh      : 0x{}".format(bin( intcap_value & ( 1<<3 ) )[2]) )
-        logger().log( "\tLocalityChangeIntSupport: 0x{}".format(bin( intcap_value & ( 1<<2 ) )[2]) )
-        logger().log( "\tstsValidIntSupport      : 0x{}".format(bin( intcap_value & ( 1<<1 ) )[2]) )
-        logger().log( "\tdataAvailIntSupport     : 0x{}".format(bin( intcap_value & ( 1<<0 ) )[2]) )
+        self.logger.log( "================================================================" )
+        self.logger.log( "                     TPM INTF CAPABILITY" )
+        self.logger.log( "================================================================" )
+        self.logger.log( "\tReserved                : 0x{:x}".format( ( intcap_value>>8 ) & 0xFFFFFE ) )
+        self.logger.log( "\tBurstCountStatic        : 0x{}".format(bin( intcap_value & ( 1<<8 ) )[2]) )
+        self.logger.log( "\tCommandReadyIntSupport  : 0x{}".format(bin( intcap_value & ( 1<<7 ) )[2]) )
+        self.logger.log( "\tInterruptEdgeFalling    : 0x{}".format(bin( intcap_value & ( 1<<6 ) )[2]) )
+        self.logger.log( "\tInterruptEdgeRising     : 0x{}".format(bin( intcap_value & ( 1<<5 ) )[2]) )
+        self.logger.log( "\tInterruptLevelLow       : 0x{}".format(bin( intcap_value & ( 1<<4 ) )[2]) )
+        self.logger.log( "\tInterruptLevelHigh      : 0x{}".format(bin( intcap_value & ( 1<<3 ) )[2]) )
+        self.logger.log( "\tLocalityChangeIntSupport: 0x{}".format(bin( intcap_value & ( 1<<2 ) )[2]) )
+        self.logger.log( "\tstsValidIntSupport      : 0x{}".format(bin( intcap_value & ( 1<<1 ) )[2]) )
+        self.logger.log( "\tdataAvailIntSupport     : 0x{}".format(bin( intcap_value & ( 1<<0 ) )[2]) )
 
     def dump_intenable( self, locality ):
         """
         View the contents of the register used to enable specific interrupts
         """
         polType = { 0:"High Level", 1:"Low Level", 2:"Rising edge", 3:"Failing edge" }
 
         try:
             Locality = LOCALITY[locality]
         except:
-            if logger().HAL: logger().log_bad("Invalid locality value\n")
+            if self.logger.HAL: self.logger.log_bad("Invalid locality value\n")
             return
 
         intenable_address = self.TPM_BASE | Locality| TPM_INTENABLE
         intenable_value = self.helper.read_mmio_reg( intenable_address, 4 )
 
-        logger().log( "================================================================" )
-        logger().log( "                         TPM INT ENABLE" )
-        logger().log( "================================================================" )
-        logger().log( "\tglobalIntEnable        : 0x{}".format(bin( intenable_value & ( 1<<31 ) )[2]) )
-        logger().log( "\tReserved               : 0x{:x}".format( (intenable_value>>8) & 0x7FFFFF00 ) )
-        logger().log( "\tcommandReadyEnable     : 0x{}".format(bin( intenable_value & ( 1<<7 ) )[2]) )
-        logger().log( "\tReserved               : 0x{:x}".format( (intenable_value>>5) & 0x3  ) )
+        self.logger.log( "================================================================" )
+        self.logger.log( "                         TPM INT ENABLE" )
+        self.logger.log( "================================================================" )
+        self.logger.log( "\tglobalIntEnable        : 0x{}".format(bin( intenable_value & ( 1<<31 ) )[2]) )
+        self.logger.log( "\tReserved               : 0x{:x}".format( (intenable_value>>8) & 0x7FFFFF00 ) )
+        self.logger.log( "\tcommandReadyEnable     : 0x{}".format(bin( intenable_value & ( 1<<7 ) )[2]) )
+        self.logger.log( "\tReserved               : 0x{:x}".format( (intenable_value>>5) & 0x3  ) )
         type = ( ( intenable_value>>3 ) & 0x3 )
-        logger().log( "\ttypePolarity           : 0x{:x}  {}".format( type, polType[type] ) )
-        logger().log( "\tlocalityChangeIntEnable: 0x{}".format(bin( intenable_value & ( 1<<2 ) )[2]) )
-        logger().log( "\tstsValidIntEnable      : 0x{}".format(bin( intenable_value & ( 1<<1 ) )[2]) )
-        logger().log( "\tdataAvailIntEnable     : 0x{}".format(bin( intenable_value & ( 1<<0 ) )[2]) )
+        self.logger.log( "\ttypePolarity           : 0x{:x}  {}".format( type, polType[type] ) )
+        self.logger.log( "\tlocalityChangeIntEnable: 0x{}".format(bin( intenable_value & ( 1<<2 ) )[2]) )
+        self.logger.log( "\tstsValidIntEnable      : 0x{}".format(bin( intenable_value & ( 1<<1 ) )[2]) )
+        self.logger.log( "\tdataAvailIntEnable     : 0x{}".format(bin( intenable_value & ( 1<<0 ) )[2]) )
```

### Comparing `chipsec-1.4.4/chipsec/hal/uefi_search.py` & `chipsec-1.5.1/chipsec/hal/uefi_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -34,15 +34,16 @@
    >>> chipsec.hal.uefi_search.check_match_criteria(efi_module, match_criteria, self.logger)
 """
 
 import re
 import binascii
 
 from chipsec import defines
-from chipsec.hal.spi_uefi import *
+from chipsec.hal.spi_uefi import EFI_SECTION
+from chipsec.logger import logger
 
 #
 # - EFI binaries are searched according to criteria defined by "match" rules.
 # - EFI binaries matching exclusion criteria defined by "exclude" rules are excluded from matching.
 #
 # Format of the matching rules (any field can be empty or missing):
 # - Individual rules are OR'ed
```

### Comparing `chipsec-1.4.4/chipsec/hal/spi_uefi.py` & `chipsec-1.5.1/chipsec/hal/spi_uefi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -30,31 +30,32 @@
 UEFI firmware image parsing and manipulation functionality
 
 usage:
     >>> parse_uefi_region_from_file(_uefi, filename, fwtype, outpath):
 """
 
 import os
-import fnmatch
 import struct
-import sys
-import time
-import collections
 import hashlib
 import re
 import random
-import binascii
 import json
+import string
 
-from chipsec.logger import *
-from chipsec.file import *
-
-from chipsec.cfg.common import *
-from chipsec.hal.uefi_common import *
-from chipsec.hal.uefi_platform import *
+from chipsec.logger import logger
+from chipsec.file import write_file, read_file
+from chipsec.defines import bytestostring, COMPRESSION_TYPE_LZMA, COMPRESSION_TYPE_EFI_STANDARD, COMPRESSION_TYPES_ALGORITHMS, COMPRESSION_TYPE_UNKNOWN
+from chipsec.hal.uefi_common import EFI_SECTION_PE32, EFI_SECTION_TE, EFI_SECTION_PIC, EFI_SECTION_RAW, SECTION_NAMES, EFI_SECTIONS_EXE, EFI_SECTION_USER_INTERFACE
+from chipsec.hal.uefi_common import NextFwVolume, bit_set, NextFwFile, NextFwVolume, NextFwFileSection, guid_size, GUID, guid_str, GetFvHeader
+from chipsec.hal.uefi_common import EFI_FVB2_ERASE_POLARITY, EFI_FIRMWARE_FILE_SYSTEM2_GUID, EFI_FIRMWARE_FILE_SYSTEM_GUID, FILE_TYPE_NAMES, EFI_FS_GUIDS, EFI_FV_FILETYPE_RAW
+from chipsec.hal.uefi_common import EFI_FILE_HEADER_VALID, EFI_FILE_HEADER_INVALID, EFI_FILE_HEADER_CONSTRUCTION, EFI_FV_FILETYPE_ALL, EFI_FV_FILETYPE_FFS_PAD
+from chipsec.hal.uefi_common import EFI_SECTION_FIRMWARE_VOLUME_IMAGE, EFI_FV_FILETYPE_ALL, EFI_SECTION_GUID_DEFINED, EFI_GUID_DEFINED_SECTION, EFI_SECTION_COMPATIBILITY16
+from chipsec.hal.uefi_common import EFI_GUID_DEFINED_SECTION_size, EFI_CRC32_GUIDED_SECTION_EXTRACTION_PROTOCOL_GUID, LZMA_CUSTOM_DECOMPRESS_GUID, TIANO_DECOMPRESSED_GUID
+from chipsec.hal.uefi_common import EFI_CERT_TYPE_RSA_2048_SHA256_GUID, EFI_CERT_TYPE_RSA_2048_SHA256_GUID_size, EFI_SECTION_COMPRESSION, EFI_COMPRESSION_SECTION_size
+from chipsec.hal.uefi_platform import FWType, ParsePFS, fw_types, EFI_NVRAM_GUIDS, EFI_PLATFORM_FS_GUIDS, NVAR_NVRAM_FS_FILE
 from chipsec.hal.uefi import identify_EFI_NVRAM
 
 CMD_UEFI_FILE_REMOVE        = 0
 CMD_UEFI_FILE_INSERT_BEFORE = 1
 CMD_UEFI_FILE_INSERT_AFTER  = 2
 CMD_UEFI_FILE_REPLACE       = 3
 
@@ -172,15 +173,15 @@
 
     def __str__(self):
         _ind = self.indent + DEF_INDENT
         _s = ''
         if self.MD5   : _s  = "\n{}MD5   : {}".format(_ind,self.MD5)
         if self.SHA1  : _s += "\n{}SHA1  : {}".format(_ind,self.SHA1)
         if self.SHA256: _s += "\n{}SHA256: {}".format(_ind,self.SHA256)
-        return _s
+        return bytestostring(_s)
 
     def calc_hashes( self, off=0 ):
         if self.Image is None: return
         hmd5 = hashlib.md5()
         hmd5.update( self.Image[off:] )
         self.MD5 = hmd5.hexdigest()
         hsha1 = hashlib.sha1()
@@ -200,15 +201,15 @@
         self.CalcSum         = CalcSum
 
     def __str__(self):
         schecksum = ('{:04X}h ({:04X}h) *** checksum mismatch ***'.format(self.Checksum,self.CalcSum)) if self.CalcSum != self.Checksum else ('{:04X}h'.format(self.Checksum))
         _s = "\n{}{} +{:08X}h {{{}}}: ".format(self.indent,type(self).__name__,self.Offset,self.Guid)
         _s += "Size {:08X}h, Attr {:08X}h, HdrSize {:04X}h, ExtHdrOffset {:08X}h, Checksum {}".format(self.Size,self.Attributes,self.HeaderSize,self.ExtHeaderOffset,schecksum)
         _s += super(EFI_FV, self).__str__()
-        return _s
+        return bytestostring(_s)
 
 class EFI_FILE(EFI_MODULE):
     def __init__(self, Offset, Guid, Type, Attributes, State, Checksum, Size, Image, HeaderSize, UD, CalcSum):
         super(EFI_FILE, self).__init__(Offset, Guid, HeaderSize, Attributes, Image)
         self.Name        = Guid
         self.Type        = Type
         self.State       = State
@@ -217,15 +218,15 @@
         self.UD          = UD
         self.CalcSum     = CalcSum
 
     def __str__(self):
         schecksum = ('{:04X}h ({:04X}h) *** checksum mismatch ***'.format(self.Checksum,self.CalcSum)) if self.CalcSum != self.Checksum else ('{:04X}h'.format(self.Checksum))
         _s = "\n{}+{:08X}h {}\n{}Type {:02X}h, Attr {:08X}h, State {:02X}h, Size {:06X}h, Checksum {}".format(self.indent,self.Offset,self.name(),self.indent,self.Type,self.Attributes,self.State,self.Size,schecksum)
         _s += (super(EFI_FILE, self).__str__() + '\n')
-        return _s
+        return bytestostring(_s)
 
 class EFI_SECTION(EFI_MODULE):
     def __init__(self, Offset, Name, Type, Image, HeaderSize):
         super(EFI_SECTION, self).__init__(Offset, None, HeaderSize, None, Image)
         self.Name        = Name
         self.Type        = Type
         self.DataOffset  = None
@@ -240,15 +241,15 @@
     def __str__(self):
         _s = "{}+{:08X}h {}: Type {:02X}h".format(self.indent,self.Offset,self.name(),self.Type)
         if self.Guid: _s += " GUID {{{}}}".format(self.Guid)
         if self.Attributes: _s += " Attr {:04X}h".format(self.Attributes)
         if self.DataOffset: _s += " DataOffset {:04X}h".format(self.DataOffset)
         if self.Comments: _s += "Comments {}".format(self.Comments)
         _s += super(EFI_SECTION, self).__str__()
-        return _s
+        return bytestostring(_s)
 
 
 def build_efi_modules_tree( _uefi, fwtype, data, Size, offset, polarity ):
     sections = []
     secn = 0
 
     _off, next_offset, _name, _type, _img, _hdrsz = NextFwFileSection( data, Size, offset, polarity )
@@ -267,61 +268,66 @@
                     sec.ui_string = sec.Image[sec.HeaderSize:-2].decode("utf-16")
                 except UnicodeDecodeError:
                     pass
             elif sec.Type == EFI_SECTION_GUID_DEFINED:
                 if len(sec.Image) < sec.HeaderSize+EFI_GUID_DEFINED_SECTION_size:
                     logger().warn("EFI Section seems to be malformed")
                     if len(sec.Image) < sec.HeaderSize+guid_size:
-                        logger().warn("Creating fake GUID of 0000-00-00-0000")
-                        guid0 = "0000"
-                        guid1 = "00"
-                        guid2 = "00"
-                        guid3 = "0000"
+                        logger().warn("Creating fake GUID of 0000-00-00-0000000")
+                        guid0 = b"\x00\x00\x00\x00"
+                        guid1 = b"\x00\x00"
+                        guid2 = b"\x00\x00"
+                        guid3 = b"\x00\x00\x00\x00\x00\x00\x00\x00"
                     else:
                         guid0, guid1, guid2, guid3 = struct.unpack(GUID, sec.Image[sec.HeaderSize:sec.HeaderSize+guid_size])
                         sec.DataOffset = len(sec.Image)-1
                 else:
                     guid0, guid1, guid2, guid3, sec.DataOffset, sec.Attributes = struct.unpack(EFI_GUID_DEFINED_SECTION, sec.Image[sec.HeaderSize:sec.HeaderSize+EFI_GUID_DEFINED_SECTION_size])
                 sec.Guid = guid_str(guid0, guid1, guid2, guid3)
 
-            # "container" sections: keep parsing
-            if sec.Type in (EFI_SECTION_COMPRESSION, EFI_SECTION_GUID_DEFINED, EFI_SECTION_FIRMWARE_VOLUME_IMAGE):
-                if sec.Type == EFI_SECTION_COMPRESSION:
-                    for mct in COMPRESSION_TYPES_ALGORITHMS:
-                        d = decompress_section_data( _uefi, "", sec_fs_name, sec.Image[sec.HeaderSize+EFI_COMPRESSION_SECTION_size:], mct, True )
-                        if d:
-                            sec.children = build_efi_modules_tree( _uefi, fwtype, d, len(d), 0, polarity )
-                        if sec.children:
-                            break
-                elif sec.Type == EFI_SECTION_GUID_DEFINED:
-                    if sec.Guid == EFI_CRC32_GUIDED_SECTION_EXTRACTION_PROTOCOL_GUID:
-                        sec.children = build_efi_modules_tree( _uefi, fwtype, sec.Image[sec.DataOffset:], Size - sec.DataOffset, 0, polarity )
-                    elif sec.Guid == LZMA_CUSTOM_DECOMPRESS_GUID or sec.Guid == TIANO_DECOMPRESSED_GUID:
-                        if sec.Guid == LZMA_CUSTOM_DECOMPRESS_GUID:
-                            d = decompress_section_data( _uefi, "", sec_fs_name, sec.Image[sec.DataOffset:], chipsec.defines.COMPRESSION_TYPE_LZMA, True )
-                        else:
-                            d = decompress_section_data( _uefi, "", sec_fs_name, sec.Image[sec.DataOffset:], chipsec.defines.COMPRESSION_TYPE_EFI_STANDARD, True )
-                        if d is None:
-                            sec.Comments = "Unable to decompress image"
-                            d = decompress_section_data( _uefi, "", sec_fs_name, sec.Image[sec.HeaderSize+EFI_GUID_DEFINED_SECTION_size:], chipsec.defines.COMPRESSION_TYPE_UNKNOWN, True )
-                        if d:
-                            sec.children = build_efi_modules_tree( _uefi, fwtype, d, len(d), 0, polarity )
-                    elif sec.Guid == EFI_CERT_TYPE_RSA_2048_SHA256_GUID:
-                        offset = sec.DataOffset + EFI_CERT_TYPE_RSA_2048_SHA256_GUID_size
-                        sec.Comments = "Certificate Type RSA2048/SHA256"
-                        if len(sec.Image) > offset:
-                            sec.children = build_efi_modules_tree( _uefi, fwtype, sec.Image[offset:], len(sec.Image[offset:]),0,polarity)
+                if sec.Guid == EFI_CRC32_GUIDED_SECTION_EXTRACTION_PROTOCOL_GUID:
+                    sec.children = build_efi_modules_tree( _uefi, fwtype, sec.Image[sec.DataOffset:], Size - sec.DataOffset, 0, polarity )
+                elif sec.Guid == LZMA_CUSTOM_DECOMPRESS_GUID or sec.Guid == TIANO_DECOMPRESSED_GUID:
+                    if sec.Guid == LZMA_CUSTOM_DECOMPRESS_GUID:
+                        d = decompress_section_data( _uefi, "", sec_fs_name, sec.Image[sec.DataOffset:], COMPRESSION_TYPE_LZMA, True )
                     else:
-                        sec.children = build_efi_model( _uefi, sec.Image[sec.HeaderSize:], fwtype )
-                elif sec.Type == EFI_SECTION_FIRMWARE_VOLUME_IMAGE:
-                    children = build_efi_file_tree( _uefi, sec.Image[sec.HeaderSize:], fwtype )
-                    if not children is None:
-                        sec.children = children
-            if sec.Type not in SECTION_NAMES.keys() or sec.Type == EFI_SECTION_RAW:
+                        d = decompress_section_data( _uefi, "", sec_fs_name, sec.Image[sec.DataOffset:], COMPRESSION_TYPE_EFI_STANDARD, True )
+                    if d is None:
+                        sec.Comments = "Unable to decompress image"
+                        d = decompress_section_data( _uefi, "", sec_fs_name, sec.Image[sec.HeaderSize+EFI_GUID_DEFINED_SECTION_size:], COMPRESSION_TYPE_UNKNOWN, True )
+                    if d:
+                        sec.children = build_efi_modules_tree( _uefi, fwtype, d, len(d), 0, polarity )
+                elif sec.Guid == EFI_CERT_TYPE_RSA_2048_SHA256_GUID:
+                    offset = sec.DataOffset + EFI_CERT_TYPE_RSA_2048_SHA256_GUID_size
+                    sec.Comments = "Certificate Type RSA2048/SHA256"
+                    if len(sec.Image) > offset:
+                        sec.children = build_efi_modules_tree( _uefi, fwtype, sec.Image[offset:], len(sec.Image[offset:]),0,polarity)
+                else:
+                    sec.children = build_efi_model( _uefi, sec.Image[sec.HeaderSize:], fwtype )
+
+            elif sec.Type == EFI_SECTION_COMPRESSION:
+                for mct in COMPRESSION_TYPES_ALGORITHMS:
+                    d = decompress_section_data( _uefi, "", sec_fs_name, sec.Image[sec.HeaderSize+EFI_COMPRESSION_SECTION_size:], mct, True )
+                    if d:
+                        sec.children = build_efi_modules_tree( _uefi, fwtype, d, len(d), 0, polarity )
+                    if sec.children:
+                        break
+
+            elif sec.Type == EFI_SECTION_FIRMWARE_VOLUME_IMAGE:
+                children = build_efi_file_tree( _uefi, sec.Image[sec.HeaderSize:], fwtype )
+                if not children is None:
+                    sec.children = children
+
+            elif sec.Type == EFI_SECTION_RAW:
+                sec.children = build_efi_model( _uefi, sec.Image[sec.HeaderSize:], fwtype)
+
+            elif sec.Type not in SECTION_NAMES.keys():
                 sec.children = build_efi_model( _uefi, sec.Image[sec.HeaderSize:], fwtype)
+                if not sec.children:
+                    sec.children = build_efi_model( _uefi, data, fwtype)
 
             sections.append(sec)
         _off, next_offset, _name, _type, _img, _hdrsz = NextFwFileSection( data, Size, next_offset, polarity )
         secn += 1
     return sections
 
 # build_efi_file_tree - extract EFI FV file from EFI image and build an object tree
```

### Comparing `chipsec-1.4.4/chipsec/hal/spi_jedec_ids.py` & `chipsec-1.5.1/chipsec/hal/spi_jedec_ids.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/hal/cpuid.py` & `chipsec-1.5.1/chipsec/hal/cpuid.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2015, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -15,34 +15,21 @@
 #along with this program; if not, write to the Free Software
 #Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
 #Contact information:
 #chipsec@intel.com
 #
 
-
-
-# -------------------------------------------------------------------------------
-#
-# CHIPSEC: Platform Hardware Security Assessment Framework
-# (c) 2010-2018 Intel Corporation
-#
-# -------------------------------------------------------------------------------
-
 """
 CPUID information
 
 usage:
     >>> cpuid(0)
 """
 
-import struct
-import sys
-import os.path
-
 from chipsec.hal import hal_base
 from chipsec.logger import logger
 
 class CpuIDRuntimeError (RuntimeError):
     pass
 
 class CpuID(hal_base.HALBase):
```

### Comparing `chipsec-1.4.4/chipsec/hal/uefi_platform.py` & `chipsec-1.5.1/chipsec/hal/uefi_platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -15,34 +15,28 @@
 #along with this program; if not, write to the Free Software
 #Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
 #Contact information:
 #chipsec@intel.com
 #
 
-
-
-# -------------------------------------------------------------------------------
-#
-# CHIPSEC: Platform Hardware Security Assessment Framework
-# (c) 2010-2019 Intel Corporation
-#
-# -------------------------------------------------------------------------------
-
 """
 Platform specific UEFI functionality (parsing platform specific EFI NVRAM, capsules, etc.)
 """
 
 import struct
-import string
 from collections import namedtuple
 from uuid import UUID
 
 from chipsec import defines
-from chipsec.hal.uefi_common import *
+from chipsec.hal.uefi_common import bit_set, NextFwFile, guid_size, guid_str, VARIABLE_SIGNATURE_VSS, NextFwVolume, S3BootScriptOpcode_MDE, op_io_pci_mem, S3BootScriptOpcode_EdkCompat
+from chipsec.hal.uefi_common import op_stall, op_dispatch, op_terminate, op_mem_poll, op_unknown, get_3b_size, get_nvar_name, op_smbus_execute, script_width_formats
+from chipsec.hal.uefi_common import S3BOOTSCRIPT_ENTRY, MAX_S3_BOOTSCRIPT_ENTRY_LENGTH, VARIABLE_STORE_FV_GUID, IS_VARIABLE_ATTRIBUTE, VARIABLE_DATA
+from chipsec.hal.uefi_common import EFI_FVB2_ERASE_POLARITY, EFI_FV_FILETYPE_RAW, EFI_VARIABLE_BOOTSERVICE_ACCESS, EFI_VARIABLE_NON_VOLATILE, EFI_VARIABLE_RUNTIME_ACCESS
+from chipsec.hal.uefi_common import EFI_VARIABLE_HARDWARE_ERROR_RECORD, EFI_VARIABLE_AUTHENTICATED_WRITE_ACCESS, EFI_VARIABLE_TIME_BASED_AUTHENTICATED_WRITE_ACCESS
 
 #################################################################################################
 # Dell PFS support,
 # relied heavily on uefi-firmware-parser (https://github.com/theopolis/uefi-firmware-parser)
 #################################################################################################
 
 PFS_SEC_HDR = "<16sIIIIIIIIII16s"
@@ -61,16 +55,16 @@
         if (self.valid):
             self.body = data[PFS_SEC_HDR_SIZE+data_offset:PFS_SEC_HDR_SIZE+sec_size]
             self.tail = data[PFS_SEC_HDR_SIZE+sec_size+size1+size2+size3:]
 
     def parse(self):
         return self.body
 
-PFS_HDR_SIG = "PFS.HDR."
-PFS_FTR_SIG = "PFS.FTR."
+PFS_HDR_SIG = b"PFS.HDR."
+PFS_FTR_SIG = b"PFS.FTR."
 PFS_HDR_STRUC = "<8sII"
 PFS_HDR_STRUC_SIZE = struct.calcsize(PFS_HDR_STRUC)
 PFS_FTR_STRUC = "<II8s"
 PFS_FTR_STRUC_SIZE = struct.calcsize(PFS_FTR_STRUC)
 
 class PfsFile:
 
@@ -98,15 +92,15 @@
             sec_data = pfs_sec.parse()
             if sec_data[:len(PFS_HDR_SIG)] == PFS_HDR_SIG:
                 sec_data = PfsFile(sec_data, True).parse()
             if sec_data is not None:
                 pfs_sec_data.append(sec_data)
             pfs_sec = PfsFileSection(pfs_sec.tail)
         if self.concat:
-            return ''.join(pfs_sec_data)
+            return b''.join(pfs_sec_data)
         else:
             return pfs_sec_data
 
 def ParsePFS(data):
     pfs_file = PfsFile(data, True)
     if not pfs_file.valid:
         return None
@@ -535,30 +529,14 @@
 Reserved  : 0x%04X
 Reserved1 : 0x%08X
 """ % ( UUID(bytes_le=self.Signature), self.Size, self.Format, self.State, self.Reserved, self.Reserved1 )
 
 VARIABLE_STORE_SIGNATURE_VSS2 = UUID('DDCF3617-3275-4164-98B6-FE85707FFE7D').bytes_le
 VARIABLE_STORE_SIGNATURE_VSS2_AUTH = UUID('AAF32C78-947B-439A-A180-2E144EC37792').bytes_le
 
-VARIABLE_STORE_HEADER_FMT_VSS2 = '=16sIBBHI'
-class VARIABLE_STORE_HEADER_VSS2( namedtuple('VARIABLE_STORE_HEADER_VSS2', 'Signature Size Format State Reserved Reserved1') ):
-    __slots__ = ()
-    def __str__(self):
-        return """
-EFI Variable Store
------------------------------
-Signature : %s
-Size      : 0x%08X bytes
-Format    : 0x%02X
-State     : 0x%02X
-Reserved  : 0x%04X
-Reserved1 : 0x%08X
-""" % ( UUID(bytes_le=self.Signature), self.Size, self.Format, self.State, self.Reserved, self.Reserved1 )
-
-
 HDR_FMT_VSS                   = '<HBBIII4s2s2s8s'
 #HDR_SIZE_VSS                  = struct.calcsize( HDR_FMT_VSS )
 #NAME_OFFSET_IN_VAR_VSS        = HDR_SIZE_VSS
 class EFI_HDR_VSS( namedtuple('EFI_HDR_VSS', 'StartId State Reserved Attributes NameSize DataSize guid0 guid1 guid2 guid3') ):
     __slots__ = ()
     def __str__(self):
         return """
@@ -641,15 +619,15 @@
     return _getNVstore_VSS(nvram_buf, FWType.EFI_FW_TYPE_VSS_AUTH)
 
 def getNVstore_VSS2( nvram_buf ):
     return _getNVstore_VSS(nvram_buf, FWType.EFI_FW_TYPE_VSS2)
 
 def getNVstore_VSS2_AUTH( nvram_buf ):
     return _getNVstore_VSS(nvram_buf, FWType.EFI_FW_TYPE_VSS2_AUTH)
-    
+
 def getNVstore_VSS_APPLE( nvram_buf):
     return _getNVstore_VSS(nvram_buf, FWType.EFI_FW_TYPE_VSS_APPLE)
 
 VSS_TYPES = (FWType.EFI_FW_TYPE_VSS, FWType.EFI_FW_TYPE_VSS_AUTH, FWType.EFI_FW_TYPE_VSS2, FWType.EFI_FW_TYPE_VSS2_AUTH, FWType.EFI_FW_TYPE_VSS_APPLE)
 MAX_VSS_VAR_ALIGNMENT = 8
 
 def isCorrectVSStype(nvram_buf, vss_type):
@@ -743,18 +721,17 @@
             data_size = efi_var_hdr.DataSize
             efi_var_name = "<not defined>"
 
             end_var_offset = start + hdr_size + name_size + data_size
             efi_var_buf  = nvram_buf[ start : end_var_offset ]
 
             name_offset = hdr_size
-            #if not IS_VARIABLE_ATTRIBUTE( efi_var_hdr.Attributes, EFI_VARIABLE_HARDWARE_ERROR_RECORD ):
-            #efi_var_name = "".join( efi_var_buf[ NAME_OFFSET_IN_VAR_VSS : NAME_OFFSET_IN_VAR_VSS + name_size ] )
             Name = efi_var_buf[ name_offset : name_offset + name_size ]
-            efi_var_name = Name.decode("utf-16-le").split('\x00')[0]
+            if Name:
+                efi_var_name = Name.decode("utf-16-le").split('\x00')[0]
 
             efi_var_data = efi_var_buf[ name_offset + name_size : name_offset + name_size + data_size ]
             guid = guid_str(efi_var_hdr.guid0, efi_var_hdr.guid1, efi_var_hdr.guid2, efi_var_hdr.guid3)
             if efi_var_name not in variables.keys():
                 variables[efi_var_name] = []
             #                                off,   buf,         hdr,         data,         guid, attrs
             variables[efi_var_name].append( (start, efi_var_buf, efi_var_hdr, efi_var_data, guid, efi_var_hdr.Attributes) )
```

### Comparing `chipsec-1.4.4/chipsec/hal/__init__.py` & `chipsec-1.5.1/chipsec/hal/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/hal/smbios.py` & `chipsec-1.5.1/chipsec/hal/smbios.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2019, Intel Corporation
+#Copyright (c) 2019-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -15,18 +15,17 @@
 #along with this program; if not, write to the Free Software
 #Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
 #Contact information:
 #chipsec@intel.com
 #
 import struct
-import uuid
 from collections import namedtuple
 
-from chipsec.defines import BOUNDARY_1MB, BOUNDARY_4GB, bytestostring
+from chipsec.defines import BOUNDARY_1MB, bytestostring
 from chipsec.hal import hal_base, uefi
 from chipsec.logger import logger
 
 SCAN_LOW_LIMIT = 0xF0000
 SCAN_SIZE = 0x10000
 
 SMBIOS_2_x_SIG = b"_SM_"
@@ -109,47 +108,85 @@
 
 
 SMBIOS_BIOS_INFO_ENTRY_ID = 0
 SMBIOS_BIOS_INFO_2_0_ENTRY_FMT = '=BBHBBHBBQ'
 SMBIOS_BIOS_INFO_2_0_ENTRY_SIZE = struct.calcsize(SMBIOS_BIOS_INFO_2_0_ENTRY_FMT)
 SMBIOS_BIOS_INFO_2_0_FORMAT_STRING = """
 SMBIOS BIOS Information:
-  Type                      : 0x{:02X} ({:d})
-  Length                    : 0x{:02X}
-  Handle                    : 0x{:04X}
-  Vendor                    : {:s}
-  BIOS Version              : {:s}
-  BIOS Starting Segment     : 0x{:04X}
-  BIOS Release Date         : {:s}
-  BIOS ROM Size             : 0x{:02X}
-  BIOS Characteristics      : 0x{:016X}
+  Type                      : 0x{0:02X} ({0:d})
+  Length                    : 0x{1:02X}
+  Handle                    : 0x{2:04X}
+  Vendor                    : {3:s}
+  BIOS Version              : {4:s}
+  BIOS Starting Segment     : 0x{5:04X}
+  BIOS Release Date         : {6:s}
+  BIOS ROM Size             : 0x{7:02X}
+  BIOS Characteristics      : 0x{8:016X}
 """
 SMBIOS_BIOS_INFO_2_0_FORMAT_STRING_FAILED = """
 SMBIOS BIOS Information structure decode failed
 """
-class SMBIOS_BIOS_INFO_2_0(namedtuple('SMBIOS_BIOS_ENTRY_2_0', 'type length handle vendor_str version_str segment release_str \
-    rom_sz bios_char strings')):
+class SMBIOS_BIOS_INFO_2_0(namedtuple('SMBIOS_BIOS_INFO_2_0_ENTRY', 'type length handle vendor_str version_str segment \
+    release_str rom_sz bios_char strings')):
     __slots__ = ()
     def __str__(self):
         str_count = len(self.strings)
         ven_str = ''
         ver_str = ''
         rel_str = ''
         if self.vendor_str != 0 and self.vendor_str <= str_count:
             ven_str = self.strings[self.vendor_str - 1]
         if self.version_str != 0 and self.version_str <= str_count:
             ver_str = self.strings[self.version_str - 1]
         if self.release_str != 0 and self.release_str <= str_count:
             rel_str = self.strings[self.release_str - 1]
-        return SMBIOS_BIOS_INFO_2_0_FORMAT_STRING.format(self.type, self.type, self.length, self.handle, ven_str, \
+        return SMBIOS_BIOS_INFO_2_0_FORMAT_STRING.format(self.type, self.length, self.handle, ven_str, \
             ver_str, self.segment, rel_str, self.rom_sz, self.bios_char)
 
 
+SMBIOS_SYSTEM_INFO_ENTRY_ID = 1
+SMBIOS_SYSTEM_INFO_2_0_ENTRY_FMT = '=BBHBBBB'
+SMBIOS_SYSTEM_INFO_2_0_ENTRY_SIZE = struct.calcsize(SMBIOS_SYSTEM_INFO_2_0_ENTRY_FMT)
+SMBIOS_SYSTEM_INFO_2_0_FORMAT_STRING = """
+SMBIOS System Information:
+  Type                      : 0x{0:02X} ({0:d})
+  Length                    : 0x{1:02X}
+  Handle                    : 0x{2:04X}
+  Manufacturer              : {3:s}
+  Product Name              : {4:s}
+  Version                   : {5:s}
+  Serial Number             : {6:s}
+"""
+SMBIOS_SYSTEM_INFO_2_0_FORMAT_STRING_FAILED = """
+SMBIOS System Information structure decode failed
+"""
+class SMBIOS_SYSTEM_INFO_2_0(namedtuple('SMBIOS_SYSTEM_INFO_2_0_ENTRY', 'type length handle manufacturer_str product_str \
+    version_str serial_str strings')):
+    __slots__ = ()
+    def __str__(self):
+        str_count = len(self.strings)
+        man_str = ''
+        pro_str = ''
+        ver_str = ''
+        ser_str = ''
+        if self.manufacturer_str != 0 and self.manufacturer_str <= str_count:
+            man_str = self.strings[self.manufacturer_str - 1]
+        if self.product_str != 0 and self.product_str <= str_count:
+            pro_str = self.strings[self.product_str - 1]
+        if self.version_str != 0 and self.version_str <= str_count:
+            ver_str = self.strings[self.version_str - 1]
+        if self.serial_str != 0 and self.serial_str <= str_count:
+            ser_str = self.strings[self.serial_str - 1]
+        return SMBIOS_SYSTEM_INFO_2_0_FORMAT_STRING.format(self.type, self.length, self.handle, man_str, \
+            pro_str, ver_str, ser_str)
+
+
 struct_decode_tree = {
-    SMBIOS_BIOS_INFO_ENTRY_ID: {'class':SMBIOS_BIOS_INFO_2_0, 'format':SMBIOS_BIOS_INFO_2_0_ENTRY_FMT}
+    SMBIOS_BIOS_INFO_ENTRY_ID: {'class': SMBIOS_BIOS_INFO_2_0, 'format': SMBIOS_BIOS_INFO_2_0_ENTRY_FMT},
+    SMBIOS_SYSTEM_INFO_ENTRY_ID: {'class': SMBIOS_SYSTEM_INFO_2_0, 'format': SMBIOS_SYSTEM_INFO_2_0_ENTRY_FMT}
 }
 
 class SMBIOS(hal_base.HALBase):
     def __init__(self, cs):
         super(SMBIOS, self).__init__(cs)
         self.uefi = uefi.UEFI(cs)
         self.smbios_2_guid_found = False
@@ -344,15 +381,15 @@
         None
         """
         ret_val = []
 
         if self.smbios_3_data is not None and not force_32bit:
             if logger().HAL: logger().log('Using 64bit SMBIOS table')
             table = self.smbios_3_data
-        elif self.smbios_3_data is not None:
+        elif self.smbios_2_data is not None:
             if logger().HAL: logger().log('Using 32bit SMBIOS table')
             table = self.smbios_2_data
         else:
             if logger().HAL: logger().log('- No SMBIOS data available')
             return None
 
         if logger().HAL: logger().log('Getting SMBIOS structures...')
```

### Comparing `chipsec-1.4.4/chipsec/hal/spi.py` & `chipsec-1.5.1/chipsec/hal/spi.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -15,23 +15,14 @@
 #along with this program; if not, write to the Free Software
 #Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
 #Contact information:
 #chipsec@intel.com
 #
 
-
-
-# -------------------------------------------------------------------------------
-#
-# CHIPSEC: Platform Hardware Security Assessment Framework
-# (c) 2010-2019 Intel Corporation
-#
-# -------------------------------------------------------------------------------
-
 """
 Access to SPI Flash parts
 
 usage:
     >>> read_spi( spi_fla, length )
     >>> write_spi( spi_fla, buf )
     >>> erase_spi_block( spi_fla )
@@ -49,44 +40,74 @@
     @TBD: SPI write cycles operate on 4 byte chunks (not optimized yet)
 
     Approximate performance (on 2-core SMT Intel Core i5-4300U (Haswell) CPU 1.9GHz):
     SPI read: ~7 sec per 1MB (with DBC=64)
 """
 
 import struct
-import sys
 import time
 
-import chipsec.defines
-from chipsec.file import *
-from chipsec.cfg.common import *
+from chipsec.defines import ALIGNED_4KB, BIT0, BIT1, BIT2, BIT5
+from chipsec.file import write_file, read_file
+from chipsec.logger import print_buffer
 from chipsec.hal import hal_base, mmio
 from chipsec.helper import oshelper
-from chipsec.hal.spi_jedec_ids import *
+from chipsec.hal.spi_jedec_ids import JEDEC_ID
 
 SPI_READ_WRITE_MAX_DBC = 64
 SPI_READ_WRITE_DEF_DBC = 4
+SFDP_HEADER = 0x50444653
 
 SPI_MAX_PR_COUNT  = 5
 SPI_FLA_SHIFT     = 12
-SPI_FLA_PAGE_MASK = chipsec.defines.ALIGNED_4KB
+SPI_FLA_PAGE_MASK = ALIGNED_4KB
+
+SPI_MMIO_BASE_LENGTH  = 0x200
+PCH_RCBA_SPI_HSFSTS_SCIP           = BIT5                          # SPI cycle in progress
+PCH_RCBA_SPI_HSFSTS_AEL            = BIT2                          # Access Error Log
+PCH_RCBA_SPI_HSFSTS_FCERR          = BIT1                          # Flash Cycle Error
+PCH_RCBA_SPI_HSFSTS_FDONE          = BIT0                          # Flash Cycle Done
+
+PCH_RCBA_SPI_HSFCTL_FCYCLE_READ    = 0                             # Flash Cycle Read
+PCH_RCBA_SPI_HSFCTL_FCYCLE_WRITE   = 2                             # Flash Cycle Write
+PCH_RCBA_SPI_HSFCTL_FCYCLE_ERASE   = 3                             # Flash Cycle Block Erase
+PCH_RCBA_SPI_HSFCTL_FCYCLE_SFDP    = 5
+PCH_RCBA_SPI_HSFCTL_FCYCLE_JEDEC   = 6                             # Flash Cycle Read JEDEC ID
+PCH_RCBA_SPI_HSFCTL_FCYCLE_FGO     = BIT0                          # Flash Cycle GO
+
+PCH_RCBA_SPI_FADDR_MASK          = 0x07FFFFFF                      # SPI Flash Address Mask [0:26]
+
+PCH_RCBA_SPI_FREGx_LIMIT_MASK    = 0x7FFF0000                    # Size
+PCH_RCBA_SPI_FREGx_BASE_MASK     = 0x00007FFF                    # Base
+
+PCH_RCBA_SPI_OPTYPE_RDNOADDR     = 0x00
+PCH_RCBA_SPI_OPTYPE_WRNOADDR     = 0x01
+PCH_RCBA_SPI_OPTYPE_RDADDR       = 0x02
+PCH_RCBA_SPI_OPTYPE_WRADDR       = 0x03
+
+PCH_RCBA_SPI_FDOC_FDSS_FSDM      = 0x0000                        # Flash Signature and Descriptor Map
+PCH_RCBA_SPI_FDOC_FDSS_COMP      = 0x1000                        # Component
+PCH_RCBA_SPI_FDOC_FDSS_REGN      = 0x2000                        # Region
+PCH_RCBA_SPI_FDOC_FDSS_MSTR      = 0x3000                        # Master
+PCH_RCBA_SPI_FDOC_FDSI_MASK      = 0x0FFC                        # Flash Descriptor Section Index
 
 # agregated SPI Flash commands
-HSFCTL_READ_CYCLE  = ( (Cfg.PCH_RCBA_SPI_HSFCTL_FCYCLE_READ<<1) | Cfg.PCH_RCBA_SPI_HSFCTL_FCYCLE_FGO)
-HSFCTL_WRITE_CYCLE = ( (Cfg.PCH_RCBA_SPI_HSFCTL_FCYCLE_WRITE<<1) | Cfg.PCH_RCBA_SPI_HSFCTL_FCYCLE_FGO)
-HSFCTL_ERASE_CYCLE = ( (Cfg.PCH_RCBA_SPI_HSFCTL_FCYCLE_ERASE<<1) | Cfg.PCH_RCBA_SPI_HSFCTL_FCYCLE_FGO)
-HSFCTL_JEDEC_CYCLE = ( (Cfg.PCH_RCBA_SPI_HSFCTL_FCYCLE_JEDEC<<1) | Cfg.PCH_RCBA_SPI_HSFCTL_FCYCLE_FGO)
+HSFCTL_READ_CYCLE  = ( (PCH_RCBA_SPI_HSFCTL_FCYCLE_READ<<1) | PCH_RCBA_SPI_HSFCTL_FCYCLE_FGO)
+HSFCTL_WRITE_CYCLE = ( (PCH_RCBA_SPI_HSFCTL_FCYCLE_WRITE<<1) | PCH_RCBA_SPI_HSFCTL_FCYCLE_FGO)
+HSFCTL_ERASE_CYCLE = ( (PCH_RCBA_SPI_HSFCTL_FCYCLE_ERASE<<1) | PCH_RCBA_SPI_HSFCTL_FCYCLE_FGO)
+HSFCTL_JEDEC_CYCLE = ( (PCH_RCBA_SPI_HSFCTL_FCYCLE_JEDEC<<1) | PCH_RCBA_SPI_HSFCTL_FCYCLE_FGO)
+HSFCTL_SFDP_CYCLE = ( (PCH_RCBA_SPI_HSFCTL_FCYCLE_SFDP<<1) | PCH_RCBA_SPI_HSFCTL_FCYCLE_FGO)
 
 # !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 # FGO bit cleared (for safety ;)
 # !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-#HSFCTL_WRITE_CYCLE = ( (Cfg.PCH_RCBA_SPI_HSFCTL_FCYCLE_WRITE<<1) )
-#HSFCTL_ERASE_CYCLE = ( (Cfg.PCH_RCBA_SPI_HSFCTL_FCYCLE_ERASE<<1) )
+#HSFCTL_WRITE_CYCLE = ( (PCH_RCBA_SPI_HSFCTL_FCYCLE_WRITE<<1) )
+#HSFCTL_ERASE_CYCLE = ( (PCH_RCBA_SPI_HSFCTL_FCYCLE_ERASE<<1) )
 
-HSFSTS_CLEAR = (Cfg.PCH_RCBA_SPI_HSFSTS_AEL | Cfg.PCH_RCBA_SPI_HSFSTS_FCERR | Cfg.PCH_RCBA_SPI_HSFSTS_FDONE)
+HSFSTS_CLEAR = (PCH_RCBA_SPI_HSFSTS_AEL | PCH_RCBA_SPI_HSFSTS_FCERR | PCH_RCBA_SPI_HSFSTS_FDONE)
 
 #
 # Hardware Sequencing Flash Status (HSFSTS)
 #
 SPI_HSFSTS_OFFSET = 0x04
 # HSFSTS bit masks
 SPI_HSFSTS_FLOCKDN_MASK = (1 << 15)
@@ -153,19 +174,18 @@
 SPI_MASTER_NAMES = {
  MASTER_HOST_CPU_BIOS : 'CPU',
  MASTER_ME            : 'ME',
  MASTER_GBE           : 'GBe',
  MASTER_EC            : 'EC'
 }
 
-
 # @TODO: DEPRECATED
 def get_SPI_region(flreg):
-    range_base  = (flreg & Cfg.PCH_RCBA_SPI_FREGx_BASE_MASK) << SPI_FLA_SHIFT
-    range_limit = ((flreg & Cfg.PCH_RCBA_SPI_FREGx_LIMIT_MASK) >> 4)
+    range_base  = (flreg & PCH_RCBA_SPI_FREGx_BASE_MASK) << SPI_FLA_SHIFT
+    range_limit = ((flreg & PCH_RCBA_SPI_FREGx_LIMIT_MASK) >> 4)
     range_limit |= SPI_FLA_PAGE_MASK
     return (range_base, range_limit)
 
 class SpiRuntimeError (RuntimeError):
     pass
 
 class SpiAccessError (RuntimeError):
@@ -177,44 +197,53 @@
     def __init__(self, cs):
         super(SPI, self).__init__(cs)
         self.mmio = mmio.MMIO(cs)
         self.rcba_spi_base = self.get_SPI_MMIO_base()
         # We try to map SPIBAR in the process memory, this will increase the
         # speed of MMIO access later on.
         try:
-            self.cs.helper.map_io_space(self.rcba_spi_base, Cfg.SPI_MMIO_BASE_LENGTH, 0)
+            self.cs.helper.map_io_space(self.rcba_spi_base, SPI_MMIO_BASE_LENGTH, 0)
         except oshelper.UnimplementedAPIError:
             pass
 
         # Reading definitions of SPI flash controller registers
         # which are required to send SPI cycles once for performance reasons
         self.hsfs_off   = int(self.cs.get_register_def("HSFS")['offset'],16)
         self.hsfc_off   = int(self.cs.get_register_def("HSFC")['offset'],16)
         self.faddr_off  = int(self.cs.get_register_def("FADDR")['offset'],16)
         self.fdata0_off = int(self.cs.get_register_def("FDATA0")['offset'],16)
-        if logger().HAL:
-            logger().log( "[spi] Reading SPI flash controller registers definitions:" )
-            logger().log( "      HSFC   offset = 0x{:04X}".format(self.hsfc_off) )
-            logger().log( "      HSFS   offset = 0x{:04X}".format(self.hsfs_off) )
-            logger().log( "      FADDR  offset = 0x{:04X}".format(self.faddr_off) )
-            logger().log( "      FDATA0 offset = 0x{:04X}".format(self.fdata0_off) )
-
-    # Fallback option when XML config is not available: using hardcoded config
-    def get_SPI_MMIO_base_fallback(self):
-        reg_value = self.cs.pci.read_dword( Cfg.SPI_MMIO_BUS, Cfg.SPI_MMIO_DEV, Cfg.SPI_MMIO_FUN, Cfg.SPI_MMIO_REG_OFFSET )
-        spi_base = ((reg_value >> Cfg.SPI_BASE_ADDR_SHIFT) << Cfg.SPI_BASE_ADDR_SHIFT) + Cfg.SPI_MMIO_BASE_OFFSET
-        if logger().HAL: logger().log( "[spi] SPI MMIO base: 0x{:016X} (assuming below 4GB)".format(spi_base) )
-        return spi_base
+        self.fdata1_off = int(self.cs.get_register_def("FDATA1")['offset'],16)
+        self.fdata2_off = int(self.cs.get_register_def("FDATA2")['offset'],16)
+        self.fdata3_off = int(self.cs.get_register_def("FDATA3")['offset'],16)
+        self.fdata4_off = int(self.cs.get_register_def("FDATA4")['offset'],16)
+        self.fdata5_off = int(self.cs.get_register_def("FDATA5")['offset'],16)
+        self.fdata6_off = int(self.cs.get_register_def("FDATA6")['offset'],16)
+        self.fdata7_off = int(self.cs.get_register_def("FDATA7")['offset'],16)
+        self.fdata8_off = int(self.cs.get_register_def("FDATA8")['offset'],16)
+        self.fdata9_off = int(self.cs.get_register_def("FDATA9")['offset'],16)
+        self.fdata10_off = int(self.cs.get_register_def("FDATA10")['offset'],16)
+        self.fdata11_off = int(self.cs.get_register_def("FDATA11")['offset'],16)
+        self.fdata12_off = int(self.cs.get_register_def("FDATA12")['offset'],16)
+        self.fdata13_off = int(self.cs.get_register_def("FDATA13")['offset'],16)
+        self.fdata14_off = int(self.cs.get_register_def("FDATA14")['offset'],16)
+        self.fdata15_off = int(self.cs.get_register_def("FDATA15")['offset'],16)
+        self.bios_ptinx  = int(self.cs.get_register_def("BIOS_PTINX")['offset'],16)
+        self.bios_ptdata  = int(self.cs.get_register_def("BIOS_PTDATA")['offset'],16)
+
+        if self.logger.HAL:
+            self.logger.log( "[spi] Reading SPI flash controller registers definitions:" )
+            self.logger.log( "      HSFC   offset = 0x{:04X}".format(self.hsfc_off) )
+            self.logger.log( "      HSFS   offset = 0x{:04X}".format(self.hsfs_off) )
+            self.logger.log( "      FADDR  offset = 0x{:04X}".format(self.faddr_off) )
+            self.logger.log( "      FDATA0 offset = 0x{:04X}".format(self.fdata0_off) )
 
     def get_SPI_MMIO_base(self):
         if self.mmio.is_MMIO_BAR_defined('SPIBAR'):
             (spi_base,spi_size) = self.mmio.get_MMIO_BAR_base_address('SPIBAR')
-        else:
-            spi_base = self.get_SPI_MMIO_base_fallback()
-        if logger().HAL: logger().log( "[spi] SPI MMIO base: 0x{:016X} (assuming below 4GB)".format(spi_base) )
+        if self.logger.HAL: self.logger.log( "[spi] SPI MMIO base: 0x{:016X} (assuming below 4GB)".format(spi_base) )
         return spi_base
 
     def spi_reg_read( self, reg, size=4 ):
         return self.mmio.read_MMIO_reg(self.rcba_spi_base, reg, size)
 
     def spi_reg_write( self, reg, value, size=4 ):
         return self.mmio.write_MMIO_reg(self.rcba_spi_base, reg, value, size)
@@ -270,289 +299,292 @@
         return (base,limit,wpe,rpe,pr_j_reg,pr_j)
 
     ##############################################################################################################
     # SPI configuration
     ##############################################################################################################
 
     def display_SPI_Flash_Descriptor( self ):
-        logger().log( "============================================================" )
-        logger().log( "SPI Flash Descriptor" )
-        logger().log( "------------------------------------------------------------" )
-        logger().log( "\nFlash Signature and Descriptor Map:" )
+        self.logger.log( "============================================================" )
+        self.logger.log( "SPI Flash Descriptor" )
+        self.logger.log( "------------------------------------------------------------" )
+        self.logger.log( "\nFlash Signature and Descriptor Map:" )
         for j in range(5):
-            self.cs.write_register('FDOC', (Cfg.PCH_RCBA_SPI_FDOC_FDSS_FSDM|(j<<2)))
+            self.cs.write_register('FDOC', (PCH_RCBA_SPI_FDOC_FDSS_FSDM|(j<<2)))
             fdod = self.cs.read_register('FDOD')
-            logger().log( "{:08X}".format(fdod) )
+            self.logger.log( "{:08X}".format(fdod) )
 
-        logger().log( "\nComponents:" )
+        self.logger.log( "\nComponents:" )
         for j in range(3):
-            self.cs.write_register('FDOC', (Cfg.PCH_RCBA_SPI_FDOC_FDSS_COMP|(j<<2)))
+            self.cs.write_register('FDOC', (PCH_RCBA_SPI_FDOC_FDSS_COMP|(j<<2)))
             fdod = self.cs.read_register('FDOD')
-            logger().log( "{:08X}".format(fdod) )
+            self.logger.log( "{:08X}".format(fdod) )
 
-        logger().log( "\nRegions:" )
+        self.logger.log( "\nRegions:" )
         for j in range(5):
-            self.cs.write_register('FDOC', (Cfg.PCH_RCBA_SPI_FDOC_FDSS_REGN|(j<<2)))
+            self.cs.write_register('FDOC', (PCH_RCBA_SPI_FDOC_FDSS_REGN|(j<<2)))
             fdod = self.cs.read_register('FDOD')
-            logger().log( "{:08X}".format(fdod) )
+            self.logger.log( "{:08X}".format(fdod) )
 
-        logger().log( "\nMasters:" )
+        self.logger.log( "\nMasters:" )
         for j in range(3):
-            self.cs.write_register('FDOC', (Cfg.PCH_RCBA_SPI_FDOC_FDSS_MSTR|(j<<2)))
+            self.cs.write_register('FDOC', (PCH_RCBA_SPI_FDOC_FDSS_MSTR|(j<<2)))
             fdod = self.cs.read_register('FDOD')
-            logger().log( "{:08X}".format(fdod) )
+            self.logger.log( "{:08X}".format(fdod) )
 
 
     def display_SPI_opcode_info( self ):
-        logger().log( "============================================================" )
-        logger().log( "SPI Opcode Info" )
-        logger().log( "------------------------------------------------------------" )
+        self.logger.log( "============================================================" )
+        self.logger.log( "SPI Opcode Info" )
+        self.logger.log( "------------------------------------------------------------" )
         preop = self.cs.read_register( 'PREOP' )
-        logger().log( "PREOP : 0x{:04X}".format(preop) )
+        self.logger.log( "PREOP : 0x{:04X}".format(preop) )
         optype = self.cs.read_register('OPTYPE' )
-        logger().log( "OPTYPE: 0x{:04X}".format(optype) )
+        self.logger.log( "OPTYPE: 0x{:04X}".format(optype) )
         opmenu_lo = self.cs.read_register('OPMENU_LO' )
         opmenu_hi = self.cs.read_register('OPMENU_HI' )
         opmenu = ((opmenu_hi << 32)|opmenu_lo)
-        logger().log( "OPMENU: 0x{:016X}".format(opmenu) )
-        logger().log('')
+        self.logger.log( "OPMENU: 0x{:016X}".format(opmenu) )
+        self.logger.log('')
         preop0 = preop&0xFF
         preop1 = (preop>>8)&0xFF
-        logger().log( "Prefix Opcode 0 = 0x{:02X}".format(preop0) )
-        logger().log( "Prefix Opcode 1 = 0x{:02X}".format(preop1) )
+        self.logger.log( "Prefix Opcode 0 = 0x{:02X}".format(preop0) )
+        self.logger.log( "Prefix Opcode 1 = 0x{:02X}".format(preop1) )
 
-        logger().log( "------------------------------------------------------------" )
-        logger().log( "Opcode # | Opcode | Optype | Description" )
-        logger().log( "------------------------------------------------------------" )
+        self.logger.log( "------------------------------------------------------------" )
+        self.logger.log( "Opcode # | Opcode | Optype | Description" )
+        self.logger.log( "------------------------------------------------------------" )
         for j in range(8):
             optype_j = ((optype >> j*2) & 0x3)
-            if (Cfg.PCH_RCBA_SPI_OPTYPE_RDNOADDR == optype_j):
+            if (PCH_RCBA_SPI_OPTYPE_RDNOADDR == optype_j):
                 desc = 'SPI read cycle without address'
-            elif (Cfg.PCH_RCBA_SPI_OPTYPE_WRNOADDR == optype_j):
+            elif (PCH_RCBA_SPI_OPTYPE_WRNOADDR == optype_j):
                 desc = 'SPI write cycle without address'
-            elif (Cfg.PCH_RCBA_SPI_OPTYPE_RDADDR == optype_j):
+            elif (PCH_RCBA_SPI_OPTYPE_RDADDR == optype_j):
                 desc = 'SPI read cycle with address'
-            elif (Cfg.PCH_RCBA_SPI_OPTYPE_WRADDR == optype_j):
+            elif (PCH_RCBA_SPI_OPTYPE_WRADDR == optype_j):
                 desc = 'SPI write cycle with address'
-            logger().log( "Opcode{:d}  | 0x{:02X}   | {:x}      | {} ".format(j,((opmenu >> j*8) & 0xFF),optype_j,desc) )
+            self.logger.log( "Opcode{:d}  | 0x{:02X}   | {:x}      | {} ".format(j,((opmenu >> j*8) & 0xFF),optype_j,desc) )
 
     def display_SPI_Flash_Regions( self ):
-        logger().log( "------------------------------------------------------------" )
-        logger().log( "Flash Region             | FREGx Reg | Base     | Limit     " )
-        logger().log( "------------------------------------------------------------" )
+        self.logger.log( "------------------------------------------------------------" )
+        self.logger.log( "Flash Region             | FREGx Reg | Base     | Limit     " )
+        self.logger.log( "------------------------------------------------------------" )
         regions = self.get_SPI_regions()
         for (region_id, region) in regions.items():
             base, limit, size, name, freg = region
-            logger().log( '{:d} {:22} | {:08X}  | {:08X} | {:08X} '.format(region_id, name, freg, base, limit) )
+            self.logger.log( '{:d} {:22} | {:08X}  | {:08X} | {:08X} '.format(region_id, name, freg, base, limit) )
 
     def display_BIOS_region( self ):
         bfpreg = self.cs.read_register('BFPR' )
         base  = self.cs.get_register_field('BFPR', bfpreg, 'PRB' ) << SPI_FLA_SHIFT
         limit = self.cs.get_register_field('BFPR', bfpreg, 'PRL' ) << SPI_FLA_SHIFT
         limit |= SPI_FLA_PAGE_MASK
-        logger().log( "BIOS Flash Primary Region" )
-        logger().log( "------------------------------------------------------------" )
-        logger().log( "BFPREG = {:08X}:".format(bfpreg) )
-        logger().log( "  Base  : {:08X}".format(base) )
-        logger().log( "  Limit : {:08X}".format(limit) )
+        self.logger.log( "BIOS Flash Primary Region" )
+        self.logger.log( "------------------------------------------------------------" )
+        self.logger.log( "BFPREG = {:08X}:".format(bfpreg) )
+        self.logger.log( "  Base  : {:08X}".format(base) )
+        self.logger.log( "  Limit : {:08X}".format(limit) )
 
     def display_SPI_Ranges_Access_Permissions( self ):
-        logger().log( "SPI Flash Region Access Permissions" )
-        logger().log( "------------------------------------------------------------" )
+        self.logger.log( "SPI Flash Region Access Permissions" )
+        self.logger.log( "------------------------------------------------------------" )
         fracc = self.cs.read_register('FRAP')
-        self.cs.print_register('FRAP', fracc)
+        if self.logger.HAL:
+            self.cs.print_register('FRAP', fracc)
         brra  = self.cs.get_register_field('FRAP', fracc, 'BRRA' )
         brwa  = self.cs.get_register_field('FRAP', fracc, 'BRWA' )
         bmrag = self.cs.get_register_field('FRAP', fracc, 'BMRAG' )
         bmwag = self.cs.get_register_field('FRAP', fracc, 'BMWAG' )
         if self.cs.is_register_defined('FDOC') and self.cs.is_register_defined('FDOD'):
+            if self.logger.HAL:
+                self.logger.log("Reading Observability Contol and Data register (may update braa and brwa)")
             self.cs.write_register('FDOC', 0x3000)
             tmp_reg = self.cs.read_register('FDOD')
             brra |= ((tmp_reg >> 8) & 0xFFF)
             brwa |= ((tmp_reg >> 20) & 0xFFF)
-        logger().log( '' )
-        logger().log( "BIOS Region Write Access Grant ({:02X}):".format(bmwag) )
+        self.logger.log( '' )
+        self.logger.log( "BIOS Region Write Access Grant ({:02X}):".format(bmwag) )
         regions = self.get_SPI_regions()
         for region_id in regions:
-            logger().log( "  {:12}: {:1d}".format(SPI_REGION[region_id], (0 != bmwag&(1<<region_id))) )
-        logger().log( "BIOS Region Read Access Grant ({:02X}):".format(bmrag) )
+            self.logger.log( "  {:12}: {:1d}".format(SPI_REGION[region_id], (0 != bmwag&(1<<region_id))) )
+        self.logger.log( "BIOS Region Read Access Grant ({:02X}):".format(bmrag) )
         for region_id in regions:
-            logger().log( "  {:12}: {:1d}".format(SPI_REGION[region_id ], (0 != bmrag&(1<<region_id))) )
-        logger().log( "BIOS Region Write Access ({:02X}):".format(brwa) )
+            self.logger.log( "  {:12}: {:1d}".format(SPI_REGION[region_id ], (0 != bmrag&(1<<region_id))) )
+        self.logger.log( "BIOS Region Write Access ({:02X}):".format(brwa) )
         for region_id in regions:
-            logger().log( "  {:12}: {:1d}".format(SPI_REGION[ region_id ], (0 != brwa&(1<<region_id))) )
-        logger().log( "BIOS Region Read Access ({:02X}):".format(brra) )
+            self.logger.log( "  {:12}: {:1d}".format(SPI_REGION[ region_id ], (0 != brwa&(1<<region_id))) )
+        self.logger.log( "BIOS Region Read Access ({:02X}):".format(brra) )
         for region_id in regions:
-            logger().log( "  {:12}: {:1d}".format(SPI_REGION[ region_id ], (0 != brra&(1<<region_id))) )
+            self.logger.log( "  {:12}: {:1d}".format(SPI_REGION[ region_id ], (0 != brra&(1<<region_id))) )
 
     def display_SPI_Protected_Ranges( self ):
-        logger().log( "SPI Protected Ranges" )
-        logger().log( "------------------------------------------------------------" )
-        logger().log( "PRx (offset) | Value    | Base     | Limit    | WP? | RP?" )
-        logger().log( "------------------------------------------------------------" )
+        self.logger.log( "SPI Protected Ranges" )
+        self.logger.log( "------------------------------------------------------------" )
+        self.logger.log( "PRx (offset) | Value    | Base     | Limit    | WP? | RP?" )
+        self.logger.log( "------------------------------------------------------------" )
         for j in range(5):
             (base,limit,wpe,rpe,pr_reg_off,pr_reg_value) = self.get_SPI_Protected_Range( j )
-            logger().log( "PR{:d} ({:02X})     | {:08X} | {:08X} | {:08X} | {:d}   | {:d} ".format(j,pr_reg_off,pr_reg_value,base,limit,wpe,rpe) )
+            self.logger.log( "PR{:d} ({:02X})     | {:08X} | {:08X} | {:08X} | {:d}   | {:d} ".format(j,pr_reg_off,pr_reg_value,base,limit,wpe,rpe) )
 
     def display_SPI_map( self ):
-        logger().log( "============================================================" )
-        logger().log( "SPI Flash Map" )
-        logger().log( "------------------------------------------------------------" )
-        logger().log('')
+        self.logger.log( "============================================================" )
+        self.logger.log( "SPI Flash Map" )
+        self.logger.log( "------------------------------------------------------------" )
+        self.logger.log('')
         self.display_BIOS_region()
-        logger().log('')
+        self.logger.log('')
         self.display_SPI_Flash_Regions()
-        logger().log('')
+        self.logger.log('')
         self.display_SPI_Flash_Descriptor()
-        logger().log('')
+        self.logger.log('')
         self.display_SPI_opcode_info()
-        logger().log('')
-        logger().log( "============================================================" )
-        logger().log( "SPI Flash Protection" )
-        logger().log( "------------------------------------------------------------" )
-        logger().log('')
+        self.logger.log('')
+        self.logger.log( "============================================================" )
+        self.logger.log( "SPI Flash Protection" )
+        self.logger.log( "------------------------------------------------------------" )
+        self.logger.log('')
         self.display_SPI_Ranges_Access_Permissions()
-        logger().log('')
-        logger().log( "BIOS Region Write Protection" )
-        logger().log( "------------------------------------------------------------" )
+        self.logger.log('')
+        self.logger.log( "BIOS Region Write Protection" )
+        self.logger.log( "------------------------------------------------------------" )
         self.display_BIOS_write_protection()
-        logger().log('')
+        self.logger.log('')
         self.display_SPI_Protected_Ranges()
-        logger().log('')
+        self.logger.log('')
 
 
     ##############################################################################################################
     # BIOS Write Protection
     ##############################################################################################################
 
     def display_BIOS_write_protection( self ):
         if self.cs.is_register_defined('BC'):
              reg_value = self.cs.read_register('BC')
              self.cs.print_register('BC', reg_value )
         else:
-            if logger().HAL: logger().error( "Could not locate the definition of 'BIOS Control' register.." )
+            if self.logger.HAL: self.logger.error( "Could not locate the definition of 'BIOS Control' register.." )
 
 
     def disable_BIOS_write_protection( self ):
-        if logger().HAL: self.display_BIOS_write_protection()
+        if self.logger.HAL: self.display_BIOS_write_protection()
         ble    = self.cs.get_control('BiosLockEnable' )
         bioswe = self.cs.get_control('BiosWriteEnable' )
         smmbwp = self.cs.get_control('SmmBiosWriteProtection' )
 
         if smmbwp == 1:
-            if logger().HAL: logger().log( "[spi] SMM BIOS write protection (SmmBiosWriteProtection) is enabled" )
+            if self.logger.HAL: self.logger.log( "[spi] SMM BIOS write protection (SmmBiosWriteProtection) is enabled" )
 
         if bioswe == 1:
-            if logger().HAL: logger().log( "[spi] BIOS write protection (BiosWriteEnable) is not enabled" )
+            if self.logger.HAL: self.logger.log( "[spi] BIOS write protection (BiosWriteEnable) is not enabled" )
             return True
         elif ble == 0:
-            if logger().HAL: logger().log( "[spi] BIOS write protection is enabled but not locked. Disabling.." )
+            if self.logger.HAL: self.logger.log( "[spi] BIOS write protection is enabled but not locked. Disabling.." )
         else: # bioswe == 0 and ble == 1
-            if logger().HAL: logger().log( "[spi] BIOS write protection is enabled. Attempting to disable.." )
+            if self.logger.HAL: self.logger.log( "[spi] BIOS write protection is enabled. Attempting to disable.." )
 
         # Set BiosWriteEnable control bit
         self.cs.set_control('BiosWriteEnable', 1 )
 
         # read BiosWriteEnable back to check if BIOS writes are enabled
         bioswe = self.cs.get_control('BiosWriteEnable' )
 
-        if logger().HAL: self.display_BIOS_write_protection()
-        if logger().HAL: logger().log_important( "BIOS write protection is {} (BiosWriteEnable = {:d})".format('disabled' if bioswe else 'still enabled', bioswe) )
+        if self.logger.HAL: self.display_BIOS_write_protection()
+        if self.logger.HAL: self.logger.log_important( "BIOS write protection is {} (BiosWriteEnable = {:d})".format('disabled' if bioswe else 'still enabled', bioswe) )
 
         return (bioswe==1)
 
 
     ##############################################################################################################
     # SPI Controller access functions
     ##############################################################################################################
 
     def _wait_SPI_flash_cycle_done(self):
-        if logger().HAL: logger().log( "[spi] wait for SPI cycle ready/done.." )
+        if self.logger.HAL: self.logger.log( "[spi] wait for SPI cycle ready/done.." )
 
         for i in range(1000):
             #time.sleep(0.001)
             hsfsts = self.spi_reg_read( self.hsfs_off, 1 )
 
             #cycle_done = (hsfsts & Cfg.Cfg.PCH_RCBA_SPI_HSFSTS_FDONE) and (0 == (hsfsts & Cfg.PCH_RCBA_SPI_HSFSTS_SCIP))
-            cycle_done = not (hsfsts & Cfg.PCH_RCBA_SPI_HSFSTS_SCIP)
+            cycle_done = not (hsfsts & PCH_RCBA_SPI_HSFSTS_SCIP)
             if cycle_done:
                 break
 
         if not cycle_done:
-            if logger().HAL: logger().log( "[spi] SPI cycle still in progress. Waiting 0.1 sec.." )
+            if self.logger.HAL: self.logger.log( "[spi] SPI cycle still in progress. Waiting 0.1 sec.." )
             time.sleep(0.1)
             hsfsts = self.spi_reg_read( self.hsfs_off, 1 )
-            cycle_done = not (hsfsts & Cfg.PCH_RCBA_SPI_HSFSTS_SCIP)
+            cycle_done = not (hsfsts & PCH_RCBA_SPI_HSFSTS_SCIP)
 
         if cycle_done:
-            if logger().HAL: logger().log( "[spi] clear FDONE/FCERR/AEL bits.." )
+            if self.logger.HAL: self.logger.log( "[spi] clear FDONE/FCERR/AEL bits.." )
             self.spi_reg_write( self.hsfs_off, HSFSTS_CLEAR, 1 )
             hsfsts = self.spi_reg_read( self.hsfs_off, 1 )
-            cycle_done = not ((hsfsts & Cfg.PCH_RCBA_SPI_HSFSTS_AEL) or (hsfsts & Cfg.PCH_RCBA_SPI_HSFSTS_FCERR))
+            cycle_done = not ((hsfsts & PCH_RCBA_SPI_HSFSTS_AEL) or (hsfsts & PCH_RCBA_SPI_HSFSTS_FCERR))
 
-        if logger().HAL: logger().log( "[spi] HSFS: 0x{:02X}".format(hsfsts) )
+        if self.logger.HAL: self.logger.log( "[spi] HSFS: 0x{:02X}".format(hsfsts) )
 
         return cycle_done
 
     def _send_spi_cycle(self, hsfctl_spi_cycle_cmd, dbc, spi_fla ):
-        if logger().HAL: logger().log( "[spi] > send SPI cycle 0x{:x} to address 0x{:08X}..".format(hsfctl_spi_cycle_cmd, spi_fla) )
+        if self.logger.HAL: self.logger.log( "[spi] > send SPI cycle 0x{:x} to address 0x{:08X}..".format(hsfctl_spi_cycle_cmd, spi_fla) )
 
         # No need to check for SPI cycle DONE status before each cycle
         # DONE status is checked once before entire SPI operation
 
-        self.spi_reg_write( self.faddr_off, (spi_fla & Cfg.PCH_RCBA_SPI_FADDR_MASK) )
+        self.spi_reg_write( self.faddr_off, (spi_fla & PCH_RCBA_SPI_FADDR_MASK) )
         # Other options ;)
         #chipsec.chipset.write_register( self.cs, "FADDR", (spi_fla & Cfg.PCH_RCBA_SPI_FADDR_MASK) )
         #write_MMIO_reg( self.cs, spi_base, self.faddr_off, (spi_fla & Cfg.PCH_RCBA_SPI_FADDR_MASK) )
         #self.cs.mem.write_physical_mem_dword( spi_base + self.faddr_off, (spi_fla & Cfg.PCH_RCBA_SPI_FADDR_MASK) )
 
-        if logger().HAL:
+        if self.logger.HAL:
             _faddr = self.spi_reg_read( self.faddr_off )
-            logger().log( "[spi] FADDR: 0x{:08X}".format(_faddr) )
+            self.logger.log( "[spi] FADDR: 0x{:08X}".format(_faddr) )
 
-        if logger().HAL: logger().log( "[spi] SPI cycle GO (DBC <- 0x{:02X}, HSFC <- 0x{:x})".format(dbc, hsfctl_spi_cycle_cmd) )
+        if self.logger.HAL: self.logger.log( "[spi] SPI cycle GO (DBC <- 0x{:02X}, HSFC <- 0x{:x})".format(dbc, hsfctl_spi_cycle_cmd) )
 
         if ( HSFCTL_ERASE_CYCLE != hsfctl_spi_cycle_cmd ):
             self.spi_reg_write( self.hsfc_off + 0x1, dbc, 1 )
 
         self.spi_reg_write( self.hsfc_off, hsfctl_spi_cycle_cmd, 1 )
         #self.spi_reg_write( self.hsfc_off, ((dbc<<8)|hsfctl_spi_cycle_cmd), 2 )
 
         # Read HSFC back (logging only)
-        if logger().HAL:
+        if self.logger.HAL:
             _hsfc = self.spi_reg_read( self.hsfc_off, 1 )
-            logger().log( "[spi] HSFC: 0x{:04X}".format(_hsfc) )
+            self.logger.log( "[spi] HSFC: 0x{:04X}".format(_hsfc) )
 
         cycle_done = self._wait_SPI_flash_cycle_done()
         if not cycle_done:
-            logger().warn( "SPI cycle not done" )
+            self.logger.warn( "SPI cycle not done" )
         else:
-            if logger().HAL: logger().log( "[spi] < SPI cycle done" )
+            if self.logger.HAL: self.logger.log( "[spi] < SPI cycle done" )
 
         return cycle_done
 
     def check_hardware_sequencing(self):
         # Test if the flash decriptor is valid (and hardware sequencing enabled)
         fdv = self.cs.read_register_field('HSFS', 'FDV')
         if fdv == 0:
-            logger().error("HSFS.FDV is 0, hardware sequencing is disabled")
+            self.logger.error("HSFS.FDV is 0, hardware sequencing is disabled")
             raise SpiRuntimeError("Chipset does not support hardware sequencing")
 
     #
     # SPI Flash operations
     #
 
     def read_spi_to_file(self, spi_fla, data_byte_count, filename ):
         buf = self.read_spi( spi_fla, data_byte_count )
         if buf is None:
             return None
         if filename is not None:
             write_file( filename, buf )
         else:
-            chipsec.logger.print_buffer( buf, 16 )
+            print_buffer( buf, 16 )
         return buf
 
     def write_spi_from_file(self, spi_fla, filename ):
         buf = read_file( filename )
         return self.write_spi( spi_fla, struct.unpack('c'*len(buf), buf) )
         #return self.write_spi( spi_fla, struct.unpack('B'*len(buf), buf) )
 
@@ -563,137 +595,213 @@
         buf = bytearray()
         dbc = SPI_READ_WRITE_DEF_DBC
         if (data_byte_count >= SPI_READ_WRITE_MAX_DBC):
             dbc = SPI_READ_WRITE_MAX_DBC
 
         n = data_byte_count // dbc
         r = data_byte_count % dbc
-        if logger().UTIL_TRACE or logger().HAL:
-            logger().log( "[spi] reading 0x{:x} bytes from SPI at FLA = 0x{:x} (in {:d} 0x{:x}-byte chunks + 0x{:x}-byte remainder)".format(data_byte_count, spi_fla, n, dbc, r) )
+        if self.logger.UTIL_TRACE or self.logger.HAL:
+            self.logger.log( "[spi] reading 0x{:x} bytes from SPI at FLA = 0x{:x} (in {:d} 0x{:x}-byte chunks + 0x{:x}-byte remainder)".format(data_byte_count, spi_fla, n, dbc, r) )
 
         cycle_done = self._wait_SPI_flash_cycle_done()
         if not cycle_done:
-            logger().error( "SPI cycle not ready" )
+            self.logger.error( "SPI cycle not ready" )
             return None
 
         for i in range(n):
-            if logger().HAL:
-                logger().log( "[spi] reading chunk {:d} of 0x{:x} bytes from 0x{:x}".format(i, dbc, spi_fla + i*dbc) )
+            if self.logger.HAL:
+                self.logger.log( "[spi] reading chunk {:d} of 0x{:x} bytes from 0x{:x}".format(i, dbc, spi_fla + i*dbc) )
             if not self._send_spi_cycle( HSFCTL_READ_CYCLE, dbc-1, spi_fla + i*dbc ):
-                logger().error( "SPI flash read failed" )
+                self.logger.error( "SPI flash read failed" )
             else:
                 for fdata_idx in range(0,dbc//4):
                     dword_value = self.spi_reg_read( self.fdata0_off + fdata_idx*4 )
-                    if logger().HAL:
-                        logger().log( "[spi] FDATA00 + 0x{:x}: 0x{:x}".format(fdata_idx*4, dword_value) )
+                    if self.logger.HAL:
+                        self.logger.log( "[spi] FDATA00 + 0x{:x}: 0x{:x}".format(fdata_idx*4, dword_value) )
                     buf += struct.pack("I",dword_value)
 
         if (0 != r):
-            if logger().HAL:
-                logger().log( "[spi] reading remaining 0x{:x} bytes from 0x{:x}".format(r, spi_fla + n*dbc) )
+            if self.logger.HAL:
+                self.logger.log( "[spi] reading remaining 0x{:x} bytes from 0x{:x}".format(r, spi_fla + n*dbc) )
             if not self._send_spi_cycle( HSFCTL_READ_CYCLE, r-1, spi_fla + n*dbc ):
-                logger().error( "SPI flash read failed" )
+                self.logger.error( "SPI flash read failed" )
             else:
                 t = 4
                 n_dwords = (r+3)//4
                 for fdata_idx in range(0, n_dwords):
                     dword_value = self.spi_reg_read( self.fdata0_off + fdata_idx*4 )
-                    if logger().HAL:
-                        logger().log( "[spi] FDATA00 + 0x{:x}: 0x{:08X}".format(fdata_idx*4, dword_value) )
+                    if self.logger.HAL:
+                        self.logger.log( "[spi] FDATA00 + 0x{:x}: 0x{:08X}".format(fdata_idx*4, dword_value) )
                     if (fdata_idx == (n_dwords-1)) and (0 != r%4):
                         t = r%4
                     for j in range(t):
                         buf += struct.pack('B',(dword_value >> (8*j)) & 0xff)
 
-        if logger().HAL:
-            logger().log( "[spi] buffer read from SPI:" )
-            chipsec.logger.print_buffer( "{}".format(buf) )
+        if self.logger.HAL:
+            self.logger.log( "[spi] buffer read from SPI:" )
+            print_buffer( "{}".format(buf) )
 
         return buf
 
     def write_spi(self, spi_fla, buf ):
 
         self.check_hardware_sequencing()
 
         write_ok = True
         data_byte_count = len(buf)
         dbc = 4
         n = data_byte_count // dbc
         r = data_byte_count % dbc
-        if logger().UTIL_TRACE or logger().HAL:
-            logger().log( "[spi] writing 0x{:x} bytes to SPI at FLA = 0x{:x} (in {:d} 0x{:x}-byte chunks + 0x{:x}-byte remainder)".format(data_byte_count, spi_fla, n, dbc, r) )
+        if self.logger.UTIL_TRACE or self.logger.HAL:
+            self.logger.log( "[spi] writing 0x{:x} bytes to SPI at FLA = 0x{:x} (in {:d} 0x{:x}-byte chunks + 0x{:x}-byte remainder)".format(data_byte_count, spi_fla, n, dbc, r) )
 
         cycle_done = self._wait_SPI_flash_cycle_done()
         if not cycle_done:
-            logger().error( "SPI cycle not ready" )
+            self.logger.error( "SPI cycle not ready" )
             return None
 
         for i in range(n):
-            if logger().UTIL_TRACE or logger().HAL:
-                logger().log( "[spi] writing chunk {:d} of 0x{:x} bytes to 0x{:x}".format(i, dbc, spi_fla + i*dbc) )
+            if self.logger.UTIL_TRACE or self.logger.HAL:
+                self.logger.log( "[spi] writing chunk {:d} of 0x{:x} bytes to 0x{:x}".format(i, dbc, spi_fla + i*dbc) )
             dword_value = (ord(buf[i*dbc + 3]) << 24) | (ord(buf[i*dbc + 2]) << 16) | (ord(buf[i*dbc + 1]) << 8) | ord(buf[i*dbc])
-            if logger().HAL:
-                logger().log( "[spi] in FDATA00 = 0x{:08X}".format(dword_value) )
+            if self.logger.HAL:
+                self.logger.log( "[spi] in FDATA00 = 0x{:08X}".format(dword_value) )
             self.spi_reg_write( self.fdata0_off, dword_value )
             if not self._send_spi_cycle( HSFCTL_WRITE_CYCLE, dbc-1, spi_fla + i*dbc ):
                 write_ok = False
-                logger().error( "SPI flash write cycle failed" )
+                self.logger.error( "SPI flash write cycle failed" )
 
         if (0 != r):
-            if logger().UTIL_TRACE or logger().HAL:
-                logger().log( "[spi] writing remaining 0x{:x} bytes to FLA = 0x{:x}".format(r, spi_fla + n*dbc) )
+            if self.logger.UTIL_TRACE or self.logger.HAL:
+                self.logger.log( "[spi] writing remaining 0x{:x} bytes to FLA = 0x{:x}".format(r, spi_fla + n*dbc) )
             dword_value = 0
             for j in range(r):
                 dword_value |= (ord(buf[n*dbc + j]) << 8*j)
-            if logger().HAL:
-                logger().log( "[spi] in FDATA00 = 0x{:08X}".format(dword_value) )
+            if self.logger.HAL:
+                self.logger.log( "[spi] in FDATA00 = 0x{:08X}".format(dword_value) )
             self.spi_reg_write( self.fdata0_off, dword_value )
             if not self._send_spi_cycle( HSFCTL_WRITE_CYCLE, r-1, spi_fla + n*dbc ):
                 write_ok = False
-                logger().error( "SPI flash write cycle failed" )
+                self.logger.error( "SPI flash write cycle failed" )
 
         return write_ok
 
     def erase_spi_block(self, spi_fla ):
 
         self.check_hardware_sequencing()
 
-        if logger().UTIL_TRACE or logger().HAL:
-            logger().log( "[spi] Erasing SPI Flash block @ 0x{:x}".format(spi_fla) )
+        if self.logger.UTIL_TRACE or self.logger.HAL:
+            self.logger.log( "[spi] Erasing SPI Flash block @ 0x{:x}".format(spi_fla) )
 
         cycle_done = self._wait_SPI_flash_cycle_done()
         if not cycle_done:
-            logger().error( "SPI cycle not ready" )
+            self.logger.error( "SPI cycle not ready" )
             return None
 
         erase_ok = self._send_spi_cycle( HSFCTL_ERASE_CYCLE, 0, spi_fla )
         if not erase_ok:
-            logger().error( "SPI Flash erase cycle failed" )
+            self.logger.error( "SPI Flash erase cycle failed" )
 
         return erase_ok
 
     #
+    # SPI SFDP operations
+    #
+    def ptmesg(self, offset):
+        self.spi_reg_write(self.bios_ptinx, offset)
+        self.spi_reg_read(self.bios_ptinx)
+        return self.spi_reg_read(self.bios_ptdata)
+
+    def get_SPI_SFDP(self):
+        ret = False
+        for component in range(0,2):
+            self.logger.log( "Scanning for Flash device {:d}".format(component+1))
+            offset = 0x0000 | (component << 14)
+            sfdp_signature = self.ptmesg(offset)
+            if sfdp_signature == SFDP_HEADER:
+                self.logger.log( "  * Found valid SFDP header for Flash device {:d}".format(component+1))
+                ret = True
+            else:
+                self.logger.log ( "  * Didn't find a valid SFDP header for Flash device {:d}".format(component+1))
+                continue
+            # Increment offset to read second dword of SFDP header structure
+            sfdp_data = self.ptmesg(offset+0x4)
+            sfdp_minor_version = sfdp_data & 0xFF
+            sfdp_major_version = ( sfdp_data  >> 8) & 0xFF
+            self.logger.log( "    SFDP version number: {}.{}".format(sfdp_major_version, sfdp_minor_version))
+            num_of_param_headers = ((sfdp_data >> 16) & 0xFF) +1
+            self.logger.log( "    Number of parameter headers: {:d}".format(num_of_param_headers))
+            # Set offset to read 1st Parameter Table in the SFDP header structure
+            offset = offset | 0x1000
+            parameter_1 = self.ptmesg(offset)
+            param1_minor_version = (parameter_1 >> 8) & 0xFF
+            param1_major_version = (parameter_1 >> 16) & 0xFF
+            param1_length = (parameter_1 >> 24) & 0xFF
+            self.logger.log( "  * Parameter Header 1 (JEDEC)" )
+            self.logger.log( "    ** Parameter version number: {}.{}".format(param1_major_version, param1_minor_version))
+            self.logger.log( "    ** Parameter length in double words: {}".format(hex(param1_length)))
+            if (num_of_param_headers > 1) and self.cs.register_has_field( 'HSFS', 'FCYCLE' ):
+                self.check_hardware_sequencing()
+                self.spi_reg_write( self.fdata12_off, 0x00000000 )
+                self.spi_reg_write( self.fdata13_off, 0x00000000 )
+                self.spi_reg_write( self.fdata14_off, 0x00000000 )
+                self.spi_reg_write( self.fdata15_off, 0x00000000 )
+                if not self._send_spi_cycle( HSFCTL_SFDP_CYCLE, 0x3F, 0 ):
+                    self.logger.error( 'SPI SFDP signature cycle failed' )
+                    continue
+                pTable_offset_list = []
+                pTable_length = []
+                # Calculate which fdata_offset registers to read, based on number of parameter headers present
+                for i in range(1,num_of_param_headers):
+                    self.logger.log( "  * Parameter Header:{:d}".format(i+1) )
+                    data_reg_1 = "self.fdata" + str(2+(2*i)) + "_off"
+                    data_reg_2 = "self.fdata" + str(2+(2*i)+1) + "_off"
+                    data_dword_1 = self.spi_reg_read( eval(data_reg_1))
+                    data_dword_2 = self.spi_reg_read( eval(data_reg_2))
+                    id_manuf = (data_dword_2 & 0xFF000000) >> 16 | (data_dword_1 & 0xFF)
+                    param_minor_version = (data_dword_1 >> 8) & 0xFF
+                    param_major_version = (data_dword_1 >> 16) & 0xFF
+                    param_length = (data_dword_1 >> 24) & 0xFF
+                    param_table_pointer = (data_dword_2 & 0x00FFFFFF)
+                    self.logger.log( "    ** Parameter version number:{}.{}".format(param_major_version, param_minor_version))
+                    self.logger.log( "    ** Pramaeter length in double words: {}".format(hex(param_length)))
+                    self.logger.log( "    ** Parameter ID: {}".format(hex(id_manuf)))
+                    self.logger.log( "    ** Parameter Table Pointer(byte address): {} ".format(hex(param_table_pointer)))
+                    pTable_offset_list.append(param_table_pointer)
+                    pTable_length.append(param_length)
+            offset = 0x0000 | (component << 14)
+            # Set offset to read 1st Parameter table ( JEDEC Basic Flash Parameter Table) content and Parse it
+            offset = offset | 0x2000
+            self.logger.log( "                                ")
+            self.logger.log( "  * 1'st Parameter Table Content ")
+            for count in range(1,param1_length+1):
+                sfdp_data = self.ptmesg(offset)
+                offset +=4
+                self.cs.print_register("DWORD{}".format(count), sfdp_data)
+        return ret
+
+    #
     # SPI JEDEC ID operations
     #
 
     def get_SPI_JEDEC_ID(self):
 
         if self.cs.register_has_field( 'HSFS', 'FCYCLE' ):
             self.check_hardware_sequencing()
 
             if not self._send_spi_cycle( HSFCTL_JEDEC_CYCLE, 4, 0 ):
-                logger().error( 'SPI JEDEC ID cycle failed' )
+                self.logger.error( 'SPI JEDEC ID cycle failed' )
             id = self.spi_reg_read( self.fdata0_off )
         else:
-            id = 0x000000
-            if logger().HAL:
-                logger().log( '[spi] get_SPI_JEDEC_ID() skipped' )
+            return False
 
         return ((id & 0xFF) << 16) | (id & 0xFF00) | ( (id >> 16) & 0xFF )
 
     def get_SPI_JEDEC_ID_decoded(self):
 
         jedec_id = self.get_SPI_JEDEC_ID()
+        if jedec_id is False:
+            return (False, 0 ,0)
         manu = JEDEC_ID.MANUFACTURER.get((jedec_id >> 16) & 0xff, 'Unknown')
         part = JEDEC_ID.DEVICE.get( jedec_id, 'Unknown')
 
         return (jedec_id, manu, part)
```

### Comparing `chipsec-1.4.4/chipsec/hal/cpu.py` & `chipsec-1.5.1/chipsec/hal/cpu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -16,32 +16,19 @@
 #Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
 #Contact information:
 #chipsec@intel.com
 #
 
 
-
-# -------------------------------------------------------------------------------
-#
-# CHIPSEC: Platform Hardware Security Assessment Framework
-# (c) 2010-2018 Intel Corporation
-#
-# -------------------------------------------------------------------------------
-
 """
 CPU related functionality
 
 """
 
-import struct
-import sys
-import os.path
-from collections import namedtuple
-
 from chipsec.hal import acpi, hal_base, paging
 from chipsec.logger import logger
 
 VMM_NONE    = 0
 VMM_XEN     = 0x1
 VMM_HYPER_V = 0x2
 VMM_VMWARE  = 0x3
```

### Comparing `chipsec-1.4.4/chipsec/hal/msr.py` & `chipsec-1.5.1/chipsec/hal/msr.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -31,50 +31,57 @@
     >>> dump_Descriptor_Table( 0, DESCRIPTOR_TABLE_CODE_IDTR )
     >>> IDT( 0 )
     >>> GDT( 0 )
     >>> IDT_all()
     >>> GDT_all()
 """
 
-import struct
-import sys
-import os
-
 from chipsec.logger import logger, print_buffer
-from chipsec.cfg.common import *
 
 
 DESCRIPTOR_TABLE_CODE_IDTR = 0
 DESCRIPTOR_TABLE_CODE_GDTR = 1
 DESCRIPTOR_TABLE_CODE_LDTR = 2
 
+MTRR_MEMTYPE_UC = 0x0
+MTRR_MEMTYPE_WC = 0x1
+MTRR_MEMTYPE_WT = 0x4
+MTRR_MEMTYPE_WP = 0x5
+MTRR_MEMTYPE_WB = 0x6
+MemType = {
+    MTRR_MEMTYPE_UC: 'Uncacheable (UC)',
+    MTRR_MEMTYPE_WB: 'Write Combining (WC)',
+    MTRR_MEMTYPE_WT: 'Write-through (WT)',
+    MTRR_MEMTYPE_WP: 'Write-protected (WP)',
+    MTRR_MEMTYPE_WB: 'Writeback (WB)'
+}
+
 class MsrRuntimeError (RuntimeError):
     pass
 
 class Msr:
 
     def __init__( self, cs ):
         self.helper = cs.helper
         self.cs = cs
 
     def get_cpu_thread_count( self ):
         thread_count = self.helper.get_threads_count()
         if thread_count is None or thread_count < 0:
             if logger().HAL: logger().log( "helper.get_threads_count didn't return anything. Reading MSR 0x35 to find out number of logical CPUs (use CPUID Leaf B instead?)" )
-            (core_thread_count, dummy) = self.helper.read_msr( 0, Cfg.IA32_MSR_CORE_THREAD_COUNT )
-            thread_count = (core_thread_count & Cfg.IA32_MSR_CORE_THREAD_COUNT_THREADCOUNT_MASK)
+            thread_count = self.cs.read_register_field("IA32_MSR_CORE_THREAD_COUNT","Thread_Count")
 
         if 0 == thread_count: thread_count = 1
         if logger().HAL: logger().log( "[cpu] # of logical CPUs: {:d}".format(thread_count) )
         return thread_count
 
     # @TODO: fix
     def get_cpu_core_count( self ):
-        (core_thread_count, dummy) = self.helper.read_msr( 0, Cfg.IA32_MSR_CORE_THREAD_COUNT )
-        return ((core_thread_count & Cfg.IA32_MSR_CORE_THREAD_COUNT_CORECOUNT_MASK) >> 16)
+        core_count = self.cs.read_register_field("IA32_MSR_CORE_THREAD_COUNT","Core_Count")
+        return core_count
 
 
 ##########################################################################################################
 #
 # Read/Write CPU MSRs
 #
 ##########################################################################################################
```

### Comparing `chipsec-1.4.4/chipsec/hal/paging.py` & `chipsec-1.5.1/chipsec/hal/paging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -19,17 +19,15 @@
 #chipsec@intel.com
 #
 
 # ====================
 # x64/IA-64 Paging functionality including x86 page tables, Extended Page Tables (EPT) and VT-d page tables
 # ====================
 
-import os
 import sys
-import time
 import struct
 
 import chipsec.defines
 from chipsec.logger import logger
 
 ADDR_MASK  = chipsec.defines.MASK_64b
 MAXPHYADDR = 0x000FFFFFFFFFF000
```

### Comparing `chipsec-1.4.4/chipsec/hal/hal_base.py` & `chipsec-1.5.1/chipsec/hal/hal_base.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/hal/acpi.py` & `chipsec-1.5.1/chipsec/hal/acpi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -15,38 +15,27 @@
 #along with this program; if not, write to the Free Software
 #Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
 #Contact information:
 #chipsec@intel.com
 #
 
-
-
-
-# -------------------------------------------------------------------------------
-#
-# CHIPSEC: Platform Hardware Security Assessment Framework
-# (c) 2010-2018 Intel Corporation
-#
-# -------------------------------------------------------------------------------
-
 """
 HAL component providing access to and decoding of ACPI tables
 """
 
 __version__ = '0.1'
 
 import struct
-import sys
 
 from collections import defaultdict
 from collections import namedtuple
 
-from chipsec.logger import *
-from chipsec.file import *
+from chipsec.logger import logger, print_buffer
+from chipsec.file import read_file
 from chipsec.defines import bytestostring
 
 from chipsec.hal import acpi_tables, hal_base, uefi
 from chipsec.helper import oshelper
 
 class AcpiRuntimeError (RuntimeError):
     pass
@@ -121,15 +110,14 @@
 ACPI_TABLE_SIG_EINJ = 'EINJ'
 ACPI_TABLE_SIG_TPM2 = 'TPM2'
 ACPI_TABLE_SIG_WSMT = 'WSMT'
 ACPI_TABLE_SIG_DBG2 = 'DBG2'
 ACPI_TABLE_SIG_NHLT = 'NHLT'
 ACPI_TABLE_SIG_MSCT = 'MSCT'
 ACPI_TABLE_SIG_RASF = 'RASF'
-ACPI_TABLE_SIG_SPMI = 'SPMI'
 ACPI_TABLE_SIG_OEM1 = 'OEM1'
 ACPI_TABLE_SIG_OEM2 = 'OEM2'
 ACPI_TABLE_SIG_OEM3 = 'OEM3'
 ACPI_TABLE_SIG_OEM4 = 'OEM4'
 ACPI_TABLE_SIG_NFIT = 'NFIT'
 
 ACPI_TABLES = {
```

### Comparing `chipsec-1.4.4/chipsec/hal/spi_descriptor.py` & `chipsec-1.5.1/chipsec/hal/spi_descriptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2015, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -15,40 +15,28 @@
 #along with this program; if not, write to the Free Software
 #Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
 #Contact information:
 #chipsec@intel.com
 #
 
-
-
-# -------------------------------------------------------------------------------
-#
-# CHIPSEC: Platform Hardware Security Assessment Framework
-# (c) 2010-2012 Intel Corporation
-#
-# -------------------------------------------------------------------------------
-
 """
 SPI Flash Descriptor binary parsing functionality
 
 
 usage:
     >>> fd = read_file( fd_file )
     >>> parse_spi_flash_descriptor( fd )
 """
 
 import struct
-import sys
 import time
 
-from chipsec.logger import *
-from chipsec.file import *
-
-from chipsec.cfg.common import *
+from chipsec.logger import logger, print_buffer
+from chipsec.defines import bytestostring
 from chipsec.hal import spi
 from binascii import hexlify
 
 SPI_FLASH_DESCRIPTOR_SIGNATURE = struct.pack('=I', 0x0FF0A55A )
 SPI_FLASH_DESCRIPTOR_SIZE      = 0x1000
 
 
@@ -110,18 +98,18 @@
     logger().log( '' )
     logger().log( '########################################################' )
     logger().log( '# SPI FLASH DESCRIPTOR' )
     logger().log( '########################################################' )
     logger().log( '' )
 
     fd     = rom[ fd_off : fd_off + SPI_FLASH_DESCRIPTOR_SIZE ]
-    fd_sig = struct.unpack_from( '=I', fd[0x10:0x14] )
+    fd_sig = struct.unpack_from( '=I', fd[0x10:0x14] )[0]
 
     logger().log( '+ 0x0000 Reserved : 0x{}'.format(hexlify(fd[0x0:0xF]).upper()) )
-    logger().log( '+ 0x0010 Signature: 0x{:8s}'.format(fd_sig) )
+    logger().log( '+ 0x0010 Signature: 0x{:08X}'.format(fd_sig) )
 
     #
     # Flash Descriptor Map Section
     #
     flmap0 = struct.unpack_from( '=I', fd[0x14:0x18] )[0]
     flmap1 = struct.unpack_from( '=I', fd[0x18:0x1C] )[0]
     flmap2 = struct.unpack_from( '=I', fd[0x1C:0x20] )[0]
```

### Comparing `chipsec-1.4.4/chipsec/modules/debugenabled.py` & `chipsec-1.5.1/chipsec/modules/debugenabled.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/bdw/__init__.py` & `chipsec-1.5.1/chipsec/modules/bdw/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/memconfig.py` & `chipsec-1.5.1/chipsec/modules/common/smm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2018, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -15,85 +15,63 @@
 #Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 #
 #Contact information:
 #chipsec@intel.com
 #
 
 
-"""
-This module verifies memory map secure configuration,
-i.e. that memory map registers are correctly configured and locked down.
-"""
-
-from chipsec.module_common import *
-
-_MODULE_NAME = 'memconfig'
 
-TAGS = [MTAG_HWCONFIG]
+"""
+In 2006, `Security Issues Related to Pentium System Management Mode <http://www.ssi.gouv.fr/archive/fr/sciences/fichiers/lti/cansecwest2006-duflot.pdf>`_ outlined a configuration issue where compatibility SMRAM was not locked on some platforms. This means that ring 0 software was able to modify System Management Mode (SMM) code and data that should have been protected.
 
+In Compatability SMRAM (CSEG), access to memory is defined by the SMRAMC register. When SMRAMC[D_LCK] is not set by the BIOS, SMRAM can be accessed even when the CPU is not in SMM. Such attacks were also described in `Using CPU SMM to Circumvent OS Security Functions <http://fawlty.cs.usfca.edu/~cruse/cs630f06/duflot.pdf>`_ and `Using SMM for Other Purposes <http://phrack.org/issues/65/7.html>`_.
 
-memmap_registers = {
-  "PCI0.0.0_GGC"        : 'GGCLOCK',
-  "PCI0.0.0_PAVPC"      : 'PAVPLCK',
-  "PCI0.0.0_DPR"        : 'LOCK',
-  "PCI0.0.0_MESEG_MASK" : 'MELCK',
-  "PCI0.0.0_REMAPBASE"  : 'LOCK',
-  "PCI0.0.0_REMAPLIMIT" : 'LOCK',
-  "PCI0.0.0_TOM"        : 'LOCK',
-  "PCI0.0.0_TOUUD"      : 'LOCK',
-  "PCI0.0.0_BDSM"       : 'LOCK',
-  "PCI0.0.0_BGSM"       : 'LOCK',
-  "PCI0.0.0_TSEGMB"     : 'LOCK',
-  "PCI0.0.0_TOLUD"      : 'LOCK'
-}
-
-memmap_registers_dev0bars = [
-  "PCI0.0.0_PXPEPBAR",
-  "PCI0.0.0_MCHBAR",
-  "PCI0.0.0_PCIEXBAR",
-  "PCI0.0.0_DMIBAR",
-]
+This CHIPSEC module simply reads SMRAMC and checks that D_LCK is set.
+"""
+from collections import namedtuple
+from chipsec.module_common import BaseModule, ModuleResult, MTAG_BIOS, MTAG_SMM
 
+TAGS = [MTAG_BIOS,MTAG_SMM]
 
-class memconfig(BaseModule):
+class smm(BaseModule):
 
     def __init__(self):
         BaseModule.__init__(self)
 
     def is_supported(self):
-        return self.cs.is_core()
-
-    def check_memmap_locks(self):
-        self.logger.start_test( "Host Bridge Memory Map Locks" )
-
-        regs = list(memmap_registers.keys())
-        regs.sort()
-        all_locked = True
-
-        for r in regs:
-            if not self.cs.is_register_defined(r) or not self.cs.register_has_field(r, memmap_registers[r]):
-                self.logger.log_unknown('Skipping Validation: Register {} or field {} was not defined for this platform.'.format(r, memmap_registers[r]))
-                continue
-            d = self.cs.get_register_def( r )
-            v = self.cs.read_register( r )
-            locked = self.cs.get_register_field( r, v, memmap_registers[r] )
-            if locked == 1:
-                self.logger.log_good( "{:20} = 0x{:016X} - LOCKED   - {}".format(r, v, d['desc']) )
+        if self.cs.is_core() and self.cs.is_register_defined('PCI0.0.0_SMRAMC'):
+            return True
+        self.res = ModuleResult.NOTAPPLICABLE
+        return False
+
+    def check_SMRAMC(self):
+        self.logger.start_test( "Compatible SMM memory (SMRAM) Protection" )
+
+        regval = self.cs.read_register( 'PCI0.0.0_SMRAMC' )
+        g_smrame = self.cs.get_register_field( 'PCI0.0.0_SMRAMC', regval, 'G_SMRAME' )
+        d_open   = self.cs.get_register_field( 'PCI0.0.0_SMRAMC', regval, 'D_OPEN' )
+        d_lock   = self.cs.get_register_field( 'PCI0.0.0_SMRAMC', regval, 'D_LCK' )
+
+        self.cs.print_register( 'PCI0.0.0_SMRAMC', regval )
+
+        if 1 == g_smrame:
+            self.logger.log( "[*] Compatible SMRAM is enabled" )
+            # When D_LCK is set HW clears D_OPEN so generally no need to check for D_OPEN but doesn't hurt double checking
+            if 1 == d_lock and 0 == d_open:
+                res = ModuleResult.PASSED
+                self.logger.log_passed_check( "Compatible SMRAM is locked down" )
             else:
-                all_locked = False
-                self.logger.log_bad(  "{:20} = 0x{:016X} - UNLOCKED - {}".format(r, v, d['desc']) )
-
-        if all_locked:
-            res = ModuleResult.PASSED
-            self.logger.log_passed_check( "All memory map registers seem to be locked down" )
+                res = ModuleResult.FAILED
+                self.logger.log_failed_check( "Compatible SMRAM is not properly locked. Expected ( D_LCK = 1, D_OPEN = 0 )" )
         else:
-            res = ModuleResult.FAILED
-            self.logger.log_failed_check( "Not all memory map registers are locked down" )
+            res = ModuleResult.SKIPPED
+            self.logger.log( "[*] Compatible SMRAM is not enabled. Skipping.." )
 
         return res
 
+
     # --------------------------------------------------------------------------
     # run( module_argv )
     # Required function: run here all tests from this module
     # --------------------------------------------------------------------------
     def run( self, module_argv ):
-        return self.check_memmap_locks()
+        return self.check_SMRAMC()
```

### Comparing `chipsec-1.4.4/chipsec/modules/remap.py` & `chipsec-1.5.1/chipsec/modules/remap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -22,15 +22,16 @@
 
 """
 `Preventing & Detecting Xen Hypervisor Subversions <http://www.invisiblethingslab.com/resources/bh08/part2-full.pdf>`_ by Joanna Rutkowska & Rafal Wojtczuk
 
 Check Memory Remapping Configuration
 """
 
-from chipsec.module_common import *
+from chipsec.module_common import BaseModule, ModuleResult, MTAG_HWCONFIG, MTAG_SMM
+from chipsec.defines import BIT32, ALIGNED_1MB
 
 _MODULE_NAME = 'remap'
 
 TAGS = [MTAG_SMM,MTAG_HWCONFIG]
 
 
 _REMAP_ADDR_MASK = 0x7FFFF00000
@@ -38,18 +39,18 @@
 
 class remap(BaseModule):
 
     def __init__(self):
         BaseModule.__init__(self)
 
     def is_supported(self):
-        if self.cs.is_atom():
-            self.res = ModuleResult.NOTAPPLICABLE
-            return False
-        return self.cs.is_core()
+        if self.cs.is_core():
+            return True
+        self.res = ModuleResult.NOTAPPLICABLE
+        return False
 
     def check_remap_config(self):
         self.logger.start_test( "Memory Remapping Configuration" )
 
         if not self.cs.is_register_defined( 'PCI0.0.0_REMAPBASE'  ) or \
            not self.cs.is_register_defined( 'PCI0.0.0_REMAPLIMIT' ) or \
            not self.cs.is_register_defined( 'PCI0.0.0_TOUUD'      ) or \
@@ -66,14 +67,17 @@
         self.logger.log( "[*] Registers:" )
         self.logger.log( "[*]   TOUUD     : 0x{:016X}".format(touud) )
         self.logger.log( "[*]   REMAPLIMIT: 0x{:016X}".format(remaplimit) )
         self.logger.log( "[*]   REMAPBASE : 0x{:016X}".format(remapbase) )
         self.logger.log( "[*]   TOLUD     : 0x{:08X}".format(tolud) )
         self.logger.log( "[*]   TSEGMB    : 0x{:08X}\n".format(tsegmb) )
 
+        ia_untrusted = 0
+        if self.cs.is_register_defined('MSR_BIOS_DONE') and self.cs.register_has_field('MSR_BIOS_DONE', 'IA_UNTRUSTED'):
+            ia_untrusted = self.cs.read_register_field('MSR_BIOS_DONE', 'IA_UNTRUSTED')
         remapbase_lock  = remapbase & 0x1
         remaplimit_lock = remaplimit & 0x1
         touud_lock      = touud & 0x1
         tolud_lock      = tolud & 0x1
         tsegmb_lock     = tsegmb & 0x1
         remapbase  &= _REMAP_ADDR_MASK
         remaplimit &= _REMAP_ADDR_MASK
@@ -81,15 +85,15 @@
         touud      &= _REMAP_ADDR_MASK
         tolud      &= _TOLUD_MASK
         tsegmb     &= _TOLUD_MASK
         self.logger.log( "[*] Memory Map:" )
         self.logger.log( "[*]   Top Of Upper Memory: 0x{:016X}".format(touud) )
         self.logger.log( "[*]   Remap Limit Address: 0x{:016X}".format(remaplimit|0xFFFFF) )
         self.logger.log( "[*]   Remap Base Address : 0x{:016X}".format(remapbase) )
-        self.logger.log( "[*]   4GB                : 0x{:016X}".format(chipsec.defines.BIT32) )
+        self.logger.log( "[*]   4GB                : 0x{:016X}".format(BIT32) )
         self.logger.log( "[*]   Top Of Low Memory  : 0x{:016X}".format(tolud) )
         self.logger.log( "[*]   TSEG (SMRAM) Base  : 0x{:016X}\n".format(tsegmb) )
 
         remap_ok = True
 
         self.logger.log( "[*] checking memory remap configuration.." )
         if remapbase > remaplimit:
@@ -98,46 +102,47 @@
             self.logger.log( "[*]   Memory Remap is enabled" )
             remaplimit_addr = (remaplimit|0xFFFFF)
             ok = ((remaplimit_addr + 1) == touud)
             remap_ok = remap_ok and ok
             if ok: self.logger.log_good( "  Remap window configuration is correct: REMAPBASE <= REMAPLIMIT < TOUUD" )
             else:  self.logger.log_bad( "  Remap window configuration is not correct" )
 
-        ok = (0 == tolud & chipsec.defines.ALIGNED_1MB)     and \
-             (0 == touud & chipsec.defines.ALIGNED_1MB)     and \
-             (0 == remapbase & chipsec.defines.ALIGNED_1MB) and \
-             (0 == remaplimit & chipsec.defines.ALIGNED_1MB)
+        ok = (0 == tolud & ALIGNED_1MB)     and \
+             (0 == touud & ALIGNED_1MB)     and \
+             (0 == remapbase & ALIGNED_1MB) and \
+             (0 == remaplimit & ALIGNED_1MB)
         remap_ok = remap_ok and ok
         if ok: self.logger.log_good( "  All addresses are 1MB aligned" )
         else:  self.logger.log_bad( "  Not all addresses are 1MB aligned" )
 
         self.logger.log( "[*] checking if memory remap configuration is locked.." )
-        ok = (0 != touud_lock)
+        ok = (0 != touud_lock) or (0 != ia_untrusted)
         remap_ok = remap_ok and ok
         if ok: self.logger.log_good( "  TOUUD is locked" )
         else:  self.logger.log_bad( "  TOUUD is not locked" )
 
-        ok = (0 != tolud_lock)
+        ok = (0 != tolud_lock) or (0 != ia_untrusted)
         remap_ok = remap_ok and ok
         if ok: self.logger.log_good( "  TOLUD is locked" )
         else:  self.logger.log_bad( "  TOLUD is not locked" )
 
-        ok = (0 != remapbase_lock) and (0 != remaplimit_lock)
+        ok = ((0 != remapbase_lock) and (0 != remaplimit_lock)) or (0 != ia_untrusted)
         remap_ok = remap_ok and ok
         if ok: self.logger.log_good( "  REMAPBASE and REMAPLIMIT are locked" )
         else:  self.logger.log_bad( "  REMAPBASE and REMAPLIMIT are not locked" )
 
         if remap_ok:
-            self.res = ModuleResult.PASSED
+            res = ModuleResult.PASSED
             self.logger.log_passed_check( "Memory Remap is configured correctly and locked" )
         else:
-            self.res = ModuleResult.FAILED
+            res = ModuleResult.FAILED
             self.logger.log_failed_check( "Memory Remap is not properly configured/locked. Remaping attack may be possible" )
 
-        return self.res
+        return res
 
     # --------------------------------------------------------------------------
     # run( module_argv )
     # Required function: run here all tests from this module
     # --------------------------------------------------------------------------
     def run( self, module_argv ):
-        return self.check_remap_config()
+        self.res = self.check_remap_config()
+        return self.res
```

### Comparing `chipsec-1.4.4/chipsec/modules/snb/__init__.py` & `chipsec-1.5.1/chipsec/modules/byt/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/smm_dma.py` & `chipsec-1.5.1/chipsec/modules/smm_dma.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2015, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -24,48 +24,52 @@
 Just like SMRAM needs to be protected from software executing on the CPU, it also needs to be protected from devices that have direct access to DRAM (DMA). Protection from DMA is configured through proper programming of SMRAM memory range. If BIOS does not correctly configure and lock the configuration, then malware could reprogram configuration and open SMRAM area to DMA access, allowing manipulation of memory that should have been protected.
 
 DMA attacks were discussed in `Programmed I/O accesses: a threat to Virtual Machine Monitors? <http://www.ssi.gouv.fr/archive/fr/sciences/fichiers/lti/pacsec2007-duflot-papier.pdf>`_ and `System Management Mode Design and Security Issues <http://www.ssi.gouv.fr/uploads/IMG/pdf/IT_Defense_2010_final.pdf>`_. This is also discussed in `Summary of Attack against BIOS and Secure Boot` https://www.defcon.org/images/defcon-22/dc-22-presentations/Bulygin-Bazhaniul-Furtak-Loucaides/DEFCON-22-Bulygin-Bazhaniul-Furtak-Loucaides-Summary-of-attacks-against-BIOS-UPDATED.pdf
 
 This module examines the configuration and locking of SMRAM range configuration protecting from DMA attacks. If it fails, then DMA protection may not be securely configured to protect SMRAM.
 """
 
-from chipsec.module_common import *
+from chipsec.module_common import BaseModule, ModuleResult, MTAG_SMM, MTAG_HWCONFIG
 
 _MODULE_NAME = 'smm_dma'
 
 TAGS = [MTAG_SMM,MTAG_HWCONFIG]
 
 
 _TSEG_MASK  = 0xFFF00000
 
 class smm_dma(BaseModule):
 
     def __init__(self):
         BaseModule.__init__(self)
 
     def is_supported(self):
+        self.res = ModuleResult.NOTAPPLICABLE
         if self.cs.is_atom(): return False
         if self.cs.is_server(): return False
         else: return True
 
     def check_tseg_locks(self):
         tseg_base_lock = self.cs.get_control('TSEGBaseLock')
         tseg_limit_lock = self.cs.get_control('TSEGLimitLock')
+        ia_untrusted = 0
+        if self.cs.is_register_defined('MSR_BIOS_DONE') and self.cs.register_has_field('MSR_BIOS_DONE', 'IA_UNTRUSTED'):
+            ia_untrusted = self.cs.read_register_field('MSR_BIOS_DONE', 'IA_UNTRUSTED')
 
-        if tseg_base_lock and tseg_limit_lock:
+        if (tseg_base_lock and tseg_limit_lock) or (0 != ia_untrusted):
             self.logger.log_good( "TSEG range is locked" )
             return ModuleResult.PASSED
         else:
             self.logger.log_bad( "TSEG range is not locked" )
             return ModuleResult.FAILED
 
     def check_tseg_config(self):
         res = ModuleResult.FAILED
         (tseg_base,  tseg_limit,  tseg_size ) = self.cs.cpu.get_TSEG()
-        self.logger.log("[*] TSEG      : 0x{:016X} - 0x{:016X} (size = 0x{:08X})".format(tseg_base,  tseg_limit,  tseg_size ))      
+        self.logger.log("[*] TSEG      : 0x{:016X} - 0x{:016X} (size = 0x{:08X})".format(tseg_base,  tseg_limit,  tseg_size ))
         if (self.cs.cpu.check_SMRR_supported()):
             (smram_base, smram_limit, smram_size) = self.cs.cpu.get_SMRR_SMRAM()
             self.logger.log("[*] SMRR range: 0x{:016X} - 0x{:016X} (size = 0x{:08X})\n".format(smram_base, smram_limit, smram_size))
         else:
             smram_base = 0
             smram_limit = 0
             self.logger.log("[*] SMRR is not supported\n")
@@ -74,15 +78,15 @@
         if (0 == smram_base) and (0 == smram_limit):
             res = ModuleResult.WARNING
             self.logger.log_warn_check( "TSEG is properly configured but can't determine if it covers entire SMRAM" )
         else:
             if (tseg_base <= smram_base) and (smram_limit <= tseg_limit):
             #if (tseg_base == smram_base) and (tseg_size == smram_size):
                 self.logger.log_good( "TSEG range covers entire SMRAM" )
-                if self.check_tseg_locks() == ModuleResult.PASSED:                    
+                if self.check_tseg_locks() == ModuleResult.PASSED:
                     res = ModuleResult.PASSED
                     self.logger.log_passed_check( "TSEG is properly configured. SMRAM is protected from DMA attacks" )
                 else:
                     self.logger.log_failed_check( "TSEG is properly configured, but the configuration is not locked." )
             else:
                 self.logger.log_bad( "TSEG range doesn't cover entire SMRAM" )
                 self.logger.log_failed_check( "TSEG is not properly configured. Portions of SMRAM may be vulnerable to DMA attacks" )
@@ -93,8 +97,8 @@
     # run( module_argv )
     # Required function: run here all tests from this module
     # --------------------------------------------------------------------------
     def run( self, module_argv ):
         self.logger.start_test( "SMM TSEG Range Configuration Check" )
         self.res = self.check_tseg_config()
         return self.res
-        
+
```

### Comparing `chipsec-1.4.4/chipsec/modules/byt/__init__.py` & `chipsec-1.5.1/chipsec/modules/common/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/hsw/__init__.py` & `chipsec-1.5.1/chipsec/modules/common/secureboot/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/ivb/__init__.py` & `chipsec-1.5.1/chipsec/modules/common/uefi/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/__init__.py` & `chipsec-1.5.1/chipsec/modules/hsw/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/common/spi_access.py` & `chipsec-1.5.1/chipsec/modules/common/spi_access.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2017, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -25,67 +25,76 @@
 
 
 
 """
 Checks SPI Flash Region Access Permissions programmed in the Flash Descriptor
 """
 
-from chipsec.module_common import *
-TAGS = [MTAG_BIOS]
+from chipsec.module_common import BaseModule, ModuleResult, MTAG_BIOS
+from chipsec.hal.spi import SPI, GBE, PLATFORM_DATA, ME, FLASH_DESCRIPTOR
 
-from chipsec.hal import spi
+TAGS = [MTAG_BIOS]
 
 class spi_access(BaseModule):
 
     def __init__(self):
         BaseModule.__init__(self)
-        self.spi    = spi.SPI( self.cs )
+        self.spi    = SPI( self.cs )
 
     def is_supported(self):
         return True
 
     ##
     # Displays the SPI Regions Access Permissions
     def check_flash_access_permissions(self):
 
         res = ModuleResult.PASSED
+        fdv = self.cs.read_register_field( 'HSFS', 'FDV' ) == 1
         frap = self.cs.read_register( 'FRAP' )
         brra = self.cs.get_register_field( 'FRAP', frap, 'BRRA' )
         brwa = self.cs.get_register_field( 'FRAP', frap, 'BRWA' )
         if self.cs.is_register_defined('FDOC') and self.cs.is_register_defined('FDOD'):
             self.cs.write_register('FDOC', 0x3000)
             tmp_reg = self.cs.read_register('FDOD')
             brra |= ((tmp_reg >> 8) & 0xFFF)
             brwa |= ((tmp_reg >> 20) & 0xFFF)
 
         # Informational
+        # State of Flash Descriptor Valid bit
+        if not fdv:
+            self.logger.log("[*] Flash Descriptor Valid bit is not set")
+
         # CPU/Software access to Platform Data region (platform specific)
-        if brwa & (1 << spi.PLATFORM_DATA):
+        if brwa & (1 << PLATFORM_DATA):
             self.logger.log("[*] Software has write access to Platform Data region in SPI flash (it's platform specific)")
 
         # Warnings
         # CPU/Software access to GBe region
-        if brwa & (1 << spi.GBE):
+        if brwa & (1 << GBE):
             res = ModuleResult.WARNING
             self.logger.log_warning("Software has write access to GBe region in SPI flash")
 
         # Failures
         # CPU/Software access to Flash Descriptor region (Read Only)
-        if brwa & (1 << spi.FLASH_DESCRIPTOR):
+        if brwa & (1 << FLASH_DESCRIPTOR):
             res = ModuleResult.FAILED
             self.logger.log_bad("Software has write access to SPI flash descriptor")
 
         # CPU/Software access to Intel ME region (Read Only)
-        if brwa & (1 << spi.ME):
+        if brwa & (1 << ME):
             res = ModuleResult.FAILED
             self.logger.log_bad("Software has write access to Management Engine (ME) region in SPI flash")
 
-        if   ModuleResult.PASSED  == res: self.logger.log_passed_check("SPI Flash Region Access Permissions in flash descriptor look ok")
-        elif ModuleResult.FAILED  == res: self.logger.log_failed_check("SPI Flash Region Access Permissions are not programmed securely in flash descriptor")
-        elif ModuleResult.WARNING == res: self.logger.log_warn_check("Certain SPI flash regions are writeable by software")
+        if fdv:
+            if   ModuleResult.PASSED  == res: self.logger.log_passed_check("SPI Flash Region Access Permissions in flash descriptor look ok")
+            elif ModuleResult.FAILED  == res: self.logger.log_failed_check("SPI Flash Region Access Permissions are not programmed securely in flash descriptor")
+            elif ModuleResult.WARNING == res: self.logger.log_warn_check("Certain SPI flash regions are writeable by software")
+        else:
+            res = ModuleResult.WARNING
+            self.logger.log_warn_check("Either flash descriptor is not valid or not present on this system")
 
         return res
 
     # --------------------------------------------------------------------------
     # run( module_argv )
     # Required function: run here all tests from this module
     # --------------------------------------------------------------------------
```

### Comparing `chipsec-1.4.4/chipsec/modules/common/spi_desc.py` & `chipsec-1.5.1/chipsec/modules/common/spi_desc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2015, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -23,16 +23,17 @@
 """
 The SPI Flash Descriptor indicates read/write permissions for devices to access regions of the flash memory. This module simply reads the Flash Descriptor and checks that software cannot modify the Flash Descriptor itself. If software can write to the Flash Descriptor, then software could bypass any protection defined by it. While often used for debugging, this should not be the case on production systems.
 
 This module checks that software cannot write to the flash descriptor.
 
 """
 
-from chipsec.module_common import *
-import chipsec.hal.spi
+from chipsec.module_common import BaseModule, ModuleResult, MTAG_BIOS
+from chipsec.hal.spi import FLASH_DESCRIPTOR
+
 TAGS = [MTAG_BIOS]
 
 class spi_desc(BaseModule):
 
     def __init__(self):
         BaseModule.__init__(self)
 
@@ -47,15 +48,15 @@
         res = ModuleResult.PASSED
         frap = self.cs.read_register( 'FRAP' )
         self.cs.print_register( 'FRAP', frap )
         brra = self.cs.get_register_field( 'FRAP', frap, 'BRRA' )
         brwa = self.cs.get_register_field( 'FRAP', frap, 'BRWA' )
 
         self.logger.log("[*] Software access to SPI flash regions: read = 0x{:02X}, write = 0x{:02X}".format(brra, brwa) )
-        if brwa & (1 << chipsec.hal.spi.FLASH_DESCRIPTOR):
+        if brwa & (1 << FLASH_DESCRIPTOR):
             res = ModuleResult.FAILED
             self.logger.log_bad("Software has write access to SPI flash descriptor")
 
         self.logger.log('')
         if   ModuleResult.PASSED == res: self.logger.log_passed_check("SPI flash permissions prevent SW from writing to flash descriptor")
         elif ModuleResult.FAILED == res: self.logger.log_failed_check("SPI flash permissions allow SW to write flash descriptor")
         return res
```

### Comparing `chipsec-1.4.4/chipsec/modules/common/spi_fdopss.py` & `chipsec-1.5.1/chipsec/modules/common/spi_fdopss.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2016, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -18,15 +18,16 @@
 #chipsec@intel.com
 #
 
 """
 Checks for SPI Controller Flash Descriptor Security Override Pin Strap (FDOPSS). On some systems, this may be routed to a jumper on the motherboard. 
 """
 
-from chipsec.module_common import *
+from chipsec.module_common import BaseModule, ModuleResult, MTAG_BIOS
+
 TAGS = [MTAG_BIOS]
 
 class spi_fdopss(BaseModule):
 
     def __init__(self):
         BaseModule.__init__(self)
```

### Comparing `chipsec-1.4.4/chipsec/modules/common/uefi/access_uefispec.py` & `chipsec-1.5.1/chipsec/modules/common/uefi/access_uefispec.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2015, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -22,21 +22,20 @@
 
 """
 Checks protection of UEFI variables defined in the UEFI spec to have certain permissions. 
 
 Returns failure if variable attributes are not as defined in `table 11 "Global Variables" <http://uefi.org/>`_ of the UEFI spec.
 """
 
-from chipsec.module_common import *
-from chipsec.file          import *
-from chipsec.hal.uefi      import *
+from chipsec.module_common import BaseModule, ModuleResult, MTAG_SECUREBOOT, MTAG_BIOS, OPT_MODIFY
+from chipsec.hal.uefi import UEFI, EFI_VARIABLE_NON_VOLATILE, EFI_VARIABLE_BOOTSERVICE_ACCESS, EFI_VARIABLE_RUNTIME_ACCESS, get_attr_string
+from chipsec.hal.uefi import EFI_VARIABLE_TIME_BASED_AUTHENTICATED_WRITE_ACCESS, EFI_VARIABLE_AUTHENTICATED_WRITE_ACCESS, EFI_VARIABLE_APPEND_WRITE
 
-TAGS = [MTAG_BIOS]
-TAGS += [MTAG_SECUREBOOT]
 
+TAGS = [MTAG_BIOS, MTAG_SECUREBOOT]
 
 class access_uefispec(BaseModule):
 
     def __init__(self):
         BaseModule.__init__(self)
         self._uefi = UEFI(self.cs)
 
@@ -125,20 +124,19 @@
                 nameguid = name+' ('+guid+')'
                 self.logger.log_bad('RECOVERY FAILED. Variable {} remains corrupted. Original data value: {}'.format(nameguid, origdata))
         return ret
 
 
     def check_vars(self, do_modify):
         res = ModuleResult.PASSED
-        error = False
         vars = self._uefi.list_EFI_variables()
         if vars is None:
-            self.logger.log_error_check( 'Could not enumerate UEFI Variables from runtime (Legacy OS?)' )
+            self.logger.log_warn_check( 'Could not enumerate UEFI Variables from runtime.' )
             self.logger.log_important( "Note that UEFI variables may still exist, OS just did not expose runtime UEFI Variable API to read them.\nYou can extract variables directly from ROM file via 'chipsec_util.py uefi nvram bios.bin' command and verify their attributes manually." )
-            return ModuleResult.ERROR
+            return ModuleResult.SKIPPED
 
         bsnv_vars = []
         bsnv_concern = []
         rtnv_vars = []
         rtnv_concern = []
         modified_concern = []
         uefispec_concern = []
@@ -174,28 +172,28 @@
                     if name in self.uefispec_ro_vars:
                         self.logger.log("[*] Testing modification of {} ..".format(name))
                         if self.can_modify(name, guid, data):
                             ro_concern.append(name)
                             self.logger.log_bad("Variable {} should be read only.".format(name))
                             res = ModuleResult.FAILED
 
-        self.logger.log('')
-        self.logger.log_bad('Variables with attributes that differ from UEFI spec:')
-        for name in uefispec_concern:
-            self.logger.log('    {}'.format(name))
+        if uefispec_concern:
+            self.logger.log('')
+            self.logger.log_bad('Variables with attributes that differ from UEFI spec:')
+            for name in uefispec_concern:
+                self.logger.log('    {}'.format(name))
 
         if do_modify:
             self.logger.log('')
             self.logger.log_bad('Variables that should have been read-only and were not:')
             for name in ro_concern:
                 self.logger.log('    {}'.format(name))
 
         self.logger.log('')
 
-        if error: return ModuleResult.ERROR
         if   ModuleResult.PASSED == res: self.logger.log_passed_check( 'All checked EFI variables are protected according to spec.' )
         elif ModuleResult.FAILED == res: self.logger.log_failed_check('Some EFI variables were not protected according to spec.')
         return res
 
 
     def run( self,  module_argv ):
         self.logger.start_test( "Access Control of EFI Variables" )
```

### Comparing `chipsec-1.4.4/chipsec/modules/common/uefi/s3bootscript.py` & `chipsec-1.5.1/chipsec/modules/common/uefi/s3bootscript.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2016, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -42,59 +42,59 @@
 Examples:
 
     >>> chipsec_main.py -m common.uefi.s3bootscript
     >>> chipsec_main.py -m common.uefi.s3bootscript -a 0x00000000BDE10000
 
 """
 
-from chipsec.module_common import *
-
-import chipsec.hal.uefi
-import chipsec.hal.uefi_common
+from chipsec.module_common import BaseModule, ModuleResult, MTAG_BIOS, MTAG_SMM, MTAG_SECUREBOOT
+from chipsec.defines import BOUNDARY_1MB, BOUNDARY_4GB
+from chipsec.hal.uefi import UEFI, parse_script
+from chipsec.hal.uefi_common import S3BootScriptOpcode
 
 TAGS = [MTAG_BIOS,MTAG_SMM,MTAG_SECUREBOOT]
 
 ########################################################################################################
 #
 # Main module functionality
 #
 ########################################################################################################
 BOOTSCRIPT_OK                  = 0x0
 BOOTSCRIPT_INSIDE_SMRAM        = 0x1
 BOOTSCRIPT_OUTSIDE_SMRAM       = 0x2
 DISPATCH_OPCODES_UNPROTECTED   = 0x4
 DISPATCH_OPCODES_PROTECTED     = 0x8
 
-HIGH_BIOS_RANGE_SIZE = 2*chipsec.defines.BOUNDARY_1MB 
+HIGH_BIOS_RANGE_SIZE = 2*BOUNDARY_1MB
 
 class s3bootscript(BaseModule):
 
     def __init__(self):
         BaseModule.__init__(self)
-        self._uefi = chipsec.hal.uefi.UEFI( self.cs )
+        self._uefi = UEFI( self.cs )
 
     def is_supported(self):
         supported = self.cs.helper.EFI_supported()
         if not supported: self.logger.log_skipped_check( "OS does not support UEFI Runtime API" )
         return supported
 
     def is_inside_SMRAM( self, pa ):
         #return ( (self.smrrbase & self.smrrmask) == ( pa & self.smrrmask ) )
         return ( pa >= self.smrambase and pa < self.smramlimit)
 
     def is_inside_SPI( self, pa ):
-        return ( pa >= (chipsec.defines.BOUNDARY_4GB - HIGH_BIOS_RANGE_SIZE) and pa < chipsec.defines.BOUNDARY_4GB )
+        return ( pa >= (BOUNDARY_4GB - HIGH_BIOS_RANGE_SIZE) and pa < BOUNDARY_4GB )
 
     def check_dispatch_opcodes( self, bootscript_entries ):
         self.logger.log( '[*] Checking entry-points of Dispatch opcodes..' )
         dispatch_ep_ok = True
         n_dispatch = 0
         for e in bootscript_entries:
             if e.decoded_opcode is None: continue
-            if chipsec.hal.uefi_common.S3BootScriptOpcode.EFI_BOOT_SCRIPT_DISPATCH_OPCODE   == e.decoded_opcode.opcode:
+            if S3BootScriptOpcode.EFI_BOOT_SCRIPT_DISPATCH_OPCODE   == e.decoded_opcode.opcode:
                #chipsec.hal.uefi_common.S3BootScriptOpcode.EFI_BOOT_SCRIPT_DISPATCH_2_OPCODE == e.decoded_opcode.opcode:
                 n_dispatch += 1
                 dispatchstr = "Dispatch opcode (off 0x{:04X}) with entry-point 0x{:016X}".format(e.offset_in_script, e.decoded_opcode.entrypoint)
                 #self.logger.log( e )
                 if not self.is_inside_SMRAM( e.decoded_opcode.entrypoint ) and not self.is_inside_SPI( e.decoded_opcode.entrypoint ):
                     dispatch_ep_ok = False
                     self.logger.log_bad( dispatchstr + " > UNPROTECTED"  )
@@ -114,48 +114,44 @@
             self.logger.log_important( "Note: the test could not verify Dispatch opcodes because the script is in SMRAM. Entry-points of Dispatch opcodes also need to be protected." )
         else:
             res |= BOOTSCRIPT_OUTSIDE_SMRAM
             self.logger.log_bad( 'S3 boot-script is not in SMRAM' )
             self.logger.log( '[*] Reading S3 boot-script from memory..' )
             script_all = self.cs.mem.read_physical_mem( bootscript_pa, 0x100000 )
             self.logger.log( '[*] Decoding S3 boot-script opcodes..' )
-            script_entries = chipsec.hal.uefi.parse_script( script_all, False )               
+            script_entries = parse_script( script_all, False )
             dispatch_opcodes_ok = self.check_dispatch_opcodes( script_entries )
             if dispatch_opcodes_ok:
                 res |= DISPATCH_OPCODES_PROTECTED
                 self.logger.log_important( "S3 boot-script is not in protected memory but didn't find unprotected Dispatch entry-points" )
             else:
                 res |= DISPATCH_OPCODES_UNPROTECTED
                 self.logger.log_bad( 'Entry-points of Dispatch opcodes in S3 boot-script are not in protected memory' )
         return res
 
     def check_s3_bootscripts( self, bsaddress = None ):
         res    = 0
-        status = ModuleResult.ERROR
         scriptInsideSMRAM = False
 
         if bsaddress:
             bootscript_PAs = [ bsaddress ]
         else:
             found,bootscript_PAs = self._uefi.find_s3_bootscript()
             if not found:
                 self.logger.log_good( "Didn't find any S3 boot-scripts in EFI variables" )
-                self.logger.log_warn_check( "S3 Boot-Script was not found. Firmware may be using other ways to store/locate it" )
+                self.logger.log_warn_check( "S3 Boot-Script was not found. Firmware may be using other ways to store/locate it, or OS might be blocking access." )
                 return ModuleResult.WARNING
 
             self.logger.log_important( 'Found {:d} S3 boot-script(s) in EFI variables'.format(len(bootscript_PAs)) )
 
         for bootscript_pa in bootscript_PAs:
             if 0 == bootscript_pa: continue
             res |= self.check_s3_bootscript( bootscript_pa )
 
         self.logger.log('')
-        #if BOOTSCRIPT_OK == res:
-        #    status = ModuleResult.PASSED
-        #    self.logger.log_passed_check( 'S3 Boot-Scripts including Dispatch entry-points seem to be stored in protected locations' )
 
         if (res & BOOTSCRIPT_OUTSIDE_SMRAM) != 0:
             # BOOTSCRIPT_OUTSIDE_SMRAM
             if (res & DISPATCH_OPCODES_UNPROTECTED) != 0:
                 # DISPATCH_OPCODES_UNPROTECTED
                 status = ModuleResult.FAILED
                 self.logger.log_failed_check( 'S3 Boot-Script and Dispatch entry-points do not appear to be protected' )
```

### Comparing `chipsec-1.4.4/chipsec/modules/common/uefi/__init__.py` & `chipsec-1.5.1/chipsec/modules/ivb/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/common/bios_wp.py` & `chipsec-1.5.1/chipsec/modules/common/bios_wp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2015, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -30,17 +30,16 @@
 SMM based write protection is controlled from the BIOS Control Register. When the BIOS Write Protect Disable bit is set (sometimes called BIOSWE or BIOS Write Enable), then writes are allowed. When cleared, it can also be locked with the BIOS Lock Enable (BLE) bit. When locked, attempts to change the WPD bit will result in generation of an SMI. This way, the SMI handler can decide whether to perform the write.
 
 As demonstrated in the `Speed Racer <https://bromiumlabs.files.wordpress.com/2015/01/speed_racer_whitepaper.pdf>`_ issue, a race condition may exist between the outstanding write and processing of the SMI that is generated. For this reason, the EISS bit (sometimes called SMM_BWP or SMM BIOS Write Protection) must be set to ensure that only SMM can write to the SPI flash.
 
 This module common.bios_wp will fail if SMM-based protection is not correctly configured and SPI protected ranges (PR registers) do not protect the entire BIOS region. 
 """
 
-from chipsec.module_common import *
-from chipsec.hal.mmio import *
-from chipsec.hal.spi import *
+from chipsec.module_common import BaseModule, ModuleResult, MTAG_BIOS
+from chipsec.hal.spi import BIOS, SPI
 
 import fnmatch
 import os
 
 TAGS = [MTAG_BIOS]
 
 class bios_wp(BaseModule):
@@ -53,22 +52,17 @@
         return True
 
     def check_BIOS_write_protection(self):
         self.logger.start_test( "BIOS Region Write Protection" )
         #
         # BIOS Control Register
         #
-        #reg_value = chipsec.chipset.read_register(self.cs, 'BC')
-        #chipsec.chipset.print_register(self.cs, 'BC', reg_value)
 
-        #ble    = chipsec.chipset.get_register_field(self.cs, 'BC', reg_value, 'BLE')
         ble = self.cs.get_control('BiosLockEnable', with_print=True)
-        #bioswe = self.cs.get_register_field('BC', reg_value, 'BIOSWE')
         bioswe = self.cs.get_control('BiosWriteEnable')
-        #smmbwp = chipsec.chipset.get_register_field(self.cs, 'BC', reg_value, 'SMM_BWP')
         smmbwp = self.cs.get_control( 'SmmBiosWriteProtection' )
 
         # Is the BIOS flash region write protected?
         write_protected = 0
         if 1 == ble and 0 == bioswe:
             if 1 == smmbwp:
                 self.logger.log_good( "BIOS region write protection is enabled (writes restricted to SMM)" )
@@ -83,20 +77,14 @@
     def check_SPI_protected_ranges(self):
         (bios_base,bios_limit,bios_freg) = self.spi.get_SPI_region( BIOS )
         self.logger.log( "\n[*] BIOS Region: Base = 0x{:08X}, Limit = 0x{:08X}".format(bios_base,bios_limit) )
         self.spi.display_SPI_Protected_Ranges()
 
         pr_cover_bios = False
         pr_partial_cover_bios = False
-    #    for j in range(5):
-    #        (base,limit,wpe,rpe,pr_reg_off,pr_reg_value) = spi.get_SPI_Protected_Range( j )
-    #        if (wpe == 1 and base < limit and base <= bios_base and limit >= bios_limit):
-    #            pr_cover_bios = True
-    #        if (wpe == 1 and base < limit and limit > bios_base):
-    #            pr_partial_cover_bios = True
 
         areas_to_protect  = [(bios_base, bios_limit)]
         protected_areas = list()
 
 
         for j in range(5):
             (base,limit,wpe,rpe,pr_reg_off,pr_reg_value) = self.spi.get_SPI_Protected_Range( j )
@@ -117,15 +105,14 @@
                     elif base <= end and limit >= end:
                         if base <= start:
                             areas_to_protect.remove(area)
                         else:
                             areas_to_protect.remove(area)
                             area = (start,base-1)
                             areas_to_protect.append(area)
-                            start,end = area
                     # split
                     elif base > start and limit < end:
                         areas_to_protect.remove(area)
                         areas_to_protect.append((start,base-1))
                         areas_to_protect.append((limit+1, end))
```

### Comparing `chipsec-1.4.4/chipsec/modules/common/bios_smi.py` & `chipsec-1.5.1/chipsec/modules/common/bios_smi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2015, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -28,41 +28,38 @@
 References:
 
 `Setup for Failure: Defeating SecureBoot <http://syscan.org/index.php/download/get/6e597f6067493dd581eed737146f3afb/SyScan2014_CoreyKallenberg_SetupforFailureDefeatingSecureBoot.zip>`_ by Corey Kallenberg, Xeno Kovah, John Butterworth, Sam Cornwell
 
 `Summary of Attacks Against BIOS and Secure Boot` (https://www.defcon.org/images/defcon-22/dc-22-presentations/Bulygin-Bazhaniul-Furtak-Loucaides/DEFCON-22-Bulygin-Bazhaniul-Furtak-Loucaides-Summary-of-attacks-against-BIOS-UPDATED.pdf)
 """
 
-from chipsec.module_common import *
-from chipsec.hal import iobar
-
+from chipsec.module_common import BaseModule, ModuleResult, MTAG_BIOS, MTAG_SMM
 
 TAGS = [MTAG_BIOS,MTAG_SMM]
 
 class bios_smi(BaseModule):
 
     def __init__(self):
         BaseModule.__init__(self)
-        self.iobar = iobar.IOBAR(self.cs)
 
     def is_supported(self):
-        return (not self.cs.is_atom())
+        return True
 
     def check_SMI_locks(self):
 
         self.logger.start_test( "SMI Events Configuration" )
-        
+
         if not self.cs.is_control_defined( 'SmmBiosWriteProtection' ) or \
            not self.cs.is_control_defined( 'TCOSMIEnable' ) or \
            not self.cs.is_control_defined( 'GlobalSMIEnable' ) or \
            not self.cs.is_control_defined( 'TCOSMILock' ) or \
            not self.cs.is_control_defined( 'SMILock' ):
             self.logger.error( "Couldn't find definition of required configuration registers" )
             return ModuleResult.ERROR
-        
+
         #
         # Checking SMM_BWP first in BIOS control to warn if SMM write-protection of the BIOS is not enabled
         #
         smm_bwp = self.cs.get_control( 'SmmBiosWriteProtection' )
         if 0 == smm_bwp: self.logger.log_bad( "SMM BIOS region write protection has not been enabled (SMM_BWP is not used)\n" )
         else:            self.logger.log_good( "SMM BIOS region write protection is enabled (SMM_BWP is used)\n" )
```

### Comparing `chipsec-1.4.4/chipsec/modules/common/smrr.py` & `chipsec-1.5.1/chipsec/modules/common/smrr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2015, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -22,36 +22,30 @@
 
 """
 Researchers demonstrated a way to use CPU cache to effectively change values in SMRAM in `Attacking SMM Memory via Intel CPU Cache Poisoning <http://www.invisiblethingslab.com/resources/misc09/smm_cache_fun.pdf>`_ and `Getting into the SMRAM: SMM Reloaded <http://cansecwest.com/csw09/csw09-duflot.pdf>`_ . If ring 0 software can make SMRAM cacheable and then populate cache lines at SMBASE with exploit code, then when an SMI is triggered, the CPU could execute the exploit code from cache. System Management Mode Range Registers (SMRRs) force non-cachable behavior and block access to SMRAM when the CPU is not in SMM. These registers need to be enabled/configured by the BIOS.
 
 This module checks to see that SMRRs are enabled and configured.
 """
 
-from chipsec.module_common import *
-from chipsec.hal.msr import *
+from chipsec.module_common import BaseModule, ModuleResult, MTAG_BIOS, MTAG_SMM, OPT_MODIFY
+from chipsec.hal.msr import MemType
 
 TAGS = [MTAG_BIOS,MTAG_SMM]
 
 class smrr(BaseModule):
 
     def __init__(self):
         BaseModule.__init__(self)
 
     def is_supported(self):
         return True
 
     #
     # Check that SMRR are supported by CPU in IA32_MTRRCAP_MSR[SMRR]
     #
-    #def check_SMRR_supported(self):
-        #mtrrcap_msr_reg = self.cs.read_register( 'MTRRCAP' )
-        #if self.logger.VERBOSE: self.cs.print_register( 'MTRRCAP', mtrrcap_msr_reg )
-        #smrr = self.cs.get_register_field( 'MTRRCAP', mtrrcap_msr_reg, 'SMRR' )
-        #return (1 == smrr)
-
     def check_SMRR(self, do_modify):
         if not self.cs.is_register_defined( 'MTRRCAP' ) or \
            not self.cs.is_register_defined( 'IA32_SMRR_PHYSBASE' ) or \
            not self.cs.is_register_defined( 'IA32_SMRR_PHYSMASK' ):
             self.logger.error( "Couldn't find definition of required configuration registers" )
             return ModuleResult.ERROR
 
@@ -74,16 +68,16 @@
         self.logger.log( "[*] Checking SMRR range base programming.." )
         msr_smrrbase = self.cs.read_register( 'IA32_SMRR_PHYSBASE' )
         self.cs.print_register( 'IA32_SMRR_PHYSBASE', msr_smrrbase )
         smrrbase = self.cs.get_register_field( 'IA32_SMRR_PHYSBASE', msr_smrrbase, 'PhysBase', True )
         smrrtype = self.cs.get_register_field( 'IA32_SMRR_PHYSBASE', msr_smrrbase, 'Type' )
         self.logger.log( "[*] SMRR range base: 0x{:016X}".format(smrrbase) )
 
-        if smrrtype in self.cs.Cfg.MemType:
-            self.logger.log( "[*] SMRR range memory type is {}".format(self.cs.Cfg.MemType[smrrtype]) )
+        if smrrtype in MemType:
+            self.logger.log( "[*] SMRR range memory type is {}".format(MemType[smrrtype]) )
         else:
             smrr_ok = False
             self.logger.log_bad( "SMRR range memory type 0x{:X} is invalid".format(smrrtype) )
 
         if ( 0 == smrrbase ):
             smrr_ok = False
             self.logger.log_bad( "SMRR range base is not programmed" )
@@ -119,35 +113,35 @@
             if (msr_base != msr_smrrbase) or (msr_mask != msr_smrrmask):
                 smrr_ok = False
                 self.logger.log_bad( "SMRR range base/mask do not match on all logical CPUs" )
                 break
 
         if smrr_ok: self.logger.log_good( "OK so far. SMRR range base/mask match on all logical CPUs" )
 
-        
+
         #
         # 5. Reading from & writing to SMRR_BASE physical address
         # writes should be dropped, reads should return all F's
         #
-        
+
         self.logger.log( "[*] Trying to read memory at SMRR base 0x{:08X}..".format(smrrbase) )
 
         ok = ( 0xFFFFFFFF == self.cs.mem.read_physical_mem_dword( smrrbase ) )
-        smrr_ok = smrr_ok and ok 
+        smrr_ok = smrr_ok and ok
         if ok: self.logger.log_passed_check( "SMRR reads are blocked in non-SMM mode" ) #return all F's
         else:  self.logger.log_failed_check( "SMRR reads are not blocked in non-SMM mode" ) #all F's are not returned
 
         if (do_modify):
             self.logger.log( "[*] Trying to modify memory at SMRR base 0x{:08X}..".format(smrrbase) )
             self.cs.mem.write_physical_mem_dword( smrrbase, 0x90909090 )
             ok = ( 0x90909090 != self.cs.mem.read_physical_mem_dword( smrrbase ) )
-            smrr_ok = smrr_ok and ok 
+            smrr_ok = smrr_ok and ok
             if ok: self.logger.log_good( "SMRR writes are blocked in non-SMM mode" )
             else:  self.logger.log_bad( "SMRR writes are not blocked in non-SMM mode" )
-        
+
 
         self.logger.log( '' )
         if not smrr_ok:
             res = ModuleResult.FAILED
             self.logger.log_failed_check( "SMRR protection against cache attack is not configured properly" )
         else:
             res = ModuleResult.PASSED
@@ -159,8 +153,7 @@
     # run( module_argv )
     # Required function: run here all tests from this module
     # --------------------------------------------------------------------------
     def run( self, module_argv ):
         self.logger.start_test( "CPU SMM Cache Poisoning / System Management Range Registers" )
         do_modify = (len(module_argv) > 0 and module_argv[0] == OPT_MODIFY)
         return self.check_SMRR( do_modify )
-
```

### Comparing `chipsec-1.4.4/chipsec/modules/common/spd_wd.py` & `chipsec-1.5.1/chipsec/modules/common/spd_wd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # CHIPSEC: Platform Security Assessment Framework
 # Copyright (c) 2019, Eclypsium, Inc.
-# Copyright (c) 2019, Intel Corporation
-# 
+# Copyright (c) 2019-2020, Intel Corporation
+#
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; Version 2.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -36,31 +36,32 @@
     INFORMATION: SMBUS_HCFG.SPD_WD is not set, but no SPDs were detected
 
 Hardware registers used:
 
     SMBUS_HCFG
 """
 
-from chipsec.module_common import *
-from chipsec.hal import smbus, spd
+from chipsec.module_common import BaseModule, ModuleResult
+from chipsec.hal.smbus import SMBus
+from chipsec.hal.spd import SPD
 
 class spd_wd(BaseModule):
 
     def __init__(self):
         BaseModule.__init__(self)
 
     def is_supported(self):
-        return self.cs.is_device_enabled( 'SMBUS' )
+        return self.cs.is_device_enabled( 'SMBUS' ) and self.cs.register_has_field('SMBUS_HCFG','SPD_WD')
 
     def check_spd_wd(self):
         self.logger.start_test( "SPD Write Disable" )
 
         try:
-            _smbus = smbus.SMBus( self.cs )
-            _spd   = spd.SPD( _smbus )
+            _smbus = SMBus( self.cs )
+            _spd   = SPD( _smbus )
         except BaseException as msg:
             self.logger.error( msg )
             self.res = ModuleResult.ERROR
             return self.res
 
         spd_wd_reg = self.cs.read_register( 'SMBUS_HCFG' )
         spd_wd = self.cs.get_register_field( 'SMBUS_HCFG', spd_wd_reg, 'SPD_WD' )
```

### Comparing `chipsec-1.4.4/chipsec/modules/common/cpu/spectre_v2.py` & `chipsec-1.5.1/chipsec/modules/common/cpu/spectre_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #CHIPSEC: Platform Security Assessment Framework
 #Copyright (c) 2018, Eclypsium, Inc.
-#Copyright (c) 2019, Intel Corporation
-# 
+#Copyright (c) 2019-2020, Intel Corporation
+#
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; Version 2.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -63,15 +63,15 @@
     STIBP is not supported or not enabled by the OS
 
 PASSED:
     IBRS/IBPB is supported
 
     Enhanced IBRS is supported
 
-    Enhanced IBRS is enabled by the OS 
+    Enhanced IBRS is enabled by the OS
 
     STIBP is supported
 
 
 Notes:
 
 - The module returns WARNING when CPU doesn't support enhanced IBRS
@@ -120,18 +120,17 @@
   https://software.intel.com/sites/default/files/managed/c5/63/336996-Speculative-Execution-Side-Channel-Mitigations.pdf
 
 - Retpoline: a software construct for preventing branch-target-injection:
   https://support.google.com/faqs/answer/7625886
 
 """
 
-from chipsec.module_common import *
-from chipsec.hal import cpu
-import chipsec.helper.oshelper
-import chipsec.defines
+from chipsec.module_common import BaseModule, MTAG_CPU, MTAG_HWCONFIG, MTAG_SMM, ModuleResult
+from chipsec.helper.oshelper import HWAccessViolationError
+from chipsec.defines import BIT26, BIT27, BIT29
 
 TAGS = [MTAG_CPU,MTAG_HWCONFIG,MTAG_SMM]
 
 class spectre_v2(BaseModule):
 
     def __init__(self):
         BaseModule.__init__(self)
@@ -147,17 +146,17 @@
         except:
            cpu_thread_count = 1
 
         #
         # Read CPUID Leaf 07H
         #
         (r_eax, r_ebx, r_ecx, r_edx) = self.cs.cpu.cpuid( 0x7, 0x0 )
-        ibrs_ibpb_supported = (r_edx & chipsec.defines.BIT26) > 0
-        stibp_supported     = (r_edx & chipsec.defines.BIT27) > 0
-        arch_cap_supported  = (r_edx & chipsec.defines.BIT29) > 0
+        ibrs_ibpb_supported = (r_edx & BIT26) > 0
+        stibp_supported     = (r_edx & BIT27) > 0
+        arch_cap_supported  = (r_edx & BIT29) > 0
         self.logger.log( "[*] CPUID.7H:EDX[26] = {:d} Indirect Branch Restricted Speculation (IBRS) & Predictor Barrier (IBPB)".format(ibrs_ibpb_supported) )
         self.logger.log( "[*] CPUID.7H:EDX[27] = {:d} Single Thread Indirect Branch Predictors (STIBP)".format(stibp_supported) )
         self.logger.log( "[*] CPUID.7H:EDX[29] = {:d} IA32_ARCH_CAPABILITIES".format(arch_cap_supported) )
 
         if ibrs_ibpb_supported: self.logger.log_good( "CPU supports IBRS and IBPB" )
         else:                   self.logger.log_bad( "CPU doesn't support IBRS and IBPB" )
 
@@ -174,15 +173,15 @@
             ibrs_enh_supported = True
             #rdcl_mitigation_supported = True
             self.logger.log( "[*] checking enhanced IBRS support in IA32_ARCH_CAPABILITIES..." )
             for tid in range(cpu_thread_count):
                 arch_cap_msr = 0
                 try:
                     arch_cap_msr = self.cs.read_register( 'IA32_ARCH_CAPABILITIES', tid )
-                except chipsec.helper.oshelper.HWAccessViolationError:
+                except HWAccessViolationError:
                     self.logger.error( "couldn't read IA32_ARCH_CAPABILITIES" )
                     ibrs_enh_supported = False
                     break
 
                 ibrs_all = self.cs.get_register_field( 'IA32_ARCH_CAPABILITIES', arch_cap_msr, 'IBRS_ALL' )
                 self.logger.log( "[*]   cpu{:d}: IBRS_ALL = {:x}".format(tid, ibrs_all) )
                 if 0 == ibrs_all:
@@ -209,15 +208,15 @@
         stibp_enabled_count = 0
         if ibrs_enh_supported:
             self.logger.log( "[*] checking if OS is using Enhanced IBRS..." )
             for tid in range(cpu_thread_count):
                 spec_ctrl_msr = 0
                 try:
                     spec_ctrl_msr = self.cs.read_register( 'IA32_SPEC_CTRL', tid )
-                except chipsec.helper.oshelper.HWAccessViolationError:
+                except HWAccessViolationError:
                     self.logger.error( "couldn't read IA32_SPEC_CTRL" )
                     ibrs_enabled = False
                     break
 
                 ibrs = self.cs.get_register_field( 'IA32_SPEC_CTRL', spec_ctrl_msr, 'IBRS' )
                 self.logger.log( "[*]   cpu{:d}: IA32_SPEC_CTRL[IBRS] = {:x}".format(tid, ibrs) )
                 if 0 == ibrs:
@@ -238,41 +237,41 @@
             elif stibp_enabled_count > 0:
                 self.logger.log_good( "OS selectively enabling STIBP" )
             else:
                 self.logger.log_information( "Unable to determine if the OS uses STIBP" )
 
         #
         # Combining results of all checks into final decision
-        # 
+        #
         # FAILED : IBRS/IBPB is not supported
         # WARNING: IBRS/IBPB is supported
         #          enhanced IBRS is not supported
         # WARNING: IBRS/IBPB is supported
         #          enhanced IBRS is supported
         #          enhanced IBRS is not enabled by the OS
         # WARNING: IBRS/IBPB is supported
         #          STIBP is not supported
         # PASSED : IBRS/IBPB is supported
         #          enhanced IBRS is supported
-        #          enhanced IBRS is enabled by the OS 
+        #          enhanced IBRS is enabled by the OS
         #          STIBP is supported
         #
         if not ibrs_ibpb_supported:
             res = ModuleResult.FAILED
             self.logger.log_failed_check( "CPU mitigation (IBRS) is missing" )
         elif not ibrs_enh_supported:
             res = ModuleResult.WARNING
-            self.logger.log_warn_check( "CPU supports mitigation (IBRS) but doesn't support enhanced IBRS" ) 
+            self.logger.log_warn_check( "CPU supports mitigation (IBRS) but doesn't support enhanced IBRS" )
         elif ibrs_enh_supported and (not ibrs_enabled):
             res = ModuleResult.WARNING
             self.logger.log_warn_check( "CPU supports mitigation (enhanced IBRS) but OS is not using it" )
         else:
             if (not stibp_supported):
                 res = ModuleResult.WARNING
-                self.logger.log_warn_check( "CPU supports mitigation (enhanced IBRS) but STIBP is not supported" ) 
+                self.logger.log_warn_check( "CPU supports mitigation (enhanced IBRS) but STIBP is not supported" )
             else:
                 res = ModuleResult.PASSED
                 self.logger.log_passed_check( "CPU and OS support hardware mitigations" )
 
         self.logger.log_important( "OS may be using software based mitigation (eg. retpoline)" )
 
         return res
```

### Comparing `chipsec-1.4.4/chipsec/modules/common/cpu/cpu_info.py` & `chipsec-1.5.1/chipsec/modules/common/cpu/cpu_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
             # Get processor brand string
             brand = ''
             for eax_val in [0x80000002, 0x80000003, 0x80000004]:
                 regs = self.cs.cpu.cpuid(eax_val, 0)
                 for i in range(4):
                     brand += bytestostring(struct.pack('<I', regs[i]))
+            brand = brand.rstrip('\x00')
             self.logger.log('[*] Processor: {}'.format(brand))
 
             # Get processor version information
             (eax, ebx, ecx, edx) = self.cs.cpu.cpuid(0x01, 0x00)
             stepping = eax & 0xF
             model = (eax >> 4) & 0xF
             family = (eax >> 8) & 0xF
```

### Comparing `chipsec-1.4.4/chipsec/modules/common/cpu/__init__.py` & `chipsec-1.5.1/chipsec/modules/common/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/common/spi_lock.py` & `chipsec-1.5.1/chipsec/modules/common/spi_lock.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2018, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -24,15 +24,16 @@
 The configuration of the SPI controller, including protected ranges (PR0-PR4), is locked by HSFS[FLOCKDN] until reset. If not locked, the controller configuration may be bypassed by reprogramming these registers. 
 
 This vulnerability (not setting FLOCKDN) is also checked by other tools, including  `flashrom <http://www.flashrom.org/>`_ and Copernicus by MITRE (ref: `Copernicus: Question Your Assumptions about BIOS Security` http://www.mitre.org/capabilities/cybersecurity/overview/cybersecurity-blog/copernicus-question-your-assumptions-about).
 
 This module checks that the SPI Flash Controller configuration is locked.
 
 """
-from chipsec.module_common import *
+from chipsec.module_common import BaseModule, ModuleResult, MTAG_BIOS
+
 TAGS = [MTAG_BIOS]
 
 class spi_lock(BaseModule):
 
     def __init__(self):
         super(spi_lock, self).__init__()
 
@@ -62,13 +63,13 @@
         reg_print = False
 
         if res == ModuleResult.FAILED:
             self.logger.log_failed_check("SPI Flash Controller not locked correctly.")
         elif res == ModuleResult.PASSED:
             self.logger.log_passed_check("SPI Flash Controller locked correctly.")
         else:
-            self.logger.log_warning_check("Unable to determine if SPI Flash Controller is locked correctly.")
+            self.logger.log_warn_check("Unable to determine if SPI Flash Controller is locked correctly.")
 
         return res
 
     def run( self, module_argv ):
         return self.check_spi_lock()
```

### Comparing `chipsec-1.4.4/chipsec/modules/common/sgx_check.py` & `chipsec-1.5.1/chipsec/modules/common/sgx_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,86 +23,83 @@
 
 """
 Check SGX related configuration
 Reference: SGX BWG, CDI/IBP#: 565432
 """
 
 _MODULE_NAME = 'sgx_check'
-from chipsec.module_common import *
-from chipsec.chipset import *
-import chipsec.logger
-from chipsec.hal.msr import *
-from chipsec.hal.mmio import *
+from chipsec.module_common import BaseModule, ModuleResult, MTAG_HWCONFIG
+from chipsec.defines import BIT0, BIT1, BIT2, BIT5, BIT6, BIT7, BIT8
 TAGS = [MTAG_HWCONFIG]
 
 
 class sgx_check(BaseModule):
     def __init__(self):
         BaseModule.__init__(self)
         self.helper = self.cs.helper
         self.res = ModuleResult.PASSED
 
-    def check_sgx_config(self):
-        self.logger.start_test("Check SGX feature support")
-        self.logger.log("[*] Test if CPU has support for SGX")
+    def is_supported(self):
         sgx_cpu_support = False
-        sgx_ok = False
         for tid in range(self.cs.msr.get_cpu_thread_count()):
             status = self.helper.set_affinity(tid)
             if status == -1:
-                if logger().VERBOSE:
+                if self.logger.VERBOSE:
                     self.logger.log("[*] Failed to set affinity to CPU{:d}".format(tid))
-            (r_eax, r_ebx, r_ecx, r_edx) = self.cs.cpu.cpuid(0x07, 0x00)
+            (_, r_ebx, _, _) = self.cs.cpu.cpuid(0x07, 0x00)
             if (r_ebx & BIT2):
-                if logger().VERBOSE: self.logger.log("[*] CPU{:d}: does support SGX".format(tid))
+                if self.logger.VERBOSE: self.logger.log("[*] CPU{:d}: does support SGX".format(tid))
                 sgx_cpu_support = True
             else:
-                if logger().VERBOSE: self.logger.log("[*]CPU{:d}: does not support SGX".format(tid))
-        if sgx_cpu_support:
-            self.logger.log_good("SGX is supported on CPU")
-        else:
-            self.logger.log_information("SGX is not supported on CPU")
-            return ModuleResult.NOTAPPLICABLE
+                if self.logger.VERBOSE: self.logger.log("[*]CPU{:d}: does not support SGX".format(tid))
+        if not sgx_cpu_support:
+            self.res = ModuleResult.NOTAPPLICABLE
+        return sgx_cpu_support
+
+    def check_sgx_config(self):
+        self.logger.start_test("Check SGX feature support")
+        self.logger.log("[*] Test if CPU has support for SGX")
+        sgx_ok = False
 
         self.logger.log("\n[*] SGX BIOS enablement check")
         self.logger.log("[*] Verifying IA32_FEATURE_CONTROL MSR is configured")
         bios_feature_control_enable = True
         for tid in range(self.cs.msr.get_cpu_thread_count()):
-            if not (self.cs.read_register('IA32_FEATURE_CONTROL', tid) & BIT18):
+            if not (self.cs.read_register_field('IA32_FEATURE_CONTROL', 'SGX_GLOBAL_EN', False, tid) == 1):
                 bios_feature_control_enable = False
         if bios_feature_control_enable:
             self.logger.log_good("Intel SGX is Enabled in BIOS")
         else:
             self.logger.log_warning( "Intel SGX is not enabled in BIOS" )
             self.res = ModuleResult.WARNING
 
         self.logger.log("\n[*] Verifying IA32_FEATURE_CONTROL MSR is locked")
         locked = True
         for tid in range(self.cs.msr.get_cpu_thread_count()):
             feature_cntl_lock = self.cs.get_control('Ia32FeatureControlLock', tid)
-            if logger().VERBOSE: self.logger.log("[*] cpu{:d}: IA32_Feature_Control Lock = {:d}".format(tid, feature_cntl_lock))
+            if self.logger.VERBOSE: self.logger.log("[*] cpu{:d}: IA32_Feature_Control Lock = {:d}".format(tid, feature_cntl_lock))
             if 0 == feature_cntl_lock:
                 locked = False
         if locked:
             self.logger.log_good("IA32_Feature_Control locked")
         else:
             self.logger.log_failed("IA32_Feature_Control is unlocked")
             self.res = ModuleResult.FAILED
 
         # Verify that Protected Memory Range (PRM) is supported, MSR IA32_MTRRCAP (FEh) [12]=1
         # Check on every CPU and make sure that they are all the same values
         self.logger.log( "\n[*] Verifying if Protected Memory Range (PRMRR) is configured" )
         prmrr_enable = False
         for tid in range(self.cs.msr.get_cpu_thread_count()):
-            mtrrcap = self.cs.read_register('MTRRCAP', tid)
-            if (0 == mtrrcap & BIT12):
-                if logger().VERBOSE: self.logger.log("[*] CPU{:d} Protected Memory Range configuration is not supported".format(tid))
+            mtrrcap = self.cs.read_register_field('MTRRCAP','PRMRR', False, tid)
+            if (0 == mtrrcap):
+                if self.logger.VERBOSE: self.logger.log("[*] CPU{:d} Protected Memory Range configuration is not supported".format(tid))
             else:
                 prmrr_enable = True
-                if logger().VERBOSE: self.logger.log("[*] CPU{:d} Protected Memory Range configuration is supported".format(tid))
+                if self.logger.VERBOSE: self.logger.log("[*] CPU{:d} Protected Memory Range configuration is supported".format(tid))
         if prmrr_enable:
             self.logger.log_good( "Protected Memory Range configuration is supported" )
         else:
             self.logger.log_failed( "Protected Memory Range configuration is not supported" )
             self.res - ModuleResult.FAILED
 
         # Check PRMRR configurations on each core.
@@ -119,28 +116,29 @@
         prmrr_mask_vld = 0
         prmrr_uncore_mask_vld = 0
         prmrr_uncore_mask_vld_new = 0
         prmrr_mask_lock = 0
         prmrr_uncore_mask_lock = 0
         prmrr_uncore_mask_lock_new = 0
         prmrr_uniform = True
+        prmrr_locked = True
         check_uncore_vals = self.cs.is_register_defined('PRMRR_UNCORE_PHYBASE') and self.cs.is_register_defined('PRMRR_UNCORE_MASK')
         for tid in range(self.cs.msr.get_cpu_thread_count()):
             prmrr_valid_config_new = self.cs.read_register('PRMRR_VALID_CONFIG', tid)
             prmrr_base_new = self.cs.read_register_field('PRMRR_PHYBASE', 'PRMRR_base_address_fields', False, tid)
             prmrr_base_memtype_new = self.cs.read_register_field('PRMRR_PHYBASE', 'PRMRR_MEMTYPE', False, tid)
             prmrr_mask_new = self.cs.read_register_field('PRMRR_MASK', 'PRMRR_mask_bits', False, tid)
             prmrr_mask_vld_new = self.cs.read_register_field('PRMRR_MASK', 'PRMRR_VLD', False, tid)
             prmrr_mask_lock_new = self.cs.read_register_field('PRMRR_MASK', 'PRMRR_LOCK', False, tid)
             if check_uncore_vals:
                 prmrr_uncore_base_new = self.cs.read_register_field('PRMRR_UNCORE_PHYBASE', 'PRMRR_base_address_fields', False, tid)
                 prmrr_uncore_mask_new = self.cs.read_register_field('PRMRR_UNCORE_MASK', 'PRMRR_mask_bits', False, tid)
                 prmrr_uncore_mask_vld_new = self.cs.read_register_field('PRMRR_UNCORE_MASK', 'PRMRR_VLD', False, tid)
                 prmrr_uncore_mask_lock_new = self.cs.read_register_field('PRMRR_UNCORE_MASK', 'PRMRR_LOCK', False, tid)
-            if logger().VERBOSE:
+            if self.logger.VERBOSE:
                 self.logger.log("[*]      CPU{:d} PRMRR_VALID_CONFIG: 0x{:010X}".format(tid, prmrr_valid_config_new))
                 self.logger.log("[*]      CPU{:d} PRMRR base address: 0x{:012X}".format(tid, prmrr_base_new))
                 self.logger.log("[*]      CPU{:d} PRMRR memory type: 0x{:d}".format(tid, prmrr_base_memtype_new))
                 self.logger.log("[*]      CPU{:d} PRMRR mask address: 0x{:012X}".format(tid, prmrr_mask_new))
                 self.logger.log("[*]      CPU{:d} PRMRR mask valid: 0x{:d}".format(tid, prmrr_mask_vld_new))
                 self.logger.log("[*]      CPU{:d} PRMRR mask lock: 0x{:d}".format(tid, prmrr_mask_lock_new))
                 if check_uncore_vals:
@@ -156,14 +154,16 @@
                 prmrr_mask_vld = prmrr_mask_vld_new
                 prmrr_mask_lock = prmrr_mask_lock_new
                 prmrr_uncore_base = prmrr_uncore_base_new
                 prmrr_uncore_mask = prmrr_uncore_mask_new
                 prmrr_uncore_mask_vld = prmrr_uncore_mask_vld_new
                 prmrr_uncore_mask_lock = prmrr_uncore_mask_lock_new
                 first_iter = False
+            if prmrr_mask_lock_new == 0:
+                prmrr_locked = False
             if ((prmrr_valid_config != prmrr_valid_config_new) or
                 (prmrr_base != prmrr_base_new) or (prmrr_mask != prmrr_mask_new) or
                 (prmrr_uncore_base != prmrr_uncore_base_new) or
                 (prmrr_uncore_mask != prmrr_uncore_mask_new) or
                 (prmrr_mask_vld != prmrr_mask_vld_new) or
                 (prmrr_mask_lock != prmrr_mask_lock_new) or
                 (prmrr_uncore_mask_vld != prmrr_uncore_mask_vld_new) or
@@ -221,15 +221,15 @@
                 if prmrr_mask_vld == 0x1:
                     self.logger.log_good( "Mcheck marked PRMRR address as valid" )
                 else:
                     self.logger.log_failed( "Mcheck marked PRMRR address as invalid" )
                     self.res = ModuleResult.FAILED
                 self.logger.log("[*]  Verifying if PRMR mask register is locked")
                 self.logger.log("[*]      PRMRR mask lock: 0x%u" % prmrr_mask_lock)
-                if prmrr_mask_lock == 0x1:
+                if prmrr_locked:
                     self.logger.log_good( "PRMRR MASK register is locked" )
                 else:
                     self.logger.log_failed( "PRMRR MASK register is not locked" )
                     self.res = ModuleResult.FAILED
                 if check_uncore_vals:
                     self.logger.log("[*]  PRMRR uncore base address: 0x%012X" % prmrr_uncore_base)
                     self.logger.log("[*]  PRMRR uncore mask address: 0x%012X" % prmrr_uncore_mask)
@@ -244,33 +244,33 @@
                     self.logger.log("[*]      PRMRR uncore mask lock: 0x%u" % prmrr_uncore_mask_lock)
                     if prmrr_uncore_mask_lock == 0x1:
                         self.logger.log_good( "PMRR uncore MASK register is locked" )
                     else:
                         self.logger.log_failed( "PMRR uncore MASK register is not locked" )
                         self.res = ModuleResult.FAILED
 
-        if sgx_cpu_support and bios_feature_control_enable and locked:
+        if bios_feature_control_enable and locked:
             sgx1_instr_support = False
             sgx2_instr_support = False
             self.logger.log("\n[*] Verifying if SGX instructions are supported")
             for tid in range(self.cs.msr.get_cpu_thread_count()):
                 status = self.helper.set_affinity(tid)
                 if status == -1:
-                    if logger().VERBOSE: self.logger.log("[*] Failed to set affinity to CPU{:d}".format(tid))
+                    if self.logger.VERBOSE: self.logger.log("[*] Failed to set affinity to CPU{:d}".format(tid))
                 (r_eax, r_ebx, r_ecx, r_edx) = self.cs.cpu.cpuid(0x012, 0x00)
                 if (r_eax & BIT0):
-                    if logger().VERBOSE: self.logger.log("[*] CPU{:d} SGX-1 instructions are supported".format(tid))
+                    if self.logger.VERBOSE: self.logger.log("[*] CPU{:d} SGX-1 instructions are supported".format(tid))
                     sgx1_instr_support = True
                 else:
-                    if logger().VERBOSE: self.logger.log("[*] CPU{:d} SGX-1 instructions are not supported".format(tid))
+                    if self.logger.VERBOSE: self.logger.log("[*] CPU{:d} SGX-1 instructions are not supported".format(tid))
                 if (r_eax & BIT1):
-                    if logger().VERBOSE: self.logger.log("[*] CPU{:d} SGX-2 instructions are supported".format(tid))
+                    if self.logger.VERBOSE: self.logger.log("[*] CPU{:d} SGX-2 instructions are supported".format(tid))
                     sgx2_instr_support = True
                 else:
-                    if logger().VERBOSE: self.logger.log("[*] CPU{:d} SGX-2 instructions are not supported".format(tid))
+                    if self.logger.VERBOSE: self.logger.log("[*] CPU{:d} SGX-2 instructions are not supported".format(tid))
             if sgx1_instr_support:
                 self.logger.log_good("Intel SGX instructions are supported and available to use")
                 sgx_ok = True
             else:
                 self.logger.log_failed("Intel SGX instructions are not supported on system")
                 sgx_ok = False
             if sgx2_instr_support:
```

### Comparing `chipsec-1.4.4/chipsec/modules/common/memlock.py` & `chipsec-1.5.1/chipsec/modules/common/memlock.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
 #Copyright (c) 2018, Eclypsium, Inc.
-#Copyright (c) 2019, Intel Corporation
+#Copyright (c) 2019-2020, Intel Corporation
 #
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; Version 2.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -27,47 +27,47 @@
 PASSED : MSR_LT_LOCK_MEMORY[0] is set.
 
 Hardware registers used:
 MSR_LT_LOCK_MEMORY
 
 """
 
-from chipsec.module_common import *
-import chipsec.chipset
-import chipsec.defines
+from chipsec.module_common import BaseModule, ModuleResult
+from chipsec.helper.oshelper import HWAccessViolationError
+
 _MODULE_NAME = 'memlock'
 
 ########################################################################################################
 #
 # Main module functionality
 #
 ########################################################################################################
 
-class memlock(chipsec.module_common.BaseModule):
+class memlock(BaseModule):
 
     def __init__(self):
         BaseModule.__init__(self)
         self.res = ModuleResult.NOTAPPLICABLE
 
     def is_supported(self):
         # Workaround for Atom based processors.  Accessing this MSR on these systems
         # causes a GP fault and can't be caught in UEFI Shell.
-        if self.cs.get_chipset_id() not in chipsec.chipset.CHIPSET_FAMILY_ATOM:
+        if not self.cs.is_atom():
             if self.cs.is_register_defined( 'MSR_LT_LOCK_MEMORY' ):
                 return self.cs.register_has_field( 'MSR_LT_LOCK_MEMORY', 'LT_LOCK' )
         return False
 
     def check_MSR_LT_LOCK_MEMORY( self ):
         self.logger.log( "[X] Checking MSR_LT_LOCK_MEMORY status" )
         status = False
         for tid in range(self.cs.msr.get_cpu_thread_count()):
                 lt_lock_msr = 0
                 try:
                     lt_lock_msr = self.cs.read_register( 'MSR_LT_LOCK_MEMORY', tid )
-                except chipsec.helper.oshelper.HWAccessViolationError:
+                except HWAccessViolationError:
                     self.logger.error( "couldn't read MSR_LT_LOCK_MEMORY" )
                     break
                 lt_lock = self.cs.get_register_field( 'MSR_LT_LOCK_MEMORY', lt_lock_msr, 'LT_LOCK' )
                 self.logger.log( "[*]   cpu{:d}: MSR_LT_LOCK_MEMORY[LT_LOCK] = {:x}".format(tid, lt_lock) )
                 if 0 == lt_lock:
                     status = True
         return status
```

### Comparing `chipsec-1.4.4/chipsec/modules/common/ia32cfg.py` & `chipsec-1.5.1/chipsec/modules/common/ia32cfg.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 class ia32cfg(BaseModule):
     def __init__(self):
         BaseModule.__init__(self)
         self.res = ModuleResult.PASSED
 
     def is_supported(self):
-        return (not self.cs.is_atom())
+        return True
 
     def check_ia32feature_control(self):
         self.logger.start_test( "IA32 Feature Control Lock" )
         self.logger.log( "[*] Verifying IA32_Feature_Control MSR is locked on all logical CPUs.." )
 
         res = ModuleResult.PASSED
         for tid in range(self.cs.msr.get_cpu_thread_count()):
```

### Comparing `chipsec-1.4.4/chipsec/modules/common/bios_kbrd_buffer.py` & `chipsec-1.5.1/chipsec/modules/common/bios_kbrd_buffer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2018, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -25,17 +25,16 @@
 
 Checks for BIOS/HDD password exposure through BIOS keyboard buffer.
 
 Checks for exposure of pre-boot passwords (BIOS/HDD/pre-bot authentication SW) in the BIOS keyboard buffer.
 
 """
 
-from chipsec.hal.mmio import *
-from chipsec.hal.spi import *
-from chipsec.module_common import *
+from chipsec.module_common import BaseModule, ModuleResult, MTAG_BIOS
+from chipsec.logger import print_buffer
 
 TAGS = [MTAG_BIOS]
 
 COMMON_FILL_PTRN = "".join( ['{:1}'.format((chr(x + 0x1E))) for x in range(32)] )
 
 
 class bios_kbrd_buffer(BaseModule):
@@ -52,15 +51,15 @@
 
         kbrd_buf_head = self.cs.mem.read_physical_mem_dword( 0x41A ) & 0x000000FF
         kbrd_buf_tail = self.cs.mem.read_physical_mem_dword( 0x41C ) & 0x000000FF
         self.logger.log( "[*] Keyboard buffer head pointer = 0x{:X} (at 0x41A), tail pointer = 0x{:X} (at 0x41C)".format(kbrd_buf_head,kbrd_buf_tail) )
         bios_kbrd_buf = self.cs.mem.read_physical_mem( 0x41E, 32 )
         self.logger.log( "[*] Keyboard buffer contents (at 0x41E):" )
         bios_kbrd_buf = bios_kbrd_buf.decode('latin_1')
-        chipsec.logger.print_buffer( bios_kbrd_buf )
+        print_buffer( bios_kbrd_buf )
 
         has_contents = False
 
         if COMMON_FILL_PTRN == bios_kbrd_buf:
             self.logger.log_passed_check( "Keyboard buffer is filled with common fill pattern" )
             return ModuleResult.PASSED
```

### Comparing `chipsec-1.4.4/chipsec/modules/common/me_mfg_mode.py` & `chipsec-1.5.1/chipsec/modules/common/me_mfg_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # CHIPSEC: Platform Security Assessment Framework
 # Copyright (c) 2018, Eclypsium, Inc.
-# Copyright (c) 2019, Intel Corporation
-# 
+# Copyright (c) 2019-2020, Intel Corporation
+#
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; Version 2.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -84,15 +84,15 @@
     PASSED : HFS.MFG_MODE is not set.
 
 Hardware registers used:
 
     HFS
 """
 
-from chipsec.module_common import *
+from chipsec.module_common import BaseModule, ModuleResult
 
 class me_mfg_mode(BaseModule):
 
     def __init__(self):
         BaseModule.__init__(self)
 
     def is_supported(self):
```

### Comparing `chipsec-1.4.4/chipsec/modules/common/__init__.py` & `chipsec-1.5.1/chipsec/modules/snb/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/common/bios_ts.py` & `chipsec-1.5.1/chipsec/modules/common/bios_ts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2016, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -22,23 +22,22 @@
 
 """
 Checks for BIOS Interface Lock including Top Swap Mode
 
 `BIOS Boot Hijacking and VMware Vulnerabilities Digging <http://powerofcommunity.net/poc2007/sunbing.pdf>`_ by Bing Sun
 """
 
-from chipsec.module_common import *
-TAGS = [chipsec.module_common.MTAG_BIOS]
+from chipsec.module_common import BaseModule, ModuleResult, MTAG_BIOS
+TAGS = [MTAG_BIOS]
 
-class bios_ts(chipsec.module_common.BaseModule):
+class bios_ts(BaseModule):
     def __init__(self):
         BaseModule.__init__(self)
 
     def is_supported(self):
-        #return (self.cs.get_chipset_id() not in chipsec.chipset.CHIPSET_FAMILY_ATOM)
         return True
 
     def check_bios_iface_lock(self):
         self.logger.start_test( "BIOS Interface Lock (including Top Swap Mode)" )
 
         bild = 0
         if self.cs.is_control_defined( 'BiosInterfaceLockDown' ):
```

### Comparing `chipsec-1.4.4/chipsec/modules/common/secureboot/variables.py` & `chipsec-1.5.1/chipsec/modules/common/secureboot/variables.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2015, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -27,18 +27,18 @@
 and protected from unauthorized modification.
 
 Use '-a modify' option for the module to also try to write/corrupt the variables.
 
 """
 
 
-from chipsec.module_common import *
-
-import chipsec.file
-from chipsec.hal.uefi      import *
+from chipsec.module_common import BaseModule, ModuleResult, MTAG_SECUREBOOT, OPT_MODIFY
+from chipsec.hal.uefi import UEFI, SECURE_BOOT_VARIABLES, IS_VARIABLE_ATTRIBUTE, EFI_VAR_NAME_SecureBoot, SECURE_BOOT_KEY_VARIABLES
+from chipsec.hal.uefi import EFI_VARIABLE_TIME_BASED_AUTHENTICATED_WRITE_ACCESS, EFI_VARIABLE_AUTHENTICATED_WRITE_ACCESS
+from chipsec.hal.uefi_common import StatusCode
 
 # ############################################################
 # SPECIFY PLATFORMS THIS MODULE IS APPLICABLE TO
 # ############################################################
 _MODULE_NAME = 'variables'
 
 
@@ -96,16 +96,16 @@
         not_found = 0
         not_auth  = 0
         not_wp    = 0
         is_secureboot_enabled = False
 
         sbvars = self._uefi.list_EFI_variables()
         if sbvars is None:
-            self.logger.log_error_check( 'Could not enumerate UEFI variables (non-UEFI OS?)' )
-            return ModuleResult.ERROR
+            self.logger.log_warn_check( 'Could not enumerate UEFI variables.' )
+            return ModuleResult.SKIPPED
 
         for name in SECURE_BOOT_VARIABLES:
 
             if name in sbvars.keys() and sbvars[name] is not None:
                 if len(sbvars[name]) > 1:
                     self.logger.log_failed_check( 'There should only be one instance of variable {}'.format(name) )
                     return ModuleResult.FAILED
```

### Comparing `chipsec-1.4.4/chipsec/modules/common/secureboot/__init__.py` & `chipsec-1.5.1/chipsec/modules/tools/uefi/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/uefi/s3script_modify.py` & `chipsec-1.5.1/chipsec/modules/tools/uefi/s3script_modify.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2016, Intel Corporation
-#Copyright (c) 2019, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -95,59 +94,66 @@
     Adding new opcode:
     chipsec_main.py -m tools.uefi.s3script_modify -a add_op,<reg_opcode>,<address>,<value>,<width>
        <reg_opcode> = pci_wr|mmio_wr|io_wr
     chipsec_main.py -m tools.uefi.s3script_modify -a add_op,dispatch[,<entrypoint>]
 
 """
 
+import struct
 
-from chipsec.module_common import *
-
-from chipsec.hal.msr import *
-import chipsec.hal.uefi
-import chipsec.hal.uefi_common
-import chipsec.hal.uefi_platform
-from chipsec.hal.physmem import *
+from chipsec.module_common import BaseModule, ModuleResult
+from chipsec.logger import print_buffer
+from chipsec.hal.uefi import UEFI
+from chipsec.hal.uefi_common import S3BootScriptOpcode, script_width_values, script_width_formats, op_io_pci_mem, op_dispatch
+from chipsec.hal.uefi_platform import encode_s3bootscript_entry, id_s3bootscript_type, create_s3bootscript_entry_buffer
 
 ########################################################################################################
 #
 # Main module functionality
 #
 ########################################################################################################
 
 cmd2opcode = {
-'pci_wr' : chipsec.hal.uefi_common.S3BootScriptOpcode.EFI_BOOT_SCRIPT_PCI_CONFIG_WRITE_OPCODE, 
-'mmio_wr': chipsec.hal.uefi_common.S3BootScriptOpcode.EFI_BOOT_SCRIPT_MEM_WRITE_OPCODE,
-'io_wr'  : chipsec.hal.uefi_common.S3BootScriptOpcode.EFI_BOOT_SCRIPT_IO_WRITE_OPCODE,
-'pci_rw' : chipsec.hal.uefi_common.S3BootScriptOpcode.EFI_BOOT_SCRIPT_PCI_CONFIG_READ_WRITE_OPCODE, 
-'mmio_rw': chipsec.hal.uefi_common.S3BootScriptOpcode.EFI_BOOT_SCRIPT_MEM_READ_WRITE_OPCODE,
-'io_rw'  : chipsec.hal.uefi_common.S3BootScriptOpcode.EFI_BOOT_SCRIPT_IO_READ_WRITE_OPCODE
+'pci_wr' : S3BootScriptOpcode.EFI_BOOT_SCRIPT_PCI_CONFIG_WRITE_OPCODE,
+'mmio_wr': S3BootScriptOpcode.EFI_BOOT_SCRIPT_MEM_WRITE_OPCODE,
+'io_wr'  : S3BootScriptOpcode.EFI_BOOT_SCRIPT_IO_WRITE_OPCODE,
+'pci_rw' : S3BootScriptOpcode.EFI_BOOT_SCRIPT_PCI_CONFIG_READ_WRITE_OPCODE,
+'mmio_rw': S3BootScriptOpcode.EFI_BOOT_SCRIPT_MEM_READ_WRITE_OPCODE,
+'io_rw'  : S3BootScriptOpcode.EFI_BOOT_SCRIPT_IO_READ_WRITE_OPCODE
 
 }
 
 
 class s3script_modify(BaseModule):
 
     DISPATCH_ENTRYPOINT_INSTR = '\x90\x90\xF4\xF4'
 
     def __init__(self):
         BaseModule.__init__(self)
         self.logger.HAL = True
-        self._uefi = chipsec.hal.uefi.UEFI( self.cs )
+        self._uefi = UEFI( self.cs )
         self.bootscript_PAs = None
         self.parsed_scripts = None
 
     def get_bootscript(self):
         if self.bootscript_PAs is None or self.parsed_scripts is None:
             (self.bootscript_PAs,self.parsed_scripts) = self._uefi.get_s3_bootscript( False )
         return (self.bootscript_PAs, self.parsed_scripts)
 
     def is_supported(self):
         supported = self.cs.helper.EFI_supported()
-        if not supported: self.logger.log_skipped_check( "OS does not support UEFI Runtime API" )
+        if not supported:
+            self.logger.log( "OS does not support UEFI Runtime API" )
+            self.res = ModuleResult.NOTAPPLICABLE
+        else:
+            _, ps = self.get_bootscript()
+            if not ps:
+                self.res = ModuleResult.NOTAPPLICABLE
+                self.logger.log( "Unable to locate boot script")
+                supported = False
         return supported
 
     def modify_s3_reg( self, opcode, address, new_value ):
         (bootscript_PAs, parsed_scripts) = self.get_bootscript()
         if parsed_scripts is None: 
             self.logger.log_bad("Did not find boot script.")
             return False
@@ -164,22 +170,22 @@
                     pa = bootscript_pa + e.offset_in_script
                     self.logger.log( "[*] Modifying S3 boot script entry at address 0x{:016X}..".format(pa) )
 
                     orig_entry_buf = self.cs.mem.read_physical_mem( pa, e.length )
                     self.logger.log( "[*] Original entry:" )
                     print_buffer( orig_entry_buf )
 
-                    if chipsec.hal.uefi_common.S3BootScriptOpcode.EFI_BOOT_SCRIPT_PCI_CONFIG_WRITE_OPCODE == opcode or \
-                       chipsec.hal.uefi_common.S3BootScriptOpcode.EFI_BOOT_SCRIPT_MEM_WRITE_OPCODE        == opcode or \
-                       chipsec.hal.uefi_common.S3BootScriptOpcode.EFI_BOOT_SCRIPT_IO_WRITE_OPCODE         == opcode:
+                    if S3BootScriptOpcode.EFI_BOOT_SCRIPT_PCI_CONFIG_WRITE_OPCODE == opcode or \
+                       S3BootScriptOpcode.EFI_BOOT_SCRIPT_MEM_WRITE_OPCODE        == opcode or \
+                       S3BootScriptOpcode.EFI_BOOT_SCRIPT_IO_WRITE_OPCODE         == opcode:
                         e.decoded_opcode.values[0] = new_value
                     else:
                         e.decoded_opcode.value = new_value
 
-                    entry_buf = chipsec.hal.uefi_platform.encode_s3bootscript_entry( e )
+                    entry_buf = encode_s3bootscript_entry( e )
                     self.cs.mem.write_physical_mem( pa, e.length, entry_buf )
 
                     new_entry_buf = self.cs.mem.read_physical_mem( pa, e.length )
                     self.logger.log( "[*] Modified entry:" )
                     print_buffer( new_entry_buf )
                     return True
 
@@ -200,27 +206,27 @@
             self.logger.log_bad("Did not find boot script.")
             return False 
         for bootscript_pa in bootscript_PAs:
             if (bootscript_pa == 0): continue
             self.logger.log( "[*] Searching the script at 0x{:016X} for DISPATCH opcodes..".format(bootscript_pa) )
             for e in parsed_scripts[ bootscript_pa ]:
                 if e.decoded_opcode is not None and \
-                   chipsec.hal.uefi_common.S3BootScriptOpcode.EFI_BOOT_SCRIPT_DISPATCH_OPCODE == e.decoded_opcode.opcode:
+                   S3BootScriptOpcode.EFI_BOOT_SCRIPT_DISPATCH_OPCODE == e.decoded_opcode.opcode:
 
                     self.logger.log_good( "Found DISPATCH opcode at offset 0x{:04X}".format(e.offset_in_script) )
                     self.logger.log( e )
                     pa = bootscript_pa + e.offset_in_script
                     self.logger.log( "[*] Modifying S3 boot script entry at address 0x{:016X}..".format(pa) )
 
                     orig_entry_buf = self.cs.mem.read_physical_mem( pa, e.length )
                     self.logger.log( "[*] Original entry:" )
                     print_buffer( orig_entry_buf )
 
                     e.decoded_opcode.entrypoint = new_entrypoint
-                    entry_buf = chipsec.hal.uefi_platform.encode_s3bootscript_entry( e )
+                    entry_buf = encode_s3bootscript_entry( e )
                     self.cs.mem.write_physical_mem( pa, e.length, entry_buf )
 
                     new_entry_buf = self.cs.mem.read_physical_mem( pa, e.length )
                     self.logger.log( "[*] Modified entry:" )
                     print_buffer( new_entry_buf )
                     self.logger.log('After sleep/resume, the system should hang' )
                     return True
@@ -235,15 +241,15 @@
             self.logger.log_bad("Did not find boot script.")
             return False 
         for script_pa in bootscript_PAs:
             if (script_pa == 0): continue
             self.logger.log( "[*] Looking for DISPATCH opcode in the script at 0x{:016X}..".format(script_pa) )
             for e in parsed_scripts[ script_pa ]:
                 if e.decoded_opcode is not None and \
-                   chipsec.hal.uefi_common.S3BootScriptOpcode.EFI_BOOT_SCRIPT_DISPATCH_OPCODE == e.decoded_opcode.opcode:
+                   S3BootScriptOpcode.EFI_BOOT_SCRIPT_DISPATCH_OPCODE == e.decoded_opcode.opcode:
                     ep_pa = e.decoded_opcode.entrypoint
                     self.logger.log_good( "Found DISPATCH opcode at offset 0x{:04X} with entry-point 0x{:016X}".format(e.offset_in_script,ep_pa) )
                     self.logger.log( e )
                     break
             if ep_pa is not None: break
 
         if ep_pa is None:
@@ -269,69 +275,69 @@
 
         (bootscript_PAs, parsed_scripts) = self.get_bootscript()
         if parsed_scripts is None: 
             self.logger.log_bad("Did not find boot script.")
             return False 
         for bootscript_pa in bootscript_PAs:
             if (bootscript_pa == 0): continue
-            self.logger.log( "[*] Looking for MEM_WRITE opcode in the script at 0x{:016X}..".formatbootscript_pa )
+            self.logger.log( "[*] Looking for MEM_WRITE opcode in the script at 0x{:016X}..".format(bootscript_pa) )
             for e in parsed_scripts[ bootscript_pa ]:
                 if e.decoded_opcode is not None and \
-                   chipsec.hal.uefi_common.S3BootScriptOpcode.EFI_BOOT_SCRIPT_MEM_WRITE_OPCODE == e.decoded_opcode.opcode:
+                   S3BootScriptOpcode.EFI_BOOT_SCRIPT_MEM_WRITE_OPCODE == e.decoded_opcode.opcode:
 
                     self.logger.log_good( "Found opcode at offset 0x{:X}".format(e.offset_in_script) )
                     self.logger.log( e )
                     pa = bootscript_pa + e.offset_in_script
                     self.logger.log( "[*] Modifying S3 boot script entry at address 0x{:016X}..".format(pa) )
 
                     orig_entry_buf = self.cs.mem.read_physical_mem( pa, e.length )
                     self.logger.log( "[*] Original entry:" )
                     print_buffer( orig_entry_buf )
 
                     e.decoded_opcode.address = address
                     e.decoded_opcode.values[0] = new_value
-                    entry_buf = chipsec.hal.uefi_platform.encode_s3bootscript_entry( e )
+                    entry_buf = encode_s3bootscript_entry( e )
                     self.cs.mem.write_physical_mem( pa, e.length, entry_buf )
 
                     new_entry_buf = self.cs.mem.read_physical_mem( pa, e.length )
                     self.logger.log( "[*] Modified entry:" )
                     print_buffer( new_entry_buf )
                     self.logger.log('After sleep/resume, read address 0x{:08X} and look for value 0x{:08X}'.format(address, new_value))
                     return True
 
-        self.logger.log_bad( "Did not find required 0x{:X} opcode in the script".format(opcode) )
+        self.logger.log_bad( "Did not find required 0x{:X} opcode in the script".format(S3BootScriptOpcode.EFI_BOOT_SCRIPT_MEM_WRITE_OPCODE) )
         return False
 
     def modify_s3_add(self, new_opcode):
         e_index = None
         (bootscript_PAs, parsed_scripts) = self.get_bootscript()
-        if parsed_scripts is None: 
+        if parsed_scripts is None:
             self.logger.log_bad("Did not find boot script.")
             return False 
         for bootscript_pa in bootscript_PAs:
             if (bootscript_pa == 0): continue
             script_buffer = self.cs.mem.read_physical_mem( bootscript_pa, 4 )
-            script_type, hdr_len = chipsec.hal.uefi_platform.id_s3bootscript_type(script_buffer, False)
+            script_type, hdr_len = id_s3bootscript_type(script_buffer, False)
             self.logger.log( "[*] S3 boot script type: 0x{:0X}".format(script_type) )
 
             self.logger.log( "[*] Looking for TERMINATE opcode in the script at 0x{:016X}..".format(bootscript_pa) )
             for e in parsed_scripts[ bootscript_pa ]:
                 if e.index is not None and e.index != -1: e_index = e.index + 1
 
-                if e.decoded_opcode is not None and chipsec.hal.uefi_common.S3BootScriptOpcode.EFI_BOOT_SCRIPT_TERMINATE_OPCODE == e.decoded_opcode.opcode:                  
+                if e.decoded_opcode is not None and S3BootScriptOpcode.EFI_BOOT_SCRIPT_TERMINATE_OPCODE == e.decoded_opcode.opcode:
                     self.logger.log_good( "Found TERMINATE opcode at offset 0x{:X}".format(e.offset_in_script) )
                     self.logger.log( e )
                     pa = bootscript_pa + e.offset_in_script
                     orig_entry_buf = self.cs.mem.read_physical_mem( pa, e.length )
                     #print_buffer( orig_entry_buf )
 
                     self.logger.log( "[*] New S3 boot script opcode:" )
                     self.logger.log( new_opcode )
                     self.logger.log( "[*] Adding new opcode entry at address 0x{:016X}..".format(pa) )
-                    new_entry = chipsec.hal.uefi_platform.create_s3bootscript_entry_buffer( script_type, new_opcode, e_index )
+                    new_entry = create_s3bootscript_entry_buffer( script_type, new_opcode, e_index )
                     print_buffer( new_entry )
 
                     self.cs.mem.write_physical_mem( pa, len(new_entry), new_entry )
                     last_entry_pa = pa + len(new_entry)
                     self.logger.log( "[*] Moving TERMINATE opcode to the last entry at 0x{:016X}..".format(last_entry_pa) )
                     self.cs.mem.write_physical_mem( last_entry_pa, len(orig_entry_buf), orig_entry_buf )
                     return True
@@ -371,32 +377,32 @@
             if scmd in cmd2opcode:
                 if len(module_argv) < 5:
                     self.logger.error( 'Expected module options: -a add_op,{},<reg_address>,<value>,<width>'.format(scmd) )
                     return ModuleResult.ERROR
                 address    = int(module_argv[2],16)
                 value      = int(module_argv[3],16)
                 width      = int(module_argv[4],16)
-                width_val  = chipsec.hal.uefi_common.script_width_values[width]
-                value_buff = struct.pack("<{}".format(chipsec.hal.uefi_common.script_width_formats[width_val]), value)
-                if ( chipsec.hal.uefi_common.S3BootScriptOpcode.EFI_BOOT_SCRIPT_MEM_WRITE_OPCODE == cmd2opcode[scmd]
-                  or chipsec.hal.uefi_common.S3BootScriptOpcode.EFI_BOOT_SCRIPT_PCI_CONFIG_WRITE_OPCODE == cmd2opcode[scmd]
-                  or chipsec.hal.uefi_common.S3BootScriptOpcode.EFI_BOOT_SCRIPT_IO_WRITE_OPCODE == cmd2opcode[scmd]):
-                    new_opcode = chipsec.hal.uefi_common.op_io_pci_mem( cmd2opcode[scmd], None, width_val, address, 0, 1, value_buff, None, None )
+                width_val  = script_width_values[width]
+                value_buff = struct.pack("<{}".format(script_width_formats[width_val]), value)
+                if ( S3BootScriptOpcode.EFI_BOOT_SCRIPT_MEM_WRITE_OPCODE == cmd2opcode[scmd]
+                  or S3BootScriptOpcode.EFI_BOOT_SCRIPT_PCI_CONFIG_WRITE_OPCODE == cmd2opcode[scmd]
+                  or S3BootScriptOpcode.EFI_BOOT_SCRIPT_IO_WRITE_OPCODE == cmd2opcode[scmd]):
+                    new_opcode = op_io_pci_mem( cmd2opcode[scmd], None, width_val, address, 0, 1, value_buff, None, None )
                 else:
                     self.logger.error( "Unsupported opcode: {}".format(scmd) )
                     self.logger.log( examples_str )
                     return ModuleResult.ERROR
             elif 'dispatch' == scmd:
                 if len(module_argv) < 3:
                     (smram_base, smram_limit, smram_size) = self.cs.cpu.get_SMRAM()
                     (va, entrypoint) = self.cs.mem.alloc_physical_mem( 0x1000, smram_base )
                     self.cs.mem.write_physical_mem( entrypoint, len(self.DISPATCH_ENTRYPOINT_INSTR), self.DISPATCH_ENTRYPOINT_INSTR )
                 else:
                     entrypoint = int(module_argv[2],16)
-                new_opcode = chipsec.hal.uefi_common.op_dispatch( chipsec.hal.uefi_common.S3BootScriptOpcode.EFI_BOOT_SCRIPT_DISPATCH_OPCODE, None, entrypoint )
+                new_opcode = op_dispatch( S3BootScriptOpcode.EFI_BOOT_SCRIPT_DISPATCH_OPCODE, None, entrypoint )
             else:
                 self.logger.error( "Unrecognized opcode: {}".format(scmd) )
                 self.logger.log( examples_str )
                 return ModuleResult.ERROR
 
             sts = self.modify_s3_add( new_opcode )
         else:
```

### Comparing `chipsec-1.4.4/chipsec/modules/tools/uefi/blacklist.json` & `chipsec-1.5.1/chipsec/modules/tools/uefi/blacklist.json`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/uefi/blacklist.py` & `chipsec-1.5.1/chipsec/modules/tools/uefi/blacklist.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2016, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -28,53 +28,54 @@
 Important! This module can only detect what it knows about from its config file.
 If a bad or vulnerable binary is not detected then its 'signature' needs to be added to the config.
 
 Usage:
   ``chipsec_main.py -i -m tools.uefi.blacklist [-a <fw_image>,<blacklist>]``
     - ``fw_image``	Full file path to UEFI firmware image. If not specified, the module will dump firmware image directly from ROM
     - ``blacklist``	JSON file with configuration of black-listed EFI binaries (default = ``blacklist.json``). Config file should be located in the same directory as this module
-    
+
 Examples:
 
->>> chipsec_main.py -m tools.uefi.blacklist 
+>>> chipsec_main.py -m tools.uefi.blacklist
 
 Dumps UEFI firmware image from flash memory device, decodes it and checks for black-listed EFI modules defined in the default config ``blacklist.json``
 
 >>> chipsec_main.py -i --no_driver -m tools.uefi.blacklist -a uefi.rom,blacklist.json
 
 Decodes ``uefi.rom`` binary with UEFI firmware image and checks for black-listed EFI modules defined in ``blacklist.json`` config
 
 Note: ``-i`` and ``--no_driver`` arguments can be used in this case because the test does not depend on the platform and no kernel driver is required when firmware image is specified
 """
 import json
+import os
 
-from chipsec.module_common import *
-
-from chipsec.hal import spi_uefi
-import chipsec.hal.uefi
-import chipsec.hal.spi
-import chipsec.hal.uefi_search
+from chipsec.module_common import BaseModule, ModuleResult, MTAG_BIOS
+from chipsec.hal.spi_uefi import search_efi_tree, build_efi_model, EFIModuleType
+from chipsec.hal.uefi import UEFI
+from chipsec.hal.spi import SPI, BIOS
+from chipsec.hal.uefi_search import check_match_criteria
+from chipsec.file import read_file, get_main_dir
 
 TAGS = [MTAG_BIOS]
 
 DEF_FWIMAGE_FILE = 'fw.bin'
 
 USAGE_TEXT = '''
 Usage:
 
     chipsec_main.py -i -m tools.uefi.blacklist [-a <fw_image>,<blacklist>]
 
       fw_image  : Full file path to UEFI firmware image
                   If not specified, the module will dump firmware image directly from ROM
       blacklist : JSON file with configuration of black-listed EFI binaries (default = blacklist.json)
                   Config file should be located in the same directory as this module
-    
+
 Examples:
 
-    chipsec_main.py -m tools.uefi.blacklist 
+    chipsec_main.py -m tools.uefi.blacklist
 
       Dumps UEFI firmware image from flash memory device, decodes it and
       checks for black-listed EFI modules defined in the default config 'blacklist.json'
 
     chipsec_main.py -i --no_driver -m tools.uefi.blacklist -a uefi.rom,blacklist.json
 
       Decodes 'uefi.rom' binary with UEFI firmware image and
@@ -84,24 +85,24 @@
 If a bad or vulnerable binary is not detected then its 'signature' needs to be added to the config.
 '''
 
 class blacklist(BaseModule):
 
     def __init__(self):
         BaseModule.__init__(self)
-        self.uefi = chipsec.hal.uefi.UEFI( self.cs )
+        self.uefi = UEFI( self.cs )
         self.cfg_name = 'blacklist.json'
         self.image = None
         self.efi_blacklist = None
 
     def is_supported(self):
         return True
 
     def blacklist_callback(self, efi_module):
-        return chipsec.hal.uefi_search.check_match_criteria(efi_module, self.efi_blacklist, self.logger)
+        return check_match_criteria(efi_module, self.efi_blacklist, self.logger)
 
     def check_blacklist( self ):
         res = ModuleResult.PASSED
 
         self.logger.log( "[*] searching for EFI binaries that match criteria from '{}':".format(self.cfg_name) )
         for k in self.efi_blacklist.keys():
             entry = self.efi_blacklist[k]
@@ -109,18 +110,18 @@
             #if 'match' in entry:
             #    for c in entry['match'].keys(): self.logger.log( "[*]   {}".format(entry['match'][c]) )
             #if 'exclude' in entry:
             #    self.logger.log( "[*]   excluding binaries:" )
             #    for c in entry['exclude']: self.logger.log( "[*]   {}".format(entry['exclude'][c]) )
 
         # parse the UEFI firmware image and look for EFI modules matching the balck-list
-        efi_tree = spi_uefi.build_efi_model(self.uefi, self.image, None)
+        efi_tree = build_efi_model(self.uefi, self.image, None)
         #match_types = (spi_uefi.EFIModuleType.SECTION_EXE|spi_uefi.EFIModuleType.FILE)
-        match_types = spi_uefi.EFIModuleType.SECTION_EXE
-        matching_modules = spi_uefi.search_efi_tree(efi_tree, self.blacklist_callback, match_types)
+        match_types = EFIModuleType.SECTION_EXE
+        matching_modules = search_efi_tree(efi_tree, self.blacklist_callback, match_types)
         found = len(matching_modules) > 0
         self.logger.log( '' )
         if found:
             res = ModuleResult.WARNING
             self.logger.log_warn_check("Black-listed EFI binary found in the UEFI firmware image")
         else:
             self.logger.log_passed_check("Didn't find any black-listed EFI binary")
@@ -138,29 +139,29 @@
         self.logger.start_test( "Check for black-listed EFI binaries in UEFI firmware" )
 
         self.usage()
 
         image_file = DEF_FWIMAGE_FILE
         if len(module_argv) == 0:
             # Read firmware image directly from SPI flash memory
-            self.spi = chipsec.hal.spi.SPI( self.cs )
-            (base,limit,freg) = self.spi.get_SPI_region( chipsec.hal.spi.BIOS )
+            self.spi = SPI( self.cs )
+            (base,limit,freg) = self.spi.get_SPI_region( BIOS )
             image_size = limit + 1 - base
             self.logger.log( "[*] dumping FW image from ROM to {}: 0x{:08X} bytes at [0x{:08X}:0x{:08X}]".format(image_file,base,limit,image_size) )
             self.logger.log( "[*] this may take a few minutes (instead, use 'chipsec_util spi dump')..." )
             self.spi.read_spi_to_file( base, image_size, image_file )
         elif len(module_argv) > 0:
             # Use provided firmware image 
             image_file = module_argv[0]
             self.logger.log( "[*] reading FW image from file: {}".format(image_file) )
 
-        self.image = chipsec.file.read_file( image_file )
+        self.image = read_file( image_file )
 
         # Load JSON config with black-listed EFI modules
         if len(module_argv) > 1: self.cfg_name = module_argv[1]
-        cfg_pth = os.path.join( os.path.dirname(os.path.realpath(__file__)), self.cfg_name )
+        cfg_pth = os.path.join( get_main_dir(), "chipsec/modules/tools/uefi", self.cfg_name )
         with open(cfg_pth, 'r') as blacklist_json:
              self.efi_blacklist = json.load( blacklist_json )
 
         return self.check_blacklist()
```

### Comparing `chipsec-1.4.4/chipsec/modules/tools/uefi/uefivar_fuzz.py` & `chipsec-1.5.1/chipsec/modules/tools/uefi/uefivar_fuzz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -75,18 +75,17 @@
 '''
 
 import random
 from time import time
 from uuid import uuid4, UUID
 import struct
 
-from chipsec.module_common import *
-from chipsec.file          import *
-from chipsec.hal.uefi      import *
-import chipsec.chipset
+from chipsec.module_common import BaseModule, ModuleResult, cs_input
+from chipsec.file import write_file
+from chipsec.hal.uefi import UEFI
 
 from chipsec.fuzzing import primitives as prim
 
 class uefivar_fuzz(BaseModule):
 
     def __init__(self):
         BaseModule.__init__(self)
```

### Comparing `chipsec-1.4.4/chipsec/modules/tools/uefi/whitelist.py` & `chipsec-1.5.1/chipsec/modules/tools/uefi/whitelist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # CHIPSEC: Platform Security Assessment Framework
-# Copyright (c) 2017, Intel Security
+# Copyright (c) 2017-2020, Intel Security
 #
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; Version 2.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -160,15 +160,15 @@
 
         for m in self.efi_list:
             if not (m in self.efi_whitelist):
                 self.suspect_modules[m] = self.efi_list[m]
                 guid = self.efi_list[m]["guid"] if 'guid' in self.efi_list[m] else '?'
                 name = self.efi_list[m]["name"] if 'name' in self.efi_list[m] else '<unknown>'
                 sha1 = self.efi_list[m]["sha1"] if 'sha1' in self.efi_list[m] else ''
-                self.logger.log_important( "found EFI executable not in the list:\n    {} (sha256)\n    {} (sha1)\n    {{}}\n    {}".format(m,sha1,guid,name))
+                self.logger.log_important( "found EFI executable not in the list:\n    {} (sha256)\n    {} (sha1)\n    {{{}}}\n    {}".format(m,sha1,guid,name))
 
         if len(self.suspect_modules) > 0:
             self.logger.log_warn_check( "found {:d} EFI executables not in the list '{}'".format(len(self.suspect_modules),json_pth) )
             return ModuleResult.WARNING
         else:
             self.logger.log_passed_check( "all EFI executables match the list '{}'".format(json_pth) )
             return ModuleResult.PASSED
```

### Comparing `chipsec-1.4.4/chipsec/modules/tools/uefi/__init__.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/cpu/sinkhole.py` & `chipsec-1.5.1/chipsec/modules/tools/cpu/sinkhole.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -24,15 +24,15 @@
 NOTE: The system may hang when running this test. In that case, the mitigation to this issue is likely working but we may not be handling the exception generated.
 
 References:
 
 The Memory Sinkhole by Christopher Domas: https://www.blackhat.com/docs/us-15/materials/us-15-Domas-The-Memory-Sinkhole-Unleashing-An-x86-Design-Flaw-Allowing-Universal-Privilege-Escalation.pdf (presentation) and https://www.blackhat.com/docs/us-15/materials/us-15-Domas-The-Memory-Sinkhole-Unleashing-An-x86-Design-Flaw-Allowing-Universal-Privilege-Escalation-wp.pdf (whitepaper).
 """
 
-from chipsec.module_common import *
+from chipsec.module_common import BaseModule, ModuleResult, MTAG_SMM
 from chipsec.hal import cpu
 import chipsec.helper.oshelper
 
 TAGS = [MTAG_SMM]
 
 class sinkhole(BaseModule):
```

### Comparing `chipsec-1.4.4/chipsec/modules/tools/cpu/__init__.py` & `chipsec-1.5.1/chipsec/modules/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/smm/rogue_mmio_bar.py` & `chipsec-1.5.1/chipsec/modules/tools/smm/rogue_mmio_bar.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # CHIPSEC: Platform Security Assessment Framework
-# Copyright (c) 2017-2018, Intel Security
+# Copyright (c) 2017-2020, Intel Security
 #
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; Version 2.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -19,29 +19,28 @@
 """
 Experimental module that may help checking SMM firmware for MMIO BAR hijacking
 vulnerabilities described in the following presentation:
 
 `BARing the System: New vulnerabilities in Coreboot & UEFI based systems <http://www.intelsecurity.com/advanced-threat-research/content/data/REConBrussels2017_BARing_the_system.pdf>`_ by Intel Advanced Threat Research team at RECon Brussels 2017
 
 Usage:
-  ``chipsec_main -m tools.smm.rogue_mmio_bar [-a <smi_start:smi_end>,<b:d.f>]`` 
-  
+  ``chipsec_main -m tools.smm.rogue_mmio_bar [-a <smi_start:smi_end>,<b:d.f>]``
+
 - ``smi_start:smi_end``: range of SMI codes (written to IO port 0xB2)
 - ``b:d.f``: PCIe bus/device/function in b:d.f format (in hex)
 
 Example:
     >>> chipsec_main.py -m tools.smm.rogue_mmio_bar -a 0x00:0x80
     >>> chipsec_main.py -m tools.smm.rogue_mmio_bar -a 0x00:0xFF,0:1C.0
 """
 
-from chipsec.module_common import *
-
-from chipsec import defines
-from chipsec import file
-from chipsec.hal import pci
+from chipsec.module_common import BaseModule, ModuleResult
+from chipsec.defines import BOUNDARY_4GB
+from chipsec.file import write_file
+from chipsec.hal.pci import PCI_HDR_BAR_STEP, PCI_HDR_BAR_BASE_MASK_MMIO64, PCI_HDR_BAR_CFGBITS_MASK
 from chipsec.hal.interrupts import Interrupts
 
 #################################################################
 # Testing configuration
 #################################################################
 
 FLUSH_OUTPUT_AFTER_SMI = False
@@ -73,25 +72,24 @@
         # SMI handler "function" often supplied in ECX register
         self.smif_start   = 0x00
         self.smif_end     = SMI_FUNC_LIMIT
         # SMM communication buffer often supplied in EBX register
         self.comm         = 0x00
 
         self.reloc_mmio   = None
-       
 
     def smi_mmio_range_fuzz(self, thread_id, b, d, f, bar_off, is64bit, bar, new_bar, base, size):
 
         # copy all registers from MMIO range to new location in memory
         # we do that once rather than before every SMI since we return after first change detected
         self.logger.log( "[*] copying BAR 0x{:X} > 0x{:X}".format(base,self.reloc_mmio) )
         orig_mmio = self.copy_bar(base, self.reloc_mmio, size)
         if self.logger.VERBOSE:
             self.cs.mmio.dump_MMIO(base, size)
-            file.write_file('mmio_mem.orig', orig_mmio)
+            write_file('mmio_mem.orig', orig_mmio)
 
         for smi_code in range(self.smic_start,self.smic_end+1):
             for smi_data in range(self.smid_start,self.smid_end+1):
                 for ecx in range(self.smif_start,self.smif_end+1):
                     self.logger.log( "> SMI# {:02X}: data {:02X}, func (ECX) {:X}".format(smi_code,smi_data,ecx) )
                     if FLUSH_OUTPUT_AFTER_SMI: self.logger.flush()
 
@@ -108,15 +106,15 @@
 
                     # check the contents at the address range used to relocate MMIO BAR
                     buf = self.cs.mem.read_physical_mem( self.reloc_mmio, size )
                     diff = DIFF(orig_mmio, buf, size)
                     self.logger.log("  checking relocated MMIO")
                     if len(diff) > 0:
                         self.logger.log_important("changes found at 0x{:X} +{}".format(self.reloc_mmio, diff))
-                        if self.logger.VERBOSE: file.write_file('mmio_mem.new', buf)
+                        if self.logger.VERBOSE: write_file('mmio_mem.new', buf)
                         return True
         return False
 
 
     def copy_bar(self, bar_base, bar_base_mem, size):
         for off in range(0,size,4):
             r = self.cs.mem.read_physical_mem_dword(bar_base + off)
@@ -132,31 +130,29 @@
             off += 4
         return self.cs.mem.read_physical_mem(bar_base_mem, size)
     """
 
     def modify_bar(self, b, d, f, off, is64bit, bar, new_bar):
         # Modify MMIO BAR address
         if is64bit:
-            #self.cs.pci.write_dword(b, d, f, off, 0x0)
-            self.cs.pci.write_dword(b, d, f, off + pci.PCI_HDR_BAR_STEP, ((new_bar>>32)&0xFFFFFFFF))
+            self.cs.pci.write_dword(b, d, f, off + PCI_HDR_BAR_STEP, ((new_bar>>32)&0xFFFFFFFF))
         self.cs.pci.write_dword(b, d, f, off, (new_bar&0xFFFFFFFF))
         # Check that the MMIO BAR has been modified correctly. Restore original and skip if not
         l = self.cs.pci.read_dword(b, d, f, off)
         if l != (new_bar&0xFFFFFFFF):
             self.restore_bar(b, d, f, off, is64bit, bar)
             self.logger.log("  skipping ({:X} != {:X})".format(l,new_bar))
             return False
         self.logger.log("  new BAR: 0x{:X}".format(l))
         return True
 
     def restore_bar(self, b, d, f, off, is64bit, bar):
         if is64bit:
-            #self.cs.pci.write_dword(b, d, f, off, 0x0)
-            self.cs.pci.write_dword(b, d, f, off + pci.PCI_HDR_BAR_STEP, ((bar>>32)&0xFFFFFFFF))
-        self.cs.pci.write_dword(b, d, f, off, (bar&0xFFFFFFFF))                        
+            self.cs.pci.write_dword(b, d, f, off + PCI_HDR_BAR_STEP, ((bar>>32)&0xFFFFFFFF))
+        self.cs.pci.write_dword(b, d, f, off, (bar&0xFFFFFFFF))
         return True
 
     def run( self, module_argv ):
         self.logger.start_test( "experimental tool to help checking for SMM MMIO BAR issues" )
 
         pcie_devices = []
 
@@ -176,32 +172,32 @@
             self.logger.log("[*] discovering PCIe devices..")
             pcie_devices = self.cs.pci.enumerate_devices()
 
         self.logger.log("[*] testing MMIO of PCIe devices:")
         for (b,d,f,_,_) in pcie_devices: self.logger.log("    {:02X}:{:02X}.{:X}".format(b,d,f))
 
         # allocate a page or SMM communication buffer (often supplied in EBX register)
-        _, self.comm = self.cs.mem.alloc_physical_mem(0x1000, defines.BOUNDARY_4GB-1)
+        _, self.comm = self.cs.mem.alloc_physical_mem(0x1000, BOUNDARY_4GB-1)
         #self.cs.mem.write_physical_mem( self.comm, 0x1000, chr(0)*0x1000 )
 
         # allocate range in physical memory (should cover all MMIO ranges including GTTMMADR)
         bsz = 2*MAX_MMIO_RANGE_SIZE
-        (va, pa) = self.cs.mem.alloc_physical_mem( bsz, defines.BOUNDARY_4GB-1 )
+        (va, pa) = self.cs.mem.alloc_physical_mem( bsz, BOUNDARY_4GB-1 )
         self.logger.log( "[*] allocated memory range : 0x{:016X} (0x{:X} bytes)".format(pa,bsz) )
         self.cs.mem.write_physical_mem(pa, bsz, _MEM_FILL_VALUE*bsz)
         # align at the MAX_MMIO_RANGE_SIZE boundary within allocated range
         self.reloc_mmio = pa & (~(MAX_MMIO_RANGE_SIZE-1))
         if self.reloc_mmio < pa: self.reloc_mmio += MAX_MMIO_RANGE_SIZE
         self.logger.log("[*] MMIO relocation address: 0x{:016X}\n".format(self.reloc_mmio))
-        
+
         for (b, d, f, vid, did) in pcie_devices:
             self.logger.log("[*] enumerating device {:02X}:{:02X}.{:X} MMIO BARs..".format(b, d, f))
             device_bars = self.cs.pci.get_device_bars(b, d, f, True)
             for (base, isMMIO, is64bit, bar_off, bar, size) in device_bars:
                 if isMMIO and size <= MAX_MMIO_RANGE_SIZE:
                     self.logger.flush()
                     self.logger.log( "[*] found MMIO BAR +0x{:02X} (base 0x{:016X}, size 0x{:X})".format(bar_off,base,size) )
-                    new_bar = ((self.reloc_mmio & pci.PCI_HDR_BAR_BASE_MASK_MMIO64)|(bar & pci.PCI_HDR_BAR_CFGBITS_MASK))
+                    new_bar = ((self.reloc_mmio & PCI_HDR_BAR_BASE_MASK_MMIO64)|(bar & PCI_HDR_BAR_CFGBITS_MASK))
                     if self.smi_mmio_range_fuzz(0, b, d, f, bar_off, is64bit, bar, new_bar, base, size):
                         return ModuleResult.FAILED
 
         return ModuleResult.PASSED
```

### Comparing `chipsec-1.4.4/chipsec/modules/tools/smm/smm_ptr.py` & `chipsec-1.5.1/chipsec/modules/tools/smm/smm_ptr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -63,17 +63,20 @@
 - ``[]``: optional line
 - ``*``: Don't Care (the module will replace * with 0x0)
 - ``PTR``: Physical address SMI handler will write to (the module will replace PTR with physical address provided as a command-line argument)
 - ``VAL``: Value SMI handler will write to PTR address (the module will replace VAL with hardcoded _FILL_VALUE_xx)
 
 """
 
-from chipsec.module_common import *
-from chipsec.file import *
+import struct
+import os
 
+from chipsec.module_common import BaseModule, ModuleResult
+from chipsec.file import write_file
+from chipsec.logger import print_buffer
 from chipsec.hal.interrupts import Interrupts
 
 #logger.VERBOSE = False
 
 #################################################################
 # Fuzzing configuration
 #################################################################
@@ -193,15 +196,15 @@
         if is_ptr_in_buffer: s += " -> PTR at +0x{:X}".format(_ptr_offset)
         if _sig is not None: s += " -> SIG at +0x{:X}".format(_sig_offset)
         self.logger.log( s )
         self.cs.mem.write_physical_mem( _addr, self.fill_size, fill_buf )
 
         if self.logger.VERBOSE:
              self.logger.log( "filling in contents at PA 0x{:016X}:".format(_addr) )
-             chipsec.logger.print_buffer( fill_buf )
+             print_buffer( fill_buf )
 
         if is_ptr_in_buffer and _ptr is not None: 
             self.logger.log( "[*] writing buffer at PA 0x{:016X} with 0x{:X} bytes '{}'".format(_ptr, self.fill_size, self.fill_byte) )
             self.cs.mem.write_physical_mem( _ptr, self.fill_size, self.fill_byte*self.fill_size )
 
         return True
 
@@ -224,17 +227,17 @@
         expected_buf = FILL_BUFFER( self.fill_byte, self.fill_size, _smi_desc.ptr_in_buffer, _smi_desc.ptr, _smi_desc.ptr_offset, _smi_desc.sig, _smi_desc.sig_offset )
         buf          = self.cs.mem.read_physical_mem( _addr, self.fill_size )
         differences  = DIFF( expected_buf, buf, self.fill_size )
         _changed     = (len(differences) > 0)
 
         if self.logger.VERBOSE:
              self.logger.log( "checking contents at PA 0x{:016X}:".format(_addr) )
-             chipsec.logger.print_buffer( buf )
+             print_buffer( buf )
              self.logger.log( "expected contents:" )
-             chipsec.logger.print_buffer( expected_buf )
+             print_buffer( expected_buf )
 
         if _changed:
             self.logger.log( "    contents changed at 0x{:016X} +{}".format(_addr,differences) )
             if restore_contents:
                 self.logger.log( "    restoring 0x{:X} bytes at 0x{:016X}".format(self.fill_size, _addr) )
                 self.cs.mem.write_physical_mem( _addr, self.fill_size, expected_buf )
             if DUMP_MEMORY_ON_DETECT:
@@ -249,15 +252,15 @@
         if _smi_desc.ptr_in_buffer and _ptr is not None:
             buf1         = self.cs.mem.read_physical_mem( _ptr, self.fill_size )
             differences1 = DIFF( expected_buf, buf1, self.fill_size )
             _changed1    = (len(differences1) > 0)
 
             if self.logger.VERBOSE:
                 self.logger.log( "checking contents at PA 0x{:016X}:".format(_ptr) )
-                chipsec.logger.print_buffer( buf1 )
+                print_buffer( buf1 )
 
             if _changed1:
                 self.logger.log( "    contents changed at 0x{:016X} +{}".format(_ptr,differences1) )
                 if restore_contents:
                     self.logger.log( "    restoring 0x{:X} bytes at PA 0x{:016X}".format(self.fill_size, _ptr) )
                     self.cs.mem.write_physical_mem( _ptr, self.fill_size, expected_buf )
                 if DUMP_MEMORY_ON_DETECT:
```

### Comparing `chipsec-1.4.4/chipsec/modules/tools/smm/__init__.py` & `chipsec-1.5.1/chipsec/modules/tools/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/msr_fuzz.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/msr_fuzz.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2015, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -25,22 +25,21 @@
 
  Usage:
    ``chipsec_main.py -i -m tools.vmm.msr_fuzz [-a random] -l log.txt``
 """
 
 import random
 
-from chipsec.module_common import *
+from chipsec.module_common import BaseModule
 
 #logger.VERBOSE = True
 
 _MODULE_NAME = 'msr_fuzz'
 
 # Number of iterations to fuzz randomly
-global _NO_ITERATIONS_TO_FUZZ
 _NO_ITERATIONS_TO_FUZZ = 100000
 
 # Read MSR?
 _READ_MSR = False
 
 # Flush log file before each MSR
 _FLUSH_LOG_EACH_MSR = False
@@ -65,18 +64,18 @@
         else:            it_max = msr_addr_range
         while it < it_max:
             if random_order: msr_addr = random.randint( msr_addr_start, msr_addr_end )
             else:            msr_addr = msr_addr_start + it
             if _FLUSH_LOG_EACH_MSR: self.logger.flush()
             if msr_addr not in _EXCLUDE_MSR:
                 if _READ_MSR:
-                    self.logger.log( "[*] rdmsr 0x{:08X}".formatmsr_addr )
+                    self.logger.log( "[*] rdmsr 0x{:08X}".format(msr_addr) )
                     try: (eax, edx) = self.cs.msr.read_msr( 0, msr_addr )
                     except: pass
-                self.logger.log( "[*] wrmsr 0x{:08X}".formatmsr_addr )
+                self.logger.log( "[*] wrmsr 0x{:08X}".format(msr_addr) )
                 if _FUZZ_VALUE_0_all1s:
                     #self.logger.log( "    0" )
                     try: self.cs.msr.write_msr( 0, msr_addr, 0, 0 )
                     except: pass
                     #self.logger.log( "    0xFFFFFFFFFFFFFFFF" )
                     try: self.cs.msr.write_msr( 0, msr_addr, 0xFFFFFFFF, 0xFFFFFFFF )
                     except: pass
```

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/hypercallfuzz.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/hypercallfuzz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2016, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -32,16 +32,16 @@
     - ``vector_reg``		hypercall vector register
     - ``maxval``		maximum value of each register
     - ``iterations``		number of iterations in random mode
 """
 import random
 import time
 
-from chipsec.module_common import *
-import chipsec.hal.vmm
+from chipsec.module_common import BaseModule, ModuleResult
+from chipsec.hal.vmm import VMM
 
 DEFAULT_VECTOR_MAXVAL     = 0xFF
 
 DEFAULT_MAXVAL_EXHAUSTIVE = 0xFF
 DEFAULT_MAXVAL_RANDOM     = 0xFFFFFFFF
 
 DEFAULT_RANDOM_ITERATIONS = 0x7FFFFFFF
@@ -52,15 +52,15 @@
 
 GPRS = { 'rax': 0, 'rbx': 0, 'rcx': 0, 'rdx': 0, 'rdi': 0, 'rsi': 0, 'r8' : 0, 'r9' : 0, 'r10': 0, 'r11': 0 }
 
 class hypercallfuzz(BaseModule):
 
     def __init__(self):
         BaseModule.__init__(self)
-        self.vmm = chipsec.hal.vmm.VMM( self.cs )
+        self.vmm = VMM( self.cs )
 
         self.random_order = True
         self.gprs         = GPRS
         self.vector_reg   = None
         self.iterations   = DEFAULT_RANDOM_ITERATIONS
         self.maxval       = DEFAULT_MAXVAL_RANDOM
 
@@ -149,8 +149,8 @@
         self.logger.log( "\n[*] Configuration:" )
         self.logger.log( "    Mode               : {}".format('random' if self.random_order else 'exhaustive') )
         self.logger.log( "    Hypercall vector in: {}".format(self.vector_reg) )
         self.logger.log( "    Max register value : 0x{:X}".format(self.maxval) )
         self.logger.log( "    Iterations         : {:d}\n".format(self.iterations) )
 
         return self.fuzz_generic_hypercalls()
-        
+
```

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/vbox/vbox_crash_apicbase.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/vbox/vbox_crash_apicbase.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/vbox/__init__.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/hv/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/xen/define.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/xen/define.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/xen/hypercallfuzz.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/xen/hypercallfuzz.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/xen/xsa188.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/xen/xsa188.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/xen/__init__.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/vbox/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/xen/hypercall.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/xen/hypercall.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/iofuzz.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/iofuzz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2015, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -24,15 +24,15 @@
 Simple port I/O VMM emulation fuzzer
 
  Usage:
    ``chipsec_main.py -i -m tools.vmm.iofuzz [-a <mode>,<count>,<iterations>] -l log.txt``
 """
 import random
 
-from chipsec.module_common import *
+from chipsec.module_common import BaseModule, ModuleResult
 
 MAX_PORTS = 0x10000
 MAX_PORT_VALUE = 0xFF
 DEFAULT_PORT_WRITE_COUNT  = 1000
 DEFAULT_RANDOM_ITERATIONS = 1000000
 
 #_READ_PORT = True
@@ -89,15 +89,14 @@
                 except: pass
 
             self.logger.log( "    writing values 0..{:X} ({:d} times each)".format(MAX_PORT_VALUE,write_count) )
             for v in range(MAX_PORT_VALUE+1):
                 for n in range(write_count):
                     try: self.cs.io.write_port_byte( io_addr, v )
                     except: pass
-                    pass
 
         return ModuleResult.PASSED
 
     def run( self, module_argv ):
 
         self.logger.start_test( "I/O port fuzzer" )
         self.logger.log( "Usage: chipsec_main -m tools.vmm.iofuzz [ -a <mode>,<count>,<iterations> ]" )
```

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/common.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -28,16 +28,16 @@
 import random
 import os.path
 import json
 import pprint
 import binascii
 from random                     import getrandbits, randint
 from time                       import strftime, localtime
-from chipsec.module_common      import *
-from chipsec.defines            import *
+from chipsec.module_common      import BaseModule
+from chipsec.defines            import DD
 
 class BaseModuleDebug(BaseModule):
     def __init__(self):
         BaseModule.__init__(self)
         self.debug = False
         self.promt = ''
 
@@ -108,14 +108,15 @@
     def __init__(self):
         BaseModuleDebug.__init__(self)
         self.initial_data        = []
         self.path = os.path.dirname(os.path.realpath(__file__))
         with open(os.path.join(self.path, 'hv', 'initial_data.json'), "r") as json_file:
             self.initial_data = json.load(json_file)
         self.statistics = {}
+        self.hv_connectionid     = {}
 
     def __del__(self):
         #self.dump_initial_data("initial_data_auto_generated.json")
         BaseModuleDebug.__del__(self)
 
     def stats_reset(self):
         self.statistics = {}
@@ -130,16 +131,16 @@
         self.msg((' {} '.format(title).center(72 - len(self.promt), '*')))
         for name in sorted(self.statistics, key=self.statistics.get, reverse=True):
             self.msg('{:50} : {:d}'.format(name, self.statistics[name]) )
         self.msg('')
         return
 
     def get_initial_data(self, statuses, vector, size, padding = '\x00'):
-        connectionid_message = [(' '.join(["{:02x}".format(ord(x)) for x in DD(k)])) for k,v in self.hv_connectionid.iteritems() if v == 1]
-        connectionid_event   = [(' '.join(["{:02x}".format(ord(x)) for x in DD(k)])) for k,v in self.hv_connectionid.iteritems() if v == 2]
+        connectionid_message = [(' '.join(["{:02x}".format(ord(x)) for x in DD(k)])) for k,v in self.hv_connectionid.items() if v == 1]
+        connectionid_event   = [(' '.join(["{:02x}".format(ord(x)) for x in DD(k)])) for k,v in self.hv_connectionid.items() if v == 2]
         result = []
         for status in statuses:
             for item in self.initial_data:
                 if (int(item['vector'], 16) == vector) and (item['status'] == status):
                     data = item['data']
                     data = data.replace('CONNECTION_ID_MESSAGE_TYPE', random.choice(connectionid_message))
                     data = data.replace('CONNECTION_ID_EVENT_TYPE',   random.choice(connectionid_event))
@@ -248,15 +249,15 @@
        exit(1)
     return arg
 
 def hv_hciv(rep_start, rep_count, call_code, fast = 0):
     return (((rep_start & 0x0FFF) << 48) + ((rep_count & 0x0FFF) << 32) + ((fast & 0x1) << 16) + (call_code & 0xFFFF))
 
 def uuid(id):
-    return '{{:08X}-{:04X}-{:04X}-{:02X}{:02X}-{:02X}{:02X}{:02X}{:02X}{:02X}{:02X}}'.format(struct.unpack('<LHH8B', *id))
+    return '{{{:08X}-{:04X}-{:04X}-{:02X}{:02X}-{:02X}{:02X}{:02X}{:02X}{:02X}{:02X}}}'.format(*struct.unpack('<IHH8B', id))
 
 ### OPTIONAL ROUTINES ##########################################################
 
 class session_logger(object):
     def __init__(self, log, details):
         self.defstdout = sys.stdout
         self.log       = log
```

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/cpuid_fuzz.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/cpuid_fuzz.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -25,27 +25,30 @@
 
  Usage:
    ``chipsec_main.py -i -m tools.vmm.cpuid_fuzz -l log.txt``
 """
 
 import random
 
-from chipsec.module_common import *
+from chipsec.module_common import BaseModule, ModuleResult
 
 #logger.VERBOSE = True
 
 _MODULE_NAME = 'cpuid_fuzz'
 
 #
 # We will only be fuzzing _NO_EAX_TO_FUZZ range of EAX values each _EAX_FUZZ_STEP step
 #
 #global _EAX_FUZZ_STEP
 _NO_EAX_TO_FUZZ       = 0x100
 _EAX_FUZZ_STEP        = 0x1000000
 
+# Number of iterations if value is Randomly chosen
+_NO_ITERATIONS_TO_FUZZ = 0x1000000
+
 # Control values to be passed in ECX
 _FUZZ_ECX_RANDOM      = False
 # Max value of ECX when fuzzed sequentially
 _MAX_ECX              = 0x100
 
 # Exclude CPUID EAX which cause VM hang/crash
 _EXCLUDE_CPUID        = [ ]
```

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/venom.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/venom.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2015, Intel Corporation
-# 
+#Copyright (c) 2010-2020, Intel Corporation
+#
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
 #MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -24,15 +24,15 @@
 QEMU VENOM vulnerability DoS PoC test
 Module is based on PoC by Marcus Meissner (https://marc.info/?l=oss-security&m=143155206320935&w=2)
 
  Usage:
    ``chipsec_main.py -i -m tools.vmm.venom``
 """
 
-from chipsec.module_common import *
+from chipsec.module_common import BaseModule
 
 _MODULE_NAME = 'venom'
 
 FDC_PORT_DATA_FIFO = 0x3F5
 ITER_COUNT         = 0x10000000
 FDC_CMD_WRVAL      = 0x42
 FD_CMD             = 0x8E # FD_CMD_DRIVE_SPECIFICATION_COMMAND # FD_CMD_READ_ID = 0x0A
```

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/pcie_fuzz.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/pcie_fuzz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -23,20 +23,22 @@
 """
 Simple PCIe device Memory-Mapped I/O (MMIO) and I/O ranges VMM emulation fuzzer
 
  Usage:
    ``chipsec_main.py -i -m tools.vmm.pcie_fuzz -l log.txt``
 """
 
-from chipsec.module_common import *
-from chipsec.hal import pci
-
 import time
 import random
 
+from chipsec.module_common import BaseModule, ModuleResult
+from chipsec.hal.pci import print_pci_devices
+
+
+
 #################################################################
 # Fuzzing configuration
 #################################################################
 #
 IO_FUZZ        = 0
 CALC_BAR_SIZE  = 1
 TIMEOUT        = 1
@@ -131,15 +133,15 @@
 
     def find_active_range(self, bar, size):
         self.logger.log( "[*] Determine MMIO BAR Active range 0x{:016X}, size  0x{:X}..".format(bar,size) )
         one = self.cs.mem.read_physical_mem(bar, size)
         time.sleep(TIMEOUT)
         two = self.cs.mem.read_physical_mem(bar, size)
         diff_index = []
-        for i in range(len(one)/4 - 1):
+        for i in range(len(one)//4 - 1):
             if one[4*i] != two[4*i] or one[4*i+1] != two[4*i+1] or one[4*i+2] != two[4*i+2] or one[4*i+3] != two[4*i+3]:
                 diff_index.append(i*4)
         return diff_index
 
     def fuzz_pcie_device(self, b, d, f):
         self.logger.log( "[*] Discovering MMIO and I/O BARs of the device.." )
         device_bars = self.cs.pci.get_device_bars( b, d, f, bCalcSize=CALC_BAR_SIZE )
@@ -175,13 +177,13 @@
             _fun = int(module_argv[2],16)
             pcie_devices.append( (_bus, _dev, _fun, 0, 0) )
         else:
             self.logger.log( "[*] Enumerating available PCIe devices.." )
             pcie_devices = self.cs.pci.enumerate_devices()
 
         self.logger.log( "[*] About to fuzz the following PCIe devices.." )
-        pci.print_pci_devices( pcie_devices )
+        print_pci_devices( pcie_devices )
         for (b, d, f, vid, did) in pcie_devices:
             self.logger.log( "[+] Fuzzing device {:02X}:{:02X}.{:X}".format(b, d, f) )
             self.fuzz_pcie_device( b, d, f )
 
         return ModuleResult.PASSED
```

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/__init__.py` & `chipsec-1.5.1/chipsec/utilcmd/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/hv/vmbusfuzz.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/hv/vmbusfuzz.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/hv/define.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/hv/define.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/hv/hypercallfuzz.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/hv/hypercallfuzz.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/hv/synth_kbd.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/hv/synth_kbd.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/hv/vmbus.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/hv/vmbus.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/hv/synth_dev.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/hv/synth_dev.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/hv/initial_data.json` & `chipsec-1.5.1/chipsec/modules/tools/vmm/hv/initial_data.json`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/hv/__init__.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/xen/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/hv/hypercall.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/hv/hypercall.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/vmm/pcie_overlap_fuzz.py` & `chipsec-1.5.1/chipsec/modules/tools/vmm/pcie_overlap_fuzz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -24,20 +24,20 @@
 PCIe device Memory-Mapped I/O (MMIO) ranges VMM emulation fuzzer which first overlaps MMIO BARs of all available PCIe devices
 then fuzzes them by writing garbage if corresponding option is enabled
 
  Usage:
    ``chipsec_main.py -i -m tools.vmm.pcie_overlap_fuzz -l log.txt``
 """
 
-from chipsec.module_common import *
-from chipsec.hal import pci
-
 import time
 import random
 
+from chipsec.module_common import BaseModule, ModuleResult
+from chipsec.hal.pci import print_pci_devices
+
 #################################################################
 # Fuzzing configuration
 #################################################################
 #
 OVERLAP_MODE = 1
 FUZZ_OVERLAP = 0
 FUZZ_RANDOM = 0
@@ -139,12 +139,12 @@
         self.logger.start_test( "Tool to overlap and fuzz MMIO spaces of available PCIe devices" )
 
         pcie_devices = []
         self.logger.log( "[*] Enumerating available PCIe devices.." )
         pcie_devices = self.cs.pci.enumerate_devices()
 
         self.logger.log( "[*] About to fuzz the following PCIe devices.." )
-        pci.print_pci_devices( pcie_devices )
+        print_pci_devices( pcie_devices )
         self.fuzz_overlap_pcie_device( pcie_devices )
 
         return ModuleResult.PASSED
```

### Comparing `chipsec-1.4.4/chipsec/modules/tools/__init__.py` & `chipsec-1.5.1/chipsec/modules/tools/secureboot/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/modules/tools/secureboot/te.py` & `chipsec-1.5.1/chipsec/modules/tools/secureboot/te.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,20 +24,20 @@
 Tool to test for 'TE Header' vulnerability in Secure Boot implementations as described in 
 `All Your Boot Are Belong To Us <https://cansecwest.com/slides/2014/AllYourBoot_csw14-intel-final.pdf>`_
 
 Usage:
   ``chipsec_main.py -m tools.secureboot.te [-a <mode>,<cfg_file>,<efi_file>]``
       - ``<mode>``
 
-          * ``generate_te``		(default) convert PE EFI binary ``<efi_file>`` to TE binary
-          * ``replace_bootloader``	replace bootloader files listed in ``<cfg_file>`` on ESP with modified ``<efi_file>``
-          * ``restore_bootloader``	restore original bootloader files from ``.bak`` files
+          * ``generate_te``     (default) convert PE EFI binary ``<efi_file>`` to TE binary
+          * ``replace_bootloader``  replace bootloader files listed in ``<cfg_file>`` on ESP with modified ``<efi_file>``
+          * ``restore_bootloader``  restore original bootloader files from ``.bak`` files
 
-      - ``<cfg_file>``	path to config file listing paths to bootloader files to replace
-      - ``<efi_file>``	path to EFI binary to convert to TE binary. If no file path is provided, the tool will look for Shell.efi
+      - ``<cfg_file>``  path to config file listing paths to bootloader files to replace
+      - ``<efi_file>``  path to EFI binary to convert to TE binary. If no file path is provided, the tool will look for Shell.efi
 
 Examples:
 
 Convert Shell.efi PE/COFF EFI executable to TE executable:
 
   ``chipsec_main.py -m tools.secureboot.te -a generate_te,Shell.efi``
 
@@ -404,18 +404,23 @@
             bootloader_paths.append( bl_path )
     return bootloader_paths
 
 def replace_bootloader( bootloader_paths, new_bootloader_file, do_mount=True ):
     logger().log( "[*] Replacing bootloaders on EFI System Partition (ESP).." )
     dsk = get_efi_mount() if do_mount else ''
     if dsk is None: return False
-    for pth in bootloader_paths:
-        bootloader_path = os.path.join(dsk,pth)
-        if os.path.exists(bootloader_path): replace_efi_binary( bootloader_path, new_bootloader_file )
-    if do_mount: umount( dsk )
+    try:
+        for pth in bootloader_paths:
+            bootloader_path = os.path.join(dsk,pth)
+            if os.path.exists(bootloader_path):
+                replace_efi_binary( bootloader_path, new_bootloader_file )
+            else:
+                logger().warn( "Bootloader {} does not exist on ESP".format(bootloader_path) )
+    finally:
+        if do_mount: umount( dsk )
     logger().log( "[*] You will need to reboot the system to see the changes" )
     return True
 
 def restore_efi_binary( orig_efi_binary ):
     logger().log( "[*] Restoring {}..".format(orig_efi_binary) )
     backup = orig_efi_binary + ".bak"
     if not os.path.exists(backup):
```

### Comparing `chipsec-1.4.4/chipsec/modules/tools/secureboot/__init__.py` & `chipsec-1.5.1/chipsec/modules/tools/smm/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/__init__.py` & `chipsec-1.5.1/chipsec/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/WARNING.txt` & `chipsec-1.5.1/drivers/linux/WARNING.txt`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec/file.py` & `chipsec-1.5.1/chipsec/file.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/setup.py` & `chipsec-1.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -224,15 +224,15 @@
 https://github.com/chipsec/chipsec/blob/master/chipsec-manual.pdf
 """)
 
 package_data = {
     # Include any configuration file.
     "": ["*.ini", "*.cfg", "*.json"],
     "chipsec": ["*VERSION", "WARNING.txt"],
-    "chipsec.cfg": ["*.xml", "*.xsd"],
+    "chipsec.cfg":  ["8086/*.xml","*.xml","*.xsd"],
 }
 data_files = [("", ["chipsec-manual.pdf"])]
 install_requires = []
 extra_kw = []
 
 if platform.system().lower() == "windows":
     package_data["chipsec.helper.win"] = ['win7_amd64/*.sys']
@@ -266,17 +266,14 @@
         'Natural Language :: English',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX :: Linux',
         'Operating System :: MacOS :: MacOS X',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.6',
         'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Topic :: Security',
         'Topic :: System :: Hardware'
     ],
 
     data_files = data_files,
     packages = find_packages(exclude=["tests.*", "tests"]),
     package_data = package_data,
```

### Comparing `chipsec-1.4.4/chipsec-manual.pdf` & `chipsec-1.5.1/chipsec-manual.pdf`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec_tools/windows/__init__.py` & `chipsec-1.5.1/chipsec_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec_tools/__init__.py` & `chipsec-1.5.1/chipsec_tools/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `chipsec-1.4.4/chipsec_main.py` & `chipsec-1.5.1/chipsec_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -77,39 +77,42 @@
   pass
 
 class ChipsecMain:
 
     def __init__(self, argv):
         self.CHIPSEC_FOLDER        = os.path.abspath(chipsec.file.get_main_dir())
         self.CHIPSEC_LOADED_AS_EXE = chipsec.file.main_is_frozen()
+        self.PYTHON_64_BITS        = True if (sys.maxsize > 2**32) else False
         self.ZIP_MODULES_RE        = None
         self.Import_Path           = "chipsec.modules."
         self.Modules_Path          = os.path.join(self.CHIPSEC_FOLDER,"chipsec","modules")
         self.Loaded_Modules        = []
         self.AVAILABLE_TAGS        = []
         self.MODPATH_RE            = re.compile(r"^\w+(\.\w+)*$")
         self.version               = defines.get_version()
+        self.message               = defines.get_message()
 
         self.argv = argv
         self.parse_args()
-        
+
     def init_cs(self):
         self._cs = chipset.cs()
 
     def print_banner(self):
         """
         Prints chipsec banner
         """
         logger().log( "################################################################\n"
                       "##                                                            ##\n"
                       "##  CHIPSEC: Platform Hardware Security Assessment Framework  ##\n"
                       "##                                                            ##\n"
                       "################################################################" )
         logger().log( "[CHIPSEC] Version {}".format(self.version) )
         logger().log( "[CHIPSEC] Arguments: {}".format( " ".join(self.argv) ) )
+        logger().log( self.message )
 
     ##################################################################################
     # Module API
     ##################################################################################
     def f_mod(self,x):
         return ( x.find('__init__') == -1 and ZIP_MODULES_RE.match(x) )
 
@@ -198,41 +201,42 @@
     #
     def load_module( self, module_path, module_argv ):
         module_name =  self.get_module_name(module_path)
         module = chipsec.module.Module(module_name)
 
         if module not in self.Loaded_Modules:
             self.Loaded_Modules.append( (module,module_argv) )
-            if not self._list_tags: logger().log( "[+] loaded {}".format(module.get_name()) )
         return True
 
     def load_modules_from_path( self, from_path, recursive = True ):
         if logger().DEBUG: logger().log( "[*] Path: {}".format(os.path.abspath( from_path )) )
         for dirname, subdirs, mod_fnames in os.walk( os.path.abspath( from_path ) ) :
             if not recursive:
                 while len(subdirs) > 0:
                     subdirs.pop()
             for modx in mod_fnames:
                 if fnmatch.fnmatch( modx, '*.py' ) and not fnmatch.fnmatch( modx, '__init__.py' ):
                     self.load_module( os.path.join( dirname, modx ), self._module_argv )
+        self.Loaded_Modules.sort()
+        self.print_loaded_modules()
 
     def load_my_modules(self):
         #
         # Step 1.
         # Load modules common to all supported platforms
         #
         common_path = os.path.join( self.Modules_Path, 'common' )
         logger().log( "[*] loading common modules from \"{}\" ..".format(common_path.replace(os.getcwd(),'.')) )
         self.load_modules_from_path( common_path )
         #
         # Step 2.
         # Load platform-specific modules from the corresponding platform module directory
         #
         chipset_path = os.path.join( self.Modules_Path, self._cs.code.lower() )
-        if (chipset.CHIPSET_ID_UNKNOWN != self._cs.id) and os.path.exists( chipset_path ):
+        if (chipset.CHIPSET_CODE_UNKNOWN != self._cs.code) and os.path.exists( chipset_path ):
             logger().log( "[*] loading platform specific modules from \"{}\" ..".format(chipset_path.replace(os.getcwd(),'.')) )
             self.load_modules_from_path( chipset_path )
         else:
             logger().log( "[*] No platform specific modules to load" )
         #
         # Step 3.
         # Enumerate all modules from the root module directory
@@ -249,15 +253,15 @@
         del self.Loaded_Modules[:]
 
 
     def print_loaded_modules(self):
         if self.Loaded_Modules == []:
             logger().log( "No modules have been loaded" )
         for (modx,modx_argv) in self.Loaded_Modules:
-            logger().log( modx )
+            logger().log( "[+] loaded {}".format(modx) )
 
 
     def run_loaded_modules(self):
 
         results          = logger().Results       
         results.add_properties(self.properties())
 
@@ -289,15 +293,18 @@
 
             logger().end_module( modx.get_name() )
 
         if self._json_out:
             chipsec.file.write_file(self._json_out, results.json_full())
             
         if self._xml_out:
-            chipsec.file.write_file(self._xml_out, results.xml_full(self._xml_out))	
+            chipsec.file.write_file(self._xml_out, results.xml_full(self._xml_out))
+
+        if self._markdown_out:
+            chipsec.file.write_file(self._markdown_out, results.markdown_full(self._markdown_out))
 
         test_deltas = None
         if self._deltas_file is not None:
             prev_results = chipsec.result_deltas.get_json_results(self._deltas_file)
             if prev_results is None:
                 logger().error("Delta processing disabled.  Displaying results summary.")
             else:
@@ -378,20 +385,21 @@
         options.add_argument('-m', '--module',dest='_module', help='specify module to run (example: -m common.bios_wp)')
         options.add_argument('-a','--module_args', nargs='*', dest="_module_argv", help="additional module arguments")
         options.add_argument('-v','--verbose', help='verbose mode', action='store_true')
         options.add_argument('--hal', help='HAL mode', action='store_true')
         options.add_argument('-d','--debug', help='debug mode', action='store_true')
         options.add_argument('-l','--log', help='output to log file')
         adv_options = parser.add_argument_group('Advanced Options')
-        adv_options.add_argument('-p','--platform',dest='_platform', help='explicitly specify platform code',choices=chipset.Chipset_Code, type=str.upper)
-        adv_options.add_argument('--pch',dest='_pch', help='explicitly specify PCH code',choices=chipset.pch_codes, type=str.upper)
+        adv_options.add_argument('-p','--platform',dest='_platform', help='explicitly specify platform code',choices=chipset.cs().chipset_codes, type=str.upper)
+        adv_options.add_argument('--pch',dest='_pch', help='explicitly specify PCH code',choices=chipset.cs().pch_codes, type=str.upper)
         adv_options.add_argument('-n', '--no_driver',dest='_no_driver', help="chipsec won't need kernel mode functions so don't load chipsec driver", action='store_true')
         adv_options.add_argument('-i', '--ignore_platform',dest='_unknownPlatform', help='run chipsec even if the platform is not recognized', action='store_false')
         adv_options.add_argument('-j', '--json',dest='_json_out', help='specify filename for JSON output')
         adv_options.add_argument('-x', '--xml', dest='_xml_out',help='specify filename for xml output (JUnit style)')
+        adv_options.add_argument('-k', '--markdown', dest='_markdown_out',help='specify filename for markdown output')
         adv_options.add_argument('-t', '--moduletype',dest='USER_MODULE_TAGS', help='run tests of a specific type (tag)',type=str.upper,default=[])
         adv_options.add_argument('--list_tags',dest='_list_tags', help='list all the available options for -t,--moduletype',action='store_true')
         adv_options.add_argument('-I', '--include',dest='IMPORT_PATHS', help='specify additional path to load modules from',default=[])
         adv_options.add_argument('--failfast', help="fail on any exception and exit (don't mask exceptions)",action='store_true')
         adv_options.add_argument('--no_time', help="don't log timestamps",action='store_true')
         adv_options.add_argument('--deltas',dest='_deltas_file', help='specifies a JSON log file to compute result deltas from')
         adv_options.add_argument('--record',dest='_to_file',help='run chipsec and clone helper results into JSON file')
@@ -419,24 +427,30 @@
             self._driver_exists = "FileHelper"
 
     def properties( self ):
         ret = OrderedDict()
         ret["OS"] = "{} {} {} {}".format(self._cs.helper.os_system, self._cs.helper.os_release, self._cs.helper.os_version, self._cs.helper.os_machine)
         ret["Python"] = "Python {}".format(platform.python_version())
         ret["Platform"] = "{}, VID: {:04X}, DID: {:04X}, RID: {:02X}".format(self._cs.longname, self._cs.vid, self._cs.did, self._cs.rid) 
-        ret["PCH"] = "{}, VID: {:04X}, DID: {:04X} RID: {:02X}".format(self._cs.pch_longname, self._cs.pch_vid, self._cs.pch_did, self._cs.pch_rid)
+        if not self._cs.is_atom():
+            ret["PCH"] = "{}, VID: {:04X}, DID: {:04X} RID: {:02X}".format(self._cs.pch_longname, self._cs.pch_vid, self._cs.pch_did, self._cs.pch_rid)
         ret["Version"] ="{}".format(self.version)
+        ret["Message"] = "{}".format(self.message)
         return ret
 
     def log_properties( self ):
         logger().log("[CHIPSEC] OS      : {} {} {} {}".format(self._cs.helper.os_system, self._cs.helper.os_release, self._cs.helper.os_version, self._cs.helper.os_machine) )
-        logger().log("[CHIPSEC] Python  : {} ({})".format(platform.python_version(),"64-bit" if sys.maxsize > 2**32 else "32-bit"))
+        logger().log("[CHIPSEC] Python  : {} ({})".format(platform.python_version(),"64-bit" if self.PYTHON_64_BITS else "32-bit"))
         logger().log("[CHIPSEC] Helper  : {} ({})".format(*self._cs.helper.helper.get_info()))
         logger().log("[CHIPSEC] Platform: {}\n[CHIPSEC]      VID: {:04X}\n[CHIPSEC]      DID: {:04X}\n[CHIPSEC]      RID: {:02X}".format(self._cs.longname, self._cs.vid, self._cs.did, self._cs.rid))
-        logger().log("[CHIPSEC] PCH     : {}\n[CHIPSEC]      VID: {:04X}\n[CHIPSEC]      DID: {:04X}\n[CHIPSEC]      RID: {:02X}".format(self._cs.pch_longname, self._cs.pch_vid, self._cs.pch_did, self._cs.pch_rid))
+        if not self._cs.is_atom():
+            logger().log("[CHIPSEC] PCH     : {}\n[CHIPSEC]      VID: {:04X}\n[CHIPSEC]      DID: {:04X}\n[CHIPSEC]      RID: {:02X}".format(self._cs.pch_longname, self._cs.pch_vid, self._cs.pch_did, self._cs.pch_rid))
+
+        if not self.PYTHON_64_BITS and platform.machine().endswith("64"):
+            logger().warn("Python architecture (32-bit) is different from OS architecture (64-bit)")
 
     ##################################################################################
     # Entry point for command-line execution
     ##################################################################################
 
     def main ( self ):
         if self.help:
```

### Comparing `chipsec-1.4.4/chipsec_util.py` & `chipsec-1.5.1/chipsec_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #CHIPSEC: Platform Security Assessment Framework
-#Copyright (c) 2010-2019, Intel Corporation
+#Copyright (c) 2010-2020, Intel Corporation
 #
 #This program is free software; you can redistribute it and/or
 #modify it under the terms of the GNU General Public License
 #as published by the Free Software Foundation; Version 2.
 #
 #This program is distributed in the hope that it will be useful,
 #but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -28,19 +28,20 @@
 import os
 import sys
 import time
 import importlib
 import argparse
 import platform
 
-from chipsec.defines import get_version
+from chipsec.defines import get_version, get_message
+from chipsec.helper import oshelper
 from chipsec.logger  import logger
 from chipsec.chipset import UnknownChipsetError
 from chipsec.testcase import ExitCode
-from chipsec.chipset import cs, Chipset_Code, pch_codes
+from chipsec.chipset import cs
 from chipsec.file import get_main_dir
 
 logger().UTIL_TRACE = True
 
 #CMD_OPTS_WIDTH = [ 'byte', 'word', 'dword', 'qword' ]
 CMD_OPTS_WIDTH = [ 'byte', 'word', 'dword' ]
 def is_option_valid_width( width_op ):
@@ -59,14 +60,16 @@
 
     def __init__(self, argv):
         self.global_usage = "All numeric values are in hex\n" + \
                    "<width> is in {1, byte, 2, word, 4, dword}\n\n"
         self.commands = {}
         # determine if CHIPSEC is loaded as chipsec_*.exe or in python
         self.CHIPSEC_LOADED_AS_EXE = True if (hasattr(sys, "frozen") or hasattr(sys, "importers")) else False
+        # determine if the hosting Python interpreter is a 64-bit executable
+        self.PYTHON_64_BITS = True if (sys.maxsize > 2**32) else False
 
         self.argv = argv
         self.print_banner()
         self.import_cmds()
         self.parse_args()
 
     def init_cs(self):
@@ -76,18 +79,19 @@
         parser = argparse.ArgumentParser(usage='%(prog)s [options] <command>',add_help=False)
         options = parser.add_argument_group('Options')
         options.add_argument('-h', '--help',dest='show_help', help="show this message and exit",action='store_true')
         options.add_argument('-v','--verbose', help='verbose mode', action='store_true')
         options.add_argument('--hal', help='HAL mode', action='store_true')
         options.add_argument('-d','--debug', help='debug mode', action='store_true')
         options.add_argument('-l','--log', help='output to log file')
-        options.add_argument('-p','--platform',dest='_platform', help='explicitly specify platform code',choices=Chipset_Code, type=str.upper)
-        options.add_argument('--pch',dest='_pch', help='explicitly specify PCH code',choices=pch_codes, type=str.upper)
+        options.add_argument('-p','--platform',dest='_platform', help='explicitly specify platform code',choices=cs().chipset_codes, type=str.upper)
+        options.add_argument('--pch',dest='_pch', help='explicitly specify PCH code',choices=cs().pch_codes, type=str.upper)
         options.add_argument('-n', '--no_driver',dest='_no_driver', help="chipsec won't need kernel mode functions so don't load chipsec driver", action='store_true')
-        options.add_argument('-i', '--ignore_platform',dest='_unkownPlatform', help='run chipsec even if the platform is not recognized', action='store_false')
+        options.add_argument('-i', '--ignore_platform',dest='_unknownPlatform', help='run chipsec even if the platform is not recognized', action='store_false')
+        options.add_argument('--helper',dest='_driver_exists', help='specify OS Helper', choices=[i for i in oshelper.avail_helpers])
         options.add_argument('_cmd',metavar='Command', nargs='?', choices=sorted(self.commands.keys()), type=str.lower, default="help",  help="Util command to run: {{{}}}".format(','.join(sorted(self.commands.keys()))))
         options.add_argument('_cmd_args',metavar='Command Args', nargs=argparse.REMAINDER, help=self.global_usage)
 
         parser.parse_args(self.argv,namespace=ChipsecUtil)
         if self.show_help or self._cmd == "help":
             parser.print_help()
         if self.verbose:
@@ -100,16 +104,16 @@
             logger().set_log_file( self.log )
         if not self._cmd_args:
             self._cmd_args = ["--help"]
 
     def import_cmds(self):
         if self.CHIPSEC_LOADED_AS_EXE:
             import zipfile
-            myzip = zipfile.ZipFile("library.zip")
-            cmds = [i.replace('/','.').replace('chipsec.utilcmd.','')[:-4] for i in myzip.namelist() if r'chipsec\/utilcmd\/' in i and i[:-4] == ".pyc" and not i[:2] == '__' ]
+            myzip = zipfile.ZipFile(os.path.join(get_main_dir(),"library.zip"))
+            cmds = [i.replace('/','.').replace('chipsec.utilcmd.','')[:-4] for i in myzip.namelist() if 'chipsec/utilcmd/' in i and i[-4:] == ".pyc" and not os.path.basename(i)[:2] == '__' ]
         else:
             cmds_dir = os.path.join(get_main_dir(),"chipsec","utilcmd")
             cmds = [i[:-3] for i in os.listdir(cmds_dir) if i[-3:] == ".py" and not i[:2] == "__"]
 
         if logger().DEBUG:
             logger().log( '[CHIPSEC] Loaded command-line extensions:' )
             logger().log( '   {}'.format(cmds) )
@@ -144,27 +148,31 @@
 
         # @TODO: change later
         # all util cmds assume 'chipsec_util.py' as the first arg so adding dummy first arg
         self.argv = ['dummy'] + [self._cmd] + self._cmd_args
         comm = self.commands[self._cmd](self.argv, cs = self._cs)
 
         try:
-            self._cs.init( self._platform, self._pch, comm.requires_driver() and not self._no_driver)
+            self._cs.init( self._platform, self._pch, comm.requires_driver() and not self._no_driver, self._driver_exists)
         except UnknownChipsetError as msg:
             logger().warn("*******************************************************************")
             logger().warn("* Unknown platform!")
             logger().warn("* Platform dependent functionality will likely be incorrect")
             logger().warn("* Error Message: \"{}\"".format(str(msg)))
             logger().warn("*******************************************************************")
+            if self._unknownPlatform:
+                logger().error('To run anyways please use -i command-line option\n\n')
+                sys.exit(ExitCode.OK)
         except Exception as msg:
             logger().error(str(msg))
             sys.exit(ExitCode.EXCEPTION)
         logger().log("[CHIPSEC] Helper  : {} ({})".format(*self._cs.helper.helper.get_info()))
         logger().log("[CHIPSEC] Platform: {}\n[CHIPSEC]      VID: {:04X}\n[CHIPSEC]      DID: {:04X}\n[CHIPSEC]      RID: {:02X}".format(self._cs.longname, self._cs.vid, self._cs.did, self._cs.rid))
-        logger().log("[CHIPSEC] PCH     : {}\n[CHIPSEC]      VID: {:04X}\n[CHIPSEC]      DID: {:04X}\n[CHIPSEC]      RID: {:02X}".format(self._cs.pch_longname, self._cs.pch_vid, self._cs.pch_did, self._cs.pch_rid))
+        if not self._cs.is_atom():
+            logger().log("[CHIPSEC] PCH     : {}\n[CHIPSEC]      VID: {:04X}\n[CHIPSEC]      DID: {:04X}\n[CHIPSEC]      RID: {:02X}".format(self._cs.pch_longname, self._cs.pch_vid, self._cs.pch_did, self._cs.pch_rid))
 
         logger().log( "[CHIPSEC] Executing command '{}' with args {}\n".format(self._cmd,self.argv[2:]) )
         comm.run()
         if comm.requires_driver() and not self._no_driver:
             self._cs.destroy(True)
         return comm.ExitCode
 
@@ -176,15 +184,19 @@
         logger().log("################################################################\n"
                      "##                                                            ##\n"
                      "##  CHIPSEC: Platform Hardware Security Assessment Framework  ##\n"
                      "##                                                            ##\n"
                      "################################################################")
         logger().log("[CHIPSEC] Version : {}".format(get_version()))
         logger().log("[CHIPSEC] OS      : {} {} {} {}".format(platform.system(), platform.release(), platform.version(), platform.machine()))
-        logger().log("[CHIPSEC] Python  : {} ({})".format(platform.python_version(),"64-bit" if sys.maxsize > 2**32 else "32-bit"))
+        logger().log("[CHIPSEC] Python  : {} ({})".format(platform.python_version(),"64-bit" if self.PYTHON_64_BITS else "32-bit"))
+        logger().log(get_message())
+
+        if not self.PYTHON_64_BITS and platform.machine().endswith("64"):
+            logger().warn("Python architecture (32-bit) is different from OS architecture (64-bit)")
 
 def main(argv=None):
     chipsecUtil = ChipsecUtil(argv if argv else sys.argv[1:])
     return chipsecUtil.main()
 
 
 if __name__ == "__main__":
```

