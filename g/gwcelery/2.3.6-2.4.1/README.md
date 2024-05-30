# Comparing `tmp/gwcelery-2.3.6.tar.gz` & `tmp/gwcelery-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwcelery-2.3.6.tar", max compression
+gzip compressed data, was "gwcelery-2.4.1.tar", max compression
```

## Comparing `gwcelery-2.3.6.tar` & `gwcelery-2.4.1.tar`

### file list

```diff
@@ -1,247 +1,256 @@
--rw-r--r--   0        0        0   108626 2024-04-30 15:22:35.528283 gwcelery-2.3.6/CHANGES.rst
--rw-r--r--   0        0        0       64 2024-04-30 13:33:22.451155 gwcelery-2.3.6/CONTRIBUTING.rst
--rw-r--r--   0        0        0    19716 2024-04-30 13:33:22.452155 gwcelery-2.3.6/LICENSE.rst
--rw-r--r--   0        0        0     1351 2024-04-30 13:33:22.452155 gwcelery-2.3.6/README.rst
--rw-r--r--   0        0        0      634 2024-04-30 13:33:22.452155 gwcelery-2.3.6/doc/Makefile
--rw-r--r--   0        0        0   191486 2024-04-30 13:33:22.453155 gwcelery-2.3.6/doc/_static/acceptance-tests-checklist.png
--rw-r--r--   0        0        0   241593 2024-04-30 13:33:22.454155 gwcelery-2.3.6/doc/_static/celeryevent-screenshot.png
--rw-r--r--   0        0        0   206465 2024-04-30 13:33:22.455155 gwcelery-2.3.6/doc/_static/deployment-screenshot.png
--rw-r--r--   0        0        0   161306 2024-04-30 13:33:22.456155 gwcelery-2.3.6/doc/_static/flask-screenshot.png
--rw-r--r--   0        0        0   328056 2024-04-30 14:56:57.505162 gwcelery-2.3.6/doc/_static/flower-screenshot.png
--rw-r--r--   0        0        0   114719 2024-04-30 13:33:22.458155 gwcelery-2.3.6/doc/_static/logo-0.5x.png
--rw-r--r--   0        0        0   351955 2024-04-30 13:33:22.460155 gwcelery-2.3.6/doc/_static/logo.png
--rw-r--r--   0        0        0   230777 2024-04-30 14:56:57.506162 gwcelery-2.3.6/doc/_static/sentry-screenshot.png
--rwxr-xr-x   0        0        0     7356 2024-04-30 13:33:22.469155 gwcelery-2.3.6/doc/conf.py
--rw-r--r--   0        0        0     4346 2024-04-30 13:33:22.469155 gwcelery-2.3.6/doc/configuration.rst
--rw-r--r--   0        0        0     5698 2024-04-30 13:33:22.469155 gwcelery-2.3.6/doc/contributing.rst
--rw-r--r--   0        0        0    10846 2024-04-30 13:33:22.469155 gwcelery-2.3.6/doc/deployment.rst
--rw-r--r--   0        0        0    10308 2024-04-30 14:56:57.507162 gwcelery-2.3.6/doc/design.rst
--rw-r--r--   0        0        0      563 2024-04-30 13:33:22.469155 gwcelery-2.3.6/doc/gwcelery.conf.rst
--rw-r--r--   0        0        0      284 2024-04-30 13:33:22.469155 gwcelery-2.3.6/doc/gwcelery.email.rst
--rw-r--r--   0        0        0      329 2024-04-30 13:33:22.469155 gwcelery-2.3.6/doc/gwcelery.igwn_alert.rst
--rw-r--r--   0        0        0      227 2024-04-30 13:33:22.470155 gwcelery-2.3.6/doc/gwcelery.rst
--rw-r--r--   0        0        0       79 2024-04-30 13:33:22.470155 gwcelery-2.3.6/doc/gwcelery.sentry.rst
--rw-r--r--   0        0        0       97 2024-04-30 13:33:22.470155 gwcelery-2.3.6/doc/gwcelery.tasks.alerts.rst
--rw-r--r--   0        0        0      103 2024-04-30 13:33:22.470155 gwcelery-2.3.6/doc/gwcelery.tasks.bayestar.rst
--rw-r--r--   0        0        0      107 2024-04-30 13:33:22.470155 gwcelery-2.3.6/doc/gwcelery.tasks.circulars.rst
--rw-r--r--   0        0        0       98 2024-04-30 13:33:22.470155 gwcelery-2.3.6/doc/gwcelery.tasks.condor.rst
--rw-r--r--   0        0        0       91 2024-04-30 13:33:22.470155 gwcelery-2.3.6/doc/gwcelery.tasks.core.rst
--rw-r--r--   0        0        0     2404 2024-04-30 13:33:22.470155 gwcelery-2.3.6/doc/gwcelery.tasks.detchar.rst
--rw-r--r--   0        0        0     1110 2024-04-30 13:33:22.470155 gwcelery-2.3.6/doc/gwcelery.tasks.em_bright.rst
--rw-r--r--   0        0        0      129 2024-04-30 13:33:22.470155 gwcelery-2.3.6/doc/gwcelery.tasks.external_skymaps.rst
--rw-r--r--   0        0        0     9887 2024-04-30 14:56:57.507162 gwcelery-2.3.6/doc/gwcelery.tasks.external_triggers.rst
--rw-r--r--   0        0        0      112 2024-04-30 13:33:22.470155 gwcelery-2.3.6/doc/gwcelery.tasks.first2years.rst
--rw-r--r--   0        0        0      139 2024-04-30 13:33:22.470155 gwcelery-2.3.6/doc/gwcelery.tasks.first2years_external.rst
--rw-r--r--   0        0        0       88 2024-04-30 13:33:22.470155 gwcelery-2.3.6/doc/gwcelery.tasks.gcn.rst
--rw-r--r--   0        0        0      100 2024-04-30 13:33:22.470155 gwcelery-2.3.6/doc/gwcelery.tasks.gracedb.rst
--rw-r--r--   0        0        0      103 2024-04-30 13:33:22.470155 gwcelery-2.3.6/doc/gwcelery.tasks.gwskynet.rst
--rw-r--r--   0        0        0      109 2024-04-30 13:33:22.470155 gwcelery-2.3.6/doc/gwcelery.tasks.igwn_alert.rst
--rw-r--r--   0        0        0      109 2024-04-30 13:33:22.470155 gwcelery-2.3.6/doc/gwcelery.tasks.inference.rst
--rw-r--r--   0        0        0      121 2024-04-30 13:33:22.470155 gwcelery-2.3.6/doc/gwcelery.tasks.legacy_gracedb.rst
--rw-r--r--   0        0        0      112 2024-04-30 13:33:22.470155 gwcelery-2.3.6/doc/gwcelery.tasks.notice_text.rst
--rw-r--r--   0        0        0     8111 2024-04-30 13:33:22.471155 gwcelery-2.3.6/doc/gwcelery.tasks.orchestrator.rst
--rw-r--r--   0        0        0      100 2024-04-30 13:33:22.471155 gwcelery-2.3.6/doc/gwcelery.tasks.p_astro.rst
--rw-r--r--   0        0        0     2385 2024-04-30 13:33:22.471155 gwcelery-2.3.6/doc/gwcelery.tasks.raven.rst
--rw-r--r--   0        0        0      106 2024-04-30 13:33:22.471155 gwcelery-2.3.6/doc/gwcelery.tasks.rrt_utils.rst
--rw-r--r--   0        0        0      814 2024-04-30 13:33:22.471155 gwcelery-2.3.6/doc/gwcelery.tasks.rst
--rw-r--r--   0        0        0      100 2024-04-30 13:33:22.471155 gwcelery-2.3.6/doc/gwcelery.tasks.skymaps.rst
--rw-r--r--   0        0        0     7161 2024-04-30 13:33:22.471155 gwcelery-2.3.6/doc/gwcelery.tasks.superevents.rst
--rw-r--r--   0        0        0       97 2024-04-30 13:33:22.471155 gwcelery-2.3.6/doc/gwcelery.tools.condor.rst
--rw-r--r--   0        0        0       94 2024-04-30 13:33:22.471155 gwcelery-2.3.6/doc/gwcelery.tools.flask.rst
--rw-r--r--   0        0        0       97 2024-04-30 13:33:22.471155 gwcelery-2.3.6/doc/gwcelery.tools.nagios.rst
--rw-r--r--   0        0        0      185 2024-04-30 13:33:22.471155 gwcelery-2.3.6/doc/gwcelery.tools.rst
--rw-r--r--   0        0        0       73 2024-04-30 13:33:22.471155 gwcelery-2.3.6/doc/gwcelery.util.rst
--rw-r--r--   0        0        0      507 2024-04-30 13:33:22.471155 gwcelery-2.3.6/doc/gwcelery.voevent.rst
--rw-r--r--   0        0        0     3564 2024-04-30 13:33:22.471155 gwcelery-2.3.6/doc/htcondor.rst
--rw-r--r--   0        0        0     1576 2024-04-30 13:33:22.471155 gwcelery-2.3.6/doc/index.rst
--rw-r--r--   0        0        0      800 2024-04-30 13:33:22.471155 gwcelery-2.3.6/doc/make.bat
--rw-r--r--   0        0        0     5541 2024-04-30 14:56:57.507162 gwcelery-2.3.6/doc/monitoring.rst
--rw-r--r--   0        0        0     5405 2024-04-30 13:33:22.472155 gwcelery-2.3.6/doc/quickstart.rst
--rw-r--r--   0        0        0     1097 2024-04-30 13:33:22.472155 gwcelery-2.3.6/gwcelery/__init__.py
--rw-r--r--   0        0        0    18447 2024-04-30 13:33:22.472155 gwcelery-2.3.6/gwcelery/_version.py
--rw-r--r--   0        0        0    19512 2024-04-30 14:56:57.507162 gwcelery-2.3.6/gwcelery/conf/__init__.py
--rw-r--r--   0        0        0     1195 2024-04-30 13:33:22.472155 gwcelery-2.3.6/gwcelery/conf/dev.py
--rw-r--r--   0        0        0     1180 2024-04-30 13:33:22.472155 gwcelery-2.3.6/gwcelery/conf/minikube.py
--rw-r--r--   0        0        0     2178 2024-04-30 13:33:22.472155 gwcelery-2.3.6/gwcelery/conf/playground.py
--rw-r--r--   0        0        0     3687 2024-04-30 13:33:22.472155 gwcelery-2.3.6/gwcelery/conf/production.py
--rw-r--r--   0        0        0     2040 2024-04-30 13:33:22.472155 gwcelery-2.3.6/gwcelery/conf/test.py
--rw-r--r--   0        0        0        0 2024-04-30 15:23:15.824382 gwcelery-2.3.6/gwcelery/data/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 15:23:15.824382 gwcelery-2.3.6/gwcelery/data/first2years/__init__.py
--rw-r--r--   0        0        0   731421 2024-04-30 13:33:22.475155 gwcelery-2.3.6/gwcelery/data/first2years/gstlal.xml.gz
--rwxr-xr-x   0        0        0     3199 2024-04-30 13:33:22.475155 gwcelery-2.3.6/gwcelery/data/gwcelery.sub
--rw-r--r--   0        0        0      505 2024-04-30 13:33:22.475155 gwcelery-2.3.6/gwcelery/email/__init__.py
--rw-r--r--   0        0        0     3317 2024-04-30 14:56:57.507162 gwcelery-2.3.6/gwcelery/email/bootsteps.py
--rw-r--r--   0        0        0      995 2024-04-30 13:33:22.475155 gwcelery-2.3.6/gwcelery/email/signals.py
--rw-r--r--   0        0        0     1457 2024-04-30 13:33:22.475155 gwcelery-2.3.6/gwcelery/flask.py
--rw-r--r--   0        0        0      529 2024-04-30 13:33:22.475155 gwcelery-2.3.6/gwcelery/igwn_alert/__init__.py
--rw-r--r--   0        0        0     4484 2024-04-30 13:33:22.475155 gwcelery-2.3.6/gwcelery/igwn_alert/bootsteps.py
--rw-r--r--   0        0        0      608 2024-04-30 13:33:22.475155 gwcelery-2.3.6/gwcelery/igwn_alert/signals.py
--rw-r--r--   0        0        0      275 2024-04-30 13:33:22.475155 gwcelery-2.3.6/gwcelery/jinja.py
--rw-r--r--   0        0        0      305 2024-04-30 13:33:22.475155 gwcelery-2.3.6/gwcelery/kafka/__init__.py
--rw-r--r--   0        0        0    11839 2024-04-30 13:33:22.476155 gwcelery-2.3.6/gwcelery/kafka/bootsteps.py
--rw-r--r--   0        0        0      522 2024-04-30 13:33:22.476155 gwcelery-2.3.6/gwcelery/kafka/signals.py
--rw-r--r--   0        0        0     2567 2024-04-30 13:33:22.476155 gwcelery-2.3.6/gwcelery/sentry/__init__.py
--rw-r--r--   0        0        0       34 2024-04-30 13:33:22.476155 gwcelery-2.3.6/gwcelery/sentry/integrations/__init__.py
--rw-r--r--   0        0        0      832 2024-04-30 13:33:22.476155 gwcelery-2.3.6/gwcelery/sentry/integrations/condor.py
--rw-r--r--   0        0        0      836 2024-04-30 13:33:22.476155 gwcelery-2.3.6/gwcelery/sentry/integrations/requests.py
--rw-r--r--   0        0        0      939 2024-04-30 13:33:22.476155 gwcelery-2.3.6/gwcelery/sentry/integrations/subprocess.py
--rw-r--r--   0        0        0     1302 2024-04-30 13:33:22.476155 gwcelery-2.3.6/gwcelery/static/typeahead.css
--rw-r--r--   0        0        0     4124 2024-04-30 13:33:22.476155 gwcelery-2.3.6/gwcelery/static/vega/index.html
--rw-r--r--   0        0        0      515 2024-04-30 13:33:22.476155 gwcelery-2.3.6/gwcelery/tasks/__init__.py
--rw-r--r--   0        0        0    14457 2024-04-30 13:33:22.476155 gwcelery-2.3.6/gwcelery/tasks/alerts.py
--rw-r--r--   0        0        0     2540 2024-04-30 13:33:22.476155 gwcelery-2.3.6/gwcelery/tasks/bayestar.py
--rw-r--r--   0        0        0     1892 2024-04-30 13:33:22.476155 gwcelery-2.3.6/gwcelery/tasks/circulars.py
--rw-r--r--   0        0        0     7552 2024-04-30 13:33:22.477155 gwcelery-2.3.6/gwcelery/tasks/condor.py
--rw-r--r--   0        0        0     2692 2024-04-30 13:33:22.477155 gwcelery-2.3.6/gwcelery/tasks/core.py
--rw-r--r--   0        0        0    23090 2024-04-30 13:33:22.477155 gwcelery-2.3.6/gwcelery/tasks/detchar.py
--rw-r--r--   0        0        0     4903 2024-04-30 13:33:22.477155 gwcelery-2.3.6/gwcelery/tasks/em_bright.py
--rw-r--r--   0        0        0    29615 2024-04-30 14:56:57.508162 gwcelery-2.3.6/gwcelery/tasks/external_skymaps.py
--rw-r--r--   0        0        0    31983 2024-04-30 14:56:57.508162 gwcelery-2.3.6/gwcelery/tasks/external_triggers.py
--rw-r--r--   0        0        0     6841 2024-04-30 13:33:22.478155 gwcelery-2.3.6/gwcelery/tasks/first2years.py
--rw-r--r--   0        0        0    10693 2024-04-30 14:56:57.508162 gwcelery-2.3.6/gwcelery/tasks/first2years_external.py
--rw-r--r--   0        0        0     4832 2024-04-30 13:33:22.478155 gwcelery-2.3.6/gwcelery/tasks/gcn.py
--rw-r--r--   0        0        0    11080 2024-04-30 14:56:57.508162 gwcelery-2.3.6/gwcelery/tasks/gracedb.py
--rw-r--r--   0        0        0     6884 2024-04-30 13:33:22.478155 gwcelery-2.3.6/gwcelery/tasks/gwskynet.py
--rw-r--r--   0        0        0     2453 2024-04-30 13:33:22.478155 gwcelery-2.3.6/gwcelery/tasks/igwn_alert.py
--rw-r--r--   0        0        0    34985 2024-04-30 14:56:57.508162 gwcelery-2.3.6/gwcelery/tasks/inference.py
--rw-r--r--   0        0        0     1407 2024-04-30 13:33:22.478155 gwcelery-2.3.6/gwcelery/tasks/legacy_gracedb.py
--rw-r--r--   0        0        0     8556 2024-04-30 13:33:22.479155 gwcelery-2.3.6/gwcelery/tasks/notice_text.py
--rw-r--r--   0        0        0    57527 2024-04-30 13:33:22.479155 gwcelery-2.3.6/gwcelery/tasks/orchestrator.py
--rw-r--r--   0        0        0     5847 2024-04-30 13:33:22.479155 gwcelery-2.3.6/gwcelery/tasks/p_astro.py
--rw-r--r--   0        0        0    24536 2024-04-30 13:33:22.479155 gwcelery-2.3.6/gwcelery/tasks/raven.py
--rw-r--r--   0        0        0     2264 2024-04-30 13:33:22.479155 gwcelery-2.3.6/gwcelery/tasks/rrt_utils.py
--rw-r--r--   0        0        0     9510 2024-04-30 13:33:22.479155 gwcelery-2.3.6/gwcelery/tasks/skymaps.py
--rw-r--r--   0        0        0    25166 2024-04-30 13:33:22.479155 gwcelery-2.3.6/gwcelery/tasks/superevents.py
--rw-r--r--   0        0        0     1084 2024-04-30 13:33:22.480155 gwcelery-2.3.6/gwcelery/templates/fits_header.jinja2
--rw-r--r--   0        0        0    41294 2024-04-30 13:33:22.480155 gwcelery-2.3.6/gwcelery/templates/index.jinja2
--rw-r--r--   0        0        0     8505 2024-04-30 13:33:22.480155 gwcelery-2.3.6/gwcelery/templates/lalinference.jinja2
--rw-r--r--   0        0        0     9473 2024-04-30 13:33:22.480155 gwcelery-2.3.6/gwcelery/templates/rapidpe.jinja2
--rw-r--r--   0        0        0      472 2024-04-30 13:33:22.480155 gwcelery-2.3.6/gwcelery/templates/vector_table.jinja2
--rw-r--r--   0        0        0        0 2024-04-30 15:23:15.826382 gwcelery-2.3.6/gwcelery/tests/__init__.py
--rw-r--r--   0        0        0     4388 2024-04-30 13:33:22.480155 gwcelery-2.3.6/gwcelery/tests/conftest.py
--rw-r--r--   0        0        0      976 2024-04-30 13:33:22.480155 gwcelery-2.3.6/gwcelery/tests/data/G000012_S0040_preferred.json
--rw-r--r--   0        0        0     6258 2024-04-30 13:33:22.480155 gwcelery-2.3.6/gwcelery/tests/data/G298048-1-Initial.xml
--rw-r--r--   0        0        0      599 2024-04-30 13:33:22.481155 gwcelery-2.3.6/gwcelery/tests/data/G298048_log.json
--rw-r--r--   0        0        0      150 2024-04-30 13:33:22.481155 gwcelery-2.3.6/gwcelery/tests/data/H1L1V1-mean_counts-1126051217-61603201.json
--rw-r--r--   0        0        0      974 2024-04-30 13:33:22.481155 gwcelery-2.3.6/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json
--rw-r--r--   0        0        0    17572 2024-04-30 13:33:22.481155 gwcelery-2.3.6/gwcelery/tests/data/MS220722v.json
--rw-r--r--   0        0        0   777600 2024-04-30 13:33:22.485155 gwcelery-2.3.6/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits
--rw-r--r--   0        0        0     8232 2024-04-30 13:33:22.485155 gwcelery-2.3.6/gwcelery/tests/data/S230413b.json
--rw-r--r--   0        0        0     7255 2024-04-30 13:33:22.485155 gwcelery-2.3.6/gwcelery/tests/data/S230413g.json
--rw-r--r--   0        0        0     7721 2024-04-30 13:33:22.485155 gwcelery-2.3.6/gwcelery/tests/data/S230413h.json
--rw-r--r--   0        0        0     3387 2024-04-30 13:33:22.485155 gwcelery-2.3.6/gwcelery/tests/data/T0212_S0039_preferred.json
--rw-r--r--   0        0        0     3384 2024-04-30 13:33:22.485155 gwcelery-2.3.6/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json
--rw-r--r--   0        0        0     5210 2024-04-30 13:33:22.485155 gwcelery-2.3.6/gwcelery/tests/data/T0219_S0041_nopreferred.json
--rw-r--r--   0        0        0        0 2024-04-30 15:23:15.827382 gwcelery-2.3.6/gwcelery/tests/data/__init__.py
--rw-r--r--   0        0        0     2290 2024-04-30 14:56:57.509162 gwcelery-2.3.6/gwcelery/tests/data/agile_grb_gcn.xml
--rw-r--r--   0        0        0   854036 2024-04-30 13:33:22.489155 gwcelery-2.3.6/gwcelery/tests/data/coinc.xml
--rw-r--r--   0        0        0     6175 2024-04-30 13:33:22.490155 gwcelery-2.3.6/gwcelery/tests/data/externaltrigger_original_data.xml
--rw-r--r--   0        0        0     5482 2024-04-30 13:33:22.490155 gwcelery-2.3.6/gwcelery/tests/data/fermi_grb_gcn.xml
--rw-r--r--   0        0        0     5469 2024-04-30 13:33:22.490155 gwcelery-2.3.6/gwcelery/tests/data/fermi_initial_grb_gcn.xml
--rw-r--r--   0        0        0     5865 2024-04-30 13:33:22.490155 gwcelery-2.3.6/gwcelery/tests/data/fermi_noise_gcn.xml
--rw-r--r--   0        0        0     5864 2024-04-30 13:33:22.490155 gwcelery-2.3.6/gwcelery/tests/data/fermi_noise_gcn_2.xml
--rw-r--r--   0        0        0     1922 2024-04-30 13:33:22.490155 gwcelery-2.3.6/gwcelery/tests/data/fermi_subgrbtargeted_template.xml
--rw-r--r--   0        0        0     4914 2024-04-30 13:33:22.490155 gwcelery-2.3.6/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml
--rw-r--r--   0        0        0     4914 2024-04-30 13:33:22.490155 gwcelery-2.3.6/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml
--rw-r--r--   0        0        0     3407 2024-04-30 13:33:22.490155 gwcelery-2.3.6/gwcelery/tests/data/fits_header_result.html
--rw-r--r--   0        0        0      882 2024-04-30 13:33:22.490155 gwcelery-2.3.6/gwcelery/tests/data/gracedb_externaltrigger_log.json
--rw-r--r--   0        0        0      446 2024-04-30 13:33:22.490155 gwcelery-2.3.6/gwcelery/tests/data/gracedb_setrigger_log.json
--rw-r--r--   0        0        0      870 2024-04-30 13:33:22.490155 gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_detchar.json
--rw-r--r--   0        0        0     2025 2024-04-30 13:33:22.490155 gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_exttrig_creation.json
--rw-r--r--   0        0        0     2007 2024-04-30 13:33:22.490155 gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json
--rw-r--r--   0        0        0      166 2024-04-30 13:33:22.490155 gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_fits.json
--rw-r--r--   0        0        0      101 2024-04-30 13:33:22.490155 gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_label_dqv.json
--rw-r--r--   0        0        0      743 2024-04-30 13:33:22.491155 gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_psd.json
--rw-r--r--   0        0        0     2020 2024-04-30 13:33:22.491155 gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_snews_creation.json
--rw-r--r--   0        0        0     2012 2024-04-30 13:33:22.491155 gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_snews_test_creation.json
--rw-r--r--   0        0        0     2028 2024-04-30 13:33:22.491155 gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_subgrb_creation.json
--rw-r--r--   0        0        0     1235 2024-04-30 13:33:22.491155 gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_superevent_creation.json
--rw-r--r--   0        0        0      107 2024-04-30 13:33:22.491155 gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_superevent_label.json
--rw-r--r--   0        0        0     5021 2024-04-30 13:33:22.491155 gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_voevent.json
--rw-r--r--   0        0        0     4429 2024-04-30 13:33:22.491155 gwcelery-2.3.6/gwcelery/tests/data/integral_grb_gcn.xml
--rw-r--r--   0        0        0     4295 2024-04-30 13:33:22.491155 gwcelery-2.3.6/gwcelery/tests/data/integral_mdc_gcn.xml
--rw-r--r--   0        0        0     4451 2024-04-30 13:33:22.491155 gwcelery-2.3.6/gwcelery/tests/data/integral_test_gcn.xml
--rw-r--r--   0        0        0  1038044 2024-04-30 13:33:22.497155 gwcelery-2.3.6/gwcelery/tests/data/kafka_alert_fermi.json
--rw-r--r--   0        0        0  1038042 2024-04-30 13:33:22.499155 gwcelery-2.3.6/gwcelery/tests/data/kafka_alert_fermi_ignore.json
--rw-r--r--   0        0        0      806 2024-04-30 13:33:22.499155 gwcelery-2.3.6/gwcelery/tests/data/kafka_alert_swift.json
--rw-r--r--   0        0        0      743 2024-04-30 13:33:22.499155 gwcelery-2.3.6/gwcelery/tests/data/kafka_alert_swift_noloc.json
--rw-r--r--   0        0        0  1037630 2024-04-30 13:33:22.500155 gwcelery-2.3.6/gwcelery/tests/data/kafka_alert_swift_wskymap.json
--rw-r--r--   0        0        0        0 2024-04-30 15:23:15.828382 gwcelery-2.3.6/gwcelery/tests/data/llhoft/__init__.py
--rw-r--r--   0        0        0     8267 2024-04-30 13:33:22.501155 gwcelery-2.3.6/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2024-04-30 15:23:15.828382 gwcelery-2.3.6/gwcelery/tests/data/llhoft/fail/L1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 15:23:15.828382 gwcelery-2.3.6/gwcelery/tests/data/llhoft/fail/__init__.py
--rw-r--r--   0        0        0    14942 2024-04-30 13:33:22.501155 gwcelery-2.3.6/gwcelery/tests/data/llhoft/idqbad/H1/H-H1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2024-04-30 15:23:15.828382 gwcelery-2.3.6/gwcelery/tests/data/llhoft/omegascan/__init__.py
--rw-r--r--   0        0        0   516419 2024-04-30 13:33:22.502155 gwcelery-2.3.6/gwcelery/tests/data/llhoft/omegascan/scanme.gwf
--rw-r--r--   0        0        0    14950 2024-04-30 13:33:22.503155 gwcelery-2.3.6/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2024-04-30 15:23:15.828382 gwcelery-2.3.6/gwcelery/tests/data/llhoft/pass/H1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 15:23:15.828382 gwcelery-2.3.6/gwcelery/tests/data/llhoft/pass/__init__.py
--rw-r--r--   0        0        0    13099 2024-04-30 13:33:22.503155 gwcelery-2.3.6/gwcelery/tests/data/lvalert_event_creation.json
--rw-r--r--   0        0        0     9060 2024-04-30 13:33:22.503155 gwcelery-2.3.6/gwcelery/tests/data/lvalert_xmpp.xml
--rw-r--r--   0        0        0      864 2024-04-30 13:33:22.503155 gwcelery-2.3.6/gwcelery/tests/data/mock_superevent_object.json
--rw-r--r--   0        0        0   445440 2024-04-30 13:33:22.504155 gwcelery-2.3.6/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite
--rw-r--r--   0        0        0   294426 2024-04-30 13:33:22.505155 gwcelery-2.3.6/gwcelery/tests/data/psd.xml.gz
--rw-r--r--   0        0        0    11520 2024-04-30 13:33:22.505155 gwcelery-2.3.6/gwcelery/tests/data/rrt_small_area.fits
--rw-r--r--   0        0        0     2961 2024-04-30 13:33:22.505155 gwcelery-2.3.6/gwcelery/tests/data/sample_events.json
--rw-r--r--   0        0        0     3648 2024-04-30 13:33:22.505155 gwcelery-2.3.6/gwcelery/tests/data/samples.hdf5
--rw-r--r--   0        0        0      616 2024-04-30 13:33:22.505155 gwcelery-2.3.6/gwcelery/tests/data/scaler_set_all.pickle
--rw-r--r--   0        0        0     6169 2024-04-30 13:33:22.506155 gwcelery-2.3.6/gwcelery/tests/data/snews_gcn.xml
--rw-r--r--   0        0        0     6161 2024-04-30 13:33:22.506155 gwcelery-2.3.6/gwcelery/tests/data/snews_gcn_test.xml
--rw-r--r--   0        0        0     9583 2024-04-30 13:33:22.506155 gwcelery-2.3.6/gwcelery/tests/data/superevents.json
--rw-r--r--   0        0        0     7713 2024-04-30 13:33:22.506155 gwcelery-2.3.6/gwcelery/tests/data/swift_grb_gcn.xml
--rw-r--r--   0        0        0     1970 2024-04-30 13:33:22.506155 gwcelery-2.3.6/gwcelery/tests/data/swift_subgrbtargeted_template.xml
--rw-r--r--   0        0        0   581918 2024-04-30 13:33:22.508155 gwcelery-2.3.6/gwcelery/tests/data/test_classifier.pickle
--rw-r--r--   0        0        0      122 2024-04-30 13:33:22.508155 gwcelery-2.3.6/gwcelery/tests/data/updated_RapidPE_RIFT.p_astro.json
--rw-r--r--   0        0        0     4063 2024-04-30 13:33:22.508155 gwcelery-2.3.6/gwcelery/tests/process.py
--rw-r--r--   0        0        0     2307 2024-04-30 13:33:22.508155 gwcelery-2.3.6/gwcelery/tests/test_sentry.py
--rw-r--r--   0        0        0     1669 2024-04-30 13:33:22.508155 gwcelery-2.3.6/gwcelery/tests/test_tasks_alerts.py
--rw-r--r--   0        0        0     4815 2024-04-30 13:33:22.508155 gwcelery-2.3.6/gwcelery/tests/test_tasks_alerts_validate.py
--rw-r--r--   0        0        0     1428 2024-04-30 13:33:22.508155 gwcelery-2.3.6/gwcelery/tests/test_tasks_bayestar.py
--rw-r--r--   0        0        0     3172 2024-04-30 13:33:22.508155 gwcelery-2.3.6/gwcelery/tests/test_tasks_circulars.py
--rw-r--r--   0        0        0     4550 2024-04-30 13:33:22.509155 gwcelery-2.3.6/gwcelery/tests/test_tasks_condor.py
--rw-r--r--   0        0        0    17285 2024-04-30 13:33:22.509155 gwcelery-2.3.6/gwcelery/tests/test_tasks_detchar.py
--rw-r--r--   0        0        0     2317 2024-04-30 13:33:22.509155 gwcelery-2.3.6/gwcelery/tests/test_tasks_em_bright.py
--rw-r--r--   0        0        0    17442 2024-04-30 13:33:22.509155 gwcelery-2.3.6/gwcelery/tests/test_tasks_external_skymaps.py
--rw-r--r--   0        0        0    42927 2024-04-30 14:56:57.509162 gwcelery-2.3.6/gwcelery/tests/test_tasks_external_triggers.py
--rw-r--r--   0        0        0     1797 2024-04-30 13:33:22.509155 gwcelery-2.3.6/gwcelery/tests/test_tasks_first2years.py
--rw-r--r--   0        0        0     7026 2024-04-30 13:33:22.509155 gwcelery-2.3.6/gwcelery/tests/test_tasks_first2years_external.py
--rw-r--r--   0        0        0     1815 2024-04-30 13:33:22.509155 gwcelery-2.3.6/gwcelery/tests/test_tasks_gcn.py
--rw-r--r--   0        0        0     1616 2024-04-30 13:33:22.510155 gwcelery-2.3.6/gwcelery/tests/test_tasks_gcn_validate.py
--rw-r--r--   0        0        0     5728 2024-04-30 13:33:22.510155 gwcelery-2.3.6/gwcelery/tests/test_tasks_gracedb.py
--rw-r--r--   0        0        0     9664 2024-04-30 13:33:22.510155 gwcelery-2.3.6/gwcelery/tests/test_tasks_gwskynet.py
--rw-r--r--   0        0        0     3676 2024-04-30 13:33:22.510155 gwcelery-2.3.6/gwcelery/tests/test_tasks_igwn_alert.py
--rw-r--r--   0        0        0    28978 2024-04-30 14:56:57.510162 gwcelery-2.3.6/gwcelery/tests/test_tasks_inference.py
--rw-r--r--   0        0        0    57191 2024-04-30 13:33:22.510155 gwcelery-2.3.6/gwcelery/tests/test_tasks_orchestrator.py
--rw-r--r--   0        0        0     1647 2024-04-30 13:33:22.510155 gwcelery-2.3.6/gwcelery/tests/test_tasks_p_astro.py
--rw-r--r--   0        0        0    28405 2024-04-30 14:56:57.510162 gwcelery-2.3.6/gwcelery/tests/test_tasks_raven.py
--rw-r--r--   0        0        0     4696 2024-04-30 13:33:22.511155 gwcelery-2.3.6/gwcelery/tests/test_tasks_rrt_utils.py
--rw-r--r--   0        0        0     5520 2024-04-30 13:33:22.511155 gwcelery-2.3.6/gwcelery/tests/test_tasks_skymaps.py
--rw-r--r--   0        0        0    50557 2024-04-30 13:33:22.511155 gwcelery-2.3.6/gwcelery/tests/test_tasks_superevents.py
--rw-r--r--   0        0        0      637 2024-04-30 13:33:22.511155 gwcelery-2.3.6/gwcelery/tests/test_tempfile.py
--rw-r--r--   0        0        0     3520 2024-04-30 13:33:22.511155 gwcelery-2.3.6/gwcelery/tests/test_tools_condor.py
--rw-r--r--   0        0        0     1098 2024-04-30 13:33:22.511155 gwcelery-2.3.6/gwcelery/tests/test_tools_condor_submit_helper.py
--rw-r--r--   0        0        0      647 2024-04-30 13:33:22.511155 gwcelery-2.3.6/gwcelery/tests/test_tools_flask.py
--rw-r--r--   0        0        0    11271 2024-04-30 13:33:22.511155 gwcelery-2.3.6/gwcelery/tests/test_tools_nagios.py
--rw-r--r--   0        0        0      269 2024-04-30 13:33:22.511155 gwcelery-2.3.6/gwcelery/tests/test_util.py
--rw-r--r--   0        0        0    25205 2024-04-30 13:33:22.512155 gwcelery-2.3.6/gwcelery/tests/test_views.py
--rw-r--r--   0        0        0      216 2024-04-30 13:33:22.512155 gwcelery-2.3.6/gwcelery/tools/__init__.py
--rw-r--r--   0        0        0     2941 2024-04-30 13:33:22.512155 gwcelery-2.3.6/gwcelery/tools/condor.py
--rw-r--r--   0        0        0     1120 2024-04-30 13:33:22.512155 gwcelery-2.3.6/gwcelery/tools/condor_submit_helper.py
--rw-r--r--   0        0        0     1938 2024-04-30 13:33:22.512155 gwcelery-2.3.6/gwcelery/tools/flask.py
--rw-r--r--   0        0        0     9145 2024-04-30 13:33:22.512155 gwcelery-2.3.6/gwcelery/tools/nagios.py
--rw-r--r--   0        0        0      413 2024-04-30 13:33:22.512155 gwcelery-2.3.6/gwcelery/util/__init__.py
--rw-r--r--   0        0        0     1007 2024-04-30 13:33:22.512155 gwcelery-2.3.6/gwcelery/util/cmdline.py
--rw-r--r--   0        0        0      453 2024-04-30 13:33:22.512155 gwcelery-2.3.6/gwcelery/util/matplotlib.py
--rw-r--r--   0        0        0      390 2024-04-30 13:33:22.512155 gwcelery-2.3.6/gwcelery/util/proxy.py
--rw-r--r--   0        0        0      585 2024-04-30 13:33:22.512155 gwcelery-2.3.6/gwcelery/util/resources.py
--rw-r--r--   0        0        0      253 2024-04-30 13:33:22.512155 gwcelery-2.3.6/gwcelery/util/sphinx.py
--rw-r--r--   0        0        0      941 2024-04-30 13:33:22.512155 gwcelery-2.3.6/gwcelery/util/tempfile.py
--rw-r--r--   0        0        0    21881 2024-04-30 13:33:22.513155 gwcelery-2.3.6/gwcelery/views.py
--rw-r--r--   0        0        0      365 2024-04-30 13:33:22.513155 gwcelery-2.3.6/gwcelery/voevent/__init__.py
--rw-r--r--   0        0        0     6388 2024-04-30 13:33:22.513155 gwcelery-2.3.6/gwcelery/voevent/bootsteps.py
--rw-r--r--   0        0        0     1063 2024-04-30 13:33:22.513155 gwcelery-2.3.6/gwcelery/voevent/logging.py
--rw-r--r--   0        0        0      779 2024-04-30 13:33:22.513155 gwcelery-2.3.6/gwcelery/voevent/signals.py
--rw-r--r--   0        0        0      884 2024-04-30 13:33:22.513155 gwcelery-2.3.6/gwcelery/voevent/subscriber.py
--rw-r--r--   0        0        0     1454 2024-04-30 13:33:22.513155 gwcelery-2.3.6/gwcelery/voevent/util.py
--rw-r--r--   0        0        0     6619 2024-04-30 15:23:24.765404 gwcelery-2.3.6/pyproject.toml
--rw-r--r--   0        0        0     4680 1970-01-01 00:00:00.000000 gwcelery-2.3.6/PKG-INFO
+-rw-r--r--   0        0        0   110112 2024-05-30 21:50:59.530844 gwcelery-2.4.1/CHANGES.rst
+-rw-r--r--   0        0        0       64 2024-05-30 15:37:19.397924 gwcelery-2.4.1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0    19716 2024-05-30 15:37:19.398923 gwcelery-2.4.1/LICENSE.rst
+-rw-r--r--   0        0        0     1351 2024-05-30 15:37:19.398923 gwcelery-2.4.1/README.rst
+-rw-r--r--   0        0        0      634 2024-05-30 15:37:19.398923 gwcelery-2.4.1/doc/Makefile
+-rw-r--r--   0        0        0   191486 2024-05-30 15:37:19.401924 gwcelery-2.4.1/doc/_static/acceptance-tests-checklist.png
+-rw-r--r--   0        0        0    28822 2024-05-30 15:37:19.401924 gwcelery-2.4.1/doc/_static/celery-log-screenshot.png
+-rw-r--r--   0        0        0   241593 2024-05-30 15:37:19.403924 gwcelery-2.4.1/doc/_static/celeryevent-screenshot.png
+-rw-r--r--   0        0        0   191960 2024-05-30 15:37:19.405924 gwcelery-2.4.1/doc/_static/condor-queue.png
+-rw-r--r--   0        0        0   206465 2024-05-30 15:37:19.406924 gwcelery-2.4.1/doc/_static/deployment-screenshot.png
+-rw-r--r--   0        0        0    37453 2024-05-30 15:37:19.407924 gwcelery-2.4.1/doc/_static/disk-usage-screenshot.png
+-rw-r--r--   0        0        0    34244 2024-05-30 15:37:19.407924 gwcelery-2.4.1/doc/_static/emfollow-login.png
+-rw-r--r--   0        0        0   161306 2024-05-30 15:37:19.408924 gwcelery-2.4.1/doc/_static/flask-screenshot.png
+-rw-r--r--   0        0        0   104212 2024-05-30 15:37:19.409924 gwcelery-2.4.1/doc/_static/flower-screenshot.png
+-rw-r--r--   0        0        0   236545 2024-05-30 15:37:19.411924 gwcelery-2.4.1/doc/_static/ganglia-screenshot.png
+-rw-r--r--   0        0        0   193945 2024-05-30 15:37:19.412924 gwcelery-2.4.1/doc/_static/issue-screenshot.png
+-rw-r--r--   0        0        0   114719 2024-05-30 15:37:19.413924 gwcelery-2.4.1/doc/_static/logo-0.5x.png
+-rw-r--r--   0        0        0   351955 2024-05-30 15:37:19.416924 gwcelery-2.4.1/doc/_static/logo.png
+-rw-r--r--   0        0        0   191782 2024-05-30 15:37:19.417924 gwcelery-2.4.1/doc/_static/munin-screenshot.png
+-rw-r--r--   0        0        0   391620 2024-05-30 15:37:19.420924 gwcelery-2.4.1/doc/_static/nagios-screenshot.png
+-rw-r--r--   0        0        0   737680 2024-05-30 15:37:19.425924 gwcelery-2.4.1/doc/_static/sentry-screenshot.png
+-rwxr-xr-x   0        0        0     7356 2024-05-30 15:37:19.426925 gwcelery-2.4.1/doc/conf.py
+-rw-r--r--   0        0        0     4346 2024-05-30 15:37:19.426925 gwcelery-2.4.1/doc/configuration.rst
+-rw-r--r--   0        0        0     5698 2024-05-30 15:37:19.426925 gwcelery-2.4.1/doc/contributing.rst
+-rw-r--r--   0        0        0    10846 2024-05-30 15:37:19.426925 gwcelery-2.4.1/doc/deployment.rst
+-rw-r--r--   0        0        0    10296 2024-05-30 15:37:19.427924 gwcelery-2.4.1/doc/design.rst
+-rw-r--r--   0        0        0      563 2024-05-30 15:37:19.427924 gwcelery-2.4.1/doc/gwcelery.conf.rst
+-rw-r--r--   0        0        0      284 2024-05-30 15:37:19.427924 gwcelery-2.4.1/doc/gwcelery.email.rst
+-rw-r--r--   0        0        0      329 2024-05-30 15:37:19.427924 gwcelery-2.4.1/doc/gwcelery.igwn_alert.rst
+-rw-r--r--   0        0        0      227 2024-05-30 15:37:19.427924 gwcelery-2.4.1/doc/gwcelery.rst
+-rw-r--r--   0        0        0       79 2024-05-30 15:37:19.427924 gwcelery-2.4.1/doc/gwcelery.sentry.rst
+-rw-r--r--   0        0        0       97 2024-05-30 15:37:19.427924 gwcelery-2.4.1/doc/gwcelery.tasks.alerts.rst
+-rw-r--r--   0        0        0      103 2024-05-30 15:37:19.427924 gwcelery-2.4.1/doc/gwcelery.tasks.bayestar.rst
+-rw-r--r--   0        0        0      107 2024-05-30 15:37:19.427924 gwcelery-2.4.1/doc/gwcelery.tasks.circulars.rst
+-rw-r--r--   0        0        0       98 2024-05-30 15:37:19.427924 gwcelery-2.4.1/doc/gwcelery.tasks.condor.rst
+-rw-r--r--   0        0        0       91 2024-05-30 15:37:19.427924 gwcelery-2.4.1/doc/gwcelery.tasks.core.rst
+-rw-r--r--   0        0        0     2404 2024-05-30 15:37:19.427924 gwcelery-2.4.1/doc/gwcelery.tasks.detchar.rst
+-rw-r--r--   0        0        0     1110 2024-05-30 15:37:19.427924 gwcelery-2.4.1/doc/gwcelery.tasks.em_bright.rst
+-rw-r--r--   0        0        0      129 2024-05-30 15:37:19.428925 gwcelery-2.4.1/doc/gwcelery.tasks.external_skymaps.rst
+-rw-r--r--   0        0        0     9812 2024-05-30 15:37:19.428925 gwcelery-2.4.1/doc/gwcelery.tasks.external_triggers.rst
+-rw-r--r--   0        0        0      112 2024-05-30 15:37:19.428925 gwcelery-2.4.1/doc/gwcelery.tasks.first2years.rst
+-rw-r--r--   0        0        0      139 2024-05-30 15:37:19.428925 gwcelery-2.4.1/doc/gwcelery.tasks.first2years_external.rst
+-rw-r--r--   0        0        0       88 2024-05-30 15:37:19.428925 gwcelery-2.4.1/doc/gwcelery.tasks.gcn.rst
+-rw-r--r--   0        0        0      100 2024-05-30 15:37:19.428925 gwcelery-2.4.1/doc/gwcelery.tasks.gracedb.rst
+-rw-r--r--   0        0        0      103 2024-05-30 15:37:19.428925 gwcelery-2.4.1/doc/gwcelery.tasks.gwskynet.rst
+-rw-r--r--   0        0        0      109 2024-05-30 15:37:19.428925 gwcelery-2.4.1/doc/gwcelery.tasks.igwn_alert.rst
+-rw-r--r--   0        0        0      109 2024-05-30 15:37:19.428925 gwcelery-2.4.1/doc/gwcelery.tasks.inference.rst
+-rw-r--r--   0        0        0      121 2024-05-30 15:37:19.428925 gwcelery-2.4.1/doc/gwcelery.tasks.legacy_gracedb.rst
+-rw-r--r--   0        0        0      112 2024-05-30 15:37:19.428925 gwcelery-2.4.1/doc/gwcelery.tasks.notice_text.rst
+-rw-r--r--   0        0        0     8111 2024-05-30 15:37:19.429925 gwcelery-2.4.1/doc/gwcelery.tasks.orchestrator.rst
+-rw-r--r--   0        0        0      100 2024-05-30 15:37:19.429925 gwcelery-2.4.1/doc/gwcelery.tasks.p_astro.rst
+-rw-r--r--   0        0        0     2385 2024-05-30 15:37:19.429925 gwcelery-2.4.1/doc/gwcelery.tasks.raven.rst
+-rw-r--r--   0        0        0      106 2024-05-30 15:37:19.429925 gwcelery-2.4.1/doc/gwcelery.tasks.rrt_utils.rst
+-rw-r--r--   0        0        0      814 2024-05-30 15:37:19.429925 gwcelery-2.4.1/doc/gwcelery.tasks.rst
+-rw-r--r--   0        0        0      100 2024-05-30 15:37:19.429925 gwcelery-2.4.1/doc/gwcelery.tasks.skymaps.rst
+-rw-r--r--   0        0        0     7161 2024-05-30 15:37:19.429925 gwcelery-2.4.1/doc/gwcelery.tasks.superevents.rst
+-rw-r--r--   0        0        0       97 2024-05-30 15:37:19.429925 gwcelery-2.4.1/doc/gwcelery.tools.condor.rst
+-rw-r--r--   0        0        0       94 2024-05-30 15:37:19.429925 gwcelery-2.4.1/doc/gwcelery.tools.flask.rst
+-rw-r--r--   0        0        0       97 2024-05-30 15:37:19.429925 gwcelery-2.4.1/doc/gwcelery.tools.nagios.rst
+-rw-r--r--   0        0        0      185 2024-05-30 15:37:19.429925 gwcelery-2.4.1/doc/gwcelery.tools.rst
+-rw-r--r--   0        0        0       73 2024-05-30 15:37:19.429925 gwcelery-2.4.1/doc/gwcelery.util.rst
+-rw-r--r--   0        0        0      507 2024-05-30 15:37:19.429925 gwcelery-2.4.1/doc/gwcelery.voevent.rst
+-rw-r--r--   0        0        0     3564 2024-05-30 15:37:19.430925 gwcelery-2.4.1/doc/htcondor.rst
+-rw-r--r--   0        0        0     1590 2024-05-30 15:37:19.430925 gwcelery-2.4.1/doc/index.rst
+-rw-r--r--   0        0        0      800 2024-05-30 15:37:19.430925 gwcelery-2.4.1/doc/make.bat
+-rw-r--r--   0        0        0     8199 2024-05-30 15:37:19.430925 gwcelery-2.4.1/doc/monitoring.rst
+-rw-r--r--   0        0        0     7240 2024-05-30 15:37:19.430925 gwcelery-2.4.1/doc/operations.rst
+-rw-r--r--   0        0        0     5405 2024-05-30 15:37:19.430925 gwcelery-2.4.1/doc/quickstart.rst
+-rw-r--r--   0        0        0     1097 2024-05-30 15:37:19.430925 gwcelery-2.4.1/gwcelery/__init__.py
+-rw-r--r--   0        0        0    18447 2024-05-30 15:37:19.431925 gwcelery-2.4.1/gwcelery/_version.py
+-rw-r--r--   0        0        0    19394 2024-05-30 15:37:19.431925 gwcelery-2.4.1/gwcelery/conf/__init__.py
+-rw-r--r--   0        0        0     1195 2024-05-30 15:37:19.431925 gwcelery-2.4.1/gwcelery/conf/dev.py
+-rw-r--r--   0        0        0     1180 2024-05-30 15:37:19.431925 gwcelery-2.4.1/gwcelery/conf/minikube.py
+-rw-r--r--   0        0        0     2178 2024-05-30 15:37:19.431925 gwcelery-2.4.1/gwcelery/conf/playground.py
+-rw-r--r--   0        0        0     3687 2024-05-30 15:37:19.431925 gwcelery-2.4.1/gwcelery/conf/production.py
+-rw-r--r--   0        0        0     2040 2024-05-30 15:37:19.432925 gwcelery-2.4.1/gwcelery/conf/test.py
+-rw-r--r--   0        0        0        0 2024-05-30 21:50:59.957858 gwcelery-2.4.1/gwcelery/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 21:50:59.958858 gwcelery-2.4.1/gwcelery/data/first2years/__init__.py
+-rw-r--r--   0        0        0   731421 2024-05-30 15:37:19.435925 gwcelery-2.4.1/gwcelery/data/first2years/gstlal.xml.gz
+-rwxr-xr-x   0        0        0     3199 2024-05-30 15:37:19.435925 gwcelery-2.4.1/gwcelery/data/gwcelery.sub
+-rw-r--r--   0        0        0      505 2024-05-30 15:37:19.435925 gwcelery-2.4.1/gwcelery/email/__init__.py
+-rw-r--r--   0        0        0     3413 2024-05-30 15:37:19.435925 gwcelery-2.4.1/gwcelery/email/bootsteps.py
+-rw-r--r--   0        0        0      995 2024-05-30 15:37:19.435925 gwcelery-2.4.1/gwcelery/email/signals.py
+-rw-r--r--   0        0        0     1457 2024-05-30 15:37:19.435925 gwcelery-2.4.1/gwcelery/flask.py
+-rw-r--r--   0        0        0      529 2024-05-30 15:37:19.435925 gwcelery-2.4.1/gwcelery/igwn_alert/__init__.py
+-rw-r--r--   0        0        0     4484 2024-05-30 15:37:19.436925 gwcelery-2.4.1/gwcelery/igwn_alert/bootsteps.py
+-rw-r--r--   0        0        0      608 2024-05-30 15:37:19.436925 gwcelery-2.4.1/gwcelery/igwn_alert/signals.py
+-rw-r--r--   0        0        0      275 2024-05-30 15:37:19.436925 gwcelery-2.4.1/gwcelery/jinja.py
+-rw-r--r--   0        0        0      305 2024-05-30 15:37:19.436925 gwcelery-2.4.1/gwcelery/kafka/__init__.py
+-rw-r--r--   0        0        0    11839 2024-05-30 15:37:19.436925 gwcelery-2.4.1/gwcelery/kafka/bootsteps.py
+-rw-r--r--   0        0        0      522 2024-05-30 15:37:19.436925 gwcelery-2.4.1/gwcelery/kafka/signals.py
+-rw-r--r--   0        0        0     2567 2024-05-30 15:37:19.436925 gwcelery-2.4.1/gwcelery/sentry/__init__.py
+-rw-r--r--   0        0        0       34 2024-05-30 15:37:19.436925 gwcelery-2.4.1/gwcelery/sentry/integrations/__init__.py
+-rw-r--r--   0        0        0      832 2024-05-30 15:37:19.436925 gwcelery-2.4.1/gwcelery/sentry/integrations/condor.py
+-rw-r--r--   0        0        0      836 2024-05-30 15:37:19.437925 gwcelery-2.4.1/gwcelery/sentry/integrations/requests.py
+-rw-r--r--   0        0        0      939 2024-05-30 15:37:19.437925 gwcelery-2.4.1/gwcelery/sentry/integrations/subprocess.py
+-rw-r--r--   0        0        0     1302 2024-05-30 15:37:19.437925 gwcelery-2.4.1/gwcelery/static/typeahead.css
+-rw-r--r--   0        0        0     4124 2024-05-30 15:37:19.437925 gwcelery-2.4.1/gwcelery/static/vega/index.html
+-rw-r--r--   0        0        0      515 2024-05-30 15:37:19.437925 gwcelery-2.4.1/gwcelery/tasks/__init__.py
+-rw-r--r--   0        0        0    14457 2024-05-30 15:37:19.437925 gwcelery-2.4.1/gwcelery/tasks/alerts.py
+-rw-r--r--   0        0        0     2540 2024-05-30 15:37:19.437925 gwcelery-2.4.1/gwcelery/tasks/bayestar.py
+-rw-r--r--   0        0        0     1892 2024-05-30 15:37:19.438925 gwcelery-2.4.1/gwcelery/tasks/circulars.py
+-rw-r--r--   0        0        0     7552 2024-05-30 15:37:19.438925 gwcelery-2.4.1/gwcelery/tasks/condor.py
+-rw-r--r--   0        0        0     2692 2024-05-30 15:37:19.438925 gwcelery-2.4.1/gwcelery/tasks/core.py
+-rw-r--r--   0        0        0    23178 2024-05-30 15:37:19.438925 gwcelery-2.4.1/gwcelery/tasks/detchar.py
+-rw-r--r--   0        0        0     4903 2024-05-30 15:37:19.438925 gwcelery-2.4.1/gwcelery/tasks/em_bright.py
+-rw-r--r--   0        0        0    29573 2024-05-30 15:37:19.439925 gwcelery-2.4.1/gwcelery/tasks/external_skymaps.py
+-rw-r--r--   0        0        0    32326 2024-05-30 16:51:32.291310 gwcelery-2.4.1/gwcelery/tasks/external_triggers.py
+-rw-r--r--   0        0        0     6841 2024-05-30 15:37:19.439925 gwcelery-2.4.1/gwcelery/tasks/first2years.py
+-rw-r--r--   0        0        0    10843 2024-05-30 16:51:32.291310 gwcelery-2.4.1/gwcelery/tasks/first2years_external.py
+-rw-r--r--   0        0        0     4832 2024-05-30 15:37:19.440925 gwcelery-2.4.1/gwcelery/tasks/gcn.py
+-rw-r--r--   0        0        0    12159 2024-05-30 15:37:19.440925 gwcelery-2.4.1/gwcelery/tasks/gracedb.py
+-rw-r--r--   0        0        0     7727 2024-05-30 15:37:19.440925 gwcelery-2.4.1/gwcelery/tasks/gwskynet.py
+-rw-r--r--   0        0        0     2453 2024-05-30 15:37:19.440925 gwcelery-2.4.1/gwcelery/tasks/igwn_alert.py
+-rw-r--r--   0        0        0    35696 2024-05-30 15:37:19.440925 gwcelery-2.4.1/gwcelery/tasks/inference.py
+-rw-r--r--   0        0        0     1407 2024-05-30 15:37:19.441925 gwcelery-2.4.1/gwcelery/tasks/legacy_gracedb.py
+-rw-r--r--   0        0        0     8556 2024-05-30 15:37:19.441925 gwcelery-2.4.1/gwcelery/tasks/notice_text.py
+-rw-r--r--   0        0        0    57712 2024-05-30 16:51:32.293310 gwcelery-2.4.1/gwcelery/tasks/orchestrator.py
+-rw-r--r--   0        0        0     5847 2024-05-30 15:37:19.442925 gwcelery-2.4.1/gwcelery/tasks/p_astro.py
+-rw-r--r--   0        0        0    25177 2024-05-30 16:51:32.294310 gwcelery-2.4.1/gwcelery/tasks/raven.py
+-rw-r--r--   0        0        0     2264 2024-05-30 15:37:19.442925 gwcelery-2.4.1/gwcelery/tasks/rrt_utils.py
+-rw-r--r--   0        0        0     9510 2024-05-30 15:37:19.442925 gwcelery-2.4.1/gwcelery/tasks/skymaps.py
+-rw-r--r--   0        0        0    25167 2024-05-30 15:37:19.443925 gwcelery-2.4.1/gwcelery/tasks/superevents.py
+-rw-r--r--   0        0        0     1084 2024-05-30 15:37:19.443925 gwcelery-2.4.1/gwcelery/templates/fits_header.jinja2
+-rw-r--r--   0        0        0    41877 2024-05-30 15:37:19.443925 gwcelery-2.4.1/gwcelery/templates/index.jinja2
+-rw-r--r--   0        0        0     8505 2024-05-30 15:37:19.443925 gwcelery-2.4.1/gwcelery/templates/lalinference.jinja2
+-rw-r--r--   0        0        0     9473 2024-05-30 15:37:19.444925 gwcelery-2.4.1/gwcelery/templates/rapidpe.jinja2
+-rw-r--r--   0        0        0      472 2024-05-30 15:37:19.444925 gwcelery-2.4.1/gwcelery/templates/vector_table.jinja2
+-rw-r--r--   0        0        0        0 2024-05-30 21:50:59.961858 gwcelery-2.4.1/gwcelery/tests/__init__.py
+-rw-r--r--   0        0        0     4388 2024-05-30 15:37:19.444925 gwcelery-2.4.1/gwcelery/tests/conftest.py
+-rw-r--r--   0        0        0      976 2024-05-30 15:37:19.444925 gwcelery-2.4.1/gwcelery/tests/data/G000012_S0040_preferred.json
+-rw-r--r--   0        0        0     6258 2024-05-30 15:37:19.444925 gwcelery-2.4.1/gwcelery/tests/data/G298048-1-Initial.xml
+-rw-r--r--   0        0        0      599 2024-05-30 15:37:19.444925 gwcelery-2.4.1/gwcelery/tests/data/G298048_log.json
+-rw-r--r--   0        0        0      150 2024-05-30 15:37:19.444925 gwcelery-2.4.1/gwcelery/tests/data/H1L1V1-mean_counts-1126051217-61603201.json
+-rw-r--r--   0        0        0      974 2024-05-30 15:37:19.445925 gwcelery-2.4.1/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json
+-rw-r--r--   0        0        0    17572 2024-05-30 15:37:19.445925 gwcelery-2.4.1/gwcelery/tests/data/MS220722v.json
+-rw-r--r--   0        0        0   777600 2024-05-30 15:37:19.451925 gwcelery-2.4.1/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits
+-rw-r--r--   0        0        0     8232 2024-05-30 15:37:19.451925 gwcelery-2.4.1/gwcelery/tests/data/S230413b.json
+-rw-r--r--   0        0        0     7255 2024-05-30 15:37:19.451925 gwcelery-2.4.1/gwcelery/tests/data/S230413g.json
+-rw-r--r--   0        0        0     7721 2024-05-30 15:37:19.451925 gwcelery-2.4.1/gwcelery/tests/data/S230413h.json
+-rw-r--r--   0        0        0     3387 2024-05-30 15:37:19.451925 gwcelery-2.4.1/gwcelery/tests/data/T0212_S0039_preferred.json
+-rw-r--r--   0        0        0     3384 2024-05-30 15:37:19.451925 gwcelery-2.4.1/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json
+-rw-r--r--   0        0        0     5210 2024-05-30 15:37:19.452925 gwcelery-2.4.1/gwcelery/tests/data/T0219_S0041_nopreferred.json
+-rw-r--r--   0        0        0        0 2024-05-30 21:50:59.962858 gwcelery-2.4.1/gwcelery/tests/data/__init__.py
+-rw-r--r--   0        0        0   854036 2024-05-30 15:37:19.457925 gwcelery-2.4.1/gwcelery/tests/data/coinc.xml
+-rw-r--r--   0        0        0     6175 2024-05-30 15:37:19.457925 gwcelery-2.4.1/gwcelery/tests/data/externaltrigger_original_data.xml
+-rw-r--r--   0        0        0     5482 2024-05-30 15:37:19.457925 gwcelery-2.4.1/gwcelery/tests/data/fermi_grb_gcn.xml
+-rw-r--r--   0        0        0     5469 2024-05-30 15:37:19.457925 gwcelery-2.4.1/gwcelery/tests/data/fermi_initial_grb_gcn.xml
+-rw-r--r--   0        0        0     5865 2024-05-30 15:37:19.458926 gwcelery-2.4.1/gwcelery/tests/data/fermi_noise_gcn.xml
+-rw-r--r--   0        0        0     5864 2024-05-30 15:37:19.458926 gwcelery-2.4.1/gwcelery/tests/data/fermi_noise_gcn_2.xml
+-rw-r--r--   0        0        0     1922 2024-05-30 15:37:19.458926 gwcelery-2.4.1/gwcelery/tests/data/fermi_subgrbtargeted_template.xml
+-rw-r--r--   0        0        0     4914 2024-05-30 15:37:19.458926 gwcelery-2.4.1/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml
+-rw-r--r--   0        0        0     4914 2024-05-30 15:37:19.458926 gwcelery-2.4.1/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml
+-rw-r--r--   0        0        0     3407 2024-05-30 15:37:19.458926 gwcelery-2.4.1/gwcelery/tests/data/fits_header_result.html
+-rw-r--r--   0        0        0      882 2024-05-30 15:37:19.458926 gwcelery-2.4.1/gwcelery/tests/data/gracedb_externaltrigger_log.json
+-rw-r--r--   0        0        0      446 2024-05-30 15:37:19.458926 gwcelery-2.4.1/gwcelery/tests/data/gracedb_setrigger_log.json
+-rw-r--r--   0        0        0      870 2024-05-30 15:37:19.458926 gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_detchar.json
+-rw-r--r--   0        0        0     2025 2024-05-30 15:37:19.459926 gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_exttrig_creation.json
+-rw-r--r--   0        0        0     2007 2024-05-30 15:37:19.459926 gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json
+-rw-r--r--   0        0        0      166 2024-05-30 15:37:19.459926 gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_fits.json
+-rw-r--r--   0        0        0      101 2024-05-30 15:37:19.459926 gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_label_dqv.json
+-rw-r--r--   0        0        0      743 2024-05-30 15:37:19.459926 gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_psd.json
+-rw-r--r--   0        0        0     2020 2024-05-30 15:37:19.459926 gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_snews_creation.json
+-rw-r--r--   0        0        0     2012 2024-05-30 15:37:19.459926 gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_snews_test_creation.json
+-rw-r--r--   0        0        0     2028 2024-05-30 15:37:19.459926 gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_subgrb_creation.json
+-rw-r--r--   0        0        0     1265 2024-05-30 15:37:19.460926 gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_superevent_burst_bbh_creation.json
+-rw-r--r--   0        0        0     1235 2024-05-30 15:37:19.460926 gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_superevent_creation.json
+-rw-r--r--   0        0        0      107 2024-05-30 15:37:19.460926 gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_superevent_label.json
+-rw-r--r--   0        0        0     5021 2024-05-30 15:37:19.460926 gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_voevent.json
+-rw-r--r--   0        0        0     4429 2024-05-30 15:37:19.460926 gwcelery-2.4.1/gwcelery/tests/data/integral_grb_gcn.xml
+-rw-r--r--   0        0        0     4295 2024-05-30 15:37:19.460926 gwcelery-2.4.1/gwcelery/tests/data/integral_mdc_gcn.xml
+-rw-r--r--   0        0        0     4451 2024-05-30 15:37:19.460926 gwcelery-2.4.1/gwcelery/tests/data/integral_test_gcn.xml
+-rw-r--r--   0        0        0  1038044 2024-05-30 15:37:19.469926 gwcelery-2.4.1/gwcelery/tests/data/kafka_alert_fermi.json
+-rw-r--r--   0        0        0  1038042 2024-05-30 15:37:19.472926 gwcelery-2.4.1/gwcelery/tests/data/kafka_alert_fermi_ignore.json
+-rw-r--r--   0        0        0      806 2024-05-30 15:37:19.472926 gwcelery-2.4.1/gwcelery/tests/data/kafka_alert_swift.json
+-rw-r--r--   0        0        0      743 2024-05-30 15:37:19.472926 gwcelery-2.4.1/gwcelery/tests/data/kafka_alert_swift_noloc.json
+-rw-r--r--   0        0        0  1037630 2024-05-30 15:37:19.474926 gwcelery-2.4.1/gwcelery/tests/data/kafka_alert_swift_wskymap.json
+-rw-r--r--   0        0        0        0 2024-05-30 21:50:59.964858 gwcelery-2.4.1/gwcelery/tests/data/llhoft/__init__.py
+-rw-r--r--   0        0        0     8267 2024-05-30 15:37:19.475926 gwcelery-2.4.1/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2024-05-30 21:50:59.964858 gwcelery-2.4.1/gwcelery/tests/data/llhoft/fail/L1/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 21:50:59.964858 gwcelery-2.4.1/gwcelery/tests/data/llhoft/fail/__init__.py
+-rw-r--r--   0        0        0    14942 2024-05-30 15:37:19.476926 gwcelery-2.4.1/gwcelery/tests/data/llhoft/idqbad/H1/H-H1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2024-05-30 21:50:59.964858 gwcelery-2.4.1/gwcelery/tests/data/llhoft/omegascan/__init__.py
+-rw-r--r--   0        0        0   516419 2024-05-30 15:37:19.477926 gwcelery-2.4.1/gwcelery/tests/data/llhoft/omegascan/scanme.gwf
+-rw-r--r--   0        0        0    14950 2024-05-30 15:37:19.478926 gwcelery-2.4.1/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2024-05-30 21:50:59.964858 gwcelery-2.4.1/gwcelery/tests/data/llhoft/pass/H1/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 21:50:59.964858 gwcelery-2.4.1/gwcelery/tests/data/llhoft/pass/__init__.py
+-rw-r--r--   0        0        0    13099 2024-05-30 15:37:19.478926 gwcelery-2.4.1/gwcelery/tests/data/lvalert_event_creation.json
+-rw-r--r--   0        0        0     9060 2024-05-30 15:37:19.478926 gwcelery-2.4.1/gwcelery/tests/data/lvalert_xmpp.xml
+-rw-r--r--   0        0        0      864 2024-05-30 15:37:19.478926 gwcelery-2.4.1/gwcelery/tests/data/mock_superevent_object.json
+-rw-r--r--   0        0        0   445440 2024-05-30 15:37:19.480926 gwcelery-2.4.1/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite
+-rw-r--r--   0        0        0   294426 2024-05-30 15:37:19.482926 gwcelery-2.4.1/gwcelery/tests/data/psd.xml.gz
+-rw-r--r--   0        0        0    11520 2024-05-30 15:37:19.482926 gwcelery-2.4.1/gwcelery/tests/data/rrt_small_area.fits
+-rw-r--r--   0        0        0     2961 2024-05-30 15:37:19.482926 gwcelery-2.4.1/gwcelery/tests/data/sample_events.json
+-rw-r--r--   0        0        0     3648 2024-05-30 15:37:19.482926 gwcelery-2.4.1/gwcelery/tests/data/samples.hdf5
+-rw-r--r--   0        0        0      616 2024-05-30 15:37:19.482926 gwcelery-2.4.1/gwcelery/tests/data/scaler_set_all.pickle
+-rw-r--r--   0        0        0     6169 2024-05-30 15:37:19.482926 gwcelery-2.4.1/gwcelery/tests/data/snews_gcn.xml
+-rw-r--r--   0        0        0     6161 2024-05-30 15:37:19.482926 gwcelery-2.4.1/gwcelery/tests/data/snews_gcn_test.xml
+-rw-r--r--   0        0        0     9583 2024-05-30 15:37:19.482926 gwcelery-2.4.1/gwcelery/tests/data/superevents.json
+-rw-r--r--   0        0        0     7713 2024-05-30 15:37:19.483926 gwcelery-2.4.1/gwcelery/tests/data/swift_grb_gcn.xml
+-rw-r--r--   0        0        0     1970 2024-05-30 15:37:19.483926 gwcelery-2.4.1/gwcelery/tests/data/swift_subgrbtargeted_template.xml
+-rw-r--r--   0        0        0   581918 2024-05-30 15:37:19.486926 gwcelery-2.4.1/gwcelery/tests/data/test_classifier.pickle
+-rw-r--r--   0        0        0      122 2024-05-30 15:37:19.486926 gwcelery-2.4.1/gwcelery/tests/data/updated_RapidPE_RIFT.p_astro.json
+-rw-r--r--   0        0        0     4063 2024-05-30 15:37:19.486926 gwcelery-2.4.1/gwcelery/tests/process.py
+-rw-r--r--   0        0        0     2307 2024-05-30 15:37:19.486926 gwcelery-2.4.1/gwcelery/tests/test_sentry.py
+-rw-r--r--   0        0        0     1669 2024-05-30 15:37:19.486926 gwcelery-2.4.1/gwcelery/tests/test_tasks_alerts.py
+-rw-r--r--   0        0        0     4815 2024-05-30 15:37:19.486926 gwcelery-2.4.1/gwcelery/tests/test_tasks_alerts_validate.py
+-rw-r--r--   0        0        0     1428 2024-05-30 15:37:19.487926 gwcelery-2.4.1/gwcelery/tests/test_tasks_bayestar.py
+-rw-r--r--   0        0        0     3172 2024-05-30 15:37:19.487926 gwcelery-2.4.1/gwcelery/tests/test_tasks_circulars.py
+-rw-r--r--   0        0        0     4550 2024-05-30 15:37:19.487926 gwcelery-2.4.1/gwcelery/tests/test_tasks_condor.py
+-rw-r--r--   0        0        0    17285 2024-05-30 15:37:19.487926 gwcelery-2.4.1/gwcelery/tests/test_tasks_detchar.py
+-rw-r--r--   0        0        0     2317 2024-05-30 15:37:19.487926 gwcelery-2.4.1/gwcelery/tests/test_tasks_em_bright.py
+-rw-r--r--   0        0        0    17442 2024-05-30 15:37:19.488927 gwcelery-2.4.1/gwcelery/tests/test_tasks_external_skymaps.py
+-rw-r--r--   0        0        0    43864 2024-05-30 16:51:32.294310 gwcelery-2.4.1/gwcelery/tests/test_tasks_external_triggers.py
+-rw-r--r--   0        0        0     1797 2024-05-30 15:37:19.488927 gwcelery-2.4.1/gwcelery/tests/test_tasks_first2years.py
+-rw-r--r--   0        0        0     7098 2024-05-30 16:51:32.294310 gwcelery-2.4.1/gwcelery/tests/test_tasks_first2years_external.py
+-rw-r--r--   0        0        0     1815 2024-05-30 15:37:19.488927 gwcelery-2.4.1/gwcelery/tests/test_tasks_gcn.py
+-rw-r--r--   0        0        0     1616 2024-05-30 15:37:19.489926 gwcelery-2.4.1/gwcelery/tests/test_tasks_gcn_validate.py
+-rw-r--r--   0        0        0     5728 2024-05-30 15:37:19.489926 gwcelery-2.4.1/gwcelery/tests/test_tasks_gracedb.py
+-rw-r--r--   0        0        0    11860 2024-05-30 15:37:19.489926 gwcelery-2.4.1/gwcelery/tests/test_tasks_gwskynet.py
+-rw-r--r--   0        0        0     3676 2024-05-30 15:37:19.489926 gwcelery-2.4.1/gwcelery/tests/test_tasks_igwn_alert.py
+-rw-r--r--   0        0        0    29687 2024-05-30 15:37:19.489926 gwcelery-2.4.1/gwcelery/tests/test_tasks_inference.py
+-rw-r--r--   0        0        0    58484 2024-05-30 16:51:32.295310 gwcelery-2.4.1/gwcelery/tests/test_tasks_orchestrator.py
+-rw-r--r--   0        0        0     1647 2024-05-30 15:37:19.490927 gwcelery-2.4.1/gwcelery/tests/test_tasks_p_astro.py
+-rw-r--r--   0        0        0    29743 2024-05-30 16:51:32.295310 gwcelery-2.4.1/gwcelery/tests/test_tasks_raven.py
+-rw-r--r--   0        0        0     4696 2024-05-30 15:37:19.490927 gwcelery-2.4.1/gwcelery/tests/test_tasks_rrt_utils.py
+-rw-r--r--   0        0        0     5520 2024-05-30 15:37:19.490927 gwcelery-2.4.1/gwcelery/tests/test_tasks_skymaps.py
+-rw-r--r--   0        0        0    50557 2024-05-30 15:37:19.491927 gwcelery-2.4.1/gwcelery/tests/test_tasks_superevents.py
+-rw-r--r--   0        0        0      637 2024-05-30 15:37:19.491927 gwcelery-2.4.1/gwcelery/tests/test_tempfile.py
+-rw-r--r--   0        0        0     3520 2024-05-30 15:37:19.491927 gwcelery-2.4.1/gwcelery/tests/test_tools_condor.py
+-rw-r--r--   0        0        0     1098 2024-05-30 15:37:19.491927 gwcelery-2.4.1/gwcelery/tests/test_tools_condor_submit_helper.py
+-rw-r--r--   0        0        0      647 2024-05-30 15:37:19.491927 gwcelery-2.4.1/gwcelery/tests/test_tools_flask.py
+-rw-r--r--   0        0        0    11271 2024-05-30 15:37:19.491927 gwcelery-2.4.1/gwcelery/tests/test_tools_nagios.py
+-rw-r--r--   0        0        0      269 2024-05-30 15:37:19.492927 gwcelery-2.4.1/gwcelery/tests/test_util.py
+-rw-r--r--   0        0        0    25205 2024-05-30 15:37:19.492927 gwcelery-2.4.1/gwcelery/tests/test_views.py
+-rw-r--r--   0        0        0      216 2024-05-30 15:37:19.492927 gwcelery-2.4.1/gwcelery/tools/__init__.py
+-rw-r--r--   0        0        0     2941 2024-05-30 15:37:19.492927 gwcelery-2.4.1/gwcelery/tools/condor.py
+-rw-r--r--   0        0        0     1120 2024-05-30 15:37:19.492927 gwcelery-2.4.1/gwcelery/tools/condor_submit_helper.py
+-rw-r--r--   0        0        0     1938 2024-05-30 15:37:19.492927 gwcelery-2.4.1/gwcelery/tools/flask.py
+-rw-r--r--   0        0        0     9145 2024-05-30 15:37:19.492927 gwcelery-2.4.1/gwcelery/tools/nagios.py
+-rw-r--r--   0        0        0      413 2024-05-30 15:37:19.493927 gwcelery-2.4.1/gwcelery/util/__init__.py
+-rw-r--r--   0        0        0     1007 2024-05-30 15:37:19.493927 gwcelery-2.4.1/gwcelery/util/cmdline.py
+-rw-r--r--   0        0        0      453 2024-05-30 15:37:19.493927 gwcelery-2.4.1/gwcelery/util/matplotlib.py
+-rw-r--r--   0        0        0      390 2024-05-30 15:37:19.493927 gwcelery-2.4.1/gwcelery/util/proxy.py
+-rw-r--r--   0        0        0      585 2024-05-30 15:37:19.493927 gwcelery-2.4.1/gwcelery/util/resources.py
+-rw-r--r--   0        0        0      253 2024-05-30 15:37:19.493927 gwcelery-2.4.1/gwcelery/util/sphinx.py
+-rw-r--r--   0        0        0      941 2024-05-30 15:37:19.493927 gwcelery-2.4.1/gwcelery/util/tempfile.py
+-rw-r--r--   0        0        0    21888 2024-05-30 16:51:32.296310 gwcelery-2.4.1/gwcelery/views.py
+-rw-r--r--   0        0        0      365 2024-05-30 15:37:19.494927 gwcelery-2.4.1/gwcelery/voevent/__init__.py
+-rw-r--r--   0        0        0     6388 2024-05-30 15:37:19.494927 gwcelery-2.4.1/gwcelery/voevent/bootsteps.py
+-rw-r--r--   0        0        0     1063 2024-05-30 15:37:19.494927 gwcelery-2.4.1/gwcelery/voevent/logging.py
+-rw-r--r--   0        0        0      779 2024-05-30 15:37:19.494927 gwcelery-2.4.1/gwcelery/voevent/signals.py
+-rw-r--r--   0        0        0      884 2024-05-30 15:37:19.494927 gwcelery-2.4.1/gwcelery/voevent/subscriber.py
+-rw-r--r--   0        0        0     1454 2024-05-30 15:37:19.494927 gwcelery-2.4.1/gwcelery/voevent/util.py
+-rw-r--r--   0        0        0     6491 2024-05-30 21:51:10.076184 gwcelery-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4654 1970-01-01 00:00:00.000000 gwcelery-2.4.1/PKG-INFO
```

### Comparing `gwcelery-2.3.6/CHANGES.rst` & `gwcelery-2.4.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,52 @@
 Changelog
 =========
 
