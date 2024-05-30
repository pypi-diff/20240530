# Comparing `tmp/ampel_hu_astro-0.8.4a0.tar.gz` & `tmp/ampel_hu_astro-0.8.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampel_hu_astro-0.8.4a0.tar", max compression
+gzip compressed data, was "ampel_hu_astro-0.8.4a1.tar", max compression
```

## Comparing `ampel_hu_astro-0.8.4a0.tar` & `ampel_hu_astro-0.8.4a1.tar`

### file list

```diff
@@ -1,129 +1,140 @@
--rw-r--r--   0        0        0     1512 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/LICENSE
--rw-r--r--   0        0        0     1794 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/README.md
--rw-r--r--   0        0        0     3122 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/alert/DynamicShaperAlertConsumer.py
--rw-r--r--   0        0        0     8895 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/alert/NeoWisePhotometryAlertSupplier.py
--rw-r--r--   0        0        0     3592 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/alert/ResourceDependentConsumer.py
--rwxr-xr-x   0        0        0     1461 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/alert/load/WiseFileAlertLoader.py
--rw-r--r--   0        0        0     1970 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/channel_notes.txt
--rwxr-xr-x   0        0        0     2185 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/ingest/ZiGWDataPointShaper.py
--rw-r--r--   0        0        0        0 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/py.typed
--rwxr-xr-x   0        0        0      981 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/LensedTransientFilter.py
--rw-r--r--   0        0        0     2066 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/PredetectionFilter.py
--rw-r--r--   0        0        0      732 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/RandFilter.py
--rwxr-xr-x   0        0        0    15789 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/RcfFilter.py
--rw-r--r--   0        0        0     6142 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/RedshiftCatalogFilter.py
--rwxr-xr-x   0        0        0    10713 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/SimpleDecentFilter.py
--rwxr-xr-x   0        0        0     3844 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/TransientInClusterFilter.py
--rwxr-xr-x   0        0        0     4843 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/XShooterFilter.py
--rw-r--r--   0        0        0    59244 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2BayesianBlocks.py
--rwxr-xr-x   0        0        0     4932 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2BrightSNProb.py
--rwxr-xr-x   0        0        0    11158 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2CatalogMatchLocal.py
--rw-r--r--   0        0        0    17872 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2DigestRedshifts.py
--rw-r--r--   0        0        0    33136 2024-01-22 10:37:01.734132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2DustEchoEval.py
--rw-r--r--   0        0        0    11549 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2ElasticcRedshiftSampler.py
--rw-r--r--   0        0        0    24754 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2ElasticcReport.py
--rwxr-xr-x   0        0        0     2378 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2FastDecliner.py
--rw-r--r--   0        0        0     8706 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2GetLensSNParameters.py
--rwxr-xr-x   0        0        0     5369 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2HealpixProb.py
--rw-r--r--   0        0        0    15055 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2InfantCatalogEval.py
--rw-r--r--   0        0        0    35526 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2KilonovaEval.py
--rwxr-xr-x   0        0        0    10191 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2LCQuality.py
--rw-r--r--   0        0        0    10357 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2LSPhotoZTap.py
--rw-r--r--   0        0        0     2250 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2LoadRedshift.py
--rw-r--r--   0        0        0     3633 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2MatchBTS.py
--rw-r--r--   0        0        0     5353 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2MatchGRB.py
--rwxr-xr-x   0        0        0     5240 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2MinorPlanetCenter.py
--rw-r--r--   0        0        0     9680 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2MultiXgbClassifier.py
--rwxr-xr-x   0        0        0     6607 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2NedSNCosmo.py
--rwxr-xr-x   0        0        0     7132 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2NedTap.py
--rwxr-xr-x   0        0        0     5646 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2Observability.py
--rwxr-xr-x   0        0        0     3364 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PS1ThumbExtCat.py
--rwxr-xr-x   0        0        0     5965 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PS1ThumbNedSNCosmo.py
--rwxr-xr-x   0        0        0     4538 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PS1ThumbNedTap.py
--rwxr-xr-x   0        0        0     2831 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PanStarrThumbPrint.py
--rw-r--r--   0        0        0    10489 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PhaseLimit.py
--rw-r--r--   0        0        0     1979 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PropagateStockInfo.py
--rwxr-xr-x   0        0        0    15779 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RiseDeclineStat.py
--rw-r--r--   0        0        0    19608 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RunParsnip.py
--rw-r--r--   0        0        0    10460 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RunPossis.py
--rw-r--r--   0        0        0    21719 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RunSncosmo.py
--rw-r--r--   0        0        0    10795 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RunSnoopy.py
--rw-r--r--   0        0        0     5933 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RunTDE.py
--rw-r--r--   0        0        0      236 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2SNCosmo.py
--rw-r--r--   0        0        0    20983 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2TNSEval.py
--rw-r--r--   0        0        0    25895 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2TabulatorRiseDecline.py
--rw-r--r--   0        0        0    10470 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2XgbClassifier.py
--rw-r--r--   0        0        0   139314 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/data/xgb_risedecline_ndet2.json
--rw-r--r--   0        0        0    91172 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/data/xgb_risedecline_ndet3.json
--rw-r--r--   0        0        0    71112 2024-01-22 10:37:01.738132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/data/xgb_risedecline_ndet4.json
--rw-r--r--   0        0        0  8028781 2024-01-22 10:37:01.758132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/xgb_trees.py
--rw-r--r--   0        0        0     3980 2024-01-22 10:37:01.758132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/AstroColibriClient.py
--rw-r--r--   0        0        0    11364 2024-01-22 10:37:01.758132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/AstroColibriPublisher.py
--rwxr-xr-x   0        0        0     5598 2024-01-22 10:37:01.758132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/ChannelSummaryPublisher.py
--rwxr-xr-x   0        0        0    13326 2024-01-22 10:37:01.758132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/DCachePublisher.py
--rw-r--r--   0        0        0    10625 2024-01-22 10:37:01.758132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/ElasticcClassPublisher.py
--rw-r--r--   0        0        0     3565 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/ElasticcTomClient.py
--rw-r--r--   0        0        0    10021 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/HealpixCorrPlotter.py
--rw-r--r--   0        0        0     7004 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/HealpixTokenGenerator.py
--rw-r--r--   0        0        0    11976 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/PlotLightcurveSample.py
--rw-r--r--   0        0        0     4246 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/RandomMapGenerator.py
--rwxr-xr-x   0        0        0     5253 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/RapidBase.py
--rwxr-xr-x   0        0        0    12504 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/RapidLco.py
--rwxr-xr-x   0        0        0     4008 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/RapidSedm.py
--rwxr-xr-x   0        0        0    11948 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/SlackSummaryPublisher.py
--rwxr-xr-x   0        0        0     1957 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/TNSMirrorUpdater.py
--rwxr-xr-x   0        0        0    21702 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/TNSTalker.py
--rwxr-xr-x   0        0        0     2849 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/TransientInfoPrinter.py
--rw-r--r--   0        0        0    12544 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/TransientTablePublisher.py
--rwxr-xr-x   0        0        0     4304 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/TransientViewDumper.py
--rw-r--r--   0        0        0     5173 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/VOEventPublisher.py
--rwxr-xr-x   0        0        0    13060 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/ampel_tns.py
--rwxr-xr-x   0        0        0     2267 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/complement/BaseCatalogRecordComplementer.py
--rwxr-xr-x   0        0        0     4905 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/tns/TNSClient.py
--rw-r--r--   0        0        0     4100 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/tns/TNSMirrorDB.py
--rwxr-xr-x   0        0        0     1738 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/tns/TNSName.py
--rw-r--r--   0        0        0      130 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/tns/TNSToken.py
--rw-r--r--   0        0        0        0 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/tns/__init__.py
--rw-r--r--   0        0        0    20855 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/lightcurve.ZTF18abmjvpb.json
--rw-r--r--   0        0        0      634 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/test_config.py
--rw-r--r--   0        0        0      150 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/test_flatten.py
--rw-r--r--   0        0        0     4750 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/test_slackpublisher.py
--rw-r--r--   0        0        0     3350 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/test_t2brightsnprob.py
--rw-r--r--   0        0        0      468 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/test_tns.py
--rw-r--r--   0        0        0     1879 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/test_tnstalker.py
--rw-r--r--   0        0        0     8107 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/util/AmpelHealpix.py
--rw-r--r--   0        0        0     1043 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/util/ned.py
--rw-r--r--   0        0        0      408 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/ampel/contrib/hu/utils.py
--rw-r--r--   0        0        0     5328 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/alias.yml
--rw-r--r--   0        0        0      920 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_GP_10.yml
--rw-r--r--   0        0        0      660 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_GP_16.yml
--rw-r--r--   0        0        0      970 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_GP_59.yml
--rw-r--r--   0        0        0      738 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_GP_SINGLE.yml
--rw-r--r--   0        0        0      829 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_NEARBY_CLUSTERS.yml
--rw-r--r--   0        0        0      965 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_PARTNER_10.yml
--rw-r--r--   0        0        0      986 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_PARTNER_59.yml
--rw-r--r--   0        0        0      194 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_RANDOM.yml
--rw-r--r--   0        0        0      242 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_RAPID.yml
--rw-r--r--   0        0        0      800 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_RAPID_INFANT.yml
--rw-r--r--   0        0        0      995 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_RAPID_LANCASTER.yml
--rw-r--r--   0        0        0      692 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_RAPID_SINGLE.yml
--rw-r--r--   0        0        0      293 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_RAPID_SOUTH.yml
--rw-r--r--   0        0        0      293 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_RAPID_UL.yml
--rw-r--r--   0        0        0      973 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_TNS_MSIP.yml
--rw-r--r--   0        0        0      967 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_TNS_PARTNER.yml
--rw-r--r--   0        0        0      794 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/AmpelAutoLco.yml
--rw-r--r--   0        0        0      992 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/ChannelSummary.yml
--rw-r--r--   0        0        0      481 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/ClusterSummary.yml
--rw-r--r--   0        0        0     1369 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/CosmologySummary.yaml
--rw-r--r--   0        0        0      456 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/DesiSkyportal.yml
--rw-r--r--   0        0        0      585 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/DesiSkyportalSNGuess.yml
--rw-r--r--   0        0        0      568 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/DesiSkyportalSaltSN.yml
--rw-r--r--   0        0        0      431 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/LensingSummary.yml
--rw-r--r--   0        0        0      371 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/RapidAllz.yml
--rw-r--r--   0        0        0      645 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/RapidReact.yml
--rw-r--r--   0        0        0      451 2024-01-22 10:37:01.762132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/TNSSubmitComplete.yml
--rw-r--r--   0        0        0      573 2024-01-22 10:37:01.766132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/TNSSubmitNew.yml
--rw-r--r--   0        0        0      205 2024-01-22 10:37:01.766132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/UpdateTNSMirror.yml
--rw-r--r--   0        0        0     2545 2024-01-22 10:37:01.766132 ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/unit.yml
--rw-r--r--   0        0        0     4774 2024-01-22 10:37:01.782132 ampel_hu_astro-0.8.4a0/pyproject.toml
--rw-r--r--   0        0        0     4332 1970-01-01 00:00:00.000000 ampel_hu_astro-0.8.4a0/PKG-INFO
+-rw-r--r--   0        0        0     1512 2024-05-30 12:04:10.438391 ampel_hu_astro-0.8.4a1/LICENSE
+-rw-r--r--   0        0        0     9363 2024-05-30 12:04:10.438391 ampel_hu_astro-0.8.4a1/README.md
+-rw-r--r--   0        0        0     3122 2024-05-30 12:04:10.438391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/alert/DynamicShaperAlertConsumer.py
+-rw-r--r--   0        0        0     8895 2024-05-30 12:04:10.438391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/alert/NeoWisePhotometryAlertSupplier.py
+-rw-r--r--   0        0        0     3592 2024-05-30 12:04:10.438391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/alert/ResourceDependentConsumer.py
+-rwxr-xr-x   0        0        0     1461 2024-05-30 12:04:10.438391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/alert/load/WiseFileAlertLoader.py
+-rw-r--r--   0        0        0     1970 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/channel_notes.txt
+-rwxr-xr-x   0        0        0     2185 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/ingest/ZiGWDataPointShaper.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/py.typed
+-rwxr-xr-x   0        0        0      981 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t0/LensedTransientFilter.py
+-rw-r--r--   0        0        0     2066 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t0/PredetectionFilter.py
+-rw-r--r--   0        0        0      732 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t0/RandFilter.py
+-rwxr-xr-x   0        0        0    15789 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t0/RcfFilter.py
+-rw-r--r--   0        0        0     6142 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t0/RedshiftCatalogFilter.py
+-rwxr-xr-x   0        0        0    10713 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t0/SimpleDecentFilter.py
+-rwxr-xr-x   0        0        0    11644 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t0/StellarFilter.py
+-rwxr-xr-x   0        0        0     3844 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t0/TransientInClusterFilter.py
+-rwxr-xr-x   0        0        0     4843 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t0/XShooterFilter.py
+-rw-r--r--   0        0        0     6941 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2BaseLightcurveFitter.py
+-rw-r--r--   0        0        0    59244 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2BayesianBlocks.py
+-rwxr-xr-x   0        0        0     4932 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2BrightSNProb.py
+-rwxr-xr-x   0        0        0    11158 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2CatalogMatchLocal.py
+-rw-r--r--   0        0        0     2501 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2DemoLightcurveFitter.py
+-rw-r--r--   0        0        0    21870 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2DigestRedshifts.py
+-rw-r--r--   0        0        0    33145 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2DustEchoEval.py
+-rw-r--r--   0        0        0    11549 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2ElasticcRedshiftSampler.py
+-rw-r--r--   0        0        0    24754 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2ElasticcReport.py
+-rwxr-xr-x   0        0        0     2378 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2FastDecliner.py
+-rw-r--r--   0        0        0     8706 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2GetLensSNParameters.py
+-rwxr-xr-x   0        0        0     5369 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2HealpixProb.py
+-rw-r--r--   0        0        0    15644 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2InfantCatalogEval.py
+-rw-r--r--   0        0        0    35779 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2KilonovaEval.py
+-rw-r--r--   0        0        0     5824 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2KilonovaStats.py
+-rwxr-xr-x   0        0        0    10191 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2LCQuality.py
+-rw-r--r--   0        0        0    10357 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2LSPhotoZTap.py
+-rw-r--r--   0        0        0     2250 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2LoadRedshift.py
+-rw-r--r--   0        0        0     3633 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2MatchBTS.py
+-rw-r--r--   0        0        0     5353 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2MatchGRB.py
+-rwxr-xr-x   0        0        0     5277 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2MinorPlanetCenter.py
+-rw-r--r--   0        0        0     9680 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2MultiXgbClassifier.py
+-rwxr-xr-x   0        0        0     6607 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2NedSNCosmo.py
+-rwxr-xr-x   0        0        0     7132 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2NedTap.py
+-rwxr-xr-x   0        0        0     5646 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2Observability.py
+-rwxr-xr-x   0        0        0     3364 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2PS1ThumbExtCat.py
+-rwxr-xr-x   0        0        0     5965 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2PS1ThumbNedSNCosmo.py
+-rwxr-xr-x   0        0        0     4538 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2PS1ThumbNedTap.py
+-rwxr-xr-x   0        0        0     2831 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2PanStarrThumbPrint.py
+-rw-r--r--   0        0        0    10489 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2PhaseLimit.py
+-rw-r--r--   0        0        0     2584 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2PolynomialFit.py
+-rw-r--r--   0        0        0     1979 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2PropagateStockInfo.py
+-rwxr-xr-x   0        0        0    15779 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2RiseDeclineStat.py
+-rw-r--r--   0        0        0    19608 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2RunParsnip.py
+-rw-r--r--   0        0        0    10460 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2RunPossis.py
+-rw-r--r--   0        0        0    21719 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2RunSncosmo.py
+-rw-r--r--   0        0        0    10803 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2RunSnoopy.py
+-rw-r--r--   0        0        0     5941 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2RunTDE.py
+-rw-r--r--   0        0        0      236 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2SNCosmo.py
+-rw-r--r--   0        0        0    20992 2024-05-30 12:04:10.442391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2TNSEval.py
+-rw-r--r--   0        0        0    26199 2024-05-30 12:04:10.446391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2TabulatorRiseDecline.py
+-rw-r--r--   0        0        0    10470 2024-05-30 12:04:10.446391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2XgbClassifier.py
+-rw-r--r--   0        0        0   139314 2024-05-30 12:04:10.446391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/data/xgb_risedecline_ndet2.json
+-rw-r--r--   0        0        0    91172 2024-05-30 12:04:10.446391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/data/xgb_risedecline_ndet3.json
+-rw-r--r--   0        0        0    71112 2024-05-30 12:04:10.446391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/data/xgb_risedecline_ndet4.json
+-rw-r--r--   0        0        0  8028781 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/xgb_trees.py
+-rw-r--r--   0        0        0     3254 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/AbsScoreCalculator.py
+-rw-r--r--   0        0        0     3980 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/AstroColibriClient.py
+-rw-r--r--   0        0        0    12550 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/AstroColibriPublisher.py
+-rwxr-xr-x   0        0        0     5598 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/ChannelSummaryPublisher.py
+-rw-r--r--   0        0        0     2362 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/CostCounter.py
+-rwxr-xr-x   0        0        0    13326 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/DCachePublisher.py
+-rw-r--r--   0        0        0    10625 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/ElasticcClassPublisher.py
+-rw-r--r--   0        0        0     3565 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/ElasticcTomClient.py
+-rw-r--r--   0        0        0    10021 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/HealpixCorrPlotter.py
+-rw-r--r--   0        0        0     7041 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/HealpixTokenGenerator.py
+-rw-r--r--   0        0        0    11976 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/PlotLightcurveSample.py
+-rwxr-xr-x   0        0        0    18199 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/PlotTransientLightcurves.py
+-rw-r--r--   0        0        0     4355 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/RandomMapGenerator.py
+-rwxr-xr-x   0        0        0     5253 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/RapidBase.py
+-rwxr-xr-x   0        0        0    12504 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/RapidLco.py
+-rwxr-xr-x   0        0        0     4008 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/RapidSedm.py
+-rw-r--r--   0        0        0     1647 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/ScoreSingleObject.py
+-rw-r--r--   0        0        0     3342 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/ScoreTNSObjects.py
+-rwxr-xr-x   0        0        0    11948 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/SlackSummaryPublisher.py
+-rw-r--r--   0        0        0     7508 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/SubmitTNS.py
+-rwxr-xr-x   0        0        0     1957 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/TNSMirrorUpdater.py
+-rwxr-xr-x   0        0        0     2849 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/TransientInfoPrinter.py
+-rw-r--r--   0        0        0     9198 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/TransientTablePublisher.py
+-rwxr-xr-x   0        0        0     4304 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/TransientViewDumper.py
+-rw-r--r--   0        0        0     5173 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/VOEventPublisher.py
+-rwxr-xr-x   0        0        0     2267 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/complement/BaseCatalogRecordComplementer.py
+-rwxr-xr-x   0        0        0     6500 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/tns/TNSClient.py
+-rw-r--r--   0        0        0     4100 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/tns/TNSMirrorDB.py
+-rwxr-xr-x   0        0        0     1738 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/tns/TNSName.py
+-rw-r--r--   0        0        0      130 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/tns/TNSToken.py
+-rw-r--r--   0        0        0      118 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/tns/__init__.py
+-rw-r--r--   0        0        0     6133 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/tns/tns_ampel_util.py
+-rw-r--r--   0        0        0    20855 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/test/lightcurve.ZTF18abmjvpb.json
+-rw-r--r--   0        0        0      634 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/test/test_config.py
+-rw-r--r--   0        0        0      150 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/test/test_flatten.py
+-rw-r--r--   0        0        0     4750 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/test/test_slackpublisher.py
+-rw-r--r--   0        0        0     3350 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/test/test_t2brightsnprob.py
+-rw-r--r--   0        0        0      468 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/test/test_tns.py
+-rw-r--r--   0        0        0     8132 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/util/AmpelHealpix.py
+-rw-r--r--   0        0        0     2585 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/util/automation/get_kn.py
+-rw-r--r--   0        0        0     2394 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/util/automation/jobfileCaller.py
+-rw-r--r--   0        0        0     3606 2024-05-30 12:04:10.466391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/util/automation/jobfileWriter.py
+-rw-r--r--   0        0        0      882 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/util/flatten.py
+-rw-r--r--   0        0        0     1043 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/util/ned.py
+-rw-r--r--   0        0        0      408 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/ampel/contrib/hu/utils.py
+-rw-r--r--   0        0        0     5328 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/alias.yml
+-rw-r--r--   0        0        0      920 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_GP_10.yml
+-rw-r--r--   0        0        0      660 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_GP_16.yml
+-rw-r--r--   0        0        0      970 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_GP_59.yml
+-rw-r--r--   0        0        0      738 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_GP_SINGLE.yml
+-rw-r--r--   0        0        0      829 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_NEARBY_CLUSTERS.yml
+-rw-r--r--   0        0        0      965 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_PARTNER_10.yml
+-rw-r--r--   0        0        0      986 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_PARTNER_59.yml
+-rw-r--r--   0        0        0      194 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_RANDOM.yml
+-rw-r--r--   0        0        0      242 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_RAPID.yml
+-rw-r--r--   0        0        0      800 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_RAPID_INFANT.yml
+-rw-r--r--   0        0        0      995 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_RAPID_LANCASTER.yml
+-rw-r--r--   0        0        0      692 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_RAPID_SINGLE.yml
+-rw-r--r--   0        0        0      293 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_RAPID_SOUTH.yml
+-rw-r--r--   0        0        0      293 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_RAPID_UL.yml
+-rw-r--r--   0        0        0      973 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_TNS_MSIP.yml
+-rw-r--r--   0        0        0      967 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_TNS_PARTNER.yml
+-rw-r--r--   0        0        0      794 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/process/AmpelAutoLco.yml
+-rw-r--r--   0        0        0      992 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/process/ChannelSummary.yml
+-rw-r--r--   0        0        0      481 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/process/ClusterSummary.yml
+-rw-r--r--   0        0        0     1369 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/process/CosmologySummary.yaml
+-rw-r--r--   0        0        0      456 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/process/DesiSkyportal.yml
+-rw-r--r--   0        0        0      585 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/process/DesiSkyportalSNGuess.yml
+-rw-r--r--   0        0        0      568 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/process/DesiSkyportalSaltSN.yml
+-rw-r--r--   0        0        0      431 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/process/LensingSummary.yml
+-rw-r--r--   0        0        0      371 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/process/RapidAllz.yml
+-rw-r--r--   0        0        0      645 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/process/RapidReact.yml
+-rw-r--r--   0        0        0      205 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/process/UpdateTNSMirror.yml
+-rw-r--r--   0        0        0     2895 2024-05-30 12:04:10.470391 ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/unit.yml
+-rw-r--r--   0        0        0     5208 2024-05-30 12:04:10.570392 ampel_hu_astro-0.8.4a1/pyproject.toml
+-rw-r--r--   0        0        0    12245 1970-01-01 00:00:00.000000 ampel_hu_astro-0.8.4a1/PKG-INFO
```

### Comparing `ampel_hu_astro-0.8.4a0/LICENSE` & `ampel_hu_astro-0.8.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/alert/DynamicShaperAlertConsumer.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/alert/DynamicShaperAlertConsumer.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/alert/NeoWisePhotometryAlertSupplier.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/alert/NeoWisePhotometryAlertSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/alert/ResourceDependentConsumer.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/alert/ResourceDependentConsumer.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/alert/load/WiseFileAlertLoader.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/alert/load/WiseFileAlertLoader.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/channel_notes.txt` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/channel_notes.txt`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/ingest/ZiGWDataPointShaper.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/ingest/ZiGWDataPointShaper.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/LensedTransientFilter.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t0/LensedTransientFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/PredetectionFilter.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t0/PredetectionFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/RandFilter.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t0/RandFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/RcfFilter.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t0/RcfFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/RedshiftCatalogFilter.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t0/RedshiftCatalogFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/SimpleDecentFilter.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t0/SimpleDecentFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/TransientInClusterFilter.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t0/TransientInClusterFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t0/XShooterFilter.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t0/XShooterFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2BayesianBlocks.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2BayesianBlocks.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2BrightSNProb.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2BrightSNProb.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2CatalogMatchLocal.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2CatalogMatchLocal.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2DustEchoEval.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2DustEchoEval.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 import os
 from collections.abc import Sequence
 from typing import Any, Literal
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd  # type: ignore
-from nltk import flatten  # type: ignore
 from uncertainties import unumpy  # type: ignore
 
 from ampel.abstract.AbsTiedLightCurveT2Unit import AbsTiedLightCurveT2Unit
