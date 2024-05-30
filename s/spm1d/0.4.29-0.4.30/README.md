# Comparing `tmp/spm1d-0.4.29.tar.gz` & `tmp/spm1d-0.4.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spm1d-0.4.29.tar", last modified: Wed May 15 11:54:59 2024, max compression
+gzip compressed data, was "spm1d-0.4.30.tar", last modified: Thu May 30 07:02:30 2024, max compression
```

## Comparing `spm1d-0.4.29.tar` & `spm1d-0.4.30.tar`

### file list

```diff
@@ -1,499 +1,499 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.755671 spm1d-0.4.29/
--rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-05-15 11:54:50.000000 spm1d-0.4.29/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-15 11:54:50.000000 spm1d-0.4.29/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-15 11:54:59.755671 spm1d-0.4.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-15 11:54:50.000000 spm1d-0.4.29/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-15 11:54:59.755671 spm1d-0.4.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-15 11:54:50.000000 spm1d-0.4.29/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.667671 spm1d-0.4.29/spm1d/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10320 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.667671 spm1d-0.4.29/spm1d/data/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8227 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.691671 spm1d-0.4.29/spm1d/data/datafiles/
--rw-r--r--   0 runner    (1001) docker     (127)    29533 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/Besier2009kneeflexion.npz
--rw-r--r--   0 runner    (1001) docker     (127)   282313 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/Besier2009muscleforces.npz
--rw-r--r--   0 runner    (1001) docker     (127)    44022 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/Dorn2012.npz
--rw-r--r--   0 runner    (1001) docker     (127)    37636 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/Neptune1999kneekin.npz
--rw-r--r--   0 runner    (1001) docker     (127)    30624 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/Pataky2014cop.npz
--rw-r--r--   0 runner    (1001) docker     (127)    23431 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/ex_grf_means.npz
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/ex_grf_speeds.npy
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/ex_grf_speeds_cond.npy
--rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/ex_grf_subj000.npy
--rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/ex_grf_subj001.npy
--rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/ex_grf_subj002.npy
--rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/ex_grf_subj003.npy
--rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/ex_grf_subj004.npy
--rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/ex_grf_subj005.npy
--rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/ex_grf_subj006.npy
--rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/ex_grf_subj007.npy
--rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/ex_grf_subj008.npy
--rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/ex_grf_subj009.npy
--rw-r--r--   0 runner    (1001) docker     (127)    24320 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/ex_kinematics.npy
--rw-r--r--   0 runner    (1001) docker     (127)    29875 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/ex_kinematics_for_interpolation.npy
--rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/ex_sim_twolocalmax.npy
--rw-r--r--   0 runner    (1001) docker     (127)    11291 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/my_spmT.npz
--rw-r--r--   0 runner    (1001) docker     (127)    12770 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/my_spmTi.npz
--rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A1.npy
--rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A10.npy
--rw-r--r--   0 runner    (1001) docker     (127)    80880 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A11.npy
--rw-r--r--   0 runner    (1001) docker     (127)   808080 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A12.npy
--rw-r--r--   0 runner    (1001) docker     (127)   808080 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A13.npy
--rw-r--r--   0 runner    (1001) docker     (127)   808080 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A14.npy
--rw-r--r--   0 runner    (1001) docker     (127)   404080 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A15.npy
--rw-r--r--   0 runner    (1001) docker     (127)   404080 2024-05-15 11:54:50.000000 spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A16.npy
--rw-r--r--   0 runner    (1001) docker     (127)   404080 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A17.npy
--rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A2.npy
--rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A3.npy
--rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A4.npy
--rw-r--r--   0 runner    (1001) docker     (127)    32400 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A5.npy
--rw-r--r--   0 runner    (1001) docker     (127)   404080 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A6.npy
--rw-r--r--   0 runner    (1001) docker     (127)    16240 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A7.npy
--rw-r--r--   0 runner    (1001) docker     (127)    16240 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A8.npy
--rw-r--r--   0 runner    (1001) docker     (127)    16240 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A9.npy
--rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/random.npy
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/random_rough.npy
--rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/simscalar_datasetA.npy
--rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/simscalar_datasetB.npy
--rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/simscalar_datasetC.npy
--rw-r--r--   0 runner    (1001) docker     (127)    17000 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2_2x2.npz
--rw-r--r--   0 runner    (1001) docker     (127)    49960 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2_2x3.npz
--rw-r--r--   0 runner    (1001) docker     (127)    59848 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2_3x3.npz
--rw-r--r--   0 runner    (1001) docker     (127)   119176 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2_3x4.npz
--rw-r--r--   0 runner    (1001) docker     (127)    87040 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2_3x5.npz
--rw-r--r--   0 runner    (1001) docker     (127)   105992 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2_4x4.npz
--rw-r--r--   0 runner    (1001) docker     (127)   198280 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2_4x5.npz
--rw-r--r--   0 runner    (1001) docker     (127)    17000 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2nested_2x2.npz
--rw-r--r--   0 runner    (1001) docker     (127)    49960 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2nested_2x3.npz
--rw-r--r--   0 runner    (1001) docker     (127)    37600 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2nested_3x3.npz
--rw-r--r--   0 runner    (1001) docker     (127)    89512 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2nested_3x4.npz
--rw-r--r--   0 runner    (1001) docker     (127)   185920 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2nested_3x5.npz
--rw-r--r--   0 runner    (1001) docker     (127)    66440 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2nested_4x4.npz
--rw-r--r--   0 runner    (1001) docker     (127)   115880 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2nested_4x5.npz
--rw-r--r--   0 runner    (1001) docker     (127)    17332 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2onerm_2x2.npz
--rw-r--r--   0 runner    (1001) docker     (127)    45620 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2onerm_2x3.npz
--rw-r--r--   0 runner    (1001) docker     (127)    38132 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2onerm_3x3.npz
--rw-r--r--   0 runner    (1001) docker     (127)    90548 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2onerm_3x4.npz
--rw-r--r--   0 runner    (1001) docker     (127)   187892 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2onerm_3x5.npz
--rw-r--r--   0 runner    (1001) docker     (127)    67252 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2onerm_4x4.npz
--rw-r--r--   0 runner    (1001) docker     (127)   117172 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2onerm_4x5.npz
--rw-r--r--   0 runner    (1001) docker     (127)    23988 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2rm_2x2.npz
--rw-r--r--   0 runner    (1001) docker     (127)    60596 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2rm_2x3.npz
--rw-r--r--   0 runner    (1001) docker     (127)    38132 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2rm_3x3.npz
--rw-r--r--   0 runner    (1001) docker     (127)    90548 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2rm_3x4.npz
--rw-r--r--   0 runner    (1001) docker     (127)    88052 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2rm_3x5.npz
--rw-r--r--   0 runner    (1001) docker     (127)    67252 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2rm_4x4.npz
--rw-r--r--   0 runner    (1001) docker     (127)   133812 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2rm_4x5.npz
--rw-r--r--   0 runner    (1001) docker     (127)    33966 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova3_2x2x2.npz
--rw-r--r--   0 runner    (1001) docker     (127)   100526 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova3_2x3x4.npz
--rw-r--r--   0 runner    (1001) docker     (127)    53934 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova3nested_2x2x2.npz
--rw-r--r--   0 runner    (1001) docker     (127)   133806 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova3nested_2x4x2.npz
--rw-r--r--   0 runner    (1001) docker     (127)    34458 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova3onerm_2x2x2.npz
--rw-r--r--   0 runner    (1001) docker     (127)   101658 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova3onerm_2x3x4.npz
--rw-r--r--   0 runner    (1001) docker     (127)    34458 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova3rm_2x2x2.npz
--rw-r--r--   0 runner    (1001) docker     (127)   101658 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova3rm_2x3x4.npz
--rw-r--r--   0 runner    (1001) docker     (127)    34458 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova3tworm_2x2x2.npz
--rw-r--r--   0 runner    (1001) docker     (127)   101658 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova3tworm_2x3x4.npz
--rw-r--r--   0 runner    (1001) docker     (127)    98728 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/datafiles/weather.npz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.691671 spm1d-0.4.29/spm1d/data/mv0d/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/mv0d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/mv0d/cca.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/mv0d/hotellings1.py
--rw-r--r--   0 runner    (1001) docker     (127)    17491 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/mv0d/hotellings2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/mv0d/hotellings_paired.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/mv0d/manova1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.695671 spm1d-0.4.29/spm1d/data/mv1d/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/mv1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/mv1d/cca.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/mv1d/hotellings2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/mv1d/hotellings_paired.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/mv1d/manova1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.695671 spm1d-0.4.29/spm1d/data/uv0d/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/anova1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/anova1rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/anova2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/anova2nested.py
--rw-r--r--   0 runner    (1001) docker     (127)    11626 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/anova2onerm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/anova2rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/anova3.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/anova3nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/anova3onerm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/anova3rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/anova3tworm.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/ci1.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/ci2.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/cipaired.py
--rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/normality.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/regress.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/t1.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/t2.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/t2nonspher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv0d/tpaired.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.699671 spm1d-0.4.29/spm1d/data/uv1d/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv1d/anova1.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv1d/anova1rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv1d/anova2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv1d/anova2nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv1d/anova2onerm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv1d/anova2rm.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv1d/anova3.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv1d/anova3nested.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv1d/anova3onerm.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv1d/anova3rm.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv1d/anova3tworm.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv1d/normality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv1d/regress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv1d/t1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv1d/t2.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/data/uv1d/tpaired.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.663671 spm1d-0.4.29/spm1d/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.699671 spm1d-0.4.29/spm1d/examples/io/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.699671 spm1d-0.4.29/spm1d/examples/io/data/
--rw-r--r--   0 runner    (1001) docker     (127)    24424 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/io/data/ex_kinematics.mat
--rw-r--r--   0 runner    (1001) docker     (127)    24755 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/io/data/ex_kinematics.txt
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/io/ex_import_mat.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/io/ex_import_txt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.663671 spm1d-0.4.29/spm1d/examples/nonparam/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.707671 spm1d-0.4.29/spm1d/examples/nonparam/0d/
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova1.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova1rm.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova2.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova2nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova2onerm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova2rm.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova3.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova3nested.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova3onerm.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova3rm.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova3tworm.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_cca.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_ci_onesample.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_ci_pairedsample.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_ci_twosample.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_hotellings.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_hotellings2.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_hotellings_paired.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_manova1.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_regress.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_ttest.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_ttest2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_ttest2_standalone.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_ttest_paired.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_ttest_standalone.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.711671 spm1d-0.4.29/spm1d/examples/nonparam/1d/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova1.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova1rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova2nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova2onerm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova2rm.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova3.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova3nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova3onerm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova3rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova3tworm.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_cca.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_ci_onesample.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_ci_pairedsample.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_ci_twosample.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_hotellings.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_hotellings2.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_hotellings_paired.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_manova1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_ttest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_ttest2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_ttest2_circular.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_ttest_other_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_ttest_paired.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.715671 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova1rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova2nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova2onerm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova2rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova3nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova3onerm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova3rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova3tworm.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_cca.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_hotellings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_hotellings2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_hotellings_paired.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_manova1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_ttest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_ttest2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_ttest_paired.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.663671 spm1d-0.4.29/spm1d/examples/normality/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.715671 spm1d-0.4.29/spm1d/examples/normality/0d/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/0d/ex_anova1.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/0d/ex_anova1rm.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/0d/ex_anova2.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/0d/ex_anova2nested.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/0d/ex_anova2onerm.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/0d/ex_anova2rm.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/0d/ex_anova3.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/0d/ex_anova3nested.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/0d/ex_anova3onerm.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/0d/ex_anova3rm.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/0d/ex_anova3tworm.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/0d/ex_regress.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/0d/ex_ttest.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/0d/ex_ttest2.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/0d/ex_ttest_paired.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.719671 spm1d-0.4.29/spm1d/examples/normality/1d/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/1d/ex_anova1.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/1d/ex_anova1rm.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/1d/ex_anova2.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/1d/ex_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/1d/ex_ttest.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/1d/ex_ttest2.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/1d/ex_ttest_paired.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.719671 spm1d-0.4.29/spm1d/examples/normality/paper/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1897 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/paper/appendix_FigA1.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1759 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/paper/appendix_FigA2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1968 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/paper/appendix_FigA3.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1887 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/paper/appendix_FigA4.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1626 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/paper/appendix_FigA5.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1927 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/paper/appendix_FigA6.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1932 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/normality/paper/appendix_FigA7.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.719671 spm1d-0.4.29/spm1d/examples/processing/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.719671 spm1d-0.4.29/spm1d/examples/processing/data/
--rw-r--r--   0 runner    (1001) docker     (127)    29875 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/processing/data/ex_kinematics_for_interpolation.npy
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/processing/ex_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/processing/ex_smooth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.719671 spm1d-0.4.29/spm1d/examples/scipy/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/scipy/ex_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/scipy/ex_ttest_normality.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/scipy/ex_ttest_onesample.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/scipy/ex_ttest_paired.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/scipy/ex_ttest_twosample.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/scipy/ex_ttest_twosample_unequalvar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.727671 spm1d-0.4.29/spm1d/examples/stats0d/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_anova1.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_anova1rm.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_anova2.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_anova2nested.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_anova2onerm.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_anova2onermub.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_anova2rm.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_anova3.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_anova3nested.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_anova3onerm.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_anova3rm.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_anova3tworm.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_cca.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_ci_onesample.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_ci_onesample_standalone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_ci_pairedsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_ci_twosample.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_hotellings1.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_hotellings2.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_hotellings_paired.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_manova1.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_ttest_onesample.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_ttest_paired.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_ttest_twosample.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats0d/ex_ttest_twosample_unequalvar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.731671 spm1d-0.4.29/spm1d/examples/stats1d/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_anova1.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_anova1_circular_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_anova1_posthoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_anova1rm.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_anova2.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_anova2nested.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_anova2onerm.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_anova2rm.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_anova3.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_anova3nested.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_anova3onerm.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_anova3rm.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_anova3tworm.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_cca_Dorn2012.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_ci_onesample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_ci_onesample_standalone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_ci_pairedsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_ci_twosample.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_eqvartest.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_glm.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_hotellings2_Besier2009muscleforces.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_hotellings_paired_Neptune1999.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_hotellings_paired_Pataky2014.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_manova1_Dorn2012.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_ttest.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_ttest2.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_ttest_paired.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/ex_ttest_roi.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/rfx_0_means.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/rfx_1_level1.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d/rfx_2_level2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.735671 spm1d-0.4.29/spm1d/examples/stats1d_roi/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova1rm.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova2.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova2nested.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova2onerm.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova2rm.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova3.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova3nested.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova3onerm.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova3rm.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova3tworm.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_cca_Dorn2012.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_glm.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_hotellings2_Besier2009muscleforces.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_hotellings_paired_Neptune1999.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_hotellings_paired_Pataky2014.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_manova1_Dorn2012.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_regression_directional.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_ttest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_ttest2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_ttest_paired.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.735671 spm1d-0.4.29/spm1d/examples/stats2d/
--rw-r--r--   0 runner    (1001) docker     (127)   307328 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats2d/data2d.npy
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/stats2d/ex2d_ttest2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.735671 spm1d-0.4.29/spm1d/examples/summarystats/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/summarystats/ex_plot_errorcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/summarystats/ex_plot_meansd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.735671 spm1d-0.4.29/spm1d/examples/validation/
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/examples/validation/val_eqvartest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.739671 spm1d-0.4.29/spm1d/rft1d/
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.663671 spm1d-0.4.29/spm1d/rft1d/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.739671 spm1d-0.4.29/spm1d/rft1d/data/weather/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/data/weather/README.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    31982 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/data/weather/daily.m
--rwxr-xr-x   0 runner    (1001) docker     (127)    44170 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/data/weather/daily.mat
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17791 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/distributions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.747671 spm1d-0.4.29/spm1d/rft1d/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.747671 spm1d-0.4.29/spm1d/rft1d/examples/paper/
--rw-r--r--   0 runner    (1001) docker     (127)    39888 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/paper/all_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/paper/fig01_fields1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/paper/fig02_EC_HC.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/paper/fig03_EC.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/paper/fig04_fields1d_broken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/paper/fig05_EC_broken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/paper/fig06_sf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/paper/fig07_bonf_sf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/paper/fig08_bonf_isf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/paper/fig09_val_maxima.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/paper/fig10_upcrossing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/paper/fig11_val_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/paper/fig12_val_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/paper/fig13_weather_0_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/paper/fig14_fwhm_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/paper/fig15_weather_1_rft.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/paper/fig16_weather_2_wrapped.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/paper/fig17_weather_3_nonparam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/random_fields_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/random_fields_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/random_fields_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/random_fields_broken_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/random_fields_broken_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/random_fields_broken_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/smoothness_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/smoothness_estimation_broken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_broken_0_gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_broken_1_t.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_broken_2_F.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_broken_3_T2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_broken_4_X2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_conj_0_gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_conj_1_t.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_conj_2_F.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_conj_3_T2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_conj_4_X2.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_max_0_gaussian_0d.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_max_0_gaussian_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_max_1_onesample_t_0d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_max_1_onesample_t_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_max_2_twosample_t_0d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_max_2_twosample_t_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_max_3_regress_0d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_max_3_regress_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_max_4_anova1_0d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_max_4_anova1_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_max_5_onesample_T2_0d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_max_5_onesample_T2_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_max_6_twosample_T2_0d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_max_6_twosample_T2_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_max_7_cca_0d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_max_7_cca_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_max_8_manova1_0d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_max_8_manova1_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_upx_0_gauss_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_upx_0_gauss_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_upx_1_t_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_upx_1_t_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_upx_2_F_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_upx_2_F_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_upx_3_T2_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_upx_3_T2_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_upx_4_X2_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/val_upx_4_X2_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/weather_0_plotdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/weather_1_rft.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/weather_2_nonparam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/examples/weather_3_wrapped.py
--rw-r--r--   0 runner    (1001) docker     (127)    23509 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/geom.py
--rw-r--r--   0 runner    (1001) docker     (127)    21899 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/prob.py
--rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/rft1d/random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.751671 spm1d-0.4.29/spm1d/stats/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/_datachecks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/_mvbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/_reml.py
--rw-r--r--   0 runner    (1001) docker     (127)    21861 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/_spm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/_spmlist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.751671 spm1d-0.4.29/spm1d/stats/anova/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/anova/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25245 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/anova/designs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/anova/factors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/anova/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    15317 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/anova/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.751671 spm1d-0.4.29/spm1d/stats/c/
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/cca.py
--rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/ci.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/hotellings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/manova.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.751671 spm1d-0.4.29/spm1d/stats/nonparam/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/nonparam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12514 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/nonparam/_snpm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/nonparam/_snpmlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/nonparam/calculators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/nonparam/ci.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/nonparam/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    17874 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/nonparam/permuters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/nonparam/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.755671 spm1d-0.4.29/spm1d/stats/normality/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/normality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/normality/k2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/normality/sw.py
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/t.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/stats/var.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-15 11:54:51.000000 spm1d-0.4.29/spm1d/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.755671 spm1d-0.4.29/spm1d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-15 11:54:59.000000 spm1d-0.4.29/spm1d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18210 2024-05-15 11:54:59.000000 spm1d-0.4.29/spm1d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:54:59.000000 spm1d-0.4.29/spm1d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 11:54:59.000000 spm1d-0.4.29/spm1d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 11:54:59.000000 spm1d-0.4.29/spm1d.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:54:59.755671 spm1d-0.4.29/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10351 2024-05-15 11:54:51.000000 spm1d-0.4.29/tests/test_0d.py
--rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-05-15 11:54:51.000000 spm1d-0.4.29/tests/test_0d_c.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-15 11:54:51.000000 spm1d-0.4.29/tests/test_0d_mv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-15 11:54:51.000000 spm1d-0.4.29/tests/test_0d_mv_c.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.816414 spm1d-0.4.30/
+-rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-05-30 07:02:22.000000 spm1d-0.4.30/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-30 07:02:22.000000 spm1d-0.4.30/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-30 07:02:30.816414 spm1d-0.4.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-30 07:02:22.000000 spm1d-0.4.30/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-30 07:02:30.816414 spm1d-0.4.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-30 07:02:22.000000 spm1d-0.4.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.716414 spm1d-0.4.30/spm1d/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10320 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.720414 spm1d-0.4.30/spm1d/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8227 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.744414 spm1d-0.4.30/spm1d/data/datafiles/
+-rw-r--r--   0 runner    (1001) docker     (127)    29533 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/Besier2009kneeflexion.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   282313 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/Besier2009muscleforces.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    44022 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/Dorn2012.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    37636 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/Neptune1999kneekin.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    30624 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/Pataky2014cop.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    23431 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/ex_grf_means.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/ex_grf_speeds.npy
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/ex_grf_speeds_cond.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/ex_grf_subj000.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/ex_grf_subj001.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/ex_grf_subj002.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/ex_grf_subj003.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/ex_grf_subj004.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/ex_grf_subj005.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/ex_grf_subj006.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/ex_grf_subj007.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/ex_grf_subj008.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/ex_grf_subj009.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    24320 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/ex_kinematics.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    29875 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/ex_kinematics_for_interpolation.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/ex_sim_twolocalmax.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    11291 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/my_spmT.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    12770 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/my_spmTi.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A1.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A10.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    80880 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A11.npy
+-rw-r--r--   0 runner    (1001) docker     (127)   808080 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A12.npy
+-rw-r--r--   0 runner    (1001) docker     (127)   808080 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A13.npy
+-rw-r--r--   0 runner    (1001) docker     (127)   808080 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A14.npy
+-rw-r--r--   0 runner    (1001) docker     (127)   404080 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A15.npy
+-rw-r--r--   0 runner    (1001) docker     (127)   404080 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A16.npy
+-rw-r--r--   0 runner    (1001) docker     (127)   404080 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A17.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A2.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A3.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A4.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    32400 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A5.npy
+-rw-r--r--   0 runner    (1001) docker     (127)   404080 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A6.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    16240 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A7.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    16240 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A8.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    16240 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A9.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/random.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/random_rough.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/simscalar_datasetA.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/simscalar_datasetB.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/simscalar_datasetC.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    17000 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2_2x2.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    49960 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2_2x3.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    59848 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2_3x3.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   119176 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2_3x4.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    87040 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2_3x5.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   105992 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2_4x4.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   198280 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2_4x5.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    17000 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2nested_2x2.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    49960 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2nested_2x3.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    37600 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2nested_3x3.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    89512 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2nested_3x4.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   185920 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2nested_3x5.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    66440 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2nested_4x4.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   115880 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2nested_4x5.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    17332 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2onerm_2x2.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    45620 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2onerm_2x3.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    38132 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2onerm_3x3.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    90548 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2onerm_3x4.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   187892 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2onerm_3x5.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    67252 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2onerm_4x4.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   117172 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2onerm_4x5.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    23988 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2rm_2x2.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    60596 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2rm_2x3.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    38132 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2rm_3x3.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    90548 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2rm_3x4.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    88052 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2rm_3x5.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    67252 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2rm_4x4.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   133812 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2rm_4x5.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    33966 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova3_2x2x2.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   100526 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova3_2x3x4.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    53934 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova3nested_2x2x2.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   133806 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova3nested_2x4x2.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    34458 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova3onerm_2x2x2.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   101658 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova3onerm_2x3x4.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    34458 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova3rm_2x2x2.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   101658 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova3rm_2x3x4.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    34458 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova3tworm_2x2x2.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   101658 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova3tworm_2x3x4.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    98728 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/datafiles/weather.npz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.748414 spm1d-0.4.30/spm1d/data/mv0d/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/mv0d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/mv0d/cca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/mv0d/hotellings1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17491 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/mv0d/hotellings2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/mv0d/hotellings_paired.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/mv0d/manova1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.748414 spm1d-0.4.30/spm1d/data/mv1d/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/mv1d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/mv1d/cca.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/mv1d/hotellings2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/mv1d/hotellings_paired.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/mv1d/manova1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.752414 spm1d-0.4.30/spm1d/data/uv0d/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/anova1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/anova1rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/anova2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/anova2nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11626 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/anova2onerm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/anova2rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/anova3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/anova3nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/anova3onerm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/anova3rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/anova3tworm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/ci1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/ci2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/cipaired.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/normality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/regress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/t1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/t2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/t2nonspher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv0d/tpaired.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.756414 spm1d-0.4.30/spm1d/data/uv1d/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv1d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv1d/anova1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv1d/anova1rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv1d/anova2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv1d/anova2nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv1d/anova2onerm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv1d/anova2rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv1d/anova3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv1d/anova3nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv1d/anova3onerm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv1d/anova3rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv1d/anova3tworm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv1d/normality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv1d/regress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv1d/t1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv1d/t2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/data/uv1d/tpaired.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.716414 spm1d-0.4.30/spm1d/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.756414 spm1d-0.4.30/spm1d/examples/io/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.756414 spm1d-0.4.30/spm1d/examples/io/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    24424 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/io/data/ex_kinematics.mat
+-rw-r--r--   0 runner    (1001) docker     (127)    24755 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/io/data/ex_kinematics.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/io/ex_import_mat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/io/ex_import_txt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.712414 spm1d-0.4.30/spm1d/examples/nonparam/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.760414 spm1d-0.4.30/spm1d/examples/nonparam/0d/
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova1rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova2nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova2onerm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova2rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova3nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova3onerm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova3rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova3tworm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_cca.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_ci_onesample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_ci_pairedsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_ci_twosample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_hotellings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_hotellings2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_hotellings_paired.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_manova1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_regress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_ttest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_ttest2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_ttest2_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_ttest_paired.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_ttest_standalone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.764414 spm1d-0.4.30/spm1d/examples/nonparam/1d/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova1rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova2nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova2onerm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova2rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova3nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova3onerm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova3rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova3tworm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_cca.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_ci_onesample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_ci_pairedsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_ci_twosample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_hotellings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_hotellings2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_hotellings_paired.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_manova1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_ttest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_ttest2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_ttest2_circular.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_ttest_other_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_ttest_paired.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.768414 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova1rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova2nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova2onerm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova2rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova3nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova3onerm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova3rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova3tworm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_cca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_hotellings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_hotellings2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_hotellings_paired.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_manova1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_ttest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_ttest2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_ttest_paired.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.712414 spm1d-0.4.30/spm1d/examples/normality/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.772414 spm1d-0.4.30/spm1d/examples/normality/0d/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/0d/ex_anova1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/0d/ex_anova1rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/0d/ex_anova2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/0d/ex_anova2nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/0d/ex_anova2onerm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/0d/ex_anova2rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/0d/ex_anova3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/0d/ex_anova3nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/0d/ex_anova3onerm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/0d/ex_anova3rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/0d/ex_anova3tworm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/0d/ex_regress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/0d/ex_ttest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/0d/ex_ttest2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/0d/ex_ttest_paired.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.772414 spm1d-0.4.30/spm1d/examples/normality/1d/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/1d/ex_anova1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/1d/ex_anova1rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/1d/ex_anova2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/1d/ex_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/1d/ex_ttest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/1d/ex_ttest2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/1d/ex_ttest_paired.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.776414 spm1d-0.4.30/spm1d/examples/normality/paper/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1897 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/paper/appendix_FigA1.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1759 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/paper/appendix_FigA2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1968 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/paper/appendix_FigA3.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1887 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/paper/appendix_FigA4.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1626 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/paper/appendix_FigA5.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1927 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/paper/appendix_FigA6.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1932 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/normality/paper/appendix_FigA7.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.776414 spm1d-0.4.30/spm1d/examples/processing/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.776414 spm1d-0.4.30/spm1d/examples/processing/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    29875 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/processing/data/ex_kinematics_for_interpolation.npy
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/processing/ex_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/processing/ex_smooth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.776414 spm1d-0.4.30/spm1d/examples/scipy/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/scipy/ex_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/scipy/ex_ttest_normality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/scipy/ex_ttest_onesample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/scipy/ex_ttest_paired.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/scipy/ex_ttest_twosample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/scipy/ex_ttest_twosample_unequalvar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.780414 spm1d-0.4.30/spm1d/examples/stats0d/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_anova1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_anova1rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_anova2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_anova2nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_anova2onerm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_anova2onermub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_anova2rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_anova3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_anova3nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_anova3onerm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_anova3rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_anova3tworm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_cca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_ci_onesample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_ci_onesample_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_ci_pairedsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_ci_twosample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_hotellings1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_hotellings2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_hotellings_paired.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_manova1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_ttest_onesample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_ttest_paired.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_ttest_twosample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats0d/ex_ttest_twosample_unequalvar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.788414 spm1d-0.4.30/spm1d/examples/stats1d/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_anova1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_anova1_circular_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_anova1_posthoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_anova1rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_anova2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_anova2nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_anova2onerm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_anova2rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_anova3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_anova3nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_anova3onerm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_anova3rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_anova3tworm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_cca_Dorn2012.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_ci_onesample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_ci_onesample_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_ci_pairedsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_ci_twosample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_eqvartest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_glm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_hotellings2_Besier2009muscleforces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_hotellings_paired_Neptune1999.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_hotellings_paired_Pataky2014.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_manova1_Dorn2012.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_ttest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_ttest2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_ttest_paired.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/ex_ttest_roi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/rfx_0_means.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/rfx_1_level1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d/rfx_2_level2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.792414 spm1d-0.4.30/spm1d/examples/stats1d_roi/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova1rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova2nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova2onerm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova2rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova3nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova3onerm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova3rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova3tworm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_cca_Dorn2012.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_glm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_hotellings2_Besier2009muscleforces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_hotellings_paired_Neptune1999.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_hotellings_paired_Pataky2014.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_manova1_Dorn2012.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_regression_directional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_ttest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_ttest2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_ttest_paired.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.792414 spm1d-0.4.30/spm1d/examples/stats2d/
+-rw-r--r--   0 runner    (1001) docker     (127)   307328 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats2d/data2d.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/stats2d/ex2d_ttest2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.792414 spm1d-0.4.30/spm1d/examples/summarystats/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/summarystats/ex_plot_errorcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/summarystats/ex_plot_meansd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.792414 spm1d-0.4.30/spm1d/examples/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/examples/validation/val_eqvartest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.792414 spm1d-0.4.30/spm1d/rft1d/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.716414 spm1d-0.4.30/spm1d/rft1d/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.796414 spm1d-0.4.30/spm1d/rft1d/data/weather/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/data/weather/README.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31982 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/data/weather/daily.m
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44170 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/data/weather/daily.mat
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17791 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/distributions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.804414 spm1d-0.4.30/spm1d/rft1d/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.808414 spm1d-0.4.30/spm1d/rft1d/examples/paper/
+-rw-r--r--   0 runner    (1001) docker     (127)    39888 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/paper/all_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/paper/fig01_fields1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/paper/fig02_EC_HC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/paper/fig03_EC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/paper/fig04_fields1d_broken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/paper/fig05_EC_broken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/paper/fig06_sf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/paper/fig07_bonf_sf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/paper/fig08_bonf_isf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/paper/fig09_val_maxima.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/paper/fig10_upcrossing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/paper/fig11_val_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/paper/fig12_val_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/paper/fig13_weather_0_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/paper/fig14_fwhm_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/paper/fig15_weather_1_rft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/paper/fig16_weather_2_wrapped.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/paper/fig17_weather_3_nonparam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/random_fields_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/random_fields_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/random_fields_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/random_fields_broken_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/random_fields_broken_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/random_fields_broken_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/smoothness_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/smoothness_estimation_broken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_broken_0_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_broken_1_t.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_broken_2_F.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_broken_3_T2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_broken_4_X2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_conj_0_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_conj_1_t.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_conj_2_F.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_conj_3_T2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_conj_4_X2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_max_0_gaussian_0d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_max_0_gaussian_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_max_1_onesample_t_0d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_max_1_onesample_t_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_max_2_twosample_t_0d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_max_2_twosample_t_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_max_3_regress_0d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_max_3_regress_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_max_4_anova1_0d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_max_4_anova1_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_max_5_onesample_T2_0d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_max_5_onesample_T2_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_max_6_twosample_T2_0d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_max_6_twosample_T2_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_max_7_cca_0d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_max_7_cca_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_max_8_manova1_0d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_max_8_manova1_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_upx_0_gauss_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_upx_0_gauss_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_upx_1_t_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_upx_1_t_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_upx_2_F_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_upx_2_F_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_upx_3_T2_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_upx_3_T2_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_upx_4_X2_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/val_upx_4_X2_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/weather_0_plotdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/weather_1_rft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/weather_2_nonparam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/examples/weather_3_wrapped.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23509 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21899 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/prob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/rft1d/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.812414 spm1d-0.4.30/spm1d/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/_datachecks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/_mvbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/_reml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21861 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/_spm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/_spmlist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.812414 spm1d-0.4.30/spm1d/stats/anova/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/anova/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25245 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/anova/designs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/anova/factors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/anova/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15317 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/anova/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.812414 spm1d-0.4.30/spm1d/stats/c/
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/cca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/hotellings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/manova.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.816414 spm1d-0.4.30/spm1d/stats/nonparam/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/nonparam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12514 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/nonparam/_snpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/nonparam/_snpmlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/nonparam/calculators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/nonparam/ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/nonparam/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17874 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/nonparam/permuters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/nonparam/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.816414 spm1d-0.4.30/spm1d/stats/normality/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/normality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/normality/k2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/normality/sw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/t.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/stats/var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-30 07:02:22.000000 spm1d-0.4.30/spm1d/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.816414 spm1d-0.4.30/spm1d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-30 07:02:30.000000 spm1d-0.4.30/spm1d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18210 2024-05-30 07:02:30.000000 spm1d-0.4.30/spm1d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 07:02:30.000000 spm1d-0.4.30/spm1d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 07:02:30.000000 spm1d-0.4.30/spm1d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 07:02:30.000000 spm1d-0.4.30/spm1d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:02:30.816414 spm1d-0.4.30/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10351 2024-05-30 07:02:22.000000 spm1d-0.4.30/tests/test_0d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-05-30 07:02:22.000000 spm1d-0.4.30/tests/test_0d_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-30 07:02:22.000000 spm1d-0.4.30/tests/test_0d_mv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-30 07:02:22.000000 spm1d-0.4.30/tests/test_0d_mv_c.py
```

### Comparing `spm1d-0.4.29/LICENSE.txt` & `spm1d-0.4.30/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/PKG-INFO` & `spm1d-0.4.30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spm1d
-Version: 0.4.29
+Version: 0.4.30
 Summary: One-Dimensional Statistical Parametric Mapping
 Home-page: https://github.com/0todd0000/spm1d
 Download-URL: https://github.com/0todd0000/spm1d/archive/master.zip
 Author: Todd Pataky
 Author-email: spm1d.mail@gmail.com
 Keywords: statistics,time series analysis
 License-File: LICENSE.txt
