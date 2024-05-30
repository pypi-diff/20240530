# Comparing `tmp/molecular_interaction_rules-0.5.96.tar.gz` & `tmp/molecular_interaction_rules-0.5.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecular_interaction_rules-0.5.96.tar", last modified: Thu May 30 04:17:57 2024, max compression
+gzip compressed data, was "molecular_interaction_rules-0.5.97.tar", last modified: Thu May 30 04:37:08 2024, max compression
```

## Comparing `molecular_interaction_rules-0.5.96.tar` & `molecular_interaction_rules-0.5.97.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:17:57.546429 molecular_interaction_rules-0.5.96/
--rw-r--r--   0 sulimansharif   (501) staff       (20)       51 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.5.96/MANIFEST.in
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2362 2024-05-30 04:17:57.546088 molecular_interaction_rules-0.5.96/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)      887 2024-05-30 03:52:35.000000 molecular_interaction_rules-0.5.96/README.md
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:17:57.444318 molecular_interaction_rules-0.5.96/molecular_interaction_rules/
--rw-r--r--   0 sulimansharif   (501) staff       (20)      273 2024-05-30 04:16:04.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:17:57.447753 molecular_interaction_rules-0.5.96/molecular_interaction_rules/ions/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:14:20.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/ions/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      795 2024-05-30 04:12:43.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/ions/potassium.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      821 2024-05-30 02:02:18.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/ions/sodium.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3234 2024-05-30 04:17:44.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecular_database.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:17:57.448703 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 02:02:18.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:17:57.480934 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    10721 2024-05-30 02:02:18.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/azulene.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4599 2024-05-30 03:39:43.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/benzene.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     6123 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/bipyrrole.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     6626 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/bromobenzene.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4399 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/chlorobenzene.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     6769 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/fluorobenzene.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4428 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/four_pyridinone.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3782 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/furan.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4017 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/imidazole.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5054 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/imidazolium.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5735 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/indole.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4533 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/indolizine.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4529 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/iodobenzene.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4914 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/isoxazole.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2783 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/methyleneoxindole.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5244 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/nitrobenzene.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     7962 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/one_phenyl_four_pyridinone.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4510 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/phenol.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3714 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/phenoxazine.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4396 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/pyridine.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2507 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/pyridinium.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4243 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/pyrimidine.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4989 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/pyrrolidine.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3947 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/thiophene.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2693 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/three_amino_pyridine.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4431 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/two_h_pyran.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4434 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/uracil.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:17:57.481822 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 02:02:18.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:17:57.482876 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alcohols/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alcohols/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3321 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alcohols/methanol.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:17:57.489785 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkanes/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkanes/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2623 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkanes/cyclobutane.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4580 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkanes/cyclohexane.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2117 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkanes/cyclopropane.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4399 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkanes/neopentane.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4530 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkanes/propane.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:17:57.495685 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkenes/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkenes/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5766 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkenes/cyclohexene.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5153 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkenes/cyclopentene.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5811 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkenes/methoxyethene.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2352 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkenes/one_three_dibutene.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2267 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkenes/propene.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1544 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkenes/two_pyrroline.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:17:57.496873 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkynes/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkynes/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2665 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkynes/propyne.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:17:57.505223 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amides/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amides/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2114 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amides/acetamide.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2494 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amides/amidinium.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4109 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amides/azetidinone.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4929 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amides/dimethylformamide.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2701 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amides/methylacetamide.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     6424 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amides/prolineamide.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3234 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amides/prolineamide_charged.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2976 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amides/two_pyrrolidinone.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:17:57.515016 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2049 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/ammonia.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     6166 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/dimethylamine.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4415 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/ethoxy_guanidine.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2534 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/ethyl_ammonium.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1905 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/hydrazine.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3208 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/methylamine.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3261 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/piperidine.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3280 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/tetramethylammonium.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5037 2024-05-30 02:31:08.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/trimethylamine.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2968 2024-05-30 02:31:08.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/trimethylammonium.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:17:57.522402 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/carbonyls/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/carbonyls/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1763 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/carbonyls/acetaldehyde.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2452 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/carbonyls/acetate.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3511 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/carbonyls/acetic_acid.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4043 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/carbonyls/acetone.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1832 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/carbonyls/carbon_dioxide.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1260 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/carbonyls/formaldehyde.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2561 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/carbonyls/methylacetate.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3413 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/carbonyls/urea.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:17:57.527896 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/ethers/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/ethers/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1822 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/ethers/dimethylether.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1794 2024-05-30 02:33:50.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/ethers/epoxide.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3066 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/ethers/oxetane.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4951 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/ethers/tetrahydrofuran.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3046 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/ethers/tetrahydropyran.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:17:57.536304 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/halogens/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/halogens/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2076 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/halogens/bromoethane.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1929 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/halogens/chloroethane.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3632 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/halogens/dibromoethane.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3781 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/halogens/difluoroethane.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3715 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/halogens/fluoroethane.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2009 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/halogens/tribromoethane.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1905 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/halogens/trichloroethane.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2031 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/halogens/trifluoroethane.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:17:57.537427 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/imines/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/imines/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2625 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/imines/ethenamine.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:17:57.538551 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/nitriles/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/nitriles/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3239 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/nitriles/acetonitrile.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:17:57.540219 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organophosphorous/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organophosphorous/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2798 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organophosphorous/dimethyl_phosphate.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2376 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organophosphorous/methyl_phosphate.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:17:57.545256 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organosulfur/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organosulfur/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4309 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organosulfur/dimethyl_sulfone.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4085 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organosulfur/dimethyl_sulfoxide.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5655 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organosulfur/dimethyl_trithiocarbonate.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2434 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organosulfur/dimethyldisulfide.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2357 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organosulfur/ethylsulfanyl_phosphonic_acid.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1860 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organosulfur/methanethiol.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2914 2024-05-30 02:38:29.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organosulfur/methylthiolate.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:17:57.446145 molecular_interaction_rules-0.5.96/molecular_interaction_rules.egg-info/
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2362 2024-05-30 04:17:56.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules.egg-info/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)     8126 2024-05-30 04:17:56.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules.egg-info/SOURCES.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 04:17:56.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules.egg-info/dependency_links.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 04:17:56.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules.egg-info/not-zip-safe
--rw-r--r--   0 sulimansharif   (501) staff       (20)       28 2024-05-30 04:17:56.000000 molecular_interaction_rules-0.5.96/molecular_interaction_rules.egg-info/top_level.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-30 04:17:57.546612 molecular_interaction_rules-0.5.96/setup.cfg
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1683 2024-05-30 04:17:54.000000 molecular_interaction_rules-0.5.96/setup.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:37:08.335386 molecular_interaction_rules-0.5.97/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       51 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.5.97/MANIFEST.in
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2362 2024-05-30 04:37:08.334951 molecular_interaction_rules-0.5.97/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      887 2024-05-30 03:52:35.000000 molecular_interaction_rules-0.5.97/README.md
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:37:08.258470 molecular_interaction_rules-0.5.97/molecular_interaction_rules/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      273 2024-05-30 04:16:04.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:37:08.263097 molecular_interaction_rules-0.5.97/molecular_interaction_rules/ions/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:14:20.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/ions/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      795 2024-05-30 04:12:43.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/ions/potassium.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      821 2024-05-30 02:02:18.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/ions/sodium.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3232 2024-05-30 04:36:55.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecular_database.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:37:08.263674 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 02:02:18.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:37:08.285665 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    10721 2024-05-30 02:02:18.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/azulene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4599 2024-05-30 03:39:43.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/benzene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     6123 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/bipyrrole.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     6626 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/bromobenzene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4399 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/chlorobenzene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     6769 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/fluorobenzene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4428 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/four_pyridinone.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3782 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/furan.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4017 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/imidazole.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5054 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/imidazolium.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5735 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/indole.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4533 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/indolizine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4529 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/iodobenzene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4914 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/isoxazole.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2783 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/methyleneoxindole.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5244 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/nitrobenzene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     7962 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/one_phenyl_four_pyridinone.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4510 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/phenol.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3714 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/phenoxazine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4396 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/pyridine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2507 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/pyridinium.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4243 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/pyrimidine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4989 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/pyrrolidine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3947 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/thiophene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2693 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/three_amino_pyridine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4431 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/two_h_pyran.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4434 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/uracil.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:37:08.286213 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 02:02:18.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:37:08.287129 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alcohols/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alcohols/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3321 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alcohols/methanol.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:37:08.292087 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkanes/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkanes/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2623 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkanes/cyclobutane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4580 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkanes/cyclohexane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2117 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkanes/cyclopropane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4399 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkanes/neopentane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4530 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkanes/propane.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:37:08.295639 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkenes/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkenes/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5766 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkenes/cyclohexene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5153 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkenes/cyclopentene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5811 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkenes/methoxyethene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2352 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkenes/one_three_dibutene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2267 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkenes/propene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1544 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkenes/two_pyrroline.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:37:08.296757 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkynes/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkynes/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2665 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkynes/propyne.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:37:08.303074 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amides/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amides/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2114 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amides/acetamide.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2494 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amides/amidinium.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4109 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amides/azetidinone.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4929 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amides/dimethylformamide.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2701 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amides/methylacetamide.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     6424 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amides/prolineamide.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3234 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amides/prolineamide_charged.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2976 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amides/two_pyrrolidinone.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:37:08.309667 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2049 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/ammonia.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     6166 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/dimethylamine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4415 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/ethoxy_guanidine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2534 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/ethyl_ammonium.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1905 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/hydrazine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3208 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/methylamine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3261 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/piperidine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3280 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/tetramethylammonium.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5037 2024-05-30 02:31:08.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/trimethylamine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2968 2024-05-30 02:31:08.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/trimethylammonium.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:37:08.315367 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/carbonyls/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/carbonyls/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1763 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/carbonyls/acetaldehyde.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2452 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/carbonyls/acetate.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3511 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/carbonyls/acetic_acid.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4043 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/carbonyls/acetone.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1832 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/carbonyls/carbon_dioxide.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1260 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/carbonyls/formaldehyde.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2561 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/carbonyls/methylacetate.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3413 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/carbonyls/urea.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:37:08.319311 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/ethers/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/ethers/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1822 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/ethers/dimethylether.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1794 2024-05-30 02:33:50.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/ethers/epoxide.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3066 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/ethers/oxetane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4951 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/ethers/tetrahydrofuran.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3046 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/ethers/tetrahydropyran.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:37:08.324736 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/halogens/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/halogens/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2076 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/halogens/bromoethane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1929 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/halogens/chloroethane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3632 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/halogens/dibromoethane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3781 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/halogens/difluoroethane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3715 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/halogens/fluoroethane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2009 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/halogens/tribromoethane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1905 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/halogens/trichloroethane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2031 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/halogens/trifluoroethane.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:37:08.325738 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/imines/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/imines/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2625 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/imines/ethenamine.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:37:08.326832 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/nitriles/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/nitriles/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3239 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/nitriles/acetonitrile.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:37:08.328382 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organophosphorous/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organophosphorous/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2798 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organophosphorous/dimethyl_phosphate.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2376 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organophosphorous/methyl_phosphate.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:37:08.333901 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organosulfur/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organosulfur/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4309 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organosulfur/dimethyl_sulfone.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4085 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organosulfur/dimethyl_sulfoxide.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5655 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organosulfur/dimethyl_trithiocarbonate.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2434 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organosulfur/dimethyldisulfide.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2357 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organosulfur/ethylsulfanyl_phosphonic_acid.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1860 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organosulfur/methanethiol.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2914 2024-05-30 02:38:29.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organosulfur/methylthiolate.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:37:08.261301 molecular_interaction_rules-0.5.97/molecular_interaction_rules.egg-info/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2362 2024-05-30 04:37:08.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules.egg-info/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     8126 2024-05-30 04:37:08.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 04:37:08.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 04:37:08.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules.egg-info/not-zip-safe
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       28 2024-05-30 04:37:08.000000 molecular_interaction_rules-0.5.97/molecular_interaction_rules.egg-info/top_level.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-30 04:37:08.335548 molecular_interaction_rules-0.5.97/setup.cfg
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1683 2024-05-30 04:36:55.000000 molecular_interaction_rules-0.5.97/setup.py
```

### Comparing `molecular_interaction_rules-0.5.96/PKG-INFO` & `molecular_interaction_rules-0.5.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecular_interaction_rules
-Version: 0.5.96
+Version: 0.5.97
 Summary: UNKNOWN
 Home-page: https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: GPL
 Description: # Molecular Interaction Rules
