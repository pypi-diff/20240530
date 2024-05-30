# Comparing `tmp/ramanchada2-0.1.0.tar.gz` & `tmp/ramanchada2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramanchada2-0.1.0.tar", last modified: Thu May 16 09:47:11 2024, max compression
+gzip compressed data, was "ramanchada2-0.1.1.tar", last modified: Thu May 30 14:29:28 2024, max compression
```

## Comparing `ramanchada2-0.1.0.tar` & `ramanchada2-0.1.1.tar`

### file list

```diff
@@ -1,248 +1,257 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.145836 ramanchada2-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-16 09:47:11.145836 ramanchada2-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/README.pypi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:47:11.145836 ramanchada2-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.089836 ramanchada2-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.093836 ramanchada2-0.1.0/src/ramanchada2/
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.093836 ramanchada2-0.1.0/src/ramanchada2/auxiliary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.093836 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.093836 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.097836 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/
--rw-r--r--   0 runner    (1001) docker     (127)   185598 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_100msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   184263 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_5msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   187339 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/PST10_iR532_Probe_100_3000msx7.txt
--rw-r--r--   0 runner    (1001) docker     (127)   187743 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0B10_iR532_Probe_100_60000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   190431 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0N10_iR532_Probe_100_30000msx3.txt
--rw-r--r--   0 runner    (1001) docker     (127)   189952 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0P10_iR532_Probe_100_60000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   187633 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S1N10_iR532_Probe_100_22000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   187638 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/Sil10_iR532_Probe_100_60000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   191297 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/nCAL10_iR532_Probe_100_2500msx3.txt
--rw-r--r--   0 runner    (1001) docker     (127)   187259 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/sCAL10_iR532_Probe_100_3200msx4.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.105836 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/
--rw-r--r--   0 runner    (1001) docker     (127)    16858 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP01.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35649 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP02.txt
--rw-r--r--   0 runner    (1001) docker     (127)   171476 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP03.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16871 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP01_40000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35658 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP02_50000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   171859 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16863 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP01_6000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35712 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP02_25000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   171856 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16841 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP01_6000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35709 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP02_25000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   171894 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16872 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP01_6000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35718 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP02_25000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   171856 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16867 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP01_6000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35694 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP02_25000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   171844 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16876 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP01_6000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35703 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP02_25000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   171846 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP01_6000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35695 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP02_20000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   171923 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP01_4000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35687 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP02_15000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   171889 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP03_8000msx2.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.113836 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/
--rw-r--r--   0 runner    (1001) docker     (127)   182699 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_110ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   184528 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_2000ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   182774 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_25ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   184434 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_800ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   174788 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z050_100_2500msx5.txt
--rw-r--r--   0 runner    (1001) docker     (127)   175407 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z100_100_50000ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   175468 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z050_100_30000ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   174802 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z100_100_22000ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   175123 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z050_100_40000ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   174660 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z100_100_28000ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   175356 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z050_100_30000ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   174887 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z100_100_20000ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   174718 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z050_100_12000ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   173754 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z100_100_6500ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   176673 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z050_100_9000ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   177120 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z100_100_30000ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   174707 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z050_100_20000ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   175243 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z100_100_65000ms.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.125836 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/
--rw-r--r--   0 runner    (1001) docker     (127)   184364 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z020_100_1300ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   185045 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z050_100_3200ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   185328 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z100_100_9000ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   189806 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_12000ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   201634 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_full.txt
--rw-r--r--   0 runner    (1001) docker     (127)   189411 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z050_100_5500ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   189005 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z100_100_4700ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   187207 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z020_100_3800ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   187573 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z050_100_3200ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   186787 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z100_100_3100ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   189400 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z020_100_12000ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   189244 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z050_100_5700ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   188792 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z100_100_4800ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   185773 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z020_100_3800ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   185317 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z050_100_2100ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   184476 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z100_100_2000ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   183722 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z020_100_1100ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   184176 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z050_100_2100ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   184535 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z100_100_6000ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   184428 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z020_100_2400ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   184511 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z050_100_3800ms.txt
--rw-r--r--   0 runner    (1001) docker     (127)   184796 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z100_100_9500ms.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.129836 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/
--rw-r--r--   0 runner    (1001) docker     (127)   101150 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Pol_HLR633_Z010_100_15sx5.txt
--rw-r--r--   0 runner    (1001) docker     (127)   101182 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0B_HLR633_Z010_100_40sx5.txt
--rw-r--r--   0 runner    (1001) docker     (127)   101185 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0N_HLR633_Z010_100_15sx5.txt
--rw-r--r--   0 runner    (1001) docker     (127)   101119 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0P_HLR633_Z010_100_40sx5.txt
--rw-r--r--   0 runner    (1001) docker     (127)   101189 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S1N_HLR633_Z010_100_10sx5.txt
--rw-r--r--   0 runner    (1001) docker     (127)   101169 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Si_HLR633_Z010_100_40sx5.txt
--rw-r--r--   0 runner    (1001) docker     (127)   101184 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/nCAL_HLR633_Z010_100_5sx5.txt
--rw-r--r--   0 runner    (1001) docker     (127)   101184 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/neon_new2_Z010.txt
--rw-r--r--   0 runner    (1001) docker     (127)   101413 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/sCAL_HLR633_Z010_100_15sx5.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.129836 ramanchada2-0.1.0/src/ramanchada2/io/
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/HSDS.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.129836 ramanchada2-0.1.0/src/ramanchada2/io/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/experimental/bw_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.129836 ramanchada2-0.1.0/src/ramanchada2/io/experimental/rc1_parser/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/experimental/rc1_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/experimental/rc1_parser/binary_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/experimental/rc1_parser/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/experimental/rc1_parser/third_party_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/experimental/rc1_parser/txt_format_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/experimental/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/experimental/read_txt.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/experimental/two_column_spe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.129836 ramanchada2-0.1.0/src/ramanchada2/io/output/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/output/write_csv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.129836 ramanchada2-0.1.0/src/ramanchada2/io/simulated/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/simulated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.129836 ramanchada2-0.1.0/src/ramanchada2/io/simulated/crystal/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/simulated/crystal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/simulated/crystal/discrete_lines_dat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/simulated/crystal/discrete_lines_out.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/simulated/lines_from_raw_dat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/simulated/read_simulated_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.129836 ramanchada2-0.1.0/src/ramanchada2/io/simulated/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/simulated/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/io/simulated/vasp/vasp_simulation_dat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.133836 ramanchada2-0.1.0/src/ramanchada2/misc/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/base_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    23672 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/plottable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.133836 ramanchada2-0.1.0/src/ramanchada2/misc/spectrum_deco/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/spectrum_deco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/spectrum_deco/dynamically_added.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/spectrum_deco/spectrum_constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/spectrum_deco/spectrum_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/spectrum_deco/spectrum_method.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.133836 ramanchada2-0.1.0/src/ramanchada2/misc/types/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/types/fit_peaks_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/types/peak_candidates.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/types/positive_not_multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/types/pydantic_base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.133836 ramanchada2-0.1.0/src/ramanchada2/misc/types/spectrum/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/types/spectrum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/types/spectrum/applied_processings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/types/spectrum/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.133836 ramanchada2-0.1.0/src/ramanchada2/misc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/utils/argmin2d.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/utils/ramanshift_to_wavelength.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/misc/utils/svd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.137836 ramanchada2-0.1.0/src/ramanchada2/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14344 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/protocols/calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.137836 ramanchada2-0.1.0/src/ramanchada2/spectral_components/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectral_components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.137836 ramanchada2-0.1.0/src/ramanchada2/spectral_components/baseline/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectral_components/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectral_components/baseline/analytical.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectral_components/baseline/baseline_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectral_components/baseline/numerical.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.137836 ramanchada2-0.1.0/src/ramanchada2/spectral_components/peak_profile/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectral_components/peak_profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectral_components/peak_profile/delta.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectral_components/peak_profile/gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectral_components/peak_profile/voigt.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectral_components/spectral_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectral_components/spectral_component_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectral_components/spectral_peak.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.137836 ramanchada2-0.1.0/src/ramanchada2/spectrum/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.137836 ramanchada2-0.1.0/src/ramanchada2/spectrum/arithmetics/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/arithmetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/arithmetics/add.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/arithmetics/mul.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/arithmetics/sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/arithmetics/truediv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.141836 ramanchada2-0.1.0/src/ramanchada2/spectrum/baseline/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/baseline/add_baseline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/baseline/baseline_rc1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/baseline/moving_minimum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.141836 ramanchada2-0.1.0/src/ramanchada2/spectrum/calc/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/calc/central_moments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.141836 ramanchada2-0.1.0/src/ramanchada2/spectrum/calibration/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/calibration/by_deltas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/calibration/change_x_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/calibration/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/calibration/scale_xaxis.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/calibration/scale_yaxis.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/calibration/set_new_xaxis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.141836 ramanchada2-0.1.0/src/ramanchada2/spectrum/creators/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/creators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/creators/from_cache_or_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/creators/from_chada.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/creators/from_delta_lines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/creators/from_local_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/creators/from_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/creators/from_spectral_component_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/creators/from_test_spe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/creators/from_theoretical_lines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/creators/hdr_from_multi_exposure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.145836 ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/add_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/add_gaussian_noise_drift.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/add_poisson_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/convolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/drop_spikes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/moving_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/moving_median.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/pad_zeros.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/resampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/sharpen_lines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/trim_axes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.145836 ramanchada2-0.1.0/src/ramanchada2/spectrum/peaks/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/peaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/peaks/find_peaks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/peaks/find_peaks_BayesianGaussianMixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/peaks/fit_peaks.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/peaks/get_fitted_peaks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/spectrum/spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.145836 ramanchada2-0.1.0/src/ramanchada2/theoretical_lines/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/theoretical_lines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-16 09:47:07.000000 ramanchada2-0.1.0/src/ramanchada2/theoretical_lines/model_from_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:47:11.145836 ramanchada2-0.1.0/src/ramanchada2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-16 09:47:11.000000 ramanchada2-0.1.0/src/ramanchada2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13387 2024-05-16 09:47:11.000000 ramanchada2-0.1.0/src/ramanchada2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:47:11.000000 ramanchada2-0.1.0/src/ramanchada2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-16 09:47:11.000000 ramanchada2-0.1.0/src/ramanchada2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 09:47:11.000000 ramanchada2-0.1.0/src/ramanchada2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.579892 ramanchada2-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-30 14:29:28.579892 ramanchada2-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/README.pypi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 14:29:28.579892 ramanchada2-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.527891 ramanchada2-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.531891 ramanchada2-0.1.1/src/ramanchada2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.531891 ramanchada2-0.1.1/src/ramanchada2/auxiliary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.531891 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.531891 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.535891 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/
+-rw-r--r--   0 runner    (1001) docker     (127)   187419 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/LED532_Probe_40msx3_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   189434 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NIST532_Probe_3000msx8_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   185598 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_100msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   184263 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_5msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   187339 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/PST10_iR532_Probe_100_3000msx7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   187743 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0B10_iR532_Probe_100_60000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   190431 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0N10_iR532_Probe_100_30000msx3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   189952 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0P10_iR532_Probe_100_60000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   187633 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S1N10_iR532_Probe_100_22000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   187638 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/Sil10_iR532_Probe_100_60000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   191297 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/nCAL10_iR532_Probe_100_2500msx3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   187259 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/sCAL10_iR532_Probe_100_3200msx4.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.543891 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/
+-rw-r--r--   0 runner    (1001) docker     (127)    15995 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/LED785_Lens_1000x10_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13877 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NIST785_Lens_80000x5_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16858 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35649 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   171476 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16871 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP01_40000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35658 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP02_50000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   171859 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16863 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP01_6000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35712 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP02_25000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   171856 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16841 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP01_6000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35709 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP02_25000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   171894 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16872 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP01_6000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35718 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP02_25000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   171856 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16867 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP01_6000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35694 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP02_25000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   171844 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16876 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP01_6000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35703 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP02_25000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   171846 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP01_6000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35695 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP02_20000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   171923 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP01_4000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35687 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP02_15000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   171889 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP03_8000msx2.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.551891 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/
+-rw-r--r--   0 runner    (1001) docker     (127)   191716 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/NISTSRM2242aC_BW532_100x_800msx10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   182699 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_110ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   184528 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_2000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   182774 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_25ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   184434 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_800ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   174788 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z050_100_2500msx5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   175407 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z100_100_50000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   175468 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z050_100_30000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   174802 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z100_100_22000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   175123 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z050_100_40000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   174660 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z100_100_28000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   175356 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z050_100_30000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   174887 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z100_100_20000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   174718 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z050_100_12000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   173754 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z100_100_6500ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   189499 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Visible_532nm_130ms_100X_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   176673 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z050_100_9000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   177120 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z100_100_30000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   174707 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z050_100_20000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   175243 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z100_100_65000ms.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.559891 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/
+-rw-r--r--   0 runner    (1001) docker     (127)   188037 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/NIR_785nm_2000ms_100X_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   190834 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/NISTSRM2241_BW785_100x_25sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   189927 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/Ne_785nm_x20_50ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   184364 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z020_100_1300ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   185045 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z050_100_3200ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   185328 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z100_100_9000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   189806 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_12000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   201634 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_full.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   189411 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z050_100_5500ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   189005 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z100_100_4700ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   187207 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z020_100_3800ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   187573 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z050_100_3200ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   186787 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z100_100_3100ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   189400 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z020_100_12000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   189244 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z050_100_5700ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   188792 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z100_100_4800ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   185773 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z020_100_3800ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   185317 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z050_100_2100ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   184476 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z100_100_2000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   183722 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z020_100_1100ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   184176 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z050_100_2100ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   184535 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z100_100_6000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   184428 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z020_100_2400ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   184511 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z050_100_3800ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   184796 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z100_100_9500ms.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.563891 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/
+-rw-r--r--   0 runner    (1001) docker     (127)   101150 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Pol_HLR633_Z010_100_15sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   101182 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0B_HLR633_Z010_100_40sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   101185 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0N_HLR633_Z010_100_15sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   101119 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0P_HLR633_Z010_100_40sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   101189 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S1N_HLR633_Z010_100_10sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   101169 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Si_HLR633_Z010_100_40sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   101184 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/nCAL_HLR633_Z010_100_5sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   101184 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/neon_new2_Z010.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   101413 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/sCAL_HLR633_Z010_100_15sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16272 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.563891 ramanchada2-0.1.1/src/ramanchada2/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/HSDS.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.563891 ramanchada2-0.1.1/src/ramanchada2/io/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/experimental/bw_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.567891 ramanchada2-0.1.1/src/ramanchada2/io/experimental/rc1_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/experimental/rc1_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/experimental/rc1_parser/binary_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/experimental/rc1_parser/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/experimental/rc1_parser/third_party_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/experimental/rc1_parser/txt_format_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/experimental/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/experimental/read_txt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/experimental/two_column_spe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.567891 ramanchada2-0.1.1/src/ramanchada2/io/output/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/output/write_csv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.567891 ramanchada2-0.1.1/src/ramanchada2/io/simulated/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/simulated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.567891 ramanchada2-0.1.1/src/ramanchada2/io/simulated/crystal/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/simulated/crystal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/simulated/crystal/discrete_lines_dat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/simulated/crystal/discrete_lines_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/simulated/lines_from_raw_dat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/simulated/read_simulated_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.567891 ramanchada2-0.1.1/src/ramanchada2/io/simulated/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/simulated/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/io/simulated/vasp/vasp_simulation_dat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.567891 ramanchada2-0.1.1/src/ramanchada2/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23672 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/plottable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.567891 ramanchada2-0.1.1/src/ramanchada2/misc/spectrum_deco/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/spectrum_deco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/spectrum_deco/dynamically_added.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/spectrum_deco/spectrum_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/spectrum_deco/spectrum_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/spectrum_deco/spectrum_method.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.571891 ramanchada2-0.1.1/src/ramanchada2/misc/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/types/fit_peaks_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/types/peak_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/types/positive_not_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/types/pydantic_base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.571891 ramanchada2-0.1.1/src/ramanchada2/misc/types/spectrum/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/types/spectrum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/types/spectrum/applied_processings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/types/spectrum/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.571891 ramanchada2-0.1.1/src/ramanchada2/misc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/utils/argmin2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/utils/ramanshift_to_wavelength.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/misc/utils/svd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.571891 ramanchada2-0.1.1/src/ramanchada2/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23617 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/protocols/calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.571891 ramanchada2-0.1.1/src/ramanchada2/spectral_components/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectral_components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.571891 ramanchada2-0.1.1/src/ramanchada2/spectral_components/baseline/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectral_components/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectral_components/baseline/analytical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectral_components/baseline/baseline_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectral_components/baseline/numerical.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.571891 ramanchada2-0.1.1/src/ramanchada2/spectral_components/peak_profile/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectral_components/peak_profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectral_components/peak_profile/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectral_components/peak_profile/gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectral_components/peak_profile/voigt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectral_components/spectral_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectral_components/spectral_component_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectral_components/spectral_peak.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.571891 ramanchada2-0.1.1/src/ramanchada2/spectrum/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.575892 ramanchada2-0.1.1/src/ramanchada2/spectrum/arithmetics/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/arithmetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/arithmetics/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/arithmetics/mul.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/arithmetics/sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/arithmetics/truediv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.575892 ramanchada2-0.1.1/src/ramanchada2/spectrum/baseline/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/baseline/add_baseline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/baseline/baseline_rc1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/baseline/moving_minimum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.575892 ramanchada2-0.1.1/src/ramanchada2/spectrum/calc/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/calc/central_moments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.575892 ramanchada2-0.1.1/src/ramanchada2/spectrum/calibration/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/calibration/by_deltas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/calibration/change_x_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/calibration/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/calibration/scale_xaxis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/calibration/scale_yaxis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/calibration/set_new_xaxis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.575892 ramanchada2-0.1.1/src/ramanchada2/spectrum/creators/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/creators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/creators/from_cache_or_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/creators/from_chada.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/creators/from_delta_lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/creators/from_local_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/creators/from_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/creators/from_spectral_component_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/creators/from_test_spe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/creators/from_theoretical_lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/creators/hdr_from_multi_exposure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.579892 ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/add_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/add_gaussian_noise_drift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/add_poisson_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/convolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/drop_spikes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/moving_median.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/pad_zeros.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/resampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/sharpen_lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/trim_axes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.579892 ramanchada2-0.1.1/src/ramanchada2/spectrum/peaks/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/peaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/peaks/find_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/peaks/find_peaks_BayesianGaussianMixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/peaks/fit_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/peaks/get_fitted_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/spectrum/spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.579892 ramanchada2-0.1.1/src/ramanchada2/theoretical_lines/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/theoretical_lines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-30 14:29:24.000000 ramanchada2-0.1.1/src/ramanchada2/theoretical_lines/model_from_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:29:28.579892 ramanchada2-0.1.1/src/ramanchada2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-30 14:29:28.000000 ramanchada2-0.1.1/src/ramanchada2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14145 2024-05-30 14:29:28.000000 ramanchada2-0.1.1/src/ramanchada2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:29:28.000000 ramanchada2-0.1.1/src/ramanchada2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-30 14:29:28.000000 ramanchada2-0.1.1/src/ramanchada2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 14:29:28.000000 ramanchada2-0.1.1/src/ramanchada2.egg-info/top_level.txt
```

### Comparing `ramanchada2-0.1.0/LICENSE` & `ramanchada2-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/PKG-INFO` & `ramanchada2-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramanchada2
-Version: 0.1.0
+Version: 0.1.1
 Summary: Harmonising Raman Spectroscopy
 Home-page: https://github.com/h2020charisma/ramanchada2
 Author: IDEAconsult Ltd.
 Author-email: dev-charisma@ideaconsult.net
 License: MIT
 Keywords: Raman,spectroscopy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ramanchada2-0.1.0/README.md` & `ramanchada2-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/README.pypi` & `ramanchada2-0.1.1/README.pypi`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/setup.py` & `ramanchada2-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/__init__.py` & `ramanchada2-0.1.1/src/ramanchada2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     'io',
     'misc',
     'protocols',
     'spectral_components',
     'spectrum',
     'theoretical_lines'
 ]
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 
 import logging
 
 
 class CustomFormatter(logging.Formatter):
     green = "\x1b[32m"
```

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_100msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_100msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_5msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_5msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/PST10_iR532_Probe_100_3000msx7.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/PST10_iR532_Probe_100_3000msx7.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0B10_iR532_Probe_100_60000msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0B10_iR532_Probe_100_60000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0N10_iR532_Probe_100_30000msx3.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0N10_iR532_Probe_100_30000msx3.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0P10_iR532_Probe_100_60000msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0P10_iR532_Probe_100_60000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S1N10_iR532_Probe_100_22000msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S1N10_iR532_Probe_100_22000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/Sil10_iR532_Probe_100_60000msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/Sil10_iR532_Probe_100_60000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/nCAL10_iR532_Probe_100_2500msx3.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/nCAL10_iR532_Probe_100_2500msx3.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/sCAL10_iR532_Probe_100_3200msx4.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/sCAL10_iR532_Probe_100_3200msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP01.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP01.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP02.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP02.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP03.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP03.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP01_40000msx4.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP01_40000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP02_50000msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP02_50000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP01_6000msx4.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP01_6000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP02_25000msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP02_25000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP01_6000msx4.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP01_6000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP02_25000msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP02_25000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP01_6000msx4.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP01_6000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP02_25000msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP02_25000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP01_6000msx4.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP01_6000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP02_25000msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP02_25000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP01_6000msx4.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP01_6000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP02_25000msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP02_25000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP01_6000msx4.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP01_6000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP02_20000msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP02_20000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP01_4000msx4.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP01_4000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP02_15000msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP02_15000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_110ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_110ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_2000ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_2000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_25ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_25ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_800ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_800ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z050_100_2500msx5.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z050_100_2500msx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z100_100_50000ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z100_100_50000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z050_100_30000ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z050_100_30000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z100_100_22000ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z100_100_22000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z050_100_40000ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z050_100_40000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z100_100_28000ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z100_100_28000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z050_100_30000ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z050_100_30000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z100_100_20000ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z100_100_20000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z050_100_12000ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z050_100_12000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z100_100_6500ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z100_100_6500ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z050_100_9000ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z050_100_9000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z100_100_30000ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z100_100_30000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z050_100_20000ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z050_100_20000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z100_100_65000ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z100_100_65000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z020_100_1300ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z020_100_1300ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z050_100_3200ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z050_100_3200ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z100_100_9000ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z100_100_9000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_12000ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_12000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_full.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_full.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z050_100_5500ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z050_100_5500ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z100_100_4700ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z100_100_4700ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z020_100_3800ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z020_100_3800ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z050_100_3200ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z050_100_3200ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z100_100_3100ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z100_100_3100ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z020_100_12000ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z020_100_12000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z050_100_5700ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z050_100_5700ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z100_100_4800ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z100_100_4800ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z020_100_3800ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z020_100_3800ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z050_100_2100ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z050_100_2100ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z100_100_2000ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z100_100_2000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z020_100_1100ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z020_100_1100ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z050_100_2100ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z050_100_2100ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z100_100_6000ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z100_100_6000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z020_100_2400ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z020_100_2400ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z050_100_3800ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z050_100_3800ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z100_100_9500ms.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z100_100_9500ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Pol_HLR633_Z010_100_15sx5.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Pol_HLR633_Z010_100_15sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0B_HLR633_Z010_100_40sx5.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0B_HLR633_Z010_100_40sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0N_HLR633_Z010_100_15sx5.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0N_HLR633_Z010_100_15sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0P_HLR633_Z010_100_40sx5.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0P_HLR633_Z010_100_40sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S1N_HLR633_Z010_100_10sx5.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S1N_HLR633_Z010_100_10sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Si_HLR633_Z010_100_40sx5.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Si_HLR633_Z010_100_40sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/nCAL_HLR633_Z010_100_5sx5.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/nCAL_HLR633_Z010_100_5sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/neon_new2_Z010.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/neon_new2_Z010.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/sCAL_HLR633_Z010_100_15sx5.txt` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/sCAL_HLR633_Z010_100_15sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/auxiliary/spectra/datasets2/__init__.py` & `ramanchada2-0.1.1/src/ramanchada2/auxiliary/spectra/datasets2/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,18 @@
         'laser_wl': '532', 'provider': 'FNMT', 'sample': 'S1N'},
     {'OP': '01', 'device': 'BWtek', 'filename': './FMNT-M_BW532/Sil10_iR532_Probe_100_60000msx2.txt',
         'laser_wl': '532', 'provider': 'FNMT', 'sample': 'Sil_'},
     {'OP': '01', 'device': 'BWtek', 'filename': './FMNT-M_BW532/nCAL10_iR532_Probe_100_2500msx3.txt',
         'laser_wl': '532', 'provider': 'FNMT', 'sample': 'nCAL'},
     {'OP': '01', 'device': 'BWtek', 'filename': './FMNT-M_BW532/sCAL10_iR532_Probe_100_3200msx4.txt',
         'laser_wl': '532', 'provider': 'FNMT', 'sample': 'sCAL'},
+    {'OP': '01', 'device': 'BWtek', 'filename': './FMNT-M_BW532/LED532_Probe_40msx3_1.txt',
+        'laser_wl': '532', 'provider': 'FNMT', 'sample': 'LED532_EL0-9001'},
+    {'OP': '01', 'device': 'BWtek', 'filename': './FMNT-M_BW532/NIST532_Probe_3000msx8_1.txt',
+        'laser_wl': '532', 'provider': 'FNMT', 'sample': 'NIST532_SRM2242a'},
     {'OP': '01', 'device': 'Horiba', 'filename': './FMNT-M_Ho785/NeonSNQ043_iR785_OP01.txt',
         'laser_wl': '785', 'provider': 'FNMT', 'sample': 'Neon'},
     {'OP': '01', 'device': 'Horiba', 'filename': './FMNT-M_Ho785/PST10_iR785_OP01_40000msx4.txt',
         'laser_wl': '785', 'provider': 'FNMT', 'sample': 'PST'},
     {'OP': '01', 'device': 'Horiba', 'filename': './FMNT-M_Ho785/S0B10_iR785_OP01_6000msx4.txt',
         'laser_wl': '785', 'provider': 'FNMT', 'sample': 'S0B'},
     {'OP': '01', 'device': 'Horiba', 'filename': './FMNT-M_Ho785/S0N10_iR785_OP01_6000msx4.txt',
@@ -73,14 +77,18 @@
         'laser_wl': '785', 'provider': 'FNMT', 'sample': 'S1N'},
     {'OP': '03', 'device': 'Horiba', 'filename': './FMNT-M_Ho785/Sil10_iR785_OP03_8000msx2.txt',
         'laser_wl': '785', 'provider': 'FNMT', 'sample': 'Sil'},
     {'OP': '03', 'device': 'Horiba', 'filename': './FMNT-M_Ho785/nCAL10_iR785_OP03_8000msx2.txt',
         'laser_wl': '785', 'provider': 'FNMT', 'sample': 'nCAL'},
     {'OP': '03', 'device': 'Horiba', 'filename': './FMNT-M_Ho785/sCAL10_iR785_OP03_8000msx2.txt',
         'laser_wl': '785', 'provider': 'FNMT', 'sample': 'sCAL'},
+    {'OP': '03', 'device': 'Horiba', 'filename': './FMNT-M_Ho785/LED785_Lens_1000x10_2.txt',
+        'laser_wl': '785', 'provider': 'FNMT', 'sample': 'NIR785_EL0-9002'},
+    {'OP': '03', 'device': 'Horiba', 'filename': './FMNT-M_Ho785/NIST785_Lens_80000x5_2.txt',
+        'laser_wl': '785', 'provider': 'FNMT', 'sample': 'NIST785_SRM2241'},
     {'OP': '050', 'device': 'BWtek', 'filename': './ICV_BW532/Ne_532nm_x50_800ms.txt',
         'laser_wl': '532', 'provider': 'ICV', 'sample': 'Neon'},
     {'OP': '050', 'device': 'BWtek', 'filename': './ICV_BW532/Ne_532nm_x50_25ms.txt',
         'laser_wl': '532', 'provider': 'ICV', 'sample': 'Neon'},
     {'OP': '050', 'device': 'BWtek', 'filename': './ICV_BW532/PST02_iRPlus532_Z050_100_2500msx5.txt',
         'laser_wl': '532', 'provider': 'ICV', 'sample': 'PST'},
     {'OP': '050', 'device': 'BWtek', 'filename': './ICV_BW532/S0B02_iRPlus532_Z050_100_30000ms.txt',
@@ -109,14 +117,18 @@
         'laser_wl': '532', 'provider': 'ICV', 'sample': 'S0P'},
     {'OP': '100', 'device': 'BWtek', 'filename': './ICV_BW532/S1N02_iRPlus532_Z100_100_6500ms.txt',
         'laser_wl': '532', 'provider': 'ICV', 'sample': 'S1N'},
     {'OP': '100', 'device': 'BWtek', 'filename': './ICV_BW532/nCAL02_iRPlus532_Z100_100_30000ms.txt',
         'laser_wl': '532', 'provider': 'ICV', 'sample': 'nCAL'},
     {'OP': '100', 'device': 'BWtek', 'filename': './ICV_BW532/sCAL02_iRPlus532_Z100_100_65000ms.txt',
         'laser_wl': '532', 'provider': 'ICV', 'sample': 'sCAL'},
+    {'OP': '100', 'device': 'BWtek', 'filename': './ICV_BW532/Visible_532nm_130ms_100X_2.txt',
+        'laser_wl': '532', 'provider': 'ICV', 'sample': 'LED532_EL0-9001'},
+    {'OP': '100', 'device': 'BWtek', 'filename': './ICV_BW532/NISTSRM2242aC_BW532_100x_800msx10.txt',
+        'laser_wl': '532', 'provider': 'ICV', 'sample': 'NIST532_SRM2242a'},
     {'OP': '020', 'device': 'BWtek', 'filename': './ICV_BW785/PST02_iRPlus785_Z020_100_1300ms.txt',
         'laser_wl': '785', 'provider': 'ICV', 'sample': 'PST'},
     {'OP': '020', 'device': 'BWtek', 'filename': './ICV_BW785/S0B02_iRPlus785_Z020_100_full.txt',
         'laser_wl': '785', 'provider': 'ICV', 'sample': 'S0B'},
     {'OP': '020', 'device': 'BWtek', 'filename': './ICV_BW785/S0B02_iRPlus785_Z020_100_12000ms.txt',
         'laser_wl': '785', 'provider': 'ICV', 'sample': 'S0B'},
     {'OP': '020', 'device': 'BWtek', 'filename': './ICV_BW785/S0N02_iRPlus785_Z020_100_3800ms.txt',
@@ -153,14 +165,21 @@
         'laser_wl': '785', 'provider': 'ICV', 'sample': 'S0P'},
     {'OP': '100', 'device': 'BWtek', 'filename': './ICV_BW785/S1N02_iRPlus785_Z100_100_2000ms.txt',
         'laser_wl': '785', 'provider': 'ICV', 'sample': 'S1N'},
     {'OP': '100', 'device': 'BWtek', 'filename': './ICV_BW785/nCAL02_iRPlus785_Z100_100_6000ms.txt',
         'laser_wl': '785', 'provider': 'ICV', 'sample': 'nCAL'},
     {'OP': '100', 'device': 'BWtek', 'filename': './ICV_BW785/sCAL02_iRPlus785_Z100_100_9500ms.txt',
         'laser_wl': '785', 'provider': 'ICV', 'sample': 'sCAL'},
+    {'OP': '100', 'device': 'BWtek', 'filename': './ICV_BW785/NIR_785nm_2000ms_100X_2.txt',
+        'laser_wl': '785', 'provider': 'ICV', 'sample': 'NIR785_EL0-9002'},
+    {'OP': '100', 'device': 'BWtek', 'filename': './ICV_BW785/NISTSRM2241_BW785_100x_25sx5.txt',
+        'laser_wl': '785', 'provider': 'ICV', 'sample': 'NIST785_SRM2241'},
+    {'OP': '100', 'device': 'BWtek', 'filename': './ICV_BW785/Ne_785nm_x20_50ms.txt',
+        'laser_wl': '785', 'provider': 'ICV', 'sample': 'Neon'},
+
     {'OP': '010', 'device': 'Horiba', 'filename': './TOP_Ho633/neon_new2_Z010.txt',
         'laser_wl': '633', 'provider': 'TOP', 'sample': 'Neon'},
     {'OP': '010', 'device': 'Horiba', 'filename': './TOP_Ho633/Pol_HLR633_Z010_100_15sx5.txt',
         'laser_wl': '633', 'provider': 'TOP', 'sample': 'PST'},
     {'OP': '010', 'device': 'Horiba', 'filename': './TOP_Ho633/S0B_HLR633_Z010_100_40sx5.txt',
         'laser_wl': '633', 'provider': 'TOP', 'sample': 'S0B'},
     {'OP': '010', 'device': 'Horiba', 'filename': './TOP_Ho633/S0N_HLR633_Z010_100_15sx5.txt',
```