```

### Comparing `spm1d-0.4.29/README.md` & `spm1d-0.4.30/README.md`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/setup.py` & `spm1d-0.4.30/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 spm1d uses <b>Random Field Theory</b> expectations regarding the behavior of smooth,
 one-dimensional Gaussian fields to make statistical inferences regarding a set of
 one-dimensional measurements.
 '''
 
 setup(
 	name             = 'spm1d',
-	version          = '0.4.29',
+	version          = '0.4.30',
 	description      = 'One-Dimensional Statistical Parametric Mapping',
 	author           = 'Todd Pataky',
 	author_email     = 'spm1d.mail@gmail.com',
 	url              = 'https://github.com/0todd0000/spm1d',
 	download_url     = 'https://github.com/0todd0000/spm1d/archive/master.zip',
 	packages         = ['spm1d'],
 	package_data     = {'spm1d' : ['examples/*.*', 'data/*.*'] },
```

### Comparing `spm1d-0.4.29/spm1d/__init__.py` & `spm1d-0.4.30/spm1d/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 probabilities in Python, Journal of Statistical Software, in press.
 
 
 Copyright (C) 2024  Todd Pataky
 '''
 
 
-__version__ = '0.4.29'  # 2024-05-15
+__version__ = '0.4.30'  # 2024-05-30
 
 
 __all__ = ['data', 'io', 'plot', 'rft1d', 'stats', 'util']
 
 from . import data
 from . import io
 from . import plot
```

### Comparing `spm1d-0.4.29/spm1d/_plot.py` & `spm1d-0.4.30/spm1d/_plot.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/_base.py` & `spm1d-0.4.30/spm1d/data/_base.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/Besier2009kneeflexion.npz` & `spm1d-0.4.30/spm1d/data/datafiles/Besier2009kneeflexion.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/Besier2009muscleforces.npz` & `spm1d-0.4.30/spm1d/data/datafiles/Besier2009muscleforces.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/Dorn2012.npz` & `spm1d-0.4.30/spm1d/data/datafiles/Dorn2012.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/Neptune1999kneekin.npz` & `spm1d-0.4.30/spm1d/data/datafiles/Neptune1999kneekin.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/Pataky2014cop.npz` & `spm1d-0.4.30/spm1d/data/datafiles/Pataky2014cop.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/ex_grf_means.npz` & `spm1d-0.4.30/spm1d/data/datafiles/ex_grf_means.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/ex_grf_speeds.npy` & `spm1d-0.4.30/spm1d/data/datafiles/ex_grf_speeds.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/ex_grf_speeds_cond.npy` & `spm1d-0.4.30/spm1d/data/datafiles/ex_grf_speeds_cond.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/ex_grf_subj000.npy` & `spm1d-0.4.30/spm1d/data/datafiles/ex_grf_subj000.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/ex_grf_subj001.npy` & `spm1d-0.4.30/spm1d/data/datafiles/ex_grf_subj001.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/ex_grf_subj002.npy` & `spm1d-0.4.30/spm1d/data/datafiles/ex_grf_subj002.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/ex_grf_subj003.npy` & `spm1d-0.4.30/spm1d/data/datafiles/ex_grf_subj003.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/ex_grf_subj004.npy` & `spm1d-0.4.30/spm1d/data/datafiles/ex_grf_subj004.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/ex_grf_subj005.npy` & `spm1d-0.4.30/spm1d/data/datafiles/ex_grf_subj005.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/ex_grf_subj006.npy` & `spm1d-0.4.30/spm1d/data/datafiles/ex_grf_subj006.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/ex_grf_subj007.npy` & `spm1d-0.4.30/spm1d/data/datafiles/ex_grf_subj007.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/ex_grf_subj008.npy` & `spm1d-0.4.30/spm1d/data/datafiles/ex_grf_subj008.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/ex_grf_subj009.npy` & `spm1d-0.4.30/spm1d/data/datafiles/ex_grf_subj009.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/ex_kinematics.npy` & `spm1d-0.4.30/spm1d/data/datafiles/ex_kinematics.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/ex_kinematics_for_interpolation.npy` & `spm1d-0.4.30/spm1d/data/datafiles/ex_kinematics_for_interpolation.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/ex_sim_twolocalmax.npy` & `spm1d-0.4.30/spm1d/data/datafiles/ex_sim_twolocalmax.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/my_spmT.npz` & `spm1d-0.4.30/spm1d/data/datafiles/my_spmT.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/my_spmTi.npz` & `spm1d-0.4.30/spm1d/data/datafiles/my_spmTi.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A1.npy` & `spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A1.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A10.npy` & `spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A10.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A11.npy` & `spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A11.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A12.npy` & `spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A12.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A13.npy` & `spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A13.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A14.npy` & `spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A14.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A15.npy` & `spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A15.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A16.npy` & `spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A16.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A17.npy` & `spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A17.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A2.npy` & `spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A2.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A3.npy` & `spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A3.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A4.npy` & `spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A4.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A5.npy` & `spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A5.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A6.npy` & `spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A6.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A7.npy` & `spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A7.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A8.npy` & `spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A8.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/normality_dataset_A9.npy` & `spm1d-0.4.30/spm1d/data/datafiles/normality_dataset_A9.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/random.npy` & `spm1d-0.4.30/spm1d/data/datafiles/random.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/random_rough.npy` & `spm1d-0.4.30/spm1d/data/datafiles/random_rough.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/simscalar_datasetA.npy` & `spm1d-0.4.30/spm1d/data/datafiles/simscalar_datasetA.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/simscalar_datasetB.npy` & `spm1d-0.4.30/spm1d/data/datafiles/simscalar_datasetB.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/simscalar_datasetC.npy` & `spm1d-0.4.30/spm1d/data/datafiles/simscalar_datasetC.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2_2x2.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2_2x2.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2_2x3.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2_2x3.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2_3x3.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2_3x3.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2_3x4.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2_3x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2_3x5.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2_3x5.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2_4x4.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2_4x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2_4x5.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2_4x5.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2nested_2x2.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2nested_2x2.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2nested_2x3.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2nested_2x3.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2nested_3x3.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2nested_3x3.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2nested_3x4.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2nested_3x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2nested_3x5.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2nested_3x5.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2nested_4x4.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2nested_4x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2nested_4x5.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2nested_4x5.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2onerm_2x2.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2onerm_2x2.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2onerm_2x3.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2onerm_2x3.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2onerm_3x3.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2onerm_3x3.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2onerm_3x4.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2onerm_3x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2onerm_3x5.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2onerm_3x5.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2onerm_4x4.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2onerm_4x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2onerm_4x5.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2onerm_4x5.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2rm_2x2.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2rm_2x2.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2rm_2x3.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2rm_2x3.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2rm_3x3.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2rm_3x3.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2rm_3x4.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2rm_3x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2rm_3x5.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2rm_3x5.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2rm_4x4.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2rm_4x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova2rm_4x5.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova2rm_4x5.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova3_2x2x2.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova3_2x2x2.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova3_2x3x4.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova3_2x3x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova3nested_2x2x2.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova3nested_2x2x2.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova3nested_2x4x2.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova3nested_2x4x2.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova3onerm_2x2x2.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova3onerm_2x2x2.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova3onerm_2x3x4.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova3onerm_2x3x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova3rm_2x2x2.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova3rm_2x2x2.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova3rm_2x3x4.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova3rm_2x3x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova3tworm_2x2x2.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova3tworm_2x2x2.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/spm1d_anova3tworm_2x3x4.npz` & `spm1d-0.4.30/spm1d/data/datafiles/spm1d_anova3tworm_2x3x4.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/datafiles/weather.npz` & `spm1d-0.4.30/spm1d/data/datafiles/weather.npz`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/mv0d/cca.py` & `spm1d-0.4.30/spm1d/data/mv0d/cca.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/mv0d/hotellings1.py` & `spm1d-0.4.30/spm1d/data/mv0d/hotellings1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/mv0d/hotellings2.py` & `spm1d-0.4.30/spm1d/data/mv0d/hotellings2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/mv0d/hotellings_paired.py` & `spm1d-0.4.30/spm1d/data/mv0d/hotellings_paired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/mv0d/manova1.py` & `spm1d-0.4.30/spm1d/data/mv0d/manova1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/mv1d/cca.py` & `spm1d-0.4.30/spm1d/data/mv1d/cca.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/mv1d/hotellings2.py` & `spm1d-0.4.30/spm1d/data/mv1d/hotellings2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/mv1d/hotellings_paired.py` & `spm1d-0.4.30/spm1d/data/mv1d/hotellings_paired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/mv1d/manova1.py` & `spm1d-0.4.30/spm1d/data/mv1d/manova1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv0d/anova1.py` & `spm1d-0.4.30/spm1d/data/uv0d/anova1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv0d/anova1rm.py` & `spm1d-0.4.30/spm1d/data/uv0d/anova1rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv0d/anova2.py` & `spm1d-0.4.30/spm1d/data/uv0d/anova2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv0d/anova2nested.py` & `spm1d-0.4.30/spm1d/data/uv0d/anova2nested.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv0d/anova2onerm.py` & `spm1d-0.4.30/spm1d/data/uv0d/anova2onerm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv0d/anova2rm.py` & `spm1d-0.4.30/spm1d/data/uv0d/anova2rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv0d/anova3.py` & `spm1d-0.4.30/spm1d/data/uv0d/anova3.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv0d/anova3nested.py` & `spm1d-0.4.30/spm1d/data/uv0d/anova3nested.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv0d/anova3onerm.py` & `spm1d-0.4.30/spm1d/data/uv0d/anova3onerm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv0d/anova3rm.py` & `spm1d-0.4.30/spm1d/data/uv0d/anova3rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv0d/anova3tworm.py` & `spm1d-0.4.30/spm1d/data/uv0d/anova3tworm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv0d/ci1.py` & `spm1d-0.4.30/spm1d/data/uv0d/ci1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv0d/ci2.py` & `spm1d-0.4.30/spm1d/data/uv0d/ci2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv0d/cipaired.py` & `spm1d-0.4.30/spm1d/data/uv0d/cipaired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv0d/normality.py` & `spm1d-0.4.30/spm1d/data/uv0d/normality.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv0d/regress.py` & `spm1d-0.4.30/spm1d/data/uv0d/regress.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv0d/t1.py` & `spm1d-0.4.30/spm1d/data/uv0d/t1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv0d/t2.py` & `spm1d-0.4.30/spm1d/data/uv0d/t2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv0d/t2nonspher.py` & `spm1d-0.4.30/spm1d/data/uv0d/t2nonspher.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv0d/tpaired.py` & `spm1d-0.4.30/spm1d/data/uv0d/tpaired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv1d/anova1.py` & `spm1d-0.4.30/spm1d/data/uv1d/anova1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv1d/anova1rm.py` & `spm1d-0.4.30/spm1d/data/uv1d/anova1rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv1d/anova2.py` & `spm1d-0.4.30/spm1d/data/uv1d/anova2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv1d/anova2nested.py` & `spm1d-0.4.30/spm1d/data/uv1d/anova2nested.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv1d/anova2onerm.py` & `spm1d-0.4.30/spm1d/data/uv1d/anova2onerm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv1d/anova2rm.py` & `spm1d-0.4.30/spm1d/data/uv1d/anova2rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv1d/anova3.py` & `spm1d-0.4.30/spm1d/data/uv1d/anova3.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv1d/anova3nested.py` & `spm1d-0.4.30/spm1d/data/uv1d/anova3nested.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv1d/anova3onerm.py` & `spm1d-0.4.30/spm1d/data/uv1d/anova3onerm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv1d/anova3rm.py` & `spm1d-0.4.30/spm1d/data/uv1d/anova3rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv1d/anova3tworm.py` & `spm1d-0.4.30/spm1d/data/uv1d/anova3tworm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv1d/normality.py` & `spm1d-0.4.30/spm1d/data/uv1d/normality.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv1d/regress.py` & `spm1d-0.4.30/spm1d/data/uv1d/regress.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv1d/t1.py` & `spm1d-0.4.30/spm1d/data/uv1d/t1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv1d/t2.py` & `spm1d-0.4.30/spm1d/data/uv1d/t2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/data/uv1d/tpaired.py` & `spm1d-0.4.30/spm1d/data/uv1d/tpaired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/io/data/ex_kinematics.mat` & `spm1d-0.4.30/spm1d/examples/io/data/ex_kinematics.mat`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/io/data/ex_kinematics.txt` & `spm1d-0.4.30/spm1d/examples/io/data/ex_kinematics.txt`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova1.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova1rm.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova1rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova2.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova2nested.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova2nested.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova2onerm.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova2onerm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova2rm.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova2rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova3.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova3.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova3nested.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova3nested.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova3onerm.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova3onerm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova3rm.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova3rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_anova3tworm.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_anova3tworm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_cca.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_cca.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_ci_onesample.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_ci_onesample.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_ci_pairedsample.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_ci_pairedsample.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_ci_twosample.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_ci_twosample.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_hotellings.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_hotellings.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_hotellings2.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_hotellings2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_hotellings_paired.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_hotellings_paired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_manova1.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_manova1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_regress.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_regress.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_ttest.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_ttest.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_ttest2.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_ttest2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_ttest2_standalone.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_ttest2_standalone.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_ttest_paired.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_ttest_paired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/0d/ex_ttest_standalone.py` & `spm1d-0.4.30/spm1d/examples/nonparam/0d/ex_ttest_standalone.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova1.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova1rm.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova1rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova2.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova2nested.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova2nested.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova2onerm.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova2onerm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova2rm.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova2rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova3.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova3.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova3nested.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova3nested.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova3onerm.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova3onerm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova3rm.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova3rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_anova3tworm.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_anova3tworm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_cca.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_cca.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_ci_onesample.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_ci_onesample.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_ci_pairedsample.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_ci_pairedsample.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_ci_twosample.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_ci_twosample.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_hotellings.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_hotellings.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_hotellings2.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_hotellings2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_hotellings_paired.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_hotellings_paired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_manova1.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_manova1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_regression.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_regression.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_ttest.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_ttest.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_ttest2.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_ttest2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_ttest2_circular.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_ttest2_circular.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_ttest_other_metrics.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_ttest_other_metrics.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/ex_ttest_paired.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/ex_ttest_paired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova1.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova1rm.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova1rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova2.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova2nested.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova2nested.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova2onerm.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova2onerm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova2rm.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova2rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova3.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova3.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova3nested.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova3nested.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova3onerm.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova3onerm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova3rm.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova3rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_anova3tworm.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_anova3tworm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_cca.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_cca.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_hotellings.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_hotellings.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_hotellings2.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_hotellings2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_hotellings_paired.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_hotellings_paired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_manova1.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_manova1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_regression.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_regression.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_ttest.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_ttest.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_ttest2.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_ttest2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/nonparam/1d/roi/ex_ttest_paired.py` & `spm1d-0.4.30/spm1d/examples/nonparam/1d/roi/ex_ttest_paired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/normality/0d/ex_ttest.py` & `spm1d-0.4.30/spm1d/examples/normality/0d/ex_ttest.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/normality/0d/ex_ttest2.py` & `spm1d-0.4.30/spm1d/examples/normality/0d/ex_ttest2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/normality/1d/ex_anova1.py` & `spm1d-0.4.30/spm1d/examples/normality/1d/ex_anova1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/normality/1d/ex_anova1rm.py` & `spm1d-0.4.30/spm1d/examples/normality/1d/ex_anova1rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/normality/1d/ex_anova2.py` & `spm1d-0.4.30/spm1d/examples/normality/1d/ex_anova2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/normality/1d/ex_regression.py` & `spm1d-0.4.30/spm1d/examples/normality/1d/ex_regression.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/normality/1d/ex_ttest.py` & `spm1d-0.4.30/spm1d/examples/normality/1d/ex_ttest.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/normality/1d/ex_ttest2.py` & `spm1d-0.4.30/spm1d/examples/normality/1d/ex_ttest2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/normality/1d/ex_ttest_paired.py` & `spm1d-0.4.30/spm1d/examples/normality/1d/ex_ttest_paired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/normality/paper/appendix_FigA1.py` & `spm1d-0.4.30/spm1d/examples/normality/paper/appendix_FigA1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/normality/paper/appendix_FigA2.py` & `spm1d-0.4.30/spm1d/examples/normality/paper/appendix_FigA2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/normality/paper/appendix_FigA3.py` & `spm1d-0.4.30/spm1d/examples/normality/paper/appendix_FigA3.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/normality/paper/appendix_FigA4.py` & `spm1d-0.4.30/spm1d/examples/normality/paper/appendix_FigA4.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/normality/paper/appendix_FigA5.py` & `spm1d-0.4.30/spm1d/examples/normality/paper/appendix_FigA5.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/normality/paper/appendix_FigA6.py` & `spm1d-0.4.30/spm1d/examples/normality/paper/appendix_FigA6.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/normality/paper/appendix_FigA7.py` & `spm1d-0.4.30/spm1d/examples/normality/paper/appendix_FigA7.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/processing/data/ex_kinematics_for_interpolation.npy` & `spm1d-0.4.30/spm1d/examples/processing/data/ex_kinematics_for_interpolation.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/processing/ex_interpolate.py` & `spm1d-0.4.30/spm1d/examples/processing/ex_interpolate.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/processing/ex_smooth.py` & `spm1d-0.4.30/spm1d/examples/processing/ex_smooth.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/scipy/ex_regression.py` & `spm1d-0.4.30/spm1d/examples/scipy/ex_regression.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/scipy/ex_ttest_normality.py` & `spm1d-0.4.30/spm1d/examples/scipy/ex_ttest_normality.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/scipy/ex_ttest_onesample.py` & `spm1d-0.4.30/spm1d/examples/scipy/ex_ttest_onesample.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/scipy/ex_ttest_paired.py` & `spm1d-0.4.30/spm1d/examples/scipy/ex_ttest_paired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/scipy/ex_ttest_twosample.py` & `spm1d-0.4.30/spm1d/examples/scipy/ex_ttest_twosample.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/scipy/ex_ttest_twosample_unequalvar.py` & `spm1d-0.4.30/spm1d/examples/scipy/ex_ttest_twosample_unequalvar.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats0d/ex_anova2.py` & `spm1d-0.4.30/spm1d/examples/stats0d/ex_anova2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats0d/ex_anova2onerm.py` & `spm1d-0.4.30/spm1d/examples/stats0d/ex_anova2onerm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats0d/ex_anova2rm.py` & `spm1d-0.4.30/spm1d/examples/stats0d/ex_anova2rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats0d/ex_ci_onesample.py` & `spm1d-0.4.30/spm1d/examples/stats0d/ex_ci_onesample.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats0d/ex_ci_onesample_standalone.py` & `spm1d-0.4.30/spm1d/examples/stats0d/ex_ci_onesample_standalone.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats0d/ex_ci_pairedsample.py` & `spm1d-0.4.30/spm1d/examples/stats0d/ex_ci_pairedsample.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats0d/ex_ci_twosample.py` & `spm1d-0.4.30/spm1d/examples/stats0d/ex_ci_twosample.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_anova1.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_anova1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_anova1_posthoc.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_anova1_posthoc.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_anova1rm.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_anova1rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_anova2.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_anova2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_anova2nested.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_anova2nested.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_anova2onerm.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_anova2onerm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_anova2rm.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_anova2rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_anova3.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_anova3.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_anova3nested.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_anova3nested.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_anova3onerm.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_anova3onerm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_anova3rm.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_anova3rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_anova3tworm.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_anova3tworm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_ci_onesample.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_ci_onesample.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_ci_onesample_standalone.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_ci_onesample_standalone.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_ci_pairedsample.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_ci_pairedsample.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_ci_twosample.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_ci_twosample.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_eqvartest.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_eqvartest.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_glm.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_glm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_hotellings_paired_Neptune1999.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_hotellings_paired_Neptune1999.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_hotellings_paired_Pataky2014.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_hotellings_paired_Pataky2014.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_regression.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_regression.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_ttest.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_ttest.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_ttest2.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_ttest2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_ttest_paired.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_ttest_paired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/ex_ttest_roi.py` & `spm1d-0.4.30/spm1d/examples/stats1d/ex_ttest_roi.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/rfx_0_means.py` & `spm1d-0.4.30/spm1d/examples/stats1d/rfx_0_means.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/rfx_1_level1.py` & `spm1d-0.4.30/spm1d/examples/stats1d/rfx_1_level1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d/rfx_2_level2.py` & `spm1d-0.4.30/spm1d/examples/stats1d/rfx_2_level2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova1.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova1rm.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova1rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova2.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova2nested.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova2nested.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova2onerm.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova2onerm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova2rm.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova2rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova3.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova3.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova3nested.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova3nested.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova3onerm.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova3onerm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova3rm.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova3rm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_anova3tworm.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_anova3tworm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_cca_Dorn2012.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_cca_Dorn2012.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_glm.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_glm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_hotellings2_Besier2009muscleforces.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_hotellings2_Besier2009muscleforces.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_hotellings_paired_Neptune1999.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_hotellings_paired_Neptune1999.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_hotellings_paired_Pataky2014.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_hotellings_paired_Pataky2014.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_manova1_Dorn2012.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_manova1_Dorn2012.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_regression.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_regression.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_regression_directional.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_regression_directional.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_ttest.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_ttest.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_ttest2.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_ttest2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats1d_roi/ex_ttest_paired.py` & `spm1d-0.4.30/spm1d/examples/stats1d_roi/ex_ttest_paired.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats2d/data2d.npy` & `spm1d-0.4.30/spm1d/examples/stats2d/data2d.npy`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/stats2d/ex2d_ttest2.py` & `spm1d-0.4.30/spm1d/examples/stats2d/ex2d_ttest2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/summarystats/ex_plot_meansd.py` & `spm1d-0.4.30/spm1d/examples/summarystats/ex_plot_meansd.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/examples/validation/val_eqvartest.py` & `spm1d-0.4.30/spm1d/examples/validation/val_eqvartest.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/io.py` & `spm1d-0.4.30/spm1d/io.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/plot.py` & `spm1d-0.4.30/spm1d/plot.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/__init__.py` & `spm1d-0.4.30/spm1d/rft1d/__init__.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/data/weather/README.txt` & `spm1d-0.4.30/spm1d/rft1d/data/weather/README.txt`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/data/weather/daily.m` & `spm1d-0.4.30/spm1d/rft1d/data/weather/daily.m`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/data/weather/daily.mat` & `spm1d-0.4.30/spm1d/rft1d/data/weather/daily.mat`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/data.py` & `spm1d-0.4.30/spm1d/rft1d/data.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/distributions.py` & `spm1d-0.4.30/spm1d/rft1d/distributions.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/paper/all_results.py` & `spm1d-0.4.30/spm1d/rft1d/examples/paper/all_results.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/paper/fig01_fields1d.py` & `spm1d-0.4.30/spm1d/rft1d/examples/paper/fig01_fields1d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/paper/fig02_EC_HC.py` & `spm1d-0.4.30/spm1d/rft1d/examples/paper/fig02_EC_HC.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/paper/fig03_EC.py` & `spm1d-0.4.30/spm1d/rft1d/examples/paper/fig03_EC.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/paper/fig04_fields1d_broken.py` & `spm1d-0.4.30/spm1d/rft1d/examples/paper/fig04_fields1d_broken.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/paper/fig05_EC_broken.py` & `spm1d-0.4.30/spm1d/rft1d/examples/paper/fig05_EC_broken.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/paper/fig06_sf.py` & `spm1d-0.4.30/spm1d/rft1d/examples/paper/fig06_sf.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/paper/fig07_bonf_sf.py` & `spm1d-0.4.30/spm1d/rft1d/examples/paper/fig07_bonf_sf.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/paper/fig08_bonf_isf.py` & `spm1d-0.4.30/spm1d/rft1d/examples/paper/fig08_bonf_isf.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/paper/fig09_val_maxima.py` & `spm1d-0.4.30/spm1d/rft1d/examples/paper/fig09_val_maxima.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/paper/fig10_upcrossing.py` & `spm1d-0.4.30/spm1d/rft1d/examples/paper/fig10_upcrossing.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/paper/fig11_val_cluster.py` & `spm1d-0.4.30/spm1d/rft1d/examples/paper/fig11_val_cluster.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/paper/fig12_val_set.py` & `spm1d-0.4.30/spm1d/rft1d/examples/paper/fig12_val_set.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/paper/fig13_weather_0_data.py` & `spm1d-0.4.30/spm1d/rft1d/examples/paper/fig13_weather_0_data.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/paper/fig14_fwhm_estimation.py` & `spm1d-0.4.30/spm1d/rft1d/examples/paper/fig14_fwhm_estimation.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/paper/fig15_weather_1_rft.py` & `spm1d-0.4.30/spm1d/rft1d/examples/paper/fig15_weather_1_rft.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/paper/fig16_weather_2_wrapped.py` & `spm1d-0.4.30/spm1d/rft1d/examples/paper/fig16_weather_2_wrapped.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/paper/fig17_weather_3_nonparam.py` & `spm1d-0.4.30/spm1d/rft1d/examples/paper/fig17_weather_3_nonparam.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/random_fields_0.py` & `spm1d-0.4.30/spm1d/rft1d/examples/random_fields_0.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/random_fields_1.py` & `spm1d-0.4.30/spm1d/rft1d/examples/random_fields_1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/random_fields_2.py` & `spm1d-0.4.30/spm1d/rft1d/examples/random_fields_2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/random_fields_broken_0.py` & `spm1d-0.4.30/spm1d/rft1d/examples/random_fields_broken_0.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/random_fields_broken_1.py` & `spm1d-0.4.30/spm1d/rft1d/examples/random_fields_broken_1.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/random_fields_broken_2.py` & `spm1d-0.4.30/spm1d/rft1d/examples/random_fields_broken_2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/smoothness_estimation.py` & `spm1d-0.4.30/spm1d/rft1d/examples/smoothness_estimation.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/smoothness_estimation_broken.py` & `spm1d-0.4.30/spm1d/rft1d/examples/smoothness_estimation_broken.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_broken_0_gauss.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_broken_0_gauss.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_broken_1_t.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_broken_1_t.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_broken_2_F.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_broken_2_F.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_broken_3_T2.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_broken_3_T2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_broken_4_X2.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_broken_4_X2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_conj_0_gauss.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_conj_0_gauss.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_conj_1_t.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_conj_1_t.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_conj_2_F.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_conj_2_F.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_conj_3_T2.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_conj_3_T2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_conj_4_X2.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_conj_4_X2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_max_0_gaussian_0d.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_max_0_gaussian_0d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_max_0_gaussian_1d.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_max_0_gaussian_1d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_max_1_onesample_t_0d.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_max_1_onesample_t_0d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_max_1_onesample_t_1d.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_max_1_onesample_t_1d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_max_2_twosample_t_0d.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_max_2_twosample_t_0d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_max_2_twosample_t_1d.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_max_2_twosample_t_1d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_max_3_regress_0d.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_max_3_regress_0d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_max_3_regress_1d.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_max_3_regress_1d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_max_4_anova1_0d.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_max_4_anova1_0d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_max_4_anova1_1d.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_max_4_anova1_1d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_max_5_onesample_T2_0d.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_max_5_onesample_T2_0d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_max_5_onesample_T2_1d.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_max_5_onesample_T2_1d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_max_6_twosample_T2_0d.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_max_6_twosample_T2_0d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_max_6_twosample_T2_1d.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_max_6_twosample_T2_1d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_max_7_cca_0d.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_max_7_cca_0d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_max_7_cca_1d.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_max_7_cca_1d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_max_8_manova1_0d.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_max_8_manova1_0d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_max_8_manova1_1d.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_max_8_manova1_1d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_upx_0_gauss_cluster.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_upx_0_gauss_cluster.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_upx_0_gauss_set.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_upx_0_gauss_set.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_upx_1_t_cluster.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_upx_1_t_cluster.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_upx_1_t_set.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_upx_1_t_set.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_upx_2_F_cluster.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_upx_2_F_cluster.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_upx_2_F_set.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_upx_2_F_set.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_upx_3_T2_cluster.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_upx_3_T2_cluster.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_upx_3_T2_set.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_upx_3_T2_set.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_upx_4_X2_cluster.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_upx_4_X2_cluster.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/val_upx_4_X2_set.py` & `spm1d-0.4.30/spm1d/rft1d/examples/val_upx_4_X2_set.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/weather_0_plotdata.py` & `spm1d-0.4.30/spm1d/rft1d/examples/weather_0_plotdata.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/weather_1_rft.py` & `spm1d-0.4.30/spm1d/rft1d/examples/weather_1_rft.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/weather_2_nonparam.py` & `spm1d-0.4.30/spm1d/rft1d/examples/weather_2_nonparam.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/examples/weather_3_wrapped.py` & `spm1d-0.4.30/spm1d/rft1d/examples/weather_3_wrapped.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/geom.py` & `spm1d-0.4.30/spm1d/rft1d/geom.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/prob.py` & `spm1d-0.4.30/spm1d/rft1d/prob.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/rft1d/random.py` & `spm1d-0.4.30/spm1d/rft1d/random.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/__init__.py` & `spm1d-0.4.30/spm1d/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/_clusters.py` & `spm1d-0.4.30/spm1d/stats/_clusters.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/_datachecks.py` & `spm1d-0.4.30/spm1d/stats/_datachecks.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/_mvbase.py` & `spm1d-0.4.30/spm1d/stats/_mvbase.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/_reml.py` & `spm1d-0.4.30/spm1d/stats/_reml.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/_spm.py` & `spm1d-0.4.30/spm1d/stats/_spm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/_spmlist.py` & `spm1d-0.4.30/spm1d/stats/_spmlist.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/anova/designs.py` & `spm1d-0.4.30/spm1d/stats/anova/designs.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/anova/factors.py` & `spm1d-0.4.30/spm1d/stats/anova/factors.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/anova/ui.py` & `spm1d-0.4.30/spm1d/stats/anova/ui.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/c/__init__.py` & `spm1d-0.4.30/spm1d/stats/c/__init__.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/cca.py` & `spm1d-0.4.30/spm1d/stats/cca.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/ci.py` & `spm1d-0.4.30/spm1d/stats/ci.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/hotellings.py` & `spm1d-0.4.30/spm1d/stats/hotellings.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/manova.py` & `spm1d-0.4.30/spm1d/stats/manova.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/nonparam/__init__.py` & `spm1d-0.4.30/spm1d/stats/nonparam/__init__.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/nonparam/_snpm.py` & `spm1d-0.4.30/spm1d/stats/nonparam/_snpm.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/nonparam/_snpmlist.py` & `spm1d-0.4.30/spm1d/stats/nonparam/_snpmlist.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/nonparam/calculators.py` & `spm1d-0.4.30/spm1d/stats/nonparam/calculators.py`

 * *Files 6% similar despite different names*

```diff
@@ -191,22 +191,26 @@
 		R      = eij.T*eij              #residual sum of squares
 		sigma2 = float(R) / self.df     #variance
 		t      = float(self.c.T*b)  /   (sigma2*self.cXXc)**0.5
 		return t
 
 
 class CalculatorRegress1D(CalculatorRegress0D):
-	def get_test_stat(self, y):
-		Y      = np.matrix(y)
-		b      = self.Xi * Y            #parameters
-		eij    = Y - self.X*b           #residuals
-		R      = eij.T*eij              #residual sum of squares
-		sigma2 = np.diag(R) / self.df   #variance
-		t      = np.array(self.c.T*b).flatten()  /   ((sigma2*self.cXXc)**0.5 + eps)
-		return t
+    def get_test_stat(self, y):
+        Y      = np.matrix(y)
+        b      = self.Xi * Y            #parameters
+        eij    = Y - self.X*b           #residuals
+        # # previous sigma2 calculation (slow when Q get large: about 5 ms for Q=1000 and about 900 ms for Q=10000! )
+        # R      = eij.T@eij              #residuals: sum of squares
+        # sigma2 = np.diag(R)/df          #variance
+        # new sigam2 calculation (using eigensum trick)
+        diagR  = np.einsum('ij,ji->i', eij.T, eij)  # residual sum of squares (eigensum trick)
+        sigma2 = diagR / df          #variance
+        t      = np.array(self.c.T*b).flatten()  /   ((sigma2*self.cXXc)**0.5 + eps)
+        return t
 
 
 class CalculatorCCA0D(object):
 	def __init__(self, x):
 		self.x           = np.asarray(x, dtype=float)
 		self.J           = x.size
 		self.X           = np.matrix(x).T
```

### Comparing `spm1d-0.4.29/spm1d/stats/nonparam/ci.py` & `spm1d-0.4.30/spm1d/stats/nonparam/ci.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/nonparam/metrics.py` & `spm1d-0.4.30/spm1d/stats/nonparam/metrics.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/nonparam/permuters.py` & `spm1d-0.4.30/spm1d/stats/nonparam/permuters.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/nonparam/stats.py` & `spm1d-0.4.30/spm1d/stats/nonparam/stats.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/normality/__init__.py` & `spm1d-0.4.30/spm1d/stats/normality/__init__.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/normality/k2.py` & `spm1d-0.4.30/spm1d/stats/normality/k2.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/normality/sw.py` & `spm1d-0.4.30/spm1d/stats/normality/sw.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/stats/t.py` & `spm1d-0.4.30/spm1d/stats/t.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,21 @@
     ### assemble data:
     Y      = np.asarray(Y)
     X      = np.asarray(X)
     c      = np.asarray([c]).T
     ### solve the GLM:
     b      = np.linalg.pinv(X) @ Y  #parameters
     eij    = Y - X@b                #residuals
-    R      = eij.T@eij              #residuals: sum of squares
     df     = Y.shape[0] - rank(X)   #degrees of freedom
-    sigma2 = np.diag(R)/df          #variance
+    # # previous sigma2 calculation (slow when Q get large: about 5 ms for Q=1000 and about 900 ms for Q=10000! )
+    # R      = eij.T@eij              #residuals: sum of squares
+    # sigma2 = np.diag(R)/df          #variance
+    # new sigam2 calculation (using Einstein summation trick)
+    diagR  = np.einsum('ij,ji->i', eij.T, eij)  # residual sum of squares (eigensum trick)
+    sigma2 = diagR / df          #variance
     ### compute t statistic
     cXXc   = c.T @ np.linalg.inv(X.T@X) @ c
     cXXc   = float(cXXc[0,0]) if isinstance(cXXc, np.ndarray) else float(cXXc)
     t      = np.array(c.T@b).flatten()  /   (np.sqrt(sigma2*cXXc + eps))
     ### estimate df due to non-sphericity:
     if Q is not None:
         df = _reml.estimate_df_T(Y, X, eij, Q)
```

### Comparing `spm1d-0.4.29/spm1d/stats/var.py` & `spm1d-0.4.30/spm1d/stats/var.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d/util.py` & `spm1d-0.4.30/spm1d/util.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/spm1d.egg-info/PKG-INFO` & `spm1d-0.4.30/spm1d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spm1d
-Version: 0.4.29
+Version: 0.4.30
 Summary: One-Dimensional Statistical Parametric Mapping
 Home-page: https://github.com/0todd0000/spm1d
 Download-URL: https://github.com/0todd0000/spm1d/archive/master.zip
 Author: Todd Pataky
 Author-email: spm1d.mail@gmail.com
 Keywords: statistics,time series analysis
 License-File: LICENSE.txt
```

### Comparing `spm1d-0.4.29/spm1d.egg-info/SOURCES.txt` & `spm1d-0.4.30/spm1d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/tests/test_0d.py` & `spm1d-0.4.30/tests/test_0d.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/tests/test_0d_c.py` & `spm1d-0.4.30/tests/test_0d_c.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/tests/test_0d_mv.py` & `spm1d-0.4.30/tests/test_0d_mv.py`

 * *Files identical despite different names*

### Comparing `spm1d-0.4.29/tests/test_0d_mv_c.py` & `spm1d-0.4.30/tests/test_0d_mv_c.py`

 * *Files identical despite different names*