+from ampel.contrib.hu.util.flatten import flatten
 from ampel.enum.DocumentCode import DocumentCode
 from ampel.model.StateT2Dependency import StateT2Dependency
 from ampel.struct.UnitResult import UnitResult
 from ampel.types import UBson
 from ampel.view.LightCurve import LightCurve
 from ampel.view.T2DocView import T2DocView
 from ampel.ztf.util.ZTFIdMapper import to_ztf_id
```

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2ElasticcRedshiftSampler.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2ElasticcRedshiftSampler.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2ElasticcReport.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2ElasticcReport.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2FastDecliner.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2FastDecliner.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2GetLensSNParameters.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2GetLensSNParameters.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2HealpixProb.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2HealpixProb.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2InfantCatalogEval.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2InfantCatalogEval.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,29 +34,30 @@
     # List of catalog-like output to search for redshift. It is assumed that
     # redshifts are stored as 'z'
     redshift_catalogs: list[str] = [
         "SDSS_spec",
         "NEDz",
         "GLADEv23",
         "NEDz_extcats",
+        "NEDLVS",
     ]  # Otherwise more
     # maximum redshift from T2 CATALOGMATCH catalogs (e.g. NEDz and SDSSspec)
     max_redshift: float = 0.05  # 0.1
     # minimum redshift from T2 CATALOGMATCH catalogs (e.g. NEDz and SDSSspec)
     min_redshift: float = 0.001
     # max abs mag through peak mag and redshift from catalog mach (require both)
     max_absmag: float = -12  # Originally -13, moved to -12 due to ZTF22aafoqrd
     # min abs mag through peak mag and redshift from catalog mach (require both)
     min_absmag: float = -20  # -17
     # arcsec, minimum distance to remove star matches to transient if found (eg in SDSSDR10)
     min_dist: float = 1.5
     # arcsec, maximum distance
     max_dist: float = 50
     # kpc, maximum distance
-    max_kpc_dist: float = 999
+    max_kpc_dist: float = 20
 
     # Cut on alert properties
 
     # A candidate need to have at least this many detections
     min_ndet: int = 1
     min_ndet_postul: int = 0  # and if it has this minimum nr of detection after the last significant (max_maglim) UL.
 
@@ -79,14 +80,16 @@
     # reject alert if PS1 star for any pp
     ps1_sgveto_rad: float = 1
     ps1_sgveto_sgth: float = 0.8
     # Minimal median RB.
     rb_minmed: float = 0.3
     # Minimal median RB.
     drb_minmed: float = 0.995
+    # Minimal pull w.r.t to image magnitude limit (i.e. (diffmaglim-mag)/magerr))
+    min_magpull: float = 0.0
 
     # Limiting magnitude to consider upper limits as 'significant'
     maglim_min: float = 19.5
     # A limiting magnitude max this time ago
     maglim_maxago: float = 2.5
 
     # Cut to apply to all the photopoints in the light curve.
@@ -109,48 +112,49 @@
             catinfo = cat_res.get(catname, False)
             if (
                 catinfo
                 and isinstance(catinfo.get("z", None), float)
                 and (self.min_redshift < catinfo["z"] < self.max_redshift)
                 and (self.min_dist < catinfo["dist2transient"] < self.max_dist)
             ):
-                self.logger.info(
+                self.logger.debug(
                     "Found z.",
                     extra={
                         "catalog": catname,
                         "z": catinfo["z"],
                         "dist": catinfo["dist2transient"],
                     },
                 )
                 # Calculate physical distance
                 dst_kpc = (
                     catinfo["dist2transient"]
                     * Planck15.kpc_proper_per_arcmin(catinfo["z"]).value
                     / 60.0
                 )
                 if self.max_kpc_dist > 0 and dst_kpc > self.max_kpc_dist:
-                    self.logger.info(
+                    self.logger.debug(
                         "Skip, physical distance too large.",
                         extra={"distance_kpc": dst_kpc},
                     )
                     continue
                 zmatchs.append([catinfo["z"]])
                 info[f"{catname}_z"] = catinfo["z"]
                 info[f"{catname}_dist2transient"] = catinfo["dist2transient"]
+                info[f"{catname}_kpcdist"] = dst_kpc
 
         if len(zmatchs) == 0:
             return None
         info["zs"] = zmatchs
 
         # Special catalog searches - mark transients close to AGNs
         milliquas = cat_res.get("milliquas", False)
         sdss_spec = cat_res.get("SDSS_spec", False)
-        if milliquas and milliquas["redshift"] > 0:
+        if milliquas and milliquas.get("redshift", -1) > 0:
             info["milliAGN"] = True
-        if sdss_spec and sdss_spec["bptclass"] in [4, 5]:
+        if sdss_spec and sdss_spec.get("bptclass", -99) in [4, 5]:
             info["sdssAGN"] = True
 
         # Return collected info
         return info
 
     def inspect_lc(self, lc: LightCurve) -> None | dict[str, Any]:
         """
@@ -159,29 +163,51 @@
         """
 
         # apply cut on history: consider photophoints which are sharp enough
         pps = lc.get_photopoints(filters=self.lc_filters)
         assert pps is not None
         info: dict[str, Any] = {}
 
+        # get position
+        if pos := lc.get_pos(ret="mean", filters=self.lc_filters):
+            ra, dec = pos
+        else:
+            return None
+        info["ra"] = ra
+        info["dec"] = dec
+
         # cut on number of detection
         if len(pps) < self.min_ndet:
-            self.logger.info("Rejected", extra={"det": len(pps)})
+            self.logger.debug("Rejected", extra={"det": len(pps)})
             return None
         info["detections"] = len(pps)
 
         # cut on age
         jds = [pp["body"]["jd"] for pp in pps]
-        most_recent_detection, first_detection = max(jds), min(jds)
-        age = most_recent_detection - first_detection
+        info["t_max"], info["t_min"] = max(jds), min(jds)
+        age = info["t_max"] - info["t_min"]
         if age > self.max_age or age < self.min_age:
-            self.logger.info("Rejected", extra={"age": age})
+            self.logger.debug("Rejected", extra={"age": age})
             return None
         info["age"] = age
 
+        # cut on pull compared with image diffmaglim
+        magpull = sum(
+            [
+                (pp["body"]["diffmaglim"] - pp["body"]["magpsf"])
+                / pp["body"]["sigmapsf"]
+                for pp in pps
+            ]
+        )
+        info["mag_pull"] = magpull
+        # cut on which filters used
+        if magpull < self.min_magpull:
+            self.logger.debug("Rejected", extra={"mag_pull": magpull})
+            return None
+
         # cut on number of detection after last SIGNIFICANT UL
         ulims = lc.get_upperlimits(
             filters={
                 "attribute": "diffmaglim",
                 "operator": ">=",
                 "value": self.maglim_min,
             }
@@ -196,96 +222,90 @@
                 ]
             )
             # Check if there are enough positive detection after the last significant UL
             if (
                 pps_after_ndet is not None
                 and len(pps_after_ndet) < self.min_ndet_postul
             ):
-                self.logger.info(
+                self.logger.debug(
                     "not enough consecutive detections after last significant UL.",
                     extra={"NDet": len(pps), "lastUlimJD": last_ulim_jd},
                 )
                 return None
             # Check that there is a recent ul
-            if (most_recent_detection - last_ulim_jd) > self.maglim_maxago:
-                self.logger.info(
+            if (info["t_max"] - last_ulim_jd) > self.maglim_maxago:
+                self.logger.debug(
                     "No recent UL.",
                     extra={
-                        "lastDet": most_recent_detection,
+                        "lastDet": info["t_max"],
                         "lastUlimJD": last_ulim_jd,
                     },
                 )
                 return None
-            info["last_UL"] = most_recent_detection - last_ulim_jd
+            info["last_UL"] = info["t_max"] - last_ulim_jd
         else:
-            self.logger.info("no UL")
+            self.logger.debug("no UL")
             return None
 
         # cut on number of filters
         used_filters = set([pp["body"]["fid"] for pp in pps])
         if len(used_filters) < self.min_n_filters:
-            self.logger.info("Rejected", extra={"nbr_filt": len(used_filters)})
+            self.logger.debug("Rejected", extra={"nbr_filt": len(used_filters)})
             return None
         # cut on which filters used
         if used_filters.isdisjoint(self.det_filterids):
-            self.logger.info(
+            self.logger.debug(
                 "Rejected (wrong filter det)", extra={"det_filters": used_filters}
             )
             return None
 
         # cut on range of peak magnitude
         mags = [pp["body"]["magpsf"] for pp in pps]
         peak_mag = min(mags)
         if peak_mag > self.min_peak_mag or peak_mag < self.max_peak_mag:
-            self.logger.info("Rejected", extra={"peak_mag": peak_mag})
+            self.logger.debug("Rejected", extra={"peak_mag": peak_mag})
             return None
         info["peak_mag"] = peak_mag
 
         # For rapidly declining sources the latest magnitude is probably more relevant
         latest_pps = lc.get_photopoints(
             filters={
                 "attribute": "jd",
                 "operator": "==",
-                "value": most_recent_detection,
+                "value": info["t_max"],
             }
         )
         if latest_pps:
             if not len(latest_pps) == 1:
                 raise ValueError("Have assumed a unique last photopoint")
             info["latest_mag"] = latest_pps[0]["body"]["magpsf"]
 
         # TODO: cut based on the mag rise per day (see submitRapid)
 
         # cut on galactic coordinates
-        if pos := lc.get_pos(ret="mean", filters=self.lc_filters):
-            ra, dec = pos
-        else:
-            raise ValueError("Light curve contains no points")
         coordinates = SkyCoord(ra, dec, unit="deg")
         b = coordinates.galactic.b.deg
         if abs(b) < self.min_gal_lat:
-            self.logger.info("Rejected (galactic plane)", extra={"gal_lat_b": b})
+            self.logger.debug("Rejected (galactic plane)", extra={"gal_lat_b": b})
             return None
-        info["ra"] = ra
-        info["dec"] = dec
 
         # cut on distance to closest solar system object
         # TODO: how to make this check: ('0.0' in list(phot["ssdistnr"])
         ssdist = np.array(
             [
                 pp["body"]["ssdistnr"]
                 for pp in pps
                 if "ssdistnr" in pp["body"] and pp["body"]["ssdistnr"] is not None
             ]
         )
         close_to_sso = np.logical_and(ssdist < self.ssdistnr_max, ssdist > 0)
 
         # TODO: Note that this discards a transient if it was ever close to a ss object!
         if np.any(close_to_sso):
-            self.logger.info(
+            self.logger.debug(
                 "Rejected (close to solar system object)",
                 extra={"ssdistnr": ssdist.tolist()},
             )
             return None
 
         # check PS1 sg for the full alert history
         # Note that we for this check do *not* use the lightcurve filter criteria
@@ -293,51 +313,51 @@
         if psdata := lc.get_tuples("distpsnr1", "sgscore1"):
             distpsnr1, sgscore1 = zip(*psdata, strict=False)
             is_ps1_star = np.logical_and(
                 np.array(distpsnr1) < self.ps1_sgveto_rad,
                 np.array(sgscore1) > self.ps1_sgveto_sgth,
             )
             if np.any(is_ps1_star):
-                self.logger.info(
+                self.logger.debug(
                     "Rejected (PS1 SG cut)",
                     extra={"distpsnr1": distpsnr1, "sgscore1": sgscore1},
                 )
                 return None
         else:
-            self.logger.info("No PS1 check as no data found.")
+            self.logger.debug("No PS1 check as no data found.")
 
         # cut on median RB and DRB score
         rbs = [pp["body"]["rb"] for pp in pps]
         if np.median(rbs) < self.rb_minmed:
-            self.logger.info(
+            self.logger.debug(
                 "Rejected (RB)",
                 extra={"median_rd": np.median(rbs)},
             )
             return None
         if (len(rbs) == 0) and self.rb_minmed > 0:
-            self.logger.info("Rejected (No rb info)")
+            self.logger.debug("Rejected (No rb info)")
             return None
         info["rb"] = np.median(rbs)
 
         # drb might not exist
         drbs = [pp["body"]["drb"] for pp in pps if "drb" in pp["body"]]
         if len(drbs) > 0 and np.median(drbs) < self.drb_minmed:
-            self.logger.info(
+            self.logger.debug(
                 "Rejected (dRB)",
                 extra={"median_drd": np.median(drbs)},
             )
             return None
         if (len(drbs) == 0) and self.drb_minmed > 0:
-            self.logger.info("Rejected (No drb info)")
+            self.logger.debug("Rejected (No drb info)")
             return None
 
         info["drb"] = np.median(drbs)
 
         # Transient passed pure LC criteria
-        self.logger.info("Passed T2infantCatalogEval", extra=info)
+        self.logger.debug("Passed T2infantCatalogEval", extra=info)
         return info
 
     # MANDATORY
     def process(
         self, light_curve: LightCurve, t2_views: Sequence[T2DocView]
     ) -> UBson | UnitResult:
         """
@@ -356,41 +376,41 @@
         dict
 
         Containing transient info, and in particular the 'action' key. This will be set to true
         for transients passing all selection criteria.
 
         """
 
+        lc_info = self.inspect_lc(light_curve)
+        # ii. Check whether the lightcurve passes selection criteria
+        if not lc_info:
+            return {"action": False, "eval": "LC fail selection."}
+
         # i. Check the catalog matching criteria
         # There might be multiple CatalogMatch associated with the transient
         # we here only take the first without specific origin
         t2_cat_match = t2_views[0]
 
         catalog_result = t2_cat_match.get_payload()
         if not isinstance(catalog_result, dict):
-            return {"action": False, "eval": "No catlog match result"}
+            return {"action": False, "eval": "No catalog match result"}
+
         transient_info = self.inspect_catalog(catalog_result)
         if not transient_info:
-            return {"action": False, "eval": "No cat match in z-range"}
-
-        # ii. Check whether the lightcurve passes selection criteria
-        lc_info = self.inspect_lc(light_curve)
-
-        if not lc_info:
-            transient_info["action"] = False
-            transient_info["eval"] = "LC fail selection."
-            return transient_info
+            lc_info["action"] = False
+            lc_info["eval"] = "No cat match in z-range."
+            return lc_info
         transient_info.update(lc_info)
 
         # iii. Check absolute magnitude
         sndist = Distance(z=np.mean(transient_info["zs"]), cosmology=Planck15)
         absmag = transient_info["peak_mag"] - sndist.distmod.value
         transient_info["absmag"] = absmag
         if not (self.min_absmag < absmag < self.max_absmag):
-            self.logger.info("Rejected (absmag)", extra={"absmag": absmag})
+            self.logger.debug("Rejected (absmag)", extra={"absmag": absmag})
             transient_info["action"] = False
             transient_info["eval"] = "Absmag"
             return transient_info
 
         # Passed all criteria - ready for action
         transient_info["action"] = True
         transient_info["eval"] = "Pass"
```

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2KilonovaEval.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2KilonovaEval.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,49 +258,51 @@
         }
         # print("T2KILONOVAEVAL:: ", best_res["fit_metrics"])
 
         info["possis_abspeak"] = best_res["fit_metrics"]["restpeak_model_absmag_B"]
         info["possis_obspeak"] = best_res["fit_metrics"]["obspeak_model_B"]
         info["possis_chisq"] = best_res["sncosmo_result"]["chisq"]
         info["possis_ndof"] = best_res["sncosmo_result"]["ndof"]