+2.4.1 "Orabou" (2024-05-30)
+---------------------------
+
+-   Add GWSkyNet 2.4.1 to avoid installing tensorflow-cpu >= 2.16.1.
+    Clairfy the version of annotated skymaps and quantities in the uploads.
+    Add public tag to GWSkyNet's uploads.
+
+-   Reduce Burst trials by one removing MLy from trials factor count.
+
+-   Add ``DQR_REQUEST`` label with a countdown for significant early-warning
+    events.
+
+-   Increase tukey window roll off to 1s to reduce biases due to windowing in bilby.
+
+-   Increase request memory for online PE with IMRPhenomXPHM waveform model.
+
+-   Enable parameter estimation on burst-BBH triggers associated with
+    low-significance CBC triggers.
+
+-   Update ROTA responsibilities in documentation.
+
+-   Remove AGILE from the RAVEN workflow since it has been decommissioned.
+
+-   Retry email bootstep when IMAP connection is reset.
+
+-   Add gracedb client side 409 error code to the list of retries.
+
+-   Don't log omegascan FloatingPointErrors to Sentry since we know that they
+    come from data which is only zeros (e.g., Virgo out of observing).
+
+-   Filter Burst-BBH superevents from SNEWS coincidence searches.
+
+-   Don't apply EM_COINC if external event is SubGRBTargeted and vetoed by
+    NOT_GRB.
+
+-   Require no spaces and specific version format for filenames when sending
+    update notices
+
+-   Serialize changing of preferred external event.
+
+-   Update Nagios URL and screenshot in the documentation.
+
 2.3.6 "Champ" (2024-04-30)
 --------------------------
 
 -   Update trials factor to account for MLy joining O4b.
 
 -   Update ligo-skymap to 2.0.0.
 
