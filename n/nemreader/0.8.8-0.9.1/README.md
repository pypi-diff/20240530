# Comparing `tmp/nemreader-0.8.8.tar.gz` & `tmp/nemreader-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemreader-0.8.8.tar", last modified: Thu Dec 14 09:48:56 2023, max compression
+gzip compressed data, was "nemreader-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nemreader-0.8.8.tar` & `nemreader-0.9.1.tar`

### file list

```diff
@@ -1,227 +1,227 @@
--rwxr-xr-x   0        0        0      135 2023-12-14 09:25:35.425049 nemreader-0.8.8/.flake8
--rw-r--r--   0        0        0      985 2023-12-14 09:25:35.425049 nemreader-0.8.8/.github/workflows/publish.yml
--rwxr-xr-x   0        0        0     1212 2023-12-14 09:25:35.425049 nemreader-0.8.8/.github/workflows/pythonpackage.yml
--rw-r--r--   0        0        0     1185 2023-12-14 09:25:35.425049 nemreader-0.8.8/.gitignore
--rw-r--r--   0        0        0     1074 2021-10-10 05:55:38.462694 nemreader-0.8.8/LICENSE
--rw-r--r--   0        0        0       26 2021-10-10 05:55:38.462694 nemreader-0.8.8/MANIFEST.in
--rw-r--r--   0        0        0     1164 2023-12-14 09:25:35.425049 nemreader-0.8.8/README.md
--rw-r--r--   0        0        0   101291 2021-10-10 05:55:38.462694 nemreader-0.8.8/docs/_static/img/nmi-suffixes.jpg
--rw-r--r--   0        0        0    38420 2021-10-10 05:55:38.466693 nemreader-0.8.8/docs/_static/img/nmi-suffixes2.png
--rw-r--r--   0        0        0    10717 2021-10-10 05:55:38.466693 nemreader-0.8.8/docs/_static/img/plot_cal.png
--rw-r--r--   0        0        0    14205 2021-10-10 05:55:38.466693 nemreader-0.8.8/docs/_static/img/plot_profile.png
--rwxr-xr-x   0        0        0     5363 2023-12-14 09:25:35.425049 nemreader-0.8.8/docs/file-format.md
--rwxr-xr-x   0        0        0      658 2023-12-14 09:25:35.425049 nemreader-0.8.8/docs/gen_ref_pages.py
--rwxr-xr-x   0        0        0      469 2023-12-14 09:25:35.425049 nemreader-0.8.8/docs/index.md
--rwxr-xr-x   0        0        0      164 2023-12-14 09:25:35.425049 nemreader-0.8.8/docs/installation.md
--rwxr-xr-x   0        0        0     5158 2023-12-14 09:30:31.899464 nemreader-0.8.8/docs/quickstart.md
--rw-r--r--   0        0        0       60 2023-12-14 09:25:35.425049 nemreader-0.8.8/docs/requirements.txt
--rw-r--r--   0        0        0    29436 2023-12-14 09:25:35.425049 nemreader-0.8.8/examples/Example_NEM12_ManyNMIs.zip
--rw-r--r--   0        0        0      708 2023-12-14 09:25:35.425049 nemreader-0.8.8/examples/Example_different_intervals.zip
--rw-r--r--   0        0        0      288 2023-12-14 09:25:35.425049 nemreader-0.8.8/examples/invalid/Example_NEM12_15min_200_30min_300.csv
--rw-r--r--   0        0        0      480 2023-12-14 09:25:35.425049 nemreader-0.8.8/examples/invalid/Example_NEM12_15min_200_30min_400.csv
--rw-r--r--   0        0        0      480 2023-12-14 09:25:35.425049 nemreader-0.8.8/examples/invalid/Example_NEM12_30min_200_15min_300.csv
--rw-r--r--   0        0        0      480 2023-12-14 09:25:35.425049 nemreader-0.8.8/examples/invalid/Example_NEM12_30min_200_15min_400.csv
--rw-r--r--   0        0        0       37 2023-12-14 09:25:35.425049 nemreader-0.8.8/examples/invalid/Example_NEM12_empty.csv
--rw-r--r--   0        0        0     1147 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/invalid/Example_NEM12_incomplete_interval.csv
--rw-r--r--   0        0        0      759 2023-12-14 09:25:35.429049 nemreader-0.8.8/examples/invalid/Example_NEM12_missing_header.csv
--rw-r--r--   0        0        0     1505 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/invalid/Example_NEM12_powercor.csv
--rw-r--r--   0        0        0      316 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/invalid/Example_NEM12_powercor.csv.zip
--rw-r--r--   0        0        0     1409 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/invalid/Example_NEM12_powercor_missing_fields.csv
--rw-r--r--   0        0        0        0 2023-12-14 09:25:35.429049 nemreader-0.8.8/examples/invalid/Example_empty_file.csv
--rw-r--r--   0        0        0     1424 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#000000000000001#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0     2190 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#000000000000002#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1016 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#000000000000003#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      534 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#000000000000004#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      861 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#000000000000005#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      836 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#000000000000006#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      769 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#000000000000007#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      513 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#000000000000008#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1325 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#000000000000009#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      525 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#000000000000010#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1614 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#01010_05030502#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0     1272 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#02030_05030501#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0     1066 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#03050_05031001#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0      702 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#05090_05031401#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0      893 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#06110_05021206#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0      867 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#07130_05021202#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0      688 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#08150_05031502#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0      650 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#10190_05031401#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0      330 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#NEM1201005Scenario1#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      432 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#NEM1202025Scenario2#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      358 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#NEM1203045Scenario3#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      355 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#NEM1205085Scenario5#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      278 2021-10-10 05:55:38.466693 nemreader-0.8.8/examples/nem12/NEM12#NEM1205085bScenario5#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      346 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#NEM1206105Scenario6#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      349 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#NEM1206105bScenario7#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      497 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#NEM1208145Scenario8#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      391 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#NEM1209165Scenario9#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      331 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#NEM1210185Scenario10#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      477 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#NEM1210185Scenario10v4#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      882 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#SCENARIO1#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      751 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#SCENARIO10#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0     1101 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#SCENARIO1005032705#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0     1508 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#SCENARIO105032701#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      956 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#SCENARIO2#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0     1635 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#SCENARIO205032701#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      892 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#SCENARIO3#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0     1652 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#SCENARIO305032701#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      552 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#SCENARIO4#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      725 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#SCENARIO5#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      934 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#SCENARIO505033001#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      862 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#SCENARIO6#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      949 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#SCENARIO605033001#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      788 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#SCENARIO7#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      901 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#SCENARIO705033001#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      380 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#SCENARIO8#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      632 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#SCENARIO805040401#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      796 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#SCENARIO9#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      759 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#Scenario01#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      761 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#Scenario01#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      361 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#Scenario04#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      364 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#Scenario04#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      332 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#Scenario05#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      336 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#Scenario05#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1368 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#Scenario06#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1371 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#Scenario06#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1315 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#Scenario07#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1320 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#Scenario07#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      583 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#Scenario08#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      586 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#Scenario08#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      384 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#Scenario09#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      387 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#Scenario09#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      705 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#Scenario10#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      700 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#Scenario10#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1125 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#mdffl0000000001#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      500 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#mdffl0000000004#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      490 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/NEM12#mdffl0000000008#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      320 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/nem12#S01#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      388 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/nem12#S02#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      304 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/nem12#S03#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      324 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/nem12#S04#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      280 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/nem12#S05#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      308 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/nem12#S06#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      307 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/nem12#S07#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      329 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/nem12#S08#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      351 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/nem12#S09#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      305 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/nem12#S10#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      898 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/nem12#SCENARIO01#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     1170 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/nem12#SCENARIO01NEM1201003#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      951 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/nem12#SCENARIO02#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     2136 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/nem12#SCENARIO02NEM1202023#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      883 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/nem12#SCENARIO03#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     1972 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/nem12#SCENARIO03NEM1203043#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      550 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/nem12#SCENARIO04#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      553 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/nem12#SCENARIO05#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     1017 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/nem12#SCENARIO05NEM1205083#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      851 2021-10-10 05:55:38.470692 nemreader-0.8.8/examples/nem12/nem12#SCENARIO06#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     1488 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem12/nem12#SCENARIO06NEM1206103#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      771 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem12/nem12#SCENARIO07#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     1450 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem12/nem12#SCENARIO07NEM1206103#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      352 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem12/nem12#SCENARIO08#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      961 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem12/nem12#SCENARIO08NEM1208143#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      717 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem12/nem12#SCENARIO09#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      693 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem12/nem12#SCENARIO10#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     1070 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem12/nem12#SCENARIO10NEM1210183#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      287 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#000000000000011#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      291 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#000000000000012#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      290 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#000000000000013#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      294 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#000000000000014#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      366 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#000000000000015#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      343 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#000000000000016#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      299 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#000000000000017#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      400 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#000000000000018#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      280 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#SEN1311003#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      287 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#SEN1312023#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      278 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#SEN1313043#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      337 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#SEN1315083#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      345 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#SEN1316103#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      291 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#SEN1317123#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      334 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#SEN1318143#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      276 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario11#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      280 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario11#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      283 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario11#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      290 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario12#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      293 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario12#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      295 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario12#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      274 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario13#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      279 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario13#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      291 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario13#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      283 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario14#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      285 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario14#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      292 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario14#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      313 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario15#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      315 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario15#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      307 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario15#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      320 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario16#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      323 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario16#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      334 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario16#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      291 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario17#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      295 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario17#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      292 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario17#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      327 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario18#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      330 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario18#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      310 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#Scenario18#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      282 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#mdffl0000000013#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      285 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#mdffl000000016A#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      283 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#mdffl000000016B#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      285 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#mdffl000000016C#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      288 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#mdffl000000018E#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      287 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/NEM13#mdffl000000018S#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      295 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/nem13#11#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      427 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/nem13#12#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      276 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/nem13#13#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      282 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/nem13#14#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      308 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/nem13#15#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      309 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/nem13#16#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      285 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/nem13#17#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      427 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/nem13#18#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      284 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/nem13#SCENARIO11#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      292 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/nem13#SCENARIO12#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      280 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/nem13#SCENARIO13#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      284 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/nem13#SCENARIO14#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      315 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/nem13#SCENARIO15#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      340 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/nem13#SCENARIO16#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      294 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/nem13#SCENARIO17#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      308 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/nem13/nem13#SCENARIO18#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      791 2021-10-10 05:55:38.474690 nemreader-0.8.8/examples/unzipped/Example_NEM12_actual_interval.csv
--rw-r--r--   0        0        0     1373 2022-09-08 05:58:30.808547 nemreader-0.8.8/examples/unzipped/Example_NEM12_different_interval_length.csv
--rw-r--r--   0        0        0    65648 2023-12-14 09:25:35.429049 nemreader-0.8.8/examples/unzipped/Example_NEM12_month_solar.csv
--rw-r--r--   0        0        0     4497 2021-10-10 05:55:38.478689 nemreader-0.8.8/examples/unzipped/Example_NEM12_multiple_meters.csv
--rw-r--r--   0        0        0      521 2021-10-10 05:55:38.478689 nemreader-0.8.8/examples/unzipped/Example_NEM12_multiple_quality.csv
--rw-r--r--   0        0        0      337 2021-10-10 05:55:38.478689 nemreader-0.8.8/examples/unzipped/Example_NEM12_no_scheduled_read.csv
--rw-r--r--   0        0        0      887 2021-10-10 05:55:38.478689 nemreader-0.8.8/examples/unzipped/Example_NEM12_substituted_interval.csv
--rw-r--r--   0        0        0      791 2023-12-14 09:25:35.429049 nemreader-0.8.8/examples/unzipped/Example_NEM12_upper_case_units.csv
--rw-r--r--   0        0        0      185 2021-10-10 05:55:38.478689 nemreader-0.8.8/examples/unzipped/Example_NEM13_consumption_data.csv
--rw-r--r--   0        0        0      345 2021-10-10 05:55:38.478689 nemreader-0.8.8/examples/unzipped/Example_NEM13_forward_estimate.csv
--rw-r--r--   0        0        0     1027 2023-12-14 09:31:06.152964 nemreader-0.8.8/examples/unzipped/Example_WesternPower.csv
--rwxr-xr-x   0        0        0      594 2023-12-14 09:25:35.429049 nemreader-0.8.8/mkdocs.yml
--rw-r--r--   0        0        0      820 2023-12-14 09:25:35.429049 nemreader-0.8.8/nemreader/__init__.py
--rw-r--r--   0        0        0       28 2022-07-20 19:50:44.084233 nemreader-0.8.8/nemreader/__main__.py
--rw-r--r--   0        0        0     3754 2023-12-14 09:25:35.429049 nemreader-0.8.8/nemreader/cli.py
--rw-r--r--   0        0        0     3515 2023-12-14 09:25:35.429049 nemreader-0.8.8/nemreader/nem_objects.py
--rw-r--r--   0        0        0    23282 2023-12-14 09:38:32.637893 nemreader-0.8.8/nemreader/nem_reader.py
--rw-r--r--   0        0        0     9582 2023-12-14 09:25:35.429049 nemreader-0.8.8/nemreader/output_db.py
--rw-r--r--   0        0        0     5139 2023-12-14 09:25:35.429049 nemreader-0.8.8/nemreader/outputs.py
--rw-r--r--   0        0        0        0 2021-10-10 05:55:38.478689 nemreader-0.8.8/nemreader/py.typed
--rw-r--r--   0        0        0     6140 2023-12-14 09:28:28.880655 nemreader-0.8.8/nemreader/split_days.py
--rw-r--r--   0        0        0       22 2023-12-14 09:45:53.163472 nemreader-0.8.8/nemreader/version.py
--rwxr-xr-x   0        0        0     1381 2023-12-14 09:25:35.429049 nemreader-0.8.8/pyproject.toml
--rw-r--r--   0        0        0     1956 2023-12-14 09:25:35.429049 nemreader-0.8.8/requirements.txt
--rw-r--r--   0        0        0        0 2021-10-10 05:55:38.478689 nemreader-0.8.8/tests/__init__.py
--rw-r--r--   0        0        0     1157 2023-12-14 09:25:35.429049 nemreader-0.8.8/tests/test_actual_interval.py
--rw-r--r--   0        0        0     1572 2023-12-14 09:25:35.429049 nemreader-0.8.8/tests/test_cli.py
--rw-r--r--   0        0        0      469 2023-12-14 09:25:35.429049 nemreader-0.8.8/tests/test_consumption_data.py
--rw-r--r--   0        0        0      850 2023-12-14 09:25:35.429049 nemreader-0.8.8/tests/test_dataframe_pivot.py
--rw-r--r--   0        0        0      814 2023-12-14 09:25:35.429049 nemreader-0.8.8/tests/test_day_split.py
--rw-r--r--   0        0        0     2111 2023-12-14 09:27:46.980342 nemreader-0.8.8/tests/test_file_outputs.py
--rw-r--r--   0        0        0      359 2023-12-14 09:25:35.429049 nemreader-0.8.8/tests/test_header_datestamp.py
--rw-r--r--   0        0        0     2043 2023-12-14 09:25:35.429049 nemreader-0.8.8/tests/test_incomplete_files.py
--rw-r--r--   0        0        0     1045 2023-12-14 09:42:37.049461 nemreader-0.8.8/tests/test_invalid_interval_mixing.py
--rw-r--r--   0        0        0      284 2023-12-14 09:25:35.429049 nemreader-0.8.8/tests/test_legacy.py
--rw-r--r--   0        0        0      252 2023-12-14 09:25:35.429049 nemreader-0.8.8/tests/test_many_nmis.py
--rw-r--r--   0        0        0     1034 2023-12-14 09:25:35.429049 nemreader-0.8.8/tests/test_multiple_quality.py
--rw-r--r--   0        0        0     1488 2023-12-14 09:25:35.429049 nemreader-0.8.8/tests/test_open_examples.py
--rw-r--r--   0        0        0      268 2023-12-14 09:25:35.429049 nemreader-0.8.8/tests/test_optional_columns.py
--rw-r--r--   0        0        0      929 2023-12-14 09:25:35.429049 nemreader-0.8.8/tests/test_output_db.py
--rw-r--r--   0        0        0     1307 2023-12-14 09:25:35.429049 nemreader-0.8.8/tests/test_unit_capitalisation.py
--rw-r--r--   0        0        0     2318 1970-01-01 00:00:00.000000 nemreader-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0      985 2024-05-30 08:48:44.742271 nemreader-0.9.1/.github/workflows/publish.yml
+-rwxr-xr-x   0        0        0     1102 2024-05-30 08:48:44.742271 nemreader-0.9.1/.github/workflows/pythonpackage.yml
+-rw-r--r--   0        0        0     1185 2024-05-30 08:48:44.742271 nemreader-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1074 2024-05-30 08:48:44.742271 nemreader-0.9.1/LICENSE
+-rw-r--r--   0        0        0       26 2024-05-30 08:48:44.742271 nemreader-0.9.1/MANIFEST.in
+-rw-r--r--   0        0        0     1164 2024-05-30 08:48:44.742271 nemreader-0.9.1/README.md
+-rw-r--r--   0        0        0   101291 2024-05-30 08:48:44.742271 nemreader-0.9.1/docs/_static/img/nmi-suffixes.jpg
+-rw-r--r--   0        0        0    38420 2024-05-30 08:48:44.742271 nemreader-0.9.1/docs/_static/img/nmi-suffixes2.png
+-rw-r--r--   0        0        0    10717 2024-05-30 08:48:44.742271 nemreader-0.9.1/docs/_static/img/plot_cal.png
+-rw-r--r--   0        0        0    14205 2024-05-30 08:48:44.742271 nemreader-0.9.1/docs/_static/img/plot_profile.png
+-rwxr-xr-x   0        0        0     5363 2024-05-30 08:48:44.742271 nemreader-0.9.1/docs/file-format.md
+-rwxr-xr-x   0        0        0      658 2024-05-30 08:48:44.742271 nemreader-0.9.1/docs/gen_ref_pages.py
+-rwxr-xr-x   0        0        0      469 2024-05-30 08:48:44.742271 nemreader-0.9.1/docs/index.md
+-rwxr-xr-x   0        0        0      164 2024-05-30 08:48:44.742271 nemreader-0.9.1/docs/installation.md
+-rwxr-xr-x   0        0        0     5158 2024-05-30 08:48:44.742271 nemreader-0.9.1/docs/quickstart.md
+-rw-r--r--   0        0        0       60 2024-05-30 08:48:44.742271 nemreader-0.9.1/docs/requirements.txt
+-rw-r--r--   0        0        0    29436 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/Example_NEM12_ManyNMIs.zip
+-rw-r--r--   0        0        0      708 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/Example_different_intervals.zip
+-rw-r--r--   0        0        0      288 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/invalid/Example_NEM12_15min_200_30min_300.csv
+-rw-r--r--   0        0        0      480 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/invalid/Example_NEM12_15min_200_30min_400.csv
+-rw-r--r--   0        0        0      480 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/invalid/Example_NEM12_30min_200_15min_300.csv
+-rw-r--r--   0        0        0      480 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/invalid/Example_NEM12_30min_200_15min_400.csv
+-rw-r--r--   0        0        0       37 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/invalid/Example_NEM12_empty.csv
+-rw-r--r--   0        0        0     1147 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/invalid/Example_NEM12_incomplete_interval.csv
+-rw-r--r--   0        0        0      759 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/invalid/Example_NEM12_missing_header.csv
+-rw-r--r--   0        0        0     1505 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/invalid/Example_NEM12_powercor.csv
+-rw-r--r--   0        0        0      316 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/invalid/Example_NEM12_powercor.csv.zip
+-rw-r--r--   0        0        0     1409 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/invalid/Example_NEM12_powercor_missing_fields.csv
+-rw-r--r--   0        0        0        0 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/invalid/Example_empty_file.csv
+-rw-r--r--   0        0        0     1424 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#000000000000001#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     2190 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#000000000000002#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1016 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#000000000000003#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      534 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#000000000000004#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      861 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#000000000000005#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      836 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#000000000000006#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      769 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#000000000000007#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      513 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#000000000000008#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1325 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#000000000000009#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      525 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#000000000000010#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1614 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#01010_05030502#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0     1272 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#02030_05030501#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0     1066 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#03050_05031001#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0      702 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#05090_05031401#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0      893 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#06110_05021206#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0      867 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#07130_05021202#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0      688 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#08150_05031502#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0      650 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#10190_05031401#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0      330 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#NEM1201005Scenario1#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      432 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#NEM1202025Scenario2#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      358 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#NEM1203045Scenario3#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      355 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#NEM1205085Scenario5#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      278 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#NEM1205085bScenario5#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      346 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#NEM1206105Scenario6#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      349 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#NEM1206105bScenario7#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      497 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#NEM1208145Scenario8#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      391 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#NEM1209165Scenario9#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      331 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#NEM1210185Scenario10#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      477 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#NEM1210185Scenario10v4#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      882 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#SCENARIO1#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      751 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#SCENARIO10#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1101 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#SCENARIO1005032705#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0     1508 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#SCENARIO105032701#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      956 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#SCENARIO2#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1635 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#SCENARIO205032701#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      892 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#SCENARIO3#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1652 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#SCENARIO305032701#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      552 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#SCENARIO4#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      725 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#SCENARIO5#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      934 2024-05-30 08:48:44.742271 nemreader-0.9.1/examples/nem12/NEM12#SCENARIO505033001#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      862 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#SCENARIO6#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      949 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#SCENARIO605033001#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      788 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#SCENARIO7#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      901 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#SCENARIO705033001#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      380 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#SCENARIO8#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      632 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#SCENARIO805040401#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      796 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#SCENARIO9#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      759 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#Scenario01#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      761 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#Scenario01#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      361 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#Scenario04#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      364 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#Scenario04#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      332 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#Scenario05#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      336 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#Scenario05#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1368 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#Scenario06#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1371 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#Scenario06#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1315 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#Scenario07#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1320 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#Scenario07#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      583 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#Scenario08#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      586 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#Scenario08#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      384 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#Scenario09#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      387 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#Scenario09#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      705 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#Scenario10#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      700 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#Scenario10#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1125 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#mdffl0000000001#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      500 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#mdffl0000000004#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      490 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/NEM12#mdffl0000000008#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      320 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#S01#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      388 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#S02#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      304 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#S03#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      324 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#S04#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      280 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#S05#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      308 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#S06#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      307 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#S07#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      329 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#S08#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      351 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#S09#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      305 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#S10#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      898 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#SCENARIO01#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     1170 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#SCENARIO01NEM1201003#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      951 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#SCENARIO02#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     2136 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#SCENARIO02NEM1202023#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      883 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#SCENARIO03#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     1972 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#SCENARIO03NEM1203043#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      550 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#SCENARIO04#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      553 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#SCENARIO05#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     1017 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#SCENARIO05NEM1205083#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      851 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#SCENARIO06#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     1488 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#SCENARIO06NEM1206103#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      771 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#SCENARIO07#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     1450 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#SCENARIO07NEM1206103#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      352 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#SCENARIO08#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      961 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#SCENARIO08NEM1208143#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      717 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#SCENARIO09#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      693 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#SCENARIO10#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     1070 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem12/nem12#SCENARIO10NEM1210183#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      287 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#000000000000011#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      291 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#000000000000012#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      290 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#000000000000013#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      294 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#000000000000014#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      366 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#000000000000015#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      343 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#000000000000016#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      299 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#000000000000017#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      400 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#000000000000018#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      280 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#SEN1311003#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      287 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#SEN1312023#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      278 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#SEN1313043#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      337 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#SEN1315083#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      345 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#SEN1316103#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      291 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#SEN1317123#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      334 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#SEN1318143#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      276 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario11#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      280 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario11#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      283 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario11#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      290 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario12#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      293 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario12#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      295 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario12#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      274 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario13#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      279 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario13#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      291 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario13#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      283 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario14#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      285 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario14#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      292 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario14#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      313 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario15#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      315 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario15#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      307 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario15#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      320 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario16#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      323 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario16#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      334 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario16#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      291 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario17#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      295 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario17#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      292 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario17#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      327 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario18#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      330 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario18#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      310 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#Scenario18#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      282 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#mdffl0000000013#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      285 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#mdffl000000016A#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      283 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#mdffl000000016B#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      285 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#mdffl000000016C#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      288 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#mdffl000000018E#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      287 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/NEM13#mdffl000000018S#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      295 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/nem13#11#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      427 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/nem13#12#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      276 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/nem13#13#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      282 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/nem13#14#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      308 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/nem13#15#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      309 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/nem13#16#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      285 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/nem13#17#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      427 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/nem13#18#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      284 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/nem13#SCENARIO11#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      292 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/nem13#SCENARIO12#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      280 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/nem13#SCENARIO13#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      284 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/nem13#SCENARIO14#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      315 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/nem13#SCENARIO15#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      340 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/nem13#SCENARIO16#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      294 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/nem13#SCENARIO17#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      308 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/nem13/nem13#SCENARIO18#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      791 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/unzipped/Example_NEM12_actual_interval.csv
+-rw-r--r--   0        0        0     1373 2024-05-30 08:48:44.746271 nemreader-0.9.1/examples/unzipped/Example_NEM12_different_interval_length.csv
+-rw-r--r--   0        0        0    65648 2024-05-30 08:48:44.750271 nemreader-0.9.1/examples/unzipped/Example_NEM12_month_solar.csv
+-rw-r--r--   0        0        0     4497 2024-05-30 08:48:44.750271 nemreader-0.9.1/examples/unzipped/Example_NEM12_multiple_meters.csv
+-rw-r--r--   0        0        0      521 2024-05-30 08:48:44.750271 nemreader-0.9.1/examples/unzipped/Example_NEM12_multiple_quality.csv
+-rw-r--r--   0        0        0      337 2024-05-30 08:48:44.750271 nemreader-0.9.1/examples/unzipped/Example_NEM12_no_scheduled_read.csv
+-rw-r--r--   0        0        0    37626 2024-05-30 08:48:44.750271 nemreader-0.9.1/examples/unzipped/Example_NEM12_partialchannel.csv
+-rw-r--r--   0        0        0      887 2024-05-30 08:48:44.750271 nemreader-0.9.1/examples/unzipped/Example_NEM12_substituted_interval.csv
+-rw-r--r--   0        0        0      791 2024-05-30 08:48:44.750271 nemreader-0.9.1/examples/unzipped/Example_NEM12_upper_case_units.csv
+-rw-r--r--   0        0        0      185 2024-05-30 08:48:44.750271 nemreader-0.9.1/examples/unzipped/Example_NEM13_consumption_data.csv
+-rw-r--r--   0        0        0      345 2024-05-30 08:48:44.750271 nemreader-0.9.1/examples/unzipped/Example_NEM13_forward_estimate.csv
+-rw-r--r--   0        0        0     1027 2024-05-30 08:48:44.750271 nemreader-0.9.1/examples/unzipped/Example_WesternPower.csv
+-rwxr-xr-x   0        0        0      594 2024-05-30 08:48:44.750271 nemreader-0.9.1/mkdocs.yml
+-rw-r--r--   0        0        0      820 2024-05-30 08:48:44.750271 nemreader-0.9.1/nemreader/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-30 08:48:44.750271 nemreader-0.9.1/nemreader/__main__.py
+-rw-r--r--   0        0        0     3618 2024-05-30 08:48:44.750271 nemreader-0.9.1/nemreader/cli.py
+-rw-r--r--   0        0        0     3503 2024-05-30 08:48:44.750271 nemreader-0.9.1/nemreader/nem_objects.py
+-rw-r--r--   0        0        0    23307 2024-05-30 08:48:44.750271 nemreader-0.9.1/nemreader/nem_reader.py
+-rw-r--r--   0        0        0     9548 2024-05-30 08:48:44.750271 nemreader-0.9.1/nemreader/output_db.py
+-rw-r--r--   0        0        0     5094 2024-05-30 08:48:44.750271 nemreader-0.9.1/nemreader/outputs.py
+-rw-r--r--   0        0        0        0 2024-05-30 08:48:44.750271 nemreader-0.9.1/nemreader/py.typed
+-rw-r--r--   0        0        0     6190 2024-05-30 08:48:44.750271 nemreader-0.9.1/nemreader/split_days.py
+-rw-r--r--   0        0        0       22 2024-05-30 08:48:44.750271 nemreader-0.9.1/nemreader/version.py
+-rwxr-xr-x   0        0        0     1338 2024-05-30 08:48:44.750271 nemreader-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1222 2024-05-30 08:48:44.750271 nemreader-0.9.1/requirements.txt
+-rw-r--r--   0        0        0        0 2024-05-30 08:48:44.750271 nemreader-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0     1157 2024-05-30 08:48:44.750271 nemreader-0.9.1/tests/test_actual_interval.py
+-rw-r--r--   0        0        0     1572 2024-05-30 08:48:44.750271 nemreader-0.9.1/tests/test_cli.py
+-rw-r--r--   0        0        0      469 2024-05-30 08:48:44.750271 nemreader-0.9.1/tests/test_consumption_data.py
+-rw-r--r--   0        0        0     1504 2024-05-30 08:48:44.750271 nemreader-0.9.1/tests/test_dataframe_pivot.py
+-rw-r--r--   0        0        0      814 2024-05-30 08:48:44.750271 nemreader-0.9.1/tests/test_day_split.py
+-rw-r--r--   0        0        0     2111 2024-05-30 08:48:44.750271 nemreader-0.9.1/tests/test_file_outputs.py
+-rw-r--r--   0        0        0      359 2024-05-30 08:48:44.750271 nemreader-0.9.1/tests/test_header_datestamp.py
+-rw-r--r--   0        0        0     2052 2024-05-30 08:48:44.750271 nemreader-0.9.1/tests/test_incomplete_files.py
+-rw-r--r--   0        0        0     1045 2024-05-30 08:48:44.750271 nemreader-0.9.1/tests/test_invalid_interval_mixing.py
+-rw-r--r--   0        0        0      284 2024-05-30 08:48:44.750271 nemreader-0.9.1/tests/test_legacy.py
+-rw-r--r--   0        0        0      252 2024-05-30 08:48:44.750271 nemreader-0.9.1/tests/test_many_nmis.py
+-rw-r--r--   0        0        0     1034 2024-05-30 08:48:44.750271 nemreader-0.9.1/tests/test_multiple_quality.py
+-rw-r--r--   0        0        0     2119 2024-05-30 08:48:44.750271 nemreader-0.9.1/tests/test_open_examples.py
+-rw-r--r--   0        0        0      268 2024-05-30 08:48:44.750271 nemreader-0.9.1/tests/test_optional_columns.py
+-rw-r--r--   0        0        0      929 2024-05-30 08:48:44.750271 nemreader-0.9.1/tests/test_output_db.py
+-rw-r--r--   0        0        0     1300 2024-05-30 08:48:44.750271 nemreader-0.9.1/tests/test_unit_capitalisation.py
+-rw-r--r--   0        0        0     2070 1970-01-01 00:00:00.000000 nemreader-0.9.1/PKG-INFO
```

