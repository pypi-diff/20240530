# Comparing `tmp/nkululeko-0.86.1.tar.gz` & `tmp/nkululeko-0.86.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.86.1.tar", last modified: Wed May 29 12:56:17 2024, max compression
+gzip compressed data, was "nkululeko-0.86.2.tar", last modified: Thu May 30 09:48:37 2024, max compression
```

## Comparing `nkululeko-0.86.1.tar` & `nkululeko-0.86.2.tar`

### file list

```diff
@@ -1,226 +1,226 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.746793 nkululeko-0.86.1/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18230 2024-05-29 12:55:54.000000 nkululeko-0.86.1/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.86.1/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    37088 2024-05-29 12:56:17.746793 nkululeko-0.86.1/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17587 2024-05-29 09:24:25.000000 nkululeko-0.86.1/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.730793 nkululeko-0.86.1/data/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.734793 nkululeko-0.86.1/data/aesdd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.86.1/data/aesdd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.734793 nkululeko-0.86.1/data/androids/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.86.1/data/androids/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.734793 nkululeko-0.86.1/data/androids_orig/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.86.1/data/androids_orig/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.734793 nkululeko-0.86.1/data/androids_test/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.86.1/data/androids_test/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.734793 nkululeko-0.86.1/data/ased/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.86.1/data/ased/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.734793 nkululeko-0.86.1/data/asvp-esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.86.1/data/asvp-esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.734793 nkululeko-0.86.1/data/baved/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.86.1/data/baved/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.734793 nkululeko-0.86.1/data/cafe/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.86.1/data/cafe/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.734793 nkululeko-0.86.1/data/clac/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.86.1/data/clac/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.734793 nkululeko-0.86.1/data/cmu-mosei/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.86.1/data/cmu-mosei/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.734793 nkululeko-0.86.1/data/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.86.1/data/demos/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.734793 nkululeko-0.86.1/data/ekorpus/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.86.1/data/ekorpus/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/emns/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.86.1/data/emns/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/emofilm/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.86.1/data/emofilm/convert_to_16k.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.86.1/data/emofilm/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/emorynlp/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.86.1/data/emorynlp/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/emov-db/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.86.1/data/emov-db/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/emovo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.86.1/data/emovo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/emozionalmente/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.86.1/data/emozionalmente/create.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/enterface/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.86.1/data/enterface/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.86.1/data/esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/gerparas/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.86.1/data/gerparas/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/iemocap/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.86.1/data/iemocap/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/jl/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.86.1/data/jl/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/jtes/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.86.1/data/jtes/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/meld/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.86.1/data/meld/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/mesd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.86.1/data/mesd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/mess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.86.1/data/mess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/mlendsnd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.86.1/data/mlendsnd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/msp-improv/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.86.1/data/msp-improv/process_database2.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/msp-podcast/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.86.1/data/msp-podcast/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/oreau2/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.86.1/data/oreau2/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/portuguese/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.86.1/data/portuguese/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/ravdess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3612 2024-04-22 09:09:10.000000 nkululeko-0.86.1/data/ravdess/process_database.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.86.1/data/ravdess/process_database_speaker.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/savee/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.86.1/data/savee/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/shemo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.86.1/data/shemo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/subesco/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.86.1/data/subesco/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/tess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.86.1/data/tess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/thorsten-emotional/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.86.1/data/thorsten-emotional/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/urdu/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.86.1/data/urdu/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/data/vivae/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.86.1/data/vivae/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.730793 nkululeko-0.86.1/docs/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/docs/source/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3070 2024-04-22 09:09:10.000000 nkululeko-0.86.1/docs/source/conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.730793 nkululeko-0.86.1/meta/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/meta/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.86.1/meta/demos/demo_best_model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.86.1/meta/demos/my_experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.86.1/meta/demos/my_experiment_local.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.86.1/meta/demos/plot_faster_anim.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.738793 nkululeko-0.86.1/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.86.1/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.86.1/nkululeko/aug_train.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.86.1/nkululeko/augment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.742793 nkululeko-0.86.1/nkululeko/augmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.86.1/nkululeko/augmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.86.1/nkululeko/augmenting/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.86.1/nkululeko/augmenting/randomsplicer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.86.1/nkululeko/augmenting/randomsplicing.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3542 2024-05-13 11:40:51.000000 nkululeko-0.86.1/nkululeko/augmenting/resampler.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.742793 nkululeko-0.86.1/nkululeko/autopredict/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.86.1/nkululeko/autopredict/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.86.1/nkululeko/autopredict/ap_age.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.86.1/nkululeko/autopredict/ap_arousal.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.86.1/nkululeko/autopredict/ap_dominance.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.86.1/nkululeko/autopredict/ap_gender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.86.1/nkululeko/autopredict/ap_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.86.1/nkululeko/autopredict/ap_pesq.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.86.1/nkululeko/autopredict/ap_sdr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.86.1/nkululeko/autopredict/ap_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.86.1/nkululeko/autopredict/ap_stoi.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.86.1/nkululeko/autopredict/ap_valence.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5048 2024-04-22 09:09:10.000000 nkululeko-0.86.1/nkululeko/autopredict/estimate_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.86.1/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-05-29 12:56:07.000000 nkululeko-0.86.1/nkululeko/constants.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.742793 nkululeko-0.86.1/nkululeko/data/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.86.1/nkululeko/data/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27650 2024-04-22 09:10:47.000000 nkululeko-0.86.1/nkululeko/data/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3933 2024-05-21 10:44:53.000000 nkululeko-0.86.1/nkululeko/data/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3232 2024-05-03 09:55:35.000000 nkululeko-0.86.1/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.86.1/nkululeko/demo_feats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4757 2024-05-03 09:56:14.000000 nkululeko-0.86.1/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    30986 2024-05-29 12:54:47.000000 nkululeko-0.86.1/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2609 2024-04-30 15:24:17.000000 nkululeko-0.86.1/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.86.1/nkululeko/export.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.742793 nkululeko-0.86.1/nkululeko/feat_extract/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.86.1/nkululeko/feat_extract/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3113 2024-04-23 09:16:18.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3424 2024-04-29 13:37:24.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_agender_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12722 2024-05-03 14:41:56.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3162 2024-04-23 09:16:18.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_auddim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3187 2024-04-23 09:16:18.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3489 2024-04-23 09:16:18.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5196 2024-04-24 17:12:28.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_hubert.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1622 2024-04-23 09:55:16.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4174 2024-04-23 10:17:00.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4028 2024-05-29 07:55:31.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4980 2024-04-23 09:16:18.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3105 2024-04-23 09:16:18.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3670 2024-04-23 09:59:48.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_spectra.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_spkrec.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4617 2024-04-29 13:37:24.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_squim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3228 2024-04-30 09:31:46.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5268 2024-04-29 13:37:24.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4703 2024-04-24 17:06:22.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_wavlm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4533 2024-05-15 15:09:05.000000 nkululeko-0.86.1/nkululeko/feat_extract/feats_whisper.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1541 2024-05-29 07:58:33.000000 nkululeko-0.86.1/nkululeko/feat_extract/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.86.1/nkululeko/feat_extract/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3976 2024-04-23 11:13:33.000000 nkululeko-0.86.1/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.86.1/nkululeko/file_checker.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.86.1/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      525 2024-05-03 12:01:14.000000 nkululeko-0.86.1/nkululeko/glob_conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.742793 nkululeko-0.86.1/nkululeko/losses/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.86.1/nkululeko/losses/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.86.1/nkululeko/losses/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.86.1/nkululeko/losses/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10452 2024-05-17 12:04:16.000000 nkululeko-0.86.1/nkululeko/modelrunner.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.746793 nkululeko-0.86.1/nkululeko/models/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.86.1/nkululeko/models/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11639 2024-05-15 15:09:05.000000 nkululeko-0.86.1/nkululeko/models/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2024-05-03 14:26:57.000000 nkululeko-0.86.1/nkululeko/models/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9954 2024-05-03 14:27:45.000000 nkululeko-0.86.1/nkululeko/models/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      649 2024-05-03 14:28:01.000000 nkululeko-0.86.1/nkululeko/models/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      599 2024-05-03 14:28:22.000000 nkululeko-0.86.1/nkululeko/models/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      610 2024-05-03 14:28:14.000000 nkululeko-0.86.1/nkululeko/models/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      422 2024-05-03 14:28:34.000000 nkululeko-0.86.1/nkululeko/models/model_lin_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9854 2024-05-03 14:29:13.000000 nkululeko-0.86.1/nkululeko/models/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10204 2024-05-03 14:28:58.000000 nkululeko-0.86.1/nkululeko/models/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      940 2024-05-03 14:29:24.000000 nkululeko-0.86.1/nkululeko/models/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      725 2024-05-03 14:29:39.000000 nkululeko-0.86.1/nkululeko/models/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      417 2024-05-03 14:30:08.000000 nkululeko-0.86.1/nkululeko/models/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      428 2024-05-03 14:29:56.000000 nkululeko-0.86.1/nkululeko/models/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18379 2024-05-29 12:54:47.000000 nkululeko-0.86.1/nkululeko/models/model_tuned.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      447 2024-05-03 14:33:39.000000 nkululeko-0.86.1/nkululeko/models/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      418 2024-05-03 14:34:29.000000 nkululeko-0.86.1/nkululeko/models/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5634 2024-04-23 14:42:13.000000 nkululeko-0.86.1/nkululeko/multidb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3725 2024-04-26 06:05:26.000000 nkululeko-0.86.1/nkululeko/nkuluflag.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1968 2024-04-23 12:35:01.000000 nkululeko-0.86.1/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23276 2024-04-29 13:37:24.000000 nkululeko-0.86.1/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2409 2024-04-22 09:09:10.000000 nkululeko-0.86.1/nkululeko/predict.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.746793 nkululeko-0.86.1/nkululeko/reporting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.86.1/nkululeko/reporting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.86.1/nkululeko/reporting/defines.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.86.1/nkululeko/reporting/latex_writer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.86.1/nkululeko/reporting/report.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.86.1/nkululeko/reporting/report_item.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12841 2024-04-25 13:02:38.000000 nkululeko-0.86.1/nkululeko/reporting/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.86.1/nkululeko/reporting/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4267 2024-05-29 12:54:47.000000 nkululeko-0.86.1/nkululeko/resample.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7624 2024-04-22 09:09:10.000000 nkululeko-0.86.1/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.86.1/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.86.1/nkululeko/segment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.746793 nkululeko-0.86.1/nkululeko/segmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.86.1/nkululeko/segmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.86.1/nkululeko/segmenting/seg_inaspeechsegmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.86.1/nkululeko/segmenting/seg_silero.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.86.1/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1677 2024-04-26 06:04:30.000000 nkululeko-0.86.1/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3237 2024-04-25 14:01:11.000000 nkululeko-0.86.1/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8465 2024-05-15 15:09:05.000000 nkululeko-0.86.1/nkululeko/test_pretrain.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.746793 nkululeko-0.86.1/nkululeko/utils/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.86.1/nkululeko/utils/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.86.1/nkululeko/utils/files.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.86.1/nkululeko/utils/stats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13946 2024-05-29 12:54:47.000000 nkululeko-0.86.1/nkululeko/utils/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.746793 nkululeko-0.86.1/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    37088 2024-05-29 12:56:17.000000 nkululeko-0.86.1/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5132 2024-05-29 12:56:17.000000 nkululeko-0.86.1/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-05-29 12:56:17.000000 nkululeko-0.86.1/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-05-29 12:56:17.000000 nkululeko-0.86.1/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-05-29 12:56:17.000000 nkululeko-0.86.1/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.86.1/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-05-29 12:56:17.746793 nkululeko-0.86.1/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.86.1/setup.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.734793 nkululeko-0.86.1/venv/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-29 12:56:17.746793 nkululeko-0.86.1/venv/bin/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.86.1/venv/bin/activate_this.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.849799 nkululeko-0.86.2/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18312 2024-05-30 09:47:56.000000 nkululeko-0.86.2/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.86.2/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    37170 2024-05-30 09:48:37.849799 nkululeko-0.86.2/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17587 2024-05-29 09:24:25.000000 nkululeko-0.86.2/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/aesdd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.86.2/data/aesdd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/androids/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.86.2/data/androids/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/androids_orig/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.86.2/data/androids_orig/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/androids_test/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.86.2/data/androids_test/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/ased/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.86.2/data/ased/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/asvp-esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.86.2/data/asvp-esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/baved/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.86.2/data/baved/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/cafe/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.86.2/data/cafe/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/clac/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.86.2/data/clac/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/cmu-mosei/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.86.2/data/cmu-mosei/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.86.2/data/demos/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/ekorpus/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.86.2/data/ekorpus/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/emns/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.86.2/data/emns/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/emofilm/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.86.2/data/emofilm/convert_to_16k.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.86.2/data/emofilm/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/emorynlp/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.86.2/data/emorynlp/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/emov-db/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.86.2/data/emov-db/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/emovo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.86.2/data/emovo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/emozionalmente/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.86.2/data/emozionalmente/create.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/enterface/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.86.2/data/enterface/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.86.2/data/esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/gerparas/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.86.2/data/gerparas/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/iemocap/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.86.2/data/iemocap/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/jl/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.86.2/data/jl/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/jtes/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.86.2/data/jtes/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/meld/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.86.2/data/meld/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/mesd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.86.2/data/mesd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/mess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.86.2/data/mess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/mlendsnd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.86.2/data/mlendsnd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/msp-improv/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.86.2/data/msp-improv/process_database2.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/msp-podcast/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.86.2/data/msp-podcast/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/oreau2/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.86.2/data/oreau2/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/portuguese/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.86.2/data/portuguese/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/ravdess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3612 2024-04-22 09:09:10.000000 nkululeko-0.86.2/data/ravdess/process_database.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.86.2/data/ravdess/process_database_speaker.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/savee/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.86.2/data/savee/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/shemo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.86.2/data/shemo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/data/subesco/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.86.2/data/subesco/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.841798 nkululeko-0.86.2/data/tess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.86.2/data/tess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.841798 nkululeko-0.86.2/data/thorsten-emotional/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.86.2/data/thorsten-emotional/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.841798 nkululeko-0.86.2/data/urdu/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.86.2/data/urdu/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.841798 nkululeko-0.86.2/data/vivae/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.86.2/data/vivae/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/docs/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.841798 nkululeko-0.86.2/docs/source/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3070 2024-04-22 09:09:10.000000 nkululeko-0.86.2/docs/source/conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/meta/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.841798 nkululeko-0.86.2/meta/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.86.2/meta/demos/demo_best_model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.86.2/meta/demos/my_experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.86.2/meta/demos/my_experiment_local.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.86.2/meta/demos/plot_faster_anim.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.841798 nkululeko-0.86.2/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.86.2/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.86.2/nkululeko/aug_train.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.86.2/nkululeko/augment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.841798 nkululeko-0.86.2/nkululeko/augmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.86.2/nkululeko/augmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.86.2/nkululeko/augmenting/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.86.2/nkululeko/augmenting/randomsplicer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.86.2/nkululeko/augmenting/randomsplicing.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3542 2024-05-13 11:40:51.000000 nkululeko-0.86.2/nkululeko/augmenting/resampler.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.845799 nkululeko-0.86.2/nkululeko/autopredict/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.86.2/nkululeko/autopredict/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.86.2/nkululeko/autopredict/ap_age.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.86.2/nkululeko/autopredict/ap_arousal.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.86.2/nkululeko/autopredict/ap_dominance.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.86.2/nkululeko/autopredict/ap_gender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.86.2/nkululeko/autopredict/ap_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.86.2/nkululeko/autopredict/ap_pesq.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.86.2/nkululeko/autopredict/ap_sdr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.86.2/nkululeko/autopredict/ap_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.86.2/nkululeko/autopredict/ap_stoi.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.86.2/nkululeko/autopredict/ap_valence.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5048 2024-04-22 09:09:10.000000 nkululeko-0.86.2/nkululeko/autopredict/estimate_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.86.2/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-05-30 09:48:23.000000 nkululeko-0.86.2/nkululeko/constants.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.845799 nkululeko-0.86.2/nkululeko/data/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.86.2/nkululeko/data/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27650 2024-04-22 09:10:47.000000 nkululeko-0.86.2/nkululeko/data/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3933 2024-05-21 10:44:53.000000 nkululeko-0.86.2/nkululeko/data/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3232 2024-05-03 09:55:35.000000 nkululeko-0.86.2/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.86.2/nkululeko/demo_feats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4757 2024-05-03 09:56:14.000000 nkululeko-0.86.2/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    30986 2024-05-29 14:39:21.000000 nkululeko-0.86.2/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2609 2024-04-30 15:24:17.000000 nkululeko-0.86.2/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.86.2/nkululeko/export.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.845799 nkululeko-0.86.2/nkululeko/feat_extract/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.86.2/nkululeko/feat_extract/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3113 2024-04-23 09:16:18.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3424 2024-04-29 13:37:24.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_agender_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12722 2024-05-03 14:41:56.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3162 2024-04-23 09:16:18.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_auddim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3187 2024-04-23 09:16:18.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3489 2024-04-23 09:16:18.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5196 2024-04-24 17:12:28.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_hubert.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1622 2024-04-23 09:55:16.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4174 2024-04-23 10:17:00.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4028 2024-05-29 07:55:31.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4980 2024-04-23 09:16:18.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3105 2024-04-23 09:16:18.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3670 2024-04-23 09:59:48.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_spectra.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_spkrec.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4617 2024-04-29 13:37:24.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_squim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3228 2024-04-30 09:31:46.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5268 2024-04-29 13:37:24.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4703 2024-04-24 17:06:22.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_wavlm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4533 2024-05-15 15:09:05.000000 nkululeko-0.86.2/nkululeko/feat_extract/feats_whisper.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1541 2024-05-29 07:58:33.000000 nkululeko-0.86.2/nkululeko/feat_extract/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.86.2/nkululeko/feat_extract/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3976 2024-04-23 11:13:33.000000 nkululeko-0.86.2/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.86.2/nkululeko/file_checker.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.86.2/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      525 2024-05-03 12:01:14.000000 nkululeko-0.86.2/nkululeko/glob_conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.845799 nkululeko-0.86.2/nkululeko/losses/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.86.2/nkululeko/losses/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.86.2/nkululeko/losses/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.86.2/nkululeko/losses/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10452 2024-05-17 12:04:16.000000 nkululeko-0.86.2/nkululeko/modelrunner.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.845799 nkululeko-0.86.2/nkululeko/models/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.86.2/nkululeko/models/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11639 2024-05-15 15:09:05.000000 nkululeko-0.86.2/nkululeko/models/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2024-05-03 14:26:57.000000 nkululeko-0.86.2/nkululeko/models/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9954 2024-05-03 14:27:45.000000 nkululeko-0.86.2/nkululeko/models/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      649 2024-05-03 14:28:01.000000 nkululeko-0.86.2/nkululeko/models/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      599 2024-05-03 14:28:22.000000 nkululeko-0.86.2/nkululeko/models/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      610 2024-05-03 14:28:14.000000 nkululeko-0.86.2/nkululeko/models/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      422 2024-05-03 14:28:34.000000 nkululeko-0.86.2/nkululeko/models/model_lin_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9856 2024-05-29 14:36:50.000000 nkululeko-0.86.2/nkululeko/models/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10204 2024-05-03 14:28:58.000000 nkululeko-0.86.2/nkululeko/models/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      940 2024-05-03 14:29:24.000000 nkululeko-0.86.2/nkululeko/models/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      725 2024-05-03 14:29:39.000000 nkululeko-0.86.2/nkululeko/models/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      417 2024-05-03 14:30:08.000000 nkululeko-0.86.2/nkululeko/models/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      428 2024-05-03 14:29:56.000000 nkululeko-0.86.2/nkululeko/models/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20777 2024-05-30 09:44:23.000000 nkululeko-0.86.2/nkululeko/models/model_tuned.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      447 2024-05-03 14:33:39.000000 nkululeko-0.86.2/nkululeko/models/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      418 2024-05-03 14:34:29.000000 nkululeko-0.86.2/nkululeko/models/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5634 2024-04-23 14:42:13.000000 nkululeko-0.86.2/nkululeko/multidb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3725 2024-04-26 06:05:26.000000 nkululeko-0.86.2/nkululeko/nkuluflag.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1968 2024-04-23 12:35:01.000000 nkululeko-0.86.2/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23070 2024-05-30 08:12:44.000000 nkululeko-0.86.2/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2409 2024-04-22 09:09:10.000000 nkululeko-0.86.2/nkululeko/predict.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.845799 nkululeko-0.86.2/nkululeko/reporting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.86.2/nkululeko/reporting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.86.2/nkululeko/reporting/defines.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.86.2/nkululeko/reporting/latex_writer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.86.2/nkululeko/reporting/report.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.86.2/nkululeko/reporting/report_item.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13445 2024-05-30 09:47:17.000000 nkululeko-0.86.2/nkululeko/reporting/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.86.2/nkululeko/reporting/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4267 2024-05-29 12:54:47.000000 nkululeko-0.86.2/nkululeko/resample.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7624 2024-04-22 09:09:10.000000 nkululeko-0.86.2/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.86.2/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.86.2/nkululeko/segment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.845799 nkululeko-0.86.2/nkululeko/segmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.86.2/nkululeko/segmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.86.2/nkululeko/segmenting/seg_inaspeechsegmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.86.2/nkululeko/segmenting/seg_silero.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.86.2/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1677 2024-04-26 06:04:30.000000 nkululeko-0.86.2/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3237 2024-04-25 14:01:11.000000 nkululeko-0.86.2/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8465 2024-05-15 15:09:05.000000 nkululeko-0.86.2/nkululeko/test_pretrain.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.845799 nkululeko-0.86.2/nkululeko/utils/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.86.2/nkululeko/utils/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.86.2/nkululeko/utils/files.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.86.2/nkululeko/utils/stats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13946 2024-05-29 12:54:47.000000 nkululeko-0.86.2/nkululeko/utils/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.845799 nkululeko-0.86.2/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    37170 2024-05-30 09:48:37.000000 nkululeko-0.86.2/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5132 2024-05-30 09:48:37.000000 nkululeko-0.86.2/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-05-30 09:48:37.000000 nkululeko-0.86.2/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-05-30 09:48:37.000000 nkululeko-0.86.2/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-05-30 09:48:37.000000 nkululeko-0.86.2/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.86.2/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-05-30 09:48:37.849799 nkululeko-0.86.2/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.86.2/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.837798 nkululeko-0.86.2/venv/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-30 09:48:37.845799 nkululeko-0.86.2/venv/bin/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.86.2/venv/bin/activate_this.py
```

### Comparing `nkululeko-0.86.1/CHANGELOG.md` & `nkululeko-0.86.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+Version 0.86.2
+--------------
+* plots epoch progression for finetuned models now
+
 Version 0.86.1
 --------------
 * functionality to push to hub
 * fixed bug that prevented wavlm finetuning
 
 Version 0.86.0
 --------------
