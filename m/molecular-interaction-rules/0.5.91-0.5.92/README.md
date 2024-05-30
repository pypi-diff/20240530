# Comparing `tmp/molecular_interaction_rules-0.5.91.tar.gz` & `tmp/molecular_interaction_rules-0.5.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecular_interaction_rules-0.5.91.tar", last modified: Thu May 30 04:07:15 2024, max compression
+gzip compressed data, was "molecular_interaction_rules-0.5.92.tar", last modified: Thu May 30 04:10:21 2024, max compression
```

## Comparing `molecular_interaction_rules-0.5.91.tar` & `molecular_interaction_rules-0.5.92.tar`

### file list

```diff
@@ -1,15 +1,141 @@
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:07:15.089326 molecular_interaction_rules-0.5.91/
--rw-r--r--   0 sulimansharif   (501) staff       (20)       51 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.5.91/MANIFEST.in
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2362 2024-05-30 04:07:15.089043 molecular_interaction_rules-0.5.91/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)      887 2024-05-30 03:52:35.000000 molecular_interaction_rules-0.5.91/README.md
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:07:15.086043 molecular_interaction_rules-0.5.91/molecular_interaction_rules/
--rw-r--r--   0 sulimansharif   (501) staff       (20)      238 2024-05-30 04:06:56.000000 molecular_interaction_rules-0.5.91/molecular_interaction_rules/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3115 2024-05-30 04:06:56.000000 molecular_interaction_rules-0.5.91/molecular_interaction_rules/molecular_database.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:07:15.088420 molecular_interaction_rules-0.5.91/molecular_interaction_rules.egg-info/
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2362 2024-05-30 04:07:14.000000 molecular_interaction_rules-0.5.91/molecular_interaction_rules.egg-info/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)      374 2024-05-30 04:07:14.000000 molecular_interaction_rules-0.5.91/molecular_interaction_rules.egg-info/SOURCES.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 04:07:14.000000 molecular_interaction_rules-0.5.91/molecular_interaction_rules.egg-info/dependency_links.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 04:07:14.000000 molecular_interaction_rules-0.5.91/molecular_interaction_rules.egg-info/not-zip-safe
--rw-r--r--   0 sulimansharif   (501) staff       (20)       28 2024-05-30 04:07:14.000000 molecular_interaction_rules-0.5.91/molecular_interaction_rules.egg-info/top_level.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-30 04:07:15.089436 molecular_interaction_rules-0.5.91/setup.cfg
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1699 2024-05-30 04:07:04.000000 molecular_interaction_rules-0.5.91/setup.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:10:21.668785 molecular_interaction_rules-0.5.92/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       51 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.5.92/MANIFEST.in
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2362 2024-05-30 04:10:21.668456 molecular_interaction_rules-0.5.92/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      887 2024-05-30 03:52:35.000000 molecular_interaction_rules-0.5.92/README.md
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:10:21.535615 molecular_interaction_rules-0.5.92/molecular_interaction_rules/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      122 2024-05-30 04:10:17.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:10:21.545139 molecular_interaction_rules-0.5.92/molecular_interaction_rules/ions/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      170 2024-05-30 02:02:18.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/ions/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      832 2024-05-30 02:02:18.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/ions/potasium.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      821 2024-05-30 02:02:18.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/ions/sodium.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3115 2024-05-30 04:06:56.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecular_database.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:10:21.546533 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 02:02:18.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:10:21.568529 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    10721 2024-05-30 02:02:18.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/azulene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4599 2024-05-30 03:39:43.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/benzene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     6123 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/bipyrrole.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     6626 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/bromobenzene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4399 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/chlorobenzene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     6769 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/fluorobenzene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4428 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/four_pyridinone.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3782 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/furan.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4017 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/imidazole.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5054 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/imidazolium.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5735 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/indole.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4533 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/indolizine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4529 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/iodobenzene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4914 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/isoxazole.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2783 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/methyleneoxindole.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5244 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/nitrobenzene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     7962 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/one_phenyl_four_pyridinone.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4510 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/phenol.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3714 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/phenoxazine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4396 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/pyridine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2507 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/pyridinium.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4243 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/pyrimidine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4989 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/pyrrolidine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3947 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/thiophene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2693 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/three_amino_pyridine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4431 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/two_h_pyran.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4434 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/aromatic/uracil.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:10:21.569291 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 02:02:18.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:10:21.570149 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alcohols/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alcohols/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3321 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alcohols/methanol.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:10:21.583886 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alkanes/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alkanes/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2623 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alkanes/cyclobutane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4580 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alkanes/cyclohexane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2117 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alkanes/cyclopropane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4399 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alkanes/neopentane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4530 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alkanes/propane.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:10:21.601014 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alkenes/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alkenes/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5766 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alkenes/cyclohexene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5153 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alkenes/cyclopentene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5811 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alkenes/methoxyethene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2352 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alkenes/one_three_dibutene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2267 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alkenes/propene.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1544 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alkenes/two_pyrroline.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:10:21.606782 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alkynes/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alkynes/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2665 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/alkynes/propyne.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:10:21.625578 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amides/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amides/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2114 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amides/acetamide.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2494 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amides/amidinium.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4109 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amides/azetidinone.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4929 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amides/dimethylformamide.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2701 2024-05-30 02:28:24.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amides/methylacetamide.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     6424 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amides/prolineamide.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3234 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amides/prolineamide_charged.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2976 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amides/two_pyrrolidinone.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:10:21.637046 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amines/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amines/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2049 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amines/ammonia.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     6166 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amines/dimethylamine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4415 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amines/ethoxy_guanidine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2534 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amines/ethyl_ammonium.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1905 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amines/hydrazine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3208 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amines/methylamine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3261 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amines/piperidine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3280 2024-05-30 02:28:23.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amines/tetramethylammonium.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5037 2024-05-30 02:31:08.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amines/trimethylamine.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2968 2024-05-30 02:31:08.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/amines/trimethylammonium.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:10:21.644523 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/carbonyls/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/carbonyls/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1763 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/carbonyls/acetaldehyde.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2452 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/carbonyls/acetate.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3511 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/carbonyls/acetic_acid.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4043 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/carbonyls/acetone.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1832 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/carbonyls/carbon_dioxide.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1260 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/carbonyls/formaldehyde.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2561 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/carbonyls/methylacetate.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3413 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/carbonyls/urea.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:10:21.648814 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/ethers/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/ethers/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1822 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/ethers/dimethylether.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1794 2024-05-30 02:33:50.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/ethers/epoxide.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3066 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/ethers/oxetane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4951 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/ethers/tetrahydrofuran.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3046 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/ethers/tetrahydropyran.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:10:21.657605 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/halogens/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/halogens/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2076 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/halogens/bromoethane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1929 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/halogens/chloroethane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3632 2024-05-30 02:33:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/halogens/dibromoethane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3781 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/halogens/difluoroethane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3715 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/halogens/fluoroethane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2009 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/halogens/tribromoethane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1905 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/halogens/trichloroethane.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2031 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/halogens/trifluoroethane.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:10:21.658680 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/imines/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/imines/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2625 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/imines/ethenamine.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:10:21.659763 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/nitriles/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/nitriles/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3239 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/nitriles/acetonitrile.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:10:21.661954 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/organophosphorous/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/organophosphorous/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2798 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/organophosphorous/dimethyl_phosphate.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2376 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/organophosphorous/methyl_phosphate.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:10:21.667426 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/organosulfur/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/organosulfur/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4309 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/organosulfur/dimethyl_sulfone.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4085 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/organosulfur/dimethyl_sulfoxide.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5655 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/organosulfur/dimethyl_trithiocarbonate.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2434 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/organosulfur/dimethyldisulfide.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2357 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/organosulfur/ethylsulfanyl_phosphonic_acid.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1860 2024-05-30 02:36:51.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/organosulfur/methanethiol.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2914 2024-05-30 02:38:29.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecules/non_aromatic/organosulfur/methylthiolate.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:10:21.541308 molecular_interaction_rules-0.5.92/molecular_interaction_rules.egg-info/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2362 2024-05-30 04:10:20.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules.egg-info/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     8125 2024-05-30 04:10:21.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 04:10:20.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 04:10:20.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules.egg-info/not-zip-safe
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       28 2024-05-30 04:10:20.000000 molecular_interaction_rules-0.5.92/molecular_interaction_rules.egg-info/top_level.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-30 04:10:21.668959 molecular_interaction_rules-0.5.92/setup.cfg
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1683 2024-05-30 04:10:17.000000 molecular_interaction_rules-0.5.92/setup.py
```

### Comparing `molecular_interaction_rules-0.5.91/PKG-INFO` & `molecular_interaction_rules-0.5.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecular_interaction_rules
-Version: 0.5.91
+Version: 0.5.92
 Summary: UNKNOWN
 Home-page: https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: GPL
 Description: # Molecular Interaction Rules
```

### Comparing `molecular_interaction_rules-0.5.91/README.md` & `molecular_interaction_rules-0.5.92/README.md`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.91/molecular_interaction_rules/molecular_database.py` & `molecular_interaction_rules-0.5.92/molecular_interaction_rules/molecular_database.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.91/molecular_interaction_rules.egg-info/PKG-INFO` & `molecular_interaction_rules-0.5.92/molecular_interaction_rules.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecular-interaction-rules
-Version: 0.5.91
+Version: 0.5.92
 Summary: UNKNOWN
 Home-page: https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: GPL
 Description: # Molecular Interaction Rules
```

### Comparing `molecular_interaction_rules-0.5.91/setup.py` & `molecular_interaction_rules-0.5.92/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 else:
     long_description = 'Non-Covalent Molecular Interaction Rules'
 
 # exec
 # ----
 setup(
     name="molecular_interaction_rules",
-    version="0.5.91",
-    packages=['molecular_interaction_rules'],
+    version="0.5.92",
+    packages=find_packages(),
     license='GPL',
     author="Suliman Sharif",
     author_email="sharifsuliman1@gmail.com",
     url="https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules",
     long_description=long_description,
     long_description_content_type='text/markdown',
     zip_safe=False,
```