### Comparing `ramanchada2-0.1.0/src/ramanchada2/io/HSDS.py` & `ramanchada2-0.1.1/src/ramanchada2/io/HSDS.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/io/experimental/bw_format.py` & `ramanchada2-0.1.1/src/ramanchada2/io/experimental/bw_format.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/io/experimental/rc1_parser/binary_readers.py` & `ramanchada2-0.1.1/src/ramanchada2/io/experimental/rc1_parser/binary_readers.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/io/experimental/rc1_parser/io.py` & `ramanchada2-0.1.1/src/ramanchada2/io/experimental/rc1_parser/io.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/io/experimental/rc1_parser/third_party_readers.py` & `ramanchada2-0.1.1/src/ramanchada2/io/experimental/rc1_parser/third_party_readers.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/io/experimental/rc1_parser/txt_format_readers.py` & `ramanchada2-0.1.1/src/ramanchada2/io/experimental/rc1_parser/txt_format_readers.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/io/experimental/read_csv.py` & `ramanchada2-0.1.1/src/ramanchada2/io/experimental/read_csv.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/io/experimental/read_txt.py` & `ramanchada2-0.1.1/src/ramanchada2/io/experimental/read_txt.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/io/simulated/crystal/discrete_lines_dat.py` & `ramanchada2-0.1.1/src/ramanchada2/io/simulated/crystal/discrete_lines_dat.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/io/simulated/crystal/discrete_lines_out.py` & `ramanchada2-0.1.1/src/ramanchada2/io/simulated/crystal/discrete_lines_out.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/io/simulated/read_simulated_lines.py` & `ramanchada2-0.1.1/src/ramanchada2/io/simulated/read_simulated_lines.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/io/simulated/vasp/vasp_simulation_dat.py` & `ramanchada2-0.1.1/src/ramanchada2/io/simulated/vasp/vasp_simulation_dat.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/misc/base_class.py` & `ramanchada2-0.1.1/src/ramanchada2/misc/base_class.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/misc/constants.py` & `ramanchada2-0.1.1/src/ramanchada2/misc/constants.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/misc/spectrum_deco/spectrum_constructor.py` & `ramanchada2-0.1.1/src/ramanchada2/misc/spectrum_deco/spectrum_constructor.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/misc/spectrum_deco/spectrum_filter.py` & `ramanchada2-0.1.1/src/ramanchada2/misc/spectrum_deco/spectrum_filter.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/misc/types/fit_peaks_result.py` & `ramanchada2-0.1.1/src/ramanchada2/misc/types/fit_peaks_result.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/misc/types/peak_candidates.py` & `ramanchada2-0.1.1/src/ramanchada2/misc/types/peak_candidates.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/misc/types/positive_not_multiple.py` & `ramanchada2-0.1.1/src/ramanchada2/misc/types/positive_not_multiple.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/misc/types/spectrum/applied_processings.py` & `ramanchada2-0.1.1/src/ramanchada2/misc/types/spectrum/applied_processings.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/misc/types/spectrum/metadata.py` & `ramanchada2-0.1.1/src/ramanchada2/misc/types/spectrum/metadata.py`

 * *Files 9% similar despite different names*