### Comparing `nemreader-0.8.8/.github/workflows/publish.yml` & `nemreader-0.9.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/.gitignore` & `nemreader-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/LICENSE` & `nemreader-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/README.md` & `nemreader-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/docs/_static/img/nmi-suffixes.jpg` & `nemreader-0.9.1/docs/_static/img/nmi-suffixes.jpg`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/docs/_static/img/nmi-suffixes2.png` & `nemreader-0.9.1/docs/_static/img/nmi-suffixes2.png`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/docs/_static/img/plot_cal.png` & `nemreader-0.9.1/docs/_static/img/plot_cal.png`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/docs/_static/img/plot_profile.png` & `nemreader-0.9.1/docs/_static/img/plot_profile.png`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/docs/file-format.md` & `nemreader-0.9.1/docs/file-format.md`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/docs/gen_ref_pages.py` & `nemreader-0.9.1/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/docs/quickstart.md` & `nemreader-0.9.1/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/Example_NEM12_ManyNMIs.zip` & `nemreader-0.9.1/examples/Example_NEM12_ManyNMIs.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/Example_different_intervals.zip` & `nemreader-0.9.1/examples/Example_different_intervals.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/invalid/Example_NEM12_incomplete_interval.csv` & `nemreader-0.9.1/examples/invalid/Example_NEM12_incomplete_interval.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/invalid/Example_NEM12_missing_header.csv` & `nemreader-0.9.1/examples/invalid/Example_NEM12_missing_header.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/invalid/Example_NEM12_powercor.csv` & `nemreader-0.9.1/examples/invalid/Example_NEM12_powercor.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/invalid/Example_NEM12_powercor_missing_fields.csv` & `nemreader-0.9.1/examples/invalid/Example_NEM12_powercor_missing_fields.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#000000000000001#CNRGYMDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#000000000000001#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#000000000000002#CNRGYMDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#000000000000002#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#000000000000003#CNRGYMDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#000000000000003#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#000000000000004#CNRGYMDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#000000000000004#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#000000000000005#CNRGYMDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#000000000000005#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#000000000000006#CNRGYMDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#000000000000006#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#000000000000007#CNRGYMDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#000000000000007#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#000000000000008#CNRGYMDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#000000000000008#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#000000000000009#CNRGYMDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#000000000000009#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#000000000000010#CNRGYMDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#000000000000010#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#01010_05030502#WBAYM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#01010_05030502#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#02030_05030501#WBAYM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#02030_05030501#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#03050_05031001#WBAYM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#03050_05031001#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#05090_05031401#WBAYM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#05090_05031401#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#06110_05021206#WBAYM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#06110_05021206#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#07130_05021202#WBAYM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#07130_05021202#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#08150_05031502#WBAYM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#08150_05031502#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#10190_05031401#WBAYM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#10190_05031401#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#SCENARIO1#UNITEDDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#SCENARIO1#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#SCENARIO10#UNITEDDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#SCENARIO10#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#SCENARIO1005032705#ENERGEXM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#SCENARIO1005032705#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#SCENARIO105032701#ENERGEXM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#SCENARIO105032701#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#SCENARIO2#UNITEDDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#SCENARIO2#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#SCENARIO205032701#ENERGEXM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#SCENARIO205032701#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#SCENARIO3#UNITEDDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#SCENARIO3#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#SCENARIO305032701#ENERGEXM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#SCENARIO305032701#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#SCENARIO4#UNITEDDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#SCENARIO4#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#SCENARIO5#UNITEDDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#SCENARIO5#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#SCENARIO505033001#ENERGEXM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#SCENARIO505033001#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#SCENARIO6#UNITEDDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#SCENARIO6#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#SCENARIO605033001#ENERGEXM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#SCENARIO605033001#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#SCENARIO7#UNITEDDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#SCENARIO7#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#SCENARIO705033001#ENERGEXM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#SCENARIO705033001#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#SCENARIO805040401#ENERGEXM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#SCENARIO805040401#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#SCENARIO9#UNITEDDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#SCENARIO9#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#Scenario01#ETSAMDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#Scenario01#ETSAMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#Scenario01#POWERMDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#Scenario01#POWERMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#Scenario06#ETSAMDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#Scenario06#ETSAMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#Scenario06#POWERMDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#Scenario06#POWERMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#Scenario07#ETSAMDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#Scenario07#ETSAMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#Scenario07#POWERMDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#Scenario07#POWERMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#Scenario08#ETSAMDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#Scenario08#ETSAMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#Scenario08#POWERMDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#Scenario08#POWERMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#Scenario10#ETSAMDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#Scenario10#ETSAMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#Scenario10#POWERMDP#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#Scenario10#POWERMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/NEM12#mdffl0000000001#ACTEWM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/NEM12#mdffl0000000001#ACTEWM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/nem12#SCENARIO01#TCAUSTM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/nem12#SCENARIO01#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/nem12#SCENARIO01NEM1201003#ELECTDSM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/nem12#SCENARIO01NEM1201003#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/nem12#SCENARIO02#TCAUSTM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/nem12#SCENARIO02#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/nem12#SCENARIO02NEM1202023#ELECTDSM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/nem12#SCENARIO02NEM1202023#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/nem12#SCENARIO03#TCAUSTM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/nem12#SCENARIO03#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/nem12#SCENARIO03NEM1203043#ELECTDSM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/nem12#SCENARIO03NEM1203043#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/nem12#SCENARIO04#TCAUSTM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/nem12#SCENARIO04#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/nem12#SCENARIO05#TCAUSTM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/nem12#SCENARIO05#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/nem12#SCENARIO05NEM1205083#ELECTDSM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/nem12#SCENARIO05NEM1205083#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/nem12#SCENARIO06#TCAUSTM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/nem12#SCENARIO06#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/nem12#SCENARIO06NEM1206103#ELECTDSM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/nem12#SCENARIO06NEM1206103#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/nem12#SCENARIO07#TCAUSTM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/nem12#SCENARIO07#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/nem12#SCENARIO07NEM1206103#ELECTDSM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/nem12#SCENARIO07NEM1206103#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/nem12#SCENARIO08NEM1208143#ELECTDSM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/nem12#SCENARIO08NEM1208143#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/nem12#SCENARIO09#TCAUSTM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/nem12#SCENARIO09#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/nem12#SCENARIO10#TCAUSTM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/nem12#SCENARIO10#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/nem12/nem12#SCENARIO10NEM1210183#ELECTDSM#NEMMCO.zip` & `nemreader-0.9.1/examples/nem12/nem12#SCENARIO10NEM1210183#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/unzipped/Example_NEM12_actual_interval.csv` & `nemreader-0.9.1/examples/unzipped/Example_NEM12_actual_interval.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/unzipped/Example_NEM12_different_interval_length.csv` & `nemreader-0.9.1/examples/unzipped/Example_NEM12_different_interval_length.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/unzipped/Example_NEM12_month_solar.csv` & `nemreader-0.9.1/examples/unzipped/Example_NEM12_month_solar.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/unzipped/Example_NEM12_multiple_meters.csv` & `nemreader-0.9.1/examples/unzipped/Example_NEM12_multiple_meters.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/unzipped/Example_NEM12_multiple_quality.csv` & `nemreader-0.9.1/examples/unzipped/Example_NEM12_multiple_quality.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/unzipped/Example_NEM12_substituted_interval.csv` & `nemreader-0.9.1/examples/unzipped/Example_NEM12_substituted_interval.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/unzipped/Example_NEM12_upper_case_units.csv` & `nemreader-0.9.1/examples/unzipped/Example_NEM12_upper_case_units.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/examples/unzipped/Example_WesternPower.csv` & `nemreader-0.9.1/examples/unzipped/Example_WesternPower.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/mkdocs.yml` & `nemreader-0.9.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/nemreader/__init__.py` & `nemreader-0.9.1/nemreader/__init__.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/nemreader/cli.py` & `nemreader-0.9.1/nemreader/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,18 +33,15 @@
     pass
 
 
 @app.command()
 def list_nmis(
     nemfile: Path, verbose: bool = typer.Option(False, "--verbose", "-v")
 ) -> None:
-    if verbose:
-        log_level = "DEBUG"
-    else:
-        log_level = "WARNING"
+    log_level = "DEBUG" if verbose else "WARNING"
     logging.basicConfig(level=log_level, format=LOG_FORMAT)
 
     nmis = list(nmis_in_file(nemfile))
     typer.echo("The following NMI[suffix] exist in this file:")
     for nmi, suffixes in nmis:
         suffix_str = ",".join(suffixes)
         typer.echo(f"{nmi}[{suffix_str}]")
@@ -63,18 +60,15 @@
         writable=True,
     ),
 ) -> None:
     """Output NEM file to transposed CSV.
 
     nemfile is the name of the file to parse.
     """
-    if verbose:
-        log_level = "DEBUG"
-    else:
-        log_level = "WARNING"
+    log_level = "DEBUG" if verbose else "WARNING"
     logging.basicConfig(level=log_level, format=LOG_FORMAT)
     for fname in output_as_csv(nemfile, output_dir=outdir, set_interval=set_interval):
         typer.echo(f"Created {fname}")
 
 
 @app.command()
 def output_csv_daily(
@@ -88,18 +82,15 @@
         writable=True,
     ),
 ) -> None:
     """Output NEM file to transposed CSV.
 
     nemfile is the name of the file to parse.
     """