-        if info["possis_ndof"] != 0:
+        if info["possis_ndof"] > 0:
             info["red_chisqu"] = info["possis_chisq"] / info["possis_ndof"]
         else:
             info["red_chisqu"] = -99
+            info["rejects"].append("possis_ndof")
 
         for k, max_red_chisqu in enumerate(self.max_red_chisquares):
             if info["red_chisqu"] <= max_red_chisqu and info["red_chisqu"] >= 0.75:
                 info["pass"] += self.chisqu_rewards[k]
                 break
 
         # redundant since we only consider fits with positive ndof
         # if info["possis_ndof"] < 0:
         #     criterium_name = "possis_ndof"
         #     info["rejects"].append(criterium_name)
         #     info["pass"] -= 0  # TODO maybe find a better way to punish this
         #     return info
         # info["pass"] += 1
 
-        if self.min_obsmag < info["possis_obspeak"] < self.max_obsmag:
-            info["pass"] += 1
-        else:
-            criterium_name = "obsmag"
-            info["rejects"].append(criterium_name)
+        if info["possis_ndof"] > 0:
+            if self.min_obsmag < info["possis_obspeak"] < self.max_obsmag:
+                info["pass"] += 1
+            else:
+                criterium_name = "obsmag"
+                info["rejects"].append(criterium_name)
 
