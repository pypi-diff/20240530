# Comparing `tmp/pocket_coffea-0.9.2.tar.gz` & `tmp/pocket_coffea-1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocket_coffea-0.9.2.tar", last modified: Thu May 30 11:07:20 2024, max compression
+gzip compressed data, was "pocket_coffea-1.0rc3.tar", last modified: Tue Oct 10 07:02:02 2023, max compression
```

## Comparing `pocket_coffea-0.9.2.tar` & `pocket_coffea-1.0rc3.tar`

### file list

```diff
@@ -1,368 +1,508 @@
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-30 11:07:20.348882 pocket_coffea-0.9.2/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      119 2022-11-17 10:04:17.000000 pocket_coffea-0.9.2/.flake8
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      125 2022-11-17 10:04:17.000000 pocket_coffea-0.9.2/.git_archival.txt
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)       32 2022-11-17 10:04:17.000000 pocket_coffea-0.9.2/.gitattributes
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-30 11:07:18.801909 pocket_coffea-0.9.2/.github/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2405 2022-11-17 10:04:17.000000 pocket_coffea-0.9.2/.github/CONTRIBUTING.md
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      163 2022-11-17 10:04:17.000000 pocket_coffea-0.9.2/.github/dependabot.yml
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-30 11:07:18.805909 pocket_coffea-0.9.2/.github/matchers/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      668 2022-11-17 10:04:17.000000 pocket_coffea-0.9.2/.github/matchers/pylint.json
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-30 11:07:18.808909 pocket_coffea-0.9.2/.github/workflows/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2320 2024-05-21 11:47:05.000000 pocket_coffea-0.9.2/.github/workflows/ci.yml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2193 2022-11-17 10:04:17.000000 pocket_coffea-0.9.2/.gitignore
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     3750 2024-05-30 11:01:12.000000 pocket_coffea-0.9.2/.gitlab-ci.yml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2811 2022-11-17 10:04:17.000000 pocket_coffea-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2866 2022-11-17 10:04:17.000000 pocket_coffea-0.9.2/.pyproject_621.toml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      493 2023-11-24 16:51:03.000000 pocket_coffea-0.9.2/.readthedocs.yml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      765 2024-05-30 11:01:12.000000 pocket_coffea-0.9.2/Dockerfile
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1528 2022-11-17 10:04:17.000000 pocket_coffea-0.9.2/LICENSE
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      216 2024-05-30 11:01:12.000000 pocket_coffea-0.9.2/MANIFEST.in
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5291 2024-05-30 11:07:20.346882 pocket_coffea-0.9.2/PKG-INFO
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2572 2023-06-20 15:50:43.000000 pocket_coffea-0.9.2/README.md
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8781 2022-11-17 10:04:17.000000 pocket_coffea-0.9.2/README_old.md
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1888 2024-05-21 11:47:05.000000 pocket_coffea-0.9.2/noxfile.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-30 11:07:18.827908 pocket_coffea-0.9.2/pocket_coffea/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      296 2024-05-30 11:01:12.000000 pocket_coffea-0.9.2/pocket_coffea/__init__.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1676 2024-05-21 22:05:42.000000 pocket_coffea-0.9.2/pocket_coffea/__main__.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      398 2024-05-30 11:04:22.000000 pocket_coffea-0.9.2/pocket_coffea/__meta__.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      467 2024-05-22 14:59:59.000000 pocket_coffea-0.9.2/pocket_coffea/_version.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      118 2022-11-17 10:04:18.000000 pocket_coffea-0.9.2/pocket_coffea/_version.pyi
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-30 11:07:18.872907 pocket_coffea-0.9.2/pocket_coffea/executors/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-21 11:47:05.000000 pocket_coffea-0.9.2/pocket_coffea/executors/__init__.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4441 2024-05-21 22:05:42.000000 pocket_coffea-0.9.2/pocket_coffea/executors/executors_DESY_NAF.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4742 2024-05-21 22:05:42.000000 pocket_coffea-0.9.2/pocket_coffea/executors/executors_RWTH.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4672 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/executors/executors_T3_CH_PSI.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2372 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/executors/executors_base.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1764 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/executors/executors_casa.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5748 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/executors/executors_lxplus.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5569 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/executors/executors_purdue_af.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-30 11:07:18.924907 pocket_coffea-0.9.2/pocket_coffea/lib/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2022-11-17 10:04:18.000000 pocket_coffea-0.9.2/pocket_coffea/lib/__init__.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    18552 2023-06-19 09:09:17.000000 pocket_coffea-0.9.2/pocket_coffea/lib/categorization.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7667 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/lib/columns_manager.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2525 2023-04-28 09:57:29.000000 pocket_coffea-0.9.2/pocket_coffea/lib/cut_definition.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    11948 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/lib/cut_functions.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8598 2023-11-24 16:51:03.000000 pocket_coffea-0.9.2/pocket_coffea/lib/deltaR_matching.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    33045 2024-02-20 13:00:54.000000 pocket_coffea-0.9.2/pocket_coffea/lib/hist_manager.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    10657 2024-05-30 11:01:12.000000 pocket_coffea-0.9.2/pocket_coffea/lib/jets.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6419 2024-05-30 11:01:12.000000 pocket_coffea-0.9.2/pocket_coffea/lib/leptons.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)       43 2022-11-17 10:04:18.000000 pocket_coffea-0.9.2/pocket_coffea/lib/objects.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9121 2023-11-24 16:51:03.000000 pocket_coffea-0.9.2/pocket_coffea/lib/parton_provenance.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    26056 2022-11-17 10:04:18.000000 pocket_coffea-0.9.2/pocket_coffea/lib/reconstruction.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    18597 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/lib/scale_factors.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2307 2024-02-20 13:00:54.000000 pocket_coffea-0.9.2/pocket_coffea/lib/triggers.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    18115 2024-05-21 22:38:49.000000 pocket_coffea-0.9.2/pocket_coffea/lib/weights_manager.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-30 11:07:18.991906 pocket_coffea-0.9.2/pocket_coffea/parameters/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)       24 2023-04-28 09:57:29.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/__init__.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-30 11:07:19.008905 pocket_coffea-0.9.2/pocket_coffea/parameters/btag_SF_calibration/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9336 2023-03-16 13:04:33.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibrationSF_2017UL.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9387 2023-03-16 13:04:33.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibrationSF_2018UL.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2637 2022-11-17 10:04:18.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4048 2022-11-17 10:04:18.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears_v2.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4101 2022-11-17 10:04:18.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears_v3_btagSF-12-09-2022.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4292 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/btagging.yaml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   220921 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/ctagSF_calibrationSF.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      181 2023-11-13 13:19:40.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/cuts.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      848 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/dask_env.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-30 11:07:19.025905 pocket_coffea-0.9.2/pocket_coffea/parameters/datacert/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    11686 2022-11-17 10:04:18.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/datacert/Cert_271036-284044_13TeV_Legacy2016_Collisions16_JSON.txt
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    15830 2022-11-17 10:04:18.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/datacert/Cert_294927-306462_13TeV_UL2017_Collisions17_GoldenJSON.txt
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    15616 2022-11-17 10:04:18.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/datacert/Cert_314472-325175_13TeV_Legacy2018_Collisions18_JSON.txt
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    10178 2024-05-21 11:47:05.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/datacert/Cert_Collisions2022_355100_362760_Golden.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6303 2024-05-21 11:47:05.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/datacert/Cert_Collisions2023_366442_370790_Golden.json
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5753 2024-05-21 11:47:05.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/defaults.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2534 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/event_flags.yaml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1412 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/executor_options_defaults.yaml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    15036 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/histograms.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-30 11:07:19.944889 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    40541 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    40538 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    41031 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    39763 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    38575 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Regrouped_Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    38572 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Regrouped_Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    39465 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Regrouped_Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    37960 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Regrouped_Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      146 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1857 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      146 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1810 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1814 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1RC_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1794 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1RC_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      139 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2L3Residual_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      137 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2L3Residual_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      139 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2L3Residual_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      137 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2L3Residual_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7391 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7386 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7371 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7425 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      137 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Residual_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      135 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Residual_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      137 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Residual_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      135 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Residual_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      135 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L3Absolute_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      133 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L3Absolute_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      135 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L3Absolute_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      133 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L3Absolute_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162003 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162001 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162003 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162001 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK8PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6951 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK4PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6949 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6951 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK8PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6949 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK8PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2413 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2440 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1826 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1RC_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1789 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1RC_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2L3Residual_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2L3Residual_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2L3Residual_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2L3Residual_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7134 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7389 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7039 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7364 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Residual_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Residual_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Residual_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Residual_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L3Absolute_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L3Absolute_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L3Absolute_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L3Absolute_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162000 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   161998 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162000 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   161998 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK8PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6948 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK4PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6946 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6948 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK8PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6946 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK8PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2680 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PF.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2685 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2683 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2680 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PF.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2685 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2683 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2697 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PF.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2702 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2700 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2697 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PF.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2702 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2700 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2485 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PF.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2490 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2488 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2485 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PF.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2490 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2488 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      403 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK4PF.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK4PFPuppi.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      406 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK4PFchs.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      403 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK8PF.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK8PFPuppi.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      406 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK8PFchs.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4222 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK4PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1857 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4217 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK8PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4268 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1834 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK4PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1817 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1811 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK8PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1834 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      131 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK4PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      131 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK8PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    95855 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    90742 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   100572 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    65138 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    91966 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    63555 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      129 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK4PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      129 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK8PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      127 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK4PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      127 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK8PF.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175761 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PF.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175766 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175764 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175761 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PF.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175766 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175764 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7552 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PF.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7557 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7555 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7552 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PF.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7557 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7555 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2741 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2739 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2741 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2739 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2705 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2703 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2705 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2703 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2446 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2444 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2446 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2444 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      410 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_SF_AK4PFPuppi.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_SF_AK4PFchs.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      410 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_SF_AK8PFPuppi.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_SF_AK8PFchs.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2432 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2409 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1798 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1RC_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1798 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1RC_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2L3Residual_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2L3Residual_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2L3Residual_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2L3Residual_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7095 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7336 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7003 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7325 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Residual_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Residual_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Residual_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Residual_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L3Absolute_AK4PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L3Absolute_AK4PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L3Absolute_AK8PFPuppi.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L3Absolute_AK8PFchs.jec.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   173480 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   173413 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   173480 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   173478 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK8PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7206 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK4PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7204 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK4PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7206 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK8PFPuppi.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7204 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK8PFchs.junc.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2814 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2713 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2814 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2713 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2749 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2735 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2749 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2735 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2504 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2490 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2504 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2490 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      410 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_SF_AK4PFPuppi.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_SF_AK4PFchs.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      410 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_SF_AK8PFPuppi.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_SF_AK8PFchs.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2778 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2693 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2778 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2693 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2774 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2692 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2774 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2692 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2524 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2461 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2524 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2461 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      403 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_SF_AK4PFPuppi.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      401 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_SF_AK4PFchs.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      403 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_SF_AK8PFPuppi.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      401 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_SF_AK8PFchs.jersf.txt.gz
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec/__init__.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2587 2023-01-10 11:06:09.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jec_config.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5506 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jet_scale_factors.yaml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    13003 2023-05-23 08:53:32.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/jets_calibration.yaml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5002 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/lepton_scale_factors.yaml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    46204 2024-05-21 11:47:05.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/lumi.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1648 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/lumi.yaml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1395 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/pileup.yaml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2132 2024-05-21 11:47:05.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/plotting_style.yaml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1127 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/parameters/variations.yaml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2022-11-17 10:04:18.000000 pocket_coffea-0.9.2/pocket_coffea/py.typed
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-30 11:07:20.159885 pocket_coffea-0.9.2/pocket_coffea/scripts/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-21 11:47:05.000000 pocket_coffea-0.9.2/pocket_coffea/scripts/__init__.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8969 2024-05-21 11:47:05.000000 pocket_coffea-0.9.2/pocket_coffea/scripts/build_jec.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-30 11:07:20.181885 pocket_coffea-0.9.2/pocket_coffea/scripts/dataset/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-21 11:47:05.000000 pocket_coffea-0.9.2/pocket_coffea/scripts/dataset/__init__.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1100 2024-05-21 11:47:05.000000 pocket_coffea-0.9.2/pocket_coffea/scripts/dataset/append_genweights.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1508 2024-05-21 11:47:05.000000 pocket_coffea-0.9.2/pocket_coffea/scripts/dataset/append_parents.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2532 2024-05-30 11:01:12.000000 pocket_coffea-0.9.2/pocket_coffea/scripts/dataset/build_datasets.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    26704 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/scripts/dataset/dataset_query.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2185 2024-05-21 11:47:05.000000 pocket_coffea-0.9.2/pocket_coffea/scripts/dataset/download.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     3591 2024-05-21 11:47:05.000000 pocket_coffea-0.9.2/pocket_coffea/scripts/hadd_skimmed_files.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-30 11:07:20.188885 pocket_coffea-0.9.2/pocket_coffea/scripts/lumi/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1302 2024-05-21 11:47:05.000000 pocket_coffea-0.9.2/pocket_coffea/scripts/lumi/filter_lumi_json.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1741 2024-05-21 11:47:05.000000 pocket_coffea-0.9.2/pocket_coffea/scripts/lumi/run_brilcalc.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      650 2024-05-30 11:01:12.000000 pocket_coffea-0.9.2/pocket_coffea/scripts/merge_outputs.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-30 11:07:20.200884 pocket_coffea-0.9.2/pocket_coffea/scripts/plot/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-21 11:47:05.000000 pocket_coffea-0.9.2/pocket_coffea/scripts/plot/__init__.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5178 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/scripts/plot/make_plots.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8656 2024-05-21 11:47:05.000000 pocket_coffea-0.9.2/pocket_coffea/scripts/plot/trigger_efficiency.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2060 2024-05-21 11:47:05.000000 pocket_coffea-0.9.2/pocket_coffea/scripts/plot/trigger_scalefactor.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9711 2024-05-30 11:01:12.000000 pocket_coffea-0.9.2/pocket_coffea/scripts/runner.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    22625 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/scripts/runner_old.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-30 11:07:20.250883 pocket_coffea-0.9.2/pocket_coffea/utils/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2022-11-17 10:04:18.000000 pocket_coffea-0.9.2/pocket_coffea/utils/__init__.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2812 2023-04-28 09:57:29.000000 pocket_coffea-0.9.2/pocket_coffea/utils/build_jets_calibrator.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    26572 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/utils/configurator.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14920 2024-05-30 11:01:12.000000 pocket_coffea-0.9.2/pocket_coffea/utils/dataset.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      193 2023-06-20 09:07:30.000000 pocket_coffea-0.9.2/pocket_coffea/utils/load_output.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4644 2022-11-20 17:13:41.000000 pocket_coffea-0.9.2/pocket_coffea/utils/logging.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      910 2022-11-17 10:04:18.000000 pocket_coffea-0.9.2/pocket_coffea/utils/network.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    55055 2023-11-24 16:51:03.000000 pocket_coffea-0.9.2/pocket_coffea/utils/plot_efficiency.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2764 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/utils/plot_functions.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7472 2023-11-24 16:51:03.000000 pocket_coffea-0.9.2/pocket_coffea/utils/plot_sf.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    45197 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/utils/plot_utils.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    12400 2024-05-30 11:01:12.000000 pocket_coffea-0.9.2/pocket_coffea/utils/rucio.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    10867 2023-11-24 16:51:03.000000 pocket_coffea-0.9.2/pocket_coffea/utils/run.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2517 2023-11-24 16:51:03.000000 pocket_coffea-0.9.2/pocket_coffea/utils/skim.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2646 2023-11-24 16:51:03.000000 pocket_coffea-0.9.2/pocket_coffea/utils/utils.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-30 11:07:20.269883 pocket_coffea-0.9.2/pocket_coffea/workflows/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2022-11-17 10:04:18.000000 pocket_coffea-0.9.2/pocket_coffea/workflows/__init__.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    38761 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/workflows/base.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1665 2023-04-28 09:57:29.000000 pocket_coffea-0.9.2/pocket_coffea/workflows/genweights.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1589 2023-02-28 09:29:31.000000 pocket_coffea-0.9.2/pocket_coffea/workflows/semileptonic_triggerSF.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1581 2022-11-17 10:04:18.000000 pocket_coffea-0.9.2/pocket_coffea/workflows/sf_lepton_variations.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4740 2024-05-21 22:05:43.000000 pocket_coffea-0.9.2/pocket_coffea/workflows/tthbb_base_processor.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-30 11:07:20.338882 pocket_coffea-0.9.2/pocket_coffea.egg-info/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5291 2024-05-30 11:07:17.000000 pocket_coffea-0.9.2/pocket_coffea.egg-info/PKG-INFO
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    22660 2024-05-30 11:07:18.000000 pocket_coffea-0.9.2/pocket_coffea.egg-info/SOURCES.txt
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        1 2024-05-30 11:07:17.000000 pocket_coffea-0.9.2/pocket_coffea.egg-info/dependency_links.txt
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      465 2024-05-30 11:07:17.000000 pocket_coffea-0.9.2/pocket_coffea.egg-info/entry_points.txt
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      455 2024-05-30 11:07:17.000000 pocket_coffea-0.9.2/pocket_coffea.egg-info/requires.txt
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)       14 2024-05-30 11:07:17.000000 pocket_coffea-0.9.2/pocket_coffea.egg-info/top_level.txt
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-30 11:07:20.297883 pocket_coffea-0.9.2/profiling/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1882 2022-06-15 09:24:30.000000 pocket_coffea-0.9.2/profiling/mem.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)  1703383 2022-06-29 14:04:29.000000 pocket_coffea-0.9.2/profiling/parton_matching_semilep_newgenmatch_v4.prof
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)  1703285 2022-06-29 14:04:29.000000 pocket_coffea-0.9.2/profiling/parton_matching_semilep_v3.prof
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2956 2024-05-30 11:01:12.000000 pocket_coffea-0.9.2/pyproject.toml
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      234 2024-05-30 11:01:12.000000 pocket_coffea-0.9.2/requirements.txt
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)       38 2024-05-30 11:07:20.349882 pocket_coffea-0.9.2/setup.cfg
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      387 2022-11-17 10:04:18.000000 pocket_coffea-0.9.2/setup.py
-drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2024-05-30 11:07:20.335882 pocket_coffea-0.9.2/tests/
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      776 2023-02-07 15:21:45.000000 pocket_coffea-0.9.2/tests/test_categorization.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1696 2022-11-20 17:13:42.000000 pocket_coffea-0.9.2/tests/test_hlt_cut.py
--rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      205 2024-02-20 13:00:54.000000 pocket_coffea-0.9.2/tests/test_package.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.400091 pocket_coffea-1.0rc3/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      119 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/.flake8
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      125 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/.git_archival.txt
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)       32 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/.gitattributes
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.147113 pocket_coffea-1.0rc3/.github/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2405 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/.github/CONTRIBUTING.md
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      163 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/.github/dependabot.yml
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.150113 pocket_coffea-1.0rc3/.github/matchers/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      668 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/.github/matchers/pylint.json
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.153113 pocket_coffea-1.0rc3/.github/workflows/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2320 2023-08-21 09:28:59.000000 pocket_coffea-1.0rc3/.github/workflows/ci.yml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2193 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/.gitignore
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2276 2023-08-11 20:33:24.000000 pocket_coffea-1.0rc3/.gitlab-ci.yml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2811 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/.pre-commit-config.yaml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2866 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/.pyproject_621.toml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      396 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/.readthedocs.yml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      656 2023-08-11 20:33:24.000000 pocket_coffea-1.0rc3/Dockerfile
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1528 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/LICENSE
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      133 2023-06-15 11:17:16.000000 pocket_coffea-1.0rc3/MANIFEST.in
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4083 2023-10-10 07:02:02.401091 pocket_coffea-1.0rc3/PKG-INFO
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2572 2023-06-20 15:50:43.000000 pocket_coffea-1.0rc3/README.md
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8781 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/README_old.md
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1880 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/noxfile.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.163113 pocket_coffea-1.0rc3/pocket_coffea/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      250 2022-11-17 10:04:17.000000 pocket_coffea-1.0rc3/pocket_coffea/__init__.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      465 2023-10-09 20:55:20.000000 pocket_coffea-1.0rc3/pocket_coffea/_version.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      118 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/_version.pyi
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.214112 pocket_coffea-1.0rc3/pocket_coffea/lib/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/__init__.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    18552 2023-06-19 09:09:17.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/categorization.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7410 2023-08-11 21:53:54.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/columns_manager.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2525 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/cut_definition.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    10391 2023-05-05 11:27:53.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/cut_functions.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8598 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/deltaR_matching.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    33055 2023-08-21 09:58:18.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/hist_manager.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9338 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/jets.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5232 2023-05-25 16:41:04.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/leptons.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)       43 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/objects.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9121 2023-07-04 13:28:25.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/parton_provenance.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    26056 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/reconstruction.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    15676 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/scale_factors.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2258 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/triggers.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    16046 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/pocket_coffea/lib/weights_manager.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.255111 pocket_coffea-1.0rc3/pocket_coffea/parameters/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)       24 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/__init__.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.267111 pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9336 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibrationSF_2017UL.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9387 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibrationSF_2018UL.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2637 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4048 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears_v2.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4101 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears_v3_btagSF-12-09-2022.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1520 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/btagging.yaml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      181 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/cuts.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      848 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/dask_env.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.275111 pocket_coffea-1.0rc3/pocket_coffea/parameters/datacert/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    11686 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/datacert/Cert_271036-284044_13TeV_Legacy2016_Collisions16_JSON.txt
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    15830 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/datacert/Cert_294927-306462_13TeV_UL2017_Collisions17_GoldenJSON.txt
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    15616 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/datacert/Cert_314472-325175_13TeV_Legacy2018_Collisions18_JSON.txt
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5569 2023-06-20 09:43:20.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/defaults.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1323 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/event_flags.yaml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    13181 2023-06-21 15:11:53.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/histograms.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.822101 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    40541 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    40538 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    41031 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    39763 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    38575 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Regrouped_Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    38572 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Regrouped_Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    39465 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Regrouped_Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    37960 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Regrouped_Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      146 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1857 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      146 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1810 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1814 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1RC_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1794 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1RC_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      139 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2L3Residual_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      137 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2L3Residual_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      139 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2L3Residual_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      137 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2L3Residual_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7391 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7386 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7371 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7425 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      137 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Residual_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      135 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Residual_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      137 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Residual_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      135 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Residual_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      135 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L3Absolute_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      133 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L3Absolute_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      135 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L3Absolute_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      133 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L3Absolute_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162003 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162001 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162003 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162001 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK8PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6951 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK4PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6949 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6951 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK8PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6949 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK8PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2413 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2440 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1826 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1RC_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1789 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1RC_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2L3Residual_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2L3Residual_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2L3Residual_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2L3Residual_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7389 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7039 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7364 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Residual_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Residual_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Residual_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Residual_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L3Absolute_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L3Absolute_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L3Absolute_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L3Absolute_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162000 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   161998 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   162000 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   161998 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK8PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6948 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK4PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6946 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6948 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK8PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6946 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK8PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2680 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PF.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2685 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2683 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2680 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PF.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2685 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2683 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2697 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PF.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2702 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2700 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2697 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PF.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2702 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2700 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2485 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PF.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2490 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2488 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2485 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PF.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2490 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2488 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      403 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK4PF.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK4PFPuppi.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      406 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK4PFchs.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      403 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK8PF.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK8PFPuppi.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      406 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_SF_AK8PFchs.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4222 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK4PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1857 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4217 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK8PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4268 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1834 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK4PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1817 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1811 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK8PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1834 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      131 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK4PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      131 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK8PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2L3Residual_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    95855 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    90742 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   100572 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    65138 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    91966 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    63555 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      129 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK4PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      129 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK8PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Residual_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      127 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK4PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      127 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK8PF.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L3Absolute_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175761 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PF.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175766 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175764 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175761 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PF.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175766 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   175764 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7552 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PF.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7557 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7555 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7552 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PF.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7557 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7555 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2741 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2739 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2741 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2739 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2705 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2703 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2705 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2703 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2446 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2444 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2446 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2444 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      410 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_SF_AK4PFPuppi.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_SF_AK4PFchs.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      410 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_SF_AK8PFPuppi.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_SF_AK8PFchs.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2432 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      143 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2409 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1798 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1RC_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1798 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1RC_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2L3Residual_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2L3Residual_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      136 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2L3Residual_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2L3Residual_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7095 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7336 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7003 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7325 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Residual_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Residual_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      134 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Residual_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Residual_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L3Absolute_AK4PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L3Absolute_AK4PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      132 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L3Absolute_AK8PFPuppi.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      130 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L3Absolute_AK8PFchs.jec.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   173480 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   173413 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   173480 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)   173478 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK8PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7206 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK4PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7204 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK4PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7206 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK8PFPuppi.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7204 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK8PFchs.junc.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2814 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2713 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2814 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2713 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2749 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2735 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2749 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2735 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2504 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2490 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2504 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2490 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      410 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_SF_AK4PFPuppi.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_SF_AK4PFchs.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      410 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_SF_AK8PFPuppi.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      408 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_SF_AK8PFchs.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2778 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2693 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2778 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2693 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2774 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2692 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2774 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2692 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2524 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2461 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2524 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2461 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      403 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_SF_AK4PFPuppi.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      401 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_SF_AK4PFchs.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      403 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_SF_AK8PFPuppi.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      401 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_SF_AK8PFchs.jersf.txt.gz
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/__init__.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2587 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jec_config.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1429 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jet_scale_factors.yaml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    13003 2023-05-23 08:53:32.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/jets_calibration.yaml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     3201 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/lepton_scale_factors.yaml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    45900 2023-01-10 11:06:09.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/lumi.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      977 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/lumi.yaml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      672 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/pileup.yaml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1824 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/plotting_style.yaml
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.091114 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.830101 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2017/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    54894 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2017/sf_trigger_electron_etaSC_phi_leading_2017_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    48984 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2017/sf_trigger_electron_etaSC_pt_leading_2017_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    34659 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2017/sf_trigger_electron_phi_pt_leading_2017_Ele32_EleHT_pass.json
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.861101 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19688 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19728 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v01.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19807 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v02.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19726 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v03.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14692 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14724 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v01.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14794 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v02.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14721 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v03.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8517 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8547 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v01.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8588 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v02.coffea
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8552 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018UL_Ele32_EleHT/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v03.coffea
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.239094 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    10370 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v03.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v04.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v05.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v06.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v07.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v08.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v09.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v10.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v11.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v12.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v13.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v14.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8396 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_2018_Ele32_EleHT_pass_v15.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19663 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19663 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19654 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19654 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v03.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19654 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v04.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    32392 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v05.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    83387 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v06.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    83387 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v07.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    83387 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v08.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    64399 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass_v09.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    16291 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    16291 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    16289 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    16289 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v03.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    16289 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v04.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    26777 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v05.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68809 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v06.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68809 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v07.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68809 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v08.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    58725 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass_v09.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    10682 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_eta_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8705 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_eta_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8705 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_eta_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14503 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14503 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    14503 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9225 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9225 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9214 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9214 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v03.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     9214 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v04.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    15002 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v05.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    38167 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v06.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    38167 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v07.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    38167 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v08.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    41466 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass_v09.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6238 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v03.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v04.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v05.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v06.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v07.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v08.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v09.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v10.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v11.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v12.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v13.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v14.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v15.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v16.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v17.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v18.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v19.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v20.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v21.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v22.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v23.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v24.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v25.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v26.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v27.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v28.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v29.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v30.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v31.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6098 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v32.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5415 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v33.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5415 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v34.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     5415 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_electron_pt_2018_Ele32_EleHT_pass_v35.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    23172 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    23172 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    21566 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    21566 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass_v03.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    21566 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_ht_2018_Ele32_EleHT_pass_v04.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    31656 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_eta_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    31653 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_eta_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    31653 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_eta_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68662 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_phi_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68659 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_phi_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68659 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_phi_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    48639 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_pt_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    48639 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_pt_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    45165 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_jet_pt_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    31635 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_eta_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    31630 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_eta_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    31630 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_eta_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68624 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_phi_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68626 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_phi_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    68626 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_phi_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    44287 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_pt_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    44284 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_pt_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    43386 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_muon_pt_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6124 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nbjet_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6122 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nbjet_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6064 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nbjet_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2925 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nelectron_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2926 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nelectron_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2926 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nelectron_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7185 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7190 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7190 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7190 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v03.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7190 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v04.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4304 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v05.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4304 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v06.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4304 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v07.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4304 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v08.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4214 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v09.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4214 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v10.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4214 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_njet_2018_Ele32_EleHT_pass_v11.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2857 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nlep_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2858 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nlep_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2858 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nlep_2018_Ele32_EleHT_pass_v02.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2872 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nmuon_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2873 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nmuon_2018_Ele32_EleHT_pass_v01.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2873 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics/sf_trigger_nmuon_2018_Ele32_EleHT_pass_v02.json
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.250094 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics_single_endcap_bin/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    58051 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics_single_endcap_bin/sf_trigger_electron_etaSC_vs_electron_phi_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    52902 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics_single_endcap_bin/sf_trigger_electron_etaSC_vs_electron_pt_2018_Ele32_EleHT_pass.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    41467 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_Ele32_EleHT_allsystematics_single_endcap_bin/sf_trigger_electron_phi_vs_electron_pt_2018_Ele32_EleHT_pass.json
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.261094 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_sfmutrigger/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    54868 2023-02-28 08:21:16.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_sfmutrigger/sf_trigger_electron_etaSC_phi_leading_2018_Ele32_EleHT_pass_v06.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    48959 2023-02-28 08:21:16.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_sfmutrigger/sf_trigger_electron_etaSC_pt_leading_2018_Ele32_EleHT_pass_v06.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    34639 2023-02-28 08:21:16.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/semileptonic_triggerSF/triggerSF_2018_sfmutrigger/sf_trigger_electron_phi_pt_leading_2018_Ele32_EleHT_pass_v06.json
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      619 2023-08-21 09:58:11.000000 pocket_coffea-1.0rc3/pocket_coffea/parameters/variations.yaml
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/py.typed
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.300093 pocket_coffea-1.0rc3/pocket_coffea/utils/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/__init__.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2812 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/build_jets_calibrator.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    26297 2023-08-11 20:40:20.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/configurator.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    13581 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/dataset.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      193 2023-06-20 09:07:30.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/load_output.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4644 2022-11-20 17:13:41.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/logging.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      910 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/network.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    55055 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/plot_efficiency.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     7472 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/plot_sf.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    39639 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/plot_utils.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6614 2023-07-05 16:40:29.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/rucio.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    10867 2023-10-10 07:00:58.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/run.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2517 2023-07-05 13:00:35.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/skim.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2646 2023-07-05 13:03:18.000000 pocket_coffea-1.0rc3/pocket_coffea/utils/utils.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.316093 pocket_coffea-1.0rc3/pocket_coffea/workflows/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        0 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/workflows/__init__.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    34647 2023-08-30 09:36:12.000000 pocket_coffea-1.0rc3/pocket_coffea/workflows/base.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1665 2023-04-28 09:57:29.000000 pocket_coffea-1.0rc3/pocket_coffea/workflows/genweights.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1589 2023-02-28 09:29:31.000000 pocket_coffea-1.0rc3/pocket_coffea/workflows/semileptonic_triggerSF.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1581 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pocket_coffea/workflows/sf_lepton_variations.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4686 2023-05-05 11:27:53.000000 pocket_coffea-1.0rc3/pocket_coffea/workflows/tthbb_base_processor.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:01.176113 pocket_coffea-1.0rc3/pocket_coffea.egg-info/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4083 2023-10-10 07:01:58.000000 pocket_coffea-1.0rc3/pocket_coffea.egg-info/PKG-INFO
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    44386 2023-10-10 07:02:00.000000 pocket_coffea-1.0rc3/pocket_coffea.egg-info/SOURCES.txt
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)        1 2023-10-10 07:01:58.000000 pocket_coffea-1.0rc3/pocket_coffea.egg-info/dependency_links.txt
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      448 2023-10-10 07:01:58.000000 pocket_coffea-1.0rc3/pocket_coffea.egg-info/requires.txt
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)       14 2023-10-10 07:01:58.000000 pocket_coffea-1.0rc3/pocket_coffea.egg-info/top_level.txt
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.337092 pocket_coffea-1.0rc3/profiling/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1882 2022-06-15 09:24:30.000000 pocket_coffea-1.0rc3/profiling/mem.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)  1703383 2022-06-29 14:04:29.000000 pocket_coffea-1.0rc3/profiling/parton_matching_semilep_newgenmatch_v4.prof
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)  1703285 2022-06-29 14:04:29.000000 pocket_coffea-1.0rc3/profiling/parton_matching_semilep_v3.prof
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1131 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/pyproject.toml
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.363092 pocket_coffea-1.0rc3/scripts/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8969 2023-05-30 08:29:35.000000 pocket_coffea-1.0rc3/scripts/build_jec.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     6976 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc3/scripts/compute_btagSF_calibration.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.375092 pocket_coffea-1.0rc3/scripts/dataset/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1100 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc3/scripts/dataset/append_genweights.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1508 2023-03-16 13:04:33.000000 pocket_coffea-1.0rc3/scripts/dataset/append_parents.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2142 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/scripts/dataset/build_datasets.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2185 2023-02-28 08:58:11.000000 pocket_coffea-1.0rc3/scripts/dataset/download.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     3275 2023-02-28 08:58:11.000000 pocket_coffea-1.0rc3/scripts/hadd_skimmed_files.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.381092 pocket_coffea-1.0rc3/scripts/lumi/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1302 2023-02-28 09:34:38.000000 pocket_coffea-1.0rc3/scripts/lumi/filter_lumi_json.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1741 2023-02-28 09:34:38.000000 pocket_coffea-1.0rc3/scripts/lumi/run_brilcalc.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      580 2023-05-18 10:10:56.000000 pocket_coffea-1.0rc3/scripts/merge_outputs.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.389092 pocket_coffea-1.0rc3/scripts/plot/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     4201 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/scripts/plot/make_plots.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     8656 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/scripts/plot/trigger_efficiency.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2060 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/scripts/plot/trigger_scalefactor.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)    19389 2023-10-09 20:53:31.000000 pocket_coffea-1.0rc3/scripts/runner.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     2194 2023-10-10 07:02:02.404091 pocket_coffea-1.0rc3/setup.cfg
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      387 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/setup.py
+drwxr-xr-x   0 dvalsecc   (741) ethz-higgs   (532)        0 2023-10-10 07:02:02.398091 pocket_coffea-1.0rc3/tests/
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      776 2023-02-07 15:21:45.000000 pocket_coffea-1.0rc3/tests/test_categorization.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)     1696 2022-11-20 17:13:42.000000 pocket_coffea-1.0rc3/tests/test_hlt_cut.py
+-rw-r--r--   0 dvalsecc   (741) ethz-higgs   (532)      109 2022-11-17 10:04:18.000000 pocket_coffea-1.0rc3/tests/test_package.py
```

### Comparing `pocket_coffea-0.9.2/.github/CONTRIBUTING.md` & `pocket_coffea-1.0rc3/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/.github/matchers/pylint.json` & `pocket_coffea-1.0rc3/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/.github/workflows/ci.yml` & `pocket_coffea-1.0rc3/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -20,21 +20,21 @@
   FORCE_COLOR: 3
 
 jobs:
   pre-commit:
     name: Format
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
-      - uses: actions/setup-python@v5
+      - uses: actions/setup-python@v4
         with:
           python-version: "3.x"