-    if verbose:
-        log_level = "DEBUG"
-    else:
-        log_level = "WARNING"
+    log_level = "DEBUG" if verbose else "WARNING"
     logging.basicConfig(level=log_level, format=LOG_FORMAT)
     fname = output_as_daily_csv(nemfile, output_dir=outdir)
     typer.echo(f"Created {fname}")
 
 
 @app.command()
 def output_sqlite(
@@ -115,18 +106,15 @@
     set_interval: Optional[int] = None,
     verbose: bool = typer.Option(False, "--verbose", "-v"),
 ) -> None:
     """Output NEM file to SQLite DB.
 
     nemfile is the name of the file or folder to parse.
     """
-    if verbose:
-        log_level = "DEBUG"
-    else:
-        log_level = "WARNING"
+    log_level = "DEBUG" if verbose else "WARNING"
     logging.basicConfig(level=log_level, format=LOG_FORMAT)
     if os.path.isdir(nemfile):
         typer.echo(f"Getting files in directory {nemfile}")
         files = list(nemfile.glob("*.csv"))
         files += list(nemfile.glob("*.zip"))
     else:
         files = [nemfile]
```

### Comparing `nemreader-0.8.8/nemreader/nem_objects.py` & `nemreader-0.9.1/nemreader/nem_objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Dict, List, NamedTuple, Optional
+from typing import NamedTuple, Optional
 
 
 class HeaderRecord(NamedTuple):
     """Header record (100)"""
 
     version_header: str
     creation_date: Optional[datetime]