@@ -47,27 +89,29 @@
     variables.
 
 -   Fix bug when creating combined sky maps in the targeted search, being
     loaded in the ring ordering rather than nested.
 
 -   Update trials factor for O4b.
 
+-   Pin bilby_pipe to bilby_pipe==1.3.1.
+
 2.2.1 "Sheepsquatch" (2024-03-08)
 ---------------------------------
 
 -   Include p_astro and em_bright in alert payload for burst-cwb-bbh trigger.
 
 -   Produce em_bright.json for burst-cwb-bbh triggers.
 
 -   Add acceptance check to if dependencies have been approved by SCCB and if
     Bilby PE summary is available.
 
 -   Do not add events involving KAGRA to superevents.
 
--   Require pesummary>=1.0.2 to fix bug in postprocessing of bilby results. 
+-   Require pesummary>=1.0.2 to fix bug in postprocessing of bilby results.
 
 -   Update gwpy>=3.0.8 to fix issue with discontiguous lal caches.
 
 -   Change the worker concurrency to 32 and set ``max-memory-per-child`` to
     2GB.
 
 -   Document librarian ROTA duties.
```

### Comparing `gwcelery-2.3.6/LICENSE.rst` & `gwcelery-2.4.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/README.rst` & `gwcelery-2.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/Makefile` & `gwcelery-2.4.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/_static/acceptance-tests-checklist.png` & `gwcelery-2.4.1/doc/_static/acceptance-tests-checklist.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/_static/celeryevent-screenshot.png` & `gwcelery-2.4.1/doc/_static/celeryevent-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/_static/deployment-screenshot.png` & `gwcelery-2.4.1/doc/_static/deployment-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/_static/flask-screenshot.png` & `gwcelery-2.4.1/doc/_static/flask-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/_static/logo-0.5x.png` & `gwcelery-2.4.1/doc/_static/logo-0.5x.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/_static/logo.png` & `gwcelery-2.4.1/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/conf.py` & `gwcelery-2.4.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/configuration.rst` & `gwcelery-2.4.1/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/contributing.rst` & `gwcelery-2.4.1/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/deployment.rst` & `gwcelery-2.4.1/doc/deployment.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/design.rst` & `gwcelery-2.4.1/doc/design.rst`

 * *Files 1% similar despite different names*

```diff
@@ -275,15 +275,15 @@
     one task that runs on the Superevent queue:
 
     *  :meth:`gwcelery.tasks.superevents.handle`
 
 7.  **External Trigger Worker**
 
     A Celery worker that is dedicated to serially process external triggers