```diff
@@ -71,7 +71,13 @@
         self.__root__.update(self.validate(val).__root__)
 
     def _del_key(self, key: str):
         del self.__root__[key]
 
     def _flush(self):
         self.__root__ = {}
+
+    def get_all_keys(self) -> list[str]:
+        """
+        Returns a list of all keys in the metadata model.
+        """
+        return list(self.__root__.keys())
```

### Comparing `ramanchada2-0.1.0/src/ramanchada2/misc/utils/__init__.py` & `ramanchada2-0.1.1/src/ramanchada2/misc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/misc/utils/argmin2d.py` & `ramanchada2-0.1.1/src/ramanchada2/misc/utils/argmin2d.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/misc/utils/ramanshift_to_wavelength.py` & `ramanchada2-0.1.1/src/ramanchada2/misc/utils/ramanshift_to_wavelength.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectral_components/peak_profile/delta.py` & `ramanchada2-0.1.1/src/ramanchada2/spectral_components/peak_profile/delta.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectral_components/peak_profile/gauss.py` & `ramanchada2-0.1.1/src/ramanchada2/spectral_components/peak_profile/gauss.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectral_components/spectral_component_collection.py` & `ramanchada2-0.1.1/src/ramanchada2/spectral_components/spectral_component_collection.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectral_components/spectral_peak.py` & `ramanchada2-0.1.1/src/ramanchada2/spectral_components/spectral_peak.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/__init__.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/__init__.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/arithmetics/add.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/arithmetics/add.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/arithmetics/mul.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/arithmetics/mul.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/arithmetics/sub.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/arithmetics/sub.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/arithmetics/truediv.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/arithmetics/truediv.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/baseline/add_baseline.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/baseline/add_baseline.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/baseline/baseline_rc1.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/baseline/baseline_rc1.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/baseline/moving_minimum.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/baseline/moving_minimum.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/calc/central_moments.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/calc/central_moments.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/calibration/by_deltas.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/calibration/by_deltas.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/calibration/change_x_units.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/calibration/change_x_units.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/calibration/normalize.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/calibration/normalize.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/calibration/scale_xaxis.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/calibration/scale_xaxis.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/calibration/set_new_xaxis.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/calibration/set_new_xaxis.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/creators/from_cache_or_calc.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/creators/from_cache_or_calc.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/creators/from_delta_lines.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/creators/from_delta_lines.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/creators/from_local_file.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/creators/from_local_file.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/creators/from_simulation.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/creators/from_simulation.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/creators/from_spectral_component_collection.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/creators/from_spectral_component_collection.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/creators/from_test_spe.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/creators/from_test_spe.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/creators/from_theoretical_lines.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/creators/from_theoretical_lines.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/creators/hdr_from_multi_exposure.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/creators/hdr_from_multi_exposure.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/add_gaussian_noise.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/add_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/add_gaussian_noise_drift.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/add_gaussian_noise_drift.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/add_poisson_noise.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/add_poisson_noise.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/convolve.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/convolve.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/drop_spikes.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/drop_spikes.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/moving_average.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/moving_average.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/moving_median.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/moving_median.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/pad_zeros.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/pad_zeros.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/resampling.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/resampling.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/sharpen_lines.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/sharpen_lines.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/smoothing.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/smoothing.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 @add_spectrum_filter
 @validate_arguments(config=dict(arbitrary_types_allowed=True))
 def smoothing_RC1(old_spe: Spectrum,
                   new_spe: Spectrum, /, *args,
                   method: Literal['savgol', 'sg',
                                   'wiener',
                                   'median',
-                                  'gauss',
+                                  'gauss', 'gaussian',
                                   'lowess',
                                   'boxcar'],
                   **kwargs):
     if method == 'savgol' or method == 'sg':
         new_spe.y = savgol_filter(old_spe.y, **kwargs)  # window_length, polyorder
     elif method == 'wiener':
         new_spe.y = wiener(old_spe.y, **kwargs)