@@ -70,15 +70,15 @@
     msats_load_datetime: Optional[datetime]
 
 
 class IntervalRecord(NamedTuple):
     """Interval data record (300)"""
 
     interval_date: Optional[datetime]
-    interval_values: List[Reading]
+    interval_values: list[Reading]
     quality_method: str
     meter_serial_number: str
     reason_code: str
     reason_description: str
     update_datetime: Optional[datetime]
     msats_load_datatime: Optional[datetime]
 
@@ -110,36 +110,36 @@
     current_trans_code: str
     current_ret_service_order: str
 
 
 class NEMReadings:
     """Represents a meter reading"""
 
-    readings: Dict[str, Dict[str, List[Reading]]]
-    transactions: Dict[str, Dict[str, list]]
+    readings: dict[str, dict[str, list[Reading]]]
+    transactions: dict[str, dict[str, list]]
 
     def __init__(self, readings, transactions):
         self.readings = readings
         self.transactions = transactions
 
     class Config:
         copy_on_model_validation = "shallow"  # faster
 
 
 class NEMData:
     """Represents a meter reading"""
 
     header: HeaderRecord
-    readings: Dict[str, Dict[str, List[Reading]]]
-    transactions: Dict[str, Dict[str, list]]
+    readings: dict[str, dict[str, list[Reading]]]
+    transactions: dict[str, dict[str, list]]
 
     def __init__(self, header, readings, transactions):
         self.header = header
         self.readings = readings
         self.transactions = transactions
 
     @property
-    def nmis(self) -> List[str]:
+    def nmis(self) -> list[str]:
         return list(self.transactions.keys())
 
     class Config:
         copy_on_model_validation = "shallow"  # faster
```

### Comparing `nemreader-0.8.8/nemreader/nem_reader.py` & `nemreader-0.9.1/nemreader/nem_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import csv
+import io
 import logging
-import os
 import zipfile
+from collections.abc import Generator, Iterable
 from datetime import datetime, timedelta
 from itertools import chain, islice