-      - uses: pre-commit/action@v3.0.1
+      - uses: pre-commit/action@v3.0.0
         with:
           extra_args: --hook-stage manual --all-files
       - name: Run PyLint
         run: |
           echo "::add-matcher::$GITHUB_WORKSPACE/.github/matchers/pylint.json"
           pipx run nox -s pylint
 
@@ -49,51 +49,51 @@
         runs-on: [ubuntu-latest, macos-latest, windows-latest]
 
         include:
           - python-version: pypy-3.8
             runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
-      - uses: actions/setup-python@v5
+      - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install package
         run: python -m pip install .[test]
 
       - name: Test package
         run: python -m pytest -ra --cov=PocketCoffea
 
       - name: Upload coverage report
-        uses: codecov/codecov-action@v4.0.1
+        uses: codecov/codecov-action@v3.1.1
 
   dist:
     name: Distribution build
     runs-on: ubuntu-latest
     needs: [pre-commit]
 
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Build sdist and wheel
         run: pipx run build
 
-      - uses: actions/upload-artifact@v4
+      - uses: actions/upload-artifact@v3
         with:
           path: dist
 
       - name: Check products
         run: pipx run twine check dist/*
 
-      - uses: pypa/gh-action-pypi-publish@v1.8.11
+      - uses: pypa/gh-action-pypi-publish@v1.8.10
         if: github.event_name == 'release' && github.event.action == 'published'
         with:
           # Remember to generate this and set it in "GitHub Secrets"
           password: ${{ secrets.pypi_password }}
           # Remove this line
           repository_url: https://test.pypi.org/legacy/
```

### Comparing `pocket_coffea-0.9.2/.gitignore` & `pocket_coffea-1.0rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/.pre-commit-config.yaml` & `pocket_coffea-1.0rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/.pyproject_621.toml` & `pocket_coffea-1.0rc3/.pyproject_621.toml`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/Dockerfile` & `pocket_coffea-1.0rc3/Dockerfile`

 * *Files 25% similar despite different names*

```diff
@@ -9,12 +9,11 @@
     echo "Installing PocketCoffea" && \
     echo "on cluster environment: $CLUSTER" && \
     echo "Current time:" $(date) && \
     echo "=======================================" && \
     if [[ ${CLUSTER} == "lxplus" ]]; then \
         echo "Fixing dependencies in the image" && \
         conda install -y numba>=0.57.0 llvmlite==0.40.0 numpy>=1.22.0 && \
-        python -m pip install -U dask-lxplus==0.3.2 dask-jobqueue==0.8.2; \
+        pip install --upgrade dask-lxplus; \
     fi && \
     echo "Installing PocketCoffea" && \
-    python -m pip install -U setuptools setuptools-scm &&\
-    python -m pip install . --verbose
+    pip3 install .
```

### Comparing `pocket_coffea-0.9.2/LICENSE` & `pocket_coffea-1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/README.md` & `pocket_coffea-1.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/README_old.md` & `pocket_coffea-1.0rc3/README_old.md`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/noxfile.py` & `pocket_coffea-1.0rc3/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 def docs(session: nox.Session) -> None:
     """
     Build the docs. Pass "serve" to serve.
     """
 
     session.install(".[docs]")
     session.chdir("docs")
-    session.run("sphinx-apidoc","-o", "modules", "../pocket_coffea")
+    session.run("sphinx-apidoc -o modules ../pocket_coffea")
     session.run("sphinx-build", "-M", "html", ".", "_build")
 
     if session.posargs:
         if "serve" in session.posargs:
             print("Launching docs at http://localhost:8000/ - use Ctrl-C to quit")
             session.run("python", "-m", "http.server", "8000", "-d", "_build/html")
         else:
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/lib/categorization.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/categorization.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/lib/columns_manager.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/columns_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import awkward as ak
 
 
 @dataclass
 class ColOut:
     collection: str  # Collection
     columns: List[str]  # list of columns to export
-    flatten: bool = True  # Flatten by default
+    flatten: bool = True  # Flatten by defaul
     store_size: bool = True
     fill_none: bool = True
     fill_value: float = -999.0  # by default the None elements are filled
     pos_start: int = None  # First position in the collection to export. If None export from the first element
     pos_end: int = None  # Last position in the collection to export. If None export until the last element
 
 
@@ -55,18 +55,15 @@
                         != self.categories_config.multidim_collection
                     ):
                         raise Exception(
                             f"Applying mask on collection {self.categories_config.multidim_collection}, \
                             while exporting collection {outarray.collection}! Please check your categorization"
                         )
                 # Applying mask after getting the collection
-                if(outarray.collection=="events"):
-                    data = events[mask]
-                else:
-                    data = events[outarray.collection][mask]
+                data = events[outarray.collection][mask]
 
                 # Filtering the position in the collection if needed
                 if outarray.pos_start and outarray.pos_end:
                     data = data[:, outarray.pos_start : outarray.pos_end]
                 elif outarray.pos_start and not outarray.pos_end:
                     data = data[:, outarray.pos_start :]
                 elif not outarray.pos_start and outarray.pos_end:
@@ -132,30 +129,26 @@
                         != self.categories_config.multidim_collection
                     ):
                         raise Exception(
                             f"Applying mask on collection {self.categories_config.multidim_collection}, \
                             while exporting collection {outarray.collection}! Please check your categorization"
                         )
                 # Applying mask after getting the collection
-                if(outarray.collection=="events"):
-                    data = events[mask]
-                else:
-                    data = events[outarray.collection][mask]
+                data = events[outarray.collection][mask]
 
                 # Filtering the position in the collection if needed
                 if outarray.pos_start and outarray.pos_end:
                     data = data[:, outarray.pos_start : outarray.pos_end]
                 elif outarray.pos_start and not outarray.pos_end:
                     data = data[:, outarray.pos_start :]
                 elif not outarray.pos_start and outarray.pos_end:
                     data = data[:, : outarray.pos_end]
 
-                if outarray.store_size and data.ndim > 1:
-                    N = ak.num(data)
-                    out_by_cat[f"{outarray.collection}_N"] = N
+                # if outarray.store_size and data.ndim > 1:
+                #     out_by_cat[f"{outarray.collection}_N"] = ak.num(data)
 
                 # looping on the columns
                 for col in outarray.columns:
                     if outarray.flatten and data.ndim > 1:
                         if outarray.fill_none:
                             out = ak.fill_none(
                                 ak.flatten(data[col]),
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/lib/cut_definition.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/cut_definition.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/lib/cut_functions.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/cut_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import awkward as ak
 from .cut_definition import Cut
 from .triggers import get_trigger_mask
-import correctionlib
-import numpy as np
 
 
 def passthrough_f(events, **kargs):
     '''
     Identity cut:  passthrough of all events.
     '''
     return ak.full_like(events.event, True, dtype=bool)
@@ -47,44 +45,14 @@
         name += "_NOT"
     return Cut(
         name=name,
         params={"primaryDatasets": primaryDatasets, "invert": invert},
         function=_get_trigger_mask_proxy,
     )
 
-###########################
-## Implementation of JetVetoMaps 
-## (Recommended for Run 3, see https://cms-jerc.web.cern.ch/Recommendations/#jet-veto-maps)
-
-def get_JetVetoMap(name="JetVetoMaps"):
-    return Cut(
-        name=name, params={}, function=get_JetVetoMap_Mask
-    )
-       
-def get_JetVetoMap_Mask(events, params, year, processor_params, sample, isMC, **kwargs):
-    jets = events.Jet
-    mask_for_VetoMap = (
-        ((jets.jetId & 2)==2) # Must fulfill tight jetId
-        & (abs(jets.eta) < 5.19) # Must be within HCal acceptance
-        & (jets.pt*(1-jets.muonSubtrFactor) > 15.) # May no be Muons misreconstructed as jets
-        & ((jets["neEmEF"]+jets["chEmEF"])<0.9) # Energy fraction not dominated by ECal
-    )
-    jets = jets[mask_for_VetoMap]
-    cset = correctionlib.CorrectionSet.from_file(
-        processor_params.jet_scale_factors.vetomaps[year]["file"]
-    )
-    corr = cset[processor_params.jet_scale_factors.vetomaps[year]["name"]]
-    etaFlat, phiFlat, etaCounts = ak.flatten(jets.eta), ak.flatten(jets.phi), ak.num(jets.eta)
-    phiFlat = np.clip(phiFlat, -3.14159, 3.14159) # Needed since no overflow included in phi binning
-    weight = ak.unflatten(
-        corr.evaluate("jetvetomap", etaFlat, phiFlat),
-        counts=etaCounts,
-    )
-    eventMask = ak.sum(weight, axis=-1)==0 # if at least one jet is vetoed, reject it event
-    return ak.where(ak.is_none(eventMask), False, eventMask)
 
 ###########################
 ## Functions to count objects
 def count_objects_gt(events, params, **kwargs):
     '''
     Count the number of objects in `params["object"]` and
     keep only events with larger (>) amount than `params["value"]`.
@@ -229,27 +197,27 @@
     else:
         btagparam = processor_params.btagging.working_point[year]
         if params["minpt"] > 0.0:
             return (
                 ak.sum(
                     (
                         events[params["coll"]][btagparam["btagging_algorithm"]]
-                        > btagparam["btagging_WP"][params["wp"]]
+                        > btagparam["btagging_WP"]
                     )
                     & (events[params["coll"]].pt >= params["minpt"]),
                     axis=1,
                 )
                 >= params["N"]
             )
         else:
             return (
                 ak.sum(
                     (
                         events[params["coll"]][btagparam["btagging_algorithm"]]
-                        > btagparam["btagging_WP"][params["wp"]]
+                        > btagparam["btagging_WP"]
                     ),
                     axis=1,
                 )
                 >= params["N"]
             )
 
 
@@ -269,27 +237,27 @@
     else:
         btagparam = processor_params.btagging.working_point[year]
         if params["minpt"] > 0.0:
             return (
                 ak.sum(
                     (
                         events[params["coll"]][btagparam["btagging_algorithm"]]
-                        > btagparam["btagging_WP"][params["wp"]]
+                        > btagparam["btagging_WP"]
                     )
                     & (events[params["coll"]].pt >= params["minpt"]),
                     axis=1,
                 )
                 == params["N"]
             )
         else:
             return (
                 ak.sum(
                     (
                         events[params["coll"]][btagparam["btagging_algorithm"]]
-                        > btagparam["btagging_WP"][params["wp"]]
+                        > btagparam["btagging_WP"]
                     ),
                     axis=1,
                 )
                 == params["N"]
             )
 
 
@@ -313,27 +281,27 @@
         raise Exception(f"The collection '{params['coll']}' does not exist.")
 
 
 ##########################33
 ## Factory methods
 
 
-def get_nBtagMin(N, minpt=0, coll="BJetGood", wp="M", name=None):
+def get_nBtagMin(N, minpt=0, coll="BJetGood", name=None):
     if name == None:
         name = f"n{coll}_btagMin{N}_pt{minpt}"
     return Cut(
-        name=name, params={"N": N, "coll": coll, "minpt": minpt, "wp": wp}, function=nBtagMin
+        name=name, params={"N": N, "coll": coll, "minpt": minpt}, function=nBtagMin
     )
 
 
-def get_nBtagEq(N, minpt=0, coll="BJetGood", wp="M", name=None):
+def get_nBtagEq(N, minpt=0, coll="BJetGood", name=None):
     if name == None:
         name = f"n{coll}_btagEq{N}_pt{minpt}"
     return Cut(
-        name=name, params={"N": N, "coll": coll, "minpt": minpt, "wp": wp}, function=nBtagEq
+        name=name, params={"N": N, "coll": coll, "minpt": minpt}, function=nBtagEq
     )
 
 
 def get_nBtag(*args, **kwargs):
     raise Exception(
         "This cut function factory is deprecated!! Use get_nBtagMin or get_nBtagEq instead."
     )
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/lib/deltaR_matching.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/deltaR_matching.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/lib/hist_manager.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/hist_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,18 +202,18 @@
         # Prepare the variations Axes summing all the required variations
         # The variation config is organized as the weights one, by sample and by category
 
         for name, hcfg in deepcopy(hist_config).items():
             # Check if the histogram is active for the current sample
             # We only check for the parent sample, not for subsamples
             if hcfg.only_samples != None:
-                if sample not in cfg.only_samples:
+                if self.sample not in cfg.only_samples:
                     continue
             elif hcfg.exclude_samples != None:
-                if sample in hcfg.exclude_samples:
+                if self.sample in hcfg.exclude_samples:
                     continue
             # Now we handle the selection of the categories
             cats = []
             for c in self.available_categories:
                 if hcfg.only_categories != None:
                     if c in hcfg.only_categories:
                         cats.append(c)
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/lib/jets.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/jets.py`

 * *Files 8% similar despite different names*

```diff
@@ -213,64 +213,22 @@
     )
     # Lepton cleaning
     if leptons_collection != "":
         dR_jets_lep = jets.metric_table(events[leptons_collection])
         mask_lepton_cleaning = ak.prod(dR_jets_lep > cuts["dr_lepton"], axis=2) == 1
 
     if jet_type == "Jet":
-        # Selection on PUid. Only available in Run2 UL, thus we need to determine which sample we run over;
-        if events.metadata["year"] in ['2016_PreVFP', '2016_PostVFP','2017','2018']:
-            mask_jetpuid = (jets.puId >= params.jet_scale_factors.jet_puId[events.metadata["year"]]["working_point"][cuts["puId"]["wp"]]) | (
-                jets.pt >= cuts["puId"]["maxpt"]
-            )
-        else:
-            mask_jetpuid = True
-  
+        mask_jetpuid = (jets.puId >= cuts["puId"]["value"]) | (
+            jets.pt >= cuts["puId"]["maxpt"]
+        )
         mask_good_jets = mask_presel & mask_lepton_cleaning & mask_jetpuid
 
     elif jet_type == "FatJet":
         # Apply the msd and preselection cuts
         mask_msd = events.FatJet.msoftdrop > cuts["msd"]
         mask_good_jets = mask_presel & mask_msd
 
     return jets[mask_good_jets], mask_good_jets
 
 
-def btagging(Jet, btag, wp):
-    return Jet[Jet[btag["btagging_algorithm"]] > btag["btagging_WP"][wp]]
-
-
-def CvsLsorted(jets, ctag):
-    return jets[ak.argsort(jets[ctag["tagger"]], axis=1, ascending=False)]
-
-
-def get_dijet(jets):
-    
-    fields = {
-        "pt": 0.,
-        "eta": 0.,
-        "phi": 0.,
-        "mass": 0.,
-    }
-
-    jets = ak.pad_none(jets, 2)
-    njet = ak.num(jets[~ak.is_none(jets, axis=1)])
-    
-    dijet = jets[:, 0] + jets[:, 1]
-
-    for var in fields.keys():
-        fields[var] = ak.where(
-            (njet >= 2),
-            getattr(dijet, var),
-            fields[var]
-        )
-
-    fields["deltaR"] = ak.where( (njet >= 2), jets[:,0].delta_r(jets[:,1]), -1)
-    fields["deltaPhi"] = ak.where( (njet >= 2), abs(jets[:,0].delta_phi(jets[:,1])), -1)
-    fields["deltaEta"] = ak.where( (njet >= 2), abs(jets[:,0].eta - jets[:,1].eta), -1)
-    fields["j1Phi"] = ak.where( (njet >= 2), jets[:,0].phi, -1)
-    fields["j2Phi"] = ak.where( (njet >= 2), jets[:,1].phi, -1)
-    
-    
-    dijet = ak.zip(fields, with_name="PtEtaPhiMCandidate")
-
-    return dijet
+def btagging(Jet, btag):
+    return Jet[Jet[btag["btagging_algorithm"]] > btag["btagging_WP"]]
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/lib/leptons.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/leptons.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,91 +13,65 @@
     passes_eta = abs(leptons.eta) < cuts["eta"]
     passes_pt = leptons.pt > cuts["pt"]
 
     if lepton_flavour == "Electron":
         # Requirements on SuperCluster eta, isolation and id
         etaSC = abs(leptons.deltaEtaSC + leptons.eta)
         passes_SC = np.invert((etaSC >= 1.4442) & (etaSC <= 1.5660))
-        passes_iso = True
-        if "iso" in cuts.keys():
-            passes_iso = leptons.pfRelIso03_all < cuts["iso"]
+        passes_iso = leptons.pfRelIso03_all < cuts["iso"]
         passes_id = leptons[cuts['id']] == True
 
         good_leptons = passes_eta & passes_pt & passes_SC & passes_iso & passes_id
 
     elif lepton_flavour == "Muon":
         # Requirements on isolation and id
         passes_iso = leptons.pfRelIso04_all < cuts["iso"]
         passes_id = leptons[cuts['id']] == True
 
         good_leptons = passes_eta & passes_pt & passes_iso & passes_id
 
     return leptons[good_leptons]
 
-def soft_lepton_selection(events, lepton_flavour, params):
-
-    leptons = events[lepton_flavour]
-    cuts = params.object_preselection[lepton_flavour]
-    # Requirements on pT and eta
-    passes_eta = abs(leptons.eta) < cuts["eta"]
-    passes_pt = leptons.pt > cuts["pt"]
-
-    if lepton_flavour == "Electron":
-        # Requirements on SuperCluster eta, isolation and id
-        etaSC = abs(leptons.deltaEtaSC + leptons.eta)
-        passes_SC = np.invert((etaSC >= 1.4442) & (etaSC <= 1.5660))
-        passes_iso = True
-        if "iso" in cuts.keys():
-            passes_iso = leptons.pfRelIso03_all < cuts["iso"]
-        passes_id = leptons[cuts['id']] == True
-
-        good_leptons = passes_eta & passes_pt & passes_SC & passes_iso & passes_id
-
-    elif lepton_flavour == "Muon":
-        # Requirements on isolation and id
-        passes_iso = leptons.pfRelIso04_all > cuts["iso_soft"]
-        passes_dxy_check = (abs(leptons.dxy / leptons.dxyErr) > 1.0)
-        passes_id = leptons[cuts['id']] == True
-
-        good_leptons = passes_eta & passes_pt & passes_iso & passes_id & passes_dxy_check
-
-    return leptons[good_leptons]
-
 
 def get_dilepton(electrons, muons, transverse=False):
 
     fields = {
         "pt": 0.,
         "eta": 0.,
         "phi": 0.,
         "mass": 0.,
         "charge": 0.,
     }
-    
-    leptons = ak.pad_none(ak.with_name(ak.concatenate([ muons[:, 0:2], electrons[:, 0:2]], axis=1), "PtEtaPhiMCandidate"), 2)
-    nlep =  ak.num(leptons[~ak.is_none(leptons, axis=1)])
-    ll = leptons[:,0] + leptons[:,1]
+
+    electrons = ak.pad_none(electrons, 2)
+    muons = ak.pad_none(muons, 2)
+
+    nelectrons = ak.num(electrons[~ak.is_none(electrons, axis=1)])
+    nmuons = ak.num(muons[~ak.is_none(muons, axis=1)])
+
+    ee = electrons[:, 0] + electrons[:, 1]
+    mumu = muons[:, 0] + muons[:, 1]
+    emu = electrons[:, 0] + muons[:, 0]
 
     for var in fields.keys():
         fields[var] = ak.where(
-            (nlep == 2),
-            getattr(ll, var),
-            fields[var]
+            ((nelectrons + nmuons) == 2) & (nelectrons == 2),
+            getattr(ee, var),
+            fields[var],
+        )
+        fields[var] = ak.where(
+            ((nelectrons + nmuons) == 2) & (nmuons == 2),
+            getattr(mumu, var),
+            fields[var],
+        )
+        fields[var] = ak.where(
+            ((nelectrons + nmuons) == 2) & (nelectrons == 1) & (nmuons == 1),
+            getattr(emu, var),
+            fields[var],
         )
-        
-    fields["deltaR"] = ak.where(
-        (nlep == 2), leptons[:,0].delta_r(leptons[:,1]), -1)
-    fields["deltaPhi"] = ak.where(
-        (nlep == 2), abs(leptons[:,0].delta_phi(leptons[:,1])), -1)
-    fields["deltaEta"] = ak.where(
-        (nlep == 2), abs(leptons[:,0].eta - leptons[:,1].eta), -1)
-    fields["l1phi"] = ak.where(
-        (nlep == 2), leptons[:,0].phi, -1)
-    fields["l2phi"] = ak.where(
-        (nlep == 2), leptons[:,1].phi, -1)
 
     if transverse:
         fields["eta"] = ak.zeros_like(fields["pt"])
     dileptons = ak.zip(fields, with_name="PtEtaPhiMCandidate")
 
     return dileptons
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/lib/parton_provenance.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/parton_provenance.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/lib/reconstruction.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/reconstruction.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/lib/scale_factors.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/scale_factors.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     if key in ['reco', 'id']:
         electron_correctionset = correctionlib.CorrectionSet.from_file(
             electronSF.JSONfiles[year]["file"]
         )
         map_name = electronSF.JSONfiles[year]["name"]
 
         if key == 'reco':
-            sfname = electronSF.JSONfiles[year]["reco"][pt_region]
+            sfname = electronSF["reco"][pt_region]
         elif key == 'id':
-            sfname = electronSF["id"][params.object_preselection["Electron"]["id"]]
+            sfname = electronSF["id"]
 
         # translate the `year` key into the corresponding key in the correction file provided by the EGM-POG
         year_pog = electronSF["era_mapping"][year]
 
         sf = electron_correctionset[map_name].evaluate(
             year_pog, "sf", sfname, eta.to_numpy(), pt.to_numpy()
         )
@@ -80,83 +80,87 @@
     This function computes the per-muon id or iso SF.
     '''
     muonSF = params["lepton_scale_factors"]["muon_sf"]
 
     muon_correctionset = correctionlib.CorrectionSet.from_file(
         muonSF.JSONfiles[year]['file']
     )
-    
     sfName = muonSF.sf_name[year][key]
-    
+
+    year_pog = muonSF.era_mapping[year]
     sf = muon_correctionset[sfName].evaluate(
-        np.abs(eta.to_numpy()), pt.to_numpy(), "nominal"
+        year_pog, np.abs(eta.to_numpy()), pt.to_numpy(), "sf"
     )
     sfup = muon_correctionset[sfName].evaluate(
-        np.abs(eta.to_numpy()), pt.to_numpy(), "systup"
+        year_pog, np.abs(eta.to_numpy()), pt.to_numpy(), "systup"
     )
     sfdown = muon_correctionset[sfName].evaluate(
-        np.abs(eta.to_numpy()), pt.to_numpy(), "systdown"
+        year_pog, np.abs(eta.to_numpy()), pt.to_numpy(), "systdown"
     )
-    
+
     # The unflattened arrays are returned in order to have one row per event.
     return (
         ak.unflatten(sf, counts),
         ak.unflatten(sfup, counts),
         ak.unflatten(sfdown, counts),
     )
 
 
 def sf_ele_reco(params, events, year):
     '''
     This function computes the per-electron reco SF and returns the corresponding per-event SF, obtained by multiplying the per-electron SF in each event.
     Additionally, also the up and down variations of the SF are returned.
-    Electrons are split into two categories based on a pt cut depending on the Run preiod, so that the proper SF is applied.
+    Electrons are split into two categories based on a pt cut at 20 GeV, so that the proper SF is applied.
     '''
+
     ele_pt = events.ElectronGood.pt
     ele_eta = events.ElectronGood.etaSC
 
-    pt_ranges = []
-    if year in ['2016_PreVFP', '2016_PostVFP','2017','2018']:
-        pt_ranges += [("pt_lt_20", (ele_pt < 20)), 
-                      ("pt_gt_20", (ele_pt >= 20))]
-    elif year in ["2022_preEE", "2022_postEE"]:
-        pt_ranges += [("pt_lt_20", (ele_pt < 20)), 
-                      ("pt_gt_20_lt_75", (ele_pt >= 20) & (ele_pt <75)), 
-                      ("pt_gt_75", (ele_pt >= 75))]
-    else:
-        raise Exception("For chosen year "+year+" sf_ele_reco are not implemented yet")
-    
-    sf_reco, sfup_reco, sfdown_reco = [], [], []
-
-    for pt_range_key, pt_range in pt_ranges:
-        ele_pt_inPtRange = ak.flatten(ele_pt[pt_range])
-        ele_eta_inPtRange = ak.flatten(ele_eta[pt_range])
-        ele_counts_inPtRange = ak.num(ele_pt[pt_range])
-
-        sf_reco_inPtRange, sfup_reco_inPtRange, sfdown_reco_inPtRange = get_ele_sf(
-            params,
-            year,
-            ele_pt_inPtRange,
-            ele_eta_inPtRange,
-            ele_counts_inPtRange,
-            'reco',
-            pt_range_key,
-        )
-        sf_reco.append(sf_reco_inPtRange)
-        sfup_reco.append(sfup_reco_inPtRange)
-        sfdown_reco.append(sfdown_reco_inPtRange)
+    Above20 = ele_pt >= 20
+    Below20 = ele_pt < 20
+
+    # Since `correctionlib` does not support jagged arrays as an input, the pt and eta arrays are flattened.
+    ele_pt_Above20, ele_counts_Above20 = ak.flatten(ele_pt[Above20]), ak.num(
+        ele_pt[Above20]
+    )
+    ele_eta_Above20 = ak.flatten(ele_eta[Above20])
+
+    ele_pt_Below20, ele_counts_Below20 = ak.flatten(ele_pt[Below20]), ak.num(
+        ele_pt[Below20]
+    )
+    ele_eta_Below20 = ak.flatten(ele_eta[Below20])
 
+    sf_reco_Above20, sfup_reco_Above20, sfdown_reco_Above20 = get_ele_sf(
+        params,
+        year,
+        ele_pt_Above20,
+        ele_eta_Above20,
+        ele_counts_Above20,
+        'reco',
+        'pt_gt_20',
+    )
+    sf_reco_Below20, sfup_reco_Below20, sfdown_reco_Below20 = get_ele_sf(
+        params,
+        year,
+        ele_pt_Below20,
+        ele_eta_Below20,
+        ele_counts_Below20,
+        'reco',
+        'pt_lt_20',
+    )
+
+    # The SF arrays corresponding to the electrons with pt above and below 20 GeV are concatenated and multiplied along the electron axis in order to obtain a per-event scale factor.
     sf_reco = ak.prod(
-        ak.concatenate(sf_reco, axis=1), axis=1
+        ak.concatenate((sf_reco_Above20, sf_reco_Below20), axis=1), axis=1
     )
     sfup_reco = ak.prod(
-        ak.concatenate(sfup_reco, axis=1), axis=1
+        ak.concatenate((sfup_reco_Above20, sfup_reco_Below20), axis=1), axis=1
     )
     sfdown_reco = ak.prod(
-        ak.concatenate(sfdown_reco, axis=1), axis=1
+        ak.concatenate((sfdown_reco_Above20, sfdown_reco_Below20), axis=1), axis=1
     )
 
     return sf_reco, sfup_reco, sfdown_reco
 
 
 def sf_ele_id(params, events, year):
     '''
@@ -330,84 +334,14 @@
         params.btagSF_calibration[year]["file"]
     )
     corr = cset[params.btagSF_calibration[year]["name"]]
     w = corr.evaluate(sample, year, ak.to_numpy(njets), ak.to_numpy(jetsHt))
     return w
 
 
-def sf_ctag(params, jets, year, njets, variations=["central"]):
-    '''
-    Shape correction scale factors (SF) for DepJet charm tagger, taken from:
-    https://cms-nanoaod-integration.web.cern.ch/commonJSONSFs/summaries/BTV_201X_UL_ctagging.html
-    SFs are obtained per jet, then multiplied to obtain an overall weight per event.
-    Note: this SF does not preserve the normalization of the MC samples!
-     One has to re-normalize the MC samples using the sf_ctag_calib() method.
-     The norm. calibration corrections are phase-space/analysis dependant.
-     Therefore one has to derive them for each analysis separately.
-    '''
-    # print("Doing sf_ctag", year)
-
-    ctagSF = params.jet_scale_factors.ctagSF[year]
-    ctagger = params.ctagging.working_point[year]["tagger"]
-    cset = correctionlib.CorrectionSet.from_file(ctagSF.SF_file)
-
-    #print(list(cset.keys()))
-    #print(list(cset.items()))
-
-    corr = cset[ctagSF.name]
-
-    #print(corr)
-
-    flav = ak.to_numpy(ak.flatten(jets.hadronFlavour))
-    CvL = ak.to_numpy(ak.flatten(jets.btagDeepCvL))
-    CvB = ak.to_numpy(ak.flatten(jets.btagDeepCvB))
-
-    central_SF_byjet = corr.evaluate("central", flav, CvL, CvB)
-
-    #print(central_SF_byjet)
-    #print("Unflatt=", ak.unflatten(central_SF_byjet, njets))
-    #print("Prod:", ak.prod(ak.unflatten(central_SF_byjet, njets), axis=1))
-
-    output = {}
-    for variation in variations:
-        if variation == "central":
-            output[variation] = [ak.prod(ak.unflatten(central_SF_byjet, njets), axis=1)]
-        else:
-            # Nominal sf==1
-            nominal = np.ones(ak.num(njets, axis=0))
-            # Systematic variations
-            up_variation_SF_byjet = corr.evaluate(f"up_{variation}", flav, CvL, CvB)
-            down_variation_SF_byjet = corr.evaluate(f"down_{variation}", flav, CvL, CvB)
-
-            output[variation] = [
-                nominal,
-                ak.prod(ak.unflatten(up_variation_SF_byjet,njets), axis=1),
-                ak.prod(ak.unflatten(down_variation_SF_byjet,njets), axis=1)
-            ]
-
-    return output
-
-
-def sf_ctag_calib(params, dataset, year, njets, jetsHt):
-    '''
-    These are correctiosn to normalization of every dataset after application of the ctag_sf shape correction.
-    It was computed in V+2J selection by comparing the inclusive shape with and without ctagSF in 2D:
-    in nJets-JetsHT bins. Each sample/year has a different correction stored in the correctionlib format.
-    Note: the correction  file in parameters/ctagSF_calibrationSF.json is uesd by default here,
-    which was  derived for V+2J phase space. It may not be suitable for other analyses.
-    '''
-    ctagSF = params.jet_scale_factors.ctagSF[year]
-    cset = correctionlib.CorrectionSet.from_file(ctagSF.Calib_file)
-
-    corr = cset["ctagSF_norm_correction"]
-    w = corr.evaluate(dataset, ak.to_numpy(njets), ak.to_numpy(jetsHt))
-
-    return w
-
-
 def sf_jet_puId(params, jets, year, njets):
     # The SF is applied only on jets passing the preselection (JetGood), pt < maxpt, and matched to a GenJet.
     # In other words the SF is not applied on jets not passing the Jet Pu ID SF.
     # We DON'T assume that the function is applied on JetGood, so we REAPPLY jetPUID selections to be sure.
     # We apply also the pt limit.
     jet_puId_cfg = params.object_preselection["Jet"]["puId"]
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/lib/triggers.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/triggers.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,13 +51,12 @@
                     & ((events.TrigObj.filterBits & 1024) == 1024),
                     axis=1,
                 )
                 > 0
             )
             trigger_mask = trigger_mask | (events.HLT[trigger] & flag)
         else:
-            if trigger in events.HLT.fields:
-                trigger_mask = trigger_mask | events.HLT[trigger.lstrip("HLT_")]
+            trigger_mask = trigger_mask | events.HLT[trigger.lstrip("HLT_")]
 
     if invert:
         trigger_mask = ~trigger_mask
     return trigger_mask
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/lib/weights_manager.py` & `pocket_coffea-1.0rc3/pocket_coffea/lib/weights_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from dataclasses import dataclass
 import inspect
 import awkward as ak
-import numpy as np
 from collections.abc import Callable
 from collections import defaultdict
 
 from coffea.analysis_tools import Weights
 
 # Scale factors functions
 from .scale_factors import (
     sf_ele_reco,
     sf_ele_id,
     sf_ele_trigger,
     sf_mu,
     sf_btag,
     sf_btag_calib,
-    sf_ctag,
-    sf_ctag_calib,
     sf_jet_puId,
     sf_L1prefiring,
     sf_pileup_reweight,
 )
 
 
 @dataclass
@@ -80,28 +77,25 @@
     def available_weights(cls):
         '''
         Predefine weights for CMS Run2 UL analysis.
         '''
         return set(
             [
                 'genWeight',
-                'signOf_genWeight',
                 'lumi',
                 'XS',
                 'pileup',
                 'sf_ele_reco',
                 'sf_ele_id',
                 'sf_ele_trigger',
                 'sf_mu_id',
                 'sf_mu_iso',
                 'sf_mu_trigger',
                 'sf_btag',
                 'sf_btag_calib',
-                'sf_ctag',
-                'sf_ctag_calib',
                 'sf_jet_puId',
                 'sf_L1prefiring',
             ]
         )
 
     @classmethod
     def available_variations(cls):
@@ -116,15 +110,14 @@
             "sf_ele_trigger",
             "sf_mu_id",
             "sf_mu_iso",
             "sf_mu_trigger",
             "sf_jet_puId",
             "sf_L1prefiring",
             "sf_btag",
-            "sf_ctag"
         ]
         return set(out)
 
     def __init__(
         self,
         params,
         weightsConf,
@@ -132,15 +125,14 @@
         events,
         shape_variation,
         metadata,
         storeIndividual=False,
     ):
         self.params = params
         self._sample = metadata["sample"]
-        self._dataset = metadata["dataset"]
         self._year = metadata["year"]
         self._xsec = metadata["xsec"]
         self._shape_variation = shape_variation
         self.weightsConf = weightsConf
         self.storeIndividual = storeIndividual
         self.size = size
         # looping on the weights configuration to create the
@@ -226,16 +218,14 @@
                  ("name", nominal, up, down)]
 
         Each variation is then added to the Weights object by the caller
         in the constructor.
         '''
         if weight_name == "genWeight":
             return [('genWeight', events.genWeight)]
-        if weight_name == "signOf_genWeight":
-            return [('signOf_genWeight', np.sign(events.genWeight))]
         elif weight_name == 'lumi':
             return [
                 (
                     'lumi',
                     ak.full_like(
                         events.genWeight, self.params.lumi.picobarns[self._year]["tot"]
                     ),
@@ -291,14 +281,15 @@
             # return the nominal and everything
             return [
                 (f"sf_ele_trigger_{var}", *weights)
                 for var, weights in triggersf.items()
             ]
 
         elif weight_name == 'sf_btag':
+
             # Get all the nominal and variation SF
             if shape_variation == "nominal":
                 btag_vars = self.params.systematic_variations.weight_variations.sf_btag[
                     self._year
                 ]
                 btagsf = sf_btag(
                     self.params,
@@ -323,15 +314,15 @@
                     events.JetGood,
                     self._year,
                     njets=events.nJetGood,
                     variations=[shape_variation],
                 )
 
             else:
-                # Only the nominal if there is a shape variation (?)
+                # Only the nominal if there is a shape variation
                 btagsf = sf_btag(
                     self.params,
                     events.JetGood,
                     self._year,
                     njets=events.nJetGood,
                     variations=["central"],
                 )
@@ -347,61 +338,14 @@
                     "sf_btag_calib",
                     sf_btag_calib(
                         self.params, self._sample, self._year, events.nJetGood, jetsHt
                     ),
                 )
             ]
 
-        elif weight_name == 'sf_ctag':
-            #print("Doing ctag SFs", shape_variation)
-
-            if shape_variation == "nominal":
-                ctag_vars = self.params.systematic_variations.weight_variations.sf_ctag[
-                    self._year
-                ]
-                ctagsf = sf_ctag(
-                    self.params,
-                    events.JetGood,
-                    self._year,
-                    njets=events.nJetGood,
-                    variations=["central"] + ctag_vars,
-                )
-
-                for var in ctag_vars:
-                    #print("ctag_var", var)
-                    #print(ctagsf[var])
-                    # Rescale the up and down variation by the central one to
-                    # avoid double counting of the central SF when adding the weights
-                    # as separate entries in the Weights object.
-                    ctagsf[var][1] = ctagsf[var][1] / ctagsf["central"][0]
-                    ctagsf[var][2] = ctagsf[var][2] / ctagsf["central"][0]
-
-            else:
-                ctagsf = sf_ctag(
-                    self.params,
-                    events.JetGood,
-                    self._year,
-                    njets=events.nJetGood,
-                    variations=["central"],
-                )
-
-            return [(f"sf_ctag_{var}", *weights) for var, weights in ctagsf.items()]
-
-        elif weight_name == 'sf_ctag_calib':
-            jetsHt = ak.sum(abs(events.JetGood.pt), axis=1)
-            return [
-                (
-                    "sf_ctag_calib",
-                    sf_ctag_calib(
-                        self.params, self._dataset, self._year, events.nJetGood, jetsHt
-                    ),
-                )
-            ]
-
-
         elif weight_name == 'sf_jet_puId':
             return [
                 (
                     'sf_jet_puId',
                     *sf_jet_puId(
                         self.params,
                         events.JetGood,
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibrationSF_2017UL.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibrationSF_2017UL.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibrationSF_2018UL.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibrationSF_2018UL.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears_v2.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears_v2.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears_v3_btagSF-12-09-2022.json` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/btag_SF_calibration/btagSF_calibration_allyears_v3_btagSF-12-09-2022.json`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/dask_env.py` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/dask_env.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/datacert/Cert_271036-284044_13TeV_Legacy2016_Collisions16_JSON.txt` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/datacert/Cert_271036-284044_13TeV_Legacy2016_Collisions16_JSON.txt`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/datacert/Cert_294927-306462_13TeV_UL2017_Collisions17_GoldenJSON.txt` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/datacert/Cert_294927-306462_13TeV_UL2017_Collisions17_GoldenJSON.txt`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/datacert/Cert_314472-325175_13TeV_Legacy2018_Collisions18_JSON.txt` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/datacert/Cert_314472-325175_13TeV_Legacy2018_Collisions18_JSON.txt`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/defaults.py` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/defaults.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,18 +59,14 @@
         btagging,
         lepton_scale_factors,
         syst_variations,
         plotting_style
     )
     return all
 
-def get_default_run_options():
-    basedir = os.path.dirname(__file__)
-    run_options = OmegaConf.load(os.path.join(basedir, "executor_options_defaults.yaml"))
-    return run_options
 
 def get_defaults_and_compose(*files: List[str]):
     default_params = get_default_parameters()
     return merge_parameters_from_files(default_params, files)
 
 
 def merge_parameters(main_config: OmegaConf, *configs: List[OmegaConf], update=True):
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/histograms.py` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/histograms.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import math
 
 default_axis_settings = {
     'muon_pt': {
         "field": "pt",
         "bins": 50,
         "start": 0,
-        'stop': 150,
-        "lim": (0, 150),
+        'stop': 500,
+        "lim": (0, 500),
         'label': "$p_{T}^{\mu}$ [GeV]",
     },
     'muon_eta': {
         "field": "eta",
         "bins": 50,
         "start": -2.5,
         'stop': 2.5,
@@ -84,18 +84,18 @@
         "start": -math.pi,
         'stop': math.pi,
         "lim": (-math.pi, math.pi),
         'label': "$\phi_{e}$",
     },
     'lepton_pt': {
         "field": "pt",
-        "bins": 60,
+        "bins": 50,
         "start": 0,
-        'stop': 300,
-        "lim": (0, 300),
+        'stop': 500,
+        "lim": (0, 500),
         'label': "$p_{T}^{\ell}$ [GeV]",
     },
     'lepton_eta': {
         "field": "eta",
         "bins": 50,
         "start": -2.5,
         'stop': 2.5,
@@ -116,18 +116,18 @@
         "start": -16,
         'stop': 16,
         "lim": (-16, 16),
         'label': "Lepton pdgId",
     },
     'jet_pt': {
         "field": "pt",
-        "bins": 50,
+        "bins": 100,
         "start": 0,
-        'stop': 300,
-        "lim": (0, 300),
+        'stop': 1000,
+        "lim": (0, 500),
         'label': "$p_{T}^{j}$ [GeV]",
     },
     'jet_eta': {
         "field": "eta",
         "bins": 50,
         "start": -2.5,
         'stop': 2.5,
@@ -146,30 +146,14 @@
         "field": "btagDeepFlavB",
         "bins": 50,
         "start": 0.0,
         'stop': 1.0,
         "lim": (0, 1),
         'label': "AK4 DeepJet b-tag score",
     },
-    'jet_btagDeepFlavCvL': {
-        "field": "btagDeepFlavCvL",
-        "bins": 50,
-        "start": 0.0,
-        'stop': 1.0,
-        "lim": (0, 1),
-        'label': "AK4 DeepJet CvsL score",
-    },
-    'jet_btagDeepFlavCvB': {
-        "field": "btagDeepFlavCvB",
-        "bins": 50,
-        "start": 0.0,
-        'stop': 1.0,
-        "lim": (0, 1),
-        'label': "AK4 DeepJet CvsB score",
-    },
     'fatjet_pt': {
         "field": "pt",
         "bins": 100,
         "start": 0,
         'stop': 1000,
         "lim": (0, 1000),
         'label': r"FatJet $p_{T}$ [GeV]",
@@ -429,21 +413,22 @@
         'stop': 1500,
         "lim": (0, 500),
         'label': "$m_{\ell\ell}$ [GeV]",
     },
 }
 
 collection_fields = {
-    'jet': ["eta", "pt", "phi", "btagDeepFlavB", "btagDeepFlavCvL", "btagDeepFlavCvB"],
+    'jet': ["eta", "pt", "phi", "btagDeepFlavB"],
     'fatjet': [
         "eta",
         "pt",
         "phi",
         "mass",
         "msoftdrop",
+        "tau21",
         "btagDDBvLV2",
         "btagDDCvLV2",
         "btagDDCvBV2",
         # "particleNetMD_Xbb", "particleNetMD_Xcc",
         "particleNetMD_Xbb_QCD",
         "particleNetMD_Xcc_QCD",
         "deepTagMD_ZHbbvsQCD",
@@ -463,108 +448,96 @@
         "sumcorrmass",
         "logsumcorrmass",
     ]
     #'sv': ["summass", "logsummass", "projmass", "logprojmass", "sv1mass", "logsv1mass", "sumcorrmass", "logsumcorrmass"]
 }
 
 
-def _get_default_hist(name, type, coll, pos=None, fields=None, axis_settings=None, **kwargs):
-    '''Factory function to create a dictionary of HistConf objects for a given collection.
-    name: name of the histogram
-    type: type of the collection (e.g. jet, fatjet, parton, electron, muon, lepton, met, sv)
-    coll: name of the collection in the coffea processor (e.g. JetGood, ElectronGood, MuonGood, MET))
-    pos: position of the object in the collection (e.g. 0, 1, 2, 3, ...)
-    fields: list of fields to plot (e.g. eta, pt, phi, ...)
-    axis_settings: dictionary of settings for the axis of the histogram, to be used to overwrite the default axis settings
-    kwargs: additional arguments to be passed to the HistConf object (e.g. `only_variations`, `exclude_samples`, `only_samples`, `exclude_categories`, `only_categories`)'''
+def _get_default_hist(name, type, coll, pos=None, fields=None, **kwargs):
     out = {}
     for field in collection_fields[type]:
         if fields == None or field in fields:
             hist_name = f"{name}_{field}"
             setting = deepcopy(default_axis_settings[f"{type}_{field}"])
-            if axis_settings != None and f"{type}_{field}" in axis_settings:
-                setting.update(axis_settings[f"{type}_{field}"])
             setting["coll"] = coll
             # If the position argument is given the histogram is
             # created for the specific position
             if pos != None:
                 setting["pos"] = pos
                 # Avoid 0-indexing for the name of the histogram
                 hist_name += f"_{pos+1}"
-                setting["label"] = setting["label"] + " for Obj. #%i"%(pos+1)
-                
+
             out[hist_name] = HistConf(
                 axes=[
                     Axis(**setting),
                 ],
-                **kwargs
+                **kwargs,
             )
     return out
 
 
-def jet_hists(coll="JetGood", pos=None, fields=None, name=None, axis_settings=None, **kwargs):
+def jet_hists(coll="JetGood", pos=None, fields=None, name=None):
     if name == None:
         name = coll
-    return _get_default_hist(name, "jet", coll, pos, fields, axis_settings, **kwargs)
+    return _get_default_hist(name, "jet", coll, pos, fields)
 
 
-def fatjet_hists(coll="FatJetGood", pos=None, fields=None, name=None, axis_settings=None, **kwargs):
+def fatjet_hists(coll="FatJetGood", pos=None, fields=None, name=None):
     if name == None:
         name = coll
-    return _get_default_hist(name, "fatjet", coll, pos, fields, axis_settings, **kwargs)
+    return _get_default_hist(name, "fatjet", coll, pos, fields)
 
 
-def parton_hists(coll="PartonMatched", pos=None, fields=None, name=None, axis_settings=None, **kwargs):
+def parton_hists(coll="PartonMatched", pos=None, fields=None, name=None):
     if name == None:
         name = coll
-    return _get_default_hist(name, "parton", coll, pos, fields, axis_settings, **kwargs)
+    return _get_default_hist(name, "parton", coll, pos, fields)
 
 
-def ele_hists(coll="ElectronGood", pos=None, fields=None, name=None, axis_settings=None, **kwargs):
+def ele_hists(coll="ElectronGood", pos=None, fields=None, name=None, **kwargs):
     if name == None:
         name = coll
-    return _get_default_hist(name, "electron", coll, pos, fields, axis_settings, **kwargs)
+    return _get_default_hist(name, "electron", coll, pos, fields, **kwargs)
 
 
-def muon_hists(coll="MuonGood", pos=None, fields=None, name=None, axis_settings=None, **kwargs):
+def muon_hists(coll="MuonGood", pos=None, fields=None, name=None, **kwargs):
     if name == None:
         name = coll
-    return _get_default_hist(name, "muon", coll, pos, fields, axis_settings, **kwargs)
+    return _get_default_hist(name, "muon", coll, pos, fields, **kwargs)
 
 
-def lepton_hists(coll="LeptonGood", pos=None, fields=None, name=None, axis_settings=None, **kwargs):
+def lepton_hists(coll="LeptonGood", pos=None, fields=None, name=None):
     if name == None:
         name = coll
-    return _get_default_hist(name, "lepton", coll, pos, fields, axis_settings, **kwargs)
+    return _get_default_hist(name, "lepton", coll, pos, fields)
 
 
-def met_hists(coll="MET", pos=None, fields=None, name=None, axis_settings=None, **kwargs):
+def met_hists(coll="MET", pos=None, fields=None, name=None):
     if name == None:
         name = coll
-    return _get_default_hist(name, "met", coll, pos, fields, axis_settings, **kwargs)
+    return _get_default_hist(name, "met", coll, pos, fields)
 
 
-def sv_hists(coll="SV", pos=None, fields=None, name=None, axis_settings=None, **kwargs):
+def sv_hists(coll="SV", pos=None, fields=None, name=None):
     if name == None:
         name = coll
-    return _get_default_hist(name, "sv", coll, pos, fields, axis_settings, **kwargs)
+    return _get_default_hist(name, "sv", coll, pos, fields)
 
 
-def count_hist(coll, bins=10, start=0, stop=9, label=None, name=None, **kwargs):
+def count_hist(coll, bins=10, start=0, stop=9, label=None, name=None):
     if name == None:
         name = f"n{coll}"
     return {
         f"{name}": HistConf(
             axes=[
                 Axis(
                     coll="events",
                     field=f"n{coll}",
                     label=f"$N_{{{coll}}}$",
                     bins=bins,
                     start=start,
                     stop=stop,
                     lim=(start, stop),
                 )
-            ],
-            **kwargs
+            ]
         )
     }
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/RegroupedV2_Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Regrouped_Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Regrouped_Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Regrouped_Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Regrouped_Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Regrouped_Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Regrouped_Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Regrouped_Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Regrouped_Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1FastJet_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1RC_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1RC_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1RC_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L1RC_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK4PFPuppi.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK4PFPuppi.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK8PFPuppi.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK8PFPuppi.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_L2Relative_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK8PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_UncertaintySources_AK8PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK4PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK4PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK8PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK8PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK8PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16APV_V7_MC_Uncertainty_AK8PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1FastJet_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1RC_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1RC_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1RC_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L1RC_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK4PFPuppi.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK4PFPuppi.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK8PFPuppi.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK8PFPuppi.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_L2Relative_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK8PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_UncertaintySources_AK8PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK4PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK4PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK8PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK8PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK8PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL16_V7_MC_Uncertainty_AK8PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PF.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PF.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PF.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PF.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PF.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PF.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PF.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PF.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PF.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PF.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PF.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PF.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK4PF.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK4PF.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK8PF.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK8PF.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1FastJet_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK4PF.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK4PF.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK8PF.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK8PF.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L1RC_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PF.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PF.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PFPuppi.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PFPuppi.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PF.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PF.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PFPuppi.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PFPuppi.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_L2Relative_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PF.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PF.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PF.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PF.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_UncertaintySources_AK8PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PF.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PF.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PF.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PF.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL17_V5_MC_Uncertainty_AK8PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_EtaResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PhiResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_JRV2_MC_PtResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1FastJet_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1RC_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1RC_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1RC_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L1RC_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK4PFPuppi.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK4PFPuppi.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK4PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK4PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK8PFPuppi.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK8PFPuppi.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK8PFchs.jec.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_L2Relative_AK8PFchs.jec.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK4PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK8PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK8PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_UncertaintySources_AK8PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK4PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK4PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK4PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK4PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK8PFPuppi.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK8PFPuppi.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK8PFchs.junc.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer19UL18_V5_MC_Uncertainty_AK8PFchs.junc.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16APV_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_EtaResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PhiResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK4PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK4PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK8PFPuppi.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec/Summer20UL16_JRV3_MC_PtResolution_AK8PFchs.jr.txt.gz`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jec_config.py` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jec_config.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/jets_calibration.yaml` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jets_calibration.yaml`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/lumi.py` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/lumi.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 # Integrated luminosity [pb^-1] for each data-taking year
 
 """
 lumi = {
     "2016" : 36773.0,
     "2017" : 41529.0,
     "2018" : 58830.0,
-    "2022": xxx,
-    "2023": zzz,
 }
 """
 
 lumi = {
     "2016_PreVFP": {
         "B": 5829.427727,
         "C": 2601.678092,
@@ -46,31 +44,14 @@
     "2018": {
         "A": 14027.614284,
         "B": 7066.552169,
         "C": 6898.816878,
         "D": 31839.492009,
         "tot": 59832.47534,
     },
-    "2022": {
-        "C": 6300,
-        "D": 3300,
-        "tot": 9600,
-    },
-    "2022_postEE": {
-        "E": 6100,
-        "F": 18400,
-        "G": 3200,
-        "tot": 27700
-    },
-    "2023": {
-        "C": 17000,
-        "D": 9500,
-        "tot": 26500,
-    },
-
 }
 
 
 goldenJSON = {
     "2016_PreVFP": os.path.join(
         os.path.dirname(__file__),
         "datacert",
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/lumi.yaml` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/lumi.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -22,32 +22,13 @@
     '2018':
       A: 14027.614284
       B: 7066.552169
       C: 6898.816878
       D: 31839.492009
       tot: 59832.47534
 
-    "2022_preEE":
-      C: 5010.4
-      D: 2970.0
-      tot: 7980.4
-    "2022_postEE":
-      E: 5807.0 
-      F: 17781.9
-      G: 3082.8
-      tot: 26671.7
-    "2023_preBPix": 
-      C: 17650 
-      tot: 17650
-    "2023_postBPix":
-      D: 9451  
-      tot: 9451
-      
   goldenJSON:
-    '2016_PreVFP': "${default_params_dir:}/datacert/Cert_271036-284044_13TeV_Legacy2016_Collisions16_JSON.txt"
-    '2016_PostVFP': "${default_params_dir:}/datacert/Cert_271036-284044_13TeV_Legacy2016_Collisions16_JSON.txt"
+    2016_PreVFP: "${default_params_dir:}/datacert/Cert_271036-284044_13TeV_Legacy2016_Collisions16_JSON.txt"
+    2016_PostVFP: "${default_params_dir:}/datacert/Cert_271036-284044_13TeV_Legacy2016_Collisions16_JSON.txt"
     '2017': "${default_params_dir:}/datacert/Cert_294927-306462_13TeV_UL2017_Collisions17_GoldenJSON.txt"
     '2018': "${default_params_dir:}/datacert/Cert_314472-325175_13TeV_Legacy2018_Collisions18_JSON.txt"
-    '2022_preEE': "${default_params_dir:}/datacert/Cert_Collisions2022_355100_362760_Golden.json"
-    '2022_postEE': "${default_params_dir:}/datacert/Cert_Collisions2022_355100_362760_Golden.json"
-    '2023_preBPix': "${default_params_dir:}/datacert/Cert_Collisions2023_366442_370790_Golden.json"
-    '2023_postBPix': "${default_params_dir:}/datacert/Cert_Collisions2023_366442_370790_Golden.json"
+
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/pileup.yaml` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/jet_scale_factors.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,35 @@
-pileupJSONfiles:
-  2016_PreVFP: 
-    file: /cvmfs/cms.cern.ch/rsync/cms-nanoAOD/jsonpog-integration/POG/LUM/2016preVFP_UL/puWeights.json.gz
-    name: Collisions16_UltraLegacy_goldenJSON
-  2016_PostVFP: 
-    file: /cvmfs/cms.cern.ch/rsync/cms-nanoAOD/jsonpog-integration/POG/LUM/2016postVFP_UL/puWeights.json.gz
-    name: Collisions16_UltraLegacy_goldenJSON
-  '2017':
-    file: /cvmfs/cms.cern.ch/rsync/cms-nanoAOD/jsonpog-integration/POG/LUM/2017_UL/puWeights.json.gz
-    name: Collisions17_UltraLegacy_goldenJSON
-  '2018':
-    file: /cvmfs/cms.cern.ch/rsync/cms-nanoAOD/jsonpog-integration/POG/LUM/2018_UL/puWeights.json.gz
-    name: Collisions18_UltraLegacy_goldenJSON
-  2022_preEE: 
-    file: /cvmfs/cms.cern.ch/rsync/cms-nanoAOD/jsonpog-integration/POG/LUM/2022_Summer22/puWeights.json.gz
-    name: Collisions2022_355100_357900_eraBCD_GoldenJson
-  2022_postEE: 
-    file: /cvmfs/cms.cern.ch/rsync/cms-nanoAOD/jsonpog-integration/POG/LUM/2022_Summer22EE/puWeights.json.gz
-    name: Collisions2022_359022_362760_eraEFG_GoldenJson
-  2023_preBPix:
-    file: /cvmfs/cms.cern.ch/rsync/cms-nanoAOD/jsonpog-integration/POG/LUM/2023_Summer23/puWeights.json.gz
-    name: Collisions2023_366403_369802_eraBC_GoldenJson
-  2023_postBPix:
-    file: /cvmfs/cms.cern.ch/rsync/cms-nanoAOD/jsonpog-integration/POG/LUM/2023_Summer23BPix/puWeights.json.gz
-    name: Collisions2023_369803_370790_eraD_GoldenJson
+# Default jet scale factors.
+# - btagSF: taking from cvmfs
+# - jetPuID SF
+
+jet_scale_factors:
+  btagSF:
+    # DeepJet AK4 tagger shape SF
+    '2016_PreVFP':
+      file: /cvmfs/cms.cern.ch/rsync/cms-nanoAOD/jsonpog-integration/POG/BTV/2016preVFP_UL/btagging.json.gz
+      name: "deepJet_shape"
+    '2016_PostVFP':
+      file: /cvmfs/cms.cern.ch/rsync/cms-nanoAOD/jsonpog-integration/POG/BTV/2016postVFP_UL/btagging.json.gz
+      name: "deepJet_shape"
+    '2017':
+      file: /cvmfs/cms.cern.ch/rsync/cms-nanoAOD/jsonpog-integration/POG/BTV/2017_UL/btagging.json.gz
+      name: "deepJet_shape"
+    '2018':
+      file: /cvmfs/cms.cern.ch/rsync/cms-nanoAOD/jsonpog-integration/POG/BTV/2018_UL/btagging.json.gz
+      name: "deepJet_shape"
+
+  jet_puId:
+      # Jet PU ID SF to be applied only on selected jets (pt<50) that are matched to GenJets
+      '2016_PreVFP':
+        file: /cvmfs/cms.cern.ch/rsync/cms-nanoAOD/jsonpog-integration/POG/JME/2016preVFP_UL/jmar.json.gz
+        name: PUJetID_eff
+      '2016_PostVFP':
+        file: /cvmfs/cms.cern.ch/rsync/cms-nanoAOD/jsonpog-integration/POG/JME/2016postVFP_UL/jmar.json.gz
+        name: PUJetID_eff
+      '2017':
+        file: /cvmfs/cms.cern.ch/rsync/cms-nanoAOD/jsonpog-integration/POG/JME/2017_UL/jmar.json.gz
+        name: PUJetID_eff
+      '2018':
+        file: /cvmfs/cms.cern.ch/rsync/cms-nanoAOD/jsonpog-integration/POG/JME/2018_UL/jmar.json.gz
+        name: PUJetID_eff
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/parameters/plotting_style.yaml` & `pocket_coffea-1.0rc3/pocket_coffea/parameters/plotting_style.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -77,12 +77,8 @@
         
     plot_upper_label:
       by_year:
         "2016_PreVFP": "${pico_to_femto:${lumi.picobarns.2016_PreVFP.tot}}"
         "2016_PostVFP": "${pico_to_femto:${lumi.picobarns.2016_PostVFP.tot}}"
         "2017": "${pico_to_femto:${lumi.picobarns.2017.tot}}"
         "2018": "${pico_to_femto:${lumi.picobarns.2018.tot}}"
-        "2022_preEE": "${pico_to_femto:${lumi.picobarns.2022_preEE.tot}}"
-        "2022_postEE": "${pico_to_femto:${lumi.picobarns.2022_postEE.tot}}"
-        "2023_preBPix": "${pico_to_femto:${lumi.picobarns.2023_preBPix.tot}}"
-        "2023_postBPix": "${pico_to_femto:${lumi.picobarns.2023_postBPix.tot}}"
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/scripts/build_jec.py` & `pocket_coffea-1.0rc3/scripts/build_jec.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/scripts/dataset/append_genweights.py` & `pocket_coffea-1.0rc3/scripts/dataset/append_genweights.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/scripts/dataset/append_parents.py` & `pocket_coffea-1.0rc3/scripts/dataset/append_parents.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/scripts/dataset/build_datasets.py` & `pocket_coffea-1.0rc3/scripts/dataset/build_datasets.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,80 @@
+#!/usr/bin/env python
+
+print(
+    """
+   ___       _ __   _____       __               __ 
+  / _ )__ __(_) /__/ / _ \___ _/ /____ ____ ___ / /_
+ / _  / // / / / _  / // / _ `/ __/ _ `(_-</ -_) __/
+/____/\_,_/_/_/\_,_/____/\_,_/\__/\_,_/___/\__/\__/ 
+                                                   
+"""
+)
+
 import os
 import sys
 import json
 import argparse
-import click
-from rich import print
 
-from pocket_coffea.utils import dataset
+from pocket_coffea.utils.dataset import build_datasets
 
-@click.command()
-@click.option(
+parser = argparse.ArgumentParser(description='Build dataset fileset in json format')
+parser.add_argument(
     '--cfg',
     default=os.getcwd() + "/datasets/datasets_definitions.json",
     help='Config file with parameters specific to the current run',
-    required=True,
+    required=False,
 )
-@click.option(
-    "-k", "--keys", 
-    type=str, 
-    multiple=True, 
-    help="Keys of the datasets to be created. If None, the keys are read from the datasets definition file."
+parser.add_argument(
+    "-k", "--keys", nargs="+", required=False, help="Keys of the datasets to be created. If None, the keys are read from the datasets definition file."
 )
-@click.option(
+parser.add_argument(
     '-d',
     '--download',
-    is_flag=True,
+    action='store_true',
     default=False,
     help='Download datasets from DAS',
+    required=False,
 )
-@click.option(
+parser.add_argument(
     '-o',
     '--overwrite',
-    is_flag=True,
+    action='store_true',
     help="Overwrite existing .json datasets",
+    default=False,
 )
-@click.option(
+parser.add_argument(
     '-c',
     '--check',
-    is_flag=True,
+    action='store_true',
     help="Check existence of the datasets",
+    default=False,
 )
-@click.option(
+parser.add_argument(
     '-s',
     '--split-by-year',
-    is_flag=True,
     help="Split datasets by year",
+    action="store_true",
+    default=False,
 )
-@click.option("-l", "--local-prefix", type=str, default=None)
-@click.option(
+parser.add_argument("-l", "--local-prefix", help="Prefix of the local path where the datasets are stored", type=str, default=None)
+parser.add_argument(
     "-ws",
-    "--allowlist-sites",
+    "--whitelist-sites",
+    help="List of sites to be whitelisted",
+    nargs="+",
     type=str,
-    multiple=True,
 )
-@click.option(
+parser.add_argument(
     "-bs",
-    "--blocklist-sites",
+    "--blacklist-sites",
+    help="List of sites to be blacklisted",
+    nargs="+",
     type=str,
-    multiple=True,
 )
-@click.option("-rs", "--regex-sites", type=str)
-@click.option("-p", "--parallelize", type=int, default=4)
-def build_datasets(cfg, keys, download, overwrite, check,
-         split_by_year, local_prefix, allowlist_sites, blocklist_sites, regex_sites, parallelize):
-    '''Build dataset fileset in json format'''
-    # Check for comma separated values
-    if len(allowlist_sites)>0 and "," in allowlist_sites[0]:
-        allowlist_sites = allowlist_sites[0].split(",")
-    if len(blocklist_sites)>0 and "," in blocklist_sites[0]:
-        blocklist_sites = blocklist_sites[0].split(",")
-
-    print("Building datasets...")
-    print("[green]Allowlist sites:[/]")
-    print(allowlist_sites)
-    print("[red]Blocklist sites:[/]")
-    print(blocklist_sites)
-        
-    dataset.build_datasets(cfg=cfg,
-                           keys=keys,
-                           download=download,
-                           overwrite=overwrite,
-                           check=check,
-                           split_by_year=split_by_year,
-                           local_prefix=local_prefix,
-                           allowlist_sites=allowlist_sites,
-                           blocklist_sites=blocklist_sites,
-                           regex_sites=regex_sites,
-                           parallelize=parallelize)
-
+parser.add_argument("-rs", "--regex-sites", help="Regex string to be used to filter the sites", type=str)
+parser.add_argument("-p", "--parallelize", help="Number of parallel processes to be used to fetch the datasets", type=int, default=4)
+args = parser.parse_args()
 
+print(vars(args))
 
-if __name__ == "__main__":
-    build_datasets()
+build_datasets(**vars(args))
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/scripts/dataset/download.py` & `pocket_coffea-1.0rc3/scripts/dataset/download.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/scripts/hadd_skimmed_files.py` & `pocket_coffea-1.0rc3/scripts/hadd_skimmed_files.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,115 +2,108 @@
 import os
 from multiprocessing import Pool
 import argparse
 from collections import defaultdict
 from coffea.util import load
 import subprocess
 import json
-import click
 
-@click.command()
-@click.option(
+parser = argparse.ArgumentParser(description='Hadd skimmed files')
+# Inputs
+parser.add_argument(
     '-fl',
     '--files-list',
     required=True,
     type=str,
     help='Parquet file containing the skimmed files metadata',
 )
-@click.option("-o", "--outputdir", type=str, help="Output folder")
-@click.option(
-    "--only-datasets", 
-    type=str, 
-    multiple=True, 
-    help="Restring list of datasets"
+parser.add_argument("-o", "--outputdir", required=False, type=str, help="Output folder")
+parser.add_argument(
+    "--only-datasets", nargs="+", type=str, help="Restring list of datasets"
 )
-@click.option("-f", "--files", type=int, help="Limit number of files")
-@click.option("-e", "--events", type=int, help="Limit number of files")
-@click.option(
+parser.add_argument("-f", "--files", type=int, help="Limit number of files")
+parser.add_argument("-e", "--events", type=int, help="Limit number of files")
+parser.add_argument(
     "-s",
     "--scaleout",
     type=int,
     help="Number of threads to process the hadd.",
     default=2,
 )
-@click.option("--overwrite", is_flag=True, help="Overwrite files")
-@click.option("--dry", is_flag=True, help="Do not execute hadd, save metadata")
-def hadd_skimmed_files(files_list, outputdir, only_datasets, files, events, scaleout, overwrite, dry):
-    '''
-    Regroup skimmed datasets by joining different files (like hadd for ROOT files) 
-    '''
-    df = load(files_list)
-    workload = []
-    groups_metadata = {}
-    
-    for dataset in df["skimmed_files"].keys():
-        if only_datasets and dataset not in only_datasets:
-            continue
-        groups_metadata[dataset] = defaultdict(dict)
-        nevents_tot = 0
-        nfiles = 0
-        group = []
-        ngroup = 1
-        for file, nevents in zip(
-            df["skimmed_files"][dataset], df["nskimmed_files"][dataset]
-        ):
-            if (files and (nfiles + 1) > files) or (
-                events and (nevents_tot + nevents) > events
-            ):
-                outfile = f"{outputdir}/{dataset}/{dataset}_{ngroup}.root"
-                workload.append((outfile, group[:]))
-                groups_metadata[dataset]["files"][outfile] = group[:]
-                group.clear()
-                ngroup += 1
-                nfiles = 0
-                nevents_tot = 0
-            else:
-                group.append(file)
-                nfiles += 1
-                nevents_tot += nevents
-
-        # add last group
-        if len(group):
-            outfile = f"{outputdir}/{dataset}/{dataset}_{ngroup}.root"
-            workload.append((outfile, group[:]))
-            groups_metadata[dataset]["files"][outfile] = group[:]
-
-    print(f"We will hadd {len(workload)} groups of files.")
-    print("Samples:", groups_metadata.keys())
-
-    def do_hadd(group):
-        try:
-            print("Running: ", group[0])
-            if overwrite:
-                subprocess.run(["hadd", "-f", group[0], *group[1]], check=True)
-            else:
-                subprocess.run(["hadd", group[0], *group[1]], check=True)
-            return group[0], 0
-        except subprocess.CalledProcessError as e:
-            print("Error producing group: ", group[0])
-            print(e.stderr)
-            return group[0], 1
-
-
-    if not dry:
-        p = Pool(scaleout)
-        results = p.map(do_hadd, workload)
-
-        print("\n\n\n")
-        for group, r in results:
-            if r != 0:
-                print("#### Failed hadd: ", group)
-
-    json.dump(groups_metadata, open("hadd.json", "w"), indent=2)
-
-    # Now saving the dataset definition file
-    dataset_definition = {
-        s: {"files": list(d['files'].keys())} for s, d in groups_metadata.items()
-    }
+parser.add_argument("--overwrite", action="store_true", help="Overwrite files")
+parser.add_argument(
+    "--dry", action="store_true", help="Do not execute hadd, save metadata"
+)
+args = parser.parse_args()
 
-    json.dump(dataset_definition, open("skimmed_dataset_definition.json", "w"), indent=2)
+df = load(args.files_list)
 
-    print("DONE!")
+workload = []
+groups_metadata = {}
 
+for dataset in df["skimmed_files"].keys():
+    if args.only_datasets and dataset not in args.only_datasets:
+        continue
+    groups_metadata[dataset] = defaultdict(dict)
+    nevents_tot = 0
+    nfiles = 0
+    group = []
+    ngroup = 1
+    for file, nevents in zip(
+        df["skimmed_files"][dataset], df["nskimmed_files"][dataset]
+    ):
+        if (args.files and (nfiles + 1) > args.files) or (
+            args.events and (nevents_tot + nevents) > args.events
+        ):
+            outfile = f"{args.outputdir}/{dataset}/{dataset}_{ngroup}.root"
+            workload.append((outfile, group[:]))
+            groups_metadata[dataset]["files"][outfile] = group[:]
+            group.clear()
+            ngroup += 1
+            nfiles = 0
+            nevents_tot = 0
+        else:
+            group.append(file)
+            nfiles += 1
+            nevents_tot += nevents
+
+    # add last group
+    if len(group):
+        outfile = f"{args.outputdir}/{dataset}/{dataset}_{ngroup}.root"
+        workload.append((outfile, group[:]))
+        groups_metadata[dataset]["files"][outfile] = group[:]
+
+print(f"We will hadd {len(workload)} groups of files.")
+print("Samples:", groups_metadata.keys())
+
+
+def do_hadd(group):
+    try:
+        print("Running: ", group[0])
+        if args.overwrite:
+            subprocess.run(["hadd", "-f", group[0], *group[1]], check=True)
+        else:
+            subprocess.run(["hadd", group[0], *group[1]], check=True)
+        return group[0], 0
+    except subprocess.CalledProcessError as e:
+        print("Error producing group: ", group[0])
+        print(e.stderr)
+        return group[0], 1
+
+
+if not args.dry:
+    p = Pool(args.scaleout)
+    results = p.map(do_hadd, workload)
+
+    print("\n\n\n")
+    for group, r in results:
+        if r != 0:
+            print("#### Failed hadd: ", group)
+
+json.dump(groups_metadata, open("./hadd.json", "w"), indent=2)
+
+# Now saving the dataset definition file
+dataset_definition = {
+    s: {"files": list(d['files'].keys())} for s, d in groups_metadata.items()
+}
 
-if __name__ == "__main__":
-    hadd_skimmed_files()
+json.dump(dataset_definition, open("./skimmed_dataset_definition.json", "w"), indent=2)
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/scripts/lumi/filter_lumi_json.py` & `pocket_coffea-1.0rc3/scripts/lumi/filter_lumi_json.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/scripts/lumi/run_brilcalc.py` & `pocket_coffea-1.0rc3/scripts/lumi/run_brilcalc.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/scripts/plot/trigger_efficiency.py` & `pocket_coffea-1.0rc3/scripts/plot/trigger_efficiency.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/scripts/plot/trigger_scalefactor.py` & `pocket_coffea-1.0rc3/scripts/plot/trigger_scalefactor.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/scripts/runner_old.py` & `pocket_coffea-1.0rc3/scripts/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python
 print("""
-    ____             __        __  ______      ________
+    ____             __        __  ______      ________          
    / __ \____  _____/ /_____  / /_/ ____/___  / __/ __/__  ____ _
   / /_/ / __ \/ ___/ //_/ _ \/ __/ /   / __ \/ /_/ /_/ _ \/ __ `/
- / ____/ /_/ / /__/ ,< /  __/ /_/ /___/ /_/ / __/ __/  __/ /_/ /
-/_/    \____/\___/_/|_|\___/\__/\____/\____/_/ /_/  \___/\__,_/
-
+ / ____/ /_/ / /__/ ,< /  __/ /_/ /___/ /_/ / __/ __/  __/ /_/ / 
+/_/    \____/\___/_/|_|\___/\__/\____/\____/_/ /_/  \___/\__,_/  
+                                                                 
 """)
-import os, getpass
+
+import os
 import sys
 import argparse
 import cloudpickle
 import socket
 import logging
 
 from coffea.util import save
@@ -23,63 +24,62 @@
 from pocket_coffea.utils.logging import setup_logging
 
 def load_run_options(cfg):
     config_module =  utils.path_import(cfg)
     try:
         config = config_module.cfg
         logging.info(config)
-        config.run_options = config_module.run_options
         config.save_config(args.outputdir)
 
     except AttributeError as e:
         print("Error: ", e)
         raise("The provided configuration module does not contain a `cfg` attribute of type Configurator. Please check your configuration!")
 
     if not isinstance(config, Configurator):
         raise("The configuration module attribute `cfg` is not of type Configurator. Please check yuor configuration!")
 
     #TODO improve the run options config
-    return config, config_module.run_options
+    return config_module.run_options
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Run analysis on NanoAOD files using PocketCoffea processors')
     # Inputs
     parser.add_argument('--cfg', default=os.getcwd() + "/config/test.py", required=True, type=str,
                         help='Config file with parameters specific to the current run')
     parser.add_argument("-o", "--outputdir", required=True, type=str, help="Output folder")
     parser.add_argument("-t", "--test", action="store_true", help="Run with limit 1 interactively")
     parser.add_argument("-lf","--limit-files", type=int, help="Limit number of files")
     parser.add_argument("-lc","--limit-chunks", type=int, help="Limit number of chunks", default=None)
     parser.add_argument("-e","--executor", type=str,
                         help="Overwrite executor from config (to be used only with the --test options)" )
     parser.add_argument("-s","--scaleout", type=int, help="Overwrite scalout config" )
-    parser.add_argument("-ll","--loglevel", type=str, help="Console logging level", default="INFO" )
+    parser.add_argument("-ll","--loglevel", type=str, help="Logging level", default="INFO" )
     parser.add_argument("-f","--full", action="store_true", help="Process all datasets at the same time", default=False )
     args = parser.parse_args()
 
 
     # Setting up the output dir
     os.makedirs(args.outputdir, exist_ok=True)
     outfile = os.path.join(
         args.outputdir, "output_{}.coffea"
     )
-    logfile = os.path.join(args.outputdir, "logfile.log")
+    
     # Prepare logging
     if (not setup_logging(console_log_output="stdout", console_log_level=args.loglevel, console_log_color=True,
-                        logfile_file=logfile, logfile_log_level="info", logfile_log_color=False,
+                        logfile_file="last_run.log", logfile_log_level="info", logfile_log_color=False,
                         log_line_template="%(color_on)s[%(levelname)-8s] %(message)s%(color_off)s")):
         print("Failed to setup logging, aborting.")
         exit(1)
 
     print("Loading the configuration file...")
     if args.cfg[-3:] == ".py":
         # Load the script
-        config, run_options = load_run_options(args.cfg)
-
+        run_options = load_run_options(args.cfg)
+        
     elif args.cfg[-4:] == ".pkl":
         # WARNING: This has to be tested!!
         config = cloudpickle.load(open(args.cfg,"rb"))
         run_options = config.run_options
     else:
         raise sys.exit("Please provide a .py/.pkl configuration file")
 
@@ -106,61 +106,53 @@
     # dask/parsl needs to export x509 to read over xrootd
     if run_options.get('voms', None) is not None:
         _x509_path = run_options['voms']
     else:
         _x509_localpath = get_proxy_path()
         _x509_path = os.environ['HOME'] + f'/{_x509_localpath.split("/")[-1]}'
         os.system(f'cp {_x509_localpath} {_x509_path}')
-
+        
     if (run_env:=run_options.get("env", "singularity")) == "singularity":
         env_extra = [
             'export XRD_RUNFORKHANDLER=1',
             f'export X509_USER_PROXY={_x509_path}',
             # f'export X509_CERT_DIR={os.environ["X509_CERT_DIR"]}',
             f'source {sys.prefix}/bin/activate',
             'ulimit -u 32768',
             'export MALLOC_TRIM_THRESHOLD_=0'
         ]
     elif run_env == "conda":
         env_extra = [
             'export XRD_RUNFORKHANDLER=1',
             f'export X509_USER_PROXY={_x509_path}',
             # f'export X509_CERT_DIR={os.environ["X509_CERT_DIR"]}',
-            'source /etc/profile.d/conda.sh',  # This looks site-specific, may not work everywhere.
+            'source /etc/profile.d/conda.sh',
             f'export PATH={os.environ["CONDA_PREFIX"]}/bin:$PATH',
             f'conda activate {os.environ["CONDA_DEFAULT_ENV"]}',
             'ulimit -u 32768',
             'export MALLOC_TRIM_THRESHOLD_=0'
         ]
-        condor_extra = [
-            'echo \"Current date and time: `date`"',
-            'echo "Hostname=`hostname`"',
-            "export XRD_RUNFORKHANDLER=1",
-            f'export X509_USER_PROXY={_x509_path}',
-            f'export PYTHONPATH=$PYTHONPATH:{os.getcwd()}',
-            f'cd {os.getcwd()}',
-            f'source {os.environ["HOME"]}/.bashrc', # Conda should be setup by .bashrc for this to work
-            f'conda activate {os.environ["CONDA_PREFIX"]}',
-            'echo "Conda has been activated, hopefylly... We are ready to roll!"'
-        ]
-
+        
     env_extra.append(f'export PYTHONPATH={os.path.dirname(args.cfg)}:$PYTHONPATH')
-
+    # condor_extra = [
+    #     f"cd {os.getcwd()}",
+    #     f'source {os.environ["HOME"]}/.bashrc',
+    #     f"source {os.getcwd()}/CondaSetup.sh",
+    #     f'conda activate {os.environ["CONDA_PREFIX"]}',
+    # ]
     logging.debug(env_extra)
 
+
     #########
     # Executors
     if run_options['executor'] in ['futures', 'iterative']:
         # source the environment variables
         os.environ["XRD_RUNFORKHANDLER"] = "1"
         os.environ["X509_USER_PROXY"] = _x509_path
 
-        #for k in config.filesets.keys():
-        #    print(k, config.filesets[k]['files'])
-        
         if run_options['executor'] == 'iterative':
             _exec = processor.iterative_executor
         else:
             _exec = processor.futures_executor
         output = processor.run_uproot_job(config.filesets,
                                     treename='Events',
                                     processor_instance=config.processor_instance,
@@ -169,39 +161,36 @@
                                         'skipbadfiles':run_options.get('skipbadfiles'),
                                         'schema': processor.NanoAODSchema,
                                         'xrootdtimeout': run_options.get('xrootdtimeout', 600),
                                         'workers': run_options['scaleout']},
                                     chunksize=run_options['chunk'],
                                     maxchunks=run_options.get('max', None)
                                     )
-
+        
         save(output, outfile.format("all"))
         print(f"Saving output to {outfile.format('all')}")
 
 
     elif 'parsl' in run_options['executor']:
         import parsl
         from parsl.providers import LocalProvider, CondorProvider, SlurmProvider
         from parsl.channels import LocalChannel
         from parsl.config import Config
         from parsl.executors import HighThroughputExecutor
         from parsl.launchers import SrunLauncher, SingleNodeLauncher
         from parsl.addresses import address_by_hostname, address_by_query
 
-        # Setting Console loglevel to ERROR in order to avoid logs from Parsl
-        logging.getLogger().handlers[0].setLevel("ERROR")
-        
         if 'slurm' in run_options['executor']:
             slurm_htex = Config(
                 executors=[
                     HighThroughputExecutor(
                         label="coffea_parsl_slurm",
                         address=address_by_hostname(),
                         prefetch_capacity=0,
-                        mem_per_worker=run_options.get("mem_per_worker_parsl", 2),
+                        mem_per_worker=run_options['mem_per_worker'],
                         provider=SlurmProvider(
                             channel=LocalChannel(script_dir='logs_parsl'),
                             launcher=SrunLauncher(),
                             #launcher=SingleNodeLauncher(),
                             max_blocks=(run_options['scaleout'])+10,
                             init_blocks=run_options['scaleout'],
                             partition=run_options['queue'],
@@ -216,150 +205,114 @@
             dfk = parsl.load(slurm_htex)
 
             output = processor.run_uproot_job(config.filesets,
                                         treename='Events',
                                         processor_instance=config.processor_instance,
                                         executor=processor.parsl_executor,
                                         executor_args={
-                                            'skipbadfiles': run_options.get('skipbadfiles', False),
+                                            'skipbadfiles':True,
                                             'schema': processor.NanoAODSchema,
                                             'config': None,
                                         },
                                         chunksize=run_options['chunk'], maxchunks=run_options.get('max', None)
                                         )
 
             save(output, outfile.format("all") )
             print(f"Saving output to {outfile.format('all')}")
-
+    
         elif 'condor' in run_options['executor']:
             #xfer_files = [process_worker_pool, _x509_path]
             #print(xfer_files)
             condor_htex = Config(
                 executors=[
                     HighThroughputExecutor(
-                        label="coffea_parsl_condor",
-                        address=address_by_hostname(),
-                        max_workers=1,
-                        worker_debug=False,
-                        #worker_debug=True,
+                        label="coffea_parsl_slurm",
+                        #address=address_by_hostname(),
+                        worker_ports=(8786,8785),
                         prefetch_capacity=0,
                         provider=CondorProvider(
-                            nodes_per_block=1,
-                            cores_per_slot=run_options["workers"],
-                            #channel=LocalChannel(script_dir='logs_parsl'),
-                            mem_per_slot=run_options.get("mem_per_worker_parsl", 2),
-                            init_blocks=run_options["scaleout"],
-                            max_blocks=(run_options["scaleout"]) + 5,
-                            worker_init="\n".join(condor_extra),
-                            walltime=run_options["walltime"],
-                            requirements=run_options["requirements"],
+                            channel=LocalChannel(script_dir='logs_parsl'),
+                            launcher=SingleNodeLauncher(),
+                            max_blocks=(run_options['scaleout'])+10,
+                            init_blocks=run_options['scaleout'],
+                            worker_init="\n".join(env_extra),
                             #transfer_input_files=xfer_files,
-                            #scheduler_options=condor_cfg,
-
+                            scheduler_options=condor_cfg,
+                            walltime='00:30:00'
                         ),
                     )
                 ],
                 retries=run_options["retries"],
-	        run_dir="/tmp/"+getpass.getuser()+"/parsl_runinfo",
             )
             ## Site config for naf-desy
             if "naf-desy" in run_options['executor']:
                 condor_htex = Config(
                     executors=[
                         HighThroughputExecutor(
                             label="coffea_parsl_condor",
                             address=address_by_query(),
                             max_workers=1,
-                            worker_debug=False,
+                            worker_debug=True,
                             provider=CondorProvider(
                                 nodes_per_block=1,
                                 cores_per_slot=run_options["workers"],
                                 mem_per_slot=run_options["mem_per_worker"],
                                 init_blocks=run_options["scaleout"],
                                 max_blocks=(run_options["scaleout"]) + 10,
-                                worker_init="\n".join(condor_extra),
+                                worker_init="\n".join(env_extra + condor_extra),
                                 walltime=run_options["walltime"],
-                                requirements=run_options["requirements"],
                             ),
                         )
                     ],
                     retries=run_options["retries"],
-                    run_dir="/tmp/"+getpass.getuser()+"/parsl_runinfo",
                 )
-
-
-
             dfk = parsl.load(condor_htex)
-            print('Ready to run with parsl')
 
-            if args.full:
-                # Running on all datasets at once
-                fileset = config.filesets
-                logging.info(f"Working on samples: {list(fileset.keys())}")
-                output = processor.run_uproot_job(fileset,
-                                                  treename='Events',
-                                                  processor_instance=config.processor_instance,
-                                                  executor=processor.parsl_executor,
-                                                  executor_args={
-                                                      'skipbadfiles': run_options.get('skipbadfiles', False),
-                                                      'schema': processor.NanoAODSchema,
-                                                      'config': None,
-                                                  },
-                                                  chunksize=run_options['chunk'], maxchunks=run_options.get('max', None)
-                                                  )
-                print(f"Saving output to {outfile.format('all')}")
-                save(output, outfile.format("all"))
-            else:
-                # Running separately on each dataset
-                for sample, files in config.filesets.items():
-                    logging.info(f"Working on sample: {sample}")
-                    print(f"Working on sample: {sample}")
-                    fileset = {sample:files}
-                    output = processor.run_uproot_job(fileset,
-                                                      treename='Events',
-                                                      processor_instance=config.processor_instance,
-                                                      executor=processor.parsl_executor,
-                                                      executor_args={
-                                                          'skipbadfiles': run_options.get('skipbadfiles', False),
-                                                          'schema': processor.NanoAODSchema,
-                                                          'config': None,
-                                                      },
-                                                      chunksize=run_options['chunk'], maxchunks=run_options.get('max', None)
-                                                      )
-                    print(f"Saving output to {outfile.format(sample)}")
-                    save(output, outfile.format(sample))
+            output = processor.run_uproot_job(config.filesets,
+                                        treename='Events',
+                                        processor_instance=config.processor_instance,
+                                        executor=processor.parsl_executor,
+                                        executor_args={
+                                            'skipbadfiles':True,
+                                            'schema': processor.NanoAODSchema,
+                                            'config': None,
+                                        },
+                                        chunksize=run_options['chunk'], maxchunks=run_options.get('max', None)
+                                        )
+            save(output, outfile.format("all"))
+            print(f"Saving output to {outfile.format('all')}")
+
 
     # DASK runners
     elif 'dask' in run_options['executor']:
         import dask.config
         from pocket_coffea.parameters.dask_env import setup_dask
         from dask_jobqueue import SLURMCluster, HTCondorCluster
         from distributed import Client
         from dask.distributed import performance_report
         setup_dask(dask.config)
-
+        
         if 'slurm' in run_options['executor']:
             log_folder = "slurm_log"
             cluster = SLURMCluster(
                 queue=run_options['queue'],
                 cores=run_options['workers'],
                 processes=run_options['workers'],
                 memory=run_options['mem_per_worker'],
                 walltime=run_options["walltime"],
                 env_extra=env_extra,
                 local_directory=os.path.join(args.outputdir, log_folder),
             )
         elif 'condor' in run_options['executor']:
             log_folder = "condor_log"
             cluster = HTCondorCluster(
-                cores=run_options['workers'],
-                memory=run_options['mem_per_worker'],
-                disk=run_options.get('disk_per_worker', "2GB"),
-                job_script_prologue=condor_extra,
-                log_directory = f"{args.outputdir}/{log_folder}",
+                 cores=run_options['workers'],
+                 memory=run_options['mem_per_worker'],
+                 disk=run_options.get('disk_per_worker', "2GB"),
+                 job_script_prologue=env_extra,
             )
         elif 'lxplus' in run_options["executor"]:
             log_folder = "condor_log"
             from pocket_coffea.utils.network import check_port
 
             if "lxplus" not in socket.gethostname():
                 raise Exception("Trying to run with dask/lxplus not at CERN! Please try different runner options")
@@ -397,24 +350,24 @@
         cluster.adapt(minimum=1 if run_options.get("adapt", False)
                                 else run_options['scaleout'],
                       maximum=run_options['scaleout'])
         client = Client(cluster)
         logging.info(">> Waiting for the first job to start...")
         client.wait_for_workers(1)
         logging.info(">> You can connect to the Dask viewer at http://localhost:8787")
-
+        
         performance_report_path = os.path.join(args.outputdir, f"{log_folder}/dask-report.html")
         print(f"Saving performance report to {performance_report_path}")
         with performance_report(filename=performance_report_path):
 
             if args.full:
-                # Running on all datasets at once
+                # Running separately on each dataset
                 fileset = config.filesets
                 logging.info(f"Working on samples: {list(fileset.keys())}")
-
+                
                 output = processor.run_uproot_job(fileset,
                                         treename='Events',
                                         processor_instance=config.processor_instance,
                                         executor=processor.dask_executor,
                                         executor_args={
                                             'client': client,
                                             'skipbadfiles': run_options.get('skipbadfiles',False),
@@ -428,15 +381,15 @@
                 print(f"Saving output to {outfile.format('all')}")
                 save(output, outfile.format("all") )
             else:
                 # Running separately on each dataset
                 for sample, files in config.filesets.items():
                     logging.info(f"Working on sample: {sample}")
                     fileset = {sample:files}
-
+                    
                     output = processor.run_uproot_job(fileset,
                                             treename='Events',
                                             processor_instance=config.processor_instance,
                                             executor=processor.dask_executor,
                                             executor_args={
                                                 'client': client,
                                                 'skipbadfiles': run_options.get('skipbadfiles',False),
@@ -449,16 +402,7 @@
                                 )
                     print(f"Saving output to {outfile.format(sample)}")
                     save(output, outfile.format(sample))
 
     else:
         print(f"Executor {run_options['executor']} not defined!")
         exit(1)
-
-
-    #print("Logger handlers:", logging.getLogger().handlers )
-    log_file = logging.getLogger().handlers[1].baseFilename
-    #print("Logfile is saved at:", log_file)
-    # Copying logfile also to last_run.log
-    import shutil
-    shutil.copyfile(log_file, 'last_run.log')
-
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/utils/build_jets_calibrator.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/build_jets_calibrator.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/utils/configurator.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/configurator.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,14 @@
         # The following attributes are loaded by load_datasets
         self.filesets = {}
         self.datasets = []
         self.samples = []
 
         self.subsamples = {}
         self.subsamples_list = []  # List of subsamples (for internal checks)
-        self.subsamples_reversed_map = {}  # Map of subsample: sample
         self.total_samples_list = []  # List of subsamples and inclusive samples names
         self.has_subsamples = {}
 
         self.years = []
         self.eras = []
 
         self.load_datasets()
@@ -209,29 +208,26 @@
         # Complete list of samples and subsamples
         self.total_samples_list = list(set(self.samples + self.subsamples_list))
 
         # Now saving the subsamples definition cuts
         for sample in self.samples:
             if sample in subsamples_dict:
                 subscfg = subsamples_dict[sample]
-                self.subsamples_reversed_map.update({f"{sample}__{subsam}": sample for subsam in subscfg.keys()})
-                    
                 if isinstance(subscfg, dict):
                     # Convert it to StandardSelection
                     self.subsamples[sample] = StandardSelection(subscfg)
                 elif isinstance(subscfg, StandardSelection):
                     self.subsamples[sample] = subscfg
                 elif isinstance(subscfg, CartesianSelection):
                     self.subsamples[sample] = subscfg
             else:
                 # if there is no configured subsample, the full sample becomes its subsample
                 # this is useful in the processor to have always a subsample
                 # the name is == the name of the sample
                 self.subsamples[sample] = StandardSelection({sample: [passthrough]})
-                self.subsamples_reversed_map.update({sample: sample})
 
     def load_cuts_and_categories(self, skim: list, preselections: list, categories):
         '''This function loads the list of cuts and groups them in categories.
         Each cut is identified by a unique id (see Cut class definition)'''
         # If the skim, preselection and categories list are empty, append a `passthrough` Cut
 
         if len(skim) == 0:
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/utils/dataset.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,74 +8,54 @@
 import subprocess
 import requests
 import parsl
 from parsl import python_app
 from parsl.config import Config
 from parsl.executors.threads import ThreadPoolExecutor
 
-import urllib3
-urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-
 from .network import get_proxy_path
 from . import rucio
 
-def do_dataset(key, config, local_prefix, allowlist_sites, blocklist_sites, regex_sites, **kwargs):
+def do_dataset(key, config, local_prefix, whitelist_sites, blacklist_sites, regex_sites, **kwargs):
     print("*" * 40)
     print("> Working on dataset: ", key)
     if key not in config:
         print("Key: not found in the dataset configuration file")
         exit(1)
     dataset_cfg = config[key]
     if local_prefix:
         dataset_cfg["storage_prefix"] = local_prefix
 
     try:
         dataset = Dataset(
             name=key,
             cfg=dataset_cfg,
             sites_cfg={
-                "allowlist_sites": allowlist_sites,
-                "blocklist_sites": blocklist_sites,
+                "whitelist_sites": whitelist_sites,
+                "blacklist_sites": blacklist_sites,
                 "regex_sites": regex_sites,
             },
         )
     except:
         raise Exception(f"Error getting info about dataset: {key}")
 
     return dataset
 
-
-
 def build_datasets(cfg, keys=None, overwrite=False, download=False, check=False, split_by_year=False, local_prefix=None,
-                   allowlist_sites=None, blocklist_sites=None, regex_sites=None, parallelize=4):
+                   whitelist_sites=None, blacklist_sites=None, regex_sites=None, parallelize=4):
 
     config = json.load(open(cfg))
 
     if not keys:
         keys = config.keys()
+    args = {arg : value for arg, value in locals().items() if arg != "keys"}
 
-    args = {
-        "config": config,
-        "overwrite": overwrite,
-        "download": download,
-        "check": check,
-        "split_by_year": split_by_year,
-        "local_prefix": local_prefix,
-        "allowlist_sites": allowlist_sites,
-        "blocklist_sites": blocklist_sites,
-        "regex_sites": regex_sites,
-        "parallelize": parallelize
-    }
-    
-    if parallelize == 1:
-        datasets = [do_dataset(key, **args) for key in keys]
-    else:
-        with Pool(parallelize) as pool:
-            print("Dataset keys:", list(keys))
-            datasets = pool.map(partial(do_dataset, **args), keys)
+    with Pool(parallelize) as pool:
+        print(keys)
+        datasets = pool.map(partial(do_dataset, **args), keys)
 
     for dataset in datasets:
         dataset.save(overwrite=overwrite, split=split_by_year)
         if check:
             dataset.check_samples()
 
         if download:
@@ -88,15 +68,15 @@
         - The name is the unique key of the sample in the dataset file.
         - The DAS name is the unique identifier of the sample in CMS
         - The sample represent the type of events: DATA/Wjets/ttHbb/ttBB. It is used to group the same type of events
         - metadata contains various keys necessary for the analysis --> the dict passed around in the coffea processor
          -- year
          -- isMC: true/false
          -- era: A/B/C/D (only for data)
-        - sites_cfg is a dictionary contaning allowlist, blocklist and regex to filter the SITES
+        - sites_cfg is a dictionary contaning whitelist, blacklist and regex to filter the SITES
         '''
         self.name = name
         self.das_names = das_names
         self.metadata = {}
         self.metadata["das_names"] = das_names
         if "dbs_instance" in kwargs.keys():
             self.metadata["dbs_instance"] = kwargs["dbs_instance"]
@@ -122,50 +102,35 @@
         '''
         for das_name in self.das_names:
             proxy = get_proxy_path()
             if "dbs_instance" in self.metadata.keys():
                 link = f"https://cmsweb.cern.ch:8443/dbs/{self.metadata['dbs_instance']}/DBSReader/files?dataset={das_name}&detail=True"
             else:
                 link = f"https://cmsweb.cern.ch:8443/dbs/prod/global/DBSReader/files?dataset={das_name}&detail=True"
-
-            # print('\t Getting files for dataset: ', das_name)
             r = requests.get(
                 link,
                 cert=proxy,
                 verify=False,
             )
             filesjson = r.json()
             for fj in filesjson:
-                if 'is_file_valid' not in fj.keys():
-                    # print("fj=", fj)
-                    raise Exception(f"(probably) an Invalid dataset name provided for entry: {self}!")
+                if fj["is_file_valid"] == 0:
+                    print(f"ERROR: File not valid on DAS: {f['name']}")
                 else:
-                    if fj["is_file_valid"] == 0:
-                        #print(fj)
-                        print(f"\t WARNING: A file not valid on DAS: {fj['logical_file_name']}")
-                        print("\t We are skipping it")
-                        #raise Exception(f"Invalid files in sample {self}!")
-                        continue
-                    
                     self.fileslist_redirector.append(fj['logical_file_name'])
                     self.metadata["nevents"] += fj['event_count']
                     self.metadata["size"] += fj['file_size']
             if len(self.fileslist_redirector) == 0:
                 raise Exception(f"Found 0 files for sample {self}!")
 
-            if self.metadata.get("dbs_instance", "prod/global") == "prod/global":
-                # Now query rucio to get the concrete dataset passing the sites filtering options
-                files_replicas, sites, sites_counts = rucio.get_dataset_files_replicas(
-                    das_name, **self.sites_cfg, mode="first"
-                )
-            else:
-                # Use DBS to get the site
-                files_replicas, sites = rucio.get_dataset_files_from_dbs(das_name, self.metadata["dbs_instance"])
-                
-            self.fileslist_concrete += files_replicas
+            # Now query rucio to get the concrete dataset passing the sites filtering options
+            files_rucio, sites = rucio.get_dataset_files(
+                das_name, **self.sites_cfg, output="first"
+            )
+            self.fileslist_concrete += files_rucio
 
     # Function to build the sample dictionary
     def get_sample_dict(self, redirector=True, prefix="root://xrootd-cms.infn.it//"):
         if redirector:
             out = {
                 self.name: {
                     'metadata': {k: str(v) for k, v in self.metadata.items()},
@@ -224,16 +189,16 @@
         self.sample_dict_concrete = {}
         self.sample_dict_local = {}
         self.samples_obj = []
         self.sites_cfg = (
             sites_cfg
             if sites_cfg
             else {
-                "allowlist_sites": None,
-                "blocklist_sites": None,
+                "whitelist_sites": None,
+                "blacklist_sites": None,
                 "regex_sites": None,
             }
         )
         self.append_parents = append_parents
         self.get_samples(self.cfg["files"])
 
     # Function to build the dataset dictionary
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/utils/logging.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/utils/network.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/network.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/utils/plot_efficiency.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/plot_efficiency.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/utils/plot_sf.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/plot_sf.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/utils/plot_utils.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/plot_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 import numpy as np
 import awkward as ak
 import hist
 
 import matplotlib
 import matplotlib.pyplot as plt
 from matplotlib.pyplot import cm
+from matplotlib.ticker import MultipleLocator, AutoMinorLocator
 import mplhep as hep
 
 from omegaconf import OmegaConf
 from pocket_coffea.parameters.defaults import merge_parameters
 
-np.seterr(divide="ignore", invalid="ignore", over="ignore")
+
 class Style:
     '''This class manages all the style options for Data/MC plots.'''
 
     def __init__(self, style_cfg) -> None:
         self.style_cfg = style_cfg
         self._required_keys = ["opts_figure", "opts_mc", "opts_data", "opts_unc"]
         for key in self._required_keys:
@@ -33,23 +34,16 @@
         self.has_labels = False
         self.has_samples_groups = False
         self.has_lumi = False
         if "labels_mc" in style_cfg:
             self.has_labels = True
         if "samples_groups" in style_cfg:
             self.has_samples_groups = True
-        self.has_exclude_samples=False
-        if "exclude_samples" in style_cfg:
-            self.has_exclude_samples = True
-        self.has_rescale_samples=False
-        if "rescale_samples" in style_cfg:
-            self.has_rescale_samples = True
-        self.set_defaults()
 
-        #print("Style config:\n", style_cfg)
+        self.set_defaults()
 
     def set_defaults(self):
         if not "stack" in self.opts_mc:
             self.opts_mc["stack"] = True
         if not hasattr(self, "fontsize"):
             self.fontsize = 22
 
@@ -78,28 +72,26 @@
         plot_dir,
         style_cfg,
         toplabel=None,
         only_cat=None,
         workers=8,
         log=False,
         density=False,
-        verbose=1,
         save=True
     ) -> None:
 
         self.shape_objects = {}
         self.plot_dir = plot_dir
         self.only_cat = only_cat
         self.workers = workers
         self.log = log
         self.density = density
         self.save = save
         self.nhists = len(variables)
         self.toplabel = toplabel
-        self.verbose=verbose
 
         # Reading the datasets_metadata to
         # build the correct shapes for each datataking year
         # taking histo objects from hist_objs
         self.hists_to_plot = {}
         for variable in variables:
             vs = {}
@@ -108,64 +100,57 @@
                 for sample, datasets in samples.items():
                     hs[sample] = {}
                     for dataset in datasets:
                         try:
                             hs[sample][dataset] = hist_objs[variable][sample][dataset]
                         except:
                             print(f"Warning: missing dataset {dataset} for variable {variable}, year {year}")
-                    if len(hs[sample].keys()) == 0:
-                        del hs[sample]
                 vs[year] = hs
             self.hists_to_plot[variable] = vs
-
+        
         for variable, histoplot in self.hists_to_plot.items():
             for year, h_dict in histoplot.items():
                 name = '_'.join([variable, year])
                 # If toplabel is overwritten we use that, if not we take the lumi from the year
                 if self.toplabel:
                     toplabel_to_use = self.toplabel
                 else:
                     toplabel_to_use = f"$\mathcal{{L}}$ = {style_cfg.plot_upper_label.by_year[year]:.2f}/fb"
-
+                
                 self.shape_objects[name] = Shape(
                     h_dict,
                     datasets_metadata["by_dataset"],
                     name,
                     plot_dir,
                     style_cfg=style_cfg,
                     only_cat=self.only_cat,
                     log=self.log,
                     density=self.density,
-                    toplabel=toplabel_to_use,
-                    verbose=self.verbose
+                    toplabel=toplabel_to_use
                 )
         if self.save:
             self.make_dirs()
             matplotlib.use('agg')
 
     def make_dirs(self):
         '''Create directories recursively before saving plots with multiprocessing
         to avoid conflicts between different processes.'''
         for name, shape in self.shape_objects.items():
             for cat in shape.categories:
-                if self.only_cat and cat not in self.only_cat:
-                    continue
                 plot_dir = os.path.join(self.plot_dir, cat)
                 if not os.path.exists(plot_dir):
                     os.makedirs(plot_dir)
 
     def plot_datamc(self, name, syst=True, spliteras=False):
         '''Plots one histogram, for all years and categories.'''
-        if self.verbose>0:
-            print("Plotting: ", name)
+        print("Plotting: ", name)
         shape = self.shape_objects[name]
         if shape.dense_dim > 1:
-            if self.verbose>0:
-                print(f"WARNING: cannot plot data/MC for histogram {shape.name} with dimension {shape.dense_dim}.")
-                print("The method `plot_datamc` will be skipped.")
+            print(f"WARNING: cannot plot data/MC for histogram {shape.name} with dimension {shape.dense_dim}.")
+            print("The method `plot_datamc` will be skipped.")
             return
 
         if ((shape.is_mc_only) | (shape.is_data_only)):
             ratio = False
         else:
             ratio = True
         shape.plot_datamc_all(ratio, syst, spliteras=spliteras, save=self.save)
@@ -178,93 +163,71 @@
                 # Parallel calls of plot_datamc() on different shape objects
                 pool.map(partial(self.plot_datamc, syst=syst, spliteras=spliteras), shape_names)
                 pool.close()
         else:
             for shape in shape_names:
                 self.plot_datamc(shape, syst=syst, spliteras=spliteras)
 
+
 class Shape:
     '''This class handles the plotting of 1D data/MC histograms.
     The constructor requires as arguments:
     - h_dict: dictionary of histograms, with the following structure {}
     - name: name that identifies the Shape object.
     - style_cfg: dictionary with style and plotting options.
     '''
     def __init__(
         self,
         h_dict,
-        datasets_metadata,
+        datasets_metadata, 
         name,
         plot_dir,
         style_cfg,
         toplabel=None,
         only_cat=None,
         log=False,
         density=False,
-        verbose=1,
     ) -> None:
         self.h_dict = h_dict
         self.name = name
         self.plot_dir = plot_dir
         self.only_cat = only_cat if only_cat is not None else []
         self.style = Style(style_cfg)
         self.toplabel = toplabel if toplabel else ""
         if self.style.has_lumi:
             self.lumi_fraction = {year : l / lumi[year]['tot'] for year, l in self.style.lumi_processed.items()}
         self.log = log
         self.density = density
         self.datasets_metadata=datasets_metadata
         self.sample_is_MC = {}
-        self.verbose = verbose
         self._stacksCache = defaultdict(dict)
         assert (
             type(h_dict) in [dict, defaultdict]
         ), "The Shape object receives a dictionary of hist.Hist objects as argument."
         self.group_samples()
-        self.exclude_samples()
-        self.rescale_samples()
         self.load_attributes()
+        self.syst_manager = SystManager(self, self.style)
 
     def load_attributes(self):
         '''Loads the attributes from the dictionary of histograms.'''
-        if self.verbose>1:
-            print(self.h_dict)
-            print("samples:", self.samples_mc)
+        assert len(
+            set([self.h_dict[s].ndim for s in self.samples_mc])
+        ), f"{self.name}: Not all the MC histograms have the same dimension."
+        assert len(
+            set([self.h_dict[s].ndim for s in self.samples_data])
+        ), f"{self.name}: Not all the data histograms have the same dimension."
         
-        self.is_mc_only = True if len(self.samples_data) == 0 else False
-        self.is_data_only = True if len(self.samples_mc) == 0 else False
-
-        if not self.is_data_only:
-            assert len(
-                set([self.h_dict[s].ndim for s in self.samples_mc])
-            ), f"{self.name}: Not all the MC histograms have the same dimension."
-            # Load categorical axes for MC histograms
-            for ax in self.categorical_axes_mc:
-                setattr(
-                    self,
-                    {'year': 'years', 'cat': 'categories', 'variation': 'variations'}[
-                        ax.name
-                    ],
-                    self.get_axis_items(ax.name, is_mc=True),
-                )
-            self.syst_manager = SystManager(self, self.style)
-        if not self.is_mc_only:
-            assert len(
-                set([self.h_dict[s].ndim for s in self.samples_data])
-            ), f"{self.name}: Not all the data histograms have the same dimension."
-            # Load categorical axes for data histograms
-            for ax in self.categorical_axes_data:
-                setattr(
-                    self,
-                    {'year': 'years', 'cat': 'categories'}[
-                        ax.name
-                    ],
-                    self.get_axis_items(ax.name, is_mc=False),
-                )
-
+        for ax in self.categorical_axes_mc:
+            setattr(
+                self,
+                {'year': 'years', 'cat': 'categories', 'variation': 'variations'}[
+                    ax.name
+                ],
+                self.get_axis_items(ax.name),
+            )
         xaxis = self.dense_axes[0]
         self.style.update(
             {
             'opts_axes' : {
                 'xlabel' : xaxis.label,
                 'xcenters' : xaxis.centers.tolist(),
                 'xedges' : xaxis.edges.tolist(),
@@ -282,14 +245,18 @@
                         'ycenters' : yaxis.centers.tolist(),
                         'yedges' : yaxis.edges.tolist(),
                         'ybinwidth' : np.ediff1d(yaxis.edges).tolist()
                     }
                 }
             )
 
+        self.is_mc_only = True if len(self.samples_data) == 0 else False
+        self.is_data_only = True if len(self.samples_mc) == 0 else False
+
+        
     @property
     def dense_axes(self):
         '''Returns the list of dense axes of a histogram, defined as the axes that are not categorical axes.'''
         dense_axes_dict = {s: [] for s in self.h_dict.keys()}
 
         for s, h in self.h_dict.items():
             for ax in h.axes:
@@ -299,91 +266,84 @@
         assert all(
             v == dense_axes[0] for v in dense_axes
         ), "Not all the histograms in the dictionary have the same dense dimension."
         dense_axes = dense_axes[0]
 
         return dense_axes
 
-    def _categorical_axes(self, is_mc=True):
+    def _categorical_axes(self, mc=True):
         '''Returns the list of categorical axes of a histogram.'''
         # Since MC and data have different categorical axes, the argument mc needs to specified
-        if is_mc:
+        if mc:
             d = {s: v for s, v in self.h_dict.items() if s in self.samples_mc}
         else:
             d = {s: v for s, v in self.h_dict.items() if s in self.samples_data}
         categorical_axes_dict = {s: [] for s in d.keys()}
 
         for s, h in d.items():
             for ax in h.axes:
                 if type(ax) in [hist.axis.StrCategory, hist.axis.IntCategory]:
                     categorical_axes_dict[s].append(ax)
         categorical_axes = list(categorical_axes_dict.values())
-        error_msg = f"The Shape object `{self.name}` contains histograms with different categorical axes in the %1 datasets.\nMismatching axes:\n"
-        if is_mc:
-            error_msg = error_msg.replace("%1", "MC")
-        else:
-            error_msg = error_msg.replace("%1", "Data")
-        for v in categorical_axes:
-            for i, axis in enumerate(v):
-                if axis != categorical_axes[0][i]:
-                    error_msg += f"{axis}\n" + f"{categorical_axes[0][i]}"
-                    raise Exception(error_msg)
+        assert all(
+            v == categorical_axes[0] for v in categorical_axes
+        ), "Not all the histograms in the dictionary have the same categorical dimension."
         categorical_axes = categorical_axes[0]
 
         return categorical_axes
 
     @property
     def categorical_axes_mc(self):
         '''Returns the list of categorical axes of a MC histogram.'''
-        return self._categorical_axes(is_mc=True)
+        return self._categorical_axes(mc=True)
 
     @property
     def categorical_axes_data(self):
         '''Returns the list of categorical axes of a data histogram.'''
-        return self._categorical_axes(is_mc=False)
+        return self._categorical_axes(mc=False)
 
     @property
     def dense_dim(self):
         '''Returns the number of dense axes of a histogram.'''
         return len(self.dense_axes)
 
-    def get_axis_items(self, axis_name, is_mc):
+    def get_axis_items(self, axis_name, mc=True):
         '''Returns the list of values contained in a Hist axis.'''
-        if is_mc:
+        if mc:
             axis = [ax for ax in self.categorical_axes_mc if ax.name == axis_name][0]
         else:
             axis = [ax for ax in self.categorical_axes_data if ax.name == axis_name][0]
         return list(axis.value(range(axis.size)))
 
-    def _stack_sum(self, cat=None, is_mc=None, stack=None):
+    def _stack_sum(self, cat=None, mc=None, stack=None):
         '''Returns the sum histogram of a stack (`hist.stack.Stack`) of histograms.'''
         if not stack:
             if not cat:
                 raise Exception("The category `cat` should be passed when the `stack` option is not specified.")
-            if is_mc:
+            if mc:
                 stack = self._stacksCache[cat]["mc"]
             else:
                 stack = self._stacksCache[cat]["data"]
         if len(stack) == 1:
             return stack[0]
         else:
             htot =hist.Hist(stack[0])
             for h in stack[1:]:
                 htot = htot + h
             return htot
 
     @property
     def stack_sum_data(self, cat):
         '''Returns the sum histogram of a stack (`hist.stack.Stack`) of data histograms.'''
-        return self._stack_sum(cat, is_mc=False)
+        return self._stack_sum(cat, mc=False)
 
     @property
     def stack_sum_mc_nominal(self, cat):
         '''Returns the sum histogram of a stack (`hist.stack.Stack`) of MC histograms.'''
-        return self._stack_sum(cat, is_mc=True)
+        return self._stack_sum(cat, mc=True)
 
     @property
     def samples(self):
         return list(self.h_dict.keys())
 
     @property
     def samples_data(self):
@@ -396,140 +356,90 @@
     def group_samples(self):
         '''Groups samples according to the dictionary self.style.samples_map'''
         # # First of all check if collapse_datasets options is true,
         # # in that case all the datasets (parts) for each sample are summed
         if self.style.collapse_datasets:
             # Sum over the different datasets for each sample
             for sample, datasets in self.h_dict.items():
-                #print("Grouping:", sample, datasets)
                 self.h_dict[sample] = self._stack_sum(
                     stack=hist.Stack.from_dict(
                         {s: h for s, h in datasets.items() if s in datasets}
                     )
                 )
                 isMC = None
                 for dataset in datasets:
                     isMC_d = self.datasets_metadata[dataset]["isMC"] == "True"
                     if isMC is None:
                         isMC = isMC_d
                         self.sample_is_MC[sample] = isMC
                     elif isMC != isMC_d:
                         raise Exception(f"You are collapsing together data and MC histogram!")
-
+                    
         else:
             raise NotImplementedError("Plotting histograms without collapsing is still not implemented")
-
+        
         if not self.style.has_samples_groups:
             return
         h_dict_grouped = {}
         samples_in_map = []
-
-        cleaned_samples_list = self.style.samples_groups.copy()
         for sample_new, samples_list in self.style.samples_groups.items():
-            #print(sample_new, samples_list)
-            for s_to_group in samples_list:
-                if s_to_group not in self.h_dict.keys():
-                    if self.verbose>=0:
-                        print("WARNING. Sample ",s_to_group," is not in the list of samples: ", list(self.h_dict.keys()), "Skipping it.")
-                    cleaned_samples_list[sample_new].remove(s_to_group)
-                    continue
-                if self.verbose>=1:
-                    print("\t Sample ",s_to_group," will be grouped into sample", sample_new)
-
-        for sample_new, samples_list in cleaned_samples_list.items():
-            if len(samples_list)==0:
-                if self.verbose>=1:
-                    print("WARNING. The list of samples to group is empty!  Group name:", sample_new)
-                continue
-            
             h_dict_grouped[sample_new] = self._stack_sum(
                 stack=hist.Stack.from_dict(
                     {s: h for s, h in self.h_dict.items() if s in samples_list}
                 )
             )
-            isMC = self.sample_is_MC[samples_list[0]]
-            self.sample_is_MC[sample_new] = self.sample_is_MC[samples_list[0]]
             samples_in_map += samples_list
-
         for s, h in self.h_dict.items():
             if s not in samples_in_map:
                 h_dict_grouped[s] = h
         self.h_dict = deepcopy(h_dict_grouped)
+        
 
-    def exclude_samples(self):
-        if not self.style.has_exclude_samples:
-            return
-
-        samples_to_exclude = self.style.exclude_samples
-        h_dict_excluded = {}
-        for s, h in self.h_dict.items():
-            if s not in samples_to_exclude:
-                h_dict_excluded[s] = h
-
-        self.h_dict = deepcopy(h_dict_excluded)
-
-    def rescale_samples(self):
-        if not self.style.has_rescale_samples:
-            return
-        for sample,scale in self.style.rescale_samples.items():
-
-            if sample in self.h_dict.keys():
-                if self.verbose>=2:
-                    print("Rescaling hist", self.h_dict[sample].name, "in sample",sample, " by ", scale)
-                self.h_dict[sample] = self.h_dict[sample]*scale
-            else:
-                if self.verbose>0:
-                    print("Warning: the rescaling sample is not among the samples in the histograms. Nothing will be rescaled! ")
-                    print("\t Rescale requested for:", sample, ";  hists exist:", self.h_dict.keys())
-                    
     def _get_stacks(self, cat, spliteras=False):
         '''Builds the data and MC stacks, applying a slicing by category.
         The stacks are cached in a dictionary so that they are not recomputed every time.
         If spliteras is True, the extra axis "era" is kept in the data stack to
         distinguish between data samples from different data-taking eras.'''
         if not cat in self._stacksCache:
             stacks = {}
-            if not self.is_data_only:
-                slicing_mc = {'cat': cat}
-                slicing_mc_nominal = {'cat': cat, 'variation': 'nominal'}
-                h_dict_mc = {d: self.h_dict[d][slicing_mc] for d in self.samples_mc}
-                h_dict_mc_nominal = {
-                    d: self.h_dict[d][slicing_mc_nominal] for d in self.samples_mc
-                }
-                # Store number of weighted MC events
-                self.nevents = {
-                    d: round(sum(h_dict_mc_nominal[d].values()), 1)
-                    for d in self.samples_mc
-                }
-
-                # Order the events dictionary by decreasing number of events if linear scale, increasing if log scale
-                reverse = True
-                if self.log:
-                    reverse = False
-                self.nevents = dict(
-                    sorted(self.nevents.items(), key=lambda x: x[1], reverse=reverse)
-                )
-                color = iter(cm.gist_rainbow(np.linspace(0, 1, len(self.nevents.keys()))))
-                # Assign random colors to each sample
-                self.colors = [next(color) for d in self.nevents.keys()]
-                if hasattr(self.style, "colors_mc"):
-                    # Initialize random colors
-                    for i, d in enumerate(self.nevents.keys()):
-                        # If the color for a corresponding sample exists in the dictionary, assign the color to the sample
-                        if d in self.style.colors_mc:
-                            self.colors[i] = self.style.colors_mc[d]
-                # Order the MC dictionary by number of events
-                h_dict_mc = {d: h_dict_mc[d] for d in self.nevents.keys()}
-                h_dict_mc_nominal = {
-                    d: h_dict_mc_nominal[d] for d in self.nevents.keys()
-                }
-                # Build MC stack with variations and nominal MC stack
-                stacks["mc"] = hist.Stack.from_dict(h_dict_mc)
-                stacks["mc_nominal"] = hist.Stack.from_dict(h_dict_mc_nominal)
-                stacks["mc_nominal_sum"] = self._stack_sum(stack = stacks["mc_nominal"])
+            slicing_mc = {'cat': cat}
+            slicing_mc_nominal = {'cat': cat, 'variation': 'nominal'}
+            h_dict_mc = {d: self.h_dict[d][slicing_mc] for d in self.samples_mc}
+            h_dict_mc_nominal = {
+                d: self.h_dict[d][slicing_mc_nominal] for d in self.samples_mc
+            }
+            # Store number of weighted MC events
+            self.nevents = {
+                d: round(sum(h_dict_mc_nominal[d].values()), 1)
+                for d in self.samples_mc
+            }
+            reverse = True
+            # Order the events dictionary by decreasing number of events if linear scale, increasing if log scale
+            # N.B.: Here implement if log: reverse=False
+            self.nevents = dict(
+                sorted(self.nevents.items(), key=lambda x: x[1], reverse=reverse)
+            )
+            color = iter(cm.gist_rainbow(np.linspace(0, 1, len(self.nevents.keys()))))
+            # Assign random colors to each sample
+            self.colors = [next(color) for d in self.nevents.keys()]
+            if hasattr(self.style, "colors_mc"):
+                # Initialize random colors
+                for i, d in enumerate(self.nevents.keys()):
+                    # If the color for a corresponding sample exists in the dictionary, assign the color to the sample
+                    if d in self.style.colors_mc:
+                        self.colors[i] = self.style.colors_mc[d]
+            # Order the MC dictionary by number of events
+            h_dict_mc = {d: h_dict_mc[d] for d in self.nevents.keys()}
+            h_dict_mc_nominal = {
+                d: h_dict_mc_nominal[d] for d in self.nevents.keys()
+            }
+            # Build MC stack with variations and nominal MC stack
+            stacks["mc"] = hist.Stack.from_dict(h_dict_mc)
+            stacks["mc_nominal"] = hist.Stack.from_dict(h_dict_mc_nominal)
+            stacks["mc_nominal_sum"] = self._stack_sum(stack = stacks["mc_nominal"])
 
             if not self.is_mc_only:
                 # Sum over eras if specified as extra argument
                 if 'era' in [ax.name for ax in self.categorical_axes_data]:
                     if spliteras:
                         slicing_data = { 'cat': cat}
                     else:
@@ -543,41 +453,28 @@
                         slicing_data = {'cat': cat}
                 self.h_dict_data = {
                     d: self.h_dict[d][slicing_data] for d in self.samples_data
                 }
                 stacks["data"] = hist.Stack.from_dict(self.h_dict_data)
                 stacks["data_sum"] = self._stack_sum(stack = stacks["data"])
             self._stacksCache[cat] = stacks
-            if not self.is_data_only:
-                self.syst_manager.update()
+            self.syst_manager.update()
         return self._stacksCache[cat]
 
-    def _is_empty(self, cat):
-        '''Checks if the data and MC stacks are empty.'''
-        is_empty = True
-        if not self.is_data_only:
-            if sum(self._stacksCache[cat]["mc_nominal_sum"].values()) != 0:
-                is_empty = False
-        if not self.is_mc_only:
-            if sum(self._stacksCache[cat]["data_sum"].values()) != 0:
-                is_empty = False
-        return is_empty
-
     def get_datamc_ratio(self, cat):
         '''Computes the data/MC ratio and the corresponding uncertainty.'''
         stacks = self._get_stacks(cat)
         num = stacks["data_sum"].values()
 
         den = stacks["mc_nominal_sum"].values()
 
         if np.any(den <0 ):
-            if self.verbose>0:
-                print(f"WARNING: negative bins in MC of shape {self.name}. BE CAREFUL! Putting negative bins to 0 for plotting..")
+            print(f"WARNING: negative bins in MC of shape {self.name}. BE CAREFUL! Putting negative bins to 0 for plotting..")
         den[den < 0] = 0
-
+            
         ratio = num / den
         # TO DO: Implement Poisson interval valid also for num~0
         # np.sqrt(num) is just an approximation of the uncertainty valid at large num
         ratio_unc = np.sqrt(num) / den
         ratio_unc[np.isnan(ratio_unc)] = np.inf
 
         return ratio, ratio_unc
@@ -640,39 +537,32 @@
             else:
                 reference_shape = stacks["data_sum"].values()
             if self.density:
                 integral = sum(reference_shape) * np.array(self.style.opts_axes["xbinwidth"])
                 reference_shape = reference_shape / integral
             ymax = max(reference_shape)
             if not np.isnan(ymax):
-                if ymax==0: ymax=1
                 self.ax.set_ylim((0, 2.0 * ymax))
         if ratio:
             self.ax.set_xlabel("")
             self.rax.set_xlabel(self.style.opts_axes["xlabel"], fontsize=self.style.fontsize)
             self.rax.set_ylabel("Data / MC", fontsize=self.style.fontsize)
             self.rax.yaxis.set_label_coords(-0.075, 1)
             self.rax.tick_params(axis='x', labelsize=self.style.fontsize)
             self.rax.tick_params(axis='y', labelsize=self.style.fontsize)
             self.rax.set_ylim((0.5, 1.5))
         if self.style.has_labels:
             handles, labels = self.ax.get_legend_handles_labels()
             labels_new = []
             handles_new = []
             for i, l in enumerate(labels):
-                # If additional scale is provided, plot it on the legend:
-                scale_str = ""
-                if self.style.has_rescale_samples and l in self.style.rescale_samples.keys():
-                    scale_str = " x%.2f"%self.style.rescale_samples[l]
                 if l in self.style.labels_mc:
-                    
-                    labels_new.append(f"{self.style.labels_mc[l]}"+scale_str)
+                    labels_new.append(f"{self.style.labels_mc[l]}")
                 else:
-                    labels_new.append(l+scale_str)
-                    
+                    labels_new.append(l)
                 handles_new.append(handles[i])
             labels = labels_new
             handles = handles_new
             self.ax.legend(
                 handles,
                 labels,
                 fontsize=self.style.fontsize,
@@ -698,30 +588,24 @@
         )
         self.format_figure(cat, ratio=False)
 
     def plot_data(self, cat, ax=None):
         '''Plots the data histogram as an errorbar plot.'''
         stacks = self._get_stacks(cat)
         if self.dense_dim > 1:
-            print(f"WARNING: cannot plot data for histogram {self.name} with dimension {self.dense_dim}.")
+            print(f"WARNING: cannot plot data/MC for histogram {self.name} with dimension {self.dense_dim}.")
             print("The method `plot_data` will be skipped.")
             return
 
         if ax:
             self.ax = ax
         else:
             if not hasattr(self, "ax"):
                 self.define_figure(ratio=False)
         y = stacks["data_sum"].values()
-        # Add underflow and overflow bins to the first and last bin, respectively
-        if self.style.opts_mc["flow"] == "sum":
-            y_underflow = stacks["data_sum"][hist.underflow].value
-            y_overflow = stacks["data_sum"][hist.overflow].value
-            y[0] += y_underflow
-            y[-1] += y_overflow
         yerr = np.sqrt(y)
         integral = sum(y) * np.array(self.style.opts_axes["xbinwidth"])
         if self.density:
             y = y / integral
             yerr = yerr / integral
         self.ax.errorbar(self.style.opts_axes["xcenters"], y, yerr=yerr, **self.style.opts_data)
         self.format_figure(cat, ratio=False)
@@ -735,19 +619,14 @@
 
         ratio, ratio_unc = self.get_datamc_ratio(cat)
         if ax:
             self.rax = ax
         else:
             if not hasattr(self, "rax"):
                 self.define_figure(ratio=True)
-
-        # Removing nans and inf
-        np.nan_to_num(ratio, copy=False)
-        np.nan_to_num(ratio_unc, copy=False)
-
         self.rax.errorbar(
             self.style.opts_axes["xcenters"], ratio, yerr=ratio_unc, **self.style.opts_data
         )
         self.format_figure(cat, ratio=True)
 
     def plot_systematic_uncertainty(self, cat, ratio=False, ax=None):
         '''Plots the asymmetric systematic uncertainty band on top of the MC stack, if `ratio` is set to False.
@@ -809,54 +688,51 @@
         if ax:
             self.ax = ax
         if rax:
             self.rax = rax
         if (not self.is_mc_only) & (not self.is_data_only):
             self.plot_mc(cat)
             self.plot_data(cat)
-            if syst & (not self._is_empty(cat)):
+            if syst:
                 self.plot_systematic_uncertainty(cat)
         elif self.is_mc_only:
             self.plot_mc(cat)
-            if syst & (not self._is_empty(cat)):
+            if syst:
                 self.plot_systematic_uncertainty(cat)
         elif self.is_data_only:
             self.plot_data(cat)
 
         if ratio:
             self.plot_datamc_ratio(cat)
-            if syst & (not self._is_empty(cat)):
+            if syst:
                 self.plot_systematic_uncertainty(cat, ratio=ratio)
 
         self.format_figure(cat, ratio=ratio)
 
     def plot_datamc_all(self, ratio=True, syst=True, spliteras=False, save=True):
         '''Plots the data and MC histograms for each year and category contained in the histograms.
         If ratio is True, also the Data/MC ratio plot is plotted.
         If syst is True, also the total systematic uncertainty is plotted.'''
         if self.dense_dim > 1:
             print(f"WARNING: cannot plot data/MC for histogram {self.name} with dimension {self.dense_dim}.")
             print("The method `plot_datamc_all` will be skipped.")
             return
 
         for cat in self.categories:
-            if self.verbose>1:
-                print('Plotting category:', cat)
             if self.only_cat and cat not in self.only_cat:
                 continue
             self.define_figure(ratio)
             self.plot_datamc(cat, ratio=ratio, syst=syst)
             if save:
                 plot_dir = os.path.join(self.plot_dir, cat)
                 if self.log:
                     filepath = os.path.join(plot_dir, f"log_{self.name}_{cat}.png")
                 else:
                     filepath = os.path.join(plot_dir, f"{self.name}_{cat}.png")
-                if self.verbose>0:
-                    print("Saving", filepath)
+                print("Saving", filepath)
                 plt.savefig(filepath, dpi=150, format="png")
             else:
                 plt.show(self.fig)
             plt.close(self.fig)
 
 
 class SystManager:
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/utils/run.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/run.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/utils/skim.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/skim.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/utils/utils.py` & `pocket_coffea-1.0rc3/pocket_coffea/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/workflows/base.py` & `pocket_coffea-1.0rc3/pocket_coffea/workflows/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,21 +68,17 @@
         self.custom_axes = []
         self.custom_histogram_fields = {}
 
         # Output format
         # Accumulators for the output
         self.output_format = {
             "sum_genweights": {},
-            "sum_signOf_genweights": {},
             "sumw": {
                 cat: {} for cat in self._categories
             },
-            "sumw2": {
-                cat: {} for cat in self._categories
-            },
             "cutflow": {
                 "initial": {},
                 "skim": {},
                 "presel": {},
                 **{cat: {} for cat in self._categories},
             },
             "variables": {
@@ -124,15 +120,15 @@
         if self._isMC:
             self._era = "MC"
             self._xsec = self.events.metadata["xsec"]
         else:
             self._era = self.events.metadata["era"]
         # Loading metadata for subsamples
         self._hasSubsamples = self.cfg.has_subsamples[self._sample]
-
+        
     def load_metadata_extra(self):
         '''
         Function that can be called by a derived processor to define additional metadata.
         For example load additional information for a specific sample.
         '''
         pass
 
@@ -144,18 +140,18 @@
           - METfilters,
           - PV requirement *at least 1 good primary vertex
           - lumi-mask (for DATA): applied the goldenJson selection
           - requested HLT triggers (from configuration, not hardcoded in the processor)
           - **user-defined** skimming cuts
 
         BE CAREFUL: the skimming is done before any object preselection and cleaning.
-        Only collections and branches already present in the NanoAOD before any corrections
+        Only collections and branches already present in the NanoAOD before any correct
         can be used.
-        Alternatively, if you need to apply the cut on preselected objects -
-        define the cut at the preselection level, not at skim level.
+        Alternatively, if you need to apply the cut on preselected objects,
+        defined the cut at the preselection level, not at skim level.
         '''
         self._skim_masks = PackedSelection()
         mask_flags = np.ones(self.nEvents_initial, dtype=bool)
         flags = self.params.event_flags[self._year]
         if not self._isMC:
             flags += self.params.event_flags_data[self._year]
         for flag in flags:
@@ -229,15 +225,15 @@
         pass
 
     @abstractmethod
     def count_objects(self, variation):
         '''
         Function that counts the preselected objects and save the counts as attributes of `events`.
         The function **must** be defined by the user processor.
-        '''
+        ''' 
         pass
 
     def apply_preselections(self, variation):
         '''The function computes all the masks from the preselection cuts
         and filter out the events to speed up the later computations.
         N.B.: Preselection happens after the objects correction and cleaning.'''
 
@@ -333,15 +329,14 @@
                 self.nEvents_after_presel,
                 self.events,  # to compute weights
                 storeIndividual=False,
                 shape_variation=variation,
                 metadata={
                     "year": self._year,
                     "sample": self._sample,
-                    "dataset": self._dataset,
                     "part": self._samplePart,
                     "xsec": self._xsec,
                 },
             )
 
     def compute_weights_extra(self, variation):
         '''Function that can be defined by user processors
@@ -364,26 +359,24 @@
             else:
                 mask_on_events = mask
 
             self.output["cutflow"][category][self._dataset] = {self._sample: ak.sum(mask_on_events)}
             if self._isMC:
                 w = self.weights_manager.get_weight(category)
                 self.output["sumw"][category][self._dataset] = {self._sample: ak.sum(w * mask_on_events)}
-                self.output["sumw2"][category][self._dataset] = {self._sample: ak.sum((w**2) * mask_on_events)}
 
             # If subsamples are defined we also save their metadata
             if self._hasSubsamples:
                 for subs, subsam_mask in self._subsamples[self._sample].get_masks():
                     mask_withsub = mask_on_events & subsam_mask
                     self.output["cutflow"][category][self._dataset][f"{self._sample}__{subs}"] = ak.sum(mask_withsub)
                     if self._isMC:
                         self.output["sumw"][category][self._dataset][f"{self._sample}__{subs}"] = ak.sum(w * mask_withsub)
-                        self.output["sumw2"][category][self._dataset][f"{self._sample}__{subs}"] = ak.sum((w**2) * mask_withsub)
-
 
+                        
     def define_custom_axes_extra(self):
         '''
         Function which get called before the definition of the Histogram
         manager.
         It is used to defined extra custom axes for the histograms
         depending on the current chunk metadata.
         E.g.: it can be used to add a `era` axes only for data.
@@ -444,27 +437,27 @@
             # there are no subsamples
             if self._hasSubsamples:
                 name = f"{self._sample}__{subs}"
             else:
                 name = self._sample
             for var, H in self.hists_managers.get_histograms(subs).items():
                 self.output["variables"][var][name][self._dataset] = H
-
+                
 
     def fill_histograms_extra(self, variation):
         '''
         The function get called after the filling of the default histograms.
         Redefine it to fill custom histograms
         '''
         pass
 
     def define_column_accumulators(self):
         '''
-        Define the ColumnsManagers to handle the requested columns from the configuration.
-        If Subsamples are defined a columnsmanager is created for each of them.
+        Define the ColumsManagers to handle the requested columns from the configuration.
+        If Subsamples are defined a columnsmager is created for each of them.
         '''
         self.column_managers = {}
         for subs in self._subsamples[self._sample].keys():
             if self._hasSubsamples:
                 name = f"{self._sample}__{subs}"
             else:
                 name = self._sample
@@ -482,35 +475,35 @@
 
     def fill_column_accumulators(self, variation):
         if variation != "nominal":
             return
 
         if len(self.column_managers) == 0:
             return
-
+    
         outcols = self.output["columns"]
         # TODO Fill column accumulator for different variations
         if self._hasSubsamples:
             # call the filling for each
             for subs in self._subsamples[self._sample].keys():
-                if self.workflow_options!=None and self.workflow_options.get("dump_columns_as_arrays_per_chunk", None)!=None:
+                if self.workflow_options.get("dump_columns_as_arrays_per_chunk", None)!=None:
                     # filling awkward arrays to be dumped per chunk
                     if self.column_managers[subs].ncols == 0: break
                     out_arrays = self.column_managers[subs].fill_ak_arrays(
                                                self.events,
                                                self._categories,
                                                subsample_mask=self._subsamples[self._sample].get_mask(subs),
                                                weights_manager=self.weights_manager
                                                )
                     fname = (self.events.behavior["__events_factory__"]._partition_key.replace( "/", "_" )
                         + ".parquet")
-                    for category, akarr in out_arrays.items():
+                    for category, akarr in out_arrays.items(): 
                         # building the file name
-                        subdirs = [self._dataset, subs, category]
-                        dump_ak_array(akarr, fname, self.workflow_options["dump_columns_as_arrays_per_chunk"]+"/", subdirs)
+                        subdirs = [self._dataset, sub, category]
+                        dump_ak_array(akarray, fname, self.workflow_options["dump_columns_as_arrays_per_chunk"]+"/", subdirs)
 
 
                 else:
                     # Filling columns to be accumulated for all the chunks
                     # Calling hist manager with a subsample mask
                     if self.column_managers[subs].ncols == 0: break
                     self.output["columns"][f"{self._sample}__{subs}"]= {
@@ -520,15 +513,15 @@
                                                    subsample_mask=self._subsamples[self._sample].get_mask(subs),
                                                    weights_manager=self.weights_manager
                                                    )
                     }
         else:
             # NO subsamples
             if self.column_managers[self._sample].ncols == 0: return
-            if self.workflow_options!=None and self.workflow_options.get("dump_columns_as_arrays_per_chunk", None)!=None:
+            if self.workflow_options.get("dump_columns_as_arrays_per_chunk", None)!=None:
                 out_arrays = self.column_managers[self._sample].fill_ak_arrays(
                                                self.events,
                                                self._categories,
                                                subsample_mask=None,
                                                weights_manager=self.weights_manager
                                                )
                 # building the file name
@@ -565,80 +558,59 @@
     @classmethod
     def available_variations(cls):
         '''
         Identifiers of the weights variabtions available thorugh this processor.
         By default they are all the weights defined in the WeightsManager
         '''
         vars = WeightsManager.available_variations()
-        available_jet_types = [
-            "AK4PFchs",
-            "AK8PFPuppi"
-        ]
-        available_jet_variations = [
-            "JES_Total",
-            'JES_FlavorQCD',
-            'JES_RelativeBal',
-            'JES_HF',
-            'JES_BBEC1',
-            'JES_EC2',
-            'JES_Absolute',
-            'JES_Absolute_2018',
-            'JES_HF_2018',
-            'JES_EC2_2018',
-            'JES_RelativeSample_2018',
-            'JES_BBEC1_2018',
-            'JER',
-        ]
-        # Here we define the naming scheme for the jet variations
-        # For each jet type, we define the variations names as `{variation}_{jet_type}`
-        available_jet_variations = [f"{v}_{jt}" for v in available_jet_variations for jt in available_jet_types]
-        vars.update(available_jet_variations)
+        vars.update(
+            [
+                "JES_Total",
+                'JES_FlavorQCD',
+                'JES_RelativeBal',
+                'JES_HF',
+                'JES_BBEC1',
+                'JES_EC2',
+                'JES_Absolute',
+                'JES_Absolute_2018',
+                'JES_HF_2018',
+                'JES_EC2_2018',
+                'JES_RelativeSample_2018',
+                'JES_BBEC1_2018',
+                'JER',
+            ]
+        )
         return vars
 
     def get_shape_variations(self):
         '''
         Generator for shape variations.
         '''
         if not self._isMC:
             yield "nominal"
             return
         # nominal is assumed to be the first
         variations = ["nominal"] + self.cfg.available_shape_variations[self._sample]
         # TO be understood if a copy is needed
-        # This can be useless or suboptimal, working on it
+        # This canbe useless or suboptimal, working on it
         nominal_events = self.events
 
-        # Define flags to know if the variations include JES or JER
-        has_jes = any(["JES" in v for v in variations])
-        has_jer = any(["JER" in v for v in variations])
-
-        # Extract the jet type to calibrate from the variation name
-        # Expected format: `JES_Total_AK4PFchs`
-        jet_types_to_calibrate = []
-        if has_jes:
-            jet_types_to_calibrate += set([v.split("_")[-1] for v in variations if "JES" in v])
-        if has_jer:
-            jet_types_to_calibrate += set([v.split("_")[-1] for v in variations if "JER" in v])
-        jet_types_to_calibrate = set(jet_types_to_calibrate)
-
         # Calibrating Jets: only the ones in the jet_types in the params.jet_calibration config
         jets_calibrated = {}
         caches = []
         jet_calib_params= self.params.jets_calibration
-        if has_jes or has_jer:
+        if "JES" in variations or "JER" in variations:
             for jet_type, factory in jet_calib_params.jet_types.items():
-                # If the jet_type read from the parameters is not included in the variations, we skip it
-                if not jet_type in jet_types_to_calibrate: continue
                 cache = cachetools.Cache(np.inf)
                 caches.append(cache)
-                jet_coll_name = jet_calib_params.collection[jet_type]
-                jets_calibrated[jet_coll_name] = jet_correction(
+                jet_coll = jet_calib_params.collection[jet_type]
+                jets_calibrated[jet_coll] = jet_correction(
                     params=self.params,
                     events=nominal_events,
-                    jets=nominal_events[jet_coll_name],
+                    jets=nominal_events[jet_coll],
                     factory=self.jmefactory,
                     jet_type = jet_type,
                     year=self._year,
                     cache=cache
                 )
 
         for variation in variations:
@@ -650,50 +622,44 @@
             # very costly!
 
             if variation == "nominal":
                 self.events = nominal_events
                 # Just assign the nominal calibration
                 for jet_coll_name, jet_coll in jets_calibrated.items():
                     self.events[jet_coll_name] = jet_coll
-
+                
                 yield "nominal"
 
-
+                
             elif ("JES" in variation) | ("JER" in variation):
                 # JES_jes is the total. JES_[type] is for different variations
-                # We recover the variation name and the jet type by splitting the variation name
-                variation_name = '_'.join(variation.split("_")[:-1])
-                jet_type = variation.split("_")[-1]
                 self.events = nominal_events
-
-                # We vary ONLY the jet collection corresponding to the jet type in the variation name
-                # This way, we vary independently the different jet types
-                # e.g. `JES_Total_AK4PFchs` will vary only the `AK4PFchs` jets,
-                # while `JES_Total_AK8PFPuppi` will vary only the `AK8PFPuppi` jets
-                jet_coll_name = jet_calib_params.collection[jet_type]
-                self.events[jet_coll_name] = jets_calibrated[jet_coll_name][variation_name].up
+                for jet_coll_name, jet_coll in jets_calibrated.items():
+                    self.events[jet_coll_name] = jet_coll[variation].up
 
                 yield variation + "Up"
 
-                # restore nominal before saving the down-variated collection
+                # then go down
+                # restore nominal before going to down
                 self.events = nominal_events
-                self.events[jet_coll_name] = jets_calibrated[jet_coll_name][variation_name].down
-
+                for jet_coll_name, jet_coll in jets_calibrated.items():
+                    self.events[jet_coll_name] = jet_coll[variation].down
+                
                 yield variation + "Down"
 
 
         # additional shape variations are handled with custom provided generators
         for additional_variation in self.get_extra_shape_variations():
             yield additional_variation
-
+        
     def get_extra_shape_variations(self):
         #empty generator
         return
         yield  # the yield defines the function as a generator and the return stops it to be empty
-
+        
     def process(self, events: ak.Array):
         '''
         This function get called by Coffea on each chunk of NanoAOD file.
         The processing steps of PocketCoffea are defined in this function.
 
         Customization points for user-defined processor are provided as
         `_extra` functions. By redefining those functions the user can change the behaviour
@@ -726,15 +692,14 @@
         self.load_metadata_extra()
 
         self.nEvents_initial = self.nevents
         self.output['cutflow']['initial'][self._dataset] = self.nEvents_initial
         if self._isMC:
             # This is computed before any preselection
             self.output['sum_genweights'][self._dataset] = ak.sum(self.events.genWeight)
-            self.output['sum_signOf_genweights'][self._dataset] = ak.sum(np.sign(self.events.genWeight))
 
         self.weights_config = self.weights_config_allsamples[self._sample]
         ########################
         # Then the first skimming happens.
         # Events that are for sure useless are removed.
         # The user can specify in the configuration a function to apply for the skiming.
         # BE CAREFUL: objects are not corrected and cleaned at this stage, the skimming
@@ -805,80 +770,48 @@
             # Count events
             if variation == "nominal":
                 self.count_events(variation)
 
         return self.output
 
 
-    def rescale_sumgenweights(self, output):
+    def rescale_sumgenweights(self, sumgenw_dict, output):
         # rescale each variable
-
         for var, vardata in output["variables"].items():
-            for samplename, dataset_in_sample in vardata.items():
+            for sample, dataset_in_sample in vardata.items():
                 for dataset, histo in dataset_in_sample.items():
-                    # First, determine whether we must use the sum_signOf_genweights or sum_genweights for rescaling.
-                    # This information is taken from a weights config file for each _sample_
-                    # Getting the original sample name to check weights config
-                    sample = self.cfg.subsamples_reversed_map[samplename] #needed for subsamples
-                    wei = self.cfg.weights_config[sample]['inclusive']
-                    if 'signOf_genWeight' in wei and 'genWeight' not in wei:
-                        sumgenw_dict = output["sum_signOf_genweights"]
-                    else:
-                        sumgenw_dict = output["sum_genweights"]
                     if dataset in sumgenw_dict:
                         scaling = 1/sumgenw_dict[dataset]
                         # it  means that's a MC sample
                         histo *= scaling
 
         # rescale sumw
         for cat, catdata in output["sumw"].items():
             for dataset, dataset_data in catdata.items():
-                # Getting the first sample for the dataset in the "sumw" output
-                # it is working also for subsamples before the first sample key is the primary sample
-                sample_from_dataset = list(dataset_data.keys())[0]
-                wei = self.cfg.weights_config[sample_from_dataset]['inclusive']
-                if 'signOf_genWeight' in wei and 'genWeight' not in wei:
-                    sumgenw_dict = output["sum_signOf_genweights"]
-                else:
-                    sumgenw_dict = output["sum_genweights"]
-
                 if dataset in sumgenw_dict:
                     scaling = 1/sumgenw_dict[dataset]
                     for sample in dataset_data.keys():
-                        dataset_data[sample] *= scaling
-
-        # rescale sumw2
-        for cat, catdata in output["sumw2"].items():
-            for dataset, dataset_data in catdata.items():
-                sample_from_dataset = list(dataset_data.keys())[0]
-                wei = self.cfg.weights_config[sample_from_dataset]['inclusive']
-                if 'signOf_genWeight' in wei and 'genWeight' not in wei:
-                    sumgenw_dict = output["sum_signOf_genweights"]
-                else:
-                    sumgenw_dict = output["sum_genweights"]
-                if dataset in sumgenw_dict:
-                    scaling = 1/sumgenw_dict[dataset]**2
-                    for sample in dataset_data.keys():
-                        dataset_data[sample] *= scaling
-
+                        dataset_data[sample] *= scaling                        
 
     def postprocess(self, accumulator):
         '''
         The function is called by coffea at the end of the processing.
         The default function calls the `rescale_sumgenweights` function to rescale the histograms
         and `sumw` metadata using the sum of the genweights computed without preselections
         for each dataset.
 
         Moreover the function saves in the output a dictionary of metadata
         with the full description of the datasets taken from the configuration.
 
         To add additional customatizaion redefine the `postprocessing` function,
         but remember to include a super().postprocess() call.
         '''
-       
+        if not self.workflow_options.get("donotscale_sumgenweights", False):
+            self.rescale_sumgenweights(accumulator["sum_genweights"], accumulator)
+
         # Saving dataset metadata directly in the output file reading from the config
         dmeta = accumulator["datasets_metadata"] = {
             "by_datataking_period": {},
             "by_dataset": defaultdict(dict)
         }
 
         for dataset in accumulator["cutflow"]["initial"].keys():
@@ -893,13 +826,8 @@
 
             if self.cfg.has_subsamples[sample]:
                 for subsam in self._subsamples[sample].keys():
                     dmeta["by_datataking_period"][year][f"{sample}__{subsam}"].add(dataset)
             else:
                 dmeta["by_datataking_period"][year][sample].add(dataset)
 
-        # Rescale the histograms and sumw using the sum of the genweights
-        if not self.workflow_options.get("donotscale_sumgenweights", False):
-            self.rescale_sumgenweights(accumulator)
-
-
         return accumulator
```

### Comparing `pocket_coffea-0.9.2/pocket_coffea/workflows/genweights.py` & `pocket_coffea-1.0rc3/pocket_coffea/workflows/genweights.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/workflows/semileptonic_triggerSF.py` & `pocket_coffea-1.0rc3/pocket_coffea/workflows/semileptonic_triggerSF.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/workflows/sf_lepton_variations.py` & `pocket_coffea-1.0rc3/pocket_coffea/workflows/sf_lepton_variations.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/pocket_coffea/workflows/tthbb_base_processor.py` & `pocket_coffea-1.0rc3/pocket_coffea/workflows/tthbb_base_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         )
         self.events["LeptonGood"] = leptons[ak.argsort(leptons.pt, ascending=False)]
 
         self.events["JetGood"], self.jetGoodMask = jet_selection(
             self.events, "Jet", self.params, "LeptonGood"
         )
         self.events["BJetGood"] = btagging(
-            self.events["JetGood"], self.params.btagging.working_point[self._year], wp=self.params.object_preselection.Jet["btag"]["wp"]
+            self.events["JetGood"], self.params.btagging.working_point[self._year]
         )
 
         # self.events["FatJetGood"], self.jetGoodMask = jet_selection(
         #     self.events, "FatJet", self.cfg.finalstate
         # )
 
     def count_objects(self, variation):
```

### Comparing `pocket_coffea-0.9.2/profiling/mem.py` & `pocket_coffea-1.0rc3/profiling/mem.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/profiling/parton_matching_semilep_newgenmatch_v4.prof` & `pocket_coffea-1.0rc3/profiling/parton_matching_semilep_newgenmatch_v4.prof`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/profiling/parton_matching_semilep_v3.prof` & `pocket_coffea-1.0rc3/profiling/parton_matching_semilep_v3.prof`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/tests/test_categorization.py` & `pocket_coffea-1.0rc3/tests/test_categorization.py`

 * *Files identical despite different names*

### Comparing `pocket_coffea-0.9.2/tests/test_hlt_cut.py` & `pocket_coffea-1.0rc3/tests/test_hlt_cut.py`

 * *Files identical despite different names*