```

### Comparing `nkululeko-0.86.1/LICENSE` & `nkululeko-0.86.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/PKG-INFO` & `nkululeko-0.86.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.86.1
+Version: 0.86.2
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -330,14 +330,18 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.86.2
+--------------
+* plots epoch progression for finetuned models now
+
 Version 0.86.1
 --------------
 * functionality to push to hub
 * fixed bug that prevented wavlm finetuning
 
 Version 0.86.0
 --------------
```

### Comparing `nkululeko-0.86.1/README.md` & `nkululeko-0.86.2/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/aesdd/process_database.py` & `nkululeko-0.86.2/data/aesdd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/androids/process_database.py` & `nkululeko-0.86.2/data/androids/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/androids_orig/process_database.py` & `nkululeko-0.86.2/data/androids_orig/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/androids_test/process_database.py` & `nkululeko-0.86.2/data/androids_test/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/ased/process_database.py` & `nkululeko-0.86.2/data/ased/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/asvp-esd/process_database.py` & `nkululeko-0.86.2/data/asvp-esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/baved/process_database.py` & `nkululeko-0.86.2/data/baved/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/cafe/process_database.py` & `nkululeko-0.86.2/data/cafe/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/clac/process_database.py` & `nkululeko-0.86.2/data/clac/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/cmu-mosei/process_database.py` & `nkululeko-0.86.2/data/cmu-mosei/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/demos/process_database.py` & `nkululeko-0.86.2/data/demos/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/ekorpus/process_database.py` & `nkululeko-0.86.2/data/ekorpus/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/emns/process_database.py` & `nkululeko-0.86.2/data/emns/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/emofilm/convert_to_16k.py` & `nkululeko-0.86.2/data/emofilm/convert_to_16k.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/emofilm/process_database.py` & `nkululeko-0.86.2/data/emofilm/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/emorynlp/process_database.py` & `nkululeko-0.86.2/data/emorynlp/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/emov-db/process_database.py` & `nkululeko-0.86.2/data/emov-db/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/emovo/process_database.py` & `nkululeko-0.86.2/data/emovo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/emozionalmente/create.py` & `nkululeko-0.86.2/data/emozionalmente/create.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/enterface/process_database.py` & `nkululeko-0.86.2/data/enterface/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/esd/process_database.py` & `nkululeko-0.86.2/data/esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/gerparas/process_database.py` & `nkululeko-0.86.2/data/gerparas/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/iemocap/process_database.py` & `nkululeko-0.86.2/data/iemocap/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/jl/process_database.py` & `nkululeko-0.86.2/data/jl/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/jtes/process_database.py` & `nkululeko-0.86.2/data/jtes/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/meld/process_database.py` & `nkululeko-0.86.2/data/meld/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/mesd/process_database.py` & `nkululeko-0.86.2/data/mesd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/mess/process_database.py` & `nkululeko-0.86.2/data/mess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/mlendsnd/process_database.py` & `nkululeko-0.86.2/data/mlendsnd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/msp-improv/process_database2.py` & `nkululeko-0.86.2/data/msp-improv/process_database2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/msp-podcast/process_database.py` & `nkululeko-0.86.2/data/msp-podcast/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/oreau2/process_database.py` & `nkululeko-0.86.2/data/oreau2/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/portuguese/process_database.py` & `nkululeko-0.86.2/data/portuguese/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/ravdess/process_database.py` & `nkululeko-0.86.2/data/ravdess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/ravdess/process_database_speaker.py` & `nkululeko-0.86.2/data/ravdess/process_database_speaker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/savee/process_database.py` & `nkululeko-0.86.2/data/savee/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/shemo/process_database.py` & `nkululeko-0.86.2/data/shemo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/subesco/process_database.py` & `nkululeko-0.86.2/data/subesco/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/tess/process_database.py` & `nkululeko-0.86.2/data/tess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/thorsten-emotional/process_database.py` & `nkululeko-0.86.2/data/thorsten-emotional/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/urdu/process_database.py` & `nkululeko-0.86.2/data/urdu/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/data/vivae/process_database.py` & `nkululeko-0.86.2/data/vivae/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/docs/source/conf.py` & `nkululeko-0.86.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/meta/demos/demo_best_model.py` & `nkululeko-0.86.2/meta/demos/demo_best_model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/meta/demos/my_experiment.py` & `nkululeko-0.86.2/meta/demos/my_experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/meta/demos/my_experiment_local.py` & `nkululeko-0.86.2/meta/demos/my_experiment_local.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/meta/demos/plot_faster_anim.py` & `nkululeko-0.86.2/meta/demos/plot_faster_anim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/aug_train.py` & `nkululeko-0.86.2/nkululeko/aug_train.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/augment.py` & `nkululeko-0.86.2/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/augmenting/augmenter.py` & `nkululeko-0.86.2/nkululeko/augmenting/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/augmenting/randomsplicer.py` & `nkululeko-0.86.2/nkululeko/augmenting/randomsplicer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/augmenting/randomsplicing.py` & `nkululeko-0.86.2/nkululeko/augmenting/randomsplicing.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/augmenting/resampler.py` & `nkululeko-0.86.2/nkululeko/augmenting/resampler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/autopredict/ap_age.py` & `nkululeko-0.86.2/nkululeko/autopredict/ap_age.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/autopredict/ap_arousal.py` & `nkululeko-0.86.2/nkululeko/autopredict/ap_arousal.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/autopredict/ap_dominance.py` & `nkululeko-0.86.2/nkululeko/autopredict/ap_dominance.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/autopredict/ap_gender.py` & `nkululeko-0.86.2/nkululeko/autopredict/ap_gender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/autopredict/ap_mos.py` & `nkululeko-0.86.2/nkululeko/autopredict/ap_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/autopredict/ap_pesq.py` & `nkululeko-0.86.2/nkululeko/autopredict/ap_pesq.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/autopredict/ap_sdr.py` & `nkululeko-0.86.2/nkululeko/autopredict/ap_sdr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/autopredict/ap_snr.py` & `nkululeko-0.86.2/nkululeko/autopredict/ap_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/autopredict/ap_stoi.py` & `nkululeko-0.86.2/nkululeko/autopredict/ap_stoi.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/autopredict/ap_valence.py` & `nkululeko-0.86.2/nkululeko/autopredict/ap_valence.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/autopredict/estimate_snr.py` & `nkululeko-0.86.2/nkululeko/autopredict/estimate_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/cacheddataset.py` & `nkululeko-0.86.2/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/data/dataset.py` & `nkululeko-0.86.2/nkululeko/data/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/data/dataset_csv.py` & `nkululeko-0.86.2/nkululeko/data/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/demo.py` & `nkululeko-0.86.2/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/demo_feats.py` & `nkululeko-0.86.2/nkululeko/demo_feats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/demo_predictor.py` & `nkululeko-0.86.2/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/experiment.py` & `nkululeko-0.86.2/nkululeko/experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/explore.py` & `nkululeko-0.86.2/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/export.py` & `nkululeko-0.86.2/nkululeko/export.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_agender.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_agender_agender.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_agender_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_analyser.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_auddim.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_auddim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_audmodel.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_clap.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_hubert.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_hubert.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_import.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_mld.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_mos.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_opensmile.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_oxbow.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_praat.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_snr.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_spectra.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_spectra.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_spkrec.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_spkrec.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_squim.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_squim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_trill.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_wav2vec2.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_wavlm.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_wavlm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feats_whisper.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feats_whisper.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/featureset.py` & `nkululeko-0.86.2/nkululeko/feat_extract/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feat_extract/feinberg_praat.py` & `nkululeko-0.86.2/nkululeko/feat_extract/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/feature_extractor.py` & `nkululeko-0.86.2/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/file_checker.py` & `nkululeko-0.86.2/nkululeko/file_checker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/filter_data.py` & `nkululeko-0.86.2/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/glob_conf.py` & `nkululeko-0.86.2/nkululeko/glob_conf.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/losses/loss_ccc.py` & `nkululeko-0.86.2/nkululeko/losses/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/losses/loss_softf1loss.py` & `nkululeko-0.86.2/nkululeko/losses/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/modelrunner.py` & `nkululeko-0.86.2/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/models/model.py` & `nkululeko-0.86.2/nkululeko/models/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/models/model_cnn.py` & `nkululeko-0.86.2/nkululeko/models/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/models/model_gmm.py` & `nkululeko-0.86.2/nkululeko/models/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/models/model_knn.py` & `nkululeko-0.86.2/nkululeko/models/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/models/model_knn_reg.py` & `nkululeko-0.86.2/nkululeko/models/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/models/model_mlp.py` & `nkululeko-0.86.2/nkululeko/models/model_mlp.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 import numpy as np
 from sklearn.metrics import recall_score
 from collections import OrderedDict
 from nkululeko.losses.loss_softf1loss import SoftF1Loss
 
 
 class MLP_model(Model):