-from typing import Any, Dict, Generator, Iterable, List, Optional, Tuple
+from typing import Any, Optional
 
 import pandas as pd
 
 from .nem_objects import (
     B2BDetails12,
     B2BDetails13,
     BasicMeterData,
@@ -26,32 +27,25 @@
 
 minutes_per_day = 24 * 60
 
 
 class NEMFile:
     """An NEM file object"""
 
-    def __init__(self, file_path: str, strict: bool = False) -> None:
+    def __init__(self, file_path, fileobj=None, strict: bool = False) -> None:
         self.file_path = file_path
+        self.fileobj = fileobj
         self.strict = strict
         self._nmis: set = set()
         self._nmi_channels: dict = {}
 
     def __repr__(self):
         return f"<NEMFile {self.file_path}>"
 
     @property
-    def zipped(self) -> bool:
-        """Check whether file is zipped or not"""
-        _, file_extension = os.path.splitext(self.file_path)
-        if file_extension.lower() == ".zip":
-            return True
-        return False
-
-    @property
     def nmis(self) -> set:
         """NMIs in file"""
         if self._nmis:
             return self._nmis
         self.nem_data()  # Need to process file first
         return self._nmis
 
@@ -82,53 +76,55 @@
                 raise ValueError("NEM Files must start with a 100 row")
             else:
                 log.warning("Missing header (100) row, assuming NEM12.")
                 header = HeaderRecord("NEM12", None, "", "", file_name, assumed=True)
         else:
             header = parse_100_row(first_row, file_name)
             if header.version_header not in ["NEM12", "NEM13"]:
-                raise ValueError("Invalid NEM version {}".format(header.version_header))
+                raise ValueError(f"Invalid NEM version {header.version_header}")
 
         self.header = header
         if header.assumed:
             # We have to parse the first row again so we don't miss any data.
             reader = chain([first_row], reader)
             return parse_nem12_rows(reader, file_name=nem_file)
         if header.version_header == "NEM12":
             return parse_nem12_rows(reader, file_name=nem_file)
         else:
             return parse_nem13_rows(reader)
 
     def nem_data(self) -> NEMData:
         """Return data in legacy data format"""
-        if self.zipped:
-            log.debug("Extracting zip file")
-            with zipfile.ZipFile(self.file_path, "r") as archive:
-                files = archive.namelist()
-                if len(files) > 1:
-                    raise ValueError("Only zip files with one file are supported")
-                csv_file = files[0]
-                with archive.open(csv_file) as csv_text:
-                    # Zip file is open in binary mode
-                    # So decode then convert back to list
-                    nmi_file = csv_text.read().decode("utf-8").splitlines()
-                reads = self.parse_nem_file(nmi_file, file_name=csv_file)
-                for nmi in reads.transactions.keys():
-                    self._nmis.add(nmi)
-                    suffixes = list(reads.transactions[nmi].keys())
-                    self._nmi_channels[nmi] = suffixes
-                return NEMData(
-                    header=self.header,
-                    readings=reads.readings,
-                    transactions=reads.transactions,
-                )
+        try:
+            if not isinstance(self.fileobj, io.IOBase):
+                datafile = zipfile.ZipFile(self.file_path)
+            else:
+                datafile = zipfile.ZipFile(self.fileobj)
+            files = datafile.namelist()
+            if len(files) > 1:
+                raise ValueError("Only zip files with one file are supported")
+            csv_file = files[0]
+            with datafile.open(csv_file) as csv_text:
+                # Zip file is open in binary mode
+                # So decode then convert back to list
+                nmi_file = csv_text.read().decode("utf-8").splitlines()
+            reads = self.parse_nem_file(nmi_file, file_name=csv_file)
+        except zipfile.BadZipFile:
+            """Not a zip"""
+            if not isinstance(self.fileobj, io.IOBase):
+                datafile = open(self.file_path)  # noqa: SIM115
+            else:
+                """If we've been given a binary IO stream change it"""
+                if not isinstance(self.fileobj, io.TextIOBase):
+                    datafile = self.fileobj.read().decode("utf-8")
+                else:
+                    datafile = self.fileobj
+            reads = self.parse_nem_file(datafile, file_name=self.file_path)
 
-        with open(self.file_path) as nmi_file:
-            reads = self.parse_nem_file(nmi_file)
-        for nmi in reads.transactions.keys():
+        for nmi in reads.transactions:
             self._nmis.add(nmi)
             suffixes = list(reads.transactions[nmi].keys())
             self._nmi_channels[nmi] = suffixes
         return NEMData(
             header=self.header,
             readings=reads.readings,
             transactions=reads.transactions,
@@ -136,16 +132,16 @@
 
     def get_data_frame(
         self, split_days: bool = False, set_interval: Optional[int] = None
     ) -> Optional[pd.DataFrame]:
         """Return NEMData as a DataFrame"""
         nd = self.nem_data()
         frames = []
-        for nmi in nd.readings.keys():
-            for suffix in nd.readings[nmi].keys():
+        for nmi in nd.readings:
+            for suffix in nd.readings[nmi]:
                 reads = nd.readings[nmi][suffix]
 
                 if split_days or set_interval:
                     reads = list(split_multiday_reads(reads))
 
                 if set_interval:
                     reads = list(make_set_interval(reads, set_interval))
@@ -194,50 +190,56 @@
         quality = 0
         evt_code = 0
         evt_desc = 0
         new_names = {}
         for col in df.columns:
             if "value_" in col:
                 new_names[col] = col[6:]
+
             if "quality" in col:
-                if not quality:
+                perc_nans = df[col].isna().sum() / len(df[col])
+                if not quality and perc_nans < 0.5:
                     new_names[col] = "quality"
+                    quality += 1
                 else:
                     del df[col]
-                quality += 1
+
             if "evt_code" in col:
-                if not evt_code:
+                perc_nans = df[col].isna().sum() / len(df[col])
+                if not evt_code and perc_nans < 0.5:
                     new_names[col] = "evt_code"
+                    evt_code += 1
                 else:
                     del df[col]
-                evt_code += 1
+
             if "evt_desc" in col:
-                if not evt_desc:
+                perc_nans = df[col].isna().sum() / len(df[col])
+                if not evt_desc and perc_nans < 0.5:
                     new_names[col] = "evt_desc"
+                    evt_desc += 1
                 else:
                     del df[col]
-                evt_desc += 1
         df.rename(columns=new_names, inplace=True)
         return df
 
     def get_per_nmi_dfs(
         self,
         split_days: bool = False,
         set_interval: Optional[int] = None,
         include_serno: bool = False,
-    ) -> Generator[Tuple[str, pd.DataFrame], None, None]:
+    ) -> Generator[tuple[str, pd.DataFrame], None, None]:
         df = self.get_pivot_data_frame(split_days, set_interval, include_serno)
         nmis = df.nmi.unique()
         for nmi in nmis:
             nmi_df = df[(df["nmi"] == nmi)]
             del nmi_df["nmi"]
             yield nmi, nmi_df
 
 
-def flatten_list(items: List[list]) -> list:
+def flatten_list(items: list[list]) -> list:
     """takes a list of lists, l and returns a flat list"""
     return [v for inner_l in items for v in inner_l]
 
 
 def read_nem_file(file_path: str, ignore_missing_header=False) -> NEMData:
     """Read in NEM file and return meter readings named tuple
 
@@ -247,31 +249,31 @@
     :returns: The file that was created
     """
 
     nf = NEMFile(file_path, strict=ignore_missing_header)
     return nf.nem_data()
 
 
-def parse_100_row(row: List[Any], file_name: str) -> HeaderRecord:
+def parse_100_row(row: list[Any], file_name: str) -> HeaderRecord:
     """Parse header record (100)
 
     RecordIndicator,VersionHeader,DateTime,FromParticipant,ToParticipant
     Example: 100,NEM12,200301011534,MDP1,Retailer1
     """
     return HeaderRecord(
         row[1], parse_datetime(row[2]), row[3], row[4], file_name, False
     )
 
 
 def parse_nem12_rows(nem_list: Iterable, file_name=None) -> NEMReadings:
     """Parse NEM row iterator and return meter readings named tuple"""
     # readings nested by NMI then channel
-    readings: Dict[str, Dict[str, List[Reading]]] = {}
+    readings: dict[str, dict[str, list[Reading]]] = {}
     # transactions nested by NMI then channel
-    trans: Dict[str, Dict[str, list]] = {}
+    trans: dict[str, dict[str, list]] = {}
     nmi_d = None  # current NMI details block that readings apply to
 
     observed_900_records = []
 
     for row_num, row in enumerate(nem_list, start=1):
         try:
             if not row:
@@ -281,15 +283,16 @@
             record_indicator = int(row[0])
 
             if record_indicator == 900:
                 # Powercor NEM12 files can concatenate multiple files together
                 # try to keep parsing anyway.
                 if observed_900_records:
                     log.warning(
-                        f"Found multiple end of data (900) rows on lines {observed_900_records}"
+                        "Found multiple end of data (900) rows on lines %s",
+                        observed_900_records,
                     )
 
                 observed_900_records.append(row_num)
                 pass
 
             elif record_indicator == 200:
                 try:
@@ -362,17 +365,17 @@
 
     return NEMReadings(readings=readings, transactions=trans)
 
 
 def parse_nem13_rows(nem_list: Iterable) -> NEMReadings:
     """Parse NEM row iterator and return meter readings named tuple"""
     # readings nested by NMI then channel
-    readings: Dict[str, Dict[str, List[Reading]]] = {}
+    readings: dict[str, dict[str, list[Reading]]] = {}
     # transactions nested by NMI then channel
-    trans: Dict[str, Dict[str, list]] = {}
+    trans: dict[str, dict[str, list]] = {}
     nmi_d = None  # current NMI details block that readings apply to
 
     for row in nem_list:
         record_indicator = int(row[0])
 
         if record_indicator == 900:
             for nmi in readings:
@@ -449,20 +452,22 @@
         row[1], row[2], row[3], row[4], row[5], row[6], row[7], int(row[8]), next_read
     )
 
 
 def parse_250_row(row: list) -> BasicMeterData:
     """Parse basic meter data record (250)
 
-        RecordIndicator,NMI,NMIConfiguration,RegisterID,NMISuffix,MDMDataStreamIdentifier,MeterSeri
-    alNumber,DirectionIndicator,PreviousRegisterRead,PreviousRegisterReadDateTime,PreviousQuali
-    tyMethod,PreviousReasonCode,PreviousReasonDescription,CurrentRegisterRead,CurrentRegister
-    ReadDateTime,CurrentQualityMethod,CurrentReasonCode,CurrentReasonDescription,Quantity,U
-    OM,NextScheduledReadDate,UpdateDateTime,MSATSLoadDateTime
-        Example: 250,1234567890,1141,01,11,11,METSER66,E,000021.2,20031001103230,A,,,000534.5,20040201100030,E64,77,,343.5,kWh,20040509, 20040202125010,20040203000130
+    RecordIndicator,NMI,NMIConfiguration,RegisterID,NMISuffix,
+    MDMDataStreamIdentifier,MeterSerialNumber,DirectionIndicator,
+    PreviousRegisterRead,PreviousRegisterReadDateTime,PreviousQualityMethod,
+    PreviousReasonCode,PreviousReasonDescription,CurrentRegisterRead,
+    CurrentRegisterReadDateTime,CurrentQualityMethod,CurrentReasonCode,
+    CurrentReasonDescription,Quantity,UOM,
+    NextScheduledReadDate,UpdateDateTime,MSATSLoadDateTime
+
     """
     return BasicMeterData(
         row[1],
         row[2],
         row[3],
         row[4],
         row[5],
@@ -508,16 +513,16 @@
     num_intervals = int(minutes_per_day / interval)
 
     interval_date = parse_datetime(row[1])
     last_interval = 2 + num_intervals
     if len(row) < num_intervals + num_required_non_reading_fields:
         num_rows = len(row) - num_required_non_reading_fields
         raise ValueError(
-            f"Unexpected number of values in 300 row: " +
-            f"{num_rows} readings for {interval}min intervals"
+            "Unexpected number of values in 300 row: "
+            + f"{num_rows} readings for {interval}min intervals"
         )
     quality_method = row[last_interval]
 
     # Optional fields
     reason_code = nth(row, last_interval + 1, "")
     reason_desc = nth(row, last_interval + 2, "")
     update_datetime = parse_datetime(nth(row, last_interval + 3, None))
@@ -550,15 +555,15 @@
     interval_date,
     interval,
     uom,
     quality_method,
     meter_serial_number,
     event_code: str = "",
     event_desc: str = "",
-) -> List[Reading]:
+) -> list[Reading]:
     """Convert interval values into tuples with datetime"""
     interval_delta = timedelta(minutes=interval)
     return [
         Reading(
             t_start=interval_date + (i * interval_delta),
             t_end=interval_date + (i * interval_delta) + interval_delta,
             read_value=parse_reading(val),
@@ -593,25 +598,25 @@
 
     Note that intervals are indexed from 1 not 0.
     """
     num_intervals = int(minutes_per_day / interval_length)
     start_interval = int(row[1])
     end_interval = int(row[2])
     if end_interval < start_interval:
-        raise ValueError(
-            f"End interval {end_interval} is earlier than start interval {start_interval} in 400 row."
-        )
+        msg = f"End interval {end_interval} is earlier than "
+        msg += f"start interval {start_interval} in 400 row."
+        raise ValueError(msg)
     if not (0 < start_interval <= num_intervals):
-        raise ValueError(
-            f"Invalid start interval {start_interval} in 400 row. Expecting {num_intervals} intervals."
-        )
+        msg = f"Invalid start interval {start_interval} in 400 row."
+        msg += " Expecting {num_intervals} intervals."
+        raise ValueError(msg)
     if not (0 < end_interval <= num_intervals):
-        raise ValueError(
-            f"Invalid end interval {end_interval} in 400 row. Expecting {num_intervals} intervals."
-        )
+        msg = f"Invalid end interval {end_interval} in 400 row."
+        msg += f"Expecting {num_intervals} intervals."
+        raise ValueError(msg)
 
     return EventRecord(int(row[1]), int(row[2]), row[3], row[4], row[5])
 
 
 def update_reading_events(readings, event_record):
     """Updates readings from a 300 row to reflect any events found in a
     subsequent 400 row
```

### Comparing `nemreader-0.8.8/nemreader/output_db.py` & `nemreader-0.9.1/nemreader/output_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 from collections import defaultdict
 from datetime import datetime
 from pathlib import Path
-from typing import List, NamedTuple, Optional, Tuple
+from typing import NamedTuple, Optional
 
 from dateutil.parser import isoparse
 from sqlite_utils import Database
 
 from .nem_reader import NEMFile
 from .split_days import make_set_interval, split_multiday_reads
 
@@ -128,31 +128,31 @@
     if s.hour < 16:
         return "Day"
     if s.hour < 21:
         return "Evening"
     return "Night"
 
 
-def get_nmis(db_path: Path) -> List[str]:
+def get_nmis(db_path: Path) -> list[str]:
     nmis = []
     db = Database(db_path)
     for row in db.query("select distinct nmi from nmi_summary"):
         nmis.append(row["nmi"])
     return nmis
 
 
-def get_nmi_channels(db_path: Path, nmi: str) -> List[str]:
+def get_nmi_channels(db_path: Path, nmi: str) -> list[str]:
     channels = []
     db = Database(db_path)
     for row in db.query("select * from nmi_summary where nmi = :nmi", {"nmi": nmi}):
         channels.append(row["channel"])
     return channels
 
 
-def get_nmi_date_range(db_path: Path, nmi: str) -> Tuple[datetime, datetime]:
+def get_nmi_date_range(db_path: Path, nmi: str) -> tuple[datetime, datetime]:
     db = Database(db_path)
     sql = """select MIN(first_interval) start, MAX(last_interval) end
             from nmi_summary where nmi = :nmi
             """
     rows = list(db.query(sql, {"nmi": nmi}))
     row = rows[0]
     start = isoparse(row["start"])
@@ -161,15 +161,15 @@
 
 
 class EnergyReading(NamedTuple):
     start: datetime
     value: float
 
 
-def get_nmi_readings(db_path: Path, nmi: str, channel: str) -> List[EnergyReading]:
+def get_nmi_readings(db_path: Path, nmi: str, channel: str) -> list[EnergyReading]:
     reads = []
     db = Database(db_path)
     for r in db.query(
         "select * from readings where nmi = :nmi and channel = :ch",
         {"nmi": nmi, "ch": channel},
     ):
         start = isoparse(r["t_start"])
@@ -183,24 +183,24 @@
     channels = get_nmi_channels(db_path, nmi)
 
     imp_values = defaultdict(lambda: defaultdict(int))
     exp_values = defaultdict(int)
     for ch in channels:
         if ch[0] not in ["B", "E"]:
             continue  # Skip other channels
-        feed_in = True if ch[0] == "B" else False
+        feed_in = ch[0] == "B"
         for read in get_nmi_readings(db_path, nmi, ch):
             day = read.start.strftime("%Y-%m-%d")
             if feed_in:
                 exp_values[day] += read.value
             else:
                 tod = time_of_day(read.start)
                 imp_values[day][tod] += read.value
 
-    for day in imp_values.keys():
+    for day in imp_values:
         imp1 = round(imp_values[day]["Morning"], 3)
         imp2 = round(imp_values[day]["Day"], 3)
         imp3 = round(imp_values[day]["Evening"], 3)
         imp4 = round(imp_values[day]["Night"], 3)
         imp = imp1 + imp2 + imp3 + imp4
         exp = round(exp_values[day], 3)
         item = {
@@ -226,15 +226,16 @@
             items, pk=("nmi", "day"), column_order=("nmi", "day")
         )
     logging.info("Updated day data")
 
     db.create_view(
         "combined_readings",
         """
-    SELECT nmi, t_start, t_end, SUM(CASE WHEN substr(channel,1,1) = 'B' THEN -1 * value ELSE value END) as value
+    SELECT nmi, t_start, t_end, 
+    SUM(CASE WHEN substr(channel,1,1) = 'B' THEN -1 * value ELSE value END) as value
     FROM readings
     GROUP BY nmi, t_start, t_end
     ORDER BY 1, 2
     """,
         replace=True,
     )
     log.info("Created combined readings view")
```

### Comparing `nemreader-0.8.8/nemreader/outputs.py` & `nemreader-0.9.1/nemreader/outputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import csv
 import logging
 import os
+from collections.abc import Generator
 from pathlib import Path
-from typing import Any, Dict, Generator, List, Optional, Tuple
+from typing import Any, Optional
 
 import pandas as pd
 
 from .nem_objects import Reading
 from .nem_reader import NEMFile
 from .split_days import split_multiday_reads
 
 log = logging.getLogger(__name__)
 
 
-def nmis_in_file(file_name) -> Generator[Tuple[str, List[str]], None, None]:
+def nmis_in_file(file_name) -> Generator[tuple[str, list[str]], None, None]:
     """Return list of NMIs in file"""
     nf = NEMFile(file_name, strict=False)
     nf.nem_data()
-    for nmi, suffixes in nf.nmi_channels.items():
-        yield nmi, suffixes
+    yield from nf.nmi_channels.items()
 
 
 def output_as_data_frames(
     file_name,
     split_days: bool = True,
     set_interval: Optional[int] = None,
     strict: bool = False,
-) -> List[Tuple[str, pd.DataFrame]]:
+) -> list[tuple[str, pd.DataFrame]]:
     """Return list of data frames for each NMI"""
     nf = NEMFile(file_name, strict=strict)
     data_frames = []
     for nmi, nmi_df in nf.get_per_nmi_dfs(
         split_days=split_days, set_interval=set_interval
     ):
         nmi_df.rename(columns={"quality": "quality_method"}, inplace=True)
@@ -60,33 +60,33 @@
         output_file = f"{nmi}_{last_date}_transposed.csv"
         output_path = output_dir / output_file
         nmi_df.to_csv(output_path, index=False)
         output_paths.append(output_path)
     return output_paths
 
 
-def save_to_csv(headings: List[str], rows: List[list], output_path):
+def save_to_csv(headings: list[str], rows: list[list], output_path):
     """save data to csv file"""
     with open(output_path, "w", newline="") as csvfile:
         cwriter = csv.writer(
             csvfile, delimiter=",", quotechar='"', quoting=csv.QUOTE_MINIMAL
         )
         cwriter.writerow(headings)
         for row in rows:
             cwriter.writerow(row)
     log.debug("Created %s", output_path)
     return output_path
 
 
 def flatten_and_group_rows(
     nmi: str,
-    nmi_transactions: Dict[str, list],
-    nmi_readings: Dict[str, List[Reading]],
+    nmi_transactions: dict[str, list],
+    nmi_readings: dict[str, list[Reading]],
     date_format: str = "%Y%m%d",
-) -> List[list]:
+) -> list[list]:
     """Create flattened list of NMI reading data"""
 
     channels = list(nmi_transactions.keys())
 
     # Datastream suffix starting with a number are Accumulated Metering Data (NEM13)
     # Ensure no reading exceeds 24 hours
     split_required = False