-    from GRB alerts received from Fermi, Swift, Integral, Agile MCAL and
+    from GRB alerts received from Fermi, Swift, Integral and
     neutrino alerts received from SNEWS  and create/modify external trigger
     events in GraceDB:
 
     *  :meth:`gwcelery.tasks.external_triggers.handle_gcn`
 
 8.  **VOEvent Worker**
```

### Comparing `gwcelery-2.3.6/doc/gwcelery.conf.rst` & `gwcelery-2.4.1/doc/gwcelery.conf.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/gwcelery.tasks.detchar.rst` & `gwcelery-2.4.1/doc/gwcelery.tasks.detchar.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/gwcelery.tasks.em_bright.rst` & `gwcelery-2.4.1/doc/gwcelery.tasks.em_bright.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/gwcelery.tasks.external_triggers.rst` & `gwcelery-2.4.1/doc/gwcelery.tasks.external_triggers.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 gwcelery.tasks.external_triggers module
 ---------------------------------------
 
 This module listens to the `GCN` notices from `SNEWS`_ and the `Fermi`_,
-`Swift`_, `INTEGRAL`_, and `AGILE`_ missions, as well as Kafka alerts from
+`Swift`_, and `INTEGRAL`_ missions, as well as Kafka alerts from
 `Fermi`_ and `Swift`_. It is also responsible for carrying out tasks related to
 external trigger-gravitational wave coincidences, including looking for
 temporal coincidences, creating combined GRB-GW sky localization probability
 maps, and computing their joint temporal and spatio-temporal false alarm
 rates.
 
 There are two GCN, one Kafka, and two IGWN Alert message handlers in the
 `gwcelery.tasks.external_triggers` module:
 
 * :meth:`~gwcelery.tasks.external_triggers.handle_snews_gcn` is called for
   each `SNEWS`_ GCN.
 
 * :meth:`~gwcelery.tasks.external_triggers.handle_grb_gcn` is called for
-  each GRB GCN such as `Fermi`_, `Swift`_, `INTEGRAL`_, and `AGILE`_ MCAL.
+  each GRB GCN such as `Fermi`_, `Swift`_, and `INTEGRAL`_.
 
 * :meth:`~gwcelery.tasks.external_triggers.handle_targeted_kafka_alert` is
   called for GRB missions involved with the targeted search, currently `Fermi`_
   and `Swift`_.
     
 * :meth:`~gwcelery.tasks.external_triggers.handle_snews_igwn_alert` is called
   for each `SNEWS`_ external trigger and superevent IGWN Alert.
@@ -340,9 +340,8 @@
 Tasks
 ~~~~~
 .. automodule:: gwcelery.tasks.external_triggers
 
 .. _`Fermi`: https://fermi.gsfc.nasa.gov/
 .. _`Swift`: https://swift.gsfc.nasa.gov/
 .. _`INTEGRAL`: https://www.cosmos.esa.int/web/integral/science-grb
-.. _`AGILE`: https://gcn.gsfc.nasa.gov/agile.html
 .. _`SNEWS`: https://snews2.org/
```

### Comparing `gwcelery-2.3.6/doc/gwcelery.tasks.orchestrator.rst` & `gwcelery-2.4.1/doc/gwcelery.tasks.orchestrator.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/gwcelery.tasks.raven.rst` & `gwcelery-2.4.1/doc/gwcelery.tasks.raven.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/gwcelery.tasks.rst` & `gwcelery-2.4.1/doc/gwcelery.tasks.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/gwcelery.tasks.superevents.rst` & `gwcelery-2.4.1/doc/gwcelery.tasks.superevents.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/htcondor.rst` & `gwcelery-2.4.1/doc/htcondor.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/index.rst` & `gwcelery-2.4.1/doc/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
    design
    configuration
    htcondor
    monitoring
    gwcelery
    contributing
    deployment
+   operations
 
 .. toctree::
    :maxdepth: 1
 
    Git repository <http://git.ligo.org/emfollow/gwcelery>
    changes
    license
```

### Comparing `gwcelery-2.3.6/doc/make.bat` & `gwcelery-2.4.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/doc/quickstart.rst` & `gwcelery-2.4.1/doc/quickstart.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/__init__.py` & `gwcelery-2.4.1/gwcelery/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/_version.py` & `gwcelery-2.4.1/gwcelery/_version.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/conf/__init__.py` & `gwcelery-2.4.1/gwcelery/conf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,36 +175,36 @@
 significant alerts. A threshold of negative infinity disables alerts."""
 
 significant_alert_trials_factor = {
     'cbc': {'allsky': 5,
             'earlywarning': 3,
             'mdc': 5,
             'ssm': 2},
-    'burst': {'allsky': 3,
+    'burst': {'allsky': 2,
               'bbh': 5}
 }
 """Trials factor corresponding to trigger categories. The CBC AllSky and Burst
 BBH searches are treated as one group with a common trials factor. CBC AllSky
 pipelines are gstlal, pycbc, mbta, and raven. The Burst BBH pipeline is cwb.
 CBC EarlyWarning pipelines are gstlal, pycbc, and mbta. CBC SSM pipelines are
 gstlal and mbta. The Burst AllSky searches are treated as one group with one
-trials factor. The Burst AllSky piplines are cwb, mly, and raven."""
+trials factor. The Burst AllSky piplines are cwb, and raven."""
 
 preliminary_alert_trials_factor = {
-    'cbc': {'allsky': 6,
+    'cbc': {'allsky': 5,
             'earlywarning': 3,
-            'mdc': 6,
+            'mdc': 5,
             'ssm': 2},
-    'burst': {'allsky': 6,
-              'bbh': 6}
+    'burst': {'allsky': 5,
+              'bbh': 5}
 }
 """Trials factor for less significant alert categories. The CBC AllSky, Burst
 AllSky, and Burst BBH searches are all treated as one group with a shared
 trials factor. CBC AllSky pipelines are gstlal, pycbc, and mbta.  Burst AllSky
-pipeline is cwb. The Burst BBH pipelines are cwb and mly."""
+pipeline is cwb. The Burst BBH pipeline is cwb."""
 
 preliminary_alert_far_threshold = {
     'cbc': {
         'allsky': 2 / (1 * 86400) * preliminary_alert_trials_factor['cbc']['allsky'],  # noqa: E501
         'earlywarning': -1 * float('inf'),
         'mdc': -1 * float('inf'),
         'ssm': -1 * float('inf')
@@ -260,15 +260,14 @@
                         'LIB': [1.5, 1.5],
                         'CWB': [1.5, 1.5],
                         'MLy': [1.5, 1.5],
                         'HardwareInjection': [2, 2],
                         'Swift': [2, 2],
                         'Fermi': [2, 2],
                         'INTEGRAL': [2, 2],
-                        'AGILE': [2, 2],
                         'SNEWS': [10, 10]}
 """Seconds before and after the superevent start and end times which the DQ
 vector check will include in its check. Pipeline dependent."""
 
 uses_gatedhoft = {'gstlal': True,
                   'spiir': True,
                   'pycbc': True,
@@ -277,15 +276,14 @@
                   'LIB': False,
                   'CWB': True,
                   'MLy': False,
                   'HardwareInjection': False,
                   'Swift': False,
                   'Fermi': False,
                   'INTEGRAL': False,
-                  'AGILE': False,
                   'SNEWS': False}
 """Whether or not a pipeline uses gated h(t). Determines whether or not
 the DMT-DQ_VECTOR will be analyzed for data quality."""
 
 llhoft_glob = '/dev/shm/kafka/{detector}_O3ReplayMDC/*.gwf'
 """File glob for playground low-latency h(t) frames. Currently points
 to O3 MDC Mock Data Challange data.
@@ -322,15 +320,14 @@
             'LIB': False,
             'CWB': False,
             'MLy': False,
             'HardwareInjection': False,
             'Swift': False,
             'Fermi': False,
             'INTEGRAL': False,
-            'AGILE': False,
             'SNEWS': False}
 """If true for a pipeline, iDQ values below the threshold defined in
 :obj:`~gwcelery.conf.idq_fap_thresh` will cause DQV to be labeled.
 Currently all False, pending iDQ review (should be done before O3).
 """
 
 low_latency_frame_types = {'H1': 'H1_O3ReplayMDC_llhoft',
```

### Comparing `gwcelery-2.3.6/gwcelery/conf/dev.py` & `gwcelery-2.4.1/gwcelery/conf/dev.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/conf/minikube.py` & `gwcelery-2.4.1/gwcelery/conf/minikube.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/conf/playground.py` & `gwcelery-2.4.1/gwcelery/conf/playground.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/conf/production.py` & `gwcelery-2.4.1/gwcelery/conf/production.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/conf/test.py` & `gwcelery-2.4.1/gwcelery/conf/test.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/data/first2years/gstlal.xml.gz` & `gwcelery-2.4.1/gwcelery/data/first2years/gstlal.xml.gz`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/data/gwcelery.sub` & `gwcelery-2.4.1/gwcelery/data/gwcelery.sub`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/email/bootsteps.py` & `gwcelery-2.4.1/gwcelery/email/bootsteps.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,16 @@
                         for _ in range(60):
                             if not self._running or conn.idle_check(timeout=5):
                                 break
                         log.debug('Idle done')
                         conn.idle_done()
             except IMAPClientAbortError:
                 log.exception('IMAP connection aborted')
+            except ConnectionResetError:
+                log.exception('IMAP connection reset')
 
     def start(self, consumer):
         super().start(consumer)
         self._host = consumer.app.conf['email_host']
         self._running = True
         self._thread = Thread(target=self._runloop, name='EmailClientThread')
         self._thread.start()
```

### Comparing `gwcelery-2.3.6/gwcelery/email/signals.py` & `gwcelery-2.4.1/gwcelery/email/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/flask.py` & `gwcelery-2.4.1/gwcelery/flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/igwn_alert/__init__.py` & `gwcelery-2.4.1/gwcelery/igwn_alert/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/igwn_alert/bootsteps.py` & `gwcelery-2.4.1/gwcelery/igwn_alert/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/igwn_alert/signals.py` & `gwcelery-2.4.1/gwcelery/igwn_alert/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/kafka/bootsteps.py` & `gwcelery-2.4.1/gwcelery/kafka/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/kafka/signals.py` & `gwcelery-2.4.1/gwcelery/kafka/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/sentry/__init__.py` & `gwcelery-2.4.1/gwcelery/sentry/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/sentry/integrations/condor.py` & `gwcelery-2.4.1/gwcelery/sentry/integrations/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/sentry/integrations/requests.py` & `gwcelery-2.4.1/gwcelery/sentry/integrations/requests.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/sentry/integrations/subprocess.py` & `gwcelery-2.4.1/gwcelery/sentry/integrations/subprocess.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/static/typeahead.css` & `gwcelery-2.4.1/gwcelery/static/typeahead.css`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/static/vega/index.html` & `gwcelery-2.4.1/gwcelery/static/vega/index.html`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tasks/__init__.py` & `gwcelery-2.4.1/gwcelery/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tasks/alerts.py` & `gwcelery-2.4.1/gwcelery/tasks/alerts.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tasks/bayestar.py` & `gwcelery-2.4.1/gwcelery/tasks/bayestar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tasks/circulars.py` & `gwcelery-2.4.1/gwcelery/tasks/circulars.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tasks/condor.py` & `gwcelery-2.4.1/gwcelery/tasks/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tasks/core.py` & `gwcelery-2.4.1/gwcelery/tasks/core.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tasks/detchar.py` & `gwcelery-2.4.1/gwcelery/tasks/detchar.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,17 @@
         ts = TimeSeries.read(cache, strain_name,
                              start=long_start, end=long_end).astype('float64')
         # Do q_transforms for the different durations
         qgrams = [ts.q_transform(
             frange=(10, 4096), gps=t0,
             outseg=(t0 - before, t0 + after), logf=True)
             for before, after in durs]
-    except (IndexError, FloatingPointError, ValueError) as err:
+    except FloatingPointError:
+        pass  # don't log this; it means that Virgo is out of observing mode
+    except (IndexError, ValueError) as err:
         # data from cache can't be properly read, or data is weird
         sentry_sdk.capture_exception(err)
         fig = plt.figure(figsize=(4, 1))
         plt.axis("off")
         plt.text(0.5, 0.5, f"Failed to create {ifo} omegascan",
                  horizontalalignment='center', verticalalignment='center',
                  fontsize=17)
```

### Comparing `gwcelery-2.3.6/gwcelery/tasks/em_bright.py` & `gwcelery-2.4.1/gwcelery/tasks/em_bright.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tasks/external_skymaps.py` & `gwcelery-2.4.1/gwcelery/tasks/external_skymaps.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
 NOTICE_TYPE_DICT = {
         '53': 'INTEGRAL_WAKEUP',
         '54': 'INTEGRAL_REFINED',
         '55': 'INTEGRAL_OFFLINE',
         '60': 'SWIFT_BAT_GRB_ALERT',
         '61': 'SWIFT_BAT_GRB_POSITION',
-        '105': 'AGILE_MCAL_ALERT',
         '110': 'FERMI_GBM_ALERT',
         '111': 'FERMI_GBM_FLT_POS',
         '112': 'FERMI_GBM_GND_POS',
         '115': 'FERMI_GBM_FINAL_POS',
         '131': 'FERMI_GBM_SUBTHRESHOLD'
 }
 
@@ -658,15 +657,15 @@
         tail_width = fermi_params[notice_type]["tail_width"]
 
         # Integrate the fermi_error_model using bayestar_adaptive_grid
         skymap = bayestar_adaptive_grid(fermi_error_model, ra, dec, error,
                                         core_width, tail_width, core_weight,
                                         rounds=8)
     else:
-        # Use generic cone method for Swift, INTEGRAL, AGILE, etc.
+        # Use generic cone method for Swift, INTEGRAL, etc.
         skymap = bayestar_adaptive_grid(from_cone, ra, dec, error, rounds=8)
 
     return skymap
 
 
 def write_to_fits(skymap, event, notice_type, notice_date):
     """Write external sky map FITS file, populating the
```

### Comparing `gwcelery-2.3.6/gwcelery/tasks/external_triggers.py` & `gwcelery-2.4.1/gwcelery/tasks/external_triggers.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,46 +76,42 @@
              gcn.NoticeType.FERMI_GBM_GND_POS,
              gcn.NoticeType.FERMI_GBM_FIN_POS,
              gcn.NoticeType.SWIFT_BAT_GRB_POS_ACK,
              gcn.NoticeType.FERMI_GBM_SUBTHRESH,
              gcn.NoticeType.INTEGRAL_WAKEUP,
              gcn.NoticeType.INTEGRAL_REFINED,
              gcn.NoticeType.INTEGRAL_OFFLINE,
-             gcn.NoticeType.AGILE_MCAL_ALERT,
              queue='exttrig',
              shared=False)
 def handle_grb_gcn(payload):
-    """Handles the payload from Fermi, Swift, INTEGRAL, and AGILE MCAL
-    GCN notices.
+    """Handles the payload from Fermi, Swift, and INTEGRAL GCN notices.
 
     Filters out candidates likely to be noise. Creates external events
     from the notice if new notice, otherwise updates existing event. Then
     creates and/or grabs external sky map to be uploaded to the external event.
 
     More info for these notices can be found at:
     Fermi-GBM: https://gcn.gsfc.nasa.gov/fermi_grbs.html
     Fermi-GBM sub: https://gcn.gsfc.nasa.gov/fermi_gbm_subthresh_archive.html
     Swift: https://gcn.gsfc.nasa.gov/swift.html
     INTEGRAL: https://gcn.gsfc.nasa.gov/integral.html
-    AGILE-MCAL: https://gcn.gsfc.nasa.gov/agile_mcal.html
 
     Parameters
     ----------
     payload : str
         XML GCN notice alert packet in string format
 
     """
     root = etree.fromstring(payload)
     u = urlparse(root.attrib['ivorn'])
     stream_path = u.path
 
     stream_obsv_dict = {'/SWIFT': 'Swift',
                         '/Fermi': 'Fermi',
-                        '/INTEGRAL': 'INTEGRAL',
-                        '/AGILE': 'AGILE'}
+                        '/INTEGRAL': 'INTEGRAL'}
     event_observatory = stream_obsv_dict[stream_path]
 
     ext_group = 'Test' if root.attrib['role'] == 'test' else 'External'
 
     #  Block Test INTEGRAL events on the production server to prevent
     #  unneeded queries of old GW data during detchar check
     if event_observatory == 'INTEGRAL' and ext_group == 'Test' and \
@@ -207,15 +203,14 @@
 
 
 @igwn_alert.handler('superevent',
                     'mdc_superevent',
                     'external_fermi',
                     'external_swift',
                     'external_integral',
-                    'external_agile',
                     shared=False)
 def handle_grb_igwn_alert(alert):
     """Parse an IGWN alert message related to superevents/GRB external triggers
     and dispatch it to other tasks.
 
     Notes
     -----
@@ -263,33 +258,40 @@
                     se_searches=['AllSky'],
                     pipelines=[alert['object']['pipeline']])
             else:
                 # launch standard Burst-GRB search
                 raven.coincidence_search(graceid, alert['object'],
                                          group='Burst', se_searches=['AllSky'])
 
-                # launch standard CBC-GRB search
+                # launch standard CBC-GRB search and similar BBH search
                 raven.coincidence_search(graceid, alert['object'],
                                          group='CBC', searches=['GRB'])
+                raven.coincidence_search(graceid, alert['object'],
+                                         group='Burst', searches=['GRB'],
+                                         se_searches=['BBH'])
         elif 'S' in graceid:
             # launch standard GRB search based on group
             gw_group = alert['object']['preferred_event_data']['group']
             search = alert['object']['preferred_event_data']['search']
+            CBC_like = gw_group == 'CBC' or search == 'BBH'
 
             # launch search with MDC events and exit
-            if alert['object']['preferred_event_data']['search'] == 'MDC':
+            if search == 'MDC':
                 raven.coincidence_search(graceid, alert['object'],
                                          group=gw_group, searches=['MDC'])
                 return
-            # Don't run search for BBH or IMBH Burst search
-            elif gw_group == 'Burst' and search.lower() != 'allsky':
+            # Don't run search for IMBH Burst search
+            elif gw_group == 'Burst' and \
+                    search.lower() not in {'allsky', 'bbh'}:
                 return
 
-            se_searches = [] if gw_group == 'CBC' else ['AllSky']
-            searches = (['SubGRB', 'SubGRBTargeted'] if gw_group == 'CBC' else
+            # Keep empty if CBC (field not needed), otherwise use AllSky or BBH
+            se_searches = ([] if gw_group == 'CBC' else
+                           [alert['object']['preferred_event_data']['search']])
+            searches = (['SubGRB', 'SubGRBTargeted'] if CBC_like else
                         ['SubGRBTargeted'])
             # launch standard GRB search
             raven.coincidence_search(graceid, alert['object'],
                                      group=gw_group, searches=['GRB'],
                                      se_searches=se_searches)
             # launch subthreshold search for Fermi and Swift separately to use
             # different time windows, for both CBC and Burst
@@ -437,30 +439,33 @@
     graceid = alert['uid']
 
     if alert['alert_type'] == 'new':
         if alert['object'].get('superevent_id'):
             group = alert['object']['preferred_event_data']['group']
             search = alert['object']['preferred_event_data']['search']
             searches = ['MDC'] if search == 'MDC' else ['Supernova']
+            se_searches = ['MDC'] if search == 'MDC' else ['AllSky']
             # Run only on Test and Burst superevents
-            if group in {'Burst', 'Test'}:
+            if group in {'Burst', 'Test'} and search in {'MDC', 'AllSky'}:
                 raven.coincidence_search(graceid, alert['object'],
                                          group='Burst', searches=searches,
+                                         se_searches=se_searches,
                                          pipelines=['SNEWS'])
         else:
             # Run on SNEWS event, either real or test
             search = alert['object']['search']
             if search == 'MDC':
                 raven.coincidence_search(graceid, alert['object'],
-                                         group='Burst',
+                                         group='Burst', searches=['MDC'],
                                          se_searches=['MDC'],
                                          pipelines=['SNEWS'])
             elif search == 'Supernova':
                 raven.coincidence_search(graceid, alert['object'],
                                          group='Burst', searches=['Supernova'],
+                                         se_searches=['AllSky'],
                                          pipelines=['SNEWS'])
 
 
 @alerts.handler('fermi',
                 'swift')
 def handle_targeted_kafka_alert(alert):
     """Parse an alert sent via Kafka from a MOU partner in our joint
@@ -590,29 +595,27 @@
         GraceDB ID of event
     use_superevent_skymap : bool
         If True/False, use/don't use skymap info from superevent.
         Else if None, check SKYMAP_READY label in external event.
 
     """
     gw_group = superevent['preferred_event_data']['group']
-    tl, th = raven._time_window(graceid, gw_group,
-                                [ext_event['pipeline']],
-                                [ext_event['search']])
+    tl, th = raven._time_window(
+        graceid, gw_group, [ext_event['pipeline']], [ext_event['search']],
+        [superevent['preferred_event_data']['search']])
     # FIXME: both overlap integral and combined sky map could be
     # done by the same function since they are so similar
     use_superevent = (use_superevent_skymap
                       if use_superevent_skymap is not None else
                       'SKYMAP_READY' in ext_event['labels'])
     canvas = raven.raven_pipeline.si(
                  [ext_event] if 'S' in graceid else [superevent],
                  graceid,
                  superevent if 'S' in graceid else ext_event,
                  tl, th, gw_group, use_superevent_skymap=use_superevent)
-    # Swift localizations are incredibly well localized and require
-    # a different method from Fermi/Integral/AGILE
     # Create new updated combined sky map
     canvas |= external_skymaps.create_combined_skymap.si(
                   superevent['superevent_id'], ext_event['graceid'],
                   preferred_event=(
                       None if use_superevent
                       else superevent['preferred_event']))
     canvas.delay()
```

### Comparing `gwcelery-2.3.6/gwcelery/tasks/first2years.py` & `gwcelery-2.4.1/gwcelery/tasks/first2years.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tasks/first2years_external.py` & `gwcelery-2.4.1/gwcelery/tasks/first2years_external.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     new_TrigID = str(int(gpstime))
     ra = random.uniform(0, 360)
     thetas = np.arange(-np.pi / 2, np.pi / 2, .01)
     dec = random.choices(np.rad2deg(thetas),
                          weights=np.cos(thetas) / sum(np.cos(thetas)))[0]
     error = .05 if pipeline == 'Swift' else random.uniform(1, 30)
 
-    if pipeline in {'Fermi', 'Swift', 'INTEGRAL', 'AGILE'}:
+    if pipeline in {'Fermi', 'Swift', 'INTEGRAL'}:
         is_grb = True
     else:
         is_grb = False
 
     # If SubGRBTargeted modify alert packet from Kafka
     if ext_search == 'SubGRBTargeted':
         if pipeline == 'Fermi':
@@ -134,37 +134,40 @@
             external_triggers.handle_grb_gcn(event)
         else:
             external_triggers.handle_snews_gcn(event)
 
         return event
 
 
-def _offset_time(gpstime, group, pipeline, ext_search):
+def _offset_time(gpstime, group, pipeline, ext_search, se_search):
     """Offsets the given GPS time by applying a random number within a time
     window, determine by the search being done.
 
     Parameters
     ----------
     gpstime : float
         Event's GPS time
     group : str
         Burst or CBC
     pipeline : str
         Pipeline field for external event
     ext_search : str
         Search field for external event
+    se_search : list
+        Search field for superevent
 
     Returns
     -------
     gsptime_adjusted : float
         Event's original gps time plus a random number within the determined
         search window
 
     """
-    tl, th = raven._time_window('S1', group, [pipeline], [ext_search])
+    tl, th = raven._time_window('S1', group, [pipeline],
+                                [ext_search], [se_search])
     return gpstime + random.uniform(tl, th)
 
 
 def _is_joint_mdc(graceid, se_search):
     """Determine whether to upload an external events using user-defined
     frequency of MDC or AllSky superevents.
 
@@ -231,18 +234,18 @@
     if alert['alert_type'] != 'new':
         return
     se_search = alert['object']['preferred_event_data']['search']
     group = alert['object']['preferred_event_data']['group']
     is_gracedb_playground = app.conf['gracedb_host'] \
         == 'gracedb-playground.ligo.org'
     joint_mdc_alert = se_search == 'MDC' and _is_joint_mdc(alert['uid'], 'MDC')
-    joint_allsky_alert = se_search == 'AllSky' and \
+    joint_o3replay_alert = se_search in {'AllSky', 'BBH'} and \
         _is_joint_mdc(alert['uid'], 'AllSky') and is_gracedb_playground and \
         group in {'CBC', 'Burst'}