```

### Comparing `molecular_interaction_rules-0.5.96/README.md` & `molecular_interaction_rules-0.5.97/README.md`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/ions/potassium.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/ions/potassium.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/ions/sodium.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/ions/sodium.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecular_database.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecular_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def __init__(self):
 
         self.master_list = self.build_molecular_database()
 
     def build_molecular_database(self):
 
         molecules = [
-            Benzene()
+            Benzene
         ]
 
         return molecules
 
     def get_atom_names(self, monomer):
 
         '''
```

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/azulene.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/azulene.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/benzene.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/benzene.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/bipyrrole.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/bipyrrole.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/bromobenzene.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/bromobenzene.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/chlorobenzene.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/chlorobenzene.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/fluorobenzene.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/fluorobenzene.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/four_pyridinone.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/four_pyridinone.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/furan.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/furan.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/imidazole.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/imidazole.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/imidazolium.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/imidazolium.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/indole.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/indole.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/indolizine.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/indolizine.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/iodobenzene.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/iodobenzene.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/isoxazole.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/isoxazole.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/methyleneoxindole.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/methyleneoxindole.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/nitrobenzene.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/nitrobenzene.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/one_phenyl_four_pyridinone.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/one_phenyl_four_pyridinone.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/phenol.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/phenol.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/phenoxazine.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/phenoxazine.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/pyridine.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/pyridine.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/pyridinium.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/pyridinium.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/pyrimidine.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/pyrimidine.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/pyrrolidine.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/pyrrolidine.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/thiophene.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/thiophene.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/three_amino_pyridine.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/three_amino_pyridine.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/two_h_pyran.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/two_h_pyran.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/aromatic/uracil.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/aromatic/uracil.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alcohols/methanol.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alcohols/methanol.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkanes/cyclobutane.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkanes/cyclobutane.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkanes/cyclohexane.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkanes/cyclohexane.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkanes/cyclopropane.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkanes/cyclopropane.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkanes/neopentane.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkanes/neopentane.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkanes/propane.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkanes/propane.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkenes/cyclohexene.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkenes/cyclohexene.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkenes/cyclopentene.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkenes/cyclopentene.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkenes/methoxyethene.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkenes/methoxyethene.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkenes/one_three_dibutene.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkenes/one_three_dibutene.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkenes/propene.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkenes/propene.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkenes/two_pyrroline.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkenes/two_pyrroline.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/alkynes/propyne.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/alkynes/propyne.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amides/acetamide.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amides/acetamide.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amides/amidinium.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amides/amidinium.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amides/azetidinone.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amides/azetidinone.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amides/dimethylformamide.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amides/dimethylformamide.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amides/methylacetamide.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amides/methylacetamide.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amides/prolineamide.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amides/prolineamide.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amides/prolineamide_charged.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amides/prolineamide_charged.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amides/two_pyrrolidinone.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amides/two_pyrrolidinone.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/ammonia.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/ammonia.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/dimethylamine.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/dimethylamine.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/ethoxy_guanidine.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/ethoxy_guanidine.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/ethyl_ammonium.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/ethyl_ammonium.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/hydrazine.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/hydrazine.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/methylamine.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/methylamine.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/piperidine.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/piperidine.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/tetramethylammonium.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/tetramethylammonium.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/trimethylamine.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/trimethylamine.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/amines/trimethylammonium.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/amines/trimethylammonium.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/carbonyls/acetaldehyde.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/carbonyls/acetaldehyde.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/carbonyls/acetate.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/carbonyls/acetate.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/carbonyls/acetic_acid.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/carbonyls/acetic_acid.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/carbonyls/acetone.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/carbonyls/acetone.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/carbonyls/carbon_dioxide.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/carbonyls/carbon_dioxide.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/carbonyls/formaldehyde.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/carbonyls/formaldehyde.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/carbonyls/methylacetate.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/carbonyls/methylacetate.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/carbonyls/urea.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/carbonyls/urea.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/ethers/dimethylether.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/ethers/dimethylether.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/ethers/epoxide.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/ethers/epoxide.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/ethers/oxetane.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/ethers/oxetane.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/ethers/tetrahydrofuran.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/ethers/tetrahydrofuran.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/ethers/tetrahydropyran.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/ethers/tetrahydropyran.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/halogens/bromoethane.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/halogens/bromoethane.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/halogens/chloroethane.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/halogens/chloroethane.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/halogens/dibromoethane.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/halogens/dibromoethane.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/halogens/difluoroethane.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/halogens/difluoroethane.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/halogens/fluoroethane.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/halogens/fluoroethane.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/halogens/tribromoethane.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/halogens/tribromoethane.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/halogens/trichloroethane.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/halogens/trichloroethane.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/halogens/trifluoroethane.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/halogens/trifluoroethane.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/imines/ethenamine.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/imines/ethenamine.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/nitriles/acetonitrile.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/nitriles/acetonitrile.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organophosphorous/dimethyl_phosphate.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organophosphorous/dimethyl_phosphate.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organophosphorous/methyl_phosphate.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organophosphorous/methyl_phosphate.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organosulfur/dimethyl_sulfone.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organosulfur/dimethyl_sulfone.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organosulfur/dimethyl_sulfoxide.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organosulfur/dimethyl_sulfoxide.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organosulfur/dimethyl_trithiocarbonate.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organosulfur/dimethyl_trithiocarbonate.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organosulfur/dimethyldisulfide.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organosulfur/dimethyldisulfide.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organosulfur/ethylsulfanyl_phosphonic_acid.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organosulfur/ethylsulfanyl_phosphonic_acid.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organosulfur/methanethiol.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organosulfur/methanethiol.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules/molecules/non_aromatic/organosulfur/methylthiolate.py` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules/molecules/non_aromatic/organosulfur/methylthiolate.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules.egg-info/PKG-INFO` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecular-interaction-rules
-Version: 0.5.96
+Version: 0.5.97
 Summary: UNKNOWN
 Home-page: https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: GPL
 Description: # Molecular Interaction Rules
```

### Comparing `molecular_interaction_rules-0.5.96/molecular_interaction_rules.egg-info/SOURCES.txt` & `molecular_interaction_rules-0.5.97/molecular_interaction_rules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.96/setup.py` & `molecular_interaction_rules-0.5.97/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 else:
     long_description = 'Non-Covalent Molecular Interaction Rules'
 
 # exec
 # ----
 setup(
     name="molecular_interaction_rules",
-    version="0.5.96",
+    version="0.5.97",
     packages=find_packages(),
     license='GPL',
     author="Suliman Sharif",
     author_email="sharifsuliman1@gmail.com",
     url="https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules",
     long_description=long_description,
     long_description_content_type='text/markdown',
```