@@ -110,25 +110,25 @@
             quality = read.quality_method
             t_group = t_end.strftime(date_format)
             try:
                 date_totals[t_group] += val
             except KeyError:
                 date_totals[t_group] = val
 
-            if t_group not in date_qualities.keys():
+            if t_group not in date_qualities:
                 date_qualities[t_group] = set()
             date_qualities[t_group].add(quality)
 
-        for day in date_totals.keys():
+        for day in date_totals:
             day_total = date_totals[day]
             qualities = list(date_qualities[day])
             day_quality = "".join(qualities)
             if len(day_quality) > 1:
                 day_quality = "V"  # Multiple quality methods
-            row: List[Any] = [nmi, sn, day, ch, day_total, uom, day_quality]
+            row: list[Any] = [nmi, sn, day, ch, day_total, uom, day_quality]
             rows.append(row)
     return rows
 
 
 def output_as_daily_csv(file_name, output_dir="."):
     """
     Transpose all channels and output a daily csv that is easier
```

### Comparing `nemreader-0.8.8/nemreader/split_days.py` & `nemreader-0.9.1/nemreader/split_days.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
+from collections.abc import Generator, Iterable
 from datetime import datetime, timedelta
 from statistics import mean
-from typing import Generator, Iterable, Tuple
 
 from .nem_objects import Reading
 
 log = logging.getLogger(__name__)
 
 
 def split_multiday_reads(
@@ -51,22 +51,26 @@
     if period_end >= end:
         period_end = end
     while period_start < end:
         if period_end > end:
             period_end = end
         period_secs = (period_end - period_start).total_seconds()
         period_val = val * (period_secs / total_secs)
-        yield period_start, period_end, period_val,
+        yield (
+            period_start,
+            period_end,
+            period_val,
+        )
         period_start += timedelta(days=1)
         period_end += timedelta(days=1)
 
 
 def new_intervals(
     start_date: datetime, end_date: datetime, interval: float = 5
-) -> Generator[Tuple[datetime, datetime], None, None]:
+) -> Generator[tuple[datetime, datetime], None, None]:
     """Generate equally spaced intervals between two dates"""
     delta = timedelta(seconds=interval * 60)
     orig_delta = end_date - start_date
     if (orig_delta / delta) % 1 != 0:
         raise ValueError(f"New interval of {delta} not an increment of {orig_delta}")
     num_intervals = int(orig_delta / delta)
     for i in range(0, num_intervals):
```

### Comparing `nemreader-0.8.8/pyproject.toml` & `nemreader-0.9.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -9,25 +9,23 @@
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.8",
     "Operating System :: OS Independent",
 ]
 keywords = ["energy", "NEM12", "NEM13"]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 dynamic = ["version", "description"]
 dependencies = ["pandas", "sqlite_utils", "typer"]
 
 [project.optional-dependencies]
-test = ["pytest >=2.7.3", "pytest-cov", "mypy"]
-dev = ["black", "flake8", "flake8-bugbear", "pep8-naming", "flake8-builtins"]
+test = ["ruff", "pytest >=2.7.3", "pytest-cov", "mypy"]
 
 [project.urls]
 Source = "https://github.com/aguinane/nem-reader/"
 Documentation = "https://nem-reader.readthedocs.io/en/latest/"
 
 [project.scripts]
 nemreader = "nemreader.cli:app"
@@ -41,7 +39,10 @@
 [tool.coverage.run]
 omit = ["*/version.py", '*/__main__.py']
 
 [tool.coverage.report]
 show_missing = true
 skip_empty = true
 fail_under = 90
+
+[tool.ruff.lint]
+select = ["A", "B", "E", "F", "I", "N", "SIM", "UP"]
```

### Comparing `nemreader-0.8.8/tests/test_actual_interval.py` & `nemreader-0.9.1/tests/test_actual_interval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 
 from nemreader import NEMFile
 
 
-def test_correct_NMIs():
+def test_correct_nmis():
     nf = NEMFile("examples/unzipped/Example_NEM12_actual_interval.csv", strict=True)
     meter_data = nf.nem_data()
     assert len(meter_data.readings) == 1
     assert "VABD000163" in meter_data.readings
 
 
 def test_correct_channels():
```

### Comparing `nemreader-0.8.8/tests/test_cli.py` & `nemreader-0.9.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/tests/test_dataframe_pivot.py` & `nemreader-0.9.1/tests/test_dataframe_pivot.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,7 +17,21 @@
     assert len(df) == 144
 
     # Check grouping to 30 min
     df = nf.get_pivot_data_frame(set_interval=30)
     for suffix in ["t_start", "E1", "E2", "V1", "quality", "evt_code", "evt_desc"]:
         assert suffix in df.columns
     assert len(df) == 48
+
+
+def test_pivot_dataframe_partialchannel():
+    """Test example where some days are missing from first channel in file"""
+    nf = NEMFile("examples/unzipped/Example_NEM12_partialchannel.csv", strict=True)
+
+    # The intervals are different, so we have 48 30min + 144 10min = 192 rows
+    df = nf.get_pivot_data_frame(set_interval=30)
+    for suffix in ["t_start", "B1", "E1", "quality", "evt_code", "evt_desc"]:
+        assert suffix in df.columns
+    assert len(df) == 1488
+    for col in ["t_start", "E1", "quality", "evt_code", "evt_desc"]:  # only B1 has nans
+        perc_nans = df[col].isna().sum() / len(df[col])
+        assert perc_nans == 0.0
```

### Comparing `nemreader-0.8.8/tests/test_day_split.py` & `nemreader-0.9.1/tests/test_day_split.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,20 +8,20 @@
     file_name = "examples/unzipped/Example_NEM12_actual_interval.csv"
 
     for _, df in output_as_data_frames(file_name, set_interval=1):
         first = df.iloc[0]
         delta = pd.Timedelta(first.t_end - first.t_start).seconds
         assert delta == 60 * 1
 
-        assert first.E1 == 1.111 / 30
+        assert 1.111 / 30 == first.E1
 
 
 def test_group_interval():
     """Create a temporary csv output"""
     file_name = "examples/unzipped/Example_NEM12_actual_interval.csv"
 
     for _, df in output_as_data_frames(file_name, set_interval=60):
         first = df.iloc[0]
         delta = pd.Timedelta(first.t_end - first.t_start).seconds
         assert delta == 60 * 60
 
-        assert first.E1 == 1.111 * 2
+        assert 1.111 * 2 == first.E1
```

### Comparing `nemreader-0.8.8/tests/test_file_outputs.py` & `nemreader-0.9.1/tests/test_file_outputs.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/tests/test_incomplete_files.py` & `nemreader-0.9.1/tests/test_incomplete_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 
 from nemreader import NEMFile
 
 
-def test_correct_NMIs():
+def test_correct_nmis_powercor():
     nf = NEMFile("examples/invalid/Example_NEM12_powercor.csv", strict=False)
     meter_data = nf.nem_data()
     assert len(meter_data.readings) == 1
     assert "VABD000163" in meter_data.readings
 
 
 def test_incomplete_interval_row():
```

### Comparing `nemreader-0.8.8/tests/test_invalid_interval_mixing.py` & `nemreader-0.9.1/tests/test_invalid_interval_mixing.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/tests/test_multiple_quality.py` & `nemreader-0.9.1/tests/test_multiple_quality.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/tests/test_open_examples.py` & `nemreader-0.9.1/tests/test_open_examples.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,14 +13,29 @@
             continue
         test_file = os.path.join(test_path, file_name)
         nf = NEMFile(test_file, strict=True)
         meter_data = nf.nem_data()
         assert meter_data.header.version_header in ["NEM12", "NEM13"]
 
 
+def test_blob_load():
+    """Loads a file into a buffer then passes it into be processed"""
+    skips = ["Example_NEM12_powercor.csv", "Example_NEM12_powercor_missing_fields.csv"]
+    test_path = os.path.abspath("examples/nem12")
+    for file_name in os.listdir(test_path):
+        if file_name in skips:
+            continue
+        test_filename = os.path.join(test_path, file_name)
+        """Blob load here"""
+        with open(test_filename, "rb") as test_file:
+            nf = NEMFile(test_file, strict=True)
+            meter_data = nf.nem_data()
+            assert meter_data.header.version_header in ["NEM12", "NEM13"]
+
+
 def test_nem12_examples():
     """Open and parse zipped NEM12 example files"""
     skips = [
         "NEM12#Scenario10#ETSAMDP#NEMMCO.zip",  # 300 Row has new line
         "Example_NEM12_powercor.csv.zip",
     ]
     test_path = os.path.abspath("examples/nem12")
```

### Comparing `nemreader-0.8.8/tests/test_output_db.py` & `nemreader-0.9.1/tests/test_output_db.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.8/tests/test_unit_capitalisation.py` & `nemreader-0.9.1/tests/test_unit_capitalisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     meter_data = nf.nem_data()
 
     df_15min = nf.get_pivot_data_frame(split_days=True, set_interval=15)
     df_30min = nf.get_pivot_data_frame(split_days=True, set_interval=30)
     df_60min = nf.get_pivot_data_frame(split_days=True, set_interval=60)
 
     for nmi, nmi_readings in meter_data.readings.items():
-        for key in nmi_readings.keys():
+        for key in nmi_readings:
             assert nmi_readings[key][0].t_end - nmi_readings[key][
                 0
             ].t_start == pd.Timedelta(minutes=30)
             assert "H" in nmi_readings[key][0].uom
 
         nmi_df_15min = df_15min[(df_15min["nmi"] == nmi)]
         nmi_df_30min = df_30min[(df_30min["nmi"] == nmi)]
```

### Comparing `nemreader-0.8.8/PKG-INFO` & `nemreader-0.9.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 Metadata-Version: 2.1
 Name: nemreader
-Version: 0.8.8
+Version: 0.9.1
 Summary: nemreader
 Keywords: energy,NEM12,NEM13
 Author-email: Alex Guinman <alex@guinman.id.au>
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Dist: pandas
 Requires-Dist: sqlite_utils
 Requires-Dist: typer
-Requires-Dist: black ; extra == "dev"
-Requires-Dist: flake8 ; extra == "dev"
-Requires-Dist: flake8-bugbear ; extra == "dev"
-Requires-Dist: pep8-naming ; extra == "dev"
-Requires-Dist: flake8-builtins ; extra == "dev"
+Requires-Dist: ruff ; extra == "test"
 Requires-Dist: pytest >=2.7.3 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: mypy ; extra == "test"
 Project-URL: Documentation, https://nem-reader.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/aguinane/nem-reader/
-Provides-Extra: dev
 Provides-Extra: test
 
 # nem-reader
 
 ![Python package](https://github.com/aguinane/nem-reader/workflows/Python%20package/badge.svg?branch=master)
 [![PyPI version](https://img.shields.io/pypi/pyversions/nemreader?color=%2344CC11)](https://pypi.org/project/nemreader/)
 [![PyPi downloads](https://img.shields.io/pypi/dw/nemreader?label=downloads@pypi&color=344CC11)](https://pypi.org/project/nemreader/)
```