-    if not (joint_mdc_alert or joint_allsky_alert):
+    if not (joint_mdc_alert or joint_o3replay_alert):
         return
 
     # Potentially upload 1, 2, or 3 GRB events
     num = 1 + np.random.choice(np.arange(3), p=[.6, .3, .1])
 
     if joint_mdc_alert:
         # If joint MDC alert, make external event MDC
@@ -254,31 +257,32 @@
             raise ValueError('External search must be "MDC" if MDC superevent')
     # If O3 replay, choose search from acceptable list
     elif ext_search is None:
         # Determine search for external event and then pipelines
         ext_search = \
             (np.random.choice(['GRB', 'SubGRB', 'SubGRBTargeted'],
                               p=[.6, .1, .3])
-             if joint_allsky_alert else 'GRB')
+             if joint_o3replay_alert else 'GRB')
     # Choose pipeline(s) based on search
     if ext_search in {'GRB', 'MDC'}:
-        pipelines = np.random.choice(['Fermi', 'Swift', 'INTEGRAL', 'AGILE'],
-                                     p=[.5, .3, .1, .1],
+        pipelines = np.random.choice(['Fermi', 'Swift', 'INTEGRAL'],
+                                     p=[.6, .3, .1,],
                                      size=num, replace=False)
     elif ext_search == 'SubGRB':
         pipelines = np.full(num, 'Fermi')
     elif ext_search == 'SubGRBTargeted':
         # Only two current pipelines in targeted search so map 3 => 2
         num = min(num, 2)
         pipelines = np.random.choice(['Fermi', 'Swift'],
                                      p=[.5, .5], size=num, replace=False)
     events = []
     for pipeline in pipelines:
         gpstime = float(alert['object']['t_0'])
-        new_time = _offset_time(gpstime, group, pipeline, ext_search)
+        new_time = _offset_time(gpstime, group, pipeline,
+                                ext_search, se_search)
 
         # Choose external grb pipeline to simulate
         ext_event = create_upload_external_event(
                         new_time, pipeline, ext_search)
 
         events.append(ext_event)
```

### Comparing `gwcelery-2.3.6/gwcelery/tasks/gcn.py` & `gwcelery-2.4.1/gwcelery/tasks/gcn.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tasks/gracedb.py` & `gwcelery-2.4.1/gwcelery/tasks/gracedb.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,22 +20,23 @@
     """Exception class for server-side HTTP errors that we should retry."""
 
 
 def catch_retryable_http_errors(f):
     """Decorator to capture server-side errors that we should retry.
 
     We retry HTTP status 502 (Bad Gateway), 503 (Service Unavailable), and
-    504 (Gateway Timeout).
+    504 (Gateway Timeout). We also retry client side error codes 408 (Timeout),
+    409 (Conflicting URL), 429 (Too many requests).
     """
     @functools.wraps(f)
     def wrapper(*args, **kwargs):
         try:
             return f(*args, **kwargs)
         except HTTPError as e:
-            if e.response.status_code in {408, 429, 502, 503, 504}:
+            if e.response.status_code in {408, 409, 429, 500, 502, 503, 504}:
                 raise RetryableHTTPError(
                     *e.args, request=e.request, response=e.response)
             else:
                 raise
 
     return wrapper
 
@@ -353,7 +354,43 @@
     try:
         client.superevents[superevent_id].add(graceid)
     except HTTPError as e:
         error_msg = b'is already assigned to a Superevent'
         if not (e.response.status_code == 400
                 and error_msg in e.response.content):
             raise
+
+
+@task(shared=False)
+@catch_retryable_http_errors
+def get_superevent_file_list(superevent_id):
+    """Get superevent file list from GraceDB."""
+    filelist = client.superevents[superevent_id].files.get()
+    return filelist
+
+
+@task(shared=False)
+@catch_retryable_http_errors
+def get_latest_file(superevent_id, filename):
+    """Get the lastest file provided a file name
+
+    Parameters
+    ----------
+    superevent_id : str
+        superevent uid
+
+    file_name : str
+        The filebase of a file name
+        e.g. 'bayestar.multiorder.fits' for 'bayestar.multiorder.fits,0'
+
+    Returns
+    ----------
+        The versioned filename for the inquired file
+    """
+    # Get file list for superevent
+    file_list = get_superevent_file_list(superevent_id)
+    # Loop over the keys and mark the key if key includes filename
+    keys = [key for key in file_list.keys() if filename in key]
+    if any(keys):
+        return max(keys)
+    else:
+        return None
```

### Comparing `gwcelery-2.3.6/gwcelery/tasks/gwskynet.py` & `gwcelery-2.4.1/gwcelery/tasks/gwskynet.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,42 +21,53 @@
     # slow operation
     from GWSkyNet import GWSkyNet
 
     return GWSkyNet.load_GWSkyNet_model()
 
 
 @app.task(queue='skynet', shared=False)
-def gwskynet_annotation(filecontents, SNRs):
+def gwskynet_annotation(input_list, SNRs, superevent_id):
     """Perform the series of tasks necessary for GWSkyNet to
 
     Parameters
     ----------
-    filecontents : bytes
-            the sky map downloaded from gracedb
-    GWSkyNet_model : keras.engine.functional.Functional object
-            the GWSkyNet model used to annotate the events
+    input_list : list
+        The output of _download_and_keep_file_name that includes the
+        downloaded the skymap and the versioned file name of the skymap.
+        This list is in the form [skymap, skymap_filename].
+    snr : numpy array of floats
+        detector SNRs.
+    superevent_id : str
+        superevent uid
+    skymap_filename : str
+        versioned filename for skymap
     """
     # FIXME Remove import from function scope once importing GWSkyNet is not a
     # slow operation
     from GWSkyNet import GWSkyNet
 
+    filecontents, skymap_filename = input_list
     with NamedTemporaryFile(content=filecontents) as fitsfile:
         GWSkyNet_input = GWSkyNet.prepare_data(fitsfile.name)
     # One of the inputs from BAYESTAR to GWSkyNet is the list of instruments,
     # i.e., metadata['instruments'], which is converted to a binary array with
     # three elements, i.e. GWSkyNet_input[2], for H1, L1 and V1.
     # GWSkyNet 2.4.0 uses this array to indicate detector with SNR >= 4.5
     GWSkyNet_input[2][0] = np.where(SNRs >= app.conf['gwskynet_snr_threshold'],
                                     1, 0)
-    class_score = GWSkyNet.predict(GWSkyNet_model(), GWSkyNet_input)
-    FAP, FNP = GWSkyNet.get_rates(class_score)
+    gwskynet_score = GWSkyNet.predict(GWSkyNet_model(), GWSkyNet_input)
+    FAP, FNP = GWSkyNet.get_rates(gwskynet_score)
     fap = FAP[0]
     fnp = FNP[0]
-    cs = class_score[0]
-    gwskynet_output = {'class_score': cs, 'FAP': fap, 'FNP': fnp}
+    gs = gwskynet_score[0]
+    gwskynet_output = {'superevent_id': superevent_id,
+                       'file': skymap_filename,
+                       'GWSkyNet_score': gs,
+                       'GWSkyNet_FAP': fap,
+                       'GWSkyNet_FNP': fnp}
     return json.dumps(gwskynet_output)
 
 
 def get_cbc_event_snr(event):
     """Get detector SNRs from the LVAlert packet.
 
     Parameters
@@ -84,32 +95,41 @@
             snr[1] = det['snr']
         if det['ifo'] == 'V1':
             snr[2] = det['snr']
     return snr
 
 
 @gracedb.task(shared=False)
-def _unpack_gwskynet_annotation_and_upload(gwskynet_output, skymap_filename,
-                                           graceid):
+def _download_and_return_file_name(filename, graceid):
+    """Wrapper around gracedb.download that returns the file name."""
+    filecontents = gracedb.download(filename, graceid)
+    return [filecontents, filename]
+
+
+@gracedb.task(shared=False)
+def _unpack_gwskynet_annotation_and_upload(gwskynet_output, graceid):
     filename = 'gwskynet.json'
     gwskynet_output_dict = json.loads(gwskynet_output)
     message = ('GWSkyNet annotation from <a href='
                '"/api/events/{graceid}/files/'
                '{skymap_filename}">'
                '{skymap_filename}</a>.'
-               ' GWSkyNet class score: {cs},'
-               ' FAP: {FAP}, FNP: {FNP}.').format(
+               ' GWSkyNet score: {cs},'
+               ' GWSkyNet FAP: {GWSkyNet_FAP},'
+               ' GWSkyNet FNP: {GWSkyNet_FNP}.').format(
                    graceid=graceid,
-                   skymap_filename=skymap_filename,
-                   cs=np.round(gwskynet_output_dict['class_score'], 3),
-                   FAP=np.round(gwskynet_output_dict['FAP'], 3),
-                   FNP=np.round(gwskynet_output_dict['FNP'], 3)
+                   skymap_filename=gwskynet_output_dict['file'],
+                   cs=np.round(gwskynet_output_dict['GWSkyNet_score'], 3),
+                   GWSkyNet_FAP=np.round(gwskynet_output_dict['GWSkyNet_FAP'],
+                                         3),
+                   GWSkyNet_FNP=np.round(gwskynet_output_dict['GWSkyNet_FNP'],
+                                         3)
                 )
     return gracedb.upload(gwskynet_output, filename, graceid, message=message,
-                          tags=['em_follow'])
+                          tags=['em_follow', 'public'])
 
 
 def _should_annotate(preferred_event, new_label, new_log_comment, labels,
                      alert_type):
     # First check if the event passes all of GWSkyNet's annotation criteria
     SNRs = get_cbc_event_snr(preferred_event)
 
@@ -160,25 +180,25 @@
         return
 
     if alert['alert_type'] != 'label_added' and \
             alert['alert_type'] != 'log':
         return
 
     superevent_id = alert['uid']
-    skymap_filename = 'bayestar.multiorder.fits'
     preferred_event = alert['object']['preferred_event_data']
     new_label = alert['data'].get('name', '')
     new_log_comment = alert['data'].get('comment', '')
     labels = alert['object'].get('labels', [])
     SNRs = get_cbc_event_snr(preferred_event)
 
     if _should_annotate(preferred_event, new_label, new_log_comment, labels,
                         alert['alert_type']):
         (
-            gracedb.download.s(skymap_filename,
-                               superevent_id)
+            gracedb.get_latest_file.s(superevent_id,
+                                      'bayestar.multiorder.fits')
+            |
+            _download_and_return_file_name.s(superevent_id)
             |
-            gwskynet_annotation.s(SNRs)
+            gwskynet_annotation.s(SNRs, superevent_id)
             |
-            _unpack_gwskynet_annotation_and_upload.s(
-                skymap_filename, superevent_id)
+            _unpack_gwskynet_annotation_and_upload.s(superevent_id)
         ).apply_async()
```

### Comparing `gwcelery-2.3.6/gwcelery/tasks/igwn_alert.py` & `gwcelery-2.4.1/gwcelery/tasks/igwn_alert.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tasks/inference.py` & `gwcelery-2.4.1/gwcelery/tasks/inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,22 +202,22 @@
         raise
 
     return os.path.join(rundir, 'multidag.dag')
 
 
 @app.task(shared=False)
 def _setup_dag_for_bilby(
-    coinc, rundir, event, superevent_id, mode="production"
+    coinc_bayestar, rundir, event, superevent_id, mode="production"
 ):
     """Create DAG for a bilby run and return the path to DAG.
 
     Parameters
     ----------
-    coinc : bytes
-        Byte contents of ``coinc.xml``. The PSD is expected to be embedded.
+    coinc_bayestar : tuple
+        Byte contents of ``coinc.xml`` and ``bayestar.multiorder.fits``.
     rundir : str
         The path to a run directory where the DAG file is created
     event : dict
         The json contents of a target G event retrieved from
         gracedb.get_event(), whose mass and spin information are used to
         determine analysis settings.
     superevent_id : str
@@ -239,29 +239,35 @@
     is `gracedb.ligo.org`, and `Online_PE_MDC` otherwise.
 
     """
     path_to_json = os.path.join(rundir, 'event.json')
     with open(path_to_json, 'w') as f:
         json.dump(event, f, indent=2)
 
+    coinc, bayestar = coinc_bayestar
     path_to_psd = os.path.join(rundir, 'coinc.xml')
     with open(path_to_psd, 'wb') as f:
         f.write(coinc)
+    path_to_bayestar = os.path.join(rundir, 'bayestar.multiorder.fits')
+    with open(path_to_bayestar, 'wb') as f:
+        f.write(bayestar)
 
     path_to_webdir = os.path.join(
         app.conf['pe_results_path'], superevent_id, 'bilby', mode
     )
 
     path_to_settings = os.path.join(rundir, 'settings.json')
     setup_arg = ['bilby_pipe_gracedb', '--webdir', path_to_webdir,
                  '--outdir', rundir, '--json', path_to_json,
-                 '--psd-file', path_to_psd, '--settings', path_to_settings]
+                 '--psd-file', path_to_psd, '--skymap-file', path_to_bayestar,
+                 '--settings', path_to_settings]
     settings = {'summarypages_arguments': {'gracedb': event['graceid'],
                                            'no_ligo_skymap': True},
-                'accounting_user': 'soichiro.morisaki'}
+                'accounting_user': 'soichiro.morisaki',
+                'tukey_roll_off': 1.0}
     if app.conf['gracedb_host'] != 'gracedb.ligo.org':
         settings['queue'] = 'Online_PE_MDC'
     else:
         settings['queue'] = 'Online_PE'
         settings['accounting'] = 'ligo.prod.o4.cbc.pe.bilby'
     # FIXME: using live data for gracedb-test events should be reconsidered
     # when we have a better idea to differentiate MDC and real events.
@@ -298,16 +304,24 @@
             likelihood_mode = 'phenompv2_bns_roq'
         # use IMRPhenomPv2 with mass ratio upper bound of 20 in chirp-mass
         # range where IMRPhenomXPHM ROQ bases are not available
         elif trigger_chirp_mass < 12:
             likelihood_mode = 'low_q_phenompv2_roq'
         else:
             likelihood_mode = 'phenomxphm_roq'
-            settings['request_memory_generation'] = 36.0
-            settings['request_memory'] = 16.0
+            if trigger_chirp_mass > 16:
+                settings['request_memory_generation'] = 36.0
+            else:
+                settings['request_memory_generation'] = 50.0
+            if trigger_chirp_mass > 25:
+                settings['request_memory'] = 16.0
+            elif trigger_chirp_mass > 16:
+                settings['request_memory'] = 24.0
+            else:
+                settings['request_memory'] = 36.0
         setup_arg += ['--cbc-likelihood-mode', likelihood_mode]
     elif mode == 'fast_test':
         setup_arg += ["--sampler-kwargs", "FastTest"]
         if trigger_chirp_mass < 3.9:
             setup_arg += ['--cbc-likelihood-mode', 'phenompv2_bns_roq']
             settings['request_memory_generation'] = 8.0
     else:
@@ -467,17 +481,20 @@
     # List of environment variables `condor_submit_dag` should be aware of.
     include_env = None
 
     if pe_pipeline == 'lalinference':
         canvas = gracedb.download.si('coinc.xml', event['graceid']) | \
             _setup_dag_for_lalinference.s(rundir, event, superevent_id)
     elif pe_pipeline == 'bilby':
-        canvas = gracedb.download.si('coinc.xml', event['graceid']) | \
-            _setup_dag_for_bilby.s(
-                rundir, event, superevent_id, kwargs['bilby_mode'])
+        canvas = group(
+            gracedb.download.si('coinc.xml', event['graceid']),
+            gracedb.download.si('bayestar.multiorder.fits', event['graceid'])
+        ) | _setup_dag_for_bilby.s(
+            rundir, event, superevent_id, kwargs['bilby_mode']
+        )
     elif pe_pipeline == 'rapidpe':
         canvas = _setup_dag_for_rapidpe.s(rundir, superevent_id, event)
         include_env = RAPIDPE_GETENV
     else:
         raise NotImplementedError(f'Unknown PE pipeline {pe_pipeline}.')
 
     canvas |= _condor_no_submit.s(include_env=include_env)
```

### Comparing `gwcelery-2.3.6/gwcelery/tasks/legacy_gracedb.py` & `gwcelery-2.4.1/gwcelery/tasks/legacy_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tasks/notice_text.py` & `gwcelery-2.4.1/gwcelery/tasks/notice_text.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tasks/orchestrator.py` & `gwcelery-2.4.1/gwcelery/tasks/orchestrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,35 +37,29 @@
     if alert['alert_type'] == 'new':
         # launching rapidpe 30s after merger.
         timeout = max(
             alert['object']['t_0'] - Time.now().gps +
             app.conf['rapidpe_timeout'], 0
         )
         (
-            _get_preferred_event.si(superevent_id).set(
+            gracedb.get_superevent.si(superevent_id).set(
                 countdown=timeout
             )
             |
-            group(
-                _get_cbc_lowest_far.si(superevent_id),
-                gracedb.get_event.s()
-            )
+            _get_pe_far_and_event.s()
             |
             parameter_estimation.s(superevent_id, 'rapidpe')
         ).apply_async()
 
         (
-            _get_preferred_event.si(superevent_id).set(
+            gracedb.get_superevent.si(superevent_id).set(
                 countdown=app.conf['pe_timeout']
             )
             |
-            group(
-                _get_cbc_lowest_far.si(superevent_id),
-                gracedb.get_event.s()
-            )
+            _get_pe_far_and_event.s()
             |
             parameter_estimation.s(superevent_id, 'bilby')
         ).apply_async()
 
         # run check_vectors. Create and upload omegascans
         group(
             detchar.omegascan.si(alert['object']['t_0'], superevent_id),
@@ -545,27 +539,14 @@
                                   t_0=event["gpstime"])
         gracedb.upload.delay(
             None, None, superevent_id,
             comment=f'DQOK applied based on new event {event_id}')
 
 
 @gracedb.task(shared=False)
-def _get_preferred_event(superevent_id):
-    """Determine preferred event for a superevent by querying GraceDB.
-
-    This works just like :func:`gwcelery.tasks.gracedb.get_superevent`, except
-    that it returns only the preferred event, and not the entire GraceDB JSON
-    response.
-    """
-    # FIXME: remove ._orig_run when this bug is fixed:
-    # https://github.com/getsentry/sentry-python/issues/370
-    return gracedb.get_superevent._orig_run(superevent_id)['preferred_event']
-
-
-@gracedb.task(shared=False)
 def _create_voevent(classification, *args, **kwargs):
     r"""Create a VOEvent record from an EM bright JSON file.
 
     Parameters
     ----------
     classification : tuple, None
         A collection of JSON strings, generated by
@@ -913,14 +894,23 @@
 
     # Send notice and upload GCN circular draft for online events.
     if is_publishable and initiate_voevent:
         # presence of advocate action blocks significant prelim alert
         # presence of adv action or significant event blocks EW alert
         # presence of adv action or significant event or EW event blocks
         # less significant alert
+        if alert_type == 'earlywarning':
+            # Launch DQR for significant early warning events after a timeout.
+            # If a full BW significant trigger arrives before the end of the
+            # timeout, the latter will apply the label instead, and this call
+            # is a noop.
+            gracedb.create_label.si(
+                'DQR_REQUEST',
+                superevent_id
+            ).apply_async(countdown=600)
         blocking_labels = (
             {'ADVOK', 'ADVNO'} if alert_type == 'preliminary'
             else
             {superevents.SIGNIFICANT_LABEL, 'ADVOK', 'ADVNO'}
             if alert_type == 'earlywarning'
             else
             {superevents.EARLY_WARNING_LABEL, superevents.SIGNIFICANT_LABEL,
@@ -937,55 +927,70 @@
             )
         )
 
     canvas.apply_async(priority=priority)
 
 
 @gracedb.task(shared=False)
-def _get_cbc_lowest_far(superevent_id):
-    """Obtain the lowest FAR of the CBC events in the target superevent."""
+def _get_pe_far_and_event(superevent):
+    """Return FAR and event input to PE workflow.
+
+    The input FAR is the lowest FAR among CBC and Burst-BBH triggers.
+    The input event is the preferred event if it is a CBC trigger, otherwise
+    the CBC trigger with the lowest FAR is returned.
+    """
     # FIXME: remove ._orig_run when this bug is fixed:
     # https://github.com/getsentry/sentry-python/issues/370
     events = [
-        gracedb.get_event._orig_run(gid) for gid in
-        gracedb.get_superevent._orig_run(superevent_id)["gw_events"]
+        gracedb.get_event._orig_run(gid) for gid in superevent['gw_events']
     ]
-    return min(
-        [e['far'] for e in events if e['group'].lower() == 'cbc'],
-        default=None
-    )
+    events = [
+        e for e in events if e['group'].lower() == 'cbc' or (
+            e['group'].lower() == 'burst' and
+            e.get('search', 'None').lower() == 'bbh'
+        )
+    ]
+    events.sort(key=lambda e: e['far'])
+    preferred_event = superevent['preferred_event_data']
+
+    if preferred_event['group'].lower() == 'cbc':
+        return events[0]['far'], preferred_event
+    for e in events:
+        if e['group'].lower() == 'cbc':
+            return events[0]['far'], e
+    return None
 
 
 @app.task(ignore_result=True, shared=False)
 def parameter_estimation(far_event, superevent_id, pe_pipeline):
     """Parameter Estimation with Bilby and RapidPE-RIFT. Parameter estimation
     runs are triggered for CBC triggers which pass the FAR threshold and are
     not mock uploads. For those which do not pass these criteria, this task
     uploads messages explaining why parameter estimation is not started.
     """
+    if far_event is None:
+        gracedb.upload.delay(
+            filecontents=None, filename=None,
+            graceid=superevent_id,
+            message='Parameter estimation will not start since no CBC triggers'
+                    ' are found.',
+            tags='pe'
+        )
+        return
     far, event = far_event
-    group = event['group'].lower()
     search = event['search'].lower()
     if search in app.conf['significant_alert_far_threshold']['cbc']:
         threshold = (
             app.conf['significant_alert_far_threshold']['cbc'][search] /
             app.conf['significant_alert_trials_factor']['cbc'][search]
         )
     else:
         # Fallback in case an event is uploaded to an unlisted search
         threshold = -1 * float('inf')
-    if group != 'cbc':
-        gracedb.upload.delay(
-            filecontents=None, filename=None,
-            graceid=superevent_id,
-            message='Parameter estimation will not start since this is not '
-                    'CBC but {}.'.format(event['group']),
-            tags='pe'
-        )
-    elif far > threshold:
+    if far > threshold:
         gracedb.upload.delay(
             filecontents=None, filename=None,
             graceid=superevent_id,
             message='Parameter estimation will not start since FAR is larger '
                     'than the PE threshold, {}  Hz.'.format(threshold),
             tags='pe'
         )
@@ -1015,18 +1020,15 @@
             filecontents=None, filename=None,
             graceid=superevent_id,
             message='Parameter estimation is disabled for MBTA triggers '
                     'on playground as MBTA analyses live data + online '
                     'injections not O3 replay data + MDC injections',
             tags='pe'
         )