-    elif method == 'gaussian':
+    elif method == 'gaussian' or method == 'gauss':
         new_spe.y = gaussian_filter1d(old_spe.y, **kwargs)  # sigma
     elif method == 'median':
         new_spe.y = medfilt(old_spe.y, **kwargs)
     elif method == 'lowess':
         kw = dict(span=11)
         kw.update(kwargs)
         x = np.linspace(0, 1, len(old_spe.y))
```

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/filters/trim_axes.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/filters/trim_axes.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/peaks/find_peaks.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/peaks/find_peaks.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/peaks/find_peaks_BayesianGaussianMixture.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/peaks/find_peaks_BayesianGaussianMixture.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/peaks/fit_peaks.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/peaks/fit_peaks.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/peaks/get_fitted_peaks.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/peaks/get_fitted_peaks.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/spectrum/spectrum.py` & `ramanchada2-0.1.1/src/ramanchada2/spectrum/spectrum.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2/theoretical_lines/model_from_lines.py` & `ramanchada2-0.1.1/src/ramanchada2/theoretical_lines/model_from_lines.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.1.0/src/ramanchada2.egg-info/PKG-INFO` & `ramanchada2-0.1.1/src/ramanchada2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramanchada2
-Version: 0.1.0
+Version: 0.1.1
 Summary: Harmonising Raman Spectroscopy
 Home-page: https://github.com/h2020charisma/ramanchada2
 Author: IDEAconsult Ltd.
 Author-email: dev-charisma@ideaconsult.net
 License: MIT
 Keywords: Raman,spectroscopy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ramanchada2-0.1.0/src/ramanchada2.egg-info/SOURCES.txt` & `ramanchada2-0.1.1/src/ramanchada2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,28 @@
 src/ramanchada2.egg-info/SOURCES.txt
 src/ramanchada2.egg-info/dependency_links.txt
 src/ramanchada2.egg-info/requires.txt
 src/ramanchada2.egg-info/top_level.txt
 src/ramanchada2/auxiliary/__init__.py
 src/ramanchada2/auxiliary/spectra/__init__.py
 src/ramanchada2/auxiliary/spectra/datasets2/__init__.py
+src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/LED532_Probe_40msx3_1.txt
+src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NIST532_Probe_3000msx8_1.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_100msx2.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_5msx2.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/PST10_iR532_Probe_100_3000msx7.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0B10_iR532_Probe_100_60000msx2.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0N10_iR532_Probe_100_30000msx3.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0P10_iR532_Probe_100_60000msx2.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S1N10_iR532_Probe_100_22000msx2.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/Sil10_iR532_Probe_100_60000msx2.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/nCAL10_iR532_Probe_100_2500msx3.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/sCAL10_iR532_Probe_100_3200msx4.txt
+src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/LED785_Lens_1000x10_2.txt
+src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NIST785_Lens_80000x5_2.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP01.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP02.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP03.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP01_40000msx4.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP02_50000msx2.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP03_8000msx2.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP01_6000msx4.txt
@@ -46,32 +50,37 @@
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP03_8000msx2.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP01_6000msx4.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP02_20000msx2.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP03_8000msx2.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP01_4000msx4.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP02_15000msx2.txt
 src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP03_8000msx2.txt
+src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/NISTSRM2242aC_BW532_100x_800msx10.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_110ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_2000ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_25ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_800ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z050_100_2500msx5.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z100_100_50000ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z050_100_30000ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z100_100_22000ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z050_100_40000ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z100_100_28000ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z050_100_30000ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z100_100_20000ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z050_100_12000ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z100_100_6500ms.txt
+src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Visible_532nm_130ms_100X_2.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z050_100_9000ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z100_100_30000ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z050_100_20000ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z100_100_65000ms.txt
+src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/NIR_785nm_2000ms_100X_2.txt
+src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/NISTSRM2241_BW785_100x_25sx5.txt
+src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/Ne_785nm_x20_50ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z020_100_1300ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z050_100_3200ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z100_100_9000ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_12000ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_full.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z050_100_5500ms.txt
 src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z100_100_4700ms.txt
```