-        for range, reward in self.absmag_range_rewards:
-            if (
-                self.ideal_absmag - range
-                < info["possis_abspeak"]
-                < self.ideal_absmag + range
-            ):
-                info["pass"] += reward
-                break
-        else:
-            criterium_name = "absmag"
-            info["rejects"].append(criterium_name)
+            for range, reward in self.absmag_range_rewards:
+                if (
+                    self.ideal_absmag - range
+                    < info["possis_abspeak"]
+                    < self.ideal_absmag + range
+                ):
+                    info["pass"] += reward
+                    break
+            else:
+                criterium_name = "absmag"
+                info["rejects"].append(criterium_name)
 
         return info
 
     @no_type_check
     def inspect_lc(self, lc: LightCurve) -> None | dict[str, Any]:
         """
         Verify whether the transient lightcurve fulfill criteria for submission.
@@ -362,14 +364,15 @@
         else:
             criterium_name = "age"
             info["rejects"].append(criterium_name)
         info["age"] = age
         info["most_recent_detection"] = most_recent_detection
         info["first_detection"] = first_detection
 
+        """
         # check if theres two consecutive detections that have significant decrease in brightness
         # DONE: filter wise distinction
         if len(pps) > 1:
             criterium_name = []
             fids_list = []
             fids_list = [
                 pp_tmp["body"]["fid"]
@@ -511,26 +514,29 @@
                 "Rejected (wrong filter det)", extra={"det_filters": used_filters}
             )
             criterium_name = "wrong_filter"
             info["rejects"].append(criterium_name)
             # return None
         info["pass"] += 1
 