-    elif (
-            pe_pipeline == 'rapidpe' and
-            event['search'].lower() == 'earlywarning'
-    ):
+    elif pe_pipeline == 'rapidpe' and search == 'earlywarning':
         # Remove this if rapidpe can ingest early warning events
         gracedb.upload.delay(
             filecontents=None, filename=None,
             graceid=superevent_id,
             message='Parameter estimation by RapidPE-RIFT is disabled for '
                     'earlywarning triggers.',
             tags='pe'
@@ -1105,25 +1107,24 @@
                     and 'combined' not in f:
                 skymap_filename = fv
             if em_bright_needed \
                     and 'em_bright' in t \
                     and f.endswith('.json'):
                 em_bright_filename = fv
             if p_astro_needed \
-                    and {'public'}.issubset(t) \
-                    and 'p_astro' in t \
+                    and {'p_astro', 'public'}.issubset(t) \
                     and f.endswith('.json'):
                 p_astro_filename = fv
             if combined_skymap_needed \
                     and {'sky_loc', 'ext_coinc'}.issubset(t) \
                     and f.startswith('combined-ext.') \
                     and 'fit' in f:
                 combined_skymap_filename = fv
             if rapidpe_pastro_needed \
-                    and 'p_astro' in t \
+                    and {'p_astro', 'public'}.issubset(t) \
                     and f == 'RapidPE_RIFT.p_astro.json':
                 rapidpe_pastro_filename = fv
 
     if combined_skymap_needed:
         # for every alert, copy combined sky map over if applicable
         # FIXME: use file inheritance once available
         ext_id = superevent['em_type']
```

### Comparing `gwcelery-2.3.6/gwcelery/tasks/p_astro.py` & `gwcelery-2.4.1/gwcelery/tasks/p_astro.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tasks/raven.py` & `gwcelery-2.4.1/gwcelery/tasks/raven.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .. import app
 from . import external_skymaps, gracedb
 from .core import identity
 
 log = get_task_logger(__name__)
 
 
-@app.task(shared=False)
+@gracedb.task(shared=False)
 def calculate_coincidence_far(superevent, exttrig, tl, th,
                               use_superevent_skymap=None):
     """Compute coincidence FAR for external trigger and superevent coincidence
     by calling ligo.raven.search.calc_signif_gracedb, using sky map info if
     available.
 
     Parameters
@@ -117,25 +117,25 @@
         List of external trigger pipeline names
     searches : list
         List of external trigger searches
     se_searches : list
         List of superevent searches
 
     """
-    tl, th = _time_window(gracedb_id, group, pipelines, searches)
+    tl, th = _time_window(gracedb_id, group, pipelines, searches, se_searches)
 
     (
         search.si(gracedb_id, alert_object, tl, th, group, pipelines,
                   searches, se_searches)
         |
         raven_pipeline.s(gracedb_id, alert_object, tl, th, group)
     ).delay()
 
 
-def _time_window(gracedb_id, group, pipelines, searches):
+def _time_window(gracedb_id, group, pipelines, searches, se_searches):
     """Determine the time window to use given the parameters of the search.
 
     Parameters
     ----------
     gracedb_id : str
         GraceDB ID of the trigger that launched RAVEN
     group : str
@@ -168,29 +168,29 @@
         if 'Fermi' in pipelines:
             tl, th = tl_subfermi, th_subfermi
         elif 'Swift' in pipelines:
             tl, th = tl_subswift, th_subswift
         else:
             raise ValueError('Specify Fermi or Swift as pipeline when ' +
                              'launching subthreshold search')
-    elif group == 'CBC':
+    elif group == 'CBC' or 'BBH' in se_searches:
         tl, th = tl_cbc, th_cbc
     elif group == 'Burst':
         tl, th = tl_burst, th_burst
     else:
         raise ValueError('Invalid RAVEN search request for {0}'.format(
             gracedb_id))
     if 'S' in gracedb_id:
         # If triggering on a superevent, need to reverse the time window
         tl, th = -th, -tl
 
     return tl, th
 
 
-@app.task(shared=False)
+@gracedb.task(shared=False)
 def search(gracedb_id, alert_object, tl=-5, th=5, group=None,
            pipelines=[], searches=[], se_searches=[]):
     """Perform ligo-raven search to look for coincidences. This function
     does a query of GraceDB and uploads a log message of the result(s).
 
     Parameters
     ----------
@@ -270,26 +270,37 @@
             superevent = result
             ext_event = alert_object
         # Don't continue if it is a different superevent than previous one.
         if ext_event['superevent'] is not None \
                 and ext_event['superevent'] != superevent['superevent_id']:
             return
 
+        # Always check publishing conditions and apply EM_COINC to external
+        # event so we can re-run the analysis if NOT_GRB is removed
+        group_canvas = \
+            trigger_raven_alert.s(superevent, gracedb_id, ext_event, gw_group),
+
+        # If the external event is not likely astrophysical and part of the
+        # targeted search, don't alert observers or redo calculations.
+        # This is to prevent large influxes of EM_COINC alerts that will never
+        # really be considered now or in the future
+        if 'NOT_GRB' not in ext_event['labels'] and \
+                ext_event['search'] != 'SubGRBTargeted':
+            group_canvas += gracedb.create_label.si('EM_COINC', superevent_id),
+            group_canvas += gracedb.create_label.si('EM_COINC', exttrig_id),
+
         canvas = (
             gracedb.add_event_to_superevent.si(superevent_id, exttrig_id)
             |
             calculate_coincidence_far.si(
                 superevent, ext_event, tl, th,
                 use_superevent_skymap=use_superevent_skymap
             )
             |
-            group(gracedb.create_label.si('EM_COINC', superevent_id),
-                  gracedb.create_label.si('EM_COINC', exttrig_id),
-                  trigger_raven_alert.s(superevent, gracedb_id,
-                                        ext_event, gw_group))
+            group(group_canvas)
         )
         canvas.delay()
 
 
 @app.task(shared=False)
 def preferred_superevent(raven_search_results):
     """Chooses the superevent with the lowest FAR for an external
@@ -308,15 +319,15 @@
 
     """
     minfar, idx = min((result['far'], idx) for (idx, result) in
                       enumerate(raven_search_results))
     return [raven_search_results[idx]]
 
 
-@app.task(shared=False)
+@app.task(queue='exttrig', shared=False)
 def update_coinc_far(coinc_far_dict, superevent, ext_event):
     """Update joint info in superevent based on the current preferred
     coincidence. In order of priority, the determing conditions are the
     following:
 
     * A SNEWS coincidence is preferred over GRB.
     * Likely astrophysical external candidates are preferred over likely
```

### Comparing `gwcelery-2.3.6/gwcelery/tasks/rrt_utils.py` & `gwcelery-2.4.1/gwcelery/tasks/rrt_utils.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tasks/skymaps.py` & `gwcelery-2.4.1/gwcelery/tasks/skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tasks/superevents.py` & `gwcelery-2.4.1/gwcelery/tasks/superevents.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,19 +63,17 @@
                     shared=False)
 def handle(payload):
     """Respond to IGWN alert topics from low-latency search pipelines and
     delegate to :meth:`process` for superevent management.
     """
     alert_type = payload['alert_type']
     gid = payload['object']['graceid']
-    alert_group = payload['object']['group'].lower()
     alert_search = payload['object']['search']
 
-    ifos = get_instruments(payload['object']) if alert_group == 'cbc' \
-        else payload['object']['instruments'].split(',')
+    ifos = get_instruments(payload['object'])
     # Ignore inclusion of events involving KAGRA; revert when policy is changed
     if "K1" in ifos:
         log.info('Skipping %s because it involves KAGRA data', gid)
         return
     # Ignore inclusion of events from VT search
     if alert_search == VT_SEARCH_NAME:
         log.info("Skipping {} event {}".format(VT_SEARCH_NAME, gid))
@@ -337,18 +335,26 @@
         :meth:`gwcelery.tasks.gracedb.get_event`, or
         ``preferred_event_data`` in igwn-alert packet.)
 
     Returns
     -------
     set
         The set of instruments that contributed to the event.
-
+        The instruments that contributed to the event are
+        generally stored in the instrument field of the G-event
+        as a comma separated list. For pipeline that
+        provide the 'SingleInspiral' use the list
+        of the detector there.
     """
-    attribs = event['extra_attributes']['SingleInspiral']
-    ifos = {single['ifo'] for single in attribs}
+    if (('extra_attributes' in event) and
+       ('SingleInspiral' in event['extra_attributes'])):
+        attribs = event['extra_attributes']['SingleInspiral']
+        ifos = {single['ifo'] for single in attribs}
+    else:
+        ifos = set(event['instruments'].split(','))
     return ifos
 
 
 def get_instruments_in_ranking_statistic(event):
     """Get the instruments that contribute to the false alarm rate.
 
     Parameters
@@ -366,31 +372,27 @@
 
     Notes
     -----
     The number of instruments that contributed *data* to an event is given by
     the ``instruments`` key of the GraceDB event JSON structure. However, some
     pipelines (e.g. gstlal) have a distinction between which instruments
     contributed *data* and which were considered in the *ranking* of the
-    candidate. For such pipelines, we infer which pipelines contributed to the
-    ranking by counting only the SingleInspiral records for which the chi
-    squared field is non-empty.
-
-    For PyCBC Live in the O3 configuration, an empty chi^2 field does not mean
-    that the detector did not contribute to the ranking; in fact, *all*
-    detectors listed in the SingleInspiral table contribute to the significance
-    even if the chi^2 is not computed for some of them. Hence PyCBC Live is
-    handled as a special case.
+    candidate. All the pipeline should conform to this rule.
 
+    Unmodeled searches do not provide a SingleInspiral table, In such case
+    use the event information.
     """
-    if event['pipeline'].lower() == 'pycbc':
-        return set(event['instruments'].split(','))
-    else:
+    if (('extra_attributes' in event) and
+       ('SingleInspiral' in event['extra_attributes'])):
         attribs = event['extra_attributes']['SingleInspiral']
-        return {single['ifo'] for single in attribs
+        ifos = {single['ifo'] for single in attribs
                 if single.get('chisq') is not None}
+    else:
+        ifos = set(event['instruments'].split(','))
+    return ifos
 
 
 @app.task(shared=False)
 def select_pipeline_preferred_event(events):
     """Group list of G events by pipeline, and apply :meth:`keyfunc`
     to select the pipeline preferred events.
```

### Comparing `gwcelery-2.3.6/gwcelery/templates/fits_header.jinja2` & `gwcelery-2.4.1/gwcelery/templates/fits_header.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/templates/index.jinja2` & `gwcelery-2.4.1/gwcelery/templates/index.jinja2`

 * *Files 1% similar despite different names*

```diff
@@ -114,29 +114,39 @@
     <div class="card mb-3">
         <div class=card-header>
             Issue Update GCN Notice
         </div>
         <div class=card-body>
             <form method=post action="{{ url_for('send_update_gcn') }}">
                 <div class="form-row">
+                    <div class=form-group>
+                        <div class=form-text>Send an update GCN notice using the chosen fields.</div>
+                    </div>
+                </div>
+                <div class="form-row">
+                    <div class=form-group>
+                        <p class="text-danger">Note: the filenames must end with the comma version and not contain spaces, e.g. bayestar.multiorder.fits,0.</p>
+                    </div>
+                </div>
+                <div class="form-row">
                     <div class="form-group col-md">
                         <label for=superevent_id>Superevent ID</label>
                         <input required name=superevent_id class="form-control typeahead">
                     </div>
                     <div class="form-group col-md">
                         <label for=skymap_filename>Sky Map File</label>
-                        <input required name=skymap_filename class="form-control superevent-dependent typeahead" data-typeahead-url-template="{{ url_for('typeahead_skymap_filename', superevent_id='SUPEREVENT_ID', filename='TERM') }}">
+                        <input required name=skymap_filename pattern="\S+,\d+$" class="form-control superevent-dependent typeahead" data-typeahead-url-template="{{ url_for('typeahead_skymap_filename', superevent_id='SUPEREVENT_ID', filename='TERM') }}">
                     </div>
                     <div class="form-group col-md">
                         <label for=em_bright_filename>Classification File</label>
-                        <input required name=em_bright_filename class="form-control superevent-dependent typeahead" data-typeahead-url-template="{{ url_for('typeahead_em_bright_filename', superevent_id='SUPEREVENT_ID', filename='TERM') }}">
+                        <input required name=em_bright_filename pattern="\S+,\d+$" class="form-control superevent-dependent typeahead" data-typeahead-url-template="{{ url_for('typeahead_em_bright_filename', superevent_id='SUPEREVENT_ID', filename='TERM') }}">
                     </div>
                     <div class="form-group col-md">
                         <label for=p_astro_filename>P_Astro File</label>
-                        <input required name=p_astro_filename class="form-control superevent-dependent typeahead" data-typeahead-url-template="{{ url_for('typeahead_p_astro_filename', superevent_id='SUPEREVENT_ID', filename='TERM') }}">
+                        <input required name=p_astro_filename pattern="\S+,\d+$" class="form-control superevent-dependent typeahead" data-typeahead-url-template="{{ url_for('typeahead_p_astro_filename', superevent_id='SUPEREVENT_ID', filename='TERM') }}">
                     </div>
                     <div class="form-group col-md">
                         <label for=submit-button class=w-100>&nbsp;</label>
                         <button type=submit id=submit-button name=submit-button class="btn btn-primary">Submit</button>
                     </div>
                 </div>
                 <div class="modal fade" tabindex=-1 role=dialog aria-labelledby=send-update-gcn-confirm-label>
```

#### html2text {}

```diff
@@ -24,14 +24,17 @@
 Preferred event ID[                    ]
   Submit
 **** RReeaallllyy IIssssuuee PPrreelliimmiinnaarryy GGCCNN NNoottiiccee?? ****
 ×
 Are you sure that you want to issue a Preliminary GCN Notice?
 Cancel Submit
 Issue Update GCN Notice
+Send an update GCN notice using the chosen fields.
+Note: the filenames must end with the comma version and not contain spaces,
+e.g. bayestar.multiorder.fits,0.
 Superevent ID[                    ]
 Sky Map File[                    ]
 Classification File[                    ]
 P_Astro File[                    ]
   Submit
 **** RReeaallllyy IIssssuuee UUppddaattee GGCCNN NNoottiiccee?? ****
 ×
```

### Comparing `gwcelery-2.3.6/gwcelery/templates/lalinference.jinja2` & `gwcelery-2.4.1/gwcelery/templates/lalinference.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/templates/rapidpe.jinja2` & `gwcelery-2.4.1/gwcelery/templates/rapidpe.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/conftest.py` & `gwcelery-2.4.1/gwcelery/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/G000012_S0040_preferred.json` & `gwcelery-2.4.1/gwcelery/tests/data/G000012_S0040_preferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/G298048-1-Initial.xml` & `gwcelery-2.4.1/gwcelery/tests/data/G298048-1-Initial.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/G298048_log.json` & `gwcelery-2.4.1/gwcelery/tests/data/G298048_log.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json` & `gwcelery-2.4.1/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/MS220722v.json` & `gwcelery-2.4.1/gwcelery/tests/data/MS220722v.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits` & `gwcelery-2.4.1/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/S230413b.json` & `gwcelery-2.4.1/gwcelery/tests/data/S230413b.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/S230413g.json` & `gwcelery-2.4.1/gwcelery/tests/data/S230413g.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/S230413h.json` & `gwcelery-2.4.1/gwcelery/tests/data/S230413h.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/T0212_S0039_preferred.json` & `gwcelery-2.4.1/gwcelery/tests/data/T0212_S0039_preferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json` & `gwcelery-2.4.1/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/T0219_S0041_nopreferred.json` & `gwcelery-2.4.1/gwcelery/tests/data/T0219_S0041_nopreferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/agile_grb_gcn.xml` & `gwcelery-2.4.1/gwcelery/tests/data/fermi_subgrbtargeted_template.xml`

 * *Files 20% similar despite different names*

#### Comparing `gwcelery-2.3.6/gwcelery/tests/data/agile_grb_gcn.xml` & `gwcelery-2.4.1/gwcelery/tests/data/fermi_subgrbtargeted_template.xml`

```diff
@@ -1,56 +1,46 @@
 <?xml version="1.0" encoding="utf-8"?>
-<voe:VOEvent xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" ivorn="ivo://nasa.gsfc.gcn/AGILE#A_Alert_2019-03-05T13:05:19.33_000000-053" role="observation" version="2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0  http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd">
+<voe:VOEvent xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0 http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd" version="2.0" role="test" ivorn="ivo://lvk.internal/fermi#targeted_subthreshold-2022-10-04T22:34:49.512Z">
   <Who>
-    <AuthorIVORN>ivo://nasa.gsfc.tan/gcn</AuthorIVORN>
+    <Description>VOEvent created with voevent-parse, version 1.0.3. See https://github.com/timstaley/voevent-parse for details.</Description>
+    <AuthorIVORN>ivo://fermi</AuthorIVORN>
+    <Date>2022-10-04T22:35:21Z</Date>
     <Author>
-      <shortName>AGILE (via VO-GCN)</shortName>
-      <contactName>Marco Feroci</contactName>
-      <contactPhone>+39-06-4993-4099</contactPhone>
-      <contactEmail>feroci@ias.rm.cnr.it</contactEmail>
+      <shortName>Fermi/LVK-joint</shortName>
+      <contactName>Joshua Woods</contactName>
+      <contactEmail>joshua.r.wood@nasa.gov</contactEmail>
     </Author>
-    <Date>2019-03-19T19:40:49</Date>
-    <Description>This VOEvent message was created with GCN VOE version: 1.33 05mar19</Description>
   </Who>
   <What>
-    <Param name="Packet_Type" value="105"/>
-    <Param name="Pkt_Ser_Num" value="1"/>
-    <Param name="TrigID" value="0" ucd="meta.id"/>
-    <Param name="Burst_TJD" value="18561" unit="days" ucd="time"/>
-    <Param name="Burst_SOD" value="70833.67" unit="sec" ucd="time"/>
+    <Param ucd="arith.rate;stat.falsealarm" unit="Hz" value="5e-06" name="FAR" dataType="float"/>
+    <Param name="TrigID" value="699554499710_20512" ucd="meta.id"/>
+    <Param name="Integ_Time" value="1.024" unit="sec" ucd="time.interval"/>
   </What>
   <WhereWhen>
     <ObsDataLocation>
       <ObservatoryLocation id="GEOLUN"/>
       <ObservationLocation>
         <AstroCoordSystem id="UTC-FK5-GEO"/>
         <AstroCoords coord_system_id="UTC-FK5-GEO">
           <Time unit="s">
             <TimeInstant>
-              <ISOTime>2019-03-05T19:40:33.67Z</ISOTime>
+              <ISOTime>2022-10-04T22:34:49.512Z</ISOTime>
             </TimeInstant>
           </Time>
           <Position2D unit="deg">
             <Name1>RA</Name1>
             <Name2>Dec</Name2>
             <Value2>
-              <C1>0.0000</C1>
-              <C2>4.3526</C2>
+              <C1>14.5</C1>
+              <C2>-40.1</C2>
             </Value2>
-            <Error2Radius>0.0000</Error2Radius>
+            <Error2Radius>0.3</Error2Radius>
           </Position2D>
         </AstroCoords>
       </ObservationLocation>
     </ObsDataLocation>
-    <Description>The RA,Dec coordinates are of the type: source_object.</Description>
   </WhereWhen>
   <How>
-    <Description>AGILE Satellite, SuperAGILE Instrument</Description>
-    <Reference uri="http://gcn.gsfc.nasa.gov/agile.html" type="url"/>
+    <Description>Fermi Satellite, GBM Instrument</Description>
+    <Reference uri="http://gcn.gsfc.nasa.gov/fermi.html" type="url"/>
   </How>
-  <Why>
-    <Inference probability="0.9">
-      <Concept>process.variation.burst;em.gamma</Concept>
-    </Inference>
-  </Why>
-  <Description/>
 </voe:VOEvent>
```

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/coinc.xml` & `gwcelery-2.4.1/gwcelery/tests/data/coinc.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/externaltrigger_original_data.xml` & `gwcelery-2.4.1/gwcelery/tests/data/externaltrigger_original_data.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/fermi_grb_gcn.xml` & `gwcelery-2.4.1/gwcelery/tests/data/fermi_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/fermi_initial_grb_gcn.xml` & `gwcelery-2.4.1/gwcelery/tests/data/fermi_initial_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/fermi_noise_gcn.xml` & `gwcelery-2.4.1/gwcelery/tests/data/fermi_noise_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/fermi_noise_gcn_2.xml` & `gwcelery-2.4.1/gwcelery/tests/data/fermi_noise_gcn_2.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/fermi_subgrbtargeted_template.xml` & `gwcelery-2.4.1/gwcelery/tests/data/swift_subgrbtargeted_template.xml`

 * *Files 14% similar despite different names*

#### Comparing `gwcelery-2.3.6/gwcelery/tests/data/fermi_subgrbtargeted_template.xml` & `gwcelery-2.4.1/gwcelery/tests/data/swift_subgrbtargeted_template.xml`

```diff
@@ -1,22 +1,23 @@
 <?xml version="1.0" encoding="utf-8"?>
-<voe:VOEvent xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0 http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd" version="2.0" role="test" ivorn="ivo://lvk.internal/fermi#targeted_subthreshold-2022-10-04T22:34:49.512Z">
+<voe:VOEvent xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0 http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd" version="2.0" role="test" ivorn="ivo://lvk.internal/swift#targeted_subthreshold-2022-10-04T22:34:49.512Z">
   <Who>
     <Description>VOEvent created with voevent-parse, version 1.0.3. See https://github.com/timstaley/voevent-parse for details.</Description>
-    <AuthorIVORN>ivo://fermi</AuthorIVORN>
+    <AuthorIVORN>ivo://swift</AuthorIVORN>
     <Date>2022-10-04T22:35:21Z</Date>
     <Author>
-      <shortName>Fermi/LVK-joint</shortName>
-      <contactName>Joshua Woods</contactName>
-      <contactEmail>joshua.r.wood@nasa.gov</contactEmail>
+      <shortName>Swift/LVK-joint</shortName>
+      <contactEmail>aaron.tohu@gmail.com</contactEmail>
+      <contactName>Aaron Tohuvavohu</contactName>
+      <shortName>Swift/LVK-joint</shortName>
     </Author>
   </Who>
   <What>
-    <Param ucd="arith.rate;stat.falsealarm" unit="Hz" value="5e-06" name="FAR" dataType="float"/>
-    <Param name="TrigID" value="699554499710_20512" ucd="meta.id"/>
+    <Param ucd="arith.rate;stat.falsealarm" unit="Hz" value="5.39583726e-08" name="FAR" dataType="float"/>
+    <Param name="TrigID" value="694215995" ucd="meta.id"/>
     <Param name="Integ_Time" value="1.024" unit="sec" ucd="time.interval"/>
   </What>
   <WhereWhen>
     <ObsDataLocation>
       <ObservatoryLocation id="GEOLUN"/>
       <ObservationLocation>
         <AstroCoordSystem id="UTC-FK5-GEO"/>
@@ -29,18 +30,18 @@
           <Position2D unit="deg">
             <Name1>RA</Name1>
             <Name2>Dec</Name2>
             <Value2>
               <C1>14.5</C1>
               <C2>-40.1</C2>
             </Value2>
-            <Error2Radius>0.3</Error2Radius>
+            <Error2Radius>0.03</Error2Radius>
           </Position2D>
         </AstroCoords>
       </ObservationLocation>
     </ObsDataLocation>
   </WhereWhen>
   <How>
-    <Description>Fermi Satellite, GBM Instrument</Description>
-    <Reference uri="http://gcn.gsfc.nasa.gov/fermi.html" type="url"/>
+    <Description>Swift Satellite, BAT Instrument</Description>
+    <Reference uri="http://gcn.gsfc.nasa.gov/swift.html" type="url"/>
   </How>
 </voe:VOEvent>
```

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml` & `gwcelery-2.4.1/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml` & `gwcelery-2.4.1/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/fits_header_result.html` & `gwcelery-2.4.1/gwcelery/tests/data/fits_header_result.html`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/gracedb_externaltrigger_log.json` & `gwcelery-2.4.1/gwcelery/tests/data/gracedb_externaltrigger_log.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_detchar.json` & `gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_detchar.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_exttrig_creation.json` & `gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_exttrig_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json` & `gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_psd.json` & `gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_psd.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_snews_creation.json` & `gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_snews_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_snews_test_creation.json` & `gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_snews_test_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_subgrb_creation.json` & `gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_subgrb_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_superevent_creation.json` & `gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_superevent_creation.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991319444444445%*

 * *Differences: {"'object'": "{'preferred_event_data': {'search': 'AllSky'}}"}*

```diff
@@ -18,15 +18,15 @@
             "logs": "https://gracedb-dev1.ligo.org/api/superevents/S180616h/logs/",
             "self": "https://gracedb-dev1.ligo.org/api/superevents/S180616h/",
             "voevents": "https://gracedb-dev1.ligo.org/api/superevents/S180616h/voevents/"
         },
         "preferred_event": "M4634",
         "preferred_event_data": {
             "group": "CBC",
-            "search": "Allsky"
+            "search": "AllSky"
         },
         "submitter": "emfollow",
         "superevent_id": "S180616h",
         "t_0": 1213205532.24,
         "t_end": 1213205542.24,
         "t_start": 1213205522.24
     },
```

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/igwn_alert_voevent.json` & `gwcelery-2.4.1/gwcelery/tests/data/igwn_alert_voevent.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/integral_grb_gcn.xml` & `gwcelery-2.4.1/gwcelery/tests/data/integral_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/integral_mdc_gcn.xml` & `gwcelery-2.4.1/gwcelery/tests/data/integral_mdc_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/integral_test_gcn.xml` & `gwcelery-2.4.1/gwcelery/tests/data/integral_test_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/kafka_alert_fermi.json` & `gwcelery-2.4.1/gwcelery/tests/data/kafka_alert_fermi.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/kafka_alert_fermi_ignore.json` & `gwcelery-2.4.1/gwcelery/tests/data/kafka_alert_fermi_ignore.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/kafka_alert_swift.json` & `gwcelery-2.4.1/gwcelery/tests/data/kafka_alert_swift.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/kafka_alert_swift_noloc.json` & `gwcelery-2.4.1/gwcelery/tests/data/kafka_alert_swift_noloc.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/kafka_alert_swift_wskymap.json` & `gwcelery-2.4.1/gwcelery/tests/data/kafka_alert_swift_wskymap.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.4.1/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/llhoft/idqbad/H1/H-H1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.4.1/gwcelery/tests/data/llhoft/idqbad/H1/H-H1_O2_llhoft-1216577976-4.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/llhoft/omegascan/scanme.gwf` & `gwcelery-2.4.1/gwcelery/tests/data/llhoft/omegascan/scanme.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.4.1/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/lvalert_event_creation.json` & `gwcelery-2.4.1/gwcelery/tests/data/lvalert_event_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/lvalert_xmpp.xml` & `gwcelery-2.4.1/gwcelery/tests/data/lvalert_xmpp.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/mock_superevent_object.json` & `gwcelery-2.4.1/gwcelery/tests/data/mock_superevent_object.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite` & `gwcelery-2.4.1/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/psd.xml.gz` & `gwcelery-2.4.1/gwcelery/tests/data/psd.xml.gz`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/rrt_small_area.fits` & `gwcelery-2.4.1/gwcelery/tests/data/rrt_small_area.fits`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/sample_events.json` & `gwcelery-2.4.1/gwcelery/tests/data/sample_events.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/samples.hdf5` & `gwcelery-2.4.1/gwcelery/tests/data/samples.hdf5`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/scaler_set_all.pickle` & `gwcelery-2.4.1/gwcelery/tests/data/scaler_set_all.pickle`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/snews_gcn.xml` & `gwcelery-2.4.1/gwcelery/tests/data/snews_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/snews_gcn_test.xml` & `gwcelery-2.4.1/gwcelery/tests/data/snews_gcn_test.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/superevents.json` & `gwcelery-2.4.1/gwcelery/tests/data/superevents.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/swift_grb_gcn.xml` & `gwcelery-2.4.1/gwcelery/tests/data/swift_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/data/test_classifier.pickle` & `gwcelery-2.4.1/gwcelery/tests/data/test_classifier.pickle`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/process.py` & `gwcelery-2.4.1/gwcelery/tests/process.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_sentry.py` & `gwcelery-2.4.1/gwcelery/tests/test_sentry.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_alerts.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_alerts.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_alerts_validate.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_alerts_validate.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_bayestar.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_bayestar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_circulars.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_circulars.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_condor.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_detchar.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_detchar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_em_bright.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_em_bright.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_external_skymaps.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_external_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_external_triggers.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_external_triggers.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 from ..util import read_binary, read_json
 from . import data
 
 
 @pytest.mark.parametrize('pipeline, path',
                          [['Fermi', 'fermi_grb_gcn.xml'],
                           ['INTEGRAL', 'integral_grb_gcn.xml'],
-                          ['INTEGRAL_MDC', 'integral_mdc_gcn.xml'],
-                          ['AGILE', 'agile_grb_gcn.xml']])
+                          ['INTEGRAL_MDC', 'integral_mdc_gcn.xml']])
 @patch('gwcelery.tasks.external_skymaps.create_upload_external_skymap.run')
 @patch('gwcelery.tasks.external_skymaps.get_upload_external_skymap.run')
 @patch('gwcelery.tasks.detchar.dqr_json', return_value='dqrjson')
 @patch('gwcelery.tasks.gracedb.upload.run')
 @patch('gwcelery.tasks.gracedb.create_event.run', return_value={
     'graceid': 'E1', 'gpstime': 1, 'instruments': '', 'pipeline': 'Fermi',
     'search': 'GRB',
@@ -62,20 +61,18 @@
                       'H1:HOFT_OK', 'H1:OBSERVATION_INTENT',
                       'L1:HOFT_OK', 'L1:OBSERVATION_INTENT',
                       'V1:HOFT_OK', 'V1:OBSERVATION_INTENT',
                       'V1:GOOD_DATA_QUALITY_CAT1'])),
             ['data_quality'])
     ]
     mock_upload.assert_has_calls(calls, any_order=True)
-    gcn_type_dict = {'Fermi': 115, 'INTEGRAL': 53, 'INTEGRAL_MDC': 53,
-                     'AGILE': 105}
+    gcn_type_dict = {'Fermi': 115, 'INTEGRAL': 53, 'INTEGRAL_MDC': 53}
     time_dict = {'Fermi': '2018-05-24T18:35:45',
                  'INTEGRAL': '2017-02-03T19:00:05',
-                 'INTEGRAL_MDC': '2023-04-04T06:31:24',
-                 'AGILE': '2019-03-19T19:40:49'}
+                 'INTEGRAL_MDC': '2023-04-04T06:31:24'}
     mock_create_upload_external_skymap.assert_called_once_with(
         {'graceid': 'E1',
          'gpstime': 1,
          'instruments': '',
          'pipeline': 'Fermi',
          'search': 'GRB',
          'extra_attributes': {
@@ -338,15 +335,16 @@
 @patch('gwcelery.tasks.raven.raven_pipeline.run')
 @patch('gwcelery.tasks.external_skymaps.create_combined_skymap.run')
 @patch('gwcelery.tasks.gracedb.get_superevent.run',
        return_value={
            'superevent_id': 'S1234',
            'preferred_event': 'G1234',
            'preferred_event_data':
-               {'group': 'CBC'}
+               {'group': 'CBC',
+                'search': 'AllSky'}
                     })
 def test_handle_skymaps_ready(mock_get_superevent,
                               mock_create_combined_skymap,
                               mock_raven_pipeline,
                               pipeline):
     """This test makes sure that once sky maps are available for a coincidence
     that the RAVEN pipeline is rerun to calculate the joint FAR with sky map
@@ -365,15 +363,16 @@
                  "search": "GRB"
                        }
              }
     external_triggers.handle_grb_igwn_alert(alert)
     mock_raven_pipeline.assert_called_once_with([{'superevent_id': 'S1234',
                                                   'preferred_event': 'G1234',
                                                   'preferred_event_data':
-                                                      {'group': 'CBC'}}],
+                                                      {'group': 'CBC',
+                                                       'search': 'AllSky'}}],
                                                 'E1212', alert['object'],
                                                 -5, 1, 'CBC',
                                                 use_superevent_skymap=False)
     mock_create_combined_skymap.assert_called_once_with(
         'S1234', 'E1212', preferred_event='G1234')
 
 