-    """MLP = multi layer perceptron"""
+    """MLP = multi layer perceptron."""
 
     is_classifier = True
 
     def __init__(self, df_train, df_test, feats_train, feats_test):
-        """Constructor taking the configuration and all dataframes"""
+        """Constructor taking the configuration and all dataframes."""
         super().__init__(df_train, df_test, feats_train, feats_test)
         super().set_model_type("ann")
         self.name = "mlp"
         self.target = glob_conf.config["DATA"]["target"]
         labels = glob_conf.labels
         self.class_num = len(labels)
         # set up loss criterion
```

### Comparing `nkululeko-0.86.1/nkululeko/models/model_mlp_regression.py` & `nkululeko-0.86.2/nkululeko/models/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/models/model_svm.py` & `nkululeko-0.86.2/nkululeko/models/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/models/model_svr.py` & `nkululeko-0.86.2/nkululeko/models/model_svr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/models/model_tuned.py` & `nkululeko-0.86.2/nkululeko/models/model_tuned.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Code based on @jwagner."""
 
+import ast
 import dataclasses
 import json
 import os
 import pickle
 import typing
 
 import datasets
@@ -47,32 +48,32 @@
             self.measure = "uar"
         else:
             self.measure = self.util.config_val("MODEL", "measure", "ccc")
         self.util.debug(f"evaluation metrics: {self.measure}")
         self.batch_size = int(self.util.config_val("MODEL", "batch_size", "8"))
         self.util.debug(f"batch size: {self.batch_size}")
         self.learning_rate = float(
-            self.util.config_val("MODEL", "learning_rate", 0.0001)
+            self.util.config_val("MODEL", "learning_rate", "0.0001")
         )
+        self.max_duration = float(self.util.config_val("MODEL", "max_duration", "8.0"))
         self.df_train, self.df_test = df_train, df_test
         self.epoch_num = int(self.util.config_val("EXP", "epochs", 1))
         drop = self.util.config_val("MODEL", "drop", False)
         self.drop = 0.1
         if drop:
             self.drop = float(drop)
         self.util.debug(f"init: training with dropout: {self.drop}")
         self._init_model()
 
     def _init_model(self):
         model_path = "facebook/wav2vec2-large-robust-ft-swbd-300h"
-        pretrained_model = self.util.config_val(
-            "MODEL", "pretrained_model", model_path)
+        pretrained_model = self.util.config_val("MODEL", "pretrained_model", model_path)
         self.num_layers = None
         self.sampling_rate = 16000
-        self.max_duration_sec = 8.0
+        self.max_duration_sec = self.max_duration
         self.accumulation_steps = 4
 
         # print finetuning information via debug
         self.util.debug(f"Finetuning from model: {pretrained_model}")
 
         # create dataset
         dataset = {}
@@ -231,37 +232,52 @@
                 scores[f"{name}"] = metric(truth, preds)
 
         return scores
 
     def train(self):
         """Train the model."""
         model_root = self.util.get_path("model_dir")
-        log_root = os.path.join(self.util.get_exp_dir(), "log")
-        audeer.mkdir(log_root)
+        self.log_root = os.path.join(self.util.get_exp_dir(), "log")
+        audeer.mkdir(self.log_root)
         self.torch_root = audeer.path(model_root, "torch")
         conf_file = os.path.join(self.torch_root, "config.json")
         if os.path.isfile(conf_file):
             self.util.debug(f"reusing finetuned model: {conf_file}")
             self.load(self.run, self.epoch_num)
             return
         targets = pd.DataFrame(self.dataset["train"]["targets"])
-        counts = targets[0].value_counts().sort_index()
 
         if self.is_classifier:
-            train_weights = 1 / counts
-            train_weights /= train_weights.sum()
-            self.util.debug(f"train weights: {train_weights}")
-            criterion = torch.nn.CrossEntropyLoss(
-                weight=torch.Tensor(train_weights).to("cuda"),
-            )
+            criterion = self.util.config_val("MODEL", "loss", "cross")
+            if criterion == "cross":
+                if self.util.config_val("MODEL", "class_weight", False):
+                    counts = targets[0].value_counts().sort_index()
+                    train_weights = 1 / counts
+                    train_weights /= train_weights.sum()
+                    self.util.debug(f"train weights: {train_weights}")
+                    criterion = torch.nn.CrossEntropyLoss(
+                        weight=torch.Tensor(train_weights).to("cuda"),
+                    )
+                else:
+                    criterion = torch.nn.CrossEntropyLoss()
+            else:
+                self.util.error(f"criterion {criterion} not supported for classifier")
         else:
-            criterion = ConcordanceCorCoeff()
+            self.criterion = self.util.config_val("MODEL", "loss", "ccc")
+            if criterion == "1-ccc":
+                criterion = ConcordanceCorCoeff()
+            elif criterion == "mse":
+                criterion = torch.nn.MSELoss()
+            elif criterion == "mae":
+                criterion = torch.nn.L1Loss()
+            else:
+                self.util.error(f"criterion {criterion} not supported for regressor")
 
         # set push_to_hub value, default false
-        push = self.util.config_val("MODEL", "push_to_hub", False)
+        push = eval(self.util.config_val("MODEL", "push_to_hub", "False"))
 
         class Trainer(transformers.Trainer):
             def compute_loss(
                 self,
                 model,
                 inputs,
                 return_outputs=False,
@@ -280,32 +296,42 @@
             len(self.dataset["train"])
             // (self.batch_size * self.accumulation_steps)
             // 5
         )
         num_steps = max(1, num_steps)
 
         metrics_for_best_model = self.measure.upper()
+        if metrics_for_best_model == "UAR":
+            greater_is_better = True
+        elif metrics_for_best_model == "CCC":
+            greater_is_better = True
+        elif metrics_for_best_model == "MSE":
+            greater_is_better = False
+        elif metrics_for_best_model == "MAE":
+            greater_is_better = False
+        else:
+            self.util.error(f"unknown metric/measure: {metrics_for_best_model}")
 
         training_args = transformers.TrainingArguments(
             output_dir=model_root,
-            logging_dir=log_root,
+            logging_dir=self.log_root,
             per_device_train_batch_size=self.batch_size,
             per_device_eval_batch_size=self.batch_size,
             gradient_accumulation_steps=self.accumulation_steps,
             evaluation_strategy="steps",
             num_train_epochs=self.epoch_num,
             fp16=self.device == "cuda",
             save_steps=num_steps,
             eval_steps=num_steps,
             logging_steps=num_steps,
             logging_strategy="epoch",
             learning_rate=self.learning_rate,
             save_total_limit=2,
             metric_for_best_model=metrics_for_best_model,
-            greater_is_better=True,
+            greater_is_better=greater_is_better,
             load_best_model_at_end=True,
             remove_unused_columns=False,
             report_to="none",
             push_to_hub=push,
             hub_model_id=f"{self.util.get_name()}",
         )
 
@@ -315,16 +341,23 @@
             args=training_args,
             compute_metrics=self.compute_metrics,
             train_dataset=self.dataset["train"],
             eval_dataset=self.dataset["dev"],
             tokenizer=self.processor.feature_extractor,
             callbacks=[transformers.integrations.TensorBoardCallback()],
         )
+
         trainer.train()
         trainer.save_model(self.torch_root)
+        log_file = os.path.join(
+            self.log_root,
+            "log.txt",
+        )
+        with open(log_file, "w") as text_file:
+            print(trainer.state.log_history, file=text_file)
         self.util.debug(f"saved best model to {self.torch_root}")
         self.load(self.run, self.epoch)
 
     def get_predictions(self):
         results = []
         for (file, start, end), _ in audeer.progress_bar(
             self.df_test.iterrows(),
@@ -347,16 +380,38 @@
         predictions = self.get_predictions()
         report = Reporter(
             self.df_test[self.target].to_numpy().astype(float),
             predictions,
             self.run,
             self.epoch_num,
         )
+        self._plot_epoch_progression(report)
         return report
 
+    def _plot_epoch_progression(self, report):
+        log_file = os.path.join(
+            self.log_root,
+            "log.txt",
+        )
+        with open(log_file, "r") as file:
+            data = file.read()
+        list = ast.literal_eval(data)
+        epochs, vals, loss = [], [], []
+        for index, tp in enumerate(list):
+            try:
+                epochs.append(tp["epoch"])
+                measure = self.measure.upper()
+                vals.append(tp[f"eval_{measure}"])
+                loss.append(tp["eval_loss"])
+            except KeyError:
+                del epochs[-1]
+                # print(f'no value at {index}')
+        df = pd.DataFrame({"results": vals, "losses": loss}, index=epochs)
+        report.plot_epoch_progression_finetuned(df)
+
     def predict_sample(self, signal):
         """Predict one sample"""
         prediction = {}
         if self.is_classifier:
             # get the class probabilities
             predictions = self.model.predict(signal)
             # pred = self.clf.predict(features)
```

### Comparing `nkululeko-0.86.1/nkululeko/multidb.py` & `nkululeko-0.86.2/nkululeko/multidb.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/nkuluflag.py` & `nkululeko-0.86.2/nkululeko/nkuluflag.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/nkululeko.py` & `nkululeko-0.86.2/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/plots.py` & `nkululeko-0.86.2/nkululeko/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # plots.py
-import pandas as pd
+import ast
+
 import matplotlib.pyplot as plt
-from sklearn.manifold import TSNE
-import seaborn as sns
 import numpy as np
-import ast
+import pandas as pd
 from scipy import stats
-from nkululeko.utils.util import Util
-import nkululeko.utils.stats as su
+import seaborn as sns
+from sklearn.manifold import TSNE
+
 import nkululeko.glob_conf as glob_conf
-from nkululeko.reporting.report_item import ReportItem
 from nkululeko.reporting.defines import Header
+from nkululeko.reporting.report_item import ReportItem
+import nkululeko.utils.stats as su
+from nkululeko.utils.util import Util
 
 
 class Plots:
     def __init__(self):
-        """Initializing the util system"""
+        """Initializing the util system."""
         self.util = Util("plots")
         self.format = self.util.config_val("PLOT", "format", "png")
         self.target = self.util.config_val("DATA", "target", "emotion")
 
     def plot_distributions_speaker(self, df):
         df_speakers = pd.DataFrame()
         pd.options.mode.chained_assignment = None  # default='warn'
@@ -134,46 +136,43 @@
                         )
                 else:
                     if self.util.is_categorical(df[att1]):
                         ax, caption = self._plotcatcont(
                             df, att1, class_label, att1, type_s
                         )
                     else:
-                        ax, caption = self._plot2cont(
-                            df, class_label, att1, type_s)
+                        ax, caption = self._plot2cont(df, class_label, att1, type_s)
                 self._save_plot(
                     ax,
                     caption,
                     f"Correlation of {self.target} and {att[0]}",
                     filename,
                     type_s,
                 )
                 # fig.clear()           # avoid error
             elif len(att) == 2:
                 att1 = att[0]
                 att2 = att[1]
                 if att1 == self.target or att2 == self.target:
-                    self.util.debug(
-                        f"no need to correlate {self.target} with itself")
+                    self.util.debug(f"no need to correlate {self.target} with itself")
                     return
                 if att1 not in df:
                     self.util.error(f"unknown feature: {att1}")
                 if att2 not in df:
                     self.util.error(f"unknown feature: {att2}")
                 att1, df = self._check_binning(att1, df)
                 att2, df = self._check_binning(att2, df)
                 self.util.debug(f"plotting {att}")
                 filename = f"{att1}-{att2}"
                 filename = f"{self.target}-{filename}"
                 if self.util.is_categorical(df["class_label"]):
                     if self.util.is_categorical(df[att1]):
                         if self.util.is_categorical(df[att2]):
                             # class_label = cat, att1 = cat, att2 = cat
-                            ax, caption = self._plot2cat(
-                                df, att1, att2, att1, type_s)
+                            ax, caption = self._plot2cat(df, att1, att2, att1, type_s)
                         else:
                             # class_label = cat, att1 = cat, att2 = cont
                             ax, caption = self._plotcatcont(
                                 df, att1, att2, att1, type_s
                             )
                     else:
                         if self.util.is_categorical(df[att2]):
@@ -186,31 +185,29 @@
                             ax, caption = self._plot2cont_cat(
                                 df, att1, att2, "class_label", type_s
                             )
                 else:  # class_label is continuous
                     if self.util.is_categorical(df[att1]):
                         if self.util.is_categorical(df[att2]):
                             # class_label = cont, att1 = cat, att2 = cat
-                            ax, caption = self._plot2cat(
-                                df, att1, att2, att1, type_s)
+                            ax, caption = self._plot2cat(df, att1, att2, att1, type_s)
                         else:
                             # class_label = cont, att1 = cat, att2 = cont
                             ax, caption = self._plot2cont_cat(
                                 df, att2, "class_label", att1, type_s
                             )
                     else:
                         if self.util.is_categorical(df[att2]):
                             # class_label = cont, att1 = cont, att2 = cat
                             ax, caption = self._plot2cont_cat(
                                 df, att1, "class_label", att2, type_s
                             )
                         else:
                             # class_label = cont, att1 = cont, att2 = cont
-                            ax, caption = self._plot2cont(
-                                df, att1, att2, type_s)
+                            ax, caption = self._plot2cont(df, att1, att2, type_s)
 
                 self._save_plot(
                     ax, caption, f"Correlation of {att1} and {att2}", filename, type_s
                 )
 
             else:
                 self.util.error(
@@ -234,16 +231,15 @@
                 header,
                 caption,
                 img_path,
             )
         )
 
     def _check_binning(self, att, df):
-        bin_reals_att = eval(self.util.config_val(
-            "EXPL", f"{att}.bin_reals", "False"))
+        bin_reals_att = eval(self.util.config_val("EXPL", f"{att}.bin_reals", "False"))
         if bin_reals_att:
             self.util.debug(f"binning continuous variable {att} to categories")
             att_new = f"{att}_binned"
             df[att_new] = self.util.continuous_to_categorical(df[att]).values
             att = att_new
         return att, df
 
@@ -338,16 +334,15 @@
                 title,
                 img_path,
             )
         )
 
     def describe_df(self, name, df, target, filename):
         """Make a stacked barplot of samples and speakers per sex and target values. speaker, gender and target columns must be present"""
-        fig_dir = self.util.get_path(
-            "fig_dir") + "../"  # one up because of the runs
+        fig_dir = self.util.get_path("fig_dir") + "../"  # one up because of the runs
         sampl_num = df.shape[0]
         sex_col = "gender"
         if target == "gender":
             sex_col = "class_label"
         if self.util.exp_is_classification() and target != "gender":
             target = "class_label"
         if df.is_labeled:
@@ -388,16 +383,15 @@
                 )
             )
 
     def scatter_plot(self, feats, label_df, label, dimred_type):
         dim_num = int(self.util.config_val("EXPL", "scatter.dim", 2))
         # one up because of the runs
         fig_dir = self.util.get_path("fig_dir") + "../"
-        sample_selection = self.util.config_val(
-            "EXPL", "sample_selection", "all")
+        sample_selection = self.util.config_val("EXPL", "sample_selection", "all")
         filename = f"{label}_{self.util.get_feattype_name()}_{sample_selection}_{dimred_type}_{str(dim_num)}d"
         filename = f"{fig_dir}{filename}.{self.format}"
         self.util.debug(f"computing {dimred_type}, this might take a while...")
         data = None
         labels = label_df[label]
         if dimred_type == "tsne":
             data = self.getTsne(feats, dim_num)
@@ -431,16 +425,15 @@
                 y,
                 feats.index,
                 columns=columns,
             )
 
         if dim_num == 2:
             plot_data = np.vstack((data.T, labels)).T
-            plot_df = pd.DataFrame(
-                data=plot_data, columns=("Dim_1", "Dim_2", "label"))
+            plot_df = pd.DataFrame(data=plot_data, columns=("Dim_1", "Dim_2", "label"))
             # plt.tight_layout()
             ax = (
                 sns.FacetGrid(plot_df, hue="label", height=6)
                 .map(plt.scatter, "Dim_1", "Dim_2")
                 .add_legend()
             )
         elif dim_num == 3:
```

### Comparing `nkululeko-0.86.1/nkululeko/predict.py` & `nkululeko-0.86.2/nkululeko/predict.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/reporting/defines.py` & `nkululeko-0.86.2/nkululeko/reporting/defines.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/reporting/latex_writer.py` & `nkululeko-0.86.2/nkululeko/reporting/latex_writer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/reporting/report.py` & `nkululeko-0.86.2/nkululeko/reporting/report.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/reporting/report_item.py` & `nkululeko-0.86.2/nkululeko/reporting/report_item.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/reporting/reporter.py` & `nkululeko-0.86.2/nkululeko/reporting/reporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,14 +296,31 @@
             imageio.mimsave(fig_dir + out_name, images, fps=int(fps))
         except RuntimeError as e:
             self.util.error("error writing anim gif: " + e)
 
     def get_result(self):
         return self.result
 
+    def plot_epoch_progression_finetuned(self, df):
+        plot_name_suggest = self.util.get_exp_name()
+        fig_dir = self.util.get_path("fig_dir")
+        plot_name = (
+            self.util.config_val("PLOT", "name", plot_name_suggest)
+            + "_epoch_progression"
+        )
+        ax = df.plot()
+        fig = ax.figure
+        plt.xlabel("epochs")
+        plt.ylabel(f"{self.MEASURE}")
+        plot_path = f"{fig_dir}{plot_name}.{self.format}"
+        plt.savefig(plot_path)
+        self.util.debug(f"plotted epoch progression to {plot_path}")
+        plt.close(fig)
+        fig.clear()
+
     def plot_epoch_progression(self, reports, out_name):
         fig_dir = self.util.get_path("fig_dir")
         results, losses, train_results, losses_eval = [], [], [], []
         for r in reports:
             results.append(r.get_result().test)
             losses.append(r.get_result().loss)
             train_results.append(r.get_result().train)
```

### Comparing `nkululeko-0.86.1/nkululeko/reporting/result.py` & `nkululeko-0.86.2/nkululeko/reporting/result.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/resample.py` & `nkululeko-0.86.2/nkululeko/resample.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/runmanager.py` & `nkululeko-0.86.2/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/scaler.py` & `nkululeko-0.86.2/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/segment.py` & `nkululeko-0.86.2/nkululeko/segment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/segmenting/seg_inaspeechsegmenter.py` & `nkululeko-0.86.2/nkululeko/segmenting/seg_inaspeechsegmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/segmenting/seg_silero.py` & `nkululeko-0.86.2/nkululeko/segmenting/seg_silero.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/syllable_nuclei.py` & `nkululeko-0.86.2/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/test.py` & `nkululeko-0.86.2/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/test_predictor.py` & `nkululeko-0.86.2/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/test_pretrain.py` & `nkululeko-0.86.2/nkululeko/test_pretrain.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/utils/files.py` & `nkululeko-0.86.2/nkululeko/utils/files.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/utils/stats.py` & `nkululeko-0.86.2/nkululeko/utils/stats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko/utils/util.py` & `nkululeko-0.86.2/nkululeko/utils/util.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.86.2/nkululeko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.86.1
+Version: 0.86.2
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -330,14 +330,18 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.86.2
+--------------
+* plots epoch progression for finetuned models now
+
 Version 0.86.1
 --------------
 * functionality to push to hub
 * fixed bug that prevented wavlm finetuning
 
 Version 0.86.0
 --------------
```

### Comparing `nkululeko-0.86.1/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.86.2/nkululeko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/setup.cfg` & `nkululeko-0.86.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `nkululeko-0.86.1/venv/bin/activate_this.py` & `nkululeko-0.86.2/venv/bin/activate_this.py`

 * *Files identical despite different names*