+        """
+
         # cut on range of peak magnitude
         mags = [pp["body"]["magpsf"] for pp in pps]
         peak_mag = min(mags)
         if peak_mag > self.min_peak_mag or peak_mag < self.max_peak_mag:
             self.logger.debug("Rejected", extra={"peak_mag": peak_mag})
             criterium_name = "peak_mag"
             info["rejects"].append(criterium_name)
             # return None
         else:
             info["pass"] += 1
         info["peak_mag"] = peak_mag
 
+        """
         # For rapidly declining sources the latest magnitude is probably more relevant
         latest_pps = lc.get_photopoints(
             filters={
                 "attribute": "jd",
                 "operator": "==",
                 "value": most_recent_detection,
             }
@@ -541,15 +547,15 @@
                 info["rejects"].append(criterium_name)
                 info["pass"] -= 0
                 return info
                 # raise ValueError("Have assumed a unique last photopoint")
             info["latest_mag"] = latest_pps[0]["body"]["magpsf"]
 
         # TODO: cut based on the mag rise per day (see submitRapid)
-
+        """
         # cut on galactic coordinates
         if pos := lc.get_pos(ret="mean", filters=self.lc_filters):
             ra, dec = pos
         else:
             criterium_name = "lc_no_points"
             info["rejects"].append(criterium_name)
             info["pass"] -= 0
@@ -560,17 +566,18 @@
         if abs(b) < self.min_gal_lat:
             self.logger.debug("Rejected (galactic plane)", extra={"gal_lat_b": b})
             criterium_name = "min_gal_lat"
             info["rejects"].append(criterium_name)
             # return None
         else:
             info["pass"] += 1
+
         info["ra"] = ra
         info["dec"] = dec
-
+        """
         # cut on distance to closest solar system object
         # TODO: how to make this check: ('0.0' in list(phot["ssdistnr"])
         ssdist = np.array(
             [
                 pp["body"]["ssdistnr"]
                 for pp in pps
                 if "ssdistnr" in pp["body"] and pp["body"]["ssdistnr"] is not None
@@ -586,14 +593,18 @@
             )
             criterium_name = "close_to_sso"
             info["rejects"].append(criterium_name)
             # return None
         else:
             info["pass"] += 1
 
+            """
+
+        """
+
         # check PS1 sg for the full alert history
         # Note that we for this check do *not* use the lightcurve filter criteria
         # TODO: Evaluate whether we should use the filters, and do a check for sufficient number of datapoints remaining
         if psdata := lc.get_tuples("distpsnr1", "sgscore1"):
             distpsnr1, sgscore1 = zip(*psdata, strict=False)
             is_ps1_star = np.logical_and(
                 np.array(distpsnr1) < self.ps1_sgveto_rad,
@@ -610,14 +621,15 @@
                 # return None
             else:
                 info[
                     "pass"
                 ] += 0  # TODO: think about whether optional checks should be rewarded more
         else:
             self.logger.debug("No PS1 check as no data found.")
+        """
 
         # cut on median RB and DRB score
         rbs = [pp["body"]["rb"] for pp in pps if "rb" in pp["body"]]
         if np.median(rbs) < self.rb_minmed:
             self.logger.debug(
                 "Rejected (RB)",
                 extra={"median_rb": np.median(rbs)},
@@ -651,15 +663,15 @@
             # return None
         else:
             info["pass"] += 1
 
         info["drb"] = np.median(drbs)
 
         # Transient passed pure LC criteria
-        self.logger.debug("Passed T2infantCatalogEval", extra=info)
+        # self.logger.debug("Passed T2infantCatalogEval", extra=info)
         return info
 
     @no_type_check
     def inspect_catmatch(self, t2res: dict[str, Any]) -> None | dict[str, Any]:
         """
         Check wether any catalog has a match for the transit.
         """
```

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2LCQuality.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2LCQuality.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2LSPhotoZTap.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2LSPhotoZTap.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2LoadRedshift.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2LoadRedshift.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2MatchBTS.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2MatchBTS.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2MatchGRB.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2MatchGRB.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2MinorPlanetCenter.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2MinorPlanetCenter.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
     # Search radius passed to MPC (arcminutes!!!)
     searchradius: float = 1
     # V-band magnitude limit passed to MPC
     maglim: float = 22
     # Potential filter for photopoint selection
     filters: None | dict | list[dict] = None
 
+    timeout: float = 30.0
+
     def process(self, pp: DataPoint) -> UBson | UnitResult:
         """
         Parameters
         -----------
                 light_curve: `ampel.base.LightCurve` instance.
                         See the LightCurve docstring for more info.
 
@@ -113,15 +115,15 @@
             "pdes": "u",
             "needed": "f",
             "ps": "n",
             "type": "p",
         }
 
         # Post the request
-        response = requests.post(url=NEO_URL, data=request_data, timeout=30)
+        response = requests.post(url=NEO_URL, data=request_data, timeout=self.timeout)
 
         # Parse the result
         soup = BeautifulSoup(response.text, "html5lib")
 
         try:
             pre = soup.find_all("pre")[-1]
             results = pre.text.lstrip(" ").split("\n")[3:]
```

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2MultiXgbClassifier.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2MultiXgbClassifier.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2NedSNCosmo.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2NedSNCosmo.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2NedTap.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2NedTap.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2Observability.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2Observability.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PS1ThumbExtCat.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2PS1ThumbExtCat.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PS1ThumbNedSNCosmo.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2PS1ThumbNedSNCosmo.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PS1ThumbNedTap.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2PS1ThumbNedTap.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PanStarrThumbPrint.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2PanStarrThumbPrint.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PhaseLimit.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2PhaseLimit.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2PropagateStockInfo.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2PropagateStockInfo.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RiseDeclineStat.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2RiseDeclineStat.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RunParsnip.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2RunParsnip.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RunPossis.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2RunPossis.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RunSncosmo.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2RunSncosmo.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RunSnoopy.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2RunSnoopy.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import os
 from collections.abc import Sequence
 from typing import Literal
 
 import numpy as np
 import snpy  # type: ignore[import]
-from sfdmap import SFDMap  # type: ignore[import]
+from sfdmap2.sfdmap import SFDMap  # type: ignore[import]
 
 from ampel.abstract.AbsTiedLightCurveT2Unit import AbsTiedLightCurveT2Unit
 from ampel.model.StateT2Dependency import StateT2Dependency
 from ampel.struct.UnitResult import UnitResult
 from ampel.types import UBson
 from ampel.view.LightCurve import LightCurve
 from ampel.view.T2DocView import T2DocView
```

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2RunTDE.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2RunTDE.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # from astropy.time import Time
 import backoff
 import numpy as np
 import sncosmo  # type: ignore[import]
 from astropy import constants as c
 from astropy import units as u
 from astropy.units import Quantity
-from sfdmap import SFDMap  # type: ignore[import]
+from sfdmap2.sfdmap import SFDMap  # type: ignore[import]
 
 from ampel.contrib.hu.t2.T2RunSncosmo import T2RunSncosmo
 
 # from ampel.enum.DocumentCode import DocumentCode
 
 # from ampel.model.StateT2Dependency import StateT2Dependency
```

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2TNSEval.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2TNSEval.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from typing import Any
 
 import numpy as np
 from astropy.coordinates import SkyCoord
 
 # T2 importing info from T3. Restructure?
 from ampel.abstract.AbsTiedLightCurveT2Unit import AbsTiedLightCurveT2Unit
-from ampel.contrib.hu.t3.ampel_tns import (
+from ampel.contrib.hu.t3.tns.tns_ampel_util import (
     TNSFILTERID,
 )
 from ampel.struct.UnitResult import UnitResult
 from ampel.types import UBson
 from ampel.view.LightCurve import LightCurve
 from ampel.view.T2DocView import T2DocView
```

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2TabulatorRiseDecline.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2TabulatorRiseDecline.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,22 +135,22 @@
      "color_list" contains a list of lists of colors which should be considered
 
     """
 
     t_cadence: float = 5.0
     significant_bands: Sequence[str] = ["lsstg", "lsstr", "lssti", "lsstz"]
     sigma_det: float = 5.0
-    sigma_slope: float = 3.0  # Threshold for having detected a slope
+    sigma_slope: float = 3.0  # Threshold for having detected a slope (flux/day)
     color_list: Sequence[Sequence[str]] = [
         ["lsstu", "lsstg"],
         ["lsstg", "lsstr"],
         ["lsstr", "lssti"],
         ["lssti", "lsstz"],
         ["lsstz", "lssty"],
-        ["ztg", "ztfr"],
+        ["ztfg", "ztfr"],
         ["ztfr", "ztfi"],
     ]
     max_tgap: int = 30
 
     # Cut the lightcurve if longer than this limit.
     # Motivated by worse classification for longer (inbalanced training?)
     # max_ndet: int = 20
@@ -170,14 +170,16 @@
 
         def linearFunc(x, intercept, slope):
             return intercept + slope * x
 
         banddata = {}
         tscale = np.mean(ftable["time"])
 
+        # print("T2TABULATORRISEDECLINE::" , np.unique(ftable["band"]))
+
         for band in set(ftable["band"]):
             bt = ftable[ftable["band"] == band]
 
             max_flux = bt["flux"].max()
             max_flux_time = bt[bt["flux"] == max_flux]["time"][0]
             banddata["jd_peak_" + band] = max_flux_time
 
@@ -217,22 +219,24 @@
         # passed after peak, such that we "should" have seen a decline.
         # We here skip this, hopefully the slope fit is sufficient
 
         # Check whether we have a significant rise detected in any band.
         risepulls = [
             banddata.get("rise_slopesig_" + band, 0) for band in set(ftable["band"])
         ]
+        # print("TABULATORRISEDECLINE:: risepulls", risepulls)
         if sum(risepulls) > self.sigma_slope:
             banddata["bool_rise"] = True
         else:
             banddata["bool_rise"] = False
         # Check whether we see a decline
         decpulls = [
             banddata.get("fall_slopesig_" + band, 0) for band in set(ftable["band"])
         ]
+        # print("TABULATORRISEDECLINE:: decpulls", decpulls)
         if sum(decpulls) < -self.sigma_slope:
             banddata["bool_fall"] = True
         else:
             banddata["bool_fall"] = False
 
         # If the transient has both a rise and a fall we can
         # define a central peak
@@ -559,15 +563,15 @@
 class T2TabulatorRiseDecline(
     AbsStateT2Unit,
     AbsTabulatedT2Unit,
     T2TabulatorRiseDeclineBase,
     BaseLightCurveFeatures,
 ):
     plot_prob: float = 0.0
-    path_testplot: str = "/home/jnordin/tmp/t2test/"
+    path_testplot: str = "./plots/"
 
     #    def __init__(self, **kwargs):
     #        super().__init__(**kwargs)
     #    def super().post_init(self):
     #        super().__init__(**kwargs)
 
     def test_plot(self, name, table, t2result):
@@ -642,14 +646,15 @@
             ]:
                 if t2result[f"bool_{boolprop}"]:
                     title += f"{boolprop} "
 
             ax.set_title(title, {"fontsize": 8})
 
         # Store figure
+        os.makedirs(self.path_testplot, exist_ok=True)
         path = os.path.join(
             self.path_testplot, "{}_{}.pdf".format(name, t2result["ndet"])
         )
         plt.tight_layout()
         plt.savefig(path)
         plt.clf()
 
@@ -663,14 +668,15 @@
         A commong Table is generated which is used as input
         to the feature generator.
         """
 
         # Convert input datapoints to standardized Astropy Table
         # Using standard tabulators
         flux_table = self.get_flux_table(datapoints)
+        # print("T2TABULATORRISEDECLINE:: ", flux_table)
 
         # Cut the flux table if requested
         if self.max_ndet > 0 and len(flux_table) > self.max_ndet:
             flux_table = self.cut_flux_table(flux_table)
 
         # Calculate get_features
         features = self.compute_stats(flux_table)
```

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/T2XgbClassifier.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/T2XgbClassifier.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/data/xgb_risedecline_ndet2.json` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/data/xgb_risedecline_ndet2.json`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/data/xgb_risedecline_ndet3.json` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/data/xgb_risedecline_ndet3.json`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/data/xgb_risedecline_ndet4.json` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/data/xgb_risedecline_ndet4.json`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t2/xgb_trees.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t2/xgb_trees.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/AstroColibriClient.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/AstroColibriClient.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/AstroColibriPublisher.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/AstroColibriPublisher.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 # Last Modified By:    jno <jnordin@physik.hu-berlin.de>
 
 # FIXME: restore mypy when this is actually ready
 # type: ignore
 
 # from itertools import islice
 import os
-import re
 from collections.abc import Generator
 
 import numpy as np
 from astropy.time import Time
 
 from ampel.abstract.AbsPhotoT3Unit import AbsPhotoT3Unit
 from ampel.content.JournalRecord import JournalRecord
@@ -74,14 +73,30 @@
     - "Nearby" if AmpelZ<0.02
     - "ProbSNIa" if ParsnipP(SNIa)>0.5
     - "ProbSN" if SNGuess=True at any phase.
     - Kilonovaness if available.
 
     Will update if new obs was made after last posting.
 
+    AC requests:
+
+
+    - Can you make sure that the event time corresponds to the one submitted to TNS?
+    - We suggest a slight renaming of the events:
+     x   * source_name: use the name of the event given by TNS and add "(Ampel)" to it. Example: TNS name "AT 2024edy" => "AT 2024edy (Ampel)"
+     x   * trigger_id: keep as it is
+     x   * we suggest you fill the ZTF identifier (e.g. ZTF24aahbwis) that you currently use a source_name into the field "discoverer_internal_name"
+    x Type: for events that are not submitted as classified to TNS (i.e. listed as AT in TNS), please change the value of the "type" parameter to "ot" (instead of "ot_sn")
+    * Classification: you can add the Ampel classification into the field "classification". E.g. if these are supernova candidates use "SN" or any classification that one could also find on TNS
+
+
+
+
+
+
     """
 
     # Limits for attributes
     nearby_z: float = 0.02
     snia_minprob: float = 0.7  # Parsnip class prob to call something SNIa
     min_kilonovaness: float = 0.0  # Parsnip class prob to call something SNIa
 
@@ -152,77 +167,35 @@
             [
                 je
                 for je in view.get_journal_entries(tier=3)
                 if self._filter_journal_astrocolobri(je, 0)
             ]
         )
 
-    def get_tnsname(self, view: "TransientView") -> bool:
-        # Was transient (successfully pushed)
-        if not view.stock:
-            return False
-        # Check whether the name is found in the name collection
-        if len(names := view.stock.get("name", [])) > 0:
-            # Will only be able to require TNS name through format
-            # dddd
-            for name in names:
-                if re.search(r"\d{4}\D{3}\D?", name):
-                    return name
-
-        # Should we look through the Journal for entries from the TNSTalker?
-        # It *should* also save these entries to name so should not be needed...
-
-        return None
-
     def process(
         self,
         tviews: Generator[TransientView, JournalAttributes, None],
         t3s: "None | T3Store" = None,
     ) -> None:
         """
         Iterate through TransientView and check which should be
         submitted / updated.
         """
 
         for tview in tviews:
-            if self.randname:
-                import random
-
-                # Generate random name (assuming publishing to dev AC)
-                tns_name = f"AmpelRand{random.randint(1, 999)}"
-            else:
-                # Find TNS name (required for AstroColibri posting)
-                # Currently assumes that this is stored either in the
-                # stock name list or can be found in the T3 journal
-                # (probably from the TNSTalker)
-                tns_name = self.get_tnsname(tview)
-                if not tns_name:
-                    self.logger.info("No TNS.", extra={"tnsName": None})
-                    continue
-
-            # Check if this was submitted
-            # TODO: How should the first submit differ from updates?
-            if self.submitted(tview):
-                # Check if it needs an update
-                if self.requires_update(tview):
-                    post_update = True
-                else:
-                    continue
-            else:
-                post_update = False
-
-            # Gather general information
+            # Gather general information, including coordinate
             payload = {
-                "type": "ot_sn",  # for optical? when to change to ot_sn?
+                "type": "ot",
                 "observatory": "ztf",
-                "source_name": to_ztf_id(int(tview.id)),
+                # "source_name": to_ztf_id(int(tview.id)),
+                "discoverer_internal_name": to_ztf_id(int(tview.id)),
                 #                'trigger_id': self.trigger_id+':'+str(tview.id),  # How do these work?
-                "trigger_id": "TNS" + tns_name,
+                # "trigger_id": "TNS" + tns_name,
                 #                'ivorn': self.trigger_id+':'+str(tview.id),       # Need ivorn schema
-                "timestamp": Time.now().iso,
+                # "timestamp": Time.now().iso,
             }
 
             # Gather photometry based information
             assert tview.t0 is not None
             # Get subset of real detections.
             # Could be complemented with further restrictions, e.g. filter / RB
             dps_det = [
@@ -231,59 +204,101 @@
                 if (pp["id"] > 0 and pp["body"].get("isdiffpos", False))
             ]
             payload["photometry"] = dps_to_astrocolobri(dps_det)
             payload["ra"] = np.mean([pp["body"]["ra"] for pp in dps_det])
             payload["dec"] = np.mean([pp["body"]["dec"] for pp in dps_det])
             payload["err"] = 1.0 / 3600  # position err ~1 arcsec in dec
 
+            # Find TNS name
+            if self.randname:
+                import random
+
+                # Generate random name (assuming publishing to dev AC)
+                tns_name = f"AmpelRand{random.randint(1, 999)}"
+                tns_submission_time = Time.now().iso
+            elif isinstance(tview.extra, dict) and "TNSReports" in tview.extra:
+                # A tns name is required, here obtained from the mirror DB through a T3 complement
+                tnsreport = next(iter(tview.extra["TNSReports"]))
+                tns_name = tnsreport["objname"]
+                tns_submission_time = tnsreport["discoverydate"]
+                print("FOUND TNS STUFF", tns_name, tns_submission_time)
+            else:
+                self.logger.debug("No TNS name", extra={"tnsName": None})
+                continue
+
+            payload["trigger_id"] = "TNS" + tns_name
+            payload["source_name"] = tns_name + " (AMPEL)"
+            payload["time"] = tns_submission_time
+
+            # Check if this was submitted
+            # TODO: How should the first submit differ from updates?
+            if self.submitted(tview):
+                # Check if it needs an update
+                if self.requires_update(tview):
+                    post_update = True
+                else:
+                    continue
+            else:
+                post_update = False
+
             # If part of random testing, perturb coordinates
             if self.randname:
                 payload["ra"] += random.randrange(-1, 1)
                 payload["dec"] += random.randrange(-1, 1)
                 payload["source_name"] += payload["trigger_id"][12:]
 
             # Gather attributes
-            attributes = []
+            attributes = {"classification": {}, "ampelProp": []}
             # Nearby attribute
             t2res = tview.get_t2_body(unit="T2DigestRedshifts")
             if isinstance(t2res, dict) and t2res.get("ampel_z", 999) < self.nearby_z:
-                attributes.append("Nearby")
-                attributes.append("AmpelZ{:.2f}".format(t2res["ampel_z"]))
+                attributes["ampelProp"].append("Nearby")
+                attributes["ampelProp"].append("AmpelZ{:.2f}".format(t2res["ampel_z"]))
             # Infant attribute
             t2res = tview.get_t2_body(unit="T2InfantCatalogEval")
             if isinstance(t2res, dict) and t2res.get("action", False):
-                attributes.append("Young")
+                attributes["ampelProp"].append("Young")
             # SNIa
             t2res = tview.get_t2_body(unit="T2RunParsnip")
             if (
                 isinstance(t2res, dict)
                 and "classification" in t2res
                 and t2res["classification"]["SNIa"] > self.snia_minprob
             ):
-                attributes.append("ProbSNIa")
+                attributes["ampelProp"].append("ProbSNIa")
+                attributes["classification"] = {
+                    "class": ["SNIa", "Other"],
+                    "prob": [
+                        t2res["classification"]["SNIa"],
+                        1 - t2res["classification"]["SNIa"],
+                    ],
+                }
             # Kilonovaness
             t2res = tview.get_t2_body(unit="T2KilonovaEval")
             if (
                 isinstance(t2res, dict)
                 and t2res.get("kilonovaness", -99) > self.min_kilonovaness
             ):
-                attributes.append("Kilonovaness{}".format(t2res["kilonovaness"]))
-                attributes.append("LVKmap{}".format(t2res["map_name"]))
+                attributes["ampelProp"].append(
+                    "Kilonovaness{}".format(t2res["kilonovaness"])
+                )
+                attributes["ampelProp"].append("LVKmap{}".format(t2res["map_name"]))
 
             # Check whether we have a figure to upload.
             # Assuming this exists locally under {stock}.png
             if self.image_path is not None:
                 ipath = self.image_path.replace("ZTFNAME", to_ztf_id(int(tview.id)))
+                ipath = self.image_path.replace("STOCK", str(tview.id))
                 # Only upload if it actually exists:
                 if not os.path.isfile(ipath):
                     ipath = None
             else:
                 ipath = None
 
-            payload["ampel_attributes"] = attributes
+            payload["broker_attributes"] = attributes
             self.logger.debug("reacting", extra={"payload": payload})
 
             # Ok, so we have a transient to react to
             if self.testcollect:
                 if post_update:
                     print("Should send an update")
                 else:
@@ -296,11 +311,14 @@
                 jcontent = {
                     "reaction": "fake submission",
                     "success": True,
                     "testcollect": True,
                 }
 
             else:
+                print("colibri submitting")
+                print(payload)
+                print(ipath)
                 jcontent = self.colibriclient.firestore_post(payload, image_path=ipath)
 
             if jcontent:
                 tviews.send(JournalAttributes(extra=jcontent))
```

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/ChannelSummaryPublisher.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/ChannelSummaryPublisher.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/DCachePublisher.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/DCachePublisher.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/ElasticcClassPublisher.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/ElasticcClassPublisher.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/ElasticcTomClient.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/ElasticcTomClient.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/HealpixCorrPlotter.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/HealpixCorrPlotter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/HealpixTokenGenerator.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/HealpixTokenGenerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,15 @@
         # count alerts before trigger time without querying for them
         count_query_dict = {
             "jd": {"$gt": start_jd, "$lt": end_jd},
             "regions": healpix_regions,
         }
         endpoint_count = "https://ampel.zeuthen.desy.de/api/ztf/archive/v3/alerts/healpix/skymap/count"
         response_count = session.post(endpoint_count, json=count_query_dict)
+        print(response_count.json())
         alert_count_nofilter = response_count.json()["count"]
         # print("ALERT COUNT NO FILTER", alert_count_nofilter)
 
         # print("HEALPIXTOKENGENERATOR::", query_dict)
 
         response = session.post(
             "streams/from_query",
```

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/PlotLightcurveSample.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/PlotLightcurveSample.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/RandomMapGenerator.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/RandomMapGenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,34 +25,27 @@
     Generate smoothed circular healpix probability values around a random coordinate.
     """
 
     save_dir: str = "."
     map_name: str = "simulated"
 
     long_range: tuple[float, float] = (0, 360)
-    lat_range: tuple[float, float] = (0, 90)
+    lat_range: tuple[float, float] = (-30, 90)
 
     fwhm_range: tuple[float, float] = (0.4, 1.2)
 
     nside: int = 32
 
     seed: int | None = None
 
     min_date: str = "2019-06-12"
     max_date: str = "2023-10-01"
 
     def process(self, t3s: T3Store) -> UBson | UnitResult:
-        tmp_date = atime.Time(self.min_date)
-        tmp_date.format = "gps"
-        self.min_date_gps = tmp_date.value
-
-        tmp_date = atime.Time(self.max_date)
-        tmp_date.format = "gps"
-        self.max_date_gps = tmp_date.value
-
+        """Generate random coordinates, generate map around coordinates, save map and generated randoms"""
         # generate random coordinates
         self.generate_randoms()
 
         # generate healpix map centered around coordinates
         self.generate_map()
 
         # save generated map
@@ -76,14 +69,22 @@
         if self.seed:
             np.random.seed(self.seed)
         else:
             self.seed = np.random.random_integers(0, 2147483647)
             print("RANDOMMAPGENERATOR:: ", self.seed)
             np.random.seed(self.seed)
 
+        tmp_date = atime.Time(self.min_date)
+        tmp_date.format = "gps"
+        self.min_date_gps = tmp_date.value
+
+        tmp_date = atime.Time(self.max_date)
+        tmp_date.format = "gps"
+        self.max_date_gps = tmp_date.value
+
         self.longitude = np.random.uniform(self.long_range[0], self.long_range[1])
         self.latitude = np.random.uniform(self.lat_range[0], self.lat_range[1])
 
         self.fwhm = np.random.uniform(self.fwhm_range[0], self.fwhm_range[1])
 
         self.distance = np.random.uniform(0, 2000)
         self.dist_unc = np.random.normal(240, 80)
```

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/RapidBase.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/RapidBase.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/RapidLco.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/RapidLco.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/RapidSedm.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/RapidSedm.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/SlackSummaryPublisher.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/SlackSummaryPublisher.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/TNSMirrorUpdater.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/TNSMirrorUpdater.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/TransientInfoPrinter.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/TransientInfoPrinter.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/TransientTablePublisher.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/TransientTablePublisher.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # File:                Ampel-contrib-HU/ampel/contrib/hu/t3/TransientTablePublisher.py
 # License:             BSD-3-Clause
 # Author:              jnordin@physik.hu-berlin.de
 # Date:                06.05.2021
-# Last Modified Date:  16.01.2024
-# Last Modified By:    ernstand@physik.hu-berlin.de
+# Last Modified Date:  15.12.2023
+# Last Modified By:    alice.townsend@physik.hu-berlin.de
 
 import io
 import os
 import re
 from collections.abc import Generator
 from typing import Any
 
 import backoff
 import pandas as pd
 import requests
 
 from ampel.abstract.AbsPhotoT3Unit import AbsPhotoT3Unit
 from ampel.secret.NamedSecret import NamedSecret
 from ampel.struct.T3Store import T3Store
-from ampel.types import T3Send
+from ampel.struct.UnitResult import UnitResult
+from ampel.types import T3Send, UBson
 from ampel.util.mappings import get_by_path
 from ampel.view.TransientView import TransientView
+from ampel.ztf.util.ZTFIdMapper import ZTFIdMapper
 
 
 class TransientTablePublisher(AbsPhotoT3Unit):
     """
 
     Construct a table based on selected T2 output values.
     Current output format can be csv or latex.
     Table can optionally saved to a local file or submitted to slack (future: posted to desy web).
 
     Config parameters:
     include_stock (bool)
     include_channels (bool)
 
-    If one wants to convert the AMPEL stock ID to external IDs, define
-    convert_stock_to (str|None)
-    For ZTF-IDs, pass 'convert_stock_to: ztf'
-
     How to deal with names. Will search each transients names for entries containing "value",
     and return any output under "key"
     name_filter = { 'ZTF name' : 'ZTF', 'TNS ID' : 'TNS' }
 
     Selection of fields to save. Matches structure of t2document result dict, e.g.:
     table_schema = { { 't2_unit'  : {
                 'table_label_1' : ['path','to','val'],
@@ -65,59 +63,49 @@
       slack_channel
       slack_token
     local save:
       local_path
 
     Todo:
     - save to desy webb?
-    - include format option for printing
+    - include format option for prointing
 
     """
 
     # Two tables describing what information to save into the table.
     # Schema for state dependent T2s (one row for each)
-    table_schema: dict[str, Any] = {}
+    table_schema: dict[str, Any]
     # Schema for transient dependent T2s (added to each row together with base info)
     transient_table_schema: dict[str, Any]
 
     name_filter: dict[str, str] = {"ZTF name": "ZTF", "TNS ID": "TNS"}
     include_stock: bool = False
-    convert_stock_to: str | None = None
-
-    sort_by_key: str | None = "kilonovaness"
-    sort_ascending: bool = False
-
     include_pos: bool = True
     include_channels: bool = True
     # Add also transients lacking any T2 info
     save_base_info: bool = False
 
     fmt: str = "csv"
-    write_mode: str = "a"
-    rename_files: bool = False
 
-    dir_name: str = "TransientTable"
-    file_name: str = dir_name
+    file_name: str = "TransientTable.csv"
     slack_channel: None | str = None
     slack_token: None | NamedSecret[str]
     local_path: None | str = None
 
-    move_files: bool = True
-
     def process(
-        self, gen: Generator[TransientView, T3Send, None], t3s: None | T3Store = None
-    ) -> None:
+        self, gen: Generator[TransientView, T3Send, None], t3s: T3Store | None = None
+    ) -> UBson | UnitResult:
         #    def process(self, gen: Generator[SnapView, T3Send, None], t3s: T3Store) -> None:
         """
         Loop through provided TransientViews and extract data according to the
         configured schema.
         """
 
         table_rows: list[dict[str, Any]] = []
-        for tran_view in gen:
+        for k, tran_view in enumerate(gen, 1):  # noqa: B007
             basetdict: dict[str, Any] = {}
             # Assemble t2 information bound to the transient (e.g. Point T2s)
             for t2unit, table_entries in self.transient_table_schema.items():
                 # New SnapView has method for directly retrieve result.
                 # Possibly use this.
                 if isinstance(t2res := tran_view.get_latest_t2_body(unit=t2unit), dict):
                     for label, path in table_entries.items():
@@ -161,24 +149,20 @@
                         isinstance((item := basetdict[label]), list | tuple)
                         and len(item) == 1
                     ):
                         basetdict[label] = item[0]
 
             if self.include_stock:
                 basetdict["stock"] = tran_view.id
-
-            if self.convert_stock_to is not None:
-                assert self.convert_stock_to in ["ztf"]
-
-                if self.convert_stock_to == "ztf":
-                    from ampel.ztf.util.ZTFIdMapper import ZTFIdMapper
-
-                    stock_id = tran_view.id
-                    ztf_id = ZTFIdMapper.to_ext_id(stock_id)
-                    basetdict["ztf_id"] = ztf_id
+                # Try to convert to external id
+                # Note: for multiple source classes beyond ZTF, could use a list of tabulator type entries?
+                try:
+                    basetdict["ztfname"] = ZTFIdMapper.to_ext_id(tran_view.id)
+                except ValueError:
+                    self.logger.info("Coult not convert stock")
 
             if self.include_pos:
                 lcurve = tran_view.get_lightcurves()
                 if lcurve is not None:
                     pos = lcurve[0].get_pos(ret="brightest")
                     if pos is not None:
                         basetdict["ra"] = pos[0]
@@ -199,99 +183,35 @@
                     table_rows.append(tdict)
             else:
                 # Only transient info
                 table_rows.append(basetdict)
 
         self.logger.info("", extra={"table_count": len(table_rows)})
         if len(table_rows) == 0:
-            return
+            return None
 
         # Export assembled information
         # Convert
         df = pd.DataFrame.from_dict(table_rows)
 
-        # if "map_name" in df.columns and "map_seed" in df.columns:
-        # df["map_name"] = np.char.replace(np.array(df["map_name"], dtype=str), "random", "random"+df["map_seed"])
-
-        # print(df["map_name"].iloc[0])
-        if "random" in df["map_name"].iloc[0] or self.rename_files:
-            # print("transienttablepublisher:: ", df["map_seed"].iloc[0])
-            tmp_seed_name = df["map_seed"].iloc[0]
-            if isinstance(tmp_seed_name, str):
-                self.file_name += "_" + tmp_seed_name
-            else:
-                self.file_name += "_" + str(int(tmp_seed_name))
-
-        # sort dataframe by key
-        if self.sort_by_key in df.keys():  # noqa: SIM118
-            df = df.sort_values(by=self.sort_by_key, ascending=self.sort_ascending)
-        else:
-            self.logger.warn(
-                f"Cannot sort table by {self.sort_by_key} - legal keys: {df.keys()}"
-            )
-
         # Local save
         if self.local_path is not None:
-            path_name = os.path.join(self.local_path, self.dir_name)
-            # print("PATHNAME::", path_name)
-            if not os.path.exists(path_name):
-                os.makedirs(path_name, exist_ok=True)
-            full_path = os.path.join(path_name, self.file_name)
-            # print("FILE PATH::", full_path)
-
-            with open(full_path + "." + self.fmt, "w") as tmp_file:
-                tmp_file.close()
+            full_path = os.path.join(self.local_path, self.file_name)
             if self.fmt == "csv":
-                # print(self.write_mode)
-                df.to_csv(full_path + ".csv", sep=";", mode=self.write_mode)
+                df.to_csv(full_path)
             elif self.fmt == "latex":
-                df.to_latex(full_path + ".tex")
-            elif self.fmt == "json":
-                json_dumps = df.to_json(indent=2)
-                with open(full_path + ".json", self.write_mode) as json_file:
-                    json_file.write(json_dumps)
-                    json_file.close()
+                df.to_latex(full_path)
             self.logger.info("Exported", extra={"path": full_path})
 
         # Export to slack if requested
         self._slack_export(df)
 
         # Could potentially return a document to T3 collection detailing
         # what was done, as well as the table itself.
-
-        # take everything local_path and put it into new folder named after skymap
-        # print(df.keys)
-        map_name_key = "map_name"
-        if map_name_key in list(df.keys()) and self.move_files:
-            files_local_path = os.listdir(self.local_path)
-            skymap_name = df[map_name_key][
-                0
-            ]  # need to change if for some reason several maps get saved in same file
-            skymap_dir_name = skymap_name  # [: skymap_name.find(".")]  # bare name
-            if skymap_name[-1] != "z":  # if non trivial rev version (hacky)
-                skymap_dir_name += (
-                    "_rev_" + skymap_name[skymap_name.find(",") + 1 :]
-                )  # find "," and add rev version after that
-
-            print("TransientTablePublisher: TMP FILES MOVED TO " + skymap_dir_name)
-
-            if self.local_path is not None:
-                skymap_directory = os.path.join(
-                    self.local_path + "/../" + skymap_dir_name
-                )
-                # print(skymap_directory)
-                os.makedirs(skymap_directory, exist_ok=True)
-                for file in files_local_path:
-                    if file.find(".fits.gz") == -1:
-                        tmp_file_path = os.path.join(self.local_path, file)
-                        if not (os.path.isfile(tmp_file_path)):
-                            continue
-                        os.replace(tmp_file_path, os.path.join(skymap_directory, file))
-
-        return
+        return None
 
     @backoff.on_exception(
         backoff.expo,
         requests.ConnectionError,
         max_tries=5,
         factor=10,
     )
@@ -308,15 +228,15 @@
         """
         if self.slack_channel is None or self.slack_token is None:
             return
 
         # Slack summary
         buffer = io.StringIO(self.file_name)
         if self.fmt == "csv":
-            df.to_csv(buffer, sep=";")
+            df.to_csv(buffer)
         elif self.fmt == "latex":
             df.to_latex(buffer)
 
         param = {
             "token": self.slack_token.get(),
             "channels": self.slack_channel,
             "title": "From the Table Publisher",
```

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/TransientViewDumper.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/TransientViewDumper.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/VOEventPublisher.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/VOEventPublisher.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/complement/BaseCatalogRecordComplementer.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/complement/BaseCatalogRecordComplementer.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/tns/TNSClient.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/tns/TNSClient.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,28 +27,32 @@
 
 
 async def tns_post(
     session: ClientSession,
     semaphore: asyncio.Semaphore,
     method: str,
     token: TNSToken,
-    data: dict,
+    data: dict | int,
+    payload_label: str = "data",
     max_retries: int = 10,
 ) -> dict:
     """
     post to TNS, asynchronously
     """
     async with semaphore:
         for _ in range(max_retries):
             with aiohttp.MultipartWriter("form-data") as mpwriter:
                 p: aiohttp.Payload = aiohttp.StringPayload(token.api_key)
                 p.set_content_disposition("form-data", name="api_key")
                 mpwriter.append(p)
-                p = aiohttp.JsonPayload(data)
-                p.set_content_disposition("form-data", name="data")
+                if isinstance(data, dict):
+                    p = aiohttp.JsonPayload(data)
+                else:
+                    p = aiohttp.StringPayload(str(data))
+                p.set_content_disposition("form-data", name=payload_label)
                 mpwriter.append(p)
                 resp = await session.post(
                     "https://www.wis-tns.org/api/" + method, data=mpwriter
                 )
             if resp.status == 429:
                 wait = max(
                     (
@@ -57,15 +61,16 @@
                         else 0,
                         int(resp.headers.get("x-rate-limit-reset", 0)),
                         1,
                     )
                 )
                 await asyncio.sleep(wait)
                 continue
-            break
+            else:  # noqa: RET507
+                break
         resp.raise_for_status()
         return await resp.json()
 
 
 class TNSClient:
     def __init__(self, token: TNSToken, timeout, maxParallelRequests, logger):
         self.token = token
@@ -108,18 +113,18 @@
             else None
         )
         self.logger.warn("gave up", extra={"exc": err, "tries": details["tries"]})
 
     @staticmethod
     def is_permanent_error(exc):
         if isinstance(exc, ClientResponseError):
-            return exc.code not in {500, 429}
+            return exc.code not in {500, 429, 404}
         return False
 
-    async def search(self, *, exclude: None | set[str] = None, **params):
+    async def search(self, exclude=set(), **params):  # noqa: B006
         semaphore = asyncio.Semaphore(self.maxParallelRequests)
         async with ClientSession(
             headers={
                 "User-Agent": "tns_marker"
                 + json.dumps(
                     {"tns_id": self.token.id, "name": self.token.name, "type": "bot"}
                 )
@@ -143,7 +148,47 @@
                 item = await fut
                 yield item["data"]["reply"]
 
     async def get(self, session, semaphore, objname):
         return await self.tns_post(
             session, semaphore, "get/object", self.token, {"objname": objname}
         )
+
+    async def sendReport(self, report):
+        semaphore = asyncio.Semaphore(self.maxParallelRequests)
+        async with ClientSession(
+            headers={
+                "User-Agent": "tns_marker"
+                + json.dumps(
+                    {"tns_id": self.token.id, "name": self.token.name, "type": "bot"}
+                )
+            },
+        ) as session:
+            postreport = partial(
+                self.tns_post, session, semaphore, "bulk-report", self.token
+            )
+            response = await postreport(report)
+            if response["id_code"] == 200:
+                return response["data"]["report_id"]
+            return False
+
+    async def reportReply(self, report_id):
+        semaphore = asyncio.Semaphore(self.maxParallelRequests)
+        async with ClientSession(
+            headers={
+                "User-Agent": "tns_marker"
+                + json.dumps(
+                    {"tns_id": self.token.id, "name": self.token.name, "type": "bot"}
+                )
+            },
+        ) as session:
+            postreport = partial(
+                self.tns_post,
+                session,
+                semaphore,
+                "bulk-report-reply",
+                self.token,
+                payload_label="report_id",
+            )
+            response = await postreport(report_id)
+
+            return response["data"]["feedback"]
```

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/tns/TNSMirrorDB.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/tns/TNSMirrorDB.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/t3/tns/TNSName.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/t3/tns/TNSName.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/lightcurve.ZTF18abmjvpb.json` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/test/lightcurve.ZTF18abmjvpb.json`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/test_config.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/test/test_config.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/test_slackpublisher.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/test/test_slackpublisher.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/test/test_t2brightsnprob.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/test/test_t2brightsnprob.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/util/AmpelHealpix.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/util/AmpelHealpix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # File:                Ampel-HU-astro/ampel/contrib/hu/util/AmpelHealpix.py
 # License:             BSD-3-Clause
 # Author:              jakob nordin
 # Date:                27.03.2023
-# Last Modified Date:  27.03.2023
-# Last Modified By:    jnordin
+# Last Modified Date:  07.02.2024
+# Last Modified By:    ernstand@physik.hu-berlin.de
 
 
 import math
 import os
 from base64 import b64encode
 from collections import defaultdict
 from datetime import datetime
@@ -44,15 +44,15 @@
         # print(self.map_url)
         if save_dir:
             self.save_dir = save_dir
         self.nside = nside
 
         self._get_map()
         # Attribues
-        self.credible_levels: None | list = None
+        self.credible_levels = np.empty(0)
         self.trigger_time: None | float = None
 
     def _get_map(self, clobber=False) -> int:
         path = os.path.join(self.save_dir, self.map_name)
         # print(path)
         if os.path.exists(path) and not clobber:
             # print("Map exists and found: ", path)
@@ -140,15 +140,15 @@
         Return pixels with total probability up to some limit.
         """
 
         if not self.nside:
             raise ValueError("First get and process map before using.")
 
         # Create mask for pixel selection
-        assert self.credible_levels
+        assert len(self.credible_levels)
         mask = np.zeros(len(self.credible_levels), dtype=int)
         mask[self.credible_levels <= pvalue_limit] = 1
 
         return mask.nonzero()[0].tolist()
 
     def get_maparea(self, pvalue_limit: float) -> float:
         """
@@ -175,15 +175,15 @@
         """
         Obtain probability for a specific coordinate based on loaded map.
         ra, dec in degrees.
         """
 
         if not self.nside:
             raise ValueError("First get and process map before using.")
-        assert self.credible_levels
+        assert len(self.credible_levels)
 
         theta = 0.5 * np.pi - np.deg2rad(dec)
         phi = np.deg2rad(ra)
         alertpix = hp.pixelfunc.ang2pix(
             hp.npix2nside(len(self.credible_levels)), theta, phi, nest=True
         )
         return self.credible_levels[alertpix]
```

### Comparing `ampel_hu_astro-0.8.4a0/ampel/contrib/hu/util/ned.py` & `ampel_hu_astro-0.8.4a1/ampel/contrib/hu/util/ned.py`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/alias.yml` & `ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/alias.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_GP_10.yml` & `ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_GP_10.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_GP_16.yml` & `ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_GP_16.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_GP_59.yml` & `ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_GP_59.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_GP_SINGLE.yml` & `ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_GP_SINGLE.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_NEARBY_CLUSTERS.yml` & `ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_NEARBY_CLUSTERS.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_PARTNER_10.yml` & `ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_PARTNER_10.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_PARTNER_59.yml` & `ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_PARTNER_59.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_RAPID_INFANT.yml` & `ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_RAPID_INFANT.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_RAPID_LANCASTER.yml` & `ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_RAPID_LANCASTER.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_RAPID_SINGLE.yml` & `ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_RAPID_SINGLE.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_TNS_MSIP.yml` & `ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_TNS_MSIP.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/channel/HU_TNS_PARTNER.yml` & `ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/channel/HU_TNS_PARTNER.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/AmpelAutoLco.yml` & `ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/process/AmpelAutoLco.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/ChannelSummary.yml` & `ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/process/ChannelSummary.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/CosmologySummary.yaml` & `ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/process/CosmologySummary.yaml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/DesiSkyportalSNGuess.yml` & `ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/process/DesiSkyportalSNGuess.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/DesiSkyportalSaltSN.yml` & `ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/process/DesiSkyportalSaltSN.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/process/RapidReact.yml` & `ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/process/RapidReact.yml`

 * *Files identical despite different names*

### Comparing `ampel_hu_astro-0.8.4a0/conf/ampel-hu-astro/unit.yml` & `ampel_hu_astro-0.8.4a1/conf/ampel-hu-astro/unit.yml`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 - ampel.contrib.hu.t0.XShooterFilter
 - ampel.contrib.hu.t0.PredetectionFilter
 - ampel.contrib.hu.t0.TransientInClusterFilter
 - ampel.contrib.hu.t0.LensedTransientFilter
 - ampel.contrib.hu.t0.RandFilter
 - ampel.contrib.hu.t0.RcfFilter
 - ampel.contrib.hu.t0.RedshiftCatalogFilter
+- ampel.contrib.hu.t0.StellarFilter
 - ampel.contrib.hu.t2.T2PanStarrThumbPrint
 - ampel.contrib.hu.t2.T2PhaseLimit
 - ampel.contrib.hu.t2.T2PS1ThumbExtCat
 - ampel.contrib.hu.t2.T2PS1ThumbNedSNCosmo
 - ampel.contrib.hu.t2.T2PS1ThumbNedTap
 - ampel.contrib.hu.t2.T2LCQuality
 - ampel.contrib.hu.t2.T2BrightSNProb
@@ -35,31 +36,38 @@
 - ampel.contrib.hu.t2.T2TabulatorRiseDecline
 - ampel.contrib.hu.t2.T2XgbClassifier
 - ampel.contrib.hu.t2.T2MultiXgbClassifier
 - ampel.contrib.hu.t2.T2ElasticcReport
 - ampel.contrib.hu.t2.T2FastDecliner
 - ampel.contrib.hu.t2.T2HealpixProb
 - ampel.contrib.hu.t2.T2KilonovaEval
+- ampel.contrib.hu.t2.T2KilonovaStats
 - ampel.contrib.hu.t2.T2MatchGRB
+- ampel.contrib.hu.t2.T2BaseLightcurveFitter
+- ampel.contrib.hu.t2.T2DemoLightcurveFitter
+- ampel.contrib.hu.t2.T2PolynomialFit
 - ampel.contrib.hu.t3.TransientInfoPrinter
 - ampel.contrib.hu.t3.TransientViewDumper
 - ampel.contrib.hu.t3.ChannelSummaryPublisher
 - ampel.contrib.hu.t3.SlackSummaryPublisher
 - ampel.contrib.hu.t3.RapidBase
 - ampel.contrib.hu.t3.RapidSedm
 - ampel.contrib.hu.t3.RapidLco
-- ampel.contrib.hu.t3.TNSTalker
 - ampel.contrib.hu.t3.TNSMirrorUpdater
 - ampel.contrib.hu.t3.TransientTablePublisher
 - ampel.contrib.hu.t3.HealpixCorrPlotter
 - ampel.contrib.hu.t3.PlotLightcurveSample
 - ampel.contrib.hu.t3.ElasticcClassPublisher
 - ampel.contrib.hu.t3.VOEventPublisher
 - ampel.contrib.hu.t3.AstroColibriPublisher
 - ampel.contrib.hu.t3.HealpixTokenGenerator
 - ampel.contrib.hu.t3.RandomMapGenerator
+- ampel.contrib.hu.t3.AbsScoreCalculator
+- ampel.contrib.hu.t3.CostCounter
+- ampel.contrib.hu.t3.ScoreSingleObject
+- ampel.contrib.hu.t3.ScoreTNSObjects
+- ampel.contrib.hu.t3.PlotTransientLightcurves
+- ampel.contrib.hu.t3.SubmitTNS
 - ampel.contrib.hu.alert.load.WiseFileAlertLoader
 - ampel.contrib.hu.alert.NeoWisePhotometryAlertSupplier
-- ampel.contrib.hu.alert.ResourceDependentConsumer
 - ampel.contrib.hu.alert.DynamicShaperAlertConsumer
 - ampel.contrib.hu.ingest.ZiGWDataPointShaper
-
```

### Comparing `ampel_hu_astro-0.8.4a0/pyproject.toml` & `ampel_hu_astro-0.8.4a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ampel-hu-astro"
-version = "0.8.4a0"
+version = "0.8.4a1"
 license = "BSD-3-Clause"
 readme = "README.md"
 description = "Astronomy units for the Ampel system from HU-Berlin"
 homepage = "https://ampelproject.github.io"
 repository = "https://github.com/AmpelProject/Ampel-HU-astro"
 authors = [
     "Valery Brinnel",
@@ -42,59 +42,72 @@
 iminuit = {version = "^2.8.0", optional = true}
 sfdmap2 = {version = "^0.2.0", optional = true}
 numpy = "^1"
 scipy = ">=1.4"
 beautifulsoup4 = "^4.10.0"
 backoff = "^2"
 requests = "^2.26.0"
-astropy = "^5.0"
-# PyPI prohibits direct dependencies in install_requires
-# see: https://github.com/pypa/pip/issues/6301
-# FIXME: restore pymage when it lands on PyPI
-# pymage = {url = "https://github.com/MickaelRigault/pymage/archive/v1.0.tar.gz#sha256=11e99c4ea06b76ca7fb5b42d1d35d64139a4fa6f7f163a2f0f9cc3ea0b3c55eb"}
-# pymage has an undeclared dependency on pandas
-pandas = "^2.0.0"
+astropy = ">=5.0"
+# pymage never made it to pypi; distribute our own package
+pymage = {version = "^0.5", optional = true, source = "desy-gitlab"}
+pandas = ">=2.0"
 seaborn = "^0.12.0"
-adjustText = "^0.7.3"
+adjustText = "^1.0.0"
 extcats = {version = "^2.4.2", optional = true, source = "pypi"}
 slack-sdk = {version = "^3", optional = true}
 xgboost = {version = "^1.6.2", optional = true}
 astro-parsnip = {version = "^1.4.1", optional = true}
 timeout-decorator = {version = "^0.5", optional = true}
 jupyter = {version = "^1.0.0", optional = true}
 voevent-parse = {version = "^1.0.3", optional = true}
 more-itertools = "^9.0.0"
 uncertainties = "^3.1.7"
 scikit-learn = "^1.1.3"
 healpy = {version = "^1.16.2", optional = true}
-light-curve = {version = "^0.7.3", optional = true}
+light-curve = {version = "^0.7.3"}
 ampel-lsst = {version = ">=0.8.6,<0.9", optional = true}
+ztfquery = {version = "^1.26.1", optional = true}
+ligo-gracedb = {version = "^2.12.0", optional = true}
+astro-datalab = {version = "^2", optional = true}
+# mainline snoopy can't be built as PEP 517 package; use our own distribution
+snpy = {version = "^2.5.3", optional = true, source = "desy-gitlab"}
 
 [tool.poetry.dev-dependencies]
 mypy = "^1.6.1"
-pytest = "^7.4.3"
-pytest-cov = "^4.1.0"
+pytest = "^8.0.2"
+pytest-cov = "^5.0.0"
 pytest-mock = "^3.12.0"
 types-requests = "^2.25.9"
 types-pytz = "^2022.1.2"
+types-pillow = "^10.2.0.20240213"
 # prevent poetry 1.3 from removing setuptools
 setuptools = "*"
 
 [tool.poetry.extras]
-elasticc = ["xgboost", "astro-parsnip", "timeout-decorator", "ampel-lsst", "light-curve"]
+elasticc = ["xgboost", "astro-parsnip", "timeout-decorator", "ampel-lsst"]
 extcats = ["extcats"]
-ligo = ["healpy", "sncosmo", "iminuit", "sfdmap2", "ampel-ztf"]
+ligo = ["healpy", "sncosmo", "iminuit", "sfdmap2", "ampel-ztf", "ligo-gracedb"]
+panstarrs = ["pymage"]
+legacy-surveys = ["astro-datalab"]
 slack = ["slack_sdk"]
 sncosmo = ["sncosmo", "iminuit", "sfdmap2"]
+snpy = ["snpy"]
 notebook = ["jupyter"]
 voevent = ["voevent-parse"]
-ztf = ["ampel-ztf"]
+ztf = ["ampel-ztf", "ztfquery"]
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.13"
+types-pyyaml = "^6.0.12.20240311"
+
+
+[[tool.poetry.source]]
+name = "desy-gitlab"
+url = "https://gitlab.desy.de/api/v4/projects/jakob.van.santen%2Fampel-pypi-demo/packages/pypi/simple"
+priority = "supplemental"
 
 [tool.conda-lock]
 channels = ["conda-forge"]
 platforms = ["linux-64", "osx-64", "osx-arm64"]
 
 [tool.conda-lock.dependencies]
 python-confluent-kafka = "1.7"
@@ -129,28 +142,31 @@
   "sncosmo.*",
   "requests_toolbelt.*",
   "adjustText.*",
   "extcats.*",
   "voeventparse.*",
   "healpy.*",
   "light_curve.*",
+  "ligo.*",
 ]
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 addopts = "--cov=ampel --showlocals -ra"
 
 [tool.black]
 line-length = 88
 
 [tool.ruff]
 target-version = "py310"
 exclude = [
     "ampel/contrib/hu/xgb_trees.py",
-    "notebooks"
+    "notebooks",
+    "scripts",
+    "setup.py",
 ]
 
 [tool.ruff.lint]
 select = [
     "E4",
     "E7",
     "E9",
```