@@ -435,15 +434,16 @@
             }
 
 
 def _mock_get_superevent(graceid):
     return {'superevent_id': 'S1',
             'preferred_event': 'G1',
             'preferred_event_data':
-                {'group': 'CBC'},
+                {'group': 'CBC',
+                 'search': 'AllSky'},
             'em_events': ['E1', 'E2', 'E3'],
             'em_type': 'E1',
             'far': 1e-5,
             'labels': ['COMBINEDSKYMAP_READY', 'RAVEN_ALERT',
                        'EM_COINC', 'GCN_PRELIM_SENT']}
 
 
@@ -541,15 +541,16 @@
     alert = {
         "alert_type": alert_type,
         "uid": 'S1',
         "object": {"labels": ["EM_COINC"], "superevent_id": 'S1',
                    "em_events": ["E1", "E2"],
                    "preferred_event": 'G1',
                    "em_type": 'E1',
-                   "preferred_event_data": {"group": "CBC"}},
+                   "preferred_event_data": {"group": "CBC",
+                                            "search": "AllSky"}},
         "data": {"comment": comment, "filename": ""}
     }
 
     external_triggers.handle_grb_igwn_alert(alert)
 
     assert mock_create_combined_skymap.call_count == expected_skymap_calls
     assert mock_raven_pipeline.call_count == expected_skymap_calls
@@ -703,43 +704,47 @@
              searches=['SubGRB', 'SubGRBTargeted'],
              pipelines=['Swift'])])
 
 
 @pytest.mark.parametrize('path',
                          ['igwn_alert_snews_test_creation.json',
                           'igwn_alert_snews_creation.json',
-                          'igwn_alert_superevent_creation.json'])
+                          'igwn_alert_superevent_creation.json',
+                          'igwn_alert_superevent_burst_bbh_creation.json'])
 @patch('gwcelery.tasks.raven.coincidence_search')
 def test_handle_sntrig_creation(mock_raven_coincidence_search, path):
-    """Test dispatch of an IGWN alert message for SNEWS alerts
+    """Test dispatch of an IGWN alert message for SNEWS alerts.
     This now includes both real and test SNEWS events to ensure both are
     ingested correctly, as well as a superevent.
     """
     # Test IGWN alert payload.
     alert = read_json(data, path)
 
     if 'superevent' in path:
         alert['object']['preferred_event_data']['group'] = 'Burst'
+        search = alert['object']['preferred_event_data']['search']
 
     # Run function under test
     external_triggers.handle_snews_igwn_alert(alert)
 
     if 'test' in path:
         graceid = 'E1236'
     else:
         graceid = 'E1235'
 
-    if 'superevent' in path:
+    if 'superevent' in path and search == 'BBH':
+        mock_raven_coincidence_search.assert_not_called()
+    elif 'superevent' in path:
         mock_raven_coincidence_search.assert_called_once_with(
             'S180616h', alert['object'], group='Burst', searches=['Supernova'],
-            pipelines=['SNEWS'])
+            se_searches=['AllSky'], pipelines=['SNEWS'])
     elif 'snews' in path:
         mock_raven_coincidence_search.assert_called_once_with(
             graceid, alert['object'], group='Burst', searches=['Supernova'],
-            pipelines=['SNEWS'])
+            se_searches=['AllSky'], pipelines=['SNEWS'])
 
 
 @patch('gwcelery.tasks.gracedb.get_superevent',
        return_value={'preferred_event': 'M4634'})
 @patch('gwcelery.tasks.gracedb.get_group', return_value='CBC')
 @patch('gwcelery.tasks.raven.coincidence_search')
 def test_handle_superevent_cbc_creation(mock_raven_coincidence_search,
@@ -776,23 +781,31 @@
     alert = read_json(data, 'igwn_alert_superevent_creation.json')
     alert['object']['preferred_event_data']['group'] = 'Burst'
     alert['object']['preferred_event_data']['search'] = search
 
     # Run function under test
     external_triggers.handle_grb_igwn_alert(alert)
 
+    # Check that the correct tasks were dispatched.
     if search == 'AllSky':
-        # Check that the correct tasks were dispatched.
         mock_raven_coincidence_search.assert_has_calls([
             call('S180616h', alert['object'], group='Burst',
                  searches=['GRB'], se_searches=['AllSky']),
             call('S180616h', alert['object'], group='Burst',
                  pipelines=['Fermi'], searches=['SubGRBTargeted']),
             call('S180616h', alert['object'], group='Burst',
                  pipelines=['Swift'], searches=['SubGRBTargeted'])])
+    elif search == 'BBH':
+        mock_raven_coincidence_search.assert_has_calls([
+            call('S180616h', alert['object'], group='Burst',
+                 searches=['GRB'], se_searches=['BBH']),
+            call('S180616h', alert['object'], group='Burst',
+                 pipelines=['Fermi'], searches=['SubGRB', 'SubGRBTargeted']),
+            call('S180616h', alert['object'], group='Burst',
+                 pipelines=['Swift'], searches=['SubGRB', 'SubGRBTargeted'])])
     else:
         mock_raven_coincidence_search.assert_not_called()
 
 
 def _mock_get_events(query):
     if "12345" in query:
         return [{"graceid": "E12345", "search": "SubGRBTargeted",
@@ -945,22 +958,24 @@
     """Test dispatch of an MDC with the supernovae igwn alert listener,
     both a superevent and external event."""
     # Test IGWN alert payload.
     alert = read_json(data, path)
     if 'superevent' in path:
         alert['object']['preferred_event_data']['search'] = 'MDC'
         alert['object']['preferred_event_data']['group'] = 'Burst'
+        graceid = 'S180616h'
     elif 'snews' in path:
         alert['object']['search'] = 'MDC'
+        graceid = 'E1235'
 
     # Run function under test
     external_triggers.handle_snews_igwn_alert(alert)
 
     # Check that the correct tasks were dispatched.
     if 'superevent' in path:
         mock_raven_coincidence_search.assert_called_once_with(
-            'S180616h', alert['object'], group='Burst', searches=['MDC'],
-            pipelines=['SNEWS'])
+            graceid, alert['object'], group='Burst', searches=['MDC'],
+            se_searches=['MDC'], pipelines=['SNEWS'])
     elif 'snews' in path:
         mock_raven_coincidence_search.assert_called_once_with(
-            'E1235', alert['object'], group='Burst', se_searches=['MDC'],
-            pipelines=['SNEWS'])
+            graceid, alert['object'], group='Burst', searches=['MDC'],
+            se_searches=['MDC'], pipelines=['SNEWS'])
```

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_first2years.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_first2years.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_first2years_external.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_first2years_external.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 @pytest.mark.parametrize('ext_search', ['GRB', 'SubGRB', 'SubGRBTargeted'])
 @pytest.mark.parametrize(
     'host,se_search,group,superevent_id,expected_result',
     [['gracedb-playground.ligo.org', 'MDC', 'CBC', 'MS180616j', True],
      ['gracedb-playground.ligo.org', 'AllSky', 'CBC', 'MS180616j', True],
      ['gracedb-playground.ligo.org', 'AllSky', 'Burst', 'MS180616j', True],
-     ['gracedb-playground.ligo.org', 'BBH', 'CBC', 'MS180616j', False],
+     ['gracedb-playground.ligo.org', 'BBH', 'CBC', 'MS180616j', True],
+     ['gracedb-playground.ligo.org', 'IMBH', 'CBC', 'MS180616j', False],
      ['gracedb-playground.ligo.org', 'AllSky', 'Test', 'TS180616j', False],
      ['gracedb.ligo.org', 'MDC', 'CBC', 'MS180616j', True],
      ['gracedb.ligo.org', 'AllSky', 'CBC', 'MS180616j', False],
      ['gracedb.ligo.org', 'AllSky', 'Burst', 'MS180616j', False],
      ['gracedb.ligo.org', 'MDC', 'CBC', 'MS180616k', False]])
 def test_handle_create_grb_event(monkeypatch,
                                  ext_search,
```

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_gcn.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_gcn.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_gcn_validate.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_gcn_validate.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_gracedb.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_igwn_alert.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_igwn_alert.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_inference.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,19 +131,20 @@
 
 
 @pytest.mark.parametrize(
     "host,mode,mc",
     product(
         ['gracedb-playground.ligo.org', 'gracedb.ligo.org'],
         ['production', 'fast_test'],
-        [30, 10, 3, 2, 1, 0.1]
+        [30, 20, 15, 10, 3, 2, 1, 0.1]
     )
 )
 def test_setup_dag_for_bilby(monkeypatch, tmp_path, host, mode, mc):
     psd = b'psd'
+    bayestar = b'bayestar'
     rundir = str(tmp_path)
     event = {'gpstime': 1187008882, 'graceid': 'G1234',
              'extra_attributes': {'CoincInspiral': {'mchirp': mc}}}
     sid = 'S1234'
     ini = 'bilby configuration ini file'
     dag = 'bilby dag'
     monkeypatch.setitem(app.conf, 'gracedb_host', host)
@@ -163,24 +164,30 @@
             assert event == json.load(f)
 
         path_to_psd = cmd[8]
         assert os.path.exists(path_to_psd)
         with open(path_to_psd, 'rb') as f:
             assert f.read() == psd
 
+        path_to_bayestar = cmd[10]
+        assert os.path.exists(path_to_bayestar)
+        with open(path_to_bayestar, 'rb') as f:
+            assert f.read() == bayestar
+
         if mode == "fast_test":
             assert "FastTest" in cmd
 
-        path_to_settings = cmd[10]
+        path_to_settings = cmd[12]
         assert os.path.exists(path_to_settings)
         ans = {
             'summarypages_arguments': {'gracedb': event['graceid'],
                                        'no_ligo_skymap': True},
             'queue': 'Online_PE',
             'accounting_user': 'soichiro.morisaki',
+            'tukey_roll_off': 1.0
         }
         if host != 'gracedb.ligo.org':
             ans['queue'] = 'Online_PE_MDC'
         else:
             ans['accounting'] = 'ligo.prod.o4.cbc.pe.bilby'
         if mode == 'production':
             ans.update(
@@ -196,16 +203,24 @@
                 ans['sampler_kwargs']['naccept'] = 10
             elif mc < 2.243:
                 assert 'phenompv2_bns_roq' in cmd
             elif mc < 12:
                 assert 'low_q_phenompv2_roq' in cmd
             else:
                 assert 'phenomxphm_roq' in cmd
-                ans['request_memory_generation'] = 36.0
-                ans['request_memory'] = 16.0
+                if mc > 16:
+                    ans['request_memory_generation'] = 36.0
+                else:
+                    ans['request_memory_generation'] = 50.0
+                if mc > 25:
+                    ans['request_memory'] = 16.0
+                elif mc > 16:
+                    ans['request_memory'] = 24.0
+                else:
+                    ans['request_memory'] = 36.0
         elif mode == 'fast_test' and mc < 3.9:
             ans['request_memory_generation'] = 8.0
         with open(path_to_settings, 'r') as f:
             assert json.load(f) == ans
 
         with open(os.path.join(rundir, 'bilby_config.ini'), 'w') as f:
             f.write(ini)
@@ -222,15 +237,15 @@
     monkeypatch.setattr('gwcelery.tasks.gracedb.upload.run', upload)
 
     if mc < 0.6:
         with pytest.raises(ValueError):
             inference._setup_dag_for_bilby(psd, rundir, event, sid, mode)
     else:
         path_to_dag = inference._setup_dag_for_bilby(
-            psd, rundir, event, sid, mode
+            (psd, bayestar), rundir, event, sid, mode
         )
 
         assert os.path.exists(path_to_dag)
         with open(path_to_dag, 'r') as f:
             assert f.read() == dag
         upload.assert_called_once()
 
@@ -322,15 +337,15 @@
     }
     with pytest.raises(subprocess.CalledProcessError):
         if pipeline == 'lalinference':
             inference._setup_dag_for_lalinference(
                 b'coinc', rundir, event, 'S1234')
         elif pipeline == 'bilby':
             inference._setup_dag_for_bilby(
-                (b'psd'), rundir, event, 'S1234', 'production')
+                (b'psd', b'bayestar'), rundir, event, 'S1234', 'production')
         elif pipeline == 'rapidpe':
             inference._setup_dag_for_rapidpe(rundir, 'S1234', event)
     if pipeline == 'bilby':
         assert upload.call_count == 1
     else:
         # For pipelines except for bilby, an ini file is uploaded before dag
         # generation, and hence the call count is 2.
@@ -338,36 +353,40 @@
 
 
 @pytest.mark.parametrize(
     'pipeline', ['lalinference', 'bilby', 'rapidpe', 'my_awesome_pipeline'])
 def test_dag_prepare_task(monkeypatch, pipeline):
     sid = 'S1234'
     coinc = b'coinc'
+    bayestar = b'bayestar'
     event = {
             'gpstime': 1187008882,
             'graceid': 'G1234',
             'extra_attributes': {
                 'CoincInspiral': {'snr': 10}
             }
     }
     rundir = 'rundir'
     path_to_dag = os.path.join(rundir, 'parameter_estimation.dag')
     kwargs = {'bilby_mode': 'production'}
 
     def mock_download(filename, gid):
         if filename == 'coinc.xml':
             return coinc
+        elif filename == 'bayestar.multiorder.fits':
+            return bayestar
 
     def _setup_dag_for_lalinference(c, r, e, s):
         assert (c == coinc and r == rundir and e == event and s == sid)
         return path_to_dag
 
-    def _setup_dag_for_bilby(c, r, e, s, m):
-        assert c == coinc and r == rundir and e == event and s == sid and \
-            m == kwargs['bilby_mode']
+    def _setup_dag_for_bilby(c_b, r, e, s, m):
+        c, b = c_b
+        assert c == coinc and b == bayestar and r == rundir and e == event \
+            and s == sid and m == kwargs['bilby_mode']
         return path_to_dag
 
     def _setup_dag_for_rapidpe(r, s, e):
         assert r == rundir and s == sid and e == event
         return path_to_dag
 
     def _subprocess_run(cmd, **kwargs):
```

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_orchestrator.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_orchestrator.py`

 * *Files 5% similar despite different names*

```diff
@@ -302,14 +302,15 @@
         if superevents.SIGNIFICANT_LABEL in superevent_labels:
             expose.assert_not_called()
             alerts_send.assert_not_called()
             gcn_send.assert_not_called()
             create_tag.assert_not_called()
             create_initial_circular.assert_not_called()
             check_high_profile.assert_not_called()
+            create_label.assert_not_called()
         else:
             annotate_fits.assert_called_once()
             update_superevent_task.assert_called_once_with(
                 'S1234', preferred_event='G1234', t_0=1234.
             )
             expose.assert_called_once_with('S1234')
             create_tag.assert_has_calls(
@@ -317,15 +318,15 @@
                  call('em-bright-filename', 'public', 'S1234'),
                  call('p-astro-filename', 'public', 'S1234'),
                  call('skymap-filename', 'public', 'S1234')],
                 any_order=True
             )
             assert call('GCN_PRELIM_SENT', superevent_id) \
                 not in create_label.call_args_list
-
+            create_label.assert_has_calls([call('DQR_REQUEST', 'S1234')])
     elif alert_label == superevents.FROZEN_LABEL:
         if (superevents.SIGNIFICANT_LABEL in superevent_labels) or \
                 (superevents.EARLY_WARNING_LABEL in superevent_labels):
             expose.assert_not_called()
             alerts_send.assert_not_called()
             gcn_send.assert_not_called()
             create_tag.assert_not_called()
@@ -1138,73 +1139,48 @@
             superevent_id,
             'preliminary'
         ).get()
         mock_alert.assert_not_called()
 
 
 @pytest.mark.parametrize(
-    'far,event,pe_pipeline',
-    [[1, {'gpstime': 1187008882, 'group': 'CBC', 'search': 'AllSky'}, 'bilby'],
-     [1e-30, {'gpstime': 1187008882, 'group': 'Burst', 'search': 'AllSky'},
-         'bilby'],
-     [1e-30, {'gpstime': 1187008882, 'group': 'CBC', 'search': 'MDC'},
-         'bilby'],
-     [1e-30, {'gpstime': 1187008882, 'group': 'CBC', 'search': 'AllSky',
-              'pipeline': 'gstlal', 'offline': True}, 'bilby'],
-     [1e-30, {'gpstime': 1187008882, 'group': 'CBC',
-              'search': 'AllSky', 'pipeline': 'gstlal'}, 'bilby'],
-     [1e-30, {'gpstime': 1187008882, 'group': 'CBC',
-              'search': 'AllSky', 'pipeline': 'pycbc'}, 'bilby'],
-     [1, {'gpstime': 1187008882, 'group': 'CBC', 'search': 'AllSky',
-          'extra_attributes': {'CoincInspiral': {'snr': 10}}},
-        'rapidpe'],
-     [1e-30, {'gpstime': 1187008882, 'group': 'Burst', 'search': 'AllSky',
-              'extra_attributes': {'CoincInspiral': {'snr': 10}}},
-        'rapidpe'],
-     [1e-30, {'gpstime': 1187008882, 'group': 'CBC', 'search': 'MDC',
-              'extra_attributes': {'CoincInspiral': {'snr': 10}}},
-        'rapidpe'],
-     [1e-30, {'gpstime': 1187008882, 'group': 'CBC', 'search': 'AllSky',
-              'pipeline': 'gstlal', 'offline': True,
-              'extra_attributes': {'CoincInspiral': {'snr': 10}}
-              }, 'rapidpe'],
-     [1e-30, {'gpstime': 1187008882, 'group': 'CBC',
-              'search': 'AllSky', 'pipeline': 'gstlal',
-              'extra_attributes': {'CoincInspiral': {'snr': 10}}
-              }, 'rapidpe'],
-     [1e-30, {'gpstime': 1187008882, 'group': 'CBC',
-              'search': 'AllSky', 'pipeline': 'pycbc',
-              'extra_attributes': {'CoincInspiral': {'snr': 10}}
-              }, 'rapidpe']]
+    'far_event,pe_pipeline,pe_required',
+    [
+        [(1e-30, {'search': 'AllSky'}), 'bilby', True],  # significant CBC
+        [(1e-30, {'search': 'AllSky'}), 'rapidpe', True],  # another pipeline
+        [(1, {'search': 'AllSky'}), 'bilby', False],  # low significance
+        [None, 'bilby', False],  # No CBC triggers
+        [(1e-30, {'search': 'wormhole'}), 'bilby', False],  # unknown search
+        [(1e-30, {'search': 'MDC'}), 'bilby', False],  # MDC upload
+        [(1e-30, {'search': 'offline'}), 'bilby', False],  # Offline upload
+        [(1e-30, {'search': 'earlywarning'}), 'rapidpe', False],
+        # rapidpe + earlywarning
+    ]
 )
-def test_parameter_estimation(monkeypatch, far, event, pe_pipeline):
+def test_parameter_estimation(
+    monkeypatch, far_event, pe_pipeline, pe_required
+):
     superevent_id = 'S1234'
     mock_upload = Mock()
     mock_start_pe = Mock()
     monkeypatch.setattr('gwcelery.tasks.gracedb.upload.run', mock_upload)
     monkeypatch.setattr('gwcelery.tasks.inference.start_pe.run', mock_start_pe)
 
     orchestrator.parameter_estimation.delay(
-        far_event=(far, event), superevent_id=superevent_id,
+        far_event=far_event, superevent_id=superevent_id,
         pe_pipeline=pe_pipeline)
 
-    group = event['group'].lower()
-    search = event['search'].lower()
-    threshold = (app.conf['significant_alert_far_threshold'][group][search] /
-                 app.conf['significant_alert_trials_factor'][group][search])
-    if (
-        far <= threshold and event['group'] == 'CBC' and
-        event['search'] != 'MDC' and
-        not event.get('offline', False)
-    ):
+    if pe_required:
+        _, event = far_event
         mock_start_pe.assert_any_call(
             event, superevent_id, pe_pipeline)
         assert mock_start_pe.call_count == 1
     else:
         mock_upload.assert_called_once()
+        assert mock_start_pe.call_count == 0
 
 
 @pytest.mark.parametrize(
     'search_pipeline,pe_pipeline',
     [["MBTA", "bilby"], ["MBTA", "rapidpe"],
      ["spiir", "bilby"], ["spiir", "rapidpe"]],
 )
@@ -1232,14 +1208,98 @@
             event, superevent_id, pe_pipeline)
         assert mock_start_pe.call_count == 1
     else:
         mock_upload.assert_called_once()
 
 
 @pytest.mark.parametrize(
+    'gevents_dict,preferred_event_id,answer_far,answer_event_id',
+    [
+        [
+            {
+                "G1": {"group": "cbc", "search": "allsky", "far": 1e-10}
+            },
+            "G1",
+            1e-10,
+            "G1"
+        ],  # one CBC trigger
+        [
+            {
+                "G1": {"group": "cbc", "search": "allsky", "far": 1},
+                "G2": {"group": "cbc", "search": "allsky", "far": 1e-10},
+                "G3": {"group": "cbc", "search": "allsky", "far": 1e-5}
+            },
+            "G2",
+            1e-10,
+            "G2"
+        ],  # multiple CBC triggers
+        [
+            {
+                "G1": {"group": "cbc", "search": "allsky", "far": 1e-10},
+                "G2": {"group": "burst", "search": "bbh", "far": 1e-12}
+            },
+            "G1",
+            1e-12,
+            "G1"
+        ],  # significant CBC + significant Burst-BBH
+        [
+            {
+                "G1": {"group": "cbc", "search": "allsky", "far": 1e-10},
+                "G2": {"group": "burst", "search": "allsky", "far": 1e-12}
+            },
+            "G1",
+            1e-10,
+            "G1"
+        ],  # significant CBC + significant unmodeled Burst
+        [
+            {
+                "G1": {"group": "burst", "search": "bbh", "far": 1e-12},
+                "G2": {"group": "cbc", "search": "allsky", "far": 1},
+                "G3": {"group": "cbc", "search": "allsky", "far": 1e-5},
+                "G4": {"group": "cbc", "search": "allsky", "far": 1e-3},
+            },
+            "G1",
+            1e-12,
+            "G3"
+        ],  # low-significance CBC + significant Burst-BBH
+        [
+            {
+                "G1": {"group": "burst", "search": "allsky", "far": 1e-10},
+            },
+            "G1",
+            None,
+            None
+        ],  # only a cWB trigger
+    ]
+)
+def test_get_pe_far_and_event(
+    monkeypatch, gevents_dict, preferred_event_id, answer_far, answer_event_id
+):
+    superevent = {}
+    superevent["gw_events"] = list(gevents_dict.keys())
+    superevent["preferred_event_data"] = gevents_dict[preferred_event_id]
+
+    def _get_event(graceid):
+        return gevents_dict[graceid]
+
+    monkeypatch.setattr(
+        'gwcelery.tasks.gracedb.get_event._orig_run',
+        _get_event
+    )
+
+    ans = orchestrator._get_pe_far_and_event(superevent)
+    if answer_event_id is None:
+        assert ans is None
+    else:
+        far, event = ans
+        assert far == answer_far
+        assert event == gevents_dict[answer_event_id]
+
+
+@pytest.mark.parametrize(
     "superevent_labels,block_by_labels",
     [
         [[superevents.FROZEN_LABEL], set()],
         [[superevents.FROZEN_LABEL], {"ADVOK", "ADVNO"}],
         [[superevents.SIGNIFICANT_LABEL, "ADVOK"], {"ADVOK", "ADVNO"}]
     ]
 )
```

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_p_astro.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_p_astro.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_raven.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_raven.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,35 +5,36 @@
 from .. import app
 from ..tasks import gracedb, raven
 from .test_tasks_skymaps import toy_fits_filecontents  # noqa: F401
 
 
 @pytest.mark.live_worker
 @pytest.mark.parametrize(
-    'group,gracedb_id,pipelines,ext_search,se_search,tl,th',
+    'group,gracedb_id,pipelines,se_search,ext_search,tl,th',
     [['CBC', 'S1', ['Fermi', 'Swift'], [], ['GRB'], -1, 5],
      ['Burst', 'S2', ['Fermi', 'Swift'], [], ['GRB'], -60, 600],
      ['Burst', 'S3', ['SNEWS'], ['Supernova'], [], -10, 10],
      ['Burst', 'T4', ['SNEWS'], 'Supernova', [], -10, 10],
      ['CBC', 'MS4', ['Fermi'], ['MDC'], [], -1, 5],
      ['CBC', 'E1', ['Fermi'], [], ['GRB'], -5, 1],
      ['CBC', 'M1', ['Fermi'], [], ['MDC'], -5, 1],
-     ['CBC', 'E1', ['Fermi'], ['SubGRB'], [], -11, 1],
-     ['Burst', 'E1', ['Swift'], ['SubGRBTargeted'], [], -20, 10],
-     [None, 'E1', ['Swift'], ['SubGRBTargeted'], [], -20, 10]])
+     ['CBC', 'E1', ['Fermi'], [], ['SubGRB'], -11, 1],
+     ['Burst', 'E1', ['Swift'], [], ['SubGRBTargeted'], -20, 10],
+     ['Burst', 'E1', ['Swift'], ['BBH'], [], -5, 1],
+     [None, 'E1', ['Swift'], [], ['SubGRBTargeted'], -20, 10]])
 @patch('gwcelery.tasks.gracedb.create_label')
 @patch('gwcelery.tasks.raven.raven_pipeline.s')
 @patch('gwcelery.tasks.raven.search.si', return_value=[{'superevent_id': 'S5',
                                                         'graceid': 'E2'}])
 @patch('gwcelery.tasks.raven.calculate_coincidence_far')
 def test_coincidence_search(mock_calculate_coincidence_far,
                             mock_search, mock_raven_pipeline,
                             mock_create_label,
                             group, gracedb_id, pipelines,
-                            ext_search, se_search, tl, th):
+                            se_search, ext_search, tl, th):
     """Test that correct time windows are used for each RAVEN search."""
     alert_object = {'superevent_id': gracedb_id}
     if 'E' in gracedb_id:
         alert_object['group'] = 'External'
     raven.coincidence_search(gracedb_id, alert_object, group,
                              pipelines, ext_search, se_search)
 
@@ -44,15 +45,15 @@
         gracedb_id, alert_object, tl, th, group)
 
 
 @pytest.mark.parametrize(
     'group,search', [['CBC', 'SubGRBTargeted'], ['Test', 'GRB']])
 def test_raven_window_errors(group, search):
     with pytest.raises(ValueError):
-        raven._time_window('S1', group, ['INTEGRAL'], [search])
+        raven._time_window('S1', group, ['INTEGRAL'], [search], [])
 
 
 @pytest.mark.parametrize(
     'event_type,event_id', [['SE', 'S1234'], ['ExtTrig', 'E1234']])
 @patch('ligo.raven.search.search')
 def test_raven_search(mock_raven_search, event_type, event_id):
     """Test that correct input parameters are used for raven."""
@@ -86,14 +87,15 @@
     mock_calc_signif.assert_called_once_with(
         'S1234', 'E4321', tl, th,
         se_dict=se, ext_dict=ext,
         incl_sky=False, grb_search=ext['search'],
         em_rate=app.conf['raven_ext_rates'][ext['search']],
         gracedb=gracedb.client, far_grb=None,
         far_gw_thresh=None, far_grb_thresh=None)
+    assert isinstance(app.conf['raven_ext_rates'][ext['search']], float)
 
 
 @patch('ligo.raven.search.calc_signif_gracedb')
 def test_calculate_coincidence_far_subgrb(mock_calc_signif):
     se = {'superevent_id': 'S1234'}
     ext = {'graceid': 'E4321',
            'pipeline': 'Fermi',
@@ -108,14 +110,18 @@
         incl_sky=False, grb_search=ext['search'],
         gracedb=gracedb.client, far_grb=ext['far'],
         em_rate=None,
         far_gw_thresh=(
             app.conf['raven_targeted_far_thresholds']['GW']['Fermi']),
         far_grb_thresh=(
             app.conf['raven_targeted_far_thresholds']['GRB']['Fermi']))
+    assert isinstance(
+        app.conf['raven_targeted_far_thresholds']['GW']['Fermi'], float)
+    assert isinstance(
+        app.conf['raven_targeted_far_thresholds']['GRB']['Fermi'], float)
 
 
 @pytest.mark.parametrize('group', ['CBC', 'Burst'])  # noqa: F811
 @patch('gwcelery.tasks.external_skymaps.get_skymap_filename',
        return_value='fermi_skymap.fits.gz')
 @patch('ligo.raven.search.calc_signif_gracedb')
 def test_calculate_spacetime_coincidence_far_fermi(
@@ -138,14 +144,15 @@
         se_fitsfile='fermi_skymap.fits.gz',
         ext_fitsfile='fermi_skymap.fits.gz',
         se_moc=True, ext_moc=False,
         em_rate=app.conf['raven_ext_rates'][ext['search']],
         gracedb=gracedb.client, far_grb=None,
         far_gw_thresh=None, far_grb_thresh=None,
         use_preferred_event_skymap=False)
+    assert isinstance(app.conf['raven_ext_rates'][ext['search']], float)
 
 
 @pytest.mark.parametrize('group', ['CBC', 'Burst'])  # noqa: F811
 @patch('gwcelery.tasks.external_skymaps.get_skymap_filename',
        return_value='swift_skymap.multiorder.fits')
 @patch('ligo.raven.search.calc_signif_gracedb')
 def test_calculate_spacetime_coincidence_far_swift(
@@ -168,14 +175,15 @@
         se_fitsfile='swift_skymap.multiorder.fits',
         ext_fitsfile='swift_skymap.multiorder.fits',
         em_rate=app.conf['raven_ext_rates'][ext['search']],
         se_moc=True, ext_moc=True,
         gracedb=gracedb.client, far_grb=None,
         far_gw_thresh=None, far_grb_thresh=None,
         use_preferred_event_skymap=False)
+    assert isinstance(app.conf['raven_ext_rates'][ext['search']], float)
 
 
 @pytest.mark.parametrize('group', ['CBC', 'Burst'])  # noqa: F811
 @patch('gwcelery.tasks.external_skymaps.get_skymap_filename',
        return_value='fermi_skymap.fits.gz')
 @patch('ligo.raven.search.calc_signif_gracedb')
 def test_calculate_spacetime_coincidence_far_preferred(
@@ -199,14 +207,15 @@
         se_fitsfile='fermi_skymap.fits.gz',
         ext_fitsfile='fermi_skymap.fits.gz',
         em_rate=app.conf['raven_ext_rates'][ext['search']],
         se_moc=True, ext_moc=False,
         gracedb=gracedb.client, far_grb=None,
         far_gw_thresh=None, far_grb_thresh=None,
         use_preferred_event_skymap=True)
+    assert isinstance(app.conf['raven_ext_rates'][ext['search']], float)
 
 
 @patch('ligo.raven.search.calc_signif_gracedb')
 def test_calculate_coincidence_far_snews(
         mock_calc_signif):
     se = {'superevent_id': 'S1234'}
     ext = {'graceid': 'E4321',
@@ -257,24 +266,25 @@
             'superevent_id': superevent_id,
             'labels': [],
             'em_type': None}
 
 
 @pytest.mark.parametrize(
     'raven_search_results,graceid,tl,th,group',
-    [[[{'graceid': 'E1', 'pipeline': 'GRB'}], 'S1', -5, 1, 'CBC'],
+    [[[{'graceid': 'E1', 'search': 'GRB'}], 'S1', -5, 1, 'CBC'],
      [[{'superevent_id': 'S10', 'far': 1, 'preferred_event': 'G1'}],
         'E2', -1, 5, 'CBC'],
-     [[{'graceid': 'E3', 'pipeline': 'GRB'},
-       {'graceid': 'E4', 'pipeline': 'GRB'}], 'S2', -600, 60, 'Burst'],
+     [[{'graceid': 'E3', 'search': 'GRB'},
+       {'graceid': 'E4', 'search': 'GRB'}], 'S2', -600, 60, 'Burst'],
      [[{'superevent_id': 'S11', 'far': 1, 'preferred_event': 'G2'},
        {'superevent_id': 'S12', 'far': .001, 'preferred_event': 'G3'}],
         'E5', -1, 5, 'CBC'],
      [[], 'S13', -1, 5, 'CBC'],
-     [[{'graceid': 'E4', 'pipeline': 'GRB'}], 'S14', -1, 5, 'CBC'],
+     [[{'graceid': 'E4', 'search': 'GRB'}], 'S14', -1, 5, 'CBC'],
+     [[{'graceid': 'E5', 'search': 'SubGRBTargeted'}], 'S14', -1, 5, 'CBC'],
      [[{'superevent_id': 'S12', 'far': .001, 'preferred_event': 'G3'}],
         'T4', -10, 10, 'Burst'],
      [[{'superevent_id': 'MS13', 'far': 1, 'preferred_event': 'M3'}],
         'M15', -1, 5, 'CBC'],
      [[{'superevent_id': 'S13', 'far': 1, 'preferred_event': 'G4'}],
         'E6', -60, 600, 'Burst']])
 @patch('gwcelery.tasks.raven.trigger_raven_alert.run')
@@ -294,15 +304,19 @@
     """
     alert_object = {'preferred_event': 'G1', 'pipeline': 'Fermi',
                     'search': 'Supernova' if graceid == 'T4' else 'GRB',
                     'labels': [],
                     'superevent': None if graceid != 'E6' else 'S14'}
 
     for result in raven_search_results:
-        result['labels'] = []
+        # Check if is an external event and is SubGRBTargeted
+        if result.get('graceid') and result['search'] == 'SubGRBTargeted':
+            result['labels'] = 'NOT_GRB'
+        else:
+            result['labels'] = []
     if 'S' not in graceid:
         alert_object['group'] = 'External'
         if 'T' in graceid:
             alert_object['group'] = 'Test'
         alert_object['graceid'] = graceid
         for result in raven_search_results:
             result['time_coinc_far'] = 1e-5
@@ -347,15 +361,18 @@
             mock_coinc_far(),
             result, graceid, alert_object, group))
     if graceid != 'E6':
         mock_trigger_raven_alert.assert_has_calls(alert_calls, any_order=True)
 
         mock_calculate_coincidence_far.assert_has_calls(coinc_calls,
                                                         any_order=True)
-        mock_create_label.assert_has_calls(label_calls, any_order=True)
+        if result.get('graceid') and result['search'] == 'SubGRBTargeted':
+            mock_create_label.assert_not_called()
+        else:
+            mock_create_label.assert_has_calls(label_calls, any_order=True)
     else:
         mock_trigger_raven_alert.assert_not_called()
         mock_calculate_coincidence_far.assert_not_called()
         mock_create_label.assert_not_called()
 
 
 @pytest.mark.parametrize(
@@ -380,19 +397,19 @@
                                          'preferred_event': 'G5'}]
 
 
 @pytest.mark.parametrize(
     'new_time_far,new_space_far,superevent_id,pipeline,result',
     [[1e-4, None, 'S1', 'Fermi', True],
      [1e-4, 1e-3, 'S1', 'Swift', True],
-     [1e-4, None, 'S2', 'AGILE', False],
+     [1e-4, None, 'S2', 'INTEGRAL', False],
      [1e-4, 1e-3, 'S3', 'Fermi', True],
      [1e-4, 1e-3, 'S4', 'Fermi', False],
      [1e-8, None, 'S4', 'Swift', False],
-     [1e-4, 1e-8, 'S5', 'AGILE', True],
+     [1e-4, 1e-8, 'S5', 'INTEGRAL', True],
      [None, None, 'S1', 'SNEWS', True]])
 @patch('gwcelery.tasks.gracedb.update_superevent')
 @patch('gwcelery.tasks.gracedb.get_superevent', mock_get_superevent)
 def test_update_superevent(mock_update_superevent,
                            new_time_far, new_space_far,
                            superevent_id,
                            pipeline, result):
@@ -512,28 +529,33 @@
                 "preferred_event_data": {"group": "Burst", "search": "AllSky"},
                 "far": 1e-3}
     elif graceid == "S9876":
         return {"superevent_id": "S9876",
                 "preferred_event": "G000003",
                 "preferred_event_data": {"group": "Burst", "search": "AllSky"},
                 "far": 1e-6}
+    elif graceid == "S9988":
+        return {"superevent_id": "S9988",
+                "preferred_event": "G000003",
+                "preferred_event_data": {"group": "Burst", "search": "BBH"},
+                "far": 1e-7}
     elif graceid == "S9999":
-        return {"superevent_id": "S9876",
+        return {"superevent_id": "S9999",
                 "preferred_event": "G000003",
                 "preferred_event_data": {"group": "Burst", "search": "AllSky"},
                 "far": -1e-6}
     elif graceid == "TS1111":
         return {"superevent_id": "TS1111",
                 "preferred_event": "G000003",
                 "preferred_event_data": {"group": "Test", "search": "AllSky"},
                 "far": 1e-6}
     elif graceid == "MS1111":
         return {"superevent_id": "MS1111",
                 "preferred_event": "M000004",
-                "preferred_event_data": {"group": "CBC", "search": "AllSky"},
+                "preferred_event_data": {"group": "CBC", "search": "MDC"},
                 "far": 1e-9}
     elif graceid == 'E1':
         return {"graceid": "E1",
                 "pipeline": 'Swift',
                 "search": 'GRB',
                 "labels": [],
                 "group": 'External'}
@@ -605,14 +627,17 @@
                 "spatiotemporal_coinc_far": None}
     elif graceid == "S8642":
         return {"temporal_coinc_far": 1e-03,
                 "spatiotemporal_coinc_far": None}
     elif graceid == "S9876":
         return {"temporal_coinc_far": 1e-07,
                 "spatiotemporal_coinc_far": 1e-13}
+    elif graceid == "S9988":
+        return {"temporal_coinc_far": 1e-09,
+                "spatiotemporal_coinc_far": 1e-14}
     elif graceid == "MS1111":
         return {"temporal_coinc_far": 1e-09,
                 "spatiotemporal_coinc_far": 1e-10}
     elif graceid == "S9999":
         return {"temporal_coinc_far": -1e-09,
                 "spatiotemporal_coinc_far": -1e-10}
     else:
@@ -630,14 +655,15 @@
      ['S2468', 'E5', 'CBC', False],
      ['S2468', 'E2', 'CBC', False],
      ['S2345', 'E3', 'Burst', True],
      ['MS1111', 'M6', 'CBC', True],
      ['S5678', 'E1', 'CBC', False],
      ['S5678', 'E7', 'CBC', False],
      ['E1', 'S9876', 'CBC', True],
+     ['E1', 'S9988', 'Burst', True],
      ['E1', 'S2468', 'CBC', False],
      ['E2', 'S5678', 'CBC', False],
      ['E3', 'S8642', 'Burst', False],
      ['E3', 'S9876', 'Burst', True],
      ['T4', 'TS1111', 'CBC', False],
      ['E5', 'S5678', 'CBC', False],
      ['E8', 'S9876', None, True],
```

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_rrt_utils.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_rrt_utils.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_skymaps.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tasks_superevents.py` & `gwcelery-2.4.1/gwcelery/tests/test_tasks_superevents.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tempfile.py` & `gwcelery-2.4.1/gwcelery/tests/test_tempfile.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tools_condor.py` & `gwcelery-2.4.1/gwcelery/tests/test_tools_condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tools_condor_submit_helper.py` & `gwcelery-2.4.1/gwcelery/tests/test_tools_condor_submit_helper.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tools_flask.py` & `gwcelery-2.4.1/gwcelery/tests/test_tools_flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_tools_nagios.py` & `gwcelery-2.4.1/gwcelery/tests/test_tools_nagios.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tests/test_views.py` & `gwcelery-2.4.1/gwcelery/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tools/condor.py` & `gwcelery-2.4.1/gwcelery/tools/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tools/condor_submit_helper.py` & `gwcelery-2.4.1/gwcelery/tools/condor_submit_helper.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tools/flask.py` & `gwcelery-2.4.1/gwcelery/tools/flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/tools/nagios.py` & `gwcelery-2.4.1/gwcelery/tools/nagios.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/util/cmdline.py` & `gwcelery-2.4.1/gwcelery/util/cmdline.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/util/resources.py` & `gwcelery-2.4.1/gwcelery/util/resources.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/util/tempfile.py` & `gwcelery-2.4.1/gwcelery/util/tempfile.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/views.py` & `gwcelery-2.4.1/gwcelery/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -499,15 +499,15 @@
     flash('Queued a mock event.', 'success')
     return redirect(url_for('index'))
 
 
 @gracedb.task(shared=False)
 def _create_upload_external_event(gpstime):
     new_time = first2years_external._offset_time(
-        gpstime, 'CBC', 'Fermi', 'GRB')
+        gpstime, 'CBC', 'Fermi', 'GRB', 'MDC')
 
     ext_event = first2years_external.create_upload_external_event(
                     new_time, 'Fermi', 'MDC')
 
     return ext_event
```

### Comparing `gwcelery-2.3.6/gwcelery/voevent/bootsteps.py` & `gwcelery-2.4.1/gwcelery/voevent/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/voevent/logging.py` & `gwcelery-2.4.1/gwcelery/voevent/logging.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/voevent/signals.py` & `gwcelery-2.4.1/gwcelery/voevent/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/voevent/subscriber.py` & `gwcelery-2.4.1/gwcelery/voevent/subscriber.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/gwcelery/voevent/util.py` & `gwcelery-2.4.1/gwcelery/voevent/util.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.6/pyproject.toml` & `gwcelery-2.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gwcelery"
-version = "2.3.6"
+version = "2.4.1"
 description = "Low-latency pipeline for annotating IGWN events"
 readme = "README.rst"
 authors = [
     "Deep Chatterjee <deep.chatterjee@ligo.org>",
     "Cody Messick <cody.messick@ligo.org>",
     "Geoffrey Mo <geoffrey.mo@ligo.org>",
     "Leo Singer <leo.singer@ligo.org>"
@@ -51,39 +51,39 @@
 "Bug Tracker" = "https://git.ligo.org/emfollow/gwcelery/issues"
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
 adc-streaming = ">=2.3.0"  # https://github.com/astronomy-commons/adc-streaming/pull/62
 astropy = ">=4.3.1,!=5.3"  # https://github.com/astropy/astropy/issues/11879, https://github.com/gwpy/gwpy/issues/1629
 bilby = ">=2.2.2"
-bilby_pipe = ">=1.3.0"
+bilby_pipe = ">=1.3.1"
 celery = {version = ">=5.1, <5.4", extras = ["redis"]}  # https://git.ligo.org/emfollow/gwcelery/-/issues/804
 ciecplib = {version = "*", extras = ["kerberos"]}  # for renew-cert.sh
 click = ">=7"
 comet = "*"
 confluent-kafka = ">=1.9.2"
 flask = ">=2.2,<3.0"  # https://github.com/pytest-dev/pytest-flask/issues/167
 flask-caching = "*"
 gracedb-sdk = ">=0.2.0"  # https://git.ligo.org/emfollow/gracedb-sdk/-/merge_requests/7
 gwdatafind = ">=1.1.1"
 gwpy = ">=3.0.8"  # https://git.ligo.org/emfollow/gwcelery/-/issues/183
-GWSkyNet = "2.4.0" # https://git.ligo.org/computing/sccb/-/issues/1153 # https://git.ligo.org/emfollow/gwcelery/-/merge_requests/1386
+GWSkyNet = "2.4.1" # https://git.ligo.org/emfollow/gwcelery/-/issues/774
 healpy = "*"
 hop-client = ">=0.7.0"  # https://github.com/scimma/hop-client/pull/176
 igwn-alert = ">=0.2.2"
 igwn-gwalert-schema = "^1.0.0"
 imapclient = "*"
 importlib-metadata = { version = "*"}
 jinja2 = ">=2.11.2"  # https://github.com/pallets/jinja/issues/1168
 lalsuite = ">=7.16"  # https://git.ligo.org/lscsoft/lalsuite/-/merge_requests/2120
 ligo-followup-advocate = ">=1.2.8"  # https://git.ligo.org/computing/sccb/-/issues/1348
 ligo-gracedb = ">=2.7.5"  # https://git.ligo.org/lscsoft/gracedb-client/-/issues/28
-ligo-raven = ">=3.2"
+ligo-raven = ">=3.2,<4.0"
 ligo-segments = "*"
-"ligo.em-bright" = ">=1.1.4.post2"  # https://git.ligo.org/emfollow/gwcelery/-/issues/653
+"ligo.em-bright" = ">=1.1.4.post2,<1.1.7"  # https://git.ligo.org/emfollow/gwcelery/-/issues/816
 "ligo.skymap" = ">=1.1.0"  # https://git.ligo.org/lscsoft/ligo.skymap/-/merge_requests/327
 lscsoft-glue = "*"
 lxml = "*"
 matplotlib = "<3.7"  # Matplotlib changed an axes behaviour which breaks some of our plotting scripts. When gwpy has a new release, we can unpin this.
 numba = ">=0.56"  # Poetry update chooses an old version of numba and its deps that break the python3.9 and 3.10 build tests if this is not specified; dependence on numba comes from rift. Version chosen because it adds python 3.10 support. This requirement can be dropped here if RIFT adds it https://git.ligo.org/rapidpe-rift/rift/-/issues/24
 numpy = "*"
 p_astro = ">=1.0.1"  # https://git.ligo.org/lscsoft/p-astro/-/merge_requests/40
@@ -95,15 +95,14 @@
 rapidpe-rift-pipe = ">=0.6.8"  # https://git.ligo.org/computing/sccb/-/issues/1449
 redis = "!=4.5.2,!=4.5.3"  # https://git.ligo.org/emfollow/gwcelery/-/issues/556
 RIFT = ">=0.0.15.9"
 scipy = ">=1.11.1"  # https://git.ligo.org/emfollow/gwcelery/-/issues/679
 safe-netrc = "*"
 sentry-sdk = {version = "*", extras = ["flask", "tornado"]}
 service-identity = "*"  # We don't actually use this package, but it silences some annoying warnings from twistd.
-tensorflow-cpu = "<2.16" # https://git.ligo.org/emfollow/gwcelery/-/issues/774
 voeventlib = ">=1.2"
 werkzeug = ">=3.0.1"  # for werkzeug.middleware.proxy_fix.ProxyFix # https://git.ligo.org/emfollow/gwcelery/-/issues/736
 zstandard = "*"  # for task compression
 
 # For docs
 pep517 = {version="*", optional=true}
 sphinx = {version=">=4.0, <=5.3.0", optional=true}  # https://git.ligo.org/andrew.toivonen/gwcelery/-/jobs/2447152
```

### Comparing `gwcelery-2.3.6/PKG-INFO` & `gwcelery-2.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwcelery
-Version: 2.3.6
+Version: 2.4.1
 Summary: Low-latency pipeline for annotating IGWN events
 Home-page: https://git.ligo.org/emfollow/gwcelery
 License: GPL-2.0+
 Author: Deep Chatterjee
 Author-email: deep.chatterjee@ligo.org
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 4 - Beta
@@ -17,20 +17,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides-Extra: doc
 Provides-Extra: test
-Requires-Dist: GWSkyNet (==2.4.0)
+Requires-Dist: GWSkyNet (==2.4.1)
 Requires-Dist: RIFT (>=0.0.15.9)
 Requires-Dist: adc-streaming (>=2.3.0)
 Requires-Dist: astropy (>=4.3.1,!=5.3)
 Requires-Dist: bilby (>=2.2.2)
-Requires-Dist: bilby_pipe (>=1.3.0)
+Requires-Dist: bilby_pipe (>=1.3.1)
 Requires-Dist: celery[redis] (>=5.1,<5.4)
 Requires-Dist: ciecplib[kerberos]
 Requires-Dist: click (>=7)
 Requires-Dist: comet
 Requires-Dist: confluent-kafka (>=1.9.2)
 Requires-Dist: fastavro (>=1.6.1,<2.0.0) ; extra == "test"
 Requires-Dist: flask (>=2.2,<3.0)
@@ -46,18 +46,18 @@
 Requires-Dist: igwn-gwalert-schema (>=1.0.0,<2.0.0)
 Requires-Dist: imapclient
 Requires-Dist: importlib-metadata
 Requires-Dist: jinja2 (>=2.11.2)
 Requires-Dist: lalsuite (>=7.16)
 Requires-Dist: ligo-followup-advocate (>=1.2.8)
 Requires-Dist: ligo-gracedb (>=2.7.5)
-Requires-Dist: ligo-raven (>=3.2)
+Requires-Dist: ligo-raven (>=3.2,<4.0)
 Requires-Dist: ligo-rrt-chat (>=0.1.1)
 Requires-Dist: ligo-segments
-Requires-Dist: ligo.em-bright (>=1.1.4.post2)
+Requires-Dist: ligo.em-bright (>=1.1.4.post2,<1.1.7)
 Requires-Dist: ligo.skymap (>=1.1.0)
 Requires-Dist: lscsoft-glue
 Requires-Dist: lxml
 Requires-Dist: matplotlib (<3.7)
 Requires-Dist: numba (>=0.56)
 Requires-Dist: numpy
 Requires-Dist: p_astro (>=1.0.1)
@@ -74,15 +74,14 @@
 Requires-Dist: rapidpe-rift-pipe (>=0.6.8)
 Requires-Dist: redis (!=4.5.2,!=4.5.3)
 Requires-Dist: safe-netrc
 Requires-Dist: scipy (>=1.11.1)
 Requires-Dist: sentry-sdk[flask,tornado]
 Requires-Dist: service-identity
 Requires-Dist: sphinx (>=4.0,<=5.3.0) ; extra == "doc"
-Requires-Dist: tensorflow-cpu (<2.16)
 Requires-Dist: voeventlib (>=1.2)
 Requires-Dist: werkzeug (>=3.0.1)
 Requires-Dist: zstandard
 Project-URL: Bug Tracker, https://git.ligo.org/emfollow/gwcelery/issues
 Project-URL: Documentation, https://gwcelery.readthedocs.io/
 Project-URL: Repository, https://git.ligo.org/emfollow/gwcelery
 Description-Content-Type: text/x-rst
```

