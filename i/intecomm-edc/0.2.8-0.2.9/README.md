# Comparing `tmp/intecomm-edc-0.2.8.tar.gz` & `tmp/intecomm-edc-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intecomm-edc-0.2.8.tar", last modified: Mon Feb 26 13:01:26 2024, max compression
+gzip compressed data, was "intecomm-edc-0.2.9.tar", last modified: Mon Feb 26 13:27:16 2024, max compression
```

## Comparing `intecomm-edc-0.2.8.tar` & `intecomm-edc-0.2.9.tar`

### file list

```diff
@@ -1,1140 +1,1141 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.764068 intecomm-edc-0.2.8/
--rw-r--r--   0 erikvw     (501) staff       (20)      261 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-08-13 15:16:15.000000 intecomm-edc-0.2.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.522320 intecomm-edc-0.2.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.537444 intecomm-edc-0.2.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2315 2024-02-15 12:37:45.000000 intecomm-edc-0.2.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1486 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1227 2024-02-15 12:37:45.000000 intecomm-edc-0.2.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)      309 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)    10047 2023-12-05 05:12:56.000000 intecomm-edc-0.2.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-11-22 15:26:51.000000 intecomm-edc-0.2.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      225 2023-08-24 03:01:35.000000 intecomm-edc-0.2.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     3937 2024-02-26 13:01:26.763984 intecomm-edc-0.2.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     2898 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.523050 intecomm-edc-0.2.8/bin/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.537656 intecomm-edc-0.2.8/bin/nginx/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.538462 intecomm-edc-0.2.8/bin/nginx/conf/
--rw-r--r--   0 erikvw     (501) staff       (20)     1202 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/bin/nginx/conf/intecomm_live.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      432 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/bin/nginx/conf/intecomm_live_sites.conf
--rw-r--r--   0 erikvw     (501) staff       (20)     1282 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/bin/nginx/conf/intecomm_uat.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      435 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/bin/nginx/conf/intecomm_uat_sites.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      290 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/bin/nginx/intecomm.clinicedc.org.conf
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.522614 intecomm-edc-0.2.8/bin/nginx/www/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.522858 intecomm-edc-0.2.8/bin/nginx/www/html/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.538609 intecomm-edc-0.2.8/bin/nginx/www/html/live.intecomm.clinicedc.org/
--rw-r--r--   0 erikvw     (501) staff       (20)     1464 2022-11-23 01:31:30.000000 intecomm-edc-0.2.8/bin/nginx/www/html/live.intecomm.clinicedc.org/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.538938 intecomm-edc-0.2.8/bin/nginx/www/html/live.intecomm.clinicedc.org/tz/
--rw-r--r--   0 erikvw     (501) staff       (20)     2297 2023-01-25 03:04:55.000000 intecomm-edc-0.2.8/bin/nginx/www/html/live.intecomm.clinicedc.org/tz/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.539382 intecomm-edc-0.2.8/bin/nginx/www/html/live.intecomm.clinicedc.org/ug/
--rw-r--r--   0 erikvw     (501) staff       (20)     2281 2023-01-25 03:04:55.000000 intecomm-edc-0.2.8/bin/nginx/www/html/live.intecomm.clinicedc.org/ug/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.539573 intecomm-edc-0.2.8/bin/nginx/www/html/uat.intecomm.clinicedc.org/
--rw-r--r--   0 erikvw     (501) staff       (20)     1464 2022-11-23 01:31:30.000000 intecomm-edc-0.2.8/bin/nginx/www/html/uat.intecomm.clinicedc.org/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.539777 intecomm-edc-0.2.8/bin/nginx/www/html/uat.intecomm.clinicedc.org/tz/
--rw-r--r--   0 erikvw     (501) staff       (20)     2334 2023-01-25 03:04:55.000000 intecomm-edc-0.2.8/bin/nginx/www/html/uat.intecomm.clinicedc.org/tz/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.539924 intecomm-edc-0.2.8/bin/nginx/www/html/uat.intecomm.clinicedc.org/ug/
--rw-r--r--   0 erikvw     (501) staff       (20)     2318 2023-01-25 03:04:55.000000 intecomm-edc-0.2.8/bin/nginx/www/html/uat.intecomm.clinicedc.org/ug/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.540543 intecomm-edc-0.2.8/bin/systemd/
--rwxr-xr-x   0 erikvw     (501) staff       (20)      435 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/bin/systemd/gunicorn-live.service
--rwxr-xr-x   0 erikvw     (501) staff       (20)      133 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/bin/systemd/gunicorn-live.socket
--rwxr-xr-x   0 erikvw     (501) staff       (20)      433 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/bin/systemd/gunicorn-uat.service
--rwxr-xr-x   0 erikvw     (501) staff       (20)      131 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/bin/systemd/gunicorn-uat.socket
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/codecov.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     5118 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/env.sample
--rw-r--r--   0 erikvw     (501) staff       (20)     1048 2021-08-13 15:16:15.000000 intecomm-edc-0.2.8/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.542394 intecomm-edc-0.2.8/intecomm_ae/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_ae/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6126 2023-09-22 03:18:08.000000 intecomm-edc-0.2.8/intecomm_ae/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.543401 intecomm-edc-0.2.8/intecomm_ae/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      197 2023-08-16 02:41:30.000000 intecomm-edc-0.2.8/intecomm_ae/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      707 2023-09-27 00:31:13.000000 intecomm-edc-0.2.8/intecomm_ae/admin/ae_followup_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1826 2023-09-27 00:31:13.000000 intecomm-edc-0.2.8/intecomm_ae/admin/ae_initial_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2784 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_ae/admin/death_report_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      748 2023-09-27 00:31:13.000000 intecomm-edc-0.2.8/intecomm_ae/admin/hospitalization_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      167 2022-10-18 02:23:36.000000 intecomm-edc-0.2.8/intecomm_ae/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      293 2023-11-30 05:45:16.000000 intecomm-edc-0.2.8/intecomm_ae/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1015 2023-08-16 02:41:30.000000 intecomm-edc-0.2.8/intecomm_ae/baker_recipes.py
--rw-r--r--   0 erikvw     (501) staff       (20)      756 2022-04-11 18:27:09.000000 intecomm-edc-0.2.8/intecomm_ae/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)       36 2022-04-11 18:27:09.000000 intecomm-edc-0.2.8/intecomm_ae/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.544878 intecomm-edc-0.2.8/intecomm_ae/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      189 2023-08-16 02:41:30.000000 intecomm-edc-0.2.8/intecomm_ae/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      298 2023-08-14 13:42:28.000000 intecomm-edc-0.2.8/intecomm_ae/forms/ae_followup_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      791 2023-08-16 02:41:30.000000 intecomm-edc-0.2.8/intecomm_ae/forms/ae_initial_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1424 2023-08-14 13:42:28.000000 intecomm-edc-0.2.8/intecomm_ae/forms/death_report_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      365 2023-08-16 02:41:30.000000 intecomm-edc-0.2.8/intecomm_ae/forms/hospitalization_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      874 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_ae/forms/modelform_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1248 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_ae/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.549208 intecomm-edc-0.2.8/intecomm_ae/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)   144620 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_ae/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5271 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_ae/migrations/0002_rename_narrative_aetmg_investigator_narrative_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1663 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_ae/migrations/0003_alter_deathreporttmg_cause_of_death_agreed_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2820 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_ae/migrations/0004_alter_aefollowup_options_alter_aeinitial_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2355 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_ae/migrations/0005_alter_aefollowup_managers_alter_aeinitial_managers_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    21815 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_ae/migrations/0006_hospitalization_historicalhospitalization.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2892 2023-08-16 02:41:30.000000 intecomm-edc-0.2.8/intecomm_ae/migrations/0007_aeinitial_ae_classification_as_text_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5140 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_ae/migrations/0008_alter_deathreporttmgsecond_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    20568 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_ae/migrations/0009_alter_aefollowup_device_created_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2068 2023-11-16 04:10:04.000000 intecomm-edc-0.2.8/intecomm_ae/migrations/0010_alter_deathreport_death_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    15388 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_ae/migrations/0011_alter_aefollowup_options_alter_aeinitial_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3328 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_ae/migrations/0012_aefollowup_intecomm_ae_subject_a0869e_idx_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4003 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_ae/migrations/0013_aetmg_intecomm_ae_subject_a182a3_idx_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5642 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_ae/migrations/0014_alter_aefollowup_site_alter_aeinitial_site_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_ae/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.549583 intecomm-edc-0.2.8/intecomm_ae/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)       54 2023-08-16 02:41:30.000000 intecomm-edc-0.2.8/intecomm_ae/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2666 2023-08-16 02:41:30.000000 intecomm-edc-0.2.8/intecomm_ae/model_mixins/ae_review_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.551156 intecomm-edc-0.2.8/intecomm_ae/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      211 2023-08-16 02:41:30.000000 intecomm-edc-0.2.8/intecomm_ae/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      406 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_ae/models/ae_followup.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1900 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_ae/models/ae_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      948 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_ae/models/compatability.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1817 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_ae/models/death_report.py
--rw-r--r--   0 erikvw     (501) staff       (20)      802 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_ae/models/hospitalization.py
--rw-r--r--   0 erikvw     (501) staff       (20)      620 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_ae/models/managers.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.551726 intecomm-edc-0.2.8/intecomm_ae/pdf_reports/
--rw-r--r--   0 erikvw     (501) staff       (20)       84 2023-08-16 02:41:30.000000 intecomm-edc-0.2.8/intecomm_ae/pdf_reports/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1365 2023-08-16 02:41:30.000000 intecomm-edc-0.2.8/intecomm_ae/pdf_reports/ae_pdf_report.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1135 2023-08-16 02:41:30.000000 intecomm-edc-0.2.8/intecomm_ae/pdf_reports/death_pdf_report.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.523601 intecomm-edc-0.2.8/intecomm_ae/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.523649 intecomm-edc-0.2.8/intecomm_ae/templates/intecomm_ae/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.551905 intecomm-edc-0.2.8/intecomm_ae/templates/intecomm_ae/bootstrap3/
--rw-r--r--   0 erikvw     (501) staff       (20)      889 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_ae/templates/intecomm_ae/bootstrap3/ae_initial_description.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.552243 intecomm-edc-0.2.8/intecomm_ae/templatetags/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_ae/templatetags/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1215 2023-08-16 02:41:30.000000 intecomm-edc-0.2.8/intecomm_ae/templatetags/protocol_ae_extras.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.552819 intecomm-edc-0.2.8/intecomm_ae/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_ae/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_ae/tests/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.553070 intecomm-edc-0.2.8/intecomm_ae/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 intecomm-edc-0.2.8/intecomm_ae/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      259 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_ae/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      205 2022-10-18 02:24:15.000000 intecomm-edc-0.2.8/intecomm_ae/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.554129 intecomm-edc-0.2.8/intecomm_auth/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_auth/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      233 2022-03-12 18:30:44.000000 intecomm-edc-0.2.8/intecomm_auth/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1166 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_auth/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2325 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_auth/auths.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.554365 intecomm-edc-0.2.8/intecomm_auth/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_auth/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.554592 intecomm-edc-0.2.8/intecomm_auth/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_auth/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      819 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_auth/tests/tests/test_auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_auth/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.556098 intecomm-edc-0.2.8/intecomm_consent/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_consent/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.557471 intecomm-edc-0.2.8/intecomm_consent/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      182 2024-02-01 03:43:59.000000 intecomm-edc-0.2.8/intecomm_consent/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1179 2023-08-29 02:39:08.000000 intecomm-edc-0.2.8/intecomm_consent/admin/fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3075 2024-02-01 06:39:00.000000 intecomm-edc-0.2.8/intecomm_consent/admin/modeladmin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1688 2024-02-01 03:43:59.000000 intecomm-edc-0.2.8/intecomm_consent/admin/subject_consent_tz_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1867 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_consent/admin/subject_consent_ug_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      754 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_consent/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-03-12 18:10:23.000000 intecomm-edc-0.2.8/intecomm_consent/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1104 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_consent/baker_recipes.py
--rw-r--r--   0 erikvw     (501) staff       (20)      826 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_consent/consents.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.558327 intecomm-edc-0.2.8/intecomm_consent/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      176 2024-02-01 03:43:59.000000 intecomm-edc-0.2.8/intecomm_consent/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2255 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_consent/forms/modelform_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      295 2024-02-01 03:43:59.000000 intecomm-edc-0.2.8/intecomm_consent/forms/subject_consent_tz_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      295 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_consent/forms/subject_consent_ug_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.558538 intecomm-edc-0.2.8/intecomm_consent/management/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-03-03 20:12:26.000000 intecomm-edc-0.2.8/intecomm_consent/management/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.558720 intecomm-edc-0.2.8/intecomm_consent/management/commands/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-03-03 20:12:26.000000 intecomm-edc-0.2.8/intecomm_consent/management/commands/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_consent/management/commands/create_missing_prescriptions.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.564250 intecomm-edc-0.2.8/intecomm_consent/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    69089 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5396 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0002_remove_subjectconsent_intecomm_co_subject_145905_idx_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1535 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0003_alter_historicalsubjectconsent_language_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1951 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0004_alter_historicalsubjectconsent_familiar_name_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1016 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0005_remove_subjectconsent_unique_consent_subject_id_and_version_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      696 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0006_historicalsubjectconsent_group_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1575 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0007_alter_historicalsubjectconsent_language_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1055 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0008_alter_historicalsubjectconsent_screening_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      922 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0009_alter_subjectconsent_options.py
--rw-r--r--   0 erikvw     (501) staff       (20)      667 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0010_alter_subjectreconsent_options.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2234 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0011_alter_subjectconsent_unique_together_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5369 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0012_alter_historicalsubjectconsent_device_created_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      859 2023-08-29 02:39:08.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0013_subjectconsentug.py
--rw-r--r--   0 erikvw     (501) staff       (20)      482 2023-08-29 02:39:08.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0014_alter_subjectconsentug_options.py
--rw-r--r--   0 erikvw     (501) staff       (20)    24440 2023-08-29 02:39:08.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0015_historicalsubjectconsentug.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2353 2023-09-22 03:18:08.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0016_alter_historicalsubjectconsent_language_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5014 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0017_alter_subjectconsent_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1700 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0018_subjectconsent_intecomm_co_modifie_45691e_idx_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1566 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0019_historicalsubjectconsent_model_name_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      664 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0020_auto_20240111_0115.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2072 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0021_remove_subjectreconsent_action_item_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    26393 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0022_subjectconsenttz_historicalsubjectconsenttz.py
--rw-r--r--   0 erikvw     (501) staff       (20)      640 2024-02-01 16:00:54.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/0023_alter_subjectconsent_managers.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_consent/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.565488 intecomm-edc-0.2.8/intecomm_consent/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      361 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_consent/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      296 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_consent/models/model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3199 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_consent/models/signals.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4688 2024-02-06 04:30:17.000000 intecomm-edc-0.2.8/intecomm_consent/models/subject_consent.py
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_consent/models/subject_consent_tz.py
--rw-r--r--   0 erikvw     (501) staff       (20)      252 2024-01-28 23:23:52.000000 intecomm-edc-0.2.8/intecomm_consent/models/subject_consent_ug.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.524559 intecomm-edc-0.2.8/intecomm_consent/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.524608 intecomm-edc-0.2.8/intecomm_consent/templates/intecomm_consent/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.565857 intecomm-edc-0.2.8/intecomm_consent/templates/intecomm_consent/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)     1829 2024-02-01 06:39:00.000000 intecomm-edc-0.2.8/intecomm_consent/templates/intecomm_consent/admin/subjectconsent_change_list.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.566643 intecomm-edc-0.2.8/intecomm_consent/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_consent/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_consent/tests/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.567501 intecomm-edc-0.2.8/intecomm_consent/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 intecomm-edc-0.2.8/intecomm_consent/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8866 2024-02-01 03:43:59.000000 intecomm-edc-0.2.8/intecomm_consent/tests/tests/test_subject_consent.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3051 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_consent/tests/tests/test_webtest.py
--rw-r--r--   0 erikvw     (501) staff       (20)      920 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_consent/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      210 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_consent/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1810 2023-08-29 02:39:08.000000 intecomm-edc-0.2.8/intecomm_consent/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.568836 intecomm-edc-0.2.8/intecomm_dashboard/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_dashboard/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      248 2023-07-02 21:12:50.000000 intecomm-edc-0.2.8/intecomm_dashboard/apps.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.569191 intecomm-edc-0.2.8/intecomm_dashboard/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_dashboard/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1163 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_dashboard/navbars.py
--rw-r--r--   0 erikvw     (501) staff       (20)       47 2022-06-24 09:14:59.000000 intecomm-edc-0.2.8/intecomm_dashboard/patterns.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.524981 intecomm-edc-0.2.8/intecomm_dashboard/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.525032 intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.569299 intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.571308 intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/
--rw-r--r--   0 erikvw     (501) staff       (20)      466 2022-11-23 01:31:30.000000 intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/add_consent_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)      239 2024-01-27 22:17:38.000000 intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/dashboard_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)      401 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/eligibility_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)      429 2022-11-23 01:31:30.000000 intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/patient_group_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)      365 2022-11-23 01:31:30.000000 intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/patient_log_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)      437 2023-05-04 03:51:54.000000 intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/refusal_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)      341 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/screening_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1739 2023-08-29 02:39:08.000000 intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/changelist_topbar.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.572140 intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/screening/
--rw-r--r--   0 erikvw     (501) staff       (20)     3973 2023-08-29 02:39:08.000000 intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/screening/listboard.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.572956 intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/
--rw-r--r--   0 erikvw     (501) staff       (20)      893 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/buttons_column.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.573224 intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/dashboard/
--rw-r--r--   0 erikvw     (501) staff       (20)      231 2023-05-11 02:01:11.000000 intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/dashboard/top_bar.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1035 2024-02-08 12:55:55.000000 intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/dashboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)     2876 2024-02-08 12:55:55.000000 intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/subject_listboard.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.573678 intecomm-edc-0.2.8/intecomm_dashboard/templatetags/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_dashboard/templatetags/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6828 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_dashboard/templatetags/protocol_dashboard_extras.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.574430 intecomm-edc-0.2.8/intecomm_dashboard/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_dashboard/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      720 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_dashboard/tests/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_dashboard/tests/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.574712 intecomm-edc-0.2.8/intecomm_dashboard/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_dashboard/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2399 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_dashboard/tests/tests/test_views.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2828 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_dashboard/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1204 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_dashboard/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.574929 intecomm-edc-0.2.8/intecomm_dashboard/views/
--rw-r--r--   0 erikvw     (501) staff       (20)      187 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_dashboard/views/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.575565 intecomm-edc-0.2.8/intecomm_dashboard/views/ae/
--rw-r--r--   0 erikvw     (501) staff       (20)      113 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_dashboard/views/ae/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      119 2023-08-16 02:41:30.000000 intecomm-edc-0.2.8/intecomm_dashboard/views/ae/ae_listboard_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      146 2023-08-16 02:41:30.000000 intecomm-edc-0.2.8/intecomm_dashboard/views/ae/death_report_listboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.575988 intecomm-edc-0.2.8/intecomm_dashboard/views/screening/
--rw-r--r--   0 erikvw     (501) staff       (20)       42 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_dashboard/views/screening/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2541 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_dashboard/views/screening/listboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.576621 intecomm-edc-0.2.8/intecomm_dashboard/views/subject/
--rw-r--r--   0 erikvw     (501) staff       (20)      114 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_dashboard/views/subject/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3413 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_dashboard/views/subject/subject_dashboard_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4059 2024-02-01 16:00:54.000000 intecomm-edc-0.2.8/intecomm_dashboard/views/subject/subject_listboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.578839 intecomm-edc-0.2.8/intecomm_edc/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_edc/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      927 2022-07-07 11:06:18.000000 intecomm-edc-0.2.8/intecomm_edc/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      382 2024-01-25 17:45:05.000000 intecomm-edc-0.2.8/intecomm_edc/apps.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.579949 intecomm-edc-0.2.8/intecomm_edc/management/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-02-01 03:43:59.000000 intecomm-edc-0.2.8/intecomm_edc/management/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.580150 intecomm-edc-0.2.8/intecomm_edc/management/commands/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-02-01 03:43:59.000000 intecomm-edc-0.2.8/intecomm_edc/management/commands/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1130 2024-02-01 03:43:59.000000 intecomm-edc-0.2.8/intecomm_edc/management/commands/update_forms_reference.py
--rw-r--r--   0 erikvw     (501) staff       (20)       46 2020-03-04 23:21:43.000000 intecomm-edc-0.2.8/intecomm_edc/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1255 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_edc/navbars.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.582181 intecomm-edc-0.2.8/intecomm_edc/settings/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-03 04:33:09.000000 intecomm-edc-0.2.8/intecomm_edc/settings/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1408 2024-02-19 22:04:54.000000 intecomm-edc-0.2.8/intecomm_edc/settings/debug.py
--rw-r--r--   0 erikvw     (501) staff       (20)    19135 2024-02-15 12:37:45.000000 intecomm-edc-0.2.8/intecomm_edc/settings/defaults.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1065 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_edc/settings/live.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1936 2023-11-21 13:15:18.000000 intecomm-edc-0.2.8/intecomm_edc/settings/logging.py
--rw-r--r--   0 erikvw     (501) staff       (20)      596 2024-02-06 04:30:17.000000 intecomm-edc-0.2.8/intecomm_edc/settings/minimal.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1302 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_edc/settings/uat.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.526127 intecomm-edc-0.2.8/intecomm_edc/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.526186 intecomm-edc-0.2.8/intecomm_edc/templates/intecomm_edc/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.583365 intecomm-edc-0.2.8/intecomm_edc/templates/intecomm_edc/bootstrap3/
--rw-r--r--   0 erikvw     (501) staff       (20)      165 2021-08-09 19:25:29.000000 intecomm-edc-0.2.8/intecomm_edc/templates/intecomm_edc/bootstrap3/base.html
--rw-r--r--   0 erikvw     (501) staff       (20)     2480 2023-09-22 03:18:09.000000 intecomm-edc-0.2.8/intecomm_edc/templates/intecomm_edc/bootstrap3/followup_community.html
--rw-r--r--   0 erikvw     (501) staff       (20)     2159 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_edc/templates/intecomm_edc/bootstrap3/grouping.html
--rw-r--r--   0 erikvw     (501) staff       (20)     2330 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_edc/templates/intecomm_edc/bootstrap3/home.html
--rw-r--r--   0 erikvw     (501) staff       (20)     2466 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_edc/templates/intecomm_edc/bootstrap3/subjects_home.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.583586 intecomm-edc-0.2.8/intecomm_edc/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:21:43.000000 intecomm-edc-0.2.8/intecomm_edc/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.585746 intecomm-edc-0.2.8/intecomm_edc/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      687 2023-02-02 02:49:25.000000 intecomm-edc-0.2.8/intecomm_edc/tests/etc/randomization_list.csv
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-02-02 02:49:25.000000 intecomm-edc-0.2.8/intecomm_edc/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-02-02 02:49:25.000000 intecomm-edc-0.2.8/intecomm_edc/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2023-02-02 02:49:25.000000 intecomm-edc-0.2.8/intecomm_edc/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2023-02-02 02:49:25.000000 intecomm-edc-0.2.8/intecomm_edc/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2023-02-02 02:49:25.000000 intecomm-edc-0.2.8/intecomm_edc/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2023-02-02 02:49:25.000000 intecomm-edc-0.2.8/intecomm_edc/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-02-02 02:49:25.000000 intecomm-edc-0.2.8/intecomm_edc/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-02-02 02:49:25.000000 intecomm-edc-0.2.8/intecomm_edc/tests/etc/user-salt-restricted.key
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.586048 intecomm-edc-0.2.8/intecomm_edc/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 intecomm-edc-0.2.8/intecomm_edc/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_edc/tests/tests/test_endpoints.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3703 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_edc/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.586711 intecomm-edc-0.2.8/intecomm_edc/views/
--rw-r--r--   0 erikvw     (501) staff       (20)      121 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_edc/views/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      398 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_edc/views/grouping_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      382 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_edc/views/home_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      626 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_edc/views/subjects_home_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      179 2022-03-12 18:45:28.000000 intecomm-edc-0.2.8/intecomm_edc/wsgi.py
--rw-r--r--   0 erikvw     (501) staff       (20)      178 2022-03-12 18:45:28.000000 intecomm-edc-0.2.8/intecomm_edc/wsgi_live.py
--rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-03-12 18:45:28.000000 intecomm-edc-0.2.8/intecomm_edc/wsgi_uat.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.763621 intecomm-edc-0.2.8/intecomm_edc.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     3937 2024-02-26 13:01:26.000000 intecomm-edc-0.2.8/intecomm_edc.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)    54697 2024-02-26 13:01:26.000000 intecomm-edc-0.2.8/intecomm_edc.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-02-26 13:01:26.000000 intecomm-edc-0.2.8/intecomm_edc.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-07-19 12:31:42.000000 intecomm-edc-0.2.8/intecomm_edc.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)      127 2024-02-26 13:01:26.000000 intecomm-edc-0.2.8/intecomm_edc.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      241 2024-02-26 13:01:26.000000 intecomm-edc-0.2.8/intecomm_edc.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.587856 intecomm-edc-0.2.8/intecomm_export/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_export/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_export/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      175 2022-03-12 18:43:23.000000 intecomm-edc-0.2.8/intecomm_export/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      161 2022-03-12 18:43:17.000000 intecomm-edc-0.2.8/intecomm_export/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_export/tests.py
--rw-r--r--   0 erikvw     (501) staff       (20)      213 2022-03-12 18:43:14.000000 intecomm-edc-0.2.8/intecomm_export/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_export/views.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.589598 intecomm-edc-0.2.8/intecomm_facility/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_facility/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2139 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_facility/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      185 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_facility/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      295 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_facility/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      370 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_facility/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)      421 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_facility/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.591105 intecomm-edc-0.2.8/intecomm_facility/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    16078 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_facility/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2958 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_facility/migrations/0002_alter_healthfacility_device_created_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2128 2023-11-16 04:10:04.000000 intecomm-edc-0.2.8/intecomm_facility/migrations/0003_auto_20230726_2030.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2663 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_facility/migrations/0004_alter_healthfacility_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1047 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_facility/migrations/0005_alter_healthfacility_site_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_facility/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      785 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_facility/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.526725 intecomm-edc-0.2.8/intecomm_facility/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.526774 intecomm-edc-0.2.8/intecomm_facility/templates/intecomm_facility/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.591213 intecomm-edc-0.2.8/intecomm_facility/templates/intecomm_facility/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      253 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_facility/templates/intecomm_facility/admin/healthfacility_changelist.html
--rw-r--r--   0 erikvw     (501) staff       (20)      211 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_facility/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.593499 intecomm-edc-0.2.8/intecomm_group/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_group/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.595423 intecomm-edc-0.2.8/intecomm_group/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      327 2023-05-10 11:59:10.000000 intecomm-edc-0.2.8/intecomm_group/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2781 2023-07-10 18:57:10.000000 intecomm-edc-0.2.8/intecomm_group/admin/community_care_location_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      486 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_group/admin/list_filters.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7213 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_group/admin/patient_followup_call_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5090 2024-02-06 04:30:17.000000 intecomm-edc-0.2.8/intecomm_group/admin/patient_group_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1555 2023-07-10 18:57:10.000000 intecomm-edc-0.2.8/intecomm_group/admin/patient_group_appointment_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2104 2023-07-10 18:57:10.000000 intecomm-edc-0.2.8/intecomm_group/admin/patient_group_meeting_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_group/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      293 2023-11-30 05:45:16.000000 intecomm-edc-0.2.8/intecomm_group/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      509 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_group/baker_recipes.py
--rw-r--r--   0 erikvw     (501) staff       (20)      800 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_group/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2023-02-28 00:36:08.000000 intecomm-edc-0.2.8/intecomm_group/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)      100 2022-11-23 01:31:30.000000 intecomm-edc-0.2.8/intecomm_group/exceptions.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.596922 intecomm-edc-0.2.8/intecomm_group/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      317 2023-07-20 02:48:14.000000 intecomm-edc-0.2.8/intecomm_group/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      366 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_group/forms/community_care_location_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      380 2023-07-20 02:48:14.000000 intecomm-edc-0.2.8/intecomm_group/forms/patient_followup_call_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      372 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_group/forms/patient_group_appointment_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      495 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_group/forms/patient_group_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      360 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_group/forms/patient_group_meeting_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.601258 intecomm-edc-0.2.8/intecomm_group/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    29538 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_group/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3393 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_group/migrations/0002_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      598 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_group/migrations/0003_alter_historicalpatientgroup_group_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      665 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_group/migrations/0004_alter_patientgroup_patients.py
--rw-r--r--   0 erikvw     (501) staff       (20)    17784 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_group/migrations/0005_patientfollowupcall_historicalpatientfollowupcall.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2952 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_group/migrations/0006_remove_historicalpatientgroup_enforce_group_size_min_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3530 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_group/migrations/0007_remove_historicalpatientfollowupcall_attend_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2554 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_group/migrations/0008_patientgroup_dm_patients_patientgroup_hiv_patients_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1517 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_group/migrations/0009_auto_20221126_0358.py
--rw-r--r--   0 erikvw     (501) staff       (20)      575 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_group/migrations/0010_alter_patientgroup_managers.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1242 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_group/migrations/0011_alter_historicalpatientfollowupcall_respondent_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1532 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_group/migrations/0012_alter_historicalpatientgroup_status_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1517 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_group/migrations/0013_alter_historicalpatientgroup_status_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4350 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_group/migrations/0014_alter_communitycarelocation_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2126 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_group/migrations/0015_alter_patientgroupmeeting_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9152 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_group/migrations/0016_alter_communitycarelocation_device_created_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11048 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_group/migrations/0017_alter_communitycarelocation_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2731 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_group/migrations/0018_alter_communitycarelocation_site_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_group/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.603445 intecomm-edc-0.2.8/intecomm_group/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      512 2023-05-04 03:51:54.000000 intecomm-edc-0.2.8/intecomm_group/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2283 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_group/models/community_care_location.py
--rw-r--r--   0 erikvw     (501) staff       (20)      747 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_group/models/patient_followup_call.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4043 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_group/models/patient_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1062 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_group/models/patient_group_appointment.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1311 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_group/models/patient_group_meeting.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3710 2023-05-24 17:50:54.000000 intecomm-edc-0.2.8/intecomm_group/models/signals.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1946 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_group/models/utils.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6270 2023-11-21 01:43:28.000000 intecomm-edc-0.2.8/intecomm_group/patient_group_updater.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.527468 intecomm-edc-0.2.8/intecomm_group/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.603980 intecomm-edc-0.2.8/intecomm_group/templates/intecomm_group/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.605192 intecomm-edc-0.2.8/intecomm_group/templates/intecomm_group/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)     1310 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_group/templates/intecomm_group/admin/communitycarelocation_change_list.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1513 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_group/templates/intecomm_group/admin/patientfollowupcall_change_list.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1349 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_group/templates/intecomm_group/admin/patientgroup_change_list.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1470 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_group/templates/intecomm_group/admin/patientgroupappointment_change_list.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1452 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_group/templates/intecomm_group/admin/patientgroupmeeting_change_list.html
--rw-r--r--   0 erikvw     (501) staff       (20)      101 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_group/templates/intecomm_group/patient_followup_call_locator.html
--rw-r--r--   0 erikvw     (501) staff       (20)      631 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_group/templates/intecomm_group/patient_followup_call_summary.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.605608 intecomm-edc-0.2.8/intecomm_group/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_group/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      524 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_group/tests/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.605993 intecomm-edc-0.2.8/intecomm_group/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_group/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6053 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_group/tests/tests/test_add_subjects_after_rando.py
--rw-r--r--   0 erikvw     (501) staff       (20)      207 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_group/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4396 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_group/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.607965 intecomm-edc-0.2.8/intecomm_labs/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-07-02 03:53:00.000000 intecomm-edc-0.2.8/intecomm_labs/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)       87 2021-07-05 19:24:26.000000 intecomm-edc-0.2.8/intecomm_labs/aliquot_types.py
--rw-r--r--   0 erikvw     (501) staff       (20)      209 2022-03-12 18:19:55.000000 intecomm-edc-0.2.8/intecomm_labs/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1011 2022-11-29 06:19:20.000000 intecomm-edc-0.2.8/intecomm_labs/lab_profiles.py
--rw-r--r--   0 erikvw     (501) staff       (20)      128 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_labs/labs.py
--rw-r--r--   0 erikvw     (501) staff       (20)      481 2022-03-12 18:19:03.000000 intecomm-edc-0.2.8/intecomm_labs/list_data.py
--rw-r--r--   0 erikvw     (501) staff       (20)      500 2021-09-17 02:16:20.000000 intecomm-edc-0.2.8/intecomm_labs/processing_profiles.py
--rw-r--r--   0 erikvw     (501) staff       (20)      516 2023-12-06 16:38:41.000000 intecomm-edc-0.2.8/intecomm_labs/reportables.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.608438 intecomm-edc-0.2.8/intecomm_labs/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_labs/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.608960 intecomm-edc-0.2.8/intecomm_labs/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_labs/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      987 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_labs/tests/tests/test_labs.py
--rw-r--r--   0 erikvw     (501) staff       (20)      539 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_labs/tests/tests/test_reportables.py
--rw-r--r--   0 erikvw     (501) staff       (20)      116 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_labs/tests/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.610657 intecomm-edc-0.2.8/intecomm_lists/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_lists/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      630 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_lists/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-03-14 02:24:52.000000 intecomm-edc-0.2.8/intecomm_lists/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      287 2022-03-12 18:10:47.000000 intecomm-edc-0.2.8/intecomm_lists/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      750 2023-10-06 00:30:17.000000 intecomm-edc-0.2.8/intecomm_lists/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)       63 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_lists/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)    13385 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_lists/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.613757 intecomm-edc-0.2.8/intecomm_lists/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    77605 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_lists/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      465 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_lists/migrations/0002_delete_reasonsfortesting_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2717 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_lists/migrations/0003_dmmanagement_dmmanagement_intecomm_li_id_b4d41f_idx.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5252 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_lists/migrations/0004_rxmodificationreasons_rxmodifications_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2722 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_lists/migrations/0005_htnmanagement_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5229 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_lists/migrations/0006_consentrefusalreasons_screeningrefusalreasons_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6012 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_lists/migrations/0007_arvdrugs_extra_value_arvregimens_extra_value_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2838 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_lists/migrations/0008_medicationshortagereasons.py
--rw-r--r--   0 erikvw     (501) staff       (20)    66840 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_lists/migrations/0009_alter_arvdrugs_options_alter_arvregimens_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4742 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_lists/migrations/0010_remove_arvdrugs_intecomm_li_name_b55bdc_idx_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8363 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_lists/migrations/0011_accompanied_moneysources_travelmethods.py
--rw-r--r--   0 erikvw     (501) staff       (20)      610 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_lists/migrations/0012_visitreasons_custom_name.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_lists/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6430 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_lists/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.613860 intecomm-edc-0.2.8/intecomm_lists/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_lists/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.614076 intecomm-edc-0.2.8/intecomm_lists/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_lists/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      212 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_lists/tests/tests/test_lists.py
--rw-r--r--   0 erikvw     (501) staff       (20)      208 2022-03-12 18:05:17.000000 intecomm-edc-0.2.8/intecomm_lists/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.616133 intecomm-edc-0.2.8/intecomm_prn/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_prn/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4566 2024-01-10 16:23:30.000000 intecomm-edc-0.2.8/intecomm_prn/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.618709 intecomm-edc-0.2.8/intecomm_prn/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      499 2023-07-20 02:48:14.000000 intecomm-edc-0.2.8/intecomm_prn/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4724 2023-09-27 00:31:13.000000 intecomm-edc-0.2.8/intecomm_prn/admin/end_of_study_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1851 2023-09-27 00:31:13.000000 intecomm-edc-0.2.8/intecomm_prn/admin/loss_to_followup_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2624 2023-07-10 18:57:10.000000 intecomm-edc-0.2.8/intecomm_prn/admin/modeladmin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      591 2023-09-27 00:31:13.000000 intecomm-edc-0.2.8/intecomm_prn/admin/offschedule_comm_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      591 2023-09-27 00:31:13.000000 intecomm-edc-0.2.8/intecomm_prn/admin/offschedule_inte_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      379 2024-02-06 04:30:17.000000 intecomm-edc-0.2.8/intecomm_prn/admin/onschedule_comm_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      379 2024-02-06 04:30:17.000000 intecomm-edc-0.2.8/intecomm_prn/admin/onschedule_inte_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      783 2024-02-06 04:30:17.000000 intecomm-edc-0.2.8/intecomm_prn/admin/protocol_incident_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1552 2024-02-06 04:30:17.000000 intecomm-edc-0.2.8/intecomm_prn/admin/subject_locator_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      767 2024-02-06 04:30:17.000000 intecomm-edc-0.2.8/intecomm_prn/admin/subject_transfer_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      169 2022-10-18 02:27:53.000000 intecomm-edc-0.2.8/intecomm_prn/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      289 2023-11-30 05:45:16.000000 intecomm-edc-0.2.8/intecomm_prn/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3151 2022-11-29 06:19:20.000000 intecomm-edc-0.2.8/intecomm_prn/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      104 2023-08-13 21:38:00.000000 intecomm-edc-0.2.8/intecomm_prn/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.620746 intecomm-edc-0.2.8/intecomm_prn/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      481 2024-02-06 04:30:17.000000 intecomm-edc-0.2.8/intecomm_prn/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      937 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_prn/forms/end_of_study_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1404 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_prn/forms/loss_to_followup_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      959 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_prn/forms/offschedule_comm_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      959 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_prn/forms/offschedule_inte_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      953 2024-02-06 04:30:17.000000 intecomm-edc-0.2.8/intecomm_prn/forms/onschedule_comm_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      953 2024-02-06 04:30:17.000000 intecomm-edc-0.2.8/intecomm_prn/forms/onschedule_inte_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      231 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_prn/forms/protocol_incident_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      734 2024-02-06 04:30:17.000000 intecomm-edc-0.2.8/intecomm_prn/forms/subject_locator_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      817 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_prn/forms/subject_transfer_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2336 2023-07-27 02:22:12.000000 intecomm-edc-0.2.8/intecomm_prn/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.624985 intecomm-edc-0.2.8/intecomm_prn/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)   149190 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_prn/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3533 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_prn/migrations/0002_remove_endofstudy_delivery_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1913 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_prn/migrations/0003_historicalprotocolincident_reasons_withdrawn_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3192 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_prn/migrations/0004_rename_historicaloffschedulebaseline_historicaloffschedulecomm_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3237 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_prn/migrations/0005_rename_historicaloffschedulefollowup_historicaloffscheduleinte_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4029 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_prn/migrations/0006_alter_historicaloffschedulecomm_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4811 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_prn/migrations/0007_alter_losstofollowup_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      715 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_prn/migrations/0008_alter_endofstudy_options.py
--rw-r--r--   0 erikvw     (501) staff       (20)    18584 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_prn/migrations/0009_subjectlocator_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      855 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_prn/migrations/0010_alter_historicalsubjectlocator_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    21655 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_prn/migrations/0011_alter_endofstudy_device_created_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5276 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_prn/migrations/0012_alter_endofstudy_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    12574 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_prn/migrations/0013_endofstudy_locale_created_endofstudy_locale_modified_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6784 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_prn/migrations/0014_endofstudy_intecomm_pr_action__f3bf58_idx_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2295 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_prn/migrations/0015_protocolincident_intecomm_pr_subject_54092b_idx_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6447 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_prn/migrations/0016_alter_endofstudy_site_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_prn/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.627064 intecomm-edc-0.2.8/intecomm_prn/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      390 2023-08-13 21:28:05.000000 intecomm-edc-0.2.8/intecomm_prn/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3592 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_prn/models/end_of_study.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2328 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_prn/models/loss_to_followup.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1206 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_prn/models/offschedule_comm.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1204 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_prn/models/offschedule_inte.py
--rw-r--r--   0 erikvw     (501) staff       (20)      598 2024-02-06 04:30:17.000000 intecomm-edc-0.2.8/intecomm_prn/models/onschedule_comm.py
--rw-r--r--   0 erikvw     (501) staff       (20)      596 2024-02-06 04:30:17.000000 intecomm-edc-0.2.8/intecomm_prn/models/onschedule_inte.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1341 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_prn/models/protocol_incident.py
--rw-r--r--   0 erikvw     (501) staff       (20)      221 2023-07-20 02:48:14.000000 intecomm-edc-0.2.8/intecomm_prn/models/proxy.py
--rw-r--r--   0 erikvw     (501) staff       (20)      339 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_prn/models/subject_transfer.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.528559 intecomm-edc-0.2.8/intecomm_prn/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.627322 intecomm-edc-0.2.8/intecomm_prn/templates/intecomm_prn/
--rw-r--r--   0 erikvw     (501) staff       (20)     1279 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_prn/templates/intecomm_prn/changelist_locator_contacts.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.627683 intecomm-edc-0.2.8/intecomm_prn/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_prn/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.627896 intecomm-edc-0.2.8/intecomm_prn/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_prn/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      290 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_prn/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      206 2022-10-18 02:47:10.000000 intecomm-edc-0.2.8/intecomm_prn/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.630842 intecomm-edc-0.2.8/intecomm_screening/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_screening/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.634121 intecomm-edc-0.2.8/intecomm_screening/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      666 2023-08-29 02:39:08.000000 intecomm-edc-0.2.8/intecomm_screening/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1355 2023-07-20 02:48:14.000000 intecomm-edc-0.2.8/intecomm_screening/admin/actions.py
--rw-r--r--   0 erikvw     (501) staff       (20)      447 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_screening/admin/autocomplete_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1647 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_screening/admin/consent_refusal_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3305 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_screening/admin/health_facility_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2982 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_screening/admin/health_talk_log_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5273 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/admin/list_filters.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3837 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/admin/modeladmin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5262 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/admin/patient_call_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2248 2023-07-10 18:57:10.000000 intecomm-edc-0.2.8/intecomm_screening/admin/patient_call_inlines.py
--rw-r--r--   0 erikvw     (501) staff       (20)    12348 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/admin/patient_group_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3966 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_screening/admin/patient_group_rando_admin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.635978 intecomm-edc-0.2.8/intecomm_screening/admin/patient_log/
--rw-r--r--   0 erikvw     (501) staff       (20)       99 2023-08-29 02:39:08.000000 intecomm-edc-0.2.8/intecomm_screening/admin/patient_log/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6811 2023-08-29 21:57:21.000000 intecomm-edc-0.2.8/intecomm_screening/admin/patient_log/change_list_template_context.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2842 2023-08-31 03:37:01.000000 intecomm-edc-0.2.8/intecomm_screening/admin/patient_log/fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)      653 2023-08-29 02:39:08.000000 intecomm-edc-0.2.8/intecomm_screening/admin/patient_log/get_search_fields.py
--rw-r--r--   0 erikvw     (501) staff       (20)    13105 2024-01-29 02:23:02.000000 intecomm-edc-0.2.8/intecomm_screening/admin/patient_log/modeladmin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2405 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/admin/patient_log/patient_log_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2379 2024-01-29 04:38:11.000000 intecomm-edc-0.2.8/intecomm_screening/admin/patient_log/patient_log_ug_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1088 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_screening/admin/patient_log_report_print_history_admin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.637269 intecomm-edc-0.2.8/intecomm_screening/admin/subject_screening/
--rw-r--r--   0 erikvw     (501) staff       (20)      187 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/admin/subject_screening/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3342 2023-08-29 02:39:08.000000 intecomm-edc-0.2.8/intecomm_screening/admin/subject_screening/fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5084 2023-08-29 21:57:21.000000 intecomm-edc-0.2.8/intecomm_screening/admin/subject_screening/modeladmin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2122 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_screening/admin/subject_screening/subject_screening_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2503 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/admin/subject_screening/subject_screening_tz_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2558 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/admin/subject_screening/subject_screening_ug_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      843 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      553 2022-03-12 17:44:16.000000 intecomm-edc-0.2.8/intecomm_screening/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      549 2023-05-04 03:51:54.000000 intecomm-edc-0.2.8/intecomm_screening/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      402 2022-03-03 20:12:26.000000 intecomm-edc-0.2.8/intecomm_screening/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1885 2023-11-22 02:42:27.000000 intecomm-edc-0.2.8/intecomm_screening/baker_recipes.py
--rw-r--r--   0 erikvw     (501) staff       (20)      226 2023-05-04 03:51:54.000000 intecomm-edc-0.2.8/intecomm_screening/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)       33 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)       49 2023-07-02 21:12:50.000000 intecomm-edc-0.2.8/intecomm_screening/exceptions.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.638828 intecomm-edc-0.2.8/intecomm_screening/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      335 2023-08-29 21:57:21.000000 intecomm-edc-0.2.8/intecomm_screening/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2028 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/forms/consent_refusal_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      366 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_screening/forms/health_talk_log_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      356 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_screening/forms/patient_call_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3696 2023-08-08 02:36:10.000000 intecomm-edc-0.2.8/intecomm_screening/forms/patient_group_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      751 2023-07-05 03:07:33.000000 intecomm-edc-0.2.8/intecomm_screening/forms/patient_group_rando_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.639529 intecomm-edc-0.2.8/intecomm_screening/forms/patient_log/
--rw-r--r--   0 erikvw     (501) staff       (20)       95 2023-08-29 02:39:08.000000 intecomm-edc-0.2.8/intecomm_screening/forms/patient_log/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1631 2023-08-29 02:39:08.000000 intecomm-edc-0.2.8/intecomm_screening/forms/patient_log/patient_log_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      676 2023-08-29 02:39:08.000000 intecomm-edc-0.2.8/intecomm_screening/forms/patient_log/patient_log_ug_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.640441 intecomm-edc-0.2.8/intecomm_screening/forms/subject_screening/
--rw-r--r--   0 erikvw     (501) staff       (20)      119 2023-08-29 21:57:21.000000 intecomm-edc-0.2.8/intecomm_screening/forms/subject_screening/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8456 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/forms/subject_screening/modelform_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1699 2023-08-29 21:57:21.000000 intecomm-edc-0.2.8/intecomm_screening/forms/subject_screening/subject_screening_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1711 2023-08-29 21:57:21.000000 intecomm-edc-0.2.8/intecomm_screening/forms/subject_screening/subject_screening_ug_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2369 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/identifiers.py
--rw-r--r--   0 erikvw     (501) staff       (20)      944 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/intecomm_admin_site_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.529350 intecomm-edc-0.2.8/intecomm_screening/locale/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.529288 intecomm-edc-0.2.8/intecomm_screening/locale/lg/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.640659 intecomm-edc-0.2.8/intecomm_screening/locale/lg/LC_MESSAGES/
--rw-r--r--   0 erikvw     (501) staff       (20)     2075 2023-11-30 05:45:16.000000 intecomm-edc-0.2.8/intecomm_screening/locale/lg/LC_MESSAGES/django.po
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.529396 intecomm-edc-0.2.8/intecomm_screening/locale/sw/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.641167 intecomm-edc-0.2.8/intecomm_screening/locale/sw/LC_MESSAGES/
--rw-r--r--   0 erikvw     (501) staff       (20)      380 2023-08-24 22:02:31.000000 intecomm-edc-0.2.8/intecomm_screening/locale/sw/LC_MESSAGES/django.mo
--rw-r--r--   0 erikvw     (501) staff       (20)     2121 2023-08-24 22:02:29.000000 intecomm-edc-0.2.8/intecomm_screening/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.641440 intecomm-edc-0.2.8/intecomm_screening/management/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-18 02:36:12.000000 intecomm-edc-0.2.8/intecomm_screening/management/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.641637 intecomm-edc-0.2.8/intecomm_screening/management/commands/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-18 02:36:12.000000 intecomm-edc-0.2.8/intecomm_screening/management/commands/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3188 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_screening/management/commands/print_patient_log_reference.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.656998 intecomm-edc-0.2.8/intecomm_screening/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)   128990 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1281 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0002_remove_healthtalklog_unique_lower_name_report_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2757 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0003_site_remove_historicalpatientlog_patient_group_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1450 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0004_rename_name_historicalpatientlog_legal_name_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2033 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0005_historicalpatientcall_alt_contact_number_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3722 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0006_remove_historicalpatientcall_willing_to_attend_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2228 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0007_historicalpatientlog_last_4_contact_number_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7009 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0008_rename_last_routine_appt_date_historicalpatientlog_last_appt_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3258 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0009_historicalsubjectscreening_familiar_name_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      716 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0010_historicalpatientlog_age_in_years_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3939 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0011_rename_hf_identifier_historicalpatientlog_hospital_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1146 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0012_alter_historicalpatientcall_last_attend_clinic_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1892 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0013_alter_healthfacility_distance_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3541 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0014_alter_historicalpatientlog_familiar_name_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      560 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0015_remove_healthtalklog_unique_health_facility_report_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      974 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0016_historicalpatientlog_group_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      925 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0017_alter_historicalpatientlog_group_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1083 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0018_alter_historicalpatientlog_age_in_years_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2673 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0019_healthfacility_fri_healthfacility_mon_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    16562 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0020_consentrefusal_historicalconsentrefusal_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4414 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0021_idenfifierformat.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1032 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0022_historicalpatientlog_filing_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      891 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0023_auto_20230501_2208.py
--rw-r--r--   0 erikvw     (501) staff       (20)      835 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0024_auto_20230502_0249.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5013 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0025_patientlogreportprinthistory_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1062 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0026_alter_historicalpatientlog_filing_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      606 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0027_historicalpatientlog_printed_patientlog_printed.py
--rw-r--r--   0 erikvw     (501) staff       (20)      463 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0028_alter_patientlogreportprinthistory_patient_log_identifier.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2289 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0029_alter_historicalpatientlog_filing_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1213 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0030_auto_20230510_0352.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0031_alter_historicalpatientlog_next_appt_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1033 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0032_patientgrouprando.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1358 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0033_remove_consentrefusal_subject_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2119 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0034_alter_consentrefusal_screening_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      991 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0035_auto_20230630_0552.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1680 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0036_alter_historicalpatientlog_screening_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2369 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0037_alter_consentrefusal_screening_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1908 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0038_auto_20230701_0117.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1026 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0039_alter_historicalpatientlog_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1165 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0040_historicalsubjectscreening_patient_log_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      852 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0041_auto_20230702_1548.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4738 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0042_alter_healthfacility_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      968 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0043_auto_20230705_0529.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2521 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0044_alter_historicalpatientlog_site_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2518 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0045_alter_consentrefusal_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3334 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0046_alter_historicalpatientlog_legal_name_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1221 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0047_rename_historicalhealthfacility_historicaloldhealthfacility_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1220 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0048_rename_historicalhealthfacility_historicaloldhealthfacility_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      731 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0049_healthfacility.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1550 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0050_delete_healthfacility_healthtalklog_health_facility_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1421 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0051_auto_20230726_1631.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1301 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0052_auto_20230726_1634.py
--rw-r--r--   0 erikvw     (501) staff       (20)      967 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0053_rename_idenfifierformat_identifierformat_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      503 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0054_alter_healthtalklog_unique_together.py
--rw-r--r--   0 erikvw     (501) staff       (20)      332 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0055_delete_identifierformat.py
--rw-r--r--   0 erikvw     (501) staff       (20)      318 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0056_delete_healthfacility.py
--rw-r--r--   0 erikvw     (501) staff       (20)    16611 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0057_alter_consentrefusal_device_created_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      931 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0058_patientlogug.py
--rw-r--r--   0 erikvw     (501) staff       (20)    25711 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0059_subjectscreeningug_historicalsubjectscreeningug.py
--rw-r--r--   0 erikvw     (501) staff       (20)    18669 2023-08-29 02:39:08.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0060_historicalpatientlogug.py
--rw-r--r--   0 erikvw     (501) staff       (20)      809 2023-08-31 03:37:01.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0061_historicalpatientlog_comment_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1688 2023-08-31 03:37:01.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0062_auto_20230831_0032.py
--rw-r--r--   0 erikvw     (501) staff       (20)    15518 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0063_alter_consentrefusal_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2811 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0064_alter_patientcall_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1920 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0065_patientlogreportprinthistory_intecomm_sc_modifie_891a97_idx_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1095 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0066_alter_patientlogreportprinthistory_managers_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1132 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0067_auto_20231216_1807.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3480 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0068_alter_consentrefusal_site_alter_healthtalklog_site_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    26534 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/0069_subjectscreeningtz_historicalsubjectscreeningtz.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_screening/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.657413 intecomm-edc-0.2.8/intecomm_screening/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)       60 2022-11-23 01:31:30.000000 intecomm-edc-0.2.8/intecomm_screening/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2626 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_screening/model_mixins/patient_call_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.660291 intecomm-edc-0.2.8/intecomm_screening/models/
--rw-r--r--   0 erikvw     (501) staff       (20)     1072 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2392 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_screening/models/consent_refusal.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1829 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_screening/models/health_talk_log.py
--rw-r--r--   0 erikvw     (501) staff       (20)      752 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_screening/models/identifier_format.py
--rw-r--r--   0 erikvw     (501) staff       (20)      485 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_screening/models/location.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3009 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_screening/models/old_health_facility.py
--rw-r--r--   0 erikvw     (501) staff       (20)      958 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_screening/models/patient_call.py
--rw-r--r--   0 erikvw     (501) staff       (20)    10303 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/models/patient_log.py
--rw-r--r--   0 erikvw     (501) staff       (20)      560 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_screening/models/patient_log_report_print_history.py
--rw-r--r--   0 erikvw     (501) staff       (20)      206 2023-08-29 02:39:08.000000 intecomm-edc-0.2.8/intecomm_screening/models/patient_log_ug.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.661758 intecomm-edc-0.2.8/intecomm_screening/models/proxy_models/
--rw-r--r--   0 erikvw     (501) staff       (20)      114 2023-08-28 14:56:49.000000 intecomm-edc-0.2.8/intecomm_screening/models/proxy_models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      196 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_screening/models/proxy_models/health_facility.py
--rw-r--r--   0 erikvw     (501) staff       (20)      265 2023-01-25 03:04:55.000000 intecomm-edc-0.2.8/intecomm_screening/models/proxy_models/patient_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)      383 2023-05-12 04:56:33.000000 intecomm-edc-0.2.8/intecomm_screening/models/proxy_models/patient_group_rando.py
--rw-r--r--   0 erikvw     (501) staff       (20)      185 2022-11-23 01:31:30.000000 intecomm-edc-0.2.8/intecomm_screening/models/proxy_models/site.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5338 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/models/signals.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9789 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/models/subject_screening.py
--rw-r--r--   0 erikvw     (501) staff       (20)      333 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/models/subject_screening_tz.py
--rw-r--r--   0 erikvw     (501) staff       (20)      329 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/models/subject_screening_ug.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.662399 intecomm-edc-0.2.8/intecomm_screening/reports/
--rw-r--r--   0 erikvw     (501) staff       (20)       72 2023-05-05 04:31:31.000000 intecomm-edc-0.2.8/intecomm_screening/reports/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)    17443 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/reports/patient_log_report.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.530024 intecomm-edc-0.2.8/intecomm_screening/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.667915 intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.669836 intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      253 2023-07-02 21:12:50.000000 intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/admin/healthtalklog_change_list.html
--rw-r--r--   0 erikvw     (501) staff       (20)      253 2023-07-02 21:12:50.000000 intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/admin/patientcall_change_list.html
--rw-r--r--   0 erikvw     (501) staff       (20)      253 2023-07-02 21:12:50.000000 intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/admin/patientgroup_change_list.html
--rw-r--r--   0 erikvw     (501) staff       (20)      253 2023-08-28 14:26:40.000000 intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/admin/patientlog_change_list.html
--rw-r--r--   0 erikvw     (501) staff       (20)      253 2023-07-05 03:07:33.000000 intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/admin/subjectscreening_change_list.html
--rw-r--r--   0 erikvw     (501) staff       (20)      240 2022-11-29 06:19:20.000000 intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/change_list_appts.html
--rw-r--r--   0 erikvw     (501) staff       (20)      484 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/change_list_contacts.html
--rw-r--r--   0 erikvw     (501) staff       (20)       94 2022-11-29 06:19:20.000000 intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/change_list_dx.html
--rw-r--r--   0 erikvw     (501) staff       (20)       65 2023-05-04 03:51:54.000000 intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/change_list_filing_identifier.html
--rw-r--r--   0 erikvw     (501) staff       (20)      606 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/change_list_group.html
--rw-r--r--   0 erikvw     (501) staff       (20)       81 2022-11-29 06:19:20.000000 intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/change_list_hospital_identifier.html
--rw-r--r--   0 erikvw     (501) staff       (20)      727 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/change_list_patient_log_first_column.html
--rw-r--r--   0 erikvw     (501) staff       (20)     3044 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/change_list_screen_and_consent.html
--rw-r--r--   0 erikvw     (501) staff       (20)      462 2022-11-29 06:19:20.000000 intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/change_list_talks.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1387 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/group_management.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.670615 intecomm-edc-0.2.8/intecomm_screening/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_screening/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_screening/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)    16784 2024-02-06 04:30:17.000000 intecomm-edc-0.2.8/intecomm_screening/tests/intecomm_test_case_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.671908 intecomm-edc-0.2.8/intecomm_screening/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:30.000000 intecomm-edc-0.2.8/intecomm_screening/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7258 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_screening/tests/tests/test_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7483 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/tests/tests/test_consent_refusal.py
--rw-r--r--   0 erikvw     (501) staff       (20)    17317 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_screening/tests/tests/test_screening.py
--rw-r--r--   0 erikvw     (501) staff       (20)      579 2023-05-10 11:59:10.000000 intecomm-edc-0.2.8/intecomm_screening/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5863 2023-08-29 02:39:08.000000 intecomm-edc-0.2.8/intecomm_screening/utils.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1828 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_screening/views.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.673038 intecomm-edc-0.2.8/intecomm_sites/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_sites/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      287 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_sites/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      428 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_sites/intecomm_site.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.673274 intecomm-edc-0.2.8/intecomm_sites/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-03-12 18:03:07.000000 intecomm-edc-0.2.8/intecomm_sites/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)       46 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_sites/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5192 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_sites/sites.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.673539 intecomm-edc-0.2.8/intecomm_sites/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_sites/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      357 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_sites/tests/site_test_case_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.675904 intecomm-edc-0.2.8/intecomm_subject/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-11-22 15:10:26.000000 intecomm-edc-0.2.8/intecomm_subject/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      628 2023-11-16 04:10:04.000000 intecomm-edc-0.2.8/intecomm_subject/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.686151 intecomm-edc-0.2.8/intecomm_subject/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)     2506 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1818 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_subject/admin/appointment_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      299 2022-11-29 06:19:20.000000 intecomm-edc-0.2.8/intecomm_subject/admin/arv_regimens_admin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.687755 intecomm-edc-0.2.8/intecomm_subject/admin/blood_results/
--rw-r--r--   0 erikvw     (501) staff       (20)      414 2022-11-29 06:19:20.000000 intecomm-edc-0.2.8/intecomm_subject/admin/blood_results/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      723 2023-07-06 02:16:06.000000 intecomm-edc-0.2.8/intecomm_subject/admin/blood_results/blood_results_fbc_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      966 2023-07-06 02:16:02.000000 intecomm-edc-0.2.8/intecomm_subject/admin/blood_results/blood_results_glu_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      785 2023-07-06 02:16:13.000000 intecomm-edc-0.2.8/intecomm_subject/admin/blood_results/blood_results_hba1c_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      746 2023-07-06 02:16:20.000000 intecomm-edc-0.2.8/intecomm_subject/admin/blood_results/blood_results_ins_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      746 2023-07-06 02:16:26.000000 intecomm-edc-0.2.8/intecomm_subject/admin/blood_results/blood_results_lft_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      760 2023-07-06 02:16:33.000000 intecomm-edc-0.2.8/intecomm_subject/admin/blood_results/blood_results_lipid_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4598 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_subject/admin/blood_results/blood_results_rft_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      584 2022-11-29 06:19:20.000000 intecomm-edc-0.2.8/intecomm_subject/admin/cd4_result_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      759 2023-08-25 12:06:52.000000 intecomm-edc-0.2.8/intecomm_subject/admin/clinic_note_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1343 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/admin/clinical_review_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1257 2023-04-20 03:59:58.000000 intecomm-edc-0.2.8/intecomm_subject/admin/clinical_review_baseline_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1599 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/admin/complications_baseline_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1621 2023-07-05 03:07:33.000000 intecomm-edc-0.2.8/intecomm_subject/admin/complications_followup_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      754 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/admin/concomitant_medication_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1653 2023-04-25 03:09:42.000000 intecomm-edc-0.2.8/intecomm_subject/admin/dm_initial_review_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      434 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_subject/admin/dm_medication_adherence_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1149 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/admin/dm_review_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      796 2023-07-10 18:57:10.000000 intecomm-edc-0.2.8/intecomm_subject/admin/drug_refill_dm_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1779 2023-07-12 23:56:44.000000 intecomm-edc-0.2.8/intecomm_subject/admin/drug_refill_hiv_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1008 2023-07-10 18:57:10.000000 intecomm-edc-0.2.8/intecomm_subject/admin/drug_refill_htn_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      618 2023-05-24 22:37:50.000000 intecomm-edc-0.2.8/intecomm_subject/admin/eq5d3l_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1851 2024-02-06 04:30:17.000000 intecomm-edc-0.2.8/intecomm_subject/admin/family_history_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      349 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_subject/admin/fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1114 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/admin/glucose_admin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.689810 intecomm-edc-0.2.8/intecomm_subject/admin/health_economics/
--rw-r--r--   0 erikvw     (501) staff       (20)      388 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/admin/health_economics/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1819 2023-08-18 02:43:47.000000 intecomm-edc-0.2.8/intecomm_subject/admin/health_economics/assets_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4262 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/admin/health_economics/careseeking_a_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5282 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/admin/health_economics/careseeking_b_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1855 2023-08-10 17:37:32.000000 intecomm-edc-0.2.8/intecomm_subject/admin/health_economics/household_head_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      488 2023-07-05 03:07:33.000000 intecomm-edc-0.2.8/intecomm_subject/admin/health_economics/income_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1783 2023-08-04 04:50:38.000000 intecomm-edc-0.2.8/intecomm_subject/admin/health_economics/patient_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      502 2023-07-05 03:07:33.000000 intecomm-edc-0.2.8/intecomm_subject/admin/health_economics/property_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2574 2024-02-02 13:01:52.000000 intecomm-edc-0.2.8/intecomm_subject/admin/hiv_initial_review_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      439 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_subject/admin/hiv_medication_adherence_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2245 2024-02-02 13:02:06.000000 intecomm-edc-0.2.8/intecomm_subject/admin/hiv_review_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1460 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/admin/htn_initial_review_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      439 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_subject/admin/htn_medication_adherence_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      840 2023-07-11 03:12:55.000000 intecomm-edc-0.2.8/intecomm_subject/admin/htn_review_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      632 2023-05-24 22:37:50.000000 intecomm-edc-0.2.8/intecomm_subject/admin/icecapa_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2339 2024-02-02 02:23:27.000000 intecomm-edc-0.2.8/intecomm_subject/admin/list_filters.py
--rw-r--r--   0 erikvw     (501) staff       (20)      840 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_subject/admin/location_update_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      422 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/admin/malaria_test_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      960 2023-05-09 03:31:16.000000 intecomm-edc-0.2.8/intecomm_subject/admin/medications_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2513 2024-02-15 12:37:45.000000 intecomm-edc-0.2.8/intecomm_subject/admin/modeladmin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      914 2023-10-06 00:30:17.000000 intecomm-edc-0.2.8/intecomm_subject/admin/next_appointment_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2893 2023-07-18 02:36:12.000000 intecomm-edc-0.2.8/intecomm_subject/admin/other_baseline_data_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5263 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/admin/social_harms_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1788 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_subject/admin/subject_requisition_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1456 2023-07-10 18:57:10.000000 intecomm-edc-0.2.8/intecomm_subject/admin/subject_visit_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1232 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/admin/subject_visit_missed_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1074 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/admin/urine_dipstick_test_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      967 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/admin/urine_pregnancy_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2229 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/admin/vitals_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-03-12 18:18:07.000000 intecomm-edc-0.2.8/intecomm_subject/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      298 2022-03-12 18:18:07.000000 intecomm-edc-0.2.8/intecomm_subject/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1736 2023-08-10 17:37:32.000000 intecomm-edc-0.2.8/intecomm_subject/baker_recipes.py
--rw-r--r--   0 erikvw     (501) staff       (20)    12615 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      413 2024-02-15 12:37:45.000000 intecomm-edc-0.2.8/intecomm_subject/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1102 2023-11-30 05:45:33.000000 intecomm-edc-0.2.8/intecomm_subject/form_runners.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.702703 intecomm-edc-0.2.8/intecomm_subject/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)     2479 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2368 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_subject/forms/appointment_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.703989 intecomm-edc-0.2.8/intecomm_subject/forms/blood_results/
--rw-r--r--   0 erikvw     (501) staff       (20)      400 2022-11-29 06:19:20.000000 intecomm-edc-0.2.8/intecomm_subject/forms/blood_results/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      714 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/forms/blood_results/blood_results_fbc_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      823 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/forms/blood_results/blood_results_glu_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      765 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/forms/blood_results/blood_results_hba1c_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      722 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/forms/blood_results/blood_results_ins_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      714 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/forms/blood_results/blood_results_lft_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      730 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/forms/blood_results/blood_results_lipid_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1362 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/forms/blood_results/blood_results_rft_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      646 2022-11-29 06:19:20.000000 intecomm-edc-0.2.8/intecomm_subject/forms/cd4_result_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      630 2023-08-01 05:53:40.000000 intecomm-edc-0.2.8/intecomm_subject/forms/clinical_note_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      422 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/forms/clinical_review_baseline_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      422 2023-08-25 11:51:02.000000 intecomm-edc-0.2.8/intecomm_subject/forms/clinical_review_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      400 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/forms/complications_baseline_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      402 2023-07-05 03:07:33.000000 intecomm-edc-0.2.8/intecomm_subject/forms/complications_followup_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      489 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/forms/concomitant_medication_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      370 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/forms/dm_initial_review_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      910 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_subject/forms/dm_medication_adherence_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      335 2022-11-29 06:19:20.000000 intecomm-edc-0.2.8/intecomm_subject/forms/dm_review_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      355 2022-11-29 06:19:20.000000 intecomm-edc-0.2.8/intecomm_subject/forms/drug_refill_dm_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      360 2022-11-29 06:19:20.000000 intecomm-edc-0.2.8/intecomm_subject/forms/drug_refill_hiv_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      360 2022-11-29 06:19:20.000000 intecomm-edc-0.2.8/intecomm_subject/forms/drug_refill_htn_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      387 2022-11-29 06:19:20.000000 intecomm-edc-0.2.8/intecomm_subject/forms/drug_supply_dm_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      781 2022-11-29 06:19:20.000000 intecomm-edc-0.2.8/intecomm_subject/forms/drug_supply_hiv_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      393 2022-11-29 06:19:20.000000 intecomm-edc-0.2.8/intecomm_subject/forms/drug_supply_htn_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      545 2023-05-24 22:37:50.000000 intecomm-edc-0.2.8/intecomm_subject/forms/eq5d3l_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      394 2024-02-06 04:30:17.000000 intecomm-edc-0.2.8/intecomm_subject/forms/family_history_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.705933 intecomm-edc-0.2.8/intecomm_subject/forms/health_economics/
--rw-r--r--   0 erikvw     (501) staff       (20)      369 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/forms/health_economics/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      594 2023-08-10 17:37:32.000000 intecomm-edc-0.2.8/intecomm_subject/forms/health_economics/assets_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      531 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/forms/health_economics/careseeking_a_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      372 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/forms/health_economics/careseeking_b_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3141 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_subject/forms/health_economics/household_head.py
--rw-r--r--   0 erikvw     (501) staff       (20)      644 2023-08-10 17:37:32.000000 intecomm-edc-0.2.8/intecomm_subject/forms/health_economics/income_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      426 2023-08-16 02:41:30.000000 intecomm-edc-0.2.8/intecomm_subject/forms/health_economics/modelform_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      599 2023-08-10 17:37:32.000000 intecomm-edc-0.2.8/intecomm_subject/forms/health_economics/patient_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      604 2023-08-10 17:37:32.000000 intecomm-edc-0.2.8/intecomm_subject/forms/health_economics/property_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      403 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/forms/hiv_initial_review_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      927 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_subject/forms/hiv_medication_adherence_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2326 2024-02-01 16:00:54.000000 intecomm-edc-0.2.8/intecomm_subject/forms/hiv_review_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      386 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/forms/htn_initial_review_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      927 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_subject/forms/htn_medication_adherence_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      340 2024-02-01 14:33:25.000000 intecomm-edc-0.2.8/intecomm_subject/forms/htn_review_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      364 2023-05-24 22:37:50.000000 intecomm-edc-0.2.8/intecomm_subject/forms/icecapa_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      982 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_subject/forms/location_update_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      365 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/forms/malaria_test_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      350 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/forms/medications_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      268 2022-12-05 14:48:19.000000 intecomm-edc-0.2.8/intecomm_subject/forms/mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      783 2023-10-06 00:30:17.000000 intecomm-edc-0.2.8/intecomm_subject/forms/next_appointment_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      380 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/forms/other_baseline_data.py
--rw-r--r--   0 erikvw     (501) staff       (20)      350 2023-01-25 03:04:55.000000 intecomm-edc-0.2.8/intecomm_subject/forms/social_harms_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      953 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/forms/subject_requisition_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      791 2024-02-01 03:43:59.000000 intecomm-edc-0.2.8/intecomm_subject/forms/subject_visit_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2274 2023-08-13 00:11:46.000000 intecomm-edc-0.2.8/intecomm_subject/forms/subject_visit_missed_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      827 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/forms/urine_dipstick_test_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1267 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/forms/urine_pregnancy_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      342 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/forms/vitals_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.531124 intecomm-edc-0.2.8/intecomm_subject/locale/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.531062 intecomm-edc-0.2.8/intecomm_subject/locale/lg/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.706477 intecomm-edc-0.2.8/intecomm_subject/locale/lg/LC_MESSAGES/
--rw-r--r--   0 erikvw     (501) staff       (20)      337 2023-11-28 00:33:14.000000 intecomm-edc-0.2.8/intecomm_subject/locale/lg/LC_MESSAGES/django.mo
--rw-r--r--   0 erikvw     (501) staff       (20)     7140 2023-11-30 05:45:16.000000 intecomm-edc-0.2.8/intecomm_subject/locale/lg/LC_MESSAGES/django.po
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.531170 intecomm-edc-0.2.8/intecomm_subject/locale/sw/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.706984 intecomm-edc-0.2.8/intecomm_subject/locale/sw/LC_MESSAGES/
--rw-r--r--   0 erikvw     (501) staff       (20)      447 2023-11-28 00:30:12.000000 intecomm-edc-0.2.8/intecomm_subject/locale/sw/LC_MESSAGES/django.mo
--rw-r--r--   0 erikvw     (501) staff       (20)     7603 2023-11-30 05:45:16.000000 intecomm-edc-0.2.8/intecomm_subject/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.707181 intecomm-edc-0.2.8/intecomm_subject/management/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_subject/management/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.707664 intecomm-edc-0.2.8/intecomm_subject/management/commands/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_subject/management/commands/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8440 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_subject/management/commands/missed.py
--rw-r--r--   0 erikvw     (501) staff       (20)      797 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_subject/management/commands/seen_on_day.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.708510 intecomm-edc-0.2.8/intecomm_subject/metadata_rules/
--rw-r--r--   0 erikvw     (501) staff       (20)      154 2023-08-06 23:03:01.000000 intecomm-edc-0.2.8/intecomm_subject/metadata_rules/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5004 2024-02-15 12:37:45.000000 intecomm-edc-0.2.8/intecomm_subject/metadata_rules/metadata_rules.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1846 2024-02-19 22:04:54.000000 intecomm-edc-0.2.8/intecomm_subject/metadata_rules/predicates.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.744154 intecomm-edc-0.2.8/intecomm_subject/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)  1030442 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)    58037 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0002_remove_historicaldminitialreview_managed_by_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1791 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0003_alter_historicalsocialharms_coworkers_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    24955 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0004_historicalsocialharms_employment_impact_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    82105 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0005_alter_historicalsocialharms_coworkers_impact_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1089 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0006_alter_healtheconomics_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1497 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0007_alter_historicalotherbaselinedata_alcohol_consumption_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    23861 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0008_historicalvitals_vitals_remove_indicators_site_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3554 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0009_remove_historicalvitals_bp_measured_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3177 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0010_remove_historicalvitals_weight_is_estmated_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1500 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0011_remove_clinicalreviewbaseline_complications_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1178 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0012_alter_historicalvitals_heart_rate_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11537 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0013_alter_bloodresultsfbc_results_abnormal_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4242 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0014_alter_historicalotherbaselinedata_activity_combined_mn_avg_day_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    14317 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0015_alter_bloodresultsfbc_results_abnormal_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7271 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0016_remove_clinicalreview_reason_other_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11082 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0017_alter_bloodresultsfbc_results_abnormal_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7971 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0018_remove_historicalhivinitialreview_vl_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1259 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0019_remove_historicalhtninitialreview_med_start_date_estimated_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4308 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0020_remove_historicalhtninitialreview_managed_by_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1770 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0021_htninitialreview_managed_by_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1020 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0022_historicalhtninitialreview_managed_by_other_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1075 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0023_auto_20230404_0411.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1004 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0024_historicalhtninitialreview_med_start_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2655 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0025_rename_med_start_ago_dminitialreview_rx_init_ago_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2660 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0026_rename_dminitialreview_med_start_date_estimated_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    15922 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0027_dminitialreview_rx_init_dminitialreview_rx_init_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5727 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0028_remove_clinicalreviewbaseline_dm_test_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2215 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0029_remove_historicaldminitialreview_med_start_estimated_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    17272 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0030_nextappointment_historicalnextappointment_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2367 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0031_alter_clinicalreviewbaseline_dm_dx_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9087 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0032_historicalnextappointment_best_visit_code_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4995 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0033_clinicalreviewbaseline_dm_dx_at_screening_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4599 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0034_clinicalreviewbaseline_protocol_incident_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3126 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0035_alter_drugrefilldm_return_in_days_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2647 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0036_alter_dminitialreview_rx_init_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6697 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0037_alter_bloodresultsins_fasting_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      791 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0038_healtheconomics_welfare_other_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    46429 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0039_icecapa_historicalicecapa_historicaleq5d3l_eq5d3l_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2094 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0040_alter_historicalhivmedicationadherence_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)   190375 2023-10-11 13:30:21.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0041_health_economics_assets_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6343 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0042_alter_bloodresultsins_fasting_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0043_healtheconomicshouseholdhead_relationship_to_hoh_other_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11978 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0044_healtheconomicshouseholdhead_hoh_education_other_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1097 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0045_healtheconomicshouseholdhead_hoh_marital_status_other_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    20588 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0046_alter_healtheconomicsassets_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9292 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0047_healtheconomicsassets_cooking_fuel_other_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    29040 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0048_alter_healtheconomicsincome_external_remittance_currency_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    23015 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0049_alter_healtheconomicsincome_external_remittance_value_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11452 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0050_alter_healtheconomicshouseholdhead_hoh_ethnicity_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    35733 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0051_alter_bloodresultsfbc_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    13854 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0052_alter_bloodresultsfbc_managers_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4705 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0053_remove_historicalhivreview_arv_initiated_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      756 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0054_remove_historicalhtnreview_dia_blood_pressure_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1259 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0055_rename_drugrefilldm_return_in_days_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2826 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0056_alter_drugrefilldm_rx_days_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6291 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0057_rename_smoker_current_duration_historicalotherbaselinedata_smoker_duration_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1145 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0058_rename_external_remittance_currency_healtheconomicsincome_external_remit_currency_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3184 2023-10-05 22:47:02.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0059_historicalnextappointment_info_source_old_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1978 2023-10-05 22:47:14.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0060_historicalnextappointment_info_source_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1593 2023-10-05 22:47:43.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0061_auto_20230725_2035.py
--rw-r--r--   0 erikvw     (501) staff       (20)    15892 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0062_historicalclinicalnote_clinicalnote.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1121 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0063_auto_20230725_2058.py
--rw-r--r--   0 erikvw     (501) staff       (20)      852 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0064_historicalnextappointment_health_facility_old_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      780 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0065_historicalnextappointment_health_facility_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1158 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0066_historicalnextappointment_health_facility_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1229 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0067_auto_20230726_0008.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11874 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0068_remove_historicalhba1cresult_history_user_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5768 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0069_alter_healtheconomicshouseholdhead_hoh_employment_type_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      687 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0070_healtheconomicshouseholdhead_hoh_ethnicity_old_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3119 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0071_healtheconomicshouseholdhead_hoh_ethnicity_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1195 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0072_auto_20230803_0305.py
--rw-r--r--   0 erikvw     (501) staff       (20)      628 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0073_healtheconomicspatient_pat_ethnicity_new_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1679 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0074_healtheconomicspatient_pat_ethnicity_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      839 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0075_auto_20230803_0459.py
--rw-r--r--   0 erikvw     (501) staff       (20)      986 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0076_healtheconomicshouseholdhead_hoh_religion_old_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5006 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0077_healtheconomicshouseholdhead_hoh_religion_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1513 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0078_alter_healtheconomicshouseholdhead_hoh_religion_old_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1817 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0079_auto_20230803_0634.py
--rw-r--r--   0 erikvw     (501) staff       (20)      696 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0080_auto_20230803_1726.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1762 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0081_healtheconomicshouseholdhead_hoh_education_old_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3837 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0082_healtheconomicshouseholdhead_hoh_education_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2928 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0083_auto_20230803_1828.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3083 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0084_alter_healtheconomicsassets_external_wall_material_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2393 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0085_alter_healtheconomicsassets_external_wall_material_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1049 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0086_rename_hoh_employment_healtheconomicshouseholdhead_hoh_employment_status_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1073 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0087_alter_healtheconomicspatient_pat_citizen_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1089 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0088_healtheconomicspatient_pat_employment_type_other_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4414 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0089_alter_healtheconomicshouseholdhead_hoh_education_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    10743 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0090_alter_healtheconomicshouseholdhead_hoh_age_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    15119 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0091_healtheconomicsassets_solar_panels_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6326 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0092_healtheconomicsproperty_land_surface_area_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2245 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0093_alter_healtheconomicsproperty_land_value_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1252 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0094_alter_healtheconomicsproperty_land_surface_area_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3098 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0095_alter_healtheconomicsassets_bedrooms_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    12480 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0096_rename_external_remittance_healtheconomicsincome_external_remit_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11438 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0097_alter_healtheconomicsincome_external_remit_value_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5715 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0098_alter_healtheconomicshouseholdhead_hoh_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      520 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0099_remove_healtheconomicspatient_pat_citizen_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2831 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0100_alter_healtheconomicspatient_pat_education_old_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3223 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0101_alter_healtheconomicspatient_pat_education_old_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3397 2023-08-10 18:18:35.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0102_alter_healtheconomicshouseholdhead_hoh_education_old_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5029 2023-08-13 00:11:46.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0103_alter_healtheconomicshouseholdhead_hoh_employment_status_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    17949 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0104_historicallocationupdate_locationupdate.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9164 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0105_alter_historicallocationupdate_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2719 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0106_dmmedicationadherence_meds_shortage_reason_other_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    16542 2023-08-23 23:05:23.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0107_alter_bloodresultsfbc_device_created_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    18686 2023-08-23 23:05:23.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0108_alter_concomitantmedication_device_created_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    27488 2023-08-23 23:05:23.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0109_alter_healtheconomicsassets_device_created_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    30836 2023-08-23 23:05:23.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0110_alter_historicalbloodresultsfbc_device_created_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    29288 2023-08-23 23:05:23.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0111_alter_historicalhealtheconomics_device_created_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    36569 2023-08-23 23:05:23.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0112_alter_historicalhivinitialreview_device_created_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    18776 2023-08-23 23:05:23.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0113_alter_htnreview_device_created_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7314 2023-08-29 02:39:08.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0114_alter_dmmedicationadherence_visual_score_confirmed_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1767 2023-09-22 03:18:09.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0115_remove_historicalnextappointment_best_visit_code_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2860 2023-09-27 00:31:13.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0116_auto_20230920_0058.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1099 2023-10-05 13:55:11.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0117_historicalnextappointment_allow_create_interim_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1302 2023-10-06 00:30:17.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0118_historicalnextappointment_info_source_new_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1070 2023-10-06 00:30:17.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0119_auto_20231006_0220.py
--rw-r--r--   0 erikvw     (501) staff       (20)      721 2023-10-06 00:30:17.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0120_remove_historicalnextappointment_info_source_new_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      604 2023-10-06 00:30:17.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0121_auto_20231006_0238.py
--rw-r--r--   0 erikvw     (501) staff       (20)      485 2023-10-06 00:30:17.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0122_remove_historicalnextappointment_info_source_old_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      640 2023-11-16 04:10:04.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0123_alter_subjectvisit_managers.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3831 2023-11-16 04:10:04.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0124_auto_20231115_0133.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3919 2023-11-30 05:45:16.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0125_healtheconomicsproperty_calculated_land_surface_area_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2650 2023-11-30 05:45:16.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0126_feat_683_land_area_units.py
--rw-r--r--   0 erikvw     (501) staff       (20)      993 2023-11-30 05:45:33.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0127_alter_historicalsubjectvisitmissed_appt_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      762 2023-11-30 05:45:33.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0128_remove_historicalsubjectvisit_clinic_services_other_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    27740 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0129_alter_bloodresultsfbc_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2728 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0130_remove_bloodresultsfbc_intecomm_su_subject_1b56bc_idx_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4266 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0131_remove_drugrefillhtn_intecomm_su_subject_33642b_idx_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    73773 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0132_alter_subjectrequisition_unique_together_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7063 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0133_bloodresultsfbc_intecomm_su_subject_3bd165_idx_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    13741 2024-02-01 23:18:18.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0134_clinicalreviewbaseline_intecomm_su_subject_67b2fa_idx_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9514 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0135_hivinitialreview_intecomm_su_subject_a055c4_idx_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4258 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0136_subjectvisit_intecomm_su_modifie_dab86a_idx_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3418 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0137_alter_bloodresultsfbc_platelets_value_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    35161 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0138_alter_bloodresultsfbc_site_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2380 2024-02-01 03:43:59.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0139_alter_bloodresultsins_fasting_duration_minutes_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3869 2024-02-01 16:00:54.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0140_historicalhivreview_drawn_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      768 2024-02-01 16:00:54.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0141_remove_viralloadresult_requisition_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1460 2024-02-06 04:30:17.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0142_alter_historicalhtninitialreview_managed_by_old_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)   143208 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0143_historicalcareseekingb_historicalcareseekinga_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      603 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0144_rename_meds_prescribed_careseekingb_med_prescribed_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2687 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0145_rename_facility_visit_alt_careseekinga_missed_activities_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1013 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0146_rename_seek_inpatient_visits_careseekingb_inpatient_days_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1693 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/0147_alter_careseekinga_accompany_num_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-03-12 18:03:07.000000 intecomm-edc-0.2.8/intecomm_subject/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.745931 intecomm-edc-0.2.8/intecomm_subject/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      575 2024-02-01 16:00:54.000000 intecomm-edc-0.2.8/intecomm_subject/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4968 2023-08-04 04:50:38.000000 intecomm-edc-0.2.8/intecomm_subject/model_mixins/clinical_review_model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      358 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/model_mixins/crf_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      298 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_subject/model_mixins/crf_with_action_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      559 2023-04-18 01:59:08.000000 intecomm-edc-0.2.8/intecomm_subject/model_mixins/followup_review_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1326 2023-08-23 05:22:45.000000 intecomm-edc-0.2.8/intecomm_subject/model_mixins/medication_adherence_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      296 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_subject/model_mixins/search_slug_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1298 2024-02-01 16:00:54.000000 intecomm-edc-0.2.8/intecomm_subject/model_mixins/viral_load_result_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.754174 intecomm-edc-0.2.8/intecomm_subject/models/
--rw-r--r--   0 erikvw     (501) staff       (20)     2166 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      201 2023-12-04 21:40:22.000000 intecomm-edc-0.2.8/intecomm_subject/models/arv_regimens.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.755599 intecomm-edc-0.2.8/intecomm_subject/models/blood_results/
--rw-r--r--   0 erikvw     (501) staff       (20)      337 2022-11-29 06:19:20.000000 intecomm-edc-0.2.8/intecomm_subject/models/blood_results/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1382 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/blood_results/blood_results_fbc.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1170 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/blood_results/blood_results_glu.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1120 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/blood_results/blood_results_hba1c.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1136 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/blood_results/blood_results_ins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1319 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/blood_results/blood_results_lft.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1252 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/blood_results/blood_results_lipid.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1730 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/blood_results/blood_results_rft.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1143 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/cd4_result.py
--rw-r--r--   0 erikvw     (501) staff       (20)      727 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/clinical_note.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1065 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/clinical_review.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1133 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/clinical_review_baseline.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4427 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/complications_baseline.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2904 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/complications_followup.py
--rw-r--r--   0 erikvw     (501) staff       (20)      442 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/concomitant_medication.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1784 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/dm_initial_review.py
--rw-r--r--   0 erikvw     (501) staff       (20)      508 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/dm_medication_adherence.py
--rw-r--r--   0 erikvw     (501) staff       (20)      478 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/dm_review.py
--rw-r--r--   0 erikvw     (501) staff       (20)      653 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/drug_refill_dm.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1502 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/drug_refill_hiv.py
--rw-r--r--   0 erikvw     (501) staff       (20)      664 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/drug_refill_htn.py
--rw-r--r--   0 erikvw     (501) staff       (20)      558 2023-12-04 21:42:02.000000 intecomm-edc-0.2.8/intecomm_subject/models/drug_supply_dm.py
--rw-r--r--   0 erikvw     (501) staff       (20)      616 2023-12-04 21:42:09.000000 intecomm-edc-0.2.8/intecomm_subject/models/drug_supply_hiv.py
--rw-r--r--   0 erikvw     (501) staff       (20)      572 2023-12-04 21:42:12.000000 intecomm-edc-0.2.8/intecomm_subject/models/drug_supply_htn.py
--rw-r--r--   0 erikvw     (501) staff       (20)      480 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/eq5d3l.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3595 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/family_history.py
--rw-r--r--   0 erikvw     (501) staff       (20)      409 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/glucose.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.757372 intecomm-edc-0.2.8/intecomm_subject/models/health_economics/
--rw-r--r--   0 erikvw     (501) staff       (20)      311 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/models/health_economics/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      673 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/health_economics/assets.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11008 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/models/health_economics/careseeking_a.py
--rw-r--r--   0 erikvw     (501) staff       (20)    14482 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/models/health_economics/careseeking_b.py
--rw-r--r--   0 erikvw     (501) staff       (20)      854 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/models/health_economics/checklist.py
--rw-r--r--   0 erikvw     (501) staff       (20)      764 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/health_economics/household_head.py
--rw-r--r--   0 erikvw     (501) staff       (20)      611 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/health_economics/income.py
--rw-r--r--   0 erikvw     (501) staff       (20)      616 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/health_economics/patient.py
--rw-r--r--   0 erikvw     (501) staff       (20)      621 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/health_economics/property.py
--rw-r--r--   0 erikvw     (501) staff       (20)    18865 2023-07-10 18:57:10.000000 intecomm-edc-0.2.8/intecomm_subject/models/health_economics_old.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2490 2024-02-01 16:00:54.000000 intecomm-edc-0.2.8/intecomm_subject/models/hiv_initial_review.py
--rw-r--r--   0 erikvw     (501) staff       (20)      494 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/hiv_medication_adherence.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1162 2024-02-02 02:07:14.000000 intecomm-edc-0.2.8/intecomm_subject/models/hiv_review.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1512 2024-02-06 04:30:17.000000 intecomm-edc-0.2.8/intecomm_subject/models/htn_initial_review.py
--rw-r--r--   0 erikvw     (501) staff       (20)      521 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/htn_medication_adherence.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1301 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/htn_review.py
--rw-r--r--   0 erikvw     (501) staff       (20)      371 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/icecapa.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1391 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/location_update.py
--rw-r--r--   0 erikvw     (501) staff       (20)      463 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/malaria_test.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1567 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/medications.py
--rw-r--r--   0 erikvw     (501) staff       (20)      498 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/next_appointment.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5408 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/other_baseline_data.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2781 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/patient_history.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1602 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/reason_for_visit.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.757965 intecomm-edc-0.2.8/intecomm_subject/models/social_harms/
--rw-r--r--   0 erikvw     (501) staff       (20)       38 2023-01-25 03:04:55.000000 intecomm-edc-0.2.8/intecomm_subject/models/social_harms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3281 2023-01-25 03:04:55.000000 intecomm-edc-0.2.8/intecomm_subject/models/social_harms/model_factories.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1220 2023-01-25 03:04:55.000000 intecomm-edc-0.2.8/intecomm_subject/models/social_harms/social_harms.py
--rw-r--r--   0 erikvw     (501) staff       (20)      482 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/subject_requisition.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2345 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_subject/models/subject_visit.py
--rw-r--r--   0 erikvw     (501) staff       (20)      911 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/subject_visit_missed.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1283 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/urine_dipstick_test.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1290 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/urine_pregnancy.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2449 2023-12-05 05:08:32.000000 intecomm-edc-0.2.8/intecomm_subject/models/vitals.py
--rw-r--r--   0 erikvw     (501) staff       (20)      702 2023-11-13 01:27:15.000000 intecomm-edc-0.2.8/intecomm_subject/reference_model_configs.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.531833 intecomm-edc-0.2.8/intecomm_subject/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.758151 intecomm-edc-0.2.8/intecomm_subject/templates/intecomm_subject/
--rw-r--r--   0 erikvw     (501) staff       (20)      339 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_subject/templates/intecomm_subject/careseeking_a_instructions.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.758376 intecomm-edc-0.2.8/intecomm_subject/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_subject/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.532072 intecomm-edc-0.2.8/intecomm_subject/tests/etc/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.758477 intecomm-edc-0.2.8/intecomm_subject/tests/etc/community_only/
--rw-r--r--   0 erikvw     (501) staff       (20)      403 2023-11-19 17:30:45.000000 intecomm-edc-0.2.8/intecomm_subject/tests/etc/community_only/randomization_list.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.758703 intecomm-edc-0.2.8/intecomm_subject/tests/etc/facility_only/
--rw-r--r--   0 erikvw     (501) staff       (20)      382 2023-11-19 17:30:45.000000 intecomm-edc-0.2.8/intecomm_subject/tests/etc/facility_only/randomization_list.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.760164 intecomm-edc-0.2.8/intecomm_subject/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_subject/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2825 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/intecomm_subject/tests/tests/test_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9854 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_subject/tests/tests/test_appointment.py
--rw-r--r--   0 erikvw     (501) staff       (20)    17077 2024-02-19 23:54:03.000000 intecomm-edc-0.2.8/intecomm_subject/tests/tests/test_he.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4470 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/intecomm_subject/tests/tests/test_hiv_initial_and_review.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3887 2023-11-21 01:43:28.000000 intecomm-edc-0.2.8/intecomm_subject/tests/tests/test_location_update.py
--rw-r--r--   0 erikvw     (501) staff       (20)      210 2022-03-14 02:25:40.000000 intecomm-edc-0.2.8/intecomm_subject/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.761103 intecomm-edc-0.2.8/intecomm_visit_schedule/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-07-07 23:18:25.000000 intecomm-edc-0.2.8/intecomm_visit_schedule/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_visit_schedule/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      172 2022-03-12 18:22:09.000000 intecomm-edc-0.2.8/intecomm_visit_schedule/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      193 2023-08-11 03:07:19.000000 intecomm-edc-0.2.8/intecomm_visit_schedule/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.761195 intecomm-edc-0.2.8/intecomm_visit_schedule/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_visit_schedule/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.8/intecomm_visit_schedule/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.761384 intecomm-edc-0.2.8/intecomm_visit_schedule/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.8/intecomm_visit_schedule/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.761765 intecomm-edc-0.2.8/intecomm_visit_schedule/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:30.000000 intecomm-edc-0.2.8/intecomm_visit_schedule/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)       79 2023-08-11 02:54:06.000000 intecomm-edc-0.2.8/intecomm_visit_schedule/tests/tests/test_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)      113 2023-10-10 05:14:41.000000 intecomm-edc-0.2.8/intecomm_visit_schedule/tests/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:01:26.763304 intecomm-edc-0.2.8/intecomm_visit_schedule/visit_schedules/
--rw-r--r--   0 erikvw     (501) staff       (20)      234 2023-10-10 05:14:41.000000 intecomm-edc-0.2.8/intecomm_visit_schedule/visit_schedules/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      743 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_visit_schedule/visit_schedules/community_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7289 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_visit_schedule/visit_schedules/crfs.py
--rw-r--r--   0 erikvw     (501) staff       (20)      765 2024-01-25 06:13:02.000000 intecomm-edc-0.2.8/intecomm_visit_schedule/visit_schedules/facility_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1190 2024-02-01 16:00:54.000000 intecomm-edc-0.2.8/intecomm_visit_schedule/visit_schedules/requisitions.py
--rw-r--r--   0 erikvw     (501) staff       (20)      606 2023-10-10 05:14:41.000000 intecomm-edc-0.2.8/intecomm_visit_schedule/visit_schedules/visit_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3171 2024-02-26 13:01:14.000000 intecomm-edc-0.2.8/intecomm_visit_schedule/visit_schedules/visits.py
--rwxr-xr-x   0 erikvw     (501) staff       (20)      789 2021-11-22 15:06:01.000000 intecomm-edc-0.2.8/manage.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1960 2023-12-15 04:21:25.000000 intecomm-edc-0.2.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     8293 2024-01-29 06:51:01.000000 intecomm-edc-0.2.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1295 2024-02-26 13:01:26.764443 intecomm-edc-0.2.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.349170 intecomm-edc-0.2.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)      261 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-08-13 15:16:15.000000 intecomm-edc-0.2.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.117542 intecomm-edc-0.2.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.133484 intecomm-edc-0.2.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2315 2024-02-15 12:37:45.000000 intecomm-edc-0.2.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1486 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1227 2024-02-15 12:37:45.000000 intecomm-edc-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)      309 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)    10047 2023-12-05 05:12:56.000000 intecomm-edc-0.2.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-11-22 15:26:51.000000 intecomm-edc-0.2.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      225 2023-08-24 03:01:35.000000 intecomm-edc-0.2.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     3937 2024-02-26 13:27:16.349093 intecomm-edc-0.2.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     2898 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.118405 intecomm-edc-0.2.9/bin/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.133711 intecomm-edc-0.2.9/bin/nginx/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.134596 intecomm-edc-0.2.9/bin/nginx/conf/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1202 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/bin/nginx/conf/intecomm_live.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      432 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/bin/nginx/conf/intecomm_live_sites.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)     1282 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/bin/nginx/conf/intecomm_uat.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      435 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/bin/nginx/conf/intecomm_uat_sites.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      290 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/bin/nginx/intecomm.clinicedc.org.conf
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.117892 intecomm-edc-0.2.9/bin/nginx/www/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.118180 intecomm-edc-0.2.9/bin/nginx/www/html/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.134757 intecomm-edc-0.2.9/bin/nginx/www/html/live.intecomm.clinicedc.org/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1464 2022-11-23 01:31:30.000000 intecomm-edc-0.2.9/bin/nginx/www/html/live.intecomm.clinicedc.org/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.135026 intecomm-edc-0.2.9/bin/nginx/www/html/live.intecomm.clinicedc.org/tz/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2297 2023-01-25 03:04:55.000000 intecomm-edc-0.2.9/bin/nginx/www/html/live.intecomm.clinicedc.org/tz/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.135269 intecomm-edc-0.2.9/bin/nginx/www/html/live.intecomm.clinicedc.org/ug/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2281 2023-01-25 03:04:55.000000 intecomm-edc-0.2.9/bin/nginx/www/html/live.intecomm.clinicedc.org/ug/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.135477 intecomm-edc-0.2.9/bin/nginx/www/html/uat.intecomm.clinicedc.org/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1464 2022-11-23 01:31:30.000000 intecomm-edc-0.2.9/bin/nginx/www/html/uat.intecomm.clinicedc.org/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.135677 intecomm-edc-0.2.9/bin/nginx/www/html/uat.intecomm.clinicedc.org/tz/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2334 2023-01-25 03:04:55.000000 intecomm-edc-0.2.9/bin/nginx/www/html/uat.intecomm.clinicedc.org/tz/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.135843 intecomm-edc-0.2.9/bin/nginx/www/html/uat.intecomm.clinicedc.org/ug/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2318 2023-01-25 03:04:55.000000 intecomm-edc-0.2.9/bin/nginx/www/html/uat.intecomm.clinicedc.org/ug/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.136528 intecomm-edc-0.2.9/bin/systemd/
+-rwxr-xr-x   0 erikvw     (501) staff       (20)      435 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/bin/systemd/gunicorn-live.service
+-rwxr-xr-x   0 erikvw     (501) staff       (20)      133 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/bin/systemd/gunicorn-live.socket
+-rwxr-xr-x   0 erikvw     (501) staff       (20)      433 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/bin/systemd/gunicorn-uat.service
+-rwxr-xr-x   0 erikvw     (501) staff       (20)      131 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/bin/systemd/gunicorn-uat.socket
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/codecov.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     5118 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/env.sample
+-rw-r--r--   0 erikvw     (501) staff       (20)     1048 2021-08-13 15:16:15.000000 intecomm-edc-0.2.9/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.138458 intecomm-edc-0.2.9/intecomm_ae/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_ae/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6126 2023-09-22 03:18:08.000000 intecomm-edc-0.2.9/intecomm_ae/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.139502 intecomm-edc-0.2.9/intecomm_ae/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      197 2023-08-16 02:41:30.000000 intecomm-edc-0.2.9/intecomm_ae/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      707 2023-09-27 00:31:13.000000 intecomm-edc-0.2.9/intecomm_ae/admin/ae_followup_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1826 2023-09-27 00:31:13.000000 intecomm-edc-0.2.9/intecomm_ae/admin/ae_initial_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2784 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_ae/admin/death_report_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      748 2023-09-27 00:31:13.000000 intecomm-edc-0.2.9/intecomm_ae/admin/hospitalization_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      167 2022-10-18 02:23:36.000000 intecomm-edc-0.2.9/intecomm_ae/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      293 2023-11-30 05:45:16.000000 intecomm-edc-0.2.9/intecomm_ae/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1015 2023-08-16 02:41:30.000000 intecomm-edc-0.2.9/intecomm_ae/baker_recipes.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      756 2022-04-11 18:27:09.000000 intecomm-edc-0.2.9/intecomm_ae/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       36 2022-04-11 18:27:09.000000 intecomm-edc-0.2.9/intecomm_ae/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.140771 intecomm-edc-0.2.9/intecomm_ae/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      189 2023-08-16 02:41:30.000000 intecomm-edc-0.2.9/intecomm_ae/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      298 2023-08-14 13:42:28.000000 intecomm-edc-0.2.9/intecomm_ae/forms/ae_followup_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      791 2023-08-16 02:41:30.000000 intecomm-edc-0.2.9/intecomm_ae/forms/ae_initial_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1424 2023-08-14 13:42:28.000000 intecomm-edc-0.2.9/intecomm_ae/forms/death_report_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      365 2023-08-16 02:41:30.000000 intecomm-edc-0.2.9/intecomm_ae/forms/hospitalization_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      874 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_ae/forms/modelform_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1248 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_ae/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.144841 intecomm-edc-0.2.9/intecomm_ae/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)   144620 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_ae/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5271 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_ae/migrations/0002_rename_narrative_aetmg_investigator_narrative_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1663 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_ae/migrations/0003_alter_deathreporttmg_cause_of_death_agreed_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2820 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_ae/migrations/0004_alter_aefollowup_options_alter_aeinitial_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2355 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_ae/migrations/0005_alter_aefollowup_managers_alter_aeinitial_managers_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    21815 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_ae/migrations/0006_hospitalization_historicalhospitalization.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2892 2023-08-16 02:41:30.000000 intecomm-edc-0.2.9/intecomm_ae/migrations/0007_aeinitial_ae_classification_as_text_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5140 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_ae/migrations/0008_alter_deathreporttmgsecond_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    20568 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_ae/migrations/0009_alter_aefollowup_device_created_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2068 2023-11-16 04:10:04.000000 intecomm-edc-0.2.9/intecomm_ae/migrations/0010_alter_deathreport_death_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    15388 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_ae/migrations/0011_alter_aefollowup_options_alter_aeinitial_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3328 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_ae/migrations/0012_aefollowup_intecomm_ae_subject_a0869e_idx_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4003 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_ae/migrations/0013_aetmg_intecomm_ae_subject_a182a3_idx_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5642 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_ae/migrations/0014_alter_aefollowup_site_alter_aeinitial_site_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_ae/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.145167 intecomm-edc-0.2.9/intecomm_ae/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)       54 2023-08-16 02:41:30.000000 intecomm-edc-0.2.9/intecomm_ae/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2666 2023-08-16 02:41:30.000000 intecomm-edc-0.2.9/intecomm_ae/model_mixins/ae_review_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.146727 intecomm-edc-0.2.9/intecomm_ae/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      211 2023-08-16 02:41:30.000000 intecomm-edc-0.2.9/intecomm_ae/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      406 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_ae/models/ae_followup.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1900 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_ae/models/ae_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      948 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_ae/models/compatability.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1817 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_ae/models/death_report.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      802 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_ae/models/hospitalization.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      620 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_ae/models/managers.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.147359 intecomm-edc-0.2.9/intecomm_ae/pdf_reports/
+-rw-r--r--   0 erikvw     (501) staff       (20)       84 2023-08-16 02:41:30.000000 intecomm-edc-0.2.9/intecomm_ae/pdf_reports/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1365 2023-08-16 02:41:30.000000 intecomm-edc-0.2.9/intecomm_ae/pdf_reports/ae_pdf_report.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1135 2023-08-16 02:41:30.000000 intecomm-edc-0.2.9/intecomm_ae/pdf_reports/death_pdf_report.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.119044 intecomm-edc-0.2.9/intecomm_ae/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.119098 intecomm-edc-0.2.9/intecomm_ae/templates/intecomm_ae/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.147531 intecomm-edc-0.2.9/intecomm_ae/templates/intecomm_ae/bootstrap3/
+-rw-r--r--   0 erikvw     (501) staff       (20)      889 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_ae/templates/intecomm_ae/bootstrap3/ae_initial_description.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.147867 intecomm-edc-0.2.9/intecomm_ae/templatetags/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_ae/templatetags/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1215 2023-08-16 02:41:30.000000 intecomm-edc-0.2.9/intecomm_ae/templatetags/protocol_ae_extras.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.148362 intecomm-edc-0.2.9/intecomm_ae/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_ae/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_ae/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.148607 intecomm-edc-0.2.9/intecomm_ae/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 intecomm-edc-0.2.9/intecomm_ae/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      259 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_ae/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      205 2022-10-18 02:24:15.000000 intecomm-edc-0.2.9/intecomm_ae/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.149469 intecomm-edc-0.2.9/intecomm_auth/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_auth/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      233 2022-03-12 18:30:44.000000 intecomm-edc-0.2.9/intecomm_auth/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1166 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_auth/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2325 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_auth/auths.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.149697 intecomm-edc-0.2.9/intecomm_auth/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_auth/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.149878 intecomm-edc-0.2.9/intecomm_auth/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_auth/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      819 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_auth/tests/tests/test_auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_auth/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.151393 intecomm-edc-0.2.9/intecomm_consent/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_consent/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.152646 intecomm-edc-0.2.9/intecomm_consent/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      182 2024-02-01 03:43:59.000000 intecomm-edc-0.2.9/intecomm_consent/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1179 2023-08-29 02:39:08.000000 intecomm-edc-0.2.9/intecomm_consent/admin/fieldsets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3075 2024-02-01 06:39:00.000000 intecomm-edc-0.2.9/intecomm_consent/admin/modeladmin_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1688 2024-02-01 03:43:59.000000 intecomm-edc-0.2.9/intecomm_consent/admin/subject_consent_tz_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1867 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_consent/admin/subject_consent_ug_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      754 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_consent/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-03-12 18:10:23.000000 intecomm-edc-0.2.9/intecomm_consent/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1104 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_consent/baker_recipes.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      826 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_consent/consents.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.153401 intecomm-edc-0.2.9/intecomm_consent/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      176 2024-02-01 03:43:59.000000 intecomm-edc-0.2.9/intecomm_consent/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2255 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_consent/forms/modelform_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      295 2024-02-01 03:43:59.000000 intecomm-edc-0.2.9/intecomm_consent/forms/subject_consent_tz_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      295 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_consent/forms/subject_consent_ug_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.153604 intecomm-edc-0.2.9/intecomm_consent/management/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-03-03 20:12:26.000000 intecomm-edc-0.2.9/intecomm_consent/management/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.153788 intecomm-edc-0.2.9/intecomm_consent/management/commands/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-03-03 20:12:26.000000 intecomm-edc-0.2.9/intecomm_consent/management/commands/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_consent/management/commands/create_missing_prescriptions.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.159199 intecomm-edc-0.2.9/intecomm_consent/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    69089 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5396 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0002_remove_subjectconsent_intecomm_co_subject_145905_idx_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1535 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0003_alter_historicalsubjectconsent_language_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1951 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0004_alter_historicalsubjectconsent_familiar_name_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1016 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0005_remove_subjectconsent_unique_consent_subject_id_and_version_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      696 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0006_historicalsubjectconsent_group_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1575 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0007_alter_historicalsubjectconsent_language_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1055 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0008_alter_historicalsubjectconsent_screening_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      922 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0009_alter_subjectconsent_options.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      667 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0010_alter_subjectreconsent_options.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2234 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0011_alter_subjectconsent_unique_together_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5369 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0012_alter_historicalsubjectconsent_device_created_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      859 2023-08-29 02:39:08.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0013_subjectconsentug.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      482 2023-08-29 02:39:08.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0014_alter_subjectconsentug_options.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    24440 2023-08-29 02:39:08.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0015_historicalsubjectconsentug.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2353 2023-09-22 03:18:08.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0016_alter_historicalsubjectconsent_language_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5014 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0017_alter_subjectconsent_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1700 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0018_subjectconsent_intecomm_co_modifie_45691e_idx_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1566 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0019_historicalsubjectconsent_model_name_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      664 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0020_auto_20240111_0115.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2072 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0021_remove_subjectreconsent_action_item_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    26393 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0022_subjectconsenttz_historicalsubjectconsenttz.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      640 2024-02-01 16:00:54.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/0023_alter_subjectconsent_managers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_consent/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.160383 intecomm-edc-0.2.9/intecomm_consent/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      361 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_consent/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      296 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_consent/models/model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3199 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_consent/models/signals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4688 2024-02-06 04:30:17.000000 intecomm-edc-0.2.9/intecomm_consent/models/subject_consent.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_consent/models/subject_consent_tz.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      252 2024-01-28 23:23:52.000000 intecomm-edc-0.2.9/intecomm_consent/models/subject_consent_ug.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.120203 intecomm-edc-0.2.9/intecomm_consent/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.120253 intecomm-edc-0.2.9/intecomm_consent/templates/intecomm_consent/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.160761 intecomm-edc-0.2.9/intecomm_consent/templates/intecomm_consent/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1829 2024-02-01 06:39:00.000000 intecomm-edc-0.2.9/intecomm_consent/templates/intecomm_consent/admin/subjectconsent_change_list.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.161315 intecomm-edc-0.2.9/intecomm_consent/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_consent/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_consent/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.162113 intecomm-edc-0.2.9/intecomm_consent/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 intecomm-edc-0.2.9/intecomm_consent/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8866 2024-02-01 03:43:59.000000 intecomm-edc-0.2.9/intecomm_consent/tests/tests/test_subject_consent.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3051 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_consent/tests/tests/test_webtest.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      920 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_consent/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      210 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_consent/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1810 2023-08-29 02:39:08.000000 intecomm-edc-0.2.9/intecomm_consent/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.163022 intecomm-edc-0.2.9/intecomm_dashboard/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_dashboard/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      248 2023-07-02 21:12:50.000000 intecomm-edc-0.2.9/intecomm_dashboard/apps.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.163325 intecomm-edc-0.2.9/intecomm_dashboard/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_dashboard/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1163 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_dashboard/navbars.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       47 2022-06-24 09:14:59.000000 intecomm-edc-0.2.9/intecomm_dashboard/patterns.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.120640 intecomm-edc-0.2.9/intecomm_dashboard/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.120700 intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.163432 intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.165312 intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/
+-rw-r--r--   0 erikvw     (501) staff       (20)      466 2022-11-23 01:31:30.000000 intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/add_consent_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      239 2024-01-27 22:17:38.000000 intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/dashboard_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      401 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/eligibility_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      429 2022-11-23 01:31:30.000000 intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/patient_group_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      365 2022-11-23 01:31:30.000000 intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/patient_log_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      437 2023-05-04 03:51:54.000000 intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/refusal_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      341 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/buttons/screening_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1739 2023-08-29 02:39:08.000000 intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/changelist_topbar.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.165584 intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/screening/
+-rw-r--r--   0 erikvw     (501) staff       (20)     3973 2023-08-29 02:39:08.000000 intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/screening/listboard.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.166350 intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/
+-rw-r--r--   0 erikvw     (501) staff       (20)      893 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/buttons_column.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.166572 intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/dashboard/
+-rw-r--r--   0 erikvw     (501) staff       (20)      231 2023-05-11 02:01:11.000000 intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/dashboard/top_bar.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1035 2024-02-08 12:55:55.000000 intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/dashboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     2876 2024-02-08 12:55:55.000000 intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/subject_listboard.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.167107 intecomm-edc-0.2.9/intecomm_dashboard/templatetags/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_dashboard/templatetags/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6828 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_dashboard/templatetags/protocol_dashboard_extras.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.167983 intecomm-edc-0.2.9/intecomm_dashboard/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_dashboard/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      720 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_dashboard/tests/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_dashboard/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.168262 intecomm-edc-0.2.9/intecomm_dashboard/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_dashboard/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2399 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_dashboard/tests/tests/test_views.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2828 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_dashboard/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1204 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_dashboard/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.168487 intecomm-edc-0.2.9/intecomm_dashboard/views/
+-rw-r--r--   0 erikvw     (501) staff       (20)      187 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_dashboard/views/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.169241 intecomm-edc-0.2.9/intecomm_dashboard/views/ae/
+-rw-r--r--   0 erikvw     (501) staff       (20)      113 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_dashboard/views/ae/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      119 2023-08-16 02:41:30.000000 intecomm-edc-0.2.9/intecomm_dashboard/views/ae/ae_listboard_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      146 2023-08-16 02:41:30.000000 intecomm-edc-0.2.9/intecomm_dashboard/views/ae/death_report_listboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.169670 intecomm-edc-0.2.9/intecomm_dashboard/views/screening/
+-rw-r--r--   0 erikvw     (501) staff       (20)       42 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_dashboard/views/screening/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2541 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_dashboard/views/screening/listboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.170239 intecomm-edc-0.2.9/intecomm_dashboard/views/subject/
+-rw-r--r--   0 erikvw     (501) staff       (20)      114 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_dashboard/views/subject/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3413 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_dashboard/views/subject/subject_dashboard_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4059 2024-02-01 16:00:54.000000 intecomm-edc-0.2.9/intecomm_dashboard/views/subject/subject_listboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.172100 intecomm-edc-0.2.9/intecomm_edc/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_edc/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      927 2022-07-07 11:06:18.000000 intecomm-edc-0.2.9/intecomm_edc/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      382 2024-01-25 17:45:05.000000 intecomm-edc-0.2.9/intecomm_edc/apps.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.173069 intecomm-edc-0.2.9/intecomm_edc/management/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-02-01 03:43:59.000000 intecomm-edc-0.2.9/intecomm_edc/management/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.173272 intecomm-edc-0.2.9/intecomm_edc/management/commands/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-02-01 03:43:59.000000 intecomm-edc-0.2.9/intecomm_edc/management/commands/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1130 2024-02-01 03:43:59.000000 intecomm-edc-0.2.9/intecomm_edc/management/commands/update_forms_reference.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       46 2020-03-04 23:21:43.000000 intecomm-edc-0.2.9/intecomm_edc/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1255 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_edc/navbars.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.175222 intecomm-edc-0.2.9/intecomm_edc/settings/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-03 04:33:09.000000 intecomm-edc-0.2.9/intecomm_edc/settings/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1408 2024-02-19 22:04:54.000000 intecomm-edc-0.2.9/intecomm_edc/settings/debug.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    19135 2024-02-15 12:37:45.000000 intecomm-edc-0.2.9/intecomm_edc/settings/defaults.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1065 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_edc/settings/live.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1936 2023-11-21 13:15:18.000000 intecomm-edc-0.2.9/intecomm_edc/settings/logging.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      596 2024-02-06 04:30:17.000000 intecomm-edc-0.2.9/intecomm_edc/settings/minimal.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1302 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_edc/settings/uat.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.122131 intecomm-edc-0.2.9/intecomm_edc/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.122183 intecomm-edc-0.2.9/intecomm_edc/templates/intecomm_edc/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.176219 intecomm-edc-0.2.9/intecomm_edc/templates/intecomm_edc/bootstrap3/
+-rw-r--r--   0 erikvw     (501) staff       (20)      165 2021-08-09 19:25:29.000000 intecomm-edc-0.2.9/intecomm_edc/templates/intecomm_edc/bootstrap3/base.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     2480 2023-09-22 03:18:09.000000 intecomm-edc-0.2.9/intecomm_edc/templates/intecomm_edc/bootstrap3/followup_community.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     2159 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_edc/templates/intecomm_edc/bootstrap3/grouping.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     2330 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_edc/templates/intecomm_edc/bootstrap3/home.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     2466 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_edc/templates/intecomm_edc/bootstrap3/subjects_home.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.176417 intecomm-edc-0.2.9/intecomm_edc/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:21:43.000000 intecomm-edc-0.2.9/intecomm_edc/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.178327 intecomm-edc-0.2.9/intecomm_edc/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      687 2023-02-02 02:49:25.000000 intecomm-edc-0.2.9/intecomm_edc/tests/etc/randomization_list.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-02-02 02:49:25.000000 intecomm-edc-0.2.9/intecomm_edc/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-02-02 02:49:25.000000 intecomm-edc-0.2.9/intecomm_edc/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2023-02-02 02:49:25.000000 intecomm-edc-0.2.9/intecomm_edc/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2023-02-02 02:49:25.000000 intecomm-edc-0.2.9/intecomm_edc/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2023-02-02 02:49:25.000000 intecomm-edc-0.2.9/intecomm_edc/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2023-02-02 02:49:25.000000 intecomm-edc-0.2.9/intecomm_edc/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-02-02 02:49:25.000000 intecomm-edc-0.2.9/intecomm_edc/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-02-02 02:49:25.000000 intecomm-edc-0.2.9/intecomm_edc/tests/etc/user-salt-restricted.key
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.178545 intecomm-edc-0.2.9/intecomm_edc/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 intecomm-edc-0.2.9/intecomm_edc/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_edc/tests/tests/test_endpoints.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3703 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_edc/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.179238 intecomm-edc-0.2.9/intecomm_edc/views/
+-rw-r--r--   0 erikvw     (501) staff       (20)      121 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_edc/views/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      398 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_edc/views/grouping_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      382 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_edc/views/home_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      626 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_edc/views/subjects_home_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      179 2022-03-12 18:45:28.000000 intecomm-edc-0.2.9/intecomm_edc/wsgi.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      178 2022-03-12 18:45:28.000000 intecomm-edc-0.2.9/intecomm_edc/wsgi_live.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-03-12 18:45:28.000000 intecomm-edc-0.2.9/intecomm_edc/wsgi_uat.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.348725 intecomm-edc-0.2.9/intecomm_edc.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     3937 2024-02-26 13:27:15.000000 intecomm-edc-0.2.9/intecomm_edc.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)    54774 2024-02-26 13:27:16.000000 intecomm-edc-0.2.9/intecomm_edc.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-02-26 13:27:15.000000 intecomm-edc-0.2.9/intecomm_edc.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-07-19 12:31:42.000000 intecomm-edc-0.2.9/intecomm_edc.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)      127 2024-02-26 13:27:15.000000 intecomm-edc-0.2.9/intecomm_edc.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      241 2024-02-26 13:27:15.000000 intecomm-edc-0.2.9/intecomm_edc.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.180206 intecomm-edc-0.2.9/intecomm_export/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_export/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_export/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      175 2022-03-12 18:43:23.000000 intecomm-edc-0.2.9/intecomm_export/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      161 2022-03-12 18:43:17.000000 intecomm-edc-0.2.9/intecomm_export/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_export/tests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      213 2022-03-12 18:43:14.000000 intecomm-edc-0.2.9/intecomm_export/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_export/views.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.181731 intecomm-edc-0.2.9/intecomm_facility/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_facility/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2139 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_facility/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      185 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_facility/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      295 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_facility/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      370 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_facility/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      421 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_facility/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.183110 intecomm-edc-0.2.9/intecomm_facility/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    16078 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_facility/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2958 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_facility/migrations/0002_alter_healthfacility_device_created_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2128 2023-11-16 04:10:04.000000 intecomm-edc-0.2.9/intecomm_facility/migrations/0003_auto_20230726_2030.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2663 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_facility/migrations/0004_alter_healthfacility_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1047 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_facility/migrations/0005_alter_healthfacility_site_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_facility/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      785 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_facility/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.122783 intecomm-edc-0.2.9/intecomm_facility/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.122829 intecomm-edc-0.2.9/intecomm_facility/templates/intecomm_facility/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.183207 intecomm-edc-0.2.9/intecomm_facility/templates/intecomm_facility/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      253 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_facility/templates/intecomm_facility/admin/healthfacility_changelist.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      211 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_facility/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.185274 intecomm-edc-0.2.9/intecomm_group/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_group/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.186865 intecomm-edc-0.2.9/intecomm_group/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      327 2023-05-10 11:59:10.000000 intecomm-edc-0.2.9/intecomm_group/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2781 2023-07-10 18:57:10.000000 intecomm-edc-0.2.9/intecomm_group/admin/community_care_location_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      486 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_group/admin/list_filters.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7213 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_group/admin/patient_followup_call_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5090 2024-02-06 04:30:17.000000 intecomm-edc-0.2.9/intecomm_group/admin/patient_group_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1555 2023-07-10 18:57:10.000000 intecomm-edc-0.2.9/intecomm_group/admin/patient_group_appointment_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2104 2023-07-10 18:57:10.000000 intecomm-edc-0.2.9/intecomm_group/admin/patient_group_meeting_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_group/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      293 2023-11-30 05:45:16.000000 intecomm-edc-0.2.9/intecomm_group/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      509 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_group/baker_recipes.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      800 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_group/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2023-02-28 00:36:08.000000 intecomm-edc-0.2.9/intecomm_group/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      100 2022-11-23 01:31:30.000000 intecomm-edc-0.2.9/intecomm_group/exceptions.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.188244 intecomm-edc-0.2.9/intecomm_group/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      317 2023-07-20 02:48:14.000000 intecomm-edc-0.2.9/intecomm_group/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      366 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_group/forms/community_care_location_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      380 2023-07-20 02:48:14.000000 intecomm-edc-0.2.9/intecomm_group/forms/patient_followup_call_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      372 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_group/forms/patient_group_appointment_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      495 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_group/forms/patient_group_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      360 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_group/forms/patient_group_meeting_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.192878 intecomm-edc-0.2.9/intecomm_group/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    29538 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_group/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3393 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_group/migrations/0002_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      598 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_group/migrations/0003_alter_historicalpatientgroup_group_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      665 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_group/migrations/0004_alter_patientgroup_patients.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    17784 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_group/migrations/0005_patientfollowupcall_historicalpatientfollowupcall.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2952 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_group/migrations/0006_remove_historicalpatientgroup_enforce_group_size_min_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3530 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_group/migrations/0007_remove_historicalpatientfollowupcall_attend_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2554 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_group/migrations/0008_patientgroup_dm_patients_patientgroup_hiv_patients_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1517 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_group/migrations/0009_auto_20221126_0358.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      575 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_group/migrations/0010_alter_patientgroup_managers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1242 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_group/migrations/0011_alter_historicalpatientfollowupcall_respondent_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1532 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_group/migrations/0012_alter_historicalpatientgroup_status_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1517 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_group/migrations/0013_alter_historicalpatientgroup_status_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4350 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_group/migrations/0014_alter_communitycarelocation_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2126 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_group/migrations/0015_alter_patientgroupmeeting_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9152 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_group/migrations/0016_alter_communitycarelocation_device_created_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    11048 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_group/migrations/0017_alter_communitycarelocation_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2731 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_group/migrations/0018_alter_communitycarelocation_site_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_group/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.194467 intecomm-edc-0.2.9/intecomm_group/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      512 2023-05-04 03:51:54.000000 intecomm-edc-0.2.9/intecomm_group/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2283 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_group/models/community_care_location.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      747 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_group/models/patient_followup_call.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4043 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_group/models/patient_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1062 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_group/models/patient_group_appointment.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1311 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_group/models/patient_group_meeting.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3710 2023-05-24 17:50:54.000000 intecomm-edc-0.2.9/intecomm_group/models/signals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1946 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_group/models/utils.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6270 2023-11-21 01:43:28.000000 intecomm-edc-0.2.9/intecomm_group/patient_group_updater.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.123262 intecomm-edc-0.2.9/intecomm_group/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.194887 intecomm-edc-0.2.9/intecomm_group/templates/intecomm_group/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.195946 intecomm-edc-0.2.9/intecomm_group/templates/intecomm_group/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1310 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_group/templates/intecomm_group/admin/communitycarelocation_change_list.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1513 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_group/templates/intecomm_group/admin/patientfollowupcall_change_list.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1349 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_group/templates/intecomm_group/admin/patientgroup_change_list.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1470 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_group/templates/intecomm_group/admin/patientgroupappointment_change_list.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1452 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_group/templates/intecomm_group/admin/patientgroupmeeting_change_list.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      101 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_group/templates/intecomm_group/patient_followup_call_locator.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      631 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_group/templates/intecomm_group/patient_followup_call_summary.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.196173 intecomm-edc-0.2.9/intecomm_group/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_group/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      524 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_group/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.196463 intecomm-edc-0.2.9/intecomm_group/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_group/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6053 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_group/tests/tests/test_add_subjects_after_rando.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      207 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_group/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4396 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_group/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.198063 intecomm-edc-0.2.9/intecomm_labs/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-07-02 03:53:00.000000 intecomm-edc-0.2.9/intecomm_labs/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       87 2021-07-05 19:24:26.000000 intecomm-edc-0.2.9/intecomm_labs/aliquot_types.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      209 2022-03-12 18:19:55.000000 intecomm-edc-0.2.9/intecomm_labs/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1011 2022-11-29 06:19:20.000000 intecomm-edc-0.2.9/intecomm_labs/lab_profiles.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      128 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_labs/labs.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      481 2022-03-12 18:19:03.000000 intecomm-edc-0.2.9/intecomm_labs/list_data.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      500 2021-09-17 02:16:20.000000 intecomm-edc-0.2.9/intecomm_labs/processing_profiles.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      516 2023-12-06 16:38:41.000000 intecomm-edc-0.2.9/intecomm_labs/reportables.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.198477 intecomm-edc-0.2.9/intecomm_labs/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_labs/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.199002 intecomm-edc-0.2.9/intecomm_labs/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_labs/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      987 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_labs/tests/tests/test_labs.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      539 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_labs/tests/tests/test_reportables.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      116 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_labs/tests/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.200795 intecomm-edc-0.2.9/intecomm_lists/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_lists/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      630 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_lists/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-03-14 02:24:52.000000 intecomm-edc-0.2.9/intecomm_lists/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      287 2022-03-12 18:10:47.000000 intecomm-edc-0.2.9/intecomm_lists/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      750 2023-10-06 00:30:17.000000 intecomm-edc-0.2.9/intecomm_lists/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       63 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_lists/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    13385 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_lists/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.204382 intecomm-edc-0.2.9/intecomm_lists/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    77605 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_lists/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      465 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_lists/migrations/0002_delete_reasonsfortesting_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2717 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_lists/migrations/0003_dmmanagement_dmmanagement_intecomm_li_id_b4d41f_idx.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5252 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_lists/migrations/0004_rxmodificationreasons_rxmodifications_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2722 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_lists/migrations/0005_htnmanagement_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5229 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_lists/migrations/0006_consentrefusalreasons_screeningrefusalreasons_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6012 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_lists/migrations/0007_arvdrugs_extra_value_arvregimens_extra_value_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2838 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_lists/migrations/0008_medicationshortagereasons.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    66840 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_lists/migrations/0009_alter_arvdrugs_options_alter_arvregimens_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4742 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_lists/migrations/0010_remove_arvdrugs_intecomm_li_name_b55bdc_idx_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8363 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_lists/migrations/0011_accompanied_moneysources_travelmethods.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      610 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_lists/migrations/0012_visitreasons_custom_name.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_lists/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6430 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_lists/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.204496 intecomm-edc-0.2.9/intecomm_lists/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_lists/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.204722 intecomm-edc-0.2.9/intecomm_lists/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_lists/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      212 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_lists/tests/tests/test_lists.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      208 2022-03-12 18:05:17.000000 intecomm-edc-0.2.9/intecomm_lists/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.206679 intecomm-edc-0.2.9/intecomm_prn/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_prn/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4566 2024-01-10 16:23:30.000000 intecomm-edc-0.2.9/intecomm_prn/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.209120 intecomm-edc-0.2.9/intecomm_prn/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      499 2023-07-20 02:48:14.000000 intecomm-edc-0.2.9/intecomm_prn/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4724 2023-09-27 00:31:13.000000 intecomm-edc-0.2.9/intecomm_prn/admin/end_of_study_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1851 2023-09-27 00:31:13.000000 intecomm-edc-0.2.9/intecomm_prn/admin/loss_to_followup_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2624 2023-07-10 18:57:10.000000 intecomm-edc-0.2.9/intecomm_prn/admin/modeladmin_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      591 2023-09-27 00:31:13.000000 intecomm-edc-0.2.9/intecomm_prn/admin/offschedule_comm_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      591 2023-09-27 00:31:13.000000 intecomm-edc-0.2.9/intecomm_prn/admin/offschedule_inte_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      379 2024-02-06 04:30:17.000000 intecomm-edc-0.2.9/intecomm_prn/admin/onschedule_comm_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      379 2024-02-06 04:30:17.000000 intecomm-edc-0.2.9/intecomm_prn/admin/onschedule_inte_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      783 2024-02-06 04:30:17.000000 intecomm-edc-0.2.9/intecomm_prn/admin/protocol_incident_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1552 2024-02-06 04:30:17.000000 intecomm-edc-0.2.9/intecomm_prn/admin/subject_locator_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      767 2024-02-06 04:30:17.000000 intecomm-edc-0.2.9/intecomm_prn/admin/subject_transfer_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      169 2022-10-18 02:27:53.000000 intecomm-edc-0.2.9/intecomm_prn/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      289 2023-11-30 05:45:16.000000 intecomm-edc-0.2.9/intecomm_prn/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3151 2022-11-29 06:19:20.000000 intecomm-edc-0.2.9/intecomm_prn/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      104 2023-08-13 21:38:00.000000 intecomm-edc-0.2.9/intecomm_prn/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.211147 intecomm-edc-0.2.9/intecomm_prn/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      481 2024-02-06 04:30:17.000000 intecomm-edc-0.2.9/intecomm_prn/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      937 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_prn/forms/end_of_study_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1404 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_prn/forms/loss_to_followup_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      959 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_prn/forms/offschedule_comm_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      959 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_prn/forms/offschedule_inte_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      953 2024-02-06 04:30:17.000000 intecomm-edc-0.2.9/intecomm_prn/forms/onschedule_comm_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      953 2024-02-06 04:30:17.000000 intecomm-edc-0.2.9/intecomm_prn/forms/onschedule_inte_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      231 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_prn/forms/protocol_incident_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      734 2024-02-06 04:30:17.000000 intecomm-edc-0.2.9/intecomm_prn/forms/subject_locator_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      817 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_prn/forms/subject_transfer_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2336 2023-07-27 02:22:12.000000 intecomm-edc-0.2.9/intecomm_prn/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.218092 intecomm-edc-0.2.9/intecomm_prn/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)   149190 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_prn/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3533 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_prn/migrations/0002_remove_endofstudy_delivery_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1913 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_prn/migrations/0003_historicalprotocolincident_reasons_withdrawn_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3192 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_prn/migrations/0004_rename_historicaloffschedulebaseline_historicaloffschedulecomm_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3237 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_prn/migrations/0005_rename_historicaloffschedulefollowup_historicaloffscheduleinte_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4029 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_prn/migrations/0006_alter_historicaloffschedulecomm_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4811 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_prn/migrations/0007_alter_losstofollowup_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      715 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_prn/migrations/0008_alter_endofstudy_options.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    18584 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_prn/migrations/0009_subjectlocator_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      855 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_prn/migrations/0010_alter_historicalsubjectlocator_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    21655 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_prn/migrations/0011_alter_endofstudy_device_created_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5276 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_prn/migrations/0012_alter_endofstudy_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    12574 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_prn/migrations/0013_endofstudy_locale_created_endofstudy_locale_modified_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6784 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_prn/migrations/0014_endofstudy_intecomm_pr_action__f3bf58_idx_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2295 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_prn/migrations/0015_protocolincident_intecomm_pr_subject_54092b_idx_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6447 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_prn/migrations/0016_alter_endofstudy_site_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_prn/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.220156 intecomm-edc-0.2.9/intecomm_prn/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      390 2023-08-13 21:28:05.000000 intecomm-edc-0.2.9/intecomm_prn/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3592 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_prn/models/end_of_study.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2328 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_prn/models/loss_to_followup.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1206 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_prn/models/offschedule_comm.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1204 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_prn/models/offschedule_inte.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      598 2024-02-06 04:30:17.000000 intecomm-edc-0.2.9/intecomm_prn/models/onschedule_comm.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      596 2024-02-06 04:30:17.000000 intecomm-edc-0.2.9/intecomm_prn/models/onschedule_inte.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1341 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_prn/models/protocol_incident.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      221 2023-07-20 02:48:14.000000 intecomm-edc-0.2.9/intecomm_prn/models/proxy.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      339 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_prn/models/subject_transfer.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.124415 intecomm-edc-0.2.9/intecomm_prn/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.220435 intecomm-edc-0.2.9/intecomm_prn/templates/intecomm_prn/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1279 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_prn/templates/intecomm_prn/changelist_locator_contacts.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.220785 intecomm-edc-0.2.9/intecomm_prn/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_prn/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.221005 intecomm-edc-0.2.9/intecomm_prn/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_prn/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      290 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_prn/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      206 2022-10-18 02:47:10.000000 intecomm-edc-0.2.9/intecomm_prn/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.224205 intecomm-edc-0.2.9/intecomm_screening/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_screening/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.227194 intecomm-edc-0.2.9/intecomm_screening/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      666 2023-08-29 02:39:08.000000 intecomm-edc-0.2.9/intecomm_screening/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1355 2023-07-20 02:48:14.000000 intecomm-edc-0.2.9/intecomm_screening/admin/actions.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      447 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_screening/admin/autocomplete_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1647 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_screening/admin/consent_refusal_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3305 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_screening/admin/health_facility_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2982 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_screening/admin/health_talk_log_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5273 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/admin/list_filters.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3837 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/admin/modeladmin_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5262 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/admin/patient_call_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2248 2023-07-10 18:57:10.000000 intecomm-edc-0.2.9/intecomm_screening/admin/patient_call_inlines.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    12348 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/admin/patient_group_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3966 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_screening/admin/patient_group_rando_admin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.228841 intecomm-edc-0.2.9/intecomm_screening/admin/patient_log/
+-rw-r--r--   0 erikvw     (501) staff       (20)       99 2023-08-29 02:39:08.000000 intecomm-edc-0.2.9/intecomm_screening/admin/patient_log/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6811 2023-08-29 21:57:21.000000 intecomm-edc-0.2.9/intecomm_screening/admin/patient_log/change_list_template_context.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2842 2023-08-31 03:37:01.000000 intecomm-edc-0.2.9/intecomm_screening/admin/patient_log/fieldsets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      653 2023-08-29 02:39:08.000000 intecomm-edc-0.2.9/intecomm_screening/admin/patient_log/get_search_fields.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    13105 2024-01-29 02:23:02.000000 intecomm-edc-0.2.9/intecomm_screening/admin/patient_log/modeladmin_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2405 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/admin/patient_log/patient_log_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2379 2024-01-29 04:38:11.000000 intecomm-edc-0.2.9/intecomm_screening/admin/patient_log/patient_log_ug_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1088 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_screening/admin/patient_log_report_print_history_admin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.229935 intecomm-edc-0.2.9/intecomm_screening/admin/subject_screening/
+-rw-r--r--   0 erikvw     (501) staff       (20)      187 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/admin/subject_screening/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3342 2023-08-29 02:39:08.000000 intecomm-edc-0.2.9/intecomm_screening/admin/subject_screening/fieldsets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5084 2023-08-29 21:57:21.000000 intecomm-edc-0.2.9/intecomm_screening/admin/subject_screening/modeladmin_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2122 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_screening/admin/subject_screening/subject_screening_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2503 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/admin/subject_screening/subject_screening_tz_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2558 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/admin/subject_screening/subject_screening_ug_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      843 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      553 2022-03-12 17:44:16.000000 intecomm-edc-0.2.9/intecomm_screening/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      549 2023-05-04 03:51:54.000000 intecomm-edc-0.2.9/intecomm_screening/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      402 2022-03-03 20:12:26.000000 intecomm-edc-0.2.9/intecomm_screening/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1885 2023-11-22 02:42:27.000000 intecomm-edc-0.2.9/intecomm_screening/baker_recipes.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      226 2023-05-04 03:51:54.000000 intecomm-edc-0.2.9/intecomm_screening/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       33 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       49 2023-07-02 21:12:50.000000 intecomm-edc-0.2.9/intecomm_screening/exceptions.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.233007 intecomm-edc-0.2.9/intecomm_screening/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      335 2023-08-29 21:57:21.000000 intecomm-edc-0.2.9/intecomm_screening/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2028 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/forms/consent_refusal_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      366 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_screening/forms/health_talk_log_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      356 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_screening/forms/patient_call_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3696 2023-08-08 02:36:10.000000 intecomm-edc-0.2.9/intecomm_screening/forms/patient_group_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      751 2023-07-05 03:07:33.000000 intecomm-edc-0.2.9/intecomm_screening/forms/patient_group_rando_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.233624 intecomm-edc-0.2.9/intecomm_screening/forms/patient_log/
+-rw-r--r--   0 erikvw     (501) staff       (20)       95 2023-08-29 02:39:08.000000 intecomm-edc-0.2.9/intecomm_screening/forms/patient_log/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1631 2023-08-29 02:39:08.000000 intecomm-edc-0.2.9/intecomm_screening/forms/patient_log/patient_log_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      676 2023-08-29 02:39:08.000000 intecomm-edc-0.2.9/intecomm_screening/forms/patient_log/patient_log_ug_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.234407 intecomm-edc-0.2.9/intecomm_screening/forms/subject_screening/
+-rw-r--r--   0 erikvw     (501) staff       (20)      119 2023-08-29 21:57:21.000000 intecomm-edc-0.2.9/intecomm_screening/forms/subject_screening/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8456 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/forms/subject_screening/modelform_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1699 2023-08-29 21:57:21.000000 intecomm-edc-0.2.9/intecomm_screening/forms/subject_screening/subject_screening_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1711 2023-08-29 21:57:21.000000 intecomm-edc-0.2.9/intecomm_screening/forms/subject_screening/subject_screening_ug_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2369 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/identifiers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      944 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/intecomm_admin_site_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.125679 intecomm-edc-0.2.9/intecomm_screening/locale/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.125606 intecomm-edc-0.2.9/intecomm_screening/locale/lg/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.234548 intecomm-edc-0.2.9/intecomm_screening/locale/lg/LC_MESSAGES/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2075 2023-11-30 05:45:16.000000 intecomm-edc-0.2.9/intecomm_screening/locale/lg/LC_MESSAGES/django.po
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.125735 intecomm-edc-0.2.9/intecomm_screening/locale/sw/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.235024 intecomm-edc-0.2.9/intecomm_screening/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 erikvw     (501) staff       (20)      380 2023-08-24 22:02:31.000000 intecomm-edc-0.2.9/intecomm_screening/locale/sw/LC_MESSAGES/django.mo
+-rw-r--r--   0 erikvw     (501) staff       (20)     2121 2023-08-24 22:02:29.000000 intecomm-edc-0.2.9/intecomm_screening/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.235257 intecomm-edc-0.2.9/intecomm_screening/management/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-18 02:36:12.000000 intecomm-edc-0.2.9/intecomm_screening/management/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.235437 intecomm-edc-0.2.9/intecomm_screening/management/commands/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-18 02:36:12.000000 intecomm-edc-0.2.9/intecomm_screening/management/commands/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3188 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_screening/management/commands/print_patient_log_reference.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.249558 intecomm-edc-0.2.9/intecomm_screening/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)   128990 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1281 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0002_remove_healthtalklog_unique_lower_name_report_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2757 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0003_site_remove_historicalpatientlog_patient_group_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1450 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0004_rename_name_historicalpatientlog_legal_name_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2033 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0005_historicalpatientcall_alt_contact_number_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3722 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0006_remove_historicalpatientcall_willing_to_attend_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2228 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0007_historicalpatientlog_last_4_contact_number_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7009 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0008_rename_last_routine_appt_date_historicalpatientlog_last_appt_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3258 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0009_historicalsubjectscreening_familiar_name_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      716 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0010_historicalpatientlog_age_in_years_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3939 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0011_rename_hf_identifier_historicalpatientlog_hospital_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1146 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0012_alter_historicalpatientcall_last_attend_clinic_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1892 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0013_alter_healthfacility_distance_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3541 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0014_alter_historicalpatientlog_familiar_name_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      560 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0015_remove_healthtalklog_unique_health_facility_report_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      974 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0016_historicalpatientlog_group_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      925 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0017_alter_historicalpatientlog_group_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1083 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0018_alter_historicalpatientlog_age_in_years_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2673 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0019_healthfacility_fri_healthfacility_mon_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    16562 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0020_consentrefusal_historicalconsentrefusal_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4414 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0021_idenfifierformat.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1032 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0022_historicalpatientlog_filing_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      891 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0023_auto_20230501_2208.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      835 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0024_auto_20230502_0249.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5013 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0025_patientlogreportprinthistory_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1062 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0026_alter_historicalpatientlog_filing_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      606 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0027_historicalpatientlog_printed_patientlog_printed.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      463 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0028_alter_patientlogreportprinthistory_patient_log_identifier.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2289 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0029_alter_historicalpatientlog_filing_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1213 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0030_auto_20230510_0352.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0031_alter_historicalpatientlog_next_appt_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1033 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0032_patientgrouprando.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1358 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0033_remove_consentrefusal_subject_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2119 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0034_alter_consentrefusal_screening_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      991 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0035_auto_20230630_0552.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1680 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0036_alter_historicalpatientlog_screening_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2369 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0037_alter_consentrefusal_screening_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1908 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0038_auto_20230701_0117.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1026 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0039_alter_historicalpatientlog_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1165 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0040_historicalsubjectscreening_patient_log_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      852 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0041_auto_20230702_1548.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4738 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0042_alter_healthfacility_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      968 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0043_auto_20230705_0529.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2521 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0044_alter_historicalpatientlog_site_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2518 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0045_alter_consentrefusal_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3334 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0046_alter_historicalpatientlog_legal_name_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1221 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0047_rename_historicalhealthfacility_historicaloldhealthfacility_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1220 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0048_rename_historicalhealthfacility_historicaloldhealthfacility_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      731 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0049_healthfacility.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1550 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0050_delete_healthfacility_healthtalklog_health_facility_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1421 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0051_auto_20230726_1631.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1301 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0052_auto_20230726_1634.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      967 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0053_rename_idenfifierformat_identifierformat_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      503 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0054_alter_healthtalklog_unique_together.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      332 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0055_delete_identifierformat.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      318 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0056_delete_healthfacility.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    16611 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0057_alter_consentrefusal_device_created_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      931 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0058_patientlogug.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    25711 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0059_subjectscreeningug_historicalsubjectscreeningug.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    18669 2023-08-29 02:39:08.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0060_historicalpatientlogug.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      809 2023-08-31 03:37:01.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0061_historicalpatientlog_comment_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1688 2023-08-31 03:37:01.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0062_auto_20230831_0032.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    15518 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0063_alter_consentrefusal_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2811 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0064_alter_patientcall_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1920 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0065_patientlogreportprinthistory_intecomm_sc_modifie_891a97_idx_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1095 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0066_alter_patientlogreportprinthistory_managers_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1132 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0067_auto_20231216_1807.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3480 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0068_alter_consentrefusal_site_alter_healthtalklog_site_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    26534 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/0069_subjectscreeningtz_historicalsubjectscreeningtz.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_screening/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.249948 intecomm-edc-0.2.9/intecomm_screening/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)       60 2022-11-23 01:31:30.000000 intecomm-edc-0.2.9/intecomm_screening/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2626 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_screening/model_mixins/patient_call_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.254603 intecomm-edc-0.2.9/intecomm_screening/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1072 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2392 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_screening/models/consent_refusal.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1829 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_screening/models/health_talk_log.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      752 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_screening/models/identifier_format.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      485 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_screening/models/location.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3009 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_screening/models/old_health_facility.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      958 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_screening/models/patient_call.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    10303 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/models/patient_log.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      560 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_screening/models/patient_log_report_print_history.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      206 2023-08-29 02:39:08.000000 intecomm-edc-0.2.9/intecomm_screening/models/patient_log_ug.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.255988 intecomm-edc-0.2.9/intecomm_screening/models/proxy_models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      114 2023-08-28 14:56:49.000000 intecomm-edc-0.2.9/intecomm_screening/models/proxy_models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      196 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_screening/models/proxy_models/health_facility.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      265 2023-01-25 03:04:55.000000 intecomm-edc-0.2.9/intecomm_screening/models/proxy_models/patient_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      383 2023-05-12 04:56:33.000000 intecomm-edc-0.2.9/intecomm_screening/models/proxy_models/patient_group_rando.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      185 2022-11-23 01:31:30.000000 intecomm-edc-0.2.9/intecomm_screening/models/proxy_models/site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5338 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/models/signals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9789 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/models/subject_screening.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      333 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/models/subject_screening_tz.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      329 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/models/subject_screening_ug.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.256525 intecomm-edc-0.2.9/intecomm_screening/reports/
+-rw-r--r--   0 erikvw     (501) staff       (20)       72 2023-05-05 04:31:31.000000 intecomm-edc-0.2.9/intecomm_screening/reports/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    17443 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/reports/patient_log_report.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.126318 intecomm-edc-0.2.9/intecomm_screening/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.258753 intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.259829 intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      253 2023-07-02 21:12:50.000000 intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/admin/healthtalklog_change_list.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      253 2023-07-02 21:12:50.000000 intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/admin/patientcall_change_list.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      253 2023-07-02 21:12:50.000000 intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/admin/patientgroup_change_list.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      253 2023-08-28 14:26:40.000000 intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/admin/patientlog_change_list.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      253 2023-07-05 03:07:33.000000 intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/admin/subjectscreening_change_list.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      240 2022-11-29 06:19:20.000000 intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/change_list_appts.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      484 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/change_list_contacts.html
+-rw-r--r--   0 erikvw     (501) staff       (20)       94 2022-11-29 06:19:20.000000 intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/change_list_dx.html
+-rw-r--r--   0 erikvw     (501) staff       (20)       65 2023-05-04 03:51:54.000000 intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/change_list_filing_identifier.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      606 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/change_list_group.html
+-rw-r--r--   0 erikvw     (501) staff       (20)       81 2022-11-29 06:19:20.000000 intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/change_list_hospital_identifier.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      727 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/change_list_patient_log_first_column.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     3044 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/change_list_screen_and_consent.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      462 2022-11-29 06:19:20.000000 intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/change_list_talks.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1387 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/group_management.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.260450 intecomm-edc-0.2.9/intecomm_screening/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_screening/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_screening/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)    16784 2024-02-06 04:30:17.000000 intecomm-edc-0.2.9/intecomm_screening/tests/intecomm_test_case_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.261684 intecomm-edc-0.2.9/intecomm_screening/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:30.000000 intecomm-edc-0.2.9/intecomm_screening/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7258 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_screening/tests/tests/test_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7483 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/tests/tests/test_consent_refusal.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    17317 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_screening/tests/tests/test_screening.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      579 2023-05-10 11:59:10.000000 intecomm-edc-0.2.9/intecomm_screening/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5863 2023-08-29 02:39:08.000000 intecomm-edc-0.2.9/intecomm_screening/utils.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1828 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_screening/views.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.262791 intecomm-edc-0.2.9/intecomm_sites/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_sites/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      287 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_sites/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      428 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_sites/intecomm_site.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.263039 intecomm-edc-0.2.9/intecomm_sites/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-03-12 18:03:07.000000 intecomm-edc-0.2.9/intecomm_sites/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       46 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_sites/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5192 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_sites/sites.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.263239 intecomm-edc-0.2.9/intecomm_sites/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_sites/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      357 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_sites/tests/site_test_case_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.265551 intecomm-edc-0.2.9/intecomm_subject/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-11-22 15:10:26.000000 intecomm-edc-0.2.9/intecomm_subject/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      628 2023-11-16 04:10:04.000000 intecomm-edc-0.2.9/intecomm_subject/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.275129 intecomm-edc-0.2.9/intecomm_subject/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2506 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1818 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_subject/admin/appointment_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      299 2022-11-29 06:19:20.000000 intecomm-edc-0.2.9/intecomm_subject/admin/arv_regimens_admin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.276602 intecomm-edc-0.2.9/intecomm_subject/admin/blood_results/
+-rw-r--r--   0 erikvw     (501) staff       (20)      414 2022-11-29 06:19:20.000000 intecomm-edc-0.2.9/intecomm_subject/admin/blood_results/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      723 2023-07-06 02:16:06.000000 intecomm-edc-0.2.9/intecomm_subject/admin/blood_results/blood_results_fbc_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      966 2023-07-06 02:16:02.000000 intecomm-edc-0.2.9/intecomm_subject/admin/blood_results/blood_results_glu_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      785 2023-07-06 02:16:13.000000 intecomm-edc-0.2.9/intecomm_subject/admin/blood_results/blood_results_hba1c_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      746 2023-07-06 02:16:20.000000 intecomm-edc-0.2.9/intecomm_subject/admin/blood_results/blood_results_ins_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      746 2023-07-06 02:16:26.000000 intecomm-edc-0.2.9/intecomm_subject/admin/blood_results/blood_results_lft_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      760 2023-07-06 02:16:33.000000 intecomm-edc-0.2.9/intecomm_subject/admin/blood_results/blood_results_lipid_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4598 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_subject/admin/blood_results/blood_results_rft_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      584 2022-11-29 06:19:20.000000 intecomm-edc-0.2.9/intecomm_subject/admin/cd4_result_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      759 2023-08-25 12:06:52.000000 intecomm-edc-0.2.9/intecomm_subject/admin/clinic_note_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1343 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/admin/clinical_review_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1257 2023-04-20 03:59:58.000000 intecomm-edc-0.2.9/intecomm_subject/admin/clinical_review_baseline_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1599 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/admin/complications_baseline_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1621 2023-07-05 03:07:33.000000 intecomm-edc-0.2.9/intecomm_subject/admin/complications_followup_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      754 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/admin/concomitant_medication_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1653 2023-04-25 03:09:42.000000 intecomm-edc-0.2.9/intecomm_subject/admin/dm_initial_review_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      434 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_subject/admin/dm_medication_adherence_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1149 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/admin/dm_review_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      796 2023-07-10 18:57:10.000000 intecomm-edc-0.2.9/intecomm_subject/admin/drug_refill_dm_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1779 2023-07-12 23:56:44.000000 intecomm-edc-0.2.9/intecomm_subject/admin/drug_refill_hiv_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1008 2023-07-10 18:57:10.000000 intecomm-edc-0.2.9/intecomm_subject/admin/drug_refill_htn_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      618 2023-05-24 22:37:50.000000 intecomm-edc-0.2.9/intecomm_subject/admin/eq5d3l_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1851 2024-02-06 04:30:17.000000 intecomm-edc-0.2.9/intecomm_subject/admin/family_history_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      349 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_subject/admin/fieldsets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1114 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/admin/glucose_admin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.278487 intecomm-edc-0.2.9/intecomm_subject/admin/health_economics/
+-rw-r--r--   0 erikvw     (501) staff       (20)      388 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/admin/health_economics/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1819 2023-08-18 02:43:47.000000 intecomm-edc-0.2.9/intecomm_subject/admin/health_economics/assets_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4262 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/admin/health_economics/careseeking_a_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5282 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/admin/health_economics/careseeking_b_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1855 2023-08-10 17:37:32.000000 intecomm-edc-0.2.9/intecomm_subject/admin/health_economics/household_head_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      488 2023-07-05 03:07:33.000000 intecomm-edc-0.2.9/intecomm_subject/admin/health_economics/income_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1783 2023-08-04 04:50:38.000000 intecomm-edc-0.2.9/intecomm_subject/admin/health_economics/patient_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      502 2023-07-05 03:07:33.000000 intecomm-edc-0.2.9/intecomm_subject/admin/health_economics/property_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2574 2024-02-02 13:01:52.000000 intecomm-edc-0.2.9/intecomm_subject/admin/hiv_initial_review_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      439 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_subject/admin/hiv_medication_adherence_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2245 2024-02-02 13:02:06.000000 intecomm-edc-0.2.9/intecomm_subject/admin/hiv_review_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1460 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/admin/htn_initial_review_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      439 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_subject/admin/htn_medication_adherence_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      840 2023-07-11 03:12:55.000000 intecomm-edc-0.2.9/intecomm_subject/admin/htn_review_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      632 2023-05-24 22:37:50.000000 intecomm-edc-0.2.9/intecomm_subject/admin/icecapa_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2339 2024-02-02 02:23:27.000000 intecomm-edc-0.2.9/intecomm_subject/admin/list_filters.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      840 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_subject/admin/location_update_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      422 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/admin/malaria_test_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      960 2023-05-09 03:31:16.000000 intecomm-edc-0.2.9/intecomm_subject/admin/medications_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2513 2024-02-15 12:37:45.000000 intecomm-edc-0.2.9/intecomm_subject/admin/modeladmin_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      914 2023-10-06 00:30:17.000000 intecomm-edc-0.2.9/intecomm_subject/admin/next_appointment_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2893 2023-07-18 02:36:12.000000 intecomm-edc-0.2.9/intecomm_subject/admin/other_baseline_data_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5263 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/admin/social_harms_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1788 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_subject/admin/subject_requisition_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1456 2023-07-10 18:57:10.000000 intecomm-edc-0.2.9/intecomm_subject/admin/subject_visit_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1232 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/admin/subject_visit_missed_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1074 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/admin/urine_dipstick_test_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      967 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/admin/urine_pregnancy_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2229 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/admin/vitals_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-03-12 18:18:07.000000 intecomm-edc-0.2.9/intecomm_subject/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      298 2022-03-12 18:18:07.000000 intecomm-edc-0.2.9/intecomm_subject/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1736 2023-08-10 17:37:32.000000 intecomm-edc-0.2.9/intecomm_subject/baker_recipes.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    12615 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      413 2024-02-15 12:37:45.000000 intecomm-edc-0.2.9/intecomm_subject/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1102 2023-11-30 05:45:33.000000 intecomm-edc-0.2.9/intecomm_subject/form_runners.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.286137 intecomm-edc-0.2.9/intecomm_subject/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2479 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2368 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_subject/forms/appointment_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.287259 intecomm-edc-0.2.9/intecomm_subject/forms/blood_results/
+-rw-r--r--   0 erikvw     (501) staff       (20)      400 2022-11-29 06:19:20.000000 intecomm-edc-0.2.9/intecomm_subject/forms/blood_results/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      714 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/forms/blood_results/blood_results_fbc_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      823 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/forms/blood_results/blood_results_glu_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      765 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/forms/blood_results/blood_results_hba1c_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      722 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/forms/blood_results/blood_results_ins_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      714 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/forms/blood_results/blood_results_lft_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      730 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/forms/blood_results/blood_results_lipid_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1362 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/forms/blood_results/blood_results_rft_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      646 2022-11-29 06:19:20.000000 intecomm-edc-0.2.9/intecomm_subject/forms/cd4_result_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      630 2023-08-01 05:53:40.000000 intecomm-edc-0.2.9/intecomm_subject/forms/clinical_note_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      422 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/forms/clinical_review_baseline_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      422 2023-08-25 11:51:02.000000 intecomm-edc-0.2.9/intecomm_subject/forms/clinical_review_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      400 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/forms/complications_baseline_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      402 2023-07-05 03:07:33.000000 intecomm-edc-0.2.9/intecomm_subject/forms/complications_followup_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      489 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/forms/concomitant_medication_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      370 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/forms/dm_initial_review_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      910 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_subject/forms/dm_medication_adherence_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      335 2022-11-29 06:19:20.000000 intecomm-edc-0.2.9/intecomm_subject/forms/dm_review_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      355 2022-11-29 06:19:20.000000 intecomm-edc-0.2.9/intecomm_subject/forms/drug_refill_dm_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      360 2022-11-29 06:19:20.000000 intecomm-edc-0.2.9/intecomm_subject/forms/drug_refill_hiv_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      360 2022-11-29 06:19:20.000000 intecomm-edc-0.2.9/intecomm_subject/forms/drug_refill_htn_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      387 2022-11-29 06:19:20.000000 intecomm-edc-0.2.9/intecomm_subject/forms/drug_supply_dm_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      781 2022-11-29 06:19:20.000000 intecomm-edc-0.2.9/intecomm_subject/forms/drug_supply_hiv_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      393 2022-11-29 06:19:20.000000 intecomm-edc-0.2.9/intecomm_subject/forms/drug_supply_htn_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      545 2023-05-24 22:37:50.000000 intecomm-edc-0.2.9/intecomm_subject/forms/eq5d3l_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      394 2024-02-06 04:30:17.000000 intecomm-edc-0.2.9/intecomm_subject/forms/family_history_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.289396 intecomm-edc-0.2.9/intecomm_subject/forms/health_economics/
+-rw-r--r--   0 erikvw     (501) staff       (20)      369 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/forms/health_economics/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      594 2023-08-10 17:37:32.000000 intecomm-edc-0.2.9/intecomm_subject/forms/health_economics/assets_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      531 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/forms/health_economics/careseeking_a_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      372 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/forms/health_economics/careseeking_b_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3141 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_subject/forms/health_economics/household_head.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      644 2023-08-10 17:37:32.000000 intecomm-edc-0.2.9/intecomm_subject/forms/health_economics/income_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      426 2023-08-16 02:41:30.000000 intecomm-edc-0.2.9/intecomm_subject/forms/health_economics/modelform_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      599 2023-08-10 17:37:32.000000 intecomm-edc-0.2.9/intecomm_subject/forms/health_economics/patient_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      604 2023-08-10 17:37:32.000000 intecomm-edc-0.2.9/intecomm_subject/forms/health_economics/property_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      403 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/forms/hiv_initial_review_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      927 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_subject/forms/hiv_medication_adherence_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2326 2024-02-01 16:00:54.000000 intecomm-edc-0.2.9/intecomm_subject/forms/hiv_review_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      386 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/forms/htn_initial_review_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      927 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_subject/forms/htn_medication_adherence_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      340 2024-02-01 14:33:25.000000 intecomm-edc-0.2.9/intecomm_subject/forms/htn_review_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      364 2023-05-24 22:37:50.000000 intecomm-edc-0.2.9/intecomm_subject/forms/icecapa_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      982 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_subject/forms/location_update_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      365 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/forms/malaria_test_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      350 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/forms/medications_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      268 2022-12-05 14:48:19.000000 intecomm-edc-0.2.9/intecomm_subject/forms/mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      783 2023-10-06 00:30:17.000000 intecomm-edc-0.2.9/intecomm_subject/forms/next_appointment_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      380 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/forms/other_baseline_data.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      350 2023-01-25 03:04:55.000000 intecomm-edc-0.2.9/intecomm_subject/forms/social_harms_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      953 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/forms/subject_requisition_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      791 2024-02-01 03:43:59.000000 intecomm-edc-0.2.9/intecomm_subject/forms/subject_visit_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2274 2023-08-13 00:11:46.000000 intecomm-edc-0.2.9/intecomm_subject/forms/subject_visit_missed_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      827 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/forms/urine_dipstick_test_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1267 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/forms/urine_pregnancy_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      342 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/forms/vitals_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.127490 intecomm-edc-0.2.9/intecomm_subject/locale/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.127429 intecomm-edc-0.2.9/intecomm_subject/locale/lg/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.289945 intecomm-edc-0.2.9/intecomm_subject/locale/lg/LC_MESSAGES/
+-rw-r--r--   0 erikvw     (501) staff       (20)      337 2023-11-28 00:33:14.000000 intecomm-edc-0.2.9/intecomm_subject/locale/lg/LC_MESSAGES/django.mo
+-rw-r--r--   0 erikvw     (501) staff       (20)     7140 2023-11-30 05:45:16.000000 intecomm-edc-0.2.9/intecomm_subject/locale/lg/LC_MESSAGES/django.po
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.127536 intecomm-edc-0.2.9/intecomm_subject/locale/sw/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.290448 intecomm-edc-0.2.9/intecomm_subject/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 erikvw     (501) staff       (20)      447 2023-11-28 00:30:12.000000 intecomm-edc-0.2.9/intecomm_subject/locale/sw/LC_MESSAGES/django.mo
+-rw-r--r--   0 erikvw     (501) staff       (20)     7603 2023-11-30 05:45:16.000000 intecomm-edc-0.2.9/intecomm_subject/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.290669 intecomm-edc-0.2.9/intecomm_subject/management/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_subject/management/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.291225 intecomm-edc-0.2.9/intecomm_subject/management/commands/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_subject/management/commands/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8440 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_subject/management/commands/missed.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      797 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_subject/management/commands/seen_on_day.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.291947 intecomm-edc-0.2.9/intecomm_subject/metadata_rules/
+-rw-r--r--   0 erikvw     (501) staff       (20)      154 2023-08-06 23:03:01.000000 intecomm-edc-0.2.9/intecomm_subject/metadata_rules/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5004 2024-02-15 12:37:45.000000 intecomm-edc-0.2.9/intecomm_subject/metadata_rules/metadata_rules.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1846 2024-02-19 22:04:54.000000 intecomm-edc-0.2.9/intecomm_subject/metadata_rules/predicates.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.327058 intecomm-edc-0.2.9/intecomm_subject/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)  1030442 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    58037 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0002_remove_historicaldminitialreview_managed_by_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1791 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0003_alter_historicalsocialharms_coworkers_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    24955 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0004_historicalsocialharms_employment_impact_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    82105 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0005_alter_historicalsocialharms_coworkers_impact_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1089 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0006_alter_healtheconomics_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1497 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0007_alter_historicalotherbaselinedata_alcohol_consumption_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    23861 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0008_historicalvitals_vitals_remove_indicators_site_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3554 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0009_remove_historicalvitals_bp_measured_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3177 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0010_remove_historicalvitals_weight_is_estmated_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1500 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0011_remove_clinicalreviewbaseline_complications_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1178 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0012_alter_historicalvitals_heart_rate_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    11537 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0013_alter_bloodresultsfbc_results_abnormal_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4242 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0014_alter_historicalotherbaselinedata_activity_combined_mn_avg_day_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    14317 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0015_alter_bloodresultsfbc_results_abnormal_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7271 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0016_remove_clinicalreview_reason_other_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    11082 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0017_alter_bloodresultsfbc_results_abnormal_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7971 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0018_remove_historicalhivinitialreview_vl_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1259 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0019_remove_historicalhtninitialreview_med_start_date_estimated_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4308 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0020_remove_historicalhtninitialreview_managed_by_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1770 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0021_htninitialreview_managed_by_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1020 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0022_historicalhtninitialreview_managed_by_other_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1075 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0023_auto_20230404_0411.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1004 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0024_historicalhtninitialreview_med_start_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2655 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0025_rename_med_start_ago_dminitialreview_rx_init_ago_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2660 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0026_rename_dminitialreview_med_start_date_estimated_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    15922 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0027_dminitialreview_rx_init_dminitialreview_rx_init_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5727 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0028_remove_clinicalreviewbaseline_dm_test_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2215 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0029_remove_historicaldminitialreview_med_start_estimated_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    17272 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0030_nextappointment_historicalnextappointment_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2367 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0031_alter_clinicalreviewbaseline_dm_dx_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9087 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0032_historicalnextappointment_best_visit_code_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4995 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0033_clinicalreviewbaseline_dm_dx_at_screening_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4599 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0034_clinicalreviewbaseline_protocol_incident_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3126 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0035_alter_drugrefilldm_return_in_days_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2647 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0036_alter_dminitialreview_rx_init_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6697 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0037_alter_bloodresultsins_fasting_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      791 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0038_healtheconomics_welfare_other_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    46429 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0039_icecapa_historicalicecapa_historicaleq5d3l_eq5d3l_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2094 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0040_alter_historicalhivmedicationadherence_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)   190375 2023-10-11 13:30:21.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0041_health_economics_assets_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6343 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0042_alter_bloodresultsins_fasting_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0043_healtheconomicshouseholdhead_relationship_to_hoh_other_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    11978 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0044_healtheconomicshouseholdhead_hoh_education_other_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1097 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0045_healtheconomicshouseholdhead_hoh_marital_status_other_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    20588 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0046_alter_healtheconomicsassets_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9292 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0047_healtheconomicsassets_cooking_fuel_other_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    29040 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0048_alter_healtheconomicsincome_external_remittance_currency_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    23015 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0049_alter_healtheconomicsincome_external_remittance_value_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    11452 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0050_alter_healtheconomicshouseholdhead_hoh_ethnicity_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    35733 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0051_alter_bloodresultsfbc_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    13854 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0052_alter_bloodresultsfbc_managers_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4705 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0053_remove_historicalhivreview_arv_initiated_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      756 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0054_remove_historicalhtnreview_dia_blood_pressure_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1259 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0055_rename_drugrefilldm_return_in_days_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2826 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0056_alter_drugrefilldm_rx_days_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6291 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0057_rename_smoker_current_duration_historicalotherbaselinedata_smoker_duration_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1145 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0058_rename_external_remittance_currency_healtheconomicsincome_external_remit_currency_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3184 2023-10-05 22:47:02.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0059_historicalnextappointment_info_source_old_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1978 2023-10-05 22:47:14.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0060_historicalnextappointment_info_source_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1593 2023-10-05 22:47:43.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0061_auto_20230725_2035.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    15892 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0062_historicalclinicalnote_clinicalnote.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1121 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0063_auto_20230725_2058.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      852 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0064_historicalnextappointment_health_facility_old_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      780 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0065_historicalnextappointment_health_facility_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1158 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0066_historicalnextappointment_health_facility_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1229 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0067_auto_20230726_0008.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    11874 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0068_remove_historicalhba1cresult_history_user_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5768 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0069_alter_healtheconomicshouseholdhead_hoh_employment_type_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      687 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0070_healtheconomicshouseholdhead_hoh_ethnicity_old_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3119 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0071_healtheconomicshouseholdhead_hoh_ethnicity_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1195 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0072_auto_20230803_0305.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      628 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0073_healtheconomicspatient_pat_ethnicity_new_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1679 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0074_healtheconomicspatient_pat_ethnicity_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      839 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0075_auto_20230803_0459.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      986 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0076_healtheconomicshouseholdhead_hoh_religion_old_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5006 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0077_healtheconomicshouseholdhead_hoh_religion_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1513 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0078_alter_healtheconomicshouseholdhead_hoh_religion_old_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1817 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0079_auto_20230803_0634.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      696 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0080_auto_20230803_1726.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1762 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0081_healtheconomicshouseholdhead_hoh_education_old_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3837 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0082_healtheconomicshouseholdhead_hoh_education_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2928 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0083_auto_20230803_1828.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3083 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0084_alter_healtheconomicsassets_external_wall_material_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2393 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0085_alter_healtheconomicsassets_external_wall_material_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1049 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0086_rename_hoh_employment_healtheconomicshouseholdhead_hoh_employment_status_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1073 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0087_alter_healtheconomicspatient_pat_citizen_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1089 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0088_healtheconomicspatient_pat_employment_type_other_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4414 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0089_alter_healtheconomicshouseholdhead_hoh_education_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    10743 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0090_alter_healtheconomicshouseholdhead_hoh_age_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    15119 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0091_healtheconomicsassets_solar_panels_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6326 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0092_healtheconomicsproperty_land_surface_area_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2245 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0093_alter_healtheconomicsproperty_land_value_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1252 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0094_alter_healtheconomicsproperty_land_surface_area_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3098 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0095_alter_healtheconomicsassets_bedrooms_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    12480 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0096_rename_external_remittance_healtheconomicsincome_external_remit_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    11438 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0097_alter_healtheconomicsincome_external_remit_value_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5715 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0098_alter_healtheconomicshouseholdhead_hoh_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      520 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0099_remove_healtheconomicspatient_pat_citizen_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2831 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0100_alter_healtheconomicspatient_pat_education_old_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3223 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0101_alter_healtheconomicspatient_pat_education_old_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3397 2023-08-10 18:18:35.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0102_alter_healtheconomicshouseholdhead_hoh_education_old_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5029 2023-08-13 00:11:46.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0103_alter_healtheconomicshouseholdhead_hoh_employment_status_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    17949 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0104_historicallocationupdate_locationupdate.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9164 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0105_alter_historicallocationupdate_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2719 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0106_dmmedicationadherence_meds_shortage_reason_other_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    16542 2023-08-23 23:05:23.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0107_alter_bloodresultsfbc_device_created_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    18686 2023-08-23 23:05:23.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0108_alter_concomitantmedication_device_created_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    27488 2023-08-23 23:05:23.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0109_alter_healtheconomicsassets_device_created_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    30836 2023-08-23 23:05:23.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0110_alter_historicalbloodresultsfbc_device_created_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    29288 2023-08-23 23:05:23.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0111_alter_historicalhealtheconomics_device_created_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    36569 2023-08-23 23:05:23.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0112_alter_historicalhivinitialreview_device_created_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    18776 2023-08-23 23:05:23.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0113_alter_htnreview_device_created_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7314 2023-08-29 02:39:08.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0114_alter_dmmedicationadherence_visual_score_confirmed_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1767 2023-09-22 03:18:09.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0115_remove_historicalnextappointment_best_visit_code_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2860 2023-09-27 00:31:13.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0116_auto_20230920_0058.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1099 2023-10-05 13:55:11.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0117_historicalnextappointment_allow_create_interim_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1302 2023-10-06 00:30:17.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0118_historicalnextappointment_info_source_new_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1070 2023-10-06 00:30:17.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0119_auto_20231006_0220.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      721 2023-10-06 00:30:17.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0120_remove_historicalnextappointment_info_source_new_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      604 2023-10-06 00:30:17.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0121_auto_20231006_0238.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      485 2023-10-06 00:30:17.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0122_remove_historicalnextappointment_info_source_old_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      640 2023-11-16 04:10:04.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0123_alter_subjectvisit_managers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3831 2023-11-16 04:10:04.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0124_auto_20231115_0133.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3919 2023-11-30 05:45:16.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0125_healtheconomicsproperty_calculated_land_surface_area_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2650 2023-11-30 05:45:16.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0126_feat_683_land_area_units.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      993 2023-11-30 05:45:33.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0127_alter_historicalsubjectvisitmissed_appt_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      762 2023-11-30 05:45:33.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0128_remove_historicalsubjectvisit_clinic_services_other_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    27740 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0129_alter_bloodresultsfbc_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2728 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0130_remove_bloodresultsfbc_intecomm_su_subject_1b56bc_idx_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4266 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0131_remove_drugrefillhtn_intecomm_su_subject_33642b_idx_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    73773 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0132_alter_subjectrequisition_unique_together_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7063 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0133_bloodresultsfbc_intecomm_su_subject_3bd165_idx_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    13741 2024-02-01 23:18:18.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0134_clinicalreviewbaseline_intecomm_su_subject_67b2fa_idx_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9514 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0135_hivinitialreview_intecomm_su_subject_a055c4_idx_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4258 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0136_subjectvisit_intecomm_su_modifie_dab86a_idx_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3418 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0137_alter_bloodresultsfbc_platelets_value_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    35161 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0138_alter_bloodresultsfbc_site_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2380 2024-02-01 03:43:59.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0139_alter_bloodresultsins_fasting_duration_minutes_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3869 2024-02-01 16:00:54.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0140_historicalhivreview_drawn_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      768 2024-02-01 16:00:54.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0141_remove_viralloadresult_requisition_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1460 2024-02-06 04:30:17.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0142_alter_historicalhtninitialreview_managed_by_old_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)   143208 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0143_historicalcareseekingb_historicalcareseekinga_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      603 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0144_rename_meds_prescribed_careseekingb_med_prescribed_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2687 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0145_rename_facility_visit_alt_careseekinga_missed_activities_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1013 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0146_rename_seek_inpatient_visits_careseekingb_inpatient_days_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1693 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0147_alter_careseekinga_accompany_num_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2352 2024-02-26 13:27:06.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/0148_alter_bloodresultslft_alp_value_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-03-12 18:03:07.000000 intecomm-edc-0.2.9/intecomm_subject/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.328814 intecomm-edc-0.2.9/intecomm_subject/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      575 2024-02-01 16:00:54.000000 intecomm-edc-0.2.9/intecomm_subject/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4968 2023-08-04 04:50:38.000000 intecomm-edc-0.2.9/intecomm_subject/model_mixins/clinical_review_model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      358 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/model_mixins/crf_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      298 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_subject/model_mixins/crf_with_action_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      559 2023-04-18 01:59:08.000000 intecomm-edc-0.2.9/intecomm_subject/model_mixins/followup_review_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1326 2023-08-23 05:22:45.000000 intecomm-edc-0.2.9/intecomm_subject/model_mixins/medication_adherence_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      296 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_subject/model_mixins/search_slug_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1298 2024-02-01 16:00:54.000000 intecomm-edc-0.2.9/intecomm_subject/model_mixins/viral_load_result_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.336523 intecomm-edc-0.2.9/intecomm_subject/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2166 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      201 2023-12-04 21:40:22.000000 intecomm-edc-0.2.9/intecomm_subject/models/arv_regimens.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.338131 intecomm-edc-0.2.9/intecomm_subject/models/blood_results/
+-rw-r--r--   0 erikvw     (501) staff       (20)      337 2022-11-29 06:19:20.000000 intecomm-edc-0.2.9/intecomm_subject/models/blood_results/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1382 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/blood_results/blood_results_fbc.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1170 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/blood_results/blood_results_glu.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1120 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/blood_results/blood_results_hba1c.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1136 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/blood_results/blood_results_ins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1319 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/blood_results/blood_results_lft.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1252 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/blood_results/blood_results_lipid.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1730 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/blood_results/blood_results_rft.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1143 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/cd4_result.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      727 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/clinical_note.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1065 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/clinical_review.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1133 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/clinical_review_baseline.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4427 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/complications_baseline.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2904 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/complications_followup.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      442 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/concomitant_medication.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1784 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/dm_initial_review.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      508 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/dm_medication_adherence.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      478 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/dm_review.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      653 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/drug_refill_dm.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1502 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/drug_refill_hiv.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      664 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/drug_refill_htn.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      558 2023-12-04 21:42:02.000000 intecomm-edc-0.2.9/intecomm_subject/models/drug_supply_dm.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      616 2023-12-04 21:42:09.000000 intecomm-edc-0.2.9/intecomm_subject/models/drug_supply_hiv.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      572 2023-12-04 21:42:12.000000 intecomm-edc-0.2.9/intecomm_subject/models/drug_supply_htn.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      480 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/eq5d3l.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3595 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/family_history.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      409 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/glucose.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.340765 intecomm-edc-0.2.9/intecomm_subject/models/health_economics/
+-rw-r--r--   0 erikvw     (501) staff       (20)      311 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/models/health_economics/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      673 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/health_economics/assets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    11008 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/models/health_economics/careseeking_a.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    14482 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/models/health_economics/careseeking_b.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      854 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/models/health_economics/checklist.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      764 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/health_economics/household_head.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      611 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/health_economics/income.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      616 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/health_economics/patient.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      621 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/health_economics/property.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    18865 2023-07-10 18:57:10.000000 intecomm-edc-0.2.9/intecomm_subject/models/health_economics_old.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2490 2024-02-01 16:00:54.000000 intecomm-edc-0.2.9/intecomm_subject/models/hiv_initial_review.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      494 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/hiv_medication_adherence.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1162 2024-02-02 02:07:14.000000 intecomm-edc-0.2.9/intecomm_subject/models/hiv_review.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1512 2024-02-06 04:30:17.000000 intecomm-edc-0.2.9/intecomm_subject/models/htn_initial_review.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      521 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/htn_medication_adherence.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1301 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/htn_review.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      371 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/icecapa.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1391 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/location_update.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      463 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/malaria_test.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1567 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/medications.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      498 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/next_appointment.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5408 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/other_baseline_data.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2781 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/patient_history.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1602 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/reason_for_visit.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.343218 intecomm-edc-0.2.9/intecomm_subject/models/social_harms/
+-rw-r--r--   0 erikvw     (501) staff       (20)       38 2023-01-25 03:04:55.000000 intecomm-edc-0.2.9/intecomm_subject/models/social_harms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3281 2023-01-25 03:04:55.000000 intecomm-edc-0.2.9/intecomm_subject/models/social_harms/model_factories.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1220 2023-01-25 03:04:55.000000 intecomm-edc-0.2.9/intecomm_subject/models/social_harms/social_harms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      482 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/subject_requisition.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2345 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_subject/models/subject_visit.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      911 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/subject_visit_missed.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1283 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/urine_dipstick_test.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1290 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/urine_pregnancy.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2449 2023-12-05 05:08:32.000000 intecomm-edc-0.2.9/intecomm_subject/models/vitals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      702 2023-11-13 01:27:15.000000 intecomm-edc-0.2.9/intecomm_subject/reference_model_configs.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.128188 intecomm-edc-0.2.9/intecomm_subject/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.343368 intecomm-edc-0.2.9/intecomm_subject/templates/intecomm_subject/
+-rw-r--r--   0 erikvw     (501) staff       (20)      339 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_subject/templates/intecomm_subject/careseeking_a_instructions.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.343594 intecomm-edc-0.2.9/intecomm_subject/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_subject/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.128412 intecomm-edc-0.2.9/intecomm_subject/tests/etc/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.343687 intecomm-edc-0.2.9/intecomm_subject/tests/etc/community_only/
+-rw-r--r--   0 erikvw     (501) staff       (20)      403 2023-11-19 17:30:45.000000 intecomm-edc-0.2.9/intecomm_subject/tests/etc/community_only/randomization_list.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.343913 intecomm-edc-0.2.9/intecomm_subject/tests/etc/facility_only/
+-rw-r--r--   0 erikvw     (501) staff       (20)      382 2023-11-19 17:30:45.000000 intecomm-edc-0.2.9/intecomm_subject/tests/etc/facility_only/randomization_list.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.345321 intecomm-edc-0.2.9/intecomm_subject/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_subject/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2825 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/intecomm_subject/tests/tests/test_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9854 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_subject/tests/tests/test_appointment.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    17077 2024-02-19 23:54:03.000000 intecomm-edc-0.2.9/intecomm_subject/tests/tests/test_he.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4470 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/intecomm_subject/tests/tests/test_hiv_initial_and_review.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3887 2023-11-21 01:43:28.000000 intecomm-edc-0.2.9/intecomm_subject/tests/tests/test_location_update.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      210 2022-03-14 02:25:40.000000 intecomm-edc-0.2.9/intecomm_subject/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.346272 intecomm-edc-0.2.9/intecomm_visit_schedule/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-07-07 23:18:25.000000 intecomm-edc-0.2.9/intecomm_visit_schedule/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_visit_schedule/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      172 2022-03-12 18:22:09.000000 intecomm-edc-0.2.9/intecomm_visit_schedule/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      193 2023-08-11 03:07:19.000000 intecomm-edc-0.2.9/intecomm_visit_schedule/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.346371 intecomm-edc-0.2.9/intecomm_visit_schedule/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_visit_schedule/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:36:08.000000 intecomm-edc-0.2.9/intecomm_visit_schedule/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.346582 intecomm-edc-0.2.9/intecomm_visit_schedule/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 intecomm-edc-0.2.9/intecomm_visit_schedule/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.346946 intecomm-edc-0.2.9/intecomm_visit_schedule/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:30.000000 intecomm-edc-0.2.9/intecomm_visit_schedule/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       79 2023-08-11 02:54:06.000000 intecomm-edc-0.2.9/intecomm_visit_schedule/tests/tests/test_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      113 2023-10-10 05:14:41.000000 intecomm-edc-0.2.9/intecomm_visit_schedule/tests/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-02-26 13:27:16.348454 intecomm-edc-0.2.9/intecomm_visit_schedule/visit_schedules/
+-rw-r--r--   0 erikvw     (501) staff       (20)      234 2023-10-10 05:14:41.000000 intecomm-edc-0.2.9/intecomm_visit_schedule/visit_schedules/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      743 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_visit_schedule/visit_schedules/community_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7289 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_visit_schedule/visit_schedules/crfs.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      765 2024-01-25 06:13:02.000000 intecomm-edc-0.2.9/intecomm_visit_schedule/visit_schedules/facility_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1190 2024-02-01 16:00:54.000000 intecomm-edc-0.2.9/intecomm_visit_schedule/visit_schedules/requisitions.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      606 2023-10-10 05:14:41.000000 intecomm-edc-0.2.9/intecomm_visit_schedule/visit_schedules/visit_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3171 2024-02-26 13:01:14.000000 intecomm-edc-0.2.9/intecomm_visit_schedule/visit_schedules/visits.py
+-rwxr-xr-x   0 erikvw     (501) staff       (20)      789 2021-11-22 15:06:01.000000 intecomm-edc-0.2.9/manage.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1960 2023-12-15 04:21:25.000000 intecomm-edc-0.2.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     8293 2024-01-29 06:51:01.000000 intecomm-edc-0.2.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1295 2024-02-26 13:27:16.349523 intecomm-edc-0.2.9/setup.cfg
```

### Comparing `intecomm-edc-0.2.8/.github/workflows/build.yml` & `intecomm-edc-0.2.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/.gitignore` & `intecomm-edc-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/.pre-commit-config.yaml` & `intecomm-edc-0.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/CHANGES` & `intecomm-edc-0.2.9/CHANGES`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/LICENSE` & `intecomm-edc-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/PKG-INFO` & `intecomm-edc-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intecomm-edc
-Version: 0.2.8
+Version: 0.2.9
 Summary: INTECOMM Trial EDC (http://www.isrctn.com/ISRCTN76157257)
 Home-page: https://github.com/intecomm-trial/intecomm-edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc INTECOMM EDC,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: edc==0.5.69
+Requires-Dist: edc==0.5.70
 Requires-Dist: beautifulsoup4
 Requires-Dist: intecomm-eligibility==0.1.10
 Requires-Dist: intecomm-form-validators==0.1.53
 Requires-Dist: intecomm-rando==0.1.24
 Requires-Dist: edc_microscopy
 
 |pypi| |actions| |codecov| |downloads|
```

### Comparing `intecomm-edc-0.2.8/README.rst` & `intecomm-edc-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/bin/nginx/conf/intecomm_live.conf` & `intecomm-edc-0.2.9/bin/nginx/conf/intecomm_live.conf`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/bin/nginx/conf/intecomm_uat.conf` & `intecomm-edc-0.2.9/bin/nginx/conf/intecomm_uat.conf`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/bin/nginx/www/html/live.intecomm.clinicedc.org/index.html` & `intecomm-edc-0.2.9/bin/nginx/www/html/live.intecomm.clinicedc.org/index.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/bin/nginx/www/html/live.intecomm.clinicedc.org/tz/index.html` & `intecomm-edc-0.2.9/bin/nginx/www/html/live.intecomm.clinicedc.org/tz/index.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/bin/nginx/www/html/live.intecomm.clinicedc.org/ug/index.html` & `intecomm-edc-0.2.9/bin/nginx/www/html/live.intecomm.clinicedc.org/ug/index.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/bin/nginx/www/html/uat.intecomm.clinicedc.org/index.html` & `intecomm-edc-0.2.9/bin/nginx/www/html/uat.intecomm.clinicedc.org/index.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/bin/nginx/www/html/uat.intecomm.clinicedc.org/tz/index.html` & `intecomm-edc-0.2.9/bin/nginx/www/html/uat.intecomm.clinicedc.org/tz/index.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/bin/nginx/www/html/uat.intecomm.clinicedc.org/ug/index.html` & `intecomm-edc-0.2.9/bin/nginx/www/html/uat.intecomm.clinicedc.org/ug/index.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/env.sample` & `intecomm-edc-0.2.9/env.sample`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/holidays.csv` & `intecomm-edc-0.2.9/holidays.csv`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/action_items.py` & `intecomm-edc-0.2.9/intecomm_ae/action_items.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/admin/ae_followup_admin.py` & `intecomm-edc-0.2.9/intecomm_ae/admin/ae_followup_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/admin/ae_initial_admin.py` & `intecomm-edc-0.2.9/intecomm_ae/admin/ae_initial_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/admin/death_report_admin.py` & `intecomm-edc-0.2.9/intecomm_ae/admin/death_report_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/admin/hospitalization_admin.py` & `intecomm-edc-0.2.9/intecomm_ae/admin/hospitalization_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/baker_recipes.py` & `intecomm-edc-0.2.9/intecomm_ae/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/choices.py` & `intecomm-edc-0.2.9/intecomm_ae/choices.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/forms/ae_initial_form.py` & `intecomm-edc-0.2.9/intecomm_ae/forms/ae_initial_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/forms/death_report_form.py` & `intecomm-edc-0.2.9/intecomm_ae/forms/death_report_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/forms/modelform_mixins.py` & `intecomm-edc-0.2.9/intecomm_ae/forms/modelform_mixins.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/list_data.py` & `intecomm-edc-0.2.9/intecomm_ae/list_data.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/migrations/0001_initial.py` & `intecomm-edc-0.2.9/intecomm_ae/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/migrations/0002_rename_narrative_aetmg_investigator_narrative_and_more.py` & `intecomm-edc-0.2.9/intecomm_ae/migrations/0002_rename_narrative_aetmg_investigator_narrative_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/migrations/0003_alter_deathreporttmg_cause_of_death_agreed_and_more.py` & `intecomm-edc-0.2.9/intecomm_ae/migrations/0003_alter_deathreporttmg_cause_of_death_agreed_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/migrations/0004_alter_aefollowup_options_alter_aeinitial_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_ae/migrations/0004_alter_aefollowup_options_alter_aeinitial_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/migrations/0005_alter_aefollowup_managers_alter_aeinitial_managers_and_more.py` & `intecomm-edc-0.2.9/intecomm_ae/migrations/0005_alter_aefollowup_managers_alter_aeinitial_managers_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/migrations/0006_hospitalization_historicalhospitalization.py` & `intecomm-edc-0.2.9/intecomm_ae/migrations/0006_hospitalization_historicalhospitalization.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/migrations/0007_aeinitial_ae_classification_as_text_and_more.py` & `intecomm-edc-0.2.9/intecomm_ae/migrations/0007_aeinitial_ae_classification_as_text_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/migrations/0008_alter_deathreporttmgsecond_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_ae/migrations/0008_alter_deathreporttmgsecond_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/migrations/0009_alter_aefollowup_device_created_and_more.py` & `intecomm-edc-0.2.9/intecomm_ae/migrations/0009_alter_aefollowup_device_created_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/migrations/0010_alter_deathreport_death_date_and_more.py` & `intecomm-edc-0.2.9/intecomm_ae/migrations/0010_alter_deathreport_death_date_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/migrations/0011_alter_aefollowup_options_alter_aeinitial_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_ae/migrations/0011_alter_aefollowup_options_alter_aeinitial_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/migrations/0012_aefollowup_intecomm_ae_subject_a0869e_idx_and_more.py` & `intecomm-edc-0.2.9/intecomm_ae/migrations/0012_aefollowup_intecomm_ae_subject_a0869e_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/migrations/0013_aetmg_intecomm_ae_subject_a182a3_idx_and_more.py` & `intecomm-edc-0.2.9/intecomm_ae/migrations/0013_aetmg_intecomm_ae_subject_a182a3_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/migrations/0014_alter_aefollowup_site_alter_aeinitial_site_and_more.py` & `intecomm-edc-0.2.9/intecomm_ae/migrations/0014_alter_aefollowup_site_alter_aeinitial_site_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/model_mixins/ae_review_model_mixin.py` & `intecomm-edc-0.2.9/intecomm_ae/model_mixins/ae_review_model_mixin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/models/ae_initial.py` & `intecomm-edc-0.2.9/intecomm_ae/models/ae_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/models/compatability.py` & `intecomm-edc-0.2.9/intecomm_ae/models/compatability.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/models/death_report.py` & `intecomm-edc-0.2.9/intecomm_ae/models/death_report.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/models/hospitalization.py` & `intecomm-edc-0.2.9/intecomm_ae/models/hospitalization.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/models/managers.py` & `intecomm-edc-0.2.9/intecomm_ae/models/managers.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/pdf_reports/ae_pdf_report.py` & `intecomm-edc-0.2.9/intecomm_ae/pdf_reports/ae_pdf_report.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/pdf_reports/death_pdf_report.py` & `intecomm-edc-0.2.9/intecomm_ae/pdf_reports/death_pdf_report.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/templates/intecomm_ae/bootstrap3/ae_initial_description.html` & `intecomm-edc-0.2.9/intecomm_ae/templates/intecomm_ae/bootstrap3/ae_initial_description.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/templatetags/protocol_ae_extras.py` & `intecomm-edc-0.2.9/intecomm_ae/templatetags/protocol_ae_extras.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_ae/tests/holidays.csv` & `intecomm-edc-0.2.9/intecomm_ae/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_auth/auth_objects.py` & `intecomm-edc-0.2.9/intecomm_auth/auth_objects.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_auth/auths.py` & `intecomm-edc-0.2.9/intecomm_auth/auths.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_auth/tests/tests/test_auths.py` & `intecomm-edc-0.2.9/intecomm_auth/tests/tests/test_auths.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/admin/fieldsets.py` & `intecomm-edc-0.2.9/intecomm_consent/admin/fieldsets.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/admin/modeladmin_mixins.py` & `intecomm-edc-0.2.9/intecomm_consent/admin/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/admin/subject_consent_tz_admin.py` & `intecomm-edc-0.2.9/intecomm_consent/admin/subject_consent_tz_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/admin/subject_consent_ug_admin.py` & `intecomm-edc-0.2.9/intecomm_consent/admin/subject_consent_ug_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/admin_site.py` & `intecomm-edc-0.2.9/intecomm_consent/admin_site.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/baker_recipes.py` & `intecomm-edc-0.2.9/intecomm_consent/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/consents.py` & `intecomm-edc-0.2.9/intecomm_consent/consents.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/forms/modelform_mixins.py` & `intecomm-edc-0.2.9/intecomm_consent/forms/modelform_mixins.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0001_initial.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0002_remove_subjectconsent_intecomm_co_subject_145905_idx_and_more.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0002_remove_subjectconsent_intecomm_co_subject_145905_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0003_alter_historicalsubjectconsent_language_and_more.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0003_alter_historicalsubjectconsent_language_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0004_alter_historicalsubjectconsent_familiar_name_and_more.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0004_alter_historicalsubjectconsent_familiar_name_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0005_remove_subjectconsent_unique_consent_subject_id_and_version_and_more.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0005_remove_subjectconsent_unique_consent_subject_id_and_version_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0006_historicalsubjectconsent_group_identifier_and_more.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0006_historicalsubjectconsent_group_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0007_alter_historicalsubjectconsent_language_and_more.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0007_alter_historicalsubjectconsent_language_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0008_alter_historicalsubjectconsent_screening_identifier_and_more.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0008_alter_historicalsubjectconsent_screening_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0009_alter_subjectconsent_options.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0009_alter_subjectconsent_options.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0010_alter_subjectreconsent_options.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0010_alter_subjectreconsent_options.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0011_alter_subjectconsent_unique_together_and_more.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0011_alter_subjectconsent_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0012_alter_historicalsubjectconsent_device_created_and_more.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0012_alter_historicalsubjectconsent_device_created_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0013_subjectconsentug.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0013_subjectconsentug.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0015_historicalsubjectconsentug.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0015_historicalsubjectconsentug.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0016_alter_historicalsubjectconsent_language_and_more.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0016_alter_historicalsubjectconsent_language_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0017_alter_subjectconsent_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0017_alter_subjectconsent_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0018_subjectconsent_intecomm_co_modifie_45691e_idx_and_more.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0018_subjectconsent_intecomm_co_modifie_45691e_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0019_historicalsubjectconsent_model_name_and_more.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0019_historicalsubjectconsent_model_name_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0020_auto_20240111_0115.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0020_auto_20240111_0115.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0021_remove_subjectreconsent_action_item_and_more.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0021_remove_subjectreconsent_action_item_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0022_subjectconsenttz_historicalsubjectconsenttz.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0022_subjectconsenttz_historicalsubjectconsenttz.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/migrations/0023_alter_subjectconsent_managers.py` & `intecomm-edc-0.2.9/intecomm_consent/migrations/0023_alter_subjectconsent_managers.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/models/signals.py` & `intecomm-edc-0.2.9/intecomm_consent/models/signals.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/models/subject_consent.py` & `intecomm-edc-0.2.9/intecomm_consent/models/subject_consent.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/templates/intecomm_consent/admin/subjectconsent_change_list.html` & `intecomm-edc-0.2.9/intecomm_consent/templates/intecomm_consent/admin/subjectconsent_change_list.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/tests/holidays.csv` & `intecomm-edc-0.2.9/intecomm_consent/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/tests/tests/test_subject_consent.py` & `intecomm-edc-0.2.9/intecomm_consent/tests/tests/test_subject_consent.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/tests/tests/test_webtest.py` & `intecomm-edc-0.2.9/intecomm_consent/tests/tests/test_webtest.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/tests/urls.py` & `intecomm-edc-0.2.9/intecomm_consent/tests/urls.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_consent/utils.py` & `intecomm-edc-0.2.9/intecomm_consent/utils.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_dashboard/navbars.py` & `intecomm-edc-0.2.9/intecomm_dashboard/navbars.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/changelist_topbar.html` & `intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/changelist_topbar.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/screening/listboard.html` & `intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/screening/listboard.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/buttons_column.html` & `intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/buttons_column.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/dashboard.html` & `intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/dashboard.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/subject_listboard.html` & `intecomm-edc-0.2.9/intecomm_dashboard/templates/intecomm_dashboard/bootstrap3/subject/subject_listboard.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_dashboard/templatetags/protocol_dashboard_extras.py` & `intecomm-edc-0.2.9/intecomm_dashboard/templatetags/protocol_dashboard_extras.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_dashboard/tests/admin.py` & `intecomm-edc-0.2.9/intecomm_dashboard/tests/admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_dashboard/tests/holidays.csv` & `intecomm-edc-0.2.9/intecomm_dashboard/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_dashboard/tests/tests/test_views.py` & `intecomm-edc-0.2.9/intecomm_dashboard/tests/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_dashboard/tests/urls.py` & `intecomm-edc-0.2.9/intecomm_dashboard/tests/urls.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_dashboard/urls.py` & `intecomm-edc-0.2.9/intecomm_dashboard/urls.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_dashboard/views/screening/listboard_view.py` & `intecomm-edc-0.2.9/intecomm_dashboard/views/screening/listboard_view.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_dashboard/views/subject/subject_dashboard_view.py` & `intecomm-edc-0.2.9/intecomm_dashboard/views/subject/subject_dashboard_view.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_dashboard/views/subject/subject_listboard_view.py` & `intecomm-edc-0.2.9/intecomm_dashboard/views/subject/subject_listboard_view.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_edc/admin.py` & `intecomm-edc-0.2.9/intecomm_edc/admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_edc/management/commands/update_forms_reference.py` & `intecomm-edc-0.2.9/intecomm_edc/management/commands/update_forms_reference.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_edc/navbars.py` & `intecomm-edc-0.2.9/intecomm_edc/navbars.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_edc/settings/debug.py` & `intecomm-edc-0.2.9/intecomm_edc/settings/debug.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_edc/settings/defaults.py` & `intecomm-edc-0.2.9/intecomm_edc/settings/defaults.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_edc/settings/live.py` & `intecomm-edc-0.2.9/intecomm_edc/settings/live.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_edc/settings/logging.py` & `intecomm-edc-0.2.9/intecomm_edc/settings/logging.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_edc/settings/minimal.py` & `intecomm-edc-0.2.9/intecomm_edc/settings/minimal.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_edc/settings/uat.py` & `intecomm-edc-0.2.9/intecomm_edc/settings/uat.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_edc/templates/intecomm_edc/bootstrap3/followup_community.html` & `intecomm-edc-0.2.9/intecomm_edc/templates/intecomm_edc/bootstrap3/followup_community.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_edc/templates/intecomm_edc/bootstrap3/grouping.html` & `intecomm-edc-0.2.9/intecomm_edc/templates/intecomm_edc/bootstrap3/grouping.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_edc/templates/intecomm_edc/bootstrap3/home.html` & `intecomm-edc-0.2.9/intecomm_edc/templates/intecomm_edc/bootstrap3/home.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_edc/templates/intecomm_edc/bootstrap3/subjects_home.html` & `intecomm-edc-0.2.9/intecomm_edc/templates/intecomm_edc/bootstrap3/subjects_home.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_edc/tests/etc/randomization_list.csv` & `intecomm-edc-0.2.9/intecomm_edc/tests/etc/randomization_list.csv`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_edc/tests/etc/user-rsa-local-private.pem` & `intecomm-edc-0.2.9/intecomm_edc/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_edc/tests/etc/user-rsa-restricted-private.pem` & `intecomm-edc-0.2.9/intecomm_edc/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_edc/urls.py` & `intecomm-edc-0.2.9/intecomm_edc/urls.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_edc/views/subjects_home_view.py` & `intecomm-edc-0.2.9/intecomm_edc/views/subjects_home_view.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_edc.egg-info/PKG-INFO` & `intecomm-edc-0.2.9/intecomm_edc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intecomm-edc
-Version: 0.2.8
+Version: 0.2.9
 Summary: INTECOMM Trial EDC (http://www.isrctn.com/ISRCTN76157257)
 Home-page: https://github.com/intecomm-trial/intecomm-edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc INTECOMM EDC,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: edc==0.5.69
+Requires-Dist: edc==0.5.70
 Requires-Dist: beautifulsoup4
 Requires-Dist: intecomm-eligibility==0.1.10
 Requires-Dist: intecomm-form-validators==0.1.53
 Requires-Dist: intecomm-rando==0.1.24
 Requires-Dist: edc_microscopy
 
 |pypi| |actions| |codecov| |downloads|
```

### Comparing `intecomm-edc-0.2.8/intecomm_edc.egg-info/SOURCES.txt` & `intecomm-edc-0.2.9/intecomm_edc.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -872,14 +872,15 @@
 intecomm_subject/migrations/0141_remove_viralloadresult_requisition_and_more.py
 intecomm_subject/migrations/0142_alter_historicalhtninitialreview_managed_by_old_and_more.py
 intecomm_subject/migrations/0143_historicalcareseekingb_historicalcareseekinga_and_more.py
 intecomm_subject/migrations/0144_rename_meds_prescribed_careseekingb_med_prescribed_and_more.py
 intecomm_subject/migrations/0145_rename_facility_visit_alt_careseekinga_missed_activities_and_more.py
 intecomm_subject/migrations/0146_rename_seek_inpatient_visits_careseekingb_inpatient_days_and_more.py
 intecomm_subject/migrations/0147_alter_careseekinga_accompany_num_and_more.py
+intecomm_subject/migrations/0148_alter_bloodresultslft_alp_value_and_more.py
 intecomm_subject/migrations/__init__.py
 intecomm_subject/model_mixins/__init__.py
 intecomm_subject/model_mixins/clinical_review_model_mixins.py
 intecomm_subject/model_mixins/crf_model_mixin.py
 intecomm_subject/model_mixins/crf_with_action_model_mixin.py
 intecomm_subject/model_mixins/followup_review_model_mixin.py
 intecomm_subject/model_mixins/medication_adherence_model_mixin.py
```

### Comparing `intecomm-edc-0.2.8/intecomm_facility/admin.py` & `intecomm-edc-0.2.9/intecomm_facility/admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_facility/migrations/0001_initial.py` & `intecomm-edc-0.2.9/intecomm_facility/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_facility/migrations/0002_alter_healthfacility_device_created_and_more.py` & `intecomm-edc-0.2.9/intecomm_facility/migrations/0002_alter_healthfacility_device_created_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_facility/migrations/0003_auto_20230726_2030.py` & `intecomm-edc-0.2.9/intecomm_facility/migrations/0003_auto_20230726_2030.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_facility/migrations/0004_alter_healthfacility_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_facility/migrations/0004_alter_healthfacility_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_facility/migrations/0005_alter_healthfacility_site_and_more.py` & `intecomm-edc-0.2.9/intecomm_facility/migrations/0005_alter_healthfacility_site_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_facility/models.py` & `intecomm-edc-0.2.9/intecomm_facility/models.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/admin/community_care_location_admin.py` & `intecomm-edc-0.2.9/intecomm_group/admin/community_care_location_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/admin/patient_followup_call_admin.py` & `intecomm-edc-0.2.9/intecomm_group/admin/patient_followup_call_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/admin/patient_group_admin.py` & `intecomm-edc-0.2.9/intecomm_group/admin/patient_group_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/admin/patient_group_appointment_admin.py` & `intecomm-edc-0.2.9/intecomm_group/admin/patient_group_appointment_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/admin/patient_group_meeting_admin.py` & `intecomm-edc-0.2.9/intecomm_group/admin/patient_group_meeting_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/choices.py` & `intecomm-edc-0.2.9/intecomm_group/choices.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/migrations/0001_initial.py` & `intecomm-edc-0.2.9/intecomm_group/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/migrations/0002_initial.py` & `intecomm-edc-0.2.9/intecomm_group/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/migrations/0003_alter_historicalpatientgroup_group_identifier_and_more.py` & `intecomm-edc-0.2.9/intecomm_group/migrations/0003_alter_historicalpatientgroup_group_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/migrations/0004_alter_patientgroup_patients.py` & `intecomm-edc-0.2.9/intecomm_group/migrations/0004_alter_patientgroup_patients.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/migrations/0005_patientfollowupcall_historicalpatientfollowupcall.py` & `intecomm-edc-0.2.9/intecomm_group/migrations/0005_patientfollowupcall_historicalpatientfollowupcall.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/migrations/0006_remove_historicalpatientgroup_enforce_group_size_min_and_more.py` & `intecomm-edc-0.2.9/intecomm_group/migrations/0006_remove_historicalpatientgroup_enforce_group_size_min_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/migrations/0007_remove_historicalpatientfollowupcall_attend_date_and_more.py` & `intecomm-edc-0.2.9/intecomm_group/migrations/0007_remove_historicalpatientfollowupcall_attend_date_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/migrations/0008_patientgroup_dm_patients_patientgroup_hiv_patients_and_more.py` & `intecomm-edc-0.2.9/intecomm_group/migrations/0008_patientgroup_dm_patients_patientgroup_hiv_patients_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/migrations/0009_auto_20221126_0358.py` & `intecomm-edc-0.2.9/intecomm_group/migrations/0009_auto_20221126_0358.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/migrations/0010_alter_patientgroup_managers.py` & `intecomm-edc-0.2.9/intecomm_group/migrations/0010_alter_patientgroup_managers.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/migrations/0011_alter_historicalpatientfollowupcall_respondent_and_more.py` & `intecomm-edc-0.2.9/intecomm_group/migrations/0011_alter_historicalpatientfollowupcall_respondent_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/migrations/0012_alter_historicalpatientgroup_status_and_more.py` & `intecomm-edc-0.2.9/intecomm_group/migrations/0012_alter_historicalpatientgroup_status_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/migrations/0013_alter_historicalpatientgroup_status_and_more.py` & `intecomm-edc-0.2.9/intecomm_group/migrations/0013_alter_historicalpatientgroup_status_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/migrations/0014_alter_communitycarelocation_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_group/migrations/0014_alter_communitycarelocation_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/migrations/0015_alter_patientgroupmeeting_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_group/migrations/0015_alter_patientgroupmeeting_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/migrations/0016_alter_communitycarelocation_device_created_and_more.py` & `intecomm-edc-0.2.9/intecomm_group/migrations/0016_alter_communitycarelocation_device_created_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/migrations/0017_alter_communitycarelocation_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_group/migrations/0017_alter_communitycarelocation_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/migrations/0018_alter_communitycarelocation_site_and_more.py` & `intecomm-edc-0.2.9/intecomm_group/migrations/0018_alter_communitycarelocation_site_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/models/__init__.py` & `intecomm-edc-0.2.9/intecomm_group/models/__init__.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/models/community_care_location.py` & `intecomm-edc-0.2.9/intecomm_group/models/community_care_location.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/models/patient_followup_call.py` & `intecomm-edc-0.2.9/intecomm_group/models/patient_followup_call.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/models/patient_group.py` & `intecomm-edc-0.2.9/intecomm_group/models/patient_group.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/models/patient_group_appointment.py` & `intecomm-edc-0.2.9/intecomm_group/models/patient_group_appointment.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/models/patient_group_meeting.py` & `intecomm-edc-0.2.9/intecomm_group/models/patient_group_meeting.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/models/signals.py` & `intecomm-edc-0.2.9/intecomm_group/models/signals.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/models/utils.py` & `intecomm-edc-0.2.9/intecomm_group/models/utils.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/patient_group_updater.py` & `intecomm-edc-0.2.9/intecomm_group/patient_group_updater.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/templates/intecomm_group/admin/communitycarelocation_change_list.html` & `intecomm-edc-0.2.9/intecomm_group/templates/intecomm_group/admin/communitycarelocation_change_list.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/templates/intecomm_group/admin/patientfollowupcall_change_list.html` & `intecomm-edc-0.2.9/intecomm_group/templates/intecomm_group/admin/patientfollowupcall_change_list.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/templates/intecomm_group/admin/patientgroup_change_list.html` & `intecomm-edc-0.2.9/intecomm_group/templates/intecomm_group/admin/patientgroup_change_list.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/templates/intecomm_group/admin/patientgroupappointment_change_list.html` & `intecomm-edc-0.2.9/intecomm_group/templates/intecomm_group/admin/patientgroupappointment_change_list.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/templates/intecomm_group/admin/patientgroupmeeting_change_list.html` & `intecomm-edc-0.2.9/intecomm_group/templates/intecomm_group/admin/patientgroupmeeting_change_list.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/templates/intecomm_group/patient_followup_call_summary.html` & `intecomm-edc-0.2.9/intecomm_group/templates/intecomm_group/patient_followup_call_summary.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/tests/holidays.csv` & `intecomm-edc-0.2.9/intecomm_group/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/tests/tests/test_add_subjects_after_rando.py` & `intecomm-edc-0.2.9/intecomm_group/tests/tests/test_add_subjects_after_rando.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_group/utils.py` & `intecomm-edc-0.2.9/intecomm_group/utils.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_labs/lab_profiles.py` & `intecomm-edc-0.2.9/intecomm_labs/lab_profiles.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_labs/reportables.py` & `intecomm-edc-0.2.9/intecomm_labs/reportables.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_labs/tests/tests/test_labs.py` & `intecomm-edc-0.2.9/intecomm_labs/tests/tests/test_labs.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_labs/tests/tests/test_reportables.py` & `intecomm-edc-0.2.9/intecomm_labs/tests/tests/test_reportables.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_lists/admin.py` & `intecomm-edc-0.2.9/intecomm_lists/admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_lists/choices.py` & `intecomm-edc-0.2.9/intecomm_lists/choices.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_lists/list_data.py` & `intecomm-edc-0.2.9/intecomm_lists/list_data.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_lists/migrations/0001_initial.py` & `intecomm-edc-0.2.9/intecomm_lists/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_lists/migrations/0003_dmmanagement_dmmanagement_intecomm_li_id_b4d41f_idx.py` & `intecomm-edc-0.2.9/intecomm_lists/migrations/0003_dmmanagement_dmmanagement_intecomm_li_id_b4d41f_idx.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_lists/migrations/0004_rxmodificationreasons_rxmodifications_and_more.py` & `intecomm-edc-0.2.9/intecomm_lists/migrations/0004_rxmodificationreasons_rxmodifications_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_lists/migrations/0005_htnmanagement_and_more.py` & `intecomm-edc-0.2.9/intecomm_lists/migrations/0005_htnmanagement_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_lists/migrations/0006_consentrefusalreasons_screeningrefusalreasons_and_more.py` & `intecomm-edc-0.2.9/intecomm_lists/migrations/0006_consentrefusalreasons_screeningrefusalreasons_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_lists/migrations/0007_arvdrugs_extra_value_arvregimens_extra_value_and_more.py` & `intecomm-edc-0.2.9/intecomm_lists/migrations/0007_arvdrugs_extra_value_arvregimens_extra_value_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_lists/migrations/0008_medicationshortagereasons.py` & `intecomm-edc-0.2.9/intecomm_lists/migrations/0008_medicationshortagereasons.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_lists/migrations/0009_alter_arvdrugs_options_alter_arvregimens_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_lists/migrations/0009_alter_arvdrugs_options_alter_arvregimens_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_lists/migrations/0010_remove_arvdrugs_intecomm_li_name_b55bdc_idx_and_more.py` & `intecomm-edc-0.2.9/intecomm_lists/migrations/0010_remove_arvdrugs_intecomm_li_name_b55bdc_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_lists/migrations/0011_accompanied_moneysources_travelmethods.py` & `intecomm-edc-0.2.9/intecomm_lists/migrations/0011_accompanied_moneysources_travelmethods.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_lists/migrations/0012_visitreasons_custom_name.py` & `intecomm-edc-0.2.9/intecomm_lists/migrations/0012_visitreasons_custom_name.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_lists/models.py` & `intecomm-edc-0.2.9/intecomm_lists/models.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/action_items.py` & `intecomm-edc-0.2.9/intecomm_prn/action_items.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/admin/end_of_study_admin.py` & `intecomm-edc-0.2.9/intecomm_prn/admin/end_of_study_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/admin/loss_to_followup_admin.py` & `intecomm-edc-0.2.9/intecomm_prn/admin/loss_to_followup_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/admin/modeladmin_mixins.py` & `intecomm-edc-0.2.9/intecomm_prn/admin/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/admin/offschedule_comm_admin.py` & `intecomm-edc-0.2.9/intecomm_prn/admin/offschedule_comm_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/admin/offschedule_inte_admin.py` & `intecomm-edc-0.2.9/intecomm_prn/admin/offschedule_inte_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/admin/protocol_incident_admin.py` & `intecomm-edc-0.2.9/intecomm_prn/admin/protocol_incident_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/admin/subject_locator_admin.py` & `intecomm-edc-0.2.9/intecomm_prn/admin/subject_locator_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/admin/subject_transfer_admin.py` & `intecomm-edc-0.2.9/intecomm_prn/admin/subject_transfer_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/choices.py` & `intecomm-edc-0.2.9/intecomm_prn/choices.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/forms/end_of_study_form.py` & `intecomm-edc-0.2.9/intecomm_prn/forms/end_of_study_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/forms/loss_to_followup_form.py` & `intecomm-edc-0.2.9/intecomm_prn/forms/loss_to_followup_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/forms/offschedule_comm_form.py` & `intecomm-edc-0.2.9/intecomm_prn/forms/offschedule_comm_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/forms/offschedule_inte_form.py` & `intecomm-edc-0.2.9/intecomm_prn/forms/offschedule_inte_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/forms/onschedule_comm_form.py` & `intecomm-edc-0.2.9/intecomm_prn/forms/onschedule_comm_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/forms/onschedule_inte_form.py` & `intecomm-edc-0.2.9/intecomm_prn/forms/onschedule_inte_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/forms/subject_locator_form.py` & `intecomm-edc-0.2.9/intecomm_prn/forms/subject_locator_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/forms/subject_transfer_form.py` & `intecomm-edc-0.2.9/intecomm_prn/forms/subject_transfer_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/list_data.py` & `intecomm-edc-0.2.9/intecomm_prn/list_data.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/migrations/0001_initial.py` & `intecomm-edc-0.2.9/intecomm_prn/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/migrations/0002_remove_endofstudy_delivery_date_and_more.py` & `intecomm-edc-0.2.9/intecomm_prn/migrations/0002_remove_endofstudy_delivery_date_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/migrations/0003_historicalprotocolincident_reasons_withdrawn_and_more.py` & `intecomm-edc-0.2.9/intecomm_prn/migrations/0003_historicalprotocolincident_reasons_withdrawn_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/migrations/0004_rename_historicaloffschedulebaseline_historicaloffschedulecomm_and_more.py` & `intecomm-edc-0.2.9/intecomm_prn/migrations/0004_rename_historicaloffschedulebaseline_historicaloffschedulecomm_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/migrations/0005_rename_historicaloffschedulefollowup_historicaloffscheduleinte_and_more.py` & `intecomm-edc-0.2.9/intecomm_prn/migrations/0005_rename_historicaloffschedulefollowup_historicaloffscheduleinte_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/migrations/0006_alter_historicaloffschedulecomm_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_prn/migrations/0006_alter_historicaloffschedulecomm_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/migrations/0007_alter_losstofollowup_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_prn/migrations/0007_alter_losstofollowup_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/migrations/0008_alter_endofstudy_options.py` & `intecomm-edc-0.2.9/intecomm_prn/migrations/0008_alter_endofstudy_options.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/migrations/0009_subjectlocator_and_more.py` & `intecomm-edc-0.2.9/intecomm_prn/migrations/0009_subjectlocator_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/migrations/0010_alter_historicalsubjectlocator_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_prn/migrations/0010_alter_historicalsubjectlocator_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/migrations/0011_alter_endofstudy_device_created_and_more.py` & `intecomm-edc-0.2.9/intecomm_prn/migrations/0011_alter_endofstudy_device_created_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/migrations/0012_alter_endofstudy_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_prn/migrations/0012_alter_endofstudy_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/migrations/0013_endofstudy_locale_created_endofstudy_locale_modified_and_more.py` & `intecomm-edc-0.2.9/intecomm_prn/migrations/0013_endofstudy_locale_created_endofstudy_locale_modified_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/migrations/0014_endofstudy_intecomm_pr_action__f3bf58_idx_and_more.py` & `intecomm-edc-0.2.9/intecomm_prn/migrations/0014_endofstudy_intecomm_pr_action__f3bf58_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/migrations/0015_protocolincident_intecomm_pr_subject_54092b_idx_and_more.py` & `intecomm-edc-0.2.9/intecomm_prn/migrations/0015_protocolincident_intecomm_pr_subject_54092b_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/migrations/0016_alter_endofstudy_site_and_more.py` & `intecomm-edc-0.2.9/intecomm_prn/migrations/0016_alter_endofstudy_site_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/models/end_of_study.py` & `intecomm-edc-0.2.9/intecomm_prn/models/end_of_study.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/models/loss_to_followup.py` & `intecomm-edc-0.2.9/intecomm_prn/models/loss_to_followup.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/models/offschedule_comm.py` & `intecomm-edc-0.2.9/intecomm_prn/models/offschedule_comm.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/models/offschedule_inte.py` & `intecomm-edc-0.2.9/intecomm_prn/models/offschedule_inte.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/models/onschedule_comm.py` & `intecomm-edc-0.2.9/intecomm_prn/models/onschedule_comm.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/models/onschedule_inte.py` & `intecomm-edc-0.2.9/intecomm_prn/models/onschedule_inte.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/models/protocol_incident.py` & `intecomm-edc-0.2.9/intecomm_prn/models/protocol_incident.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_prn/templates/intecomm_prn/changelist_locator_contacts.html` & `intecomm-edc-0.2.9/intecomm_prn/templates/intecomm_prn/changelist_locator_contacts.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/__init__.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/actions.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/actions.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/consent_refusal_admin.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/consent_refusal_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/health_facility_admin.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/health_facility_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/health_talk_log_admin.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/health_talk_log_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/list_filters.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/list_filters.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/modeladmin_mixins.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/patient_call_admin.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/patient_call_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/patient_call_inlines.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/patient_call_inlines.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/patient_group_admin.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/patient_group_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/patient_group_rando_admin.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/patient_group_rando_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/patient_log/change_list_template_context.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/patient_log/change_list_template_context.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/patient_log/fieldsets.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/patient_log/fieldsets.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/patient_log/get_search_fields.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/patient_log/get_search_fields.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/patient_log/modeladmin_mixins.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/patient_log/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/patient_log/patient_log_admin.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/patient_log/patient_log_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/patient_log/patient_log_ug_admin.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/patient_log/patient_log_ug_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/patient_log_report_print_history_admin.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/patient_log_report_print_history_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/subject_screening/fieldsets.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/subject_screening/fieldsets.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/subject_screening/modeladmin_mixins.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/subject_screening/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/subject_screening/subject_screening_admin.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/subject_screening/subject_screening_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/subject_screening/subject_screening_tz_admin.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/subject_screening/subject_screening_tz_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin/subject_screening/subject_screening_ug_admin.py` & `intecomm-edc-0.2.9/intecomm_screening/admin/subject_screening/subject_screening_ug_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/admin_site.py` & `intecomm-edc-0.2.9/intecomm_screening/admin_site.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/apps.py` & `intecomm-edc-0.2.9/intecomm_screening/apps.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/auth_objects.py` & `intecomm-edc-0.2.9/intecomm_screening/auth_objects.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/baker_recipes.py` & `intecomm-edc-0.2.9/intecomm_screening/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/forms/consent_refusal_form.py` & `intecomm-edc-0.2.9/intecomm_screening/forms/consent_refusal_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/forms/patient_group_form.py` & `intecomm-edc-0.2.9/intecomm_screening/forms/patient_group_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/forms/patient_group_rando_form.py` & `intecomm-edc-0.2.9/intecomm_screening/forms/patient_group_rando_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/forms/patient_log/patient_log_form.py` & `intecomm-edc-0.2.9/intecomm_screening/forms/patient_log/patient_log_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/forms/patient_log/patient_log_ug_form.py` & `intecomm-edc-0.2.9/intecomm_screening/forms/patient_log/patient_log_ug_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/forms/subject_screening/modelform_mixins.py` & `intecomm-edc-0.2.9/intecomm_screening/forms/subject_screening/modelform_mixins.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/forms/subject_screening/subject_screening_form.py` & `intecomm-edc-0.2.9/intecomm_screening/forms/subject_screening/subject_screening_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/forms/subject_screening/subject_screening_ug_form.py` & `intecomm-edc-0.2.9/intecomm_screening/forms/subject_screening/subject_screening_ug_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/identifiers.py` & `intecomm-edc-0.2.9/intecomm_screening/identifiers.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/intecomm_admin_site_mixin.py` & `intecomm-edc-0.2.9/intecomm_screening/intecomm_admin_site_mixin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/locale/lg/LC_MESSAGES/django.po` & `intecomm-edc-0.2.9/intecomm_screening/locale/lg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/locale/sw/LC_MESSAGES/django.po` & `intecomm-edc-0.2.9/intecomm_screening/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/management/commands/print_patient_log_reference.py` & `intecomm-edc-0.2.9/intecomm_screening/management/commands/print_patient_log_reference.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0001_initial.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0002_remove_healthtalklog_unique_lower_name_report_date_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0002_remove_healthtalklog_unique_lower_name_report_date_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0003_site_remove_historicalpatientlog_patient_group_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0003_site_remove_historicalpatientlog_patient_group_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0004_rename_name_historicalpatientlog_legal_name_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0004_rename_name_historicalpatientlog_legal_name_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0005_historicalpatientcall_alt_contact_number_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0005_historicalpatientcall_alt_contact_number_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0006_remove_historicalpatientcall_willing_to_attend_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0006_remove_historicalpatientcall_willing_to_attend_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0007_historicalpatientlog_last_4_contact_number_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0007_historicalpatientlog_last_4_contact_number_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0008_rename_last_routine_appt_date_historicalpatientlog_last_appt_date_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0008_rename_last_routine_appt_date_historicalpatientlog_last_appt_date_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0009_historicalsubjectscreening_familiar_name_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0009_historicalsubjectscreening_familiar_name_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0010_historicalpatientlog_age_in_years_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0010_historicalpatientlog_age_in_years_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0011_rename_hf_identifier_historicalpatientlog_hospital_identifier_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0011_rename_hf_identifier_historicalpatientlog_hospital_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0012_alter_historicalpatientcall_last_attend_clinic_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0012_alter_historicalpatientcall_last_attend_clinic_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0013_alter_healthfacility_distance_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0013_alter_healthfacility_distance_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0014_alter_historicalpatientlog_familiar_name_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0014_alter_historicalpatientlog_familiar_name_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0015_remove_healthtalklog_unique_health_facility_report_date_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0015_remove_healthtalklog_unique_health_facility_report_date_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0016_historicalpatientlog_group_identifier_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0016_historicalpatientlog_group_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0017_alter_historicalpatientlog_group_identifier_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0017_alter_historicalpatientlog_group_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0018_alter_historicalpatientlog_age_in_years_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0018_alter_historicalpatientlog_age_in_years_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0019_healthfacility_fri_healthfacility_mon_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0019_healthfacility_fri_healthfacility_mon_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0020_consentrefusal_historicalconsentrefusal_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0020_consentrefusal_historicalconsentrefusal_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0021_idenfifierformat.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0021_idenfifierformat.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0022_historicalpatientlog_filing_identifier_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0022_historicalpatientlog_filing_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0023_auto_20230501_2208.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0023_auto_20230501_2208.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0024_auto_20230502_0249.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0024_auto_20230502_0249.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0025_patientlogreportprinthistory_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0025_patientlogreportprinthistory_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0026_alter_historicalpatientlog_filing_identifier_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0026_alter_historicalpatientlog_filing_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0027_historicalpatientlog_printed_patientlog_printed.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0027_historicalpatientlog_printed_patientlog_printed.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0029_alter_historicalpatientlog_filing_identifier_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0029_alter_historicalpatientlog_filing_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0030_auto_20230510_0352.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0030_auto_20230510_0352.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0031_alter_historicalpatientlog_next_appt_date_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0031_alter_historicalpatientlog_next_appt_date_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0032_patientgrouprando.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0032_patientgrouprando.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0033_remove_consentrefusal_subject_identifier_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0033_remove_consentrefusal_subject_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0034_alter_consentrefusal_screening_identifier_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0034_alter_consentrefusal_screening_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0035_auto_20230630_0552.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0035_auto_20230630_0552.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0036_alter_historicalpatientlog_screening_identifier_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0036_alter_historicalpatientlog_screening_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0037_alter_consentrefusal_screening_identifier_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0037_alter_consentrefusal_screening_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0038_auto_20230701_0117.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0038_auto_20230701_0117.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0039_alter_historicalpatientlog_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0039_alter_historicalpatientlog_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0040_historicalsubjectscreening_patient_log_identifier_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0040_historicalsubjectscreening_patient_log_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0041_auto_20230702_1548.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0041_auto_20230702_1548.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0042_alter_healthfacility_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0042_alter_healthfacility_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0043_auto_20230705_0529.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0043_auto_20230705_0529.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0044_alter_historicalpatientlog_site_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0044_alter_historicalpatientlog_site_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0045_alter_consentrefusal_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0045_alter_consentrefusal_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0046_alter_historicalpatientlog_legal_name_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0046_alter_historicalpatientlog_legal_name_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0047_rename_historicalhealthfacility_historicaloldhealthfacility_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0047_rename_historicalhealthfacility_historicaloldhealthfacility_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0048_rename_historicalhealthfacility_historicaloldhealthfacility_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0048_rename_historicalhealthfacility_historicaloldhealthfacility_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0049_healthfacility.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0049_healthfacility.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0050_delete_healthfacility_healthtalklog_health_facility_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0050_delete_healthfacility_healthtalklog_health_facility_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0051_auto_20230726_1631.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0051_auto_20230726_1631.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0052_auto_20230726_1634.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0052_auto_20230726_1634.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0053_rename_idenfifierformat_identifierformat_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0053_rename_idenfifierformat_identifierformat_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0057_alter_consentrefusal_device_created_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0057_alter_consentrefusal_device_created_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0058_patientlogug.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0058_patientlogug.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0059_subjectscreeningug_historicalsubjectscreeningug.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0059_subjectscreeningug_historicalsubjectscreeningug.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0060_historicalpatientlogug.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0060_historicalpatientlogug.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0061_historicalpatientlog_comment_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0061_historicalpatientlog_comment_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0062_auto_20230831_0032.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0062_auto_20230831_0032.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0063_alter_consentrefusal_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0063_alter_consentrefusal_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0064_alter_patientcall_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0064_alter_patientcall_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0065_patientlogreportprinthistory_intecomm_sc_modifie_891a97_idx_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0065_patientlogreportprinthistory_intecomm_sc_modifie_891a97_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0066_alter_patientlogreportprinthistory_managers_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0066_alter_patientlogreportprinthistory_managers_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0067_auto_20231216_1807.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0067_auto_20231216_1807.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0068_alter_consentrefusal_site_alter_healthtalklog_site_and_more.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0068_alter_consentrefusal_site_alter_healthtalklog_site_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/migrations/0069_subjectscreeningtz_historicalsubjectscreeningtz.py` & `intecomm-edc-0.2.9/intecomm_screening/migrations/0069_subjectscreeningtz_historicalsubjectscreeningtz.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/model_mixins/patient_call_model_mixin.py` & `intecomm-edc-0.2.9/intecomm_screening/model_mixins/patient_call_model_mixin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/models/__init__.py` & `intecomm-edc-0.2.9/intecomm_screening/models/__init__.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/models/consent_refusal.py` & `intecomm-edc-0.2.9/intecomm_screening/models/consent_refusal.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/models/health_talk_log.py` & `intecomm-edc-0.2.9/intecomm_screening/models/health_talk_log.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/models/identifier_format.py` & `intecomm-edc-0.2.9/intecomm_screening/models/identifier_format.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/models/old_health_facility.py` & `intecomm-edc-0.2.9/intecomm_screening/models/old_health_facility.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/models/patient_call.py` & `intecomm-edc-0.2.9/intecomm_screening/models/patient_call.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/models/patient_log.py` & `intecomm-edc-0.2.9/intecomm_screening/models/patient_log.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/models/patient_log_report_print_history.py` & `intecomm-edc-0.2.9/intecomm_screening/models/patient_log_report_print_history.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/models/signals.py` & `intecomm-edc-0.2.9/intecomm_screening/models/signals.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/models/subject_screening.py` & `intecomm-edc-0.2.9/intecomm_screening/models/subject_screening.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/reports/patient_log_report.py` & `intecomm-edc-0.2.9/intecomm_screening/reports/patient_log_report.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/change_list_group.html` & `intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/change_list_group.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/change_list_patient_log_first_column.html` & `intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/change_list_patient_log_first_column.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/change_list_screen_and_consent.html` & `intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/change_list_screen_and_consent.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/templates/intecomm_screening/group_management.html` & `intecomm-edc-0.2.9/intecomm_screening/templates/intecomm_screening/group_management.html`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/tests/holidays.csv` & `intecomm-edc-0.2.9/intecomm_screening/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/tests/intecomm_test_case_mixin.py` & `intecomm-edc-0.2.9/intecomm_screening/tests/intecomm_test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/tests/tests/test_admin.py` & `intecomm-edc-0.2.9/intecomm_screening/tests/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/tests/tests/test_consent_refusal.py` & `intecomm-edc-0.2.9/intecomm_screening/tests/tests/test_consent_refusal.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/tests/tests/test_screening.py` & `intecomm-edc-0.2.9/intecomm_screening/tests/tests/test_screening.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/urls.py` & `intecomm-edc-0.2.9/intecomm_screening/urls.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/utils.py` & `intecomm-edc-0.2.9/intecomm_screening/utils.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_screening/views.py` & `intecomm-edc-0.2.9/intecomm_screening/views.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_sites/sites.py` & `intecomm-edc-0.2.9/intecomm_sites/sites.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/action_items.py` & `intecomm-edc-0.2.9/intecomm_subject/action_items.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/__init__.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/appointment_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/appointment_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/blood_results/blood_results_fbc_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/blood_results/blood_results_fbc_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/blood_results/blood_results_glu_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/blood_results/blood_results_glu_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/blood_results/blood_results_hba1c_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/blood_results/blood_results_hba1c_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/blood_results/blood_results_ins_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/blood_results/blood_results_ins_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/blood_results/blood_results_lft_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/blood_results/blood_results_lft_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/blood_results/blood_results_lipid_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/blood_results/blood_results_lipid_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/blood_results/blood_results_rft_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/blood_results/blood_results_rft_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/cd4_result_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/cd4_result_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/clinic_note_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/clinic_note_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/clinical_review_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/clinical_review_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/clinical_review_baseline_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/clinical_review_baseline_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/complications_baseline_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/complications_baseline_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/complications_followup_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/complications_followup_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/concomitant_medication_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/concomitant_medication_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/dm_initial_review_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/dm_initial_review_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/dm_review_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/dm_review_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/drug_refill_dm_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/drug_refill_dm_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/drug_refill_hiv_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/drug_refill_hiv_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/drug_refill_htn_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/drug_refill_htn_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/eq5d3l_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/eq5d3l_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/family_history_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/family_history_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/glucose_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/glucose_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/health_economics/assets_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/health_economics/assets_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/health_economics/careseeking_a_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/health_economics/careseeking_a_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/health_economics/careseeking_b_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/health_economics/careseeking_b_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/health_economics/household_head_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/health_economics/household_head_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/health_economics/patient_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/health_economics/patient_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/hiv_initial_review_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/hiv_initial_review_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/hiv_review_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/hiv_review_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/htn_initial_review_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/htn_initial_review_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/htn_review_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/htn_review_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/icecapa_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/icecapa_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/list_filters.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/list_filters.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/location_update_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/location_update_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/medications_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/medications_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/modeladmin_mixins.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/next_appointment_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/next_appointment_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/other_baseline_data_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/other_baseline_data_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/social_harms_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/social_harms_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/subject_requisition_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/subject_requisition_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/subject_visit_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/subject_visit_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/subject_visit_missed_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/subject_visit_missed_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/urine_dipstick_test_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/urine_dipstick_test_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/urine_pregnancy_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/urine_pregnancy_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/admin/vitals_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/admin/vitals_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/baker_recipes.py` & `intecomm-edc-0.2.9/intecomm_subject/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/choices.py` & `intecomm-edc-0.2.9/intecomm_subject/choices.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/form_runners.py` & `intecomm-edc-0.2.9/intecomm_subject/form_runners.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/__init__.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/appointment_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/appointment_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/blood_results/blood_results_fbc_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/blood_results/blood_results_fbc_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/blood_results/blood_results_glu_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/blood_results/blood_results_glu_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/blood_results/blood_results_hba1c_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/blood_results/blood_results_hba1c_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/blood_results/blood_results_ins_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/blood_results/blood_results_ins_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/blood_results/blood_results_lft_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/blood_results/blood_results_lft_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/blood_results/blood_results_lipid_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/blood_results/blood_results_lipid_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/blood_results/blood_results_rft_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/blood_results/blood_results_rft_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/cd4_result_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/cd4_result_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/clinical_note_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/clinical_note_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/dm_medication_adherence_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/dm_medication_adherence_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/drug_supply_hiv_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/drug_supply_hiv_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/eq5d3l_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/eq5d3l_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/health_economics/assets_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/health_economics/assets_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/health_economics/careseeking_a_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/health_economics/careseeking_a_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/health_economics/household_head.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/health_economics/household_head.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/health_economics/income_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/health_economics/income_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/health_economics/patient_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/health_economics/patient_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/health_economics/property_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/health_economics/property_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/hiv_medication_adherence_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/hiv_medication_adherence_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/hiv_review_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/hiv_review_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/htn_medication_adherence_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/htn_medication_adherence_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/location_update_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/location_update_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/next_appointment_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/next_appointment_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/subject_requisition_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/subject_requisition_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/subject_visit_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/subject_visit_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/subject_visit_missed_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/subject_visit_missed_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/urine_dipstick_test_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/urine_dipstick_test_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/forms/urine_pregnancy_form.py` & `intecomm-edc-0.2.9/intecomm_subject/forms/urine_pregnancy_form.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/locale/lg/LC_MESSAGES/django.po` & `intecomm-edc-0.2.9/intecomm_subject/locale/lg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/locale/sw/LC_MESSAGES/django.po` & `intecomm-edc-0.2.9/intecomm_subject/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/management/commands/missed.py` & `intecomm-edc-0.2.9/intecomm_subject/management/commands/missed.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/management/commands/seen_on_day.py` & `intecomm-edc-0.2.9/intecomm_subject/management/commands/seen_on_day.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/metadata_rules/metadata_rules.py` & `intecomm-edc-0.2.9/intecomm_subject/metadata_rules/metadata_rules.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/metadata_rules/predicates.py` & `intecomm-edc-0.2.9/intecomm_subject/metadata_rules/predicates.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0001_initial.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0002_remove_historicaldminitialreview_managed_by_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0002_remove_historicaldminitialreview_managed_by_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0003_alter_historicalsocialharms_coworkers_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0003_alter_historicalsocialharms_coworkers_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0004_historicalsocialharms_employment_impact_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0004_historicalsocialharms_employment_impact_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0005_alter_historicalsocialharms_coworkers_impact_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0005_alter_historicalsocialharms_coworkers_impact_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0006_alter_healtheconomics_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0006_alter_healtheconomics_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0007_alter_historicalotherbaselinedata_alcohol_consumption_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0007_alter_historicalotherbaselinedata_alcohol_consumption_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0008_historicalvitals_vitals_remove_indicators_site_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0008_historicalvitals_vitals_remove_indicators_site_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0009_remove_historicalvitals_bp_measured_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0009_remove_historicalvitals_bp_measured_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0010_remove_historicalvitals_weight_is_estmated_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0010_remove_historicalvitals_weight_is_estmated_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0011_remove_clinicalreviewbaseline_complications_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0011_remove_clinicalreviewbaseline_complications_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0012_alter_historicalvitals_heart_rate_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0012_alter_historicalvitals_heart_rate_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0013_alter_bloodresultsfbc_results_abnormal_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0013_alter_bloodresultsfbc_results_abnormal_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0014_alter_historicalotherbaselinedata_activity_combined_mn_avg_day_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0014_alter_historicalotherbaselinedata_activity_combined_mn_avg_day_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0015_alter_bloodresultsfbc_results_abnormal_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0015_alter_bloodresultsfbc_results_abnormal_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0016_remove_clinicalreview_reason_other_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0016_remove_clinicalreview_reason_other_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0017_alter_bloodresultsfbc_results_abnormal_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0017_alter_bloodresultsfbc_results_abnormal_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0018_remove_historicalhivinitialreview_vl_date_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0018_remove_historicalhivinitialreview_vl_date_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0019_remove_historicalhtninitialreview_med_start_date_estimated_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0019_remove_historicalhtninitialreview_med_start_date_estimated_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0020_remove_historicalhtninitialreview_managed_by_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0020_remove_historicalhtninitialreview_managed_by_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0021_htninitialreview_managed_by_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0021_htninitialreview_managed_by_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0022_historicalhtninitialreview_managed_by_other_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0022_historicalhtninitialreview_managed_by_other_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0023_auto_20230404_0411.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0023_auto_20230404_0411.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0024_historicalhtninitialreview_med_start_date_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0024_historicalhtninitialreview_med_start_date_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0025_rename_med_start_ago_dminitialreview_rx_init_ago_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0025_rename_med_start_ago_dminitialreview_rx_init_ago_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0026_rename_dminitialreview_med_start_date_estimated_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0026_rename_dminitialreview_med_start_date_estimated_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0027_dminitialreview_rx_init_dminitialreview_rx_init_date_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0027_dminitialreview_rx_init_dminitialreview_rx_init_date_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0028_remove_clinicalreviewbaseline_dm_test_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0028_remove_clinicalreviewbaseline_dm_test_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0029_remove_historicaldminitialreview_med_start_estimated_date_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0029_remove_historicaldminitialreview_med_start_estimated_date_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0030_nextappointment_historicalnextappointment_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0030_nextappointment_historicalnextappointment_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0031_alter_clinicalreviewbaseline_dm_dx_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0031_alter_clinicalreviewbaseline_dm_dx_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0032_historicalnextappointment_best_visit_code_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0032_historicalnextappointment_best_visit_code_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0033_clinicalreviewbaseline_dm_dx_at_screening_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0033_clinicalreviewbaseline_dm_dx_at_screening_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0034_clinicalreviewbaseline_protocol_incident_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0034_clinicalreviewbaseline_protocol_incident_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0035_alter_drugrefilldm_return_in_days_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0035_alter_drugrefilldm_return_in_days_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0036_alter_dminitialreview_rx_init_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0036_alter_dminitialreview_rx_init_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0037_alter_bloodresultsins_fasting_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0037_alter_bloodresultsins_fasting_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0038_healtheconomics_welfare_other_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0038_healtheconomics_welfare_other_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0039_icecapa_historicalicecapa_historicaleq5d3l_eq5d3l_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0039_icecapa_historicalicecapa_historicaleq5d3l_eq5d3l_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0040_alter_historicalhivmedicationadherence_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0040_alter_historicalhivmedicationadherence_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0041_health_economics_assets_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0041_health_economics_assets_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0042_alter_bloodresultsins_fasting_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0042_alter_bloodresultsins_fasting_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0043_healtheconomicshouseholdhead_relationship_to_hoh_other_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0043_healtheconomicshouseholdhead_relationship_to_hoh_other_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0044_healtheconomicshouseholdhead_hoh_education_other_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0044_healtheconomicshouseholdhead_hoh_education_other_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0045_healtheconomicshouseholdhead_hoh_marital_status_other_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0045_healtheconomicshouseholdhead_hoh_marital_status_other_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0046_alter_healtheconomicsassets_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0046_alter_healtheconomicsassets_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0047_healtheconomicsassets_cooking_fuel_other_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0047_healtheconomicsassets_cooking_fuel_other_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0048_alter_healtheconomicsincome_external_remittance_currency_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0048_alter_healtheconomicsincome_external_remittance_currency_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0049_alter_healtheconomicsincome_external_remittance_value_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0049_alter_healtheconomicsincome_external_remittance_value_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0050_alter_healtheconomicshouseholdhead_hoh_ethnicity_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0050_alter_healtheconomicshouseholdhead_hoh_ethnicity_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0051_alter_bloodresultsfbc_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0051_alter_bloodresultsfbc_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0052_alter_bloodresultsfbc_managers_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0052_alter_bloodresultsfbc_managers_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0053_remove_historicalhivreview_arv_initiated_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0053_remove_historicalhivreview_arv_initiated_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0054_remove_historicalhtnreview_dia_blood_pressure_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0054_remove_historicalhtnreview_dia_blood_pressure_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0055_rename_drugrefilldm_return_in_days_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0055_rename_drugrefilldm_return_in_days_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0056_alter_drugrefilldm_rx_days_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0056_alter_drugrefilldm_rx_days_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0057_rename_smoker_current_duration_historicalotherbaselinedata_smoker_duration_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0057_rename_smoker_current_duration_historicalotherbaselinedata_smoker_duration_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0058_rename_external_remittance_currency_healtheconomicsincome_external_remit_currency_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0058_rename_external_remittance_currency_healtheconomicsincome_external_remit_currency_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0059_historicalnextappointment_info_source_old_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0059_historicalnextappointment_info_source_old_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0060_historicalnextappointment_info_source_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0060_historicalnextappointment_info_source_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0061_auto_20230725_2035.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0061_auto_20230725_2035.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0062_historicalclinicalnote_clinicalnote.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0062_historicalclinicalnote_clinicalnote.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0063_auto_20230725_2058.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0063_auto_20230725_2058.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0064_historicalnextappointment_health_facility_old_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0064_historicalnextappointment_health_facility_old_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0065_historicalnextappointment_health_facility_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0065_historicalnextappointment_health_facility_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0066_historicalnextappointment_health_facility_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0066_historicalnextappointment_health_facility_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0067_auto_20230726_0008.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0067_auto_20230726_0008.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0068_remove_historicalhba1cresult_history_user_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0068_remove_historicalhba1cresult_history_user_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0069_alter_healtheconomicshouseholdhead_hoh_employment_type_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0069_alter_healtheconomicshouseholdhead_hoh_employment_type_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0070_healtheconomicshouseholdhead_hoh_ethnicity_old_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0070_healtheconomicshouseholdhead_hoh_ethnicity_old_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0071_healtheconomicshouseholdhead_hoh_ethnicity_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0071_healtheconomicshouseholdhead_hoh_ethnicity_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0072_auto_20230803_0305.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0072_auto_20230803_0305.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0073_healtheconomicspatient_pat_ethnicity_new_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0073_healtheconomicspatient_pat_ethnicity_new_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0074_healtheconomicspatient_pat_ethnicity_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0074_healtheconomicspatient_pat_ethnicity_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0075_auto_20230803_0459.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0075_auto_20230803_0459.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0076_healtheconomicshouseholdhead_hoh_religion_old_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0076_healtheconomicshouseholdhead_hoh_religion_old_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0077_healtheconomicshouseholdhead_hoh_religion_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0077_healtheconomicshouseholdhead_hoh_religion_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0078_alter_healtheconomicshouseholdhead_hoh_religion_old_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0078_alter_healtheconomicshouseholdhead_hoh_religion_old_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0079_auto_20230803_0634.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0079_auto_20230803_0634.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0080_auto_20230803_1726.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0080_auto_20230803_1726.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0081_healtheconomicshouseholdhead_hoh_education_old_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0081_healtheconomicshouseholdhead_hoh_education_old_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0082_healtheconomicshouseholdhead_hoh_education_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0082_healtheconomicshouseholdhead_hoh_education_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0083_auto_20230803_1828.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0083_auto_20230803_1828.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0084_alter_healtheconomicsassets_external_wall_material_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0084_alter_healtheconomicsassets_external_wall_material_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0085_alter_healtheconomicsassets_external_wall_material_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0085_alter_healtheconomicsassets_external_wall_material_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0086_rename_hoh_employment_healtheconomicshouseholdhead_hoh_employment_status_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0086_rename_hoh_employment_healtheconomicshouseholdhead_hoh_employment_status_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0087_alter_healtheconomicspatient_pat_citizen_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0087_alter_healtheconomicspatient_pat_citizen_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0088_healtheconomicspatient_pat_employment_type_other_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0088_healtheconomicspatient_pat_employment_type_other_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0089_alter_healtheconomicshouseholdhead_hoh_education_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0089_alter_healtheconomicshouseholdhead_hoh_education_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0090_alter_healtheconomicshouseholdhead_hoh_age_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0090_alter_healtheconomicshouseholdhead_hoh_age_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0091_healtheconomicsassets_solar_panels_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0091_healtheconomicsassets_solar_panels_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0092_healtheconomicsproperty_land_surface_area_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0092_healtheconomicsproperty_land_surface_area_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0093_alter_healtheconomicsproperty_land_value_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0093_alter_healtheconomicsproperty_land_value_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0094_alter_healtheconomicsproperty_land_surface_area_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0094_alter_healtheconomicsproperty_land_surface_area_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0095_alter_healtheconomicsassets_bedrooms_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0095_alter_healtheconomicsassets_bedrooms_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0096_rename_external_remittance_healtheconomicsincome_external_remit_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0096_rename_external_remittance_healtheconomicsincome_external_remit_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0097_alter_healtheconomicsincome_external_remit_value_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0097_alter_healtheconomicsincome_external_remit_value_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0098_alter_healtheconomicshouseholdhead_hoh_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0098_alter_healtheconomicshouseholdhead_hoh_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0099_remove_healtheconomicspatient_pat_citizen_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0099_remove_healtheconomicspatient_pat_citizen_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0100_alter_healtheconomicspatient_pat_education_old_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0100_alter_healtheconomicspatient_pat_education_old_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0101_alter_healtheconomicspatient_pat_education_old_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0101_alter_healtheconomicspatient_pat_education_old_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0102_alter_healtheconomicshouseholdhead_hoh_education_old_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0102_alter_healtheconomicshouseholdhead_hoh_education_old_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0103_alter_healtheconomicshouseholdhead_hoh_employment_status_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0103_alter_healtheconomicshouseholdhead_hoh_employment_status_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0104_historicallocationupdate_locationupdate.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0104_historicallocationupdate_locationupdate.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0105_alter_historicallocationupdate_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0105_alter_historicallocationupdate_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0106_dmmedicationadherence_meds_shortage_reason_other_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0106_dmmedicationadherence_meds_shortage_reason_other_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0107_alter_bloodresultsfbc_device_created_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0107_alter_bloodresultsfbc_device_created_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0108_alter_concomitantmedication_device_created_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0108_alter_concomitantmedication_device_created_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0109_alter_healtheconomicsassets_device_created_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0109_alter_healtheconomicsassets_device_created_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0110_alter_historicalbloodresultsfbc_device_created_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0110_alter_historicalbloodresultsfbc_device_created_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0111_alter_historicalhealtheconomics_device_created_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0111_alter_historicalhealtheconomics_device_created_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0112_alter_historicalhivinitialreview_device_created_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0112_alter_historicalhivinitialreview_device_created_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0113_alter_htnreview_device_created_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0113_alter_htnreview_device_created_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0114_alter_dmmedicationadherence_visual_score_confirmed_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0114_alter_dmmedicationadherence_visual_score_confirmed_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0115_remove_historicalnextappointment_best_visit_code_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0115_remove_historicalnextappointment_best_visit_code_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0116_auto_20230920_0058.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0116_auto_20230920_0058.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0117_historicalnextappointment_allow_create_interim_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0117_historicalnextappointment_allow_create_interim_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0118_historicalnextappointment_info_source_new_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0118_historicalnextappointment_info_source_new_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0119_auto_20231006_0220.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0119_auto_20231006_0220.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0120_remove_historicalnextappointment_info_source_new_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0120_remove_historicalnextappointment_info_source_new_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0121_auto_20231006_0238.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0121_auto_20231006_0238.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0123_alter_subjectvisit_managers.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0123_alter_subjectvisit_managers.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0124_auto_20231115_0133.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0124_auto_20231115_0133.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0125_healtheconomicsproperty_calculated_land_surface_area_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0125_healtheconomicsproperty_calculated_land_surface_area_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0126_feat_683_land_area_units.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0126_feat_683_land_area_units.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0127_alter_historicalsubjectvisitmissed_appt_date_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0127_alter_historicalsubjectvisitmissed_appt_date_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0128_remove_historicalsubjectvisit_clinic_services_other_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0128_remove_historicalsubjectvisit_clinic_services_other_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0129_alter_bloodresultsfbc_options_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0129_alter_bloodresultsfbc_options_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0130_remove_bloodresultsfbc_intecomm_su_subject_1b56bc_idx_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0130_remove_bloodresultsfbc_intecomm_su_subject_1b56bc_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0131_remove_drugrefillhtn_intecomm_su_subject_33642b_idx_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0131_remove_drugrefillhtn_intecomm_su_subject_33642b_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0132_alter_subjectrequisition_unique_together_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0132_alter_subjectrequisition_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0133_bloodresultsfbc_intecomm_su_subject_3bd165_idx_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0133_bloodresultsfbc_intecomm_su_subject_3bd165_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0134_clinicalreviewbaseline_intecomm_su_subject_67b2fa_idx_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0134_clinicalreviewbaseline_intecomm_su_subject_67b2fa_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0135_hivinitialreview_intecomm_su_subject_a055c4_idx_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0135_hivinitialreview_intecomm_su_subject_a055c4_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0136_subjectvisit_intecomm_su_modifie_dab86a_idx_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0136_subjectvisit_intecomm_su_modifie_dab86a_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0137_alter_bloodresultsfbc_platelets_value_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0137_alter_bloodresultsfbc_platelets_value_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0138_alter_bloodresultsfbc_site_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0138_alter_bloodresultsfbc_site_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0139_alter_bloodresultsins_fasting_duration_minutes_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0139_alter_bloodresultsins_fasting_duration_minutes_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0140_historicalhivreview_drawn_date_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0140_historicalhivreview_drawn_date_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0141_remove_viralloadresult_requisition_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0141_remove_viralloadresult_requisition_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0142_alter_historicalhtninitialreview_managed_by_old_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0142_alter_historicalhtninitialreview_managed_by_old_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0143_historicalcareseekingb_historicalcareseekinga_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0143_historicalcareseekingb_historicalcareseekinga_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0144_rename_meds_prescribed_careseekingb_med_prescribed_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0144_rename_meds_prescribed_careseekingb_med_prescribed_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0145_rename_facility_visit_alt_careseekinga_missed_activities_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0145_rename_facility_visit_alt_careseekinga_missed_activities_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0146_rename_seek_inpatient_visits_careseekingb_inpatient_days_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0146_rename_seek_inpatient_visits_careseekingb_inpatient_days_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/migrations/0147_alter_careseekinga_accompany_num_and_more.py` & `intecomm-edc-0.2.9/intecomm_subject/migrations/0147_alter_careseekinga_accompany_num_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/model_mixins/__init__.py` & `intecomm-edc-0.2.9/intecomm_subject/model_mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/model_mixins/clinical_review_model_mixins.py` & `intecomm-edc-0.2.9/intecomm_subject/model_mixins/clinical_review_model_mixins.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/model_mixins/followup_review_model_mixin.py` & `intecomm-edc-0.2.9/intecomm_subject/model_mixins/followup_review_model_mixin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/model_mixins/medication_adherence_model_mixin.py` & `intecomm-edc-0.2.9/intecomm_subject/model_mixins/medication_adherence_model_mixin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/model_mixins/viral_load_result_model_mixin.py` & `intecomm-edc-0.2.9/intecomm_subject/model_mixins/viral_load_result_model_mixin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/__init__.py` & `intecomm-edc-0.2.9/intecomm_subject/models/__init__.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/blood_results/blood_results_fbc.py` & `intecomm-edc-0.2.9/intecomm_subject/models/blood_results/blood_results_fbc.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/blood_results/blood_results_glu.py` & `intecomm-edc-0.2.9/intecomm_subject/models/blood_results/blood_results_glu.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/blood_results/blood_results_hba1c.py` & `intecomm-edc-0.2.9/intecomm_subject/models/blood_results/blood_results_hba1c.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/blood_results/blood_results_ins.py` & `intecomm-edc-0.2.9/intecomm_subject/models/blood_results/blood_results_ins.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/blood_results/blood_results_lft.py` & `intecomm-edc-0.2.9/intecomm_subject/models/blood_results/blood_results_lft.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/blood_results/blood_results_lipid.py` & `intecomm-edc-0.2.9/intecomm_subject/models/blood_results/blood_results_lipid.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/blood_results/blood_results_rft.py` & `intecomm-edc-0.2.9/intecomm_subject/models/blood_results/blood_results_rft.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/cd4_result.py` & `intecomm-edc-0.2.9/intecomm_subject/models/cd4_result.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/clinical_note.py` & `intecomm-edc-0.2.9/intecomm_subject/models/clinical_note.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/clinical_review.py` & `intecomm-edc-0.2.9/intecomm_subject/models/clinical_review.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/clinical_review_baseline.py` & `intecomm-edc-0.2.9/intecomm_subject/models/clinical_review_baseline.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/complications_baseline.py` & `intecomm-edc-0.2.9/intecomm_subject/models/complications_baseline.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/complications_followup.py` & `intecomm-edc-0.2.9/intecomm_subject/models/complications_followup.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/dm_initial_review.py` & `intecomm-edc-0.2.9/intecomm_subject/models/dm_initial_review.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/drug_refill_dm.py` & `intecomm-edc-0.2.9/intecomm_subject/models/drug_refill_dm.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/drug_refill_hiv.py` & `intecomm-edc-0.2.9/intecomm_subject/models/drug_refill_hiv.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/drug_refill_htn.py` & `intecomm-edc-0.2.9/intecomm_subject/models/drug_refill_htn.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/drug_supply_dm.py` & `intecomm-edc-0.2.9/intecomm_subject/models/drug_supply_dm.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/drug_supply_hiv.py` & `intecomm-edc-0.2.9/intecomm_subject/models/drug_supply_hiv.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/drug_supply_htn.py` & `intecomm-edc-0.2.9/intecomm_subject/models/drug_supply_htn.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/family_history.py` & `intecomm-edc-0.2.9/intecomm_subject/models/family_history.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/health_economics/assets.py` & `intecomm-edc-0.2.9/intecomm_subject/models/health_economics/assets.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/health_economics/careseeking_a.py` & `intecomm-edc-0.2.9/intecomm_subject/models/health_economics/careseeking_a.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/health_economics/careseeking_b.py` & `intecomm-edc-0.2.9/intecomm_subject/models/health_economics/careseeking_b.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/health_economics/checklist.py` & `intecomm-edc-0.2.9/intecomm_subject/models/health_economics/checklist.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/health_economics/household_head.py` & `intecomm-edc-0.2.9/intecomm_subject/models/health_economics/household_head.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/health_economics/income.py` & `intecomm-edc-0.2.9/intecomm_subject/models/health_economics/income.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/health_economics/patient.py` & `intecomm-edc-0.2.9/intecomm_subject/models/health_economics/patient.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/health_economics/property.py` & `intecomm-edc-0.2.9/intecomm_subject/models/health_economics/property.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/health_economics_old.py` & `intecomm-edc-0.2.9/intecomm_subject/models/health_economics_old.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/hiv_initial_review.py` & `intecomm-edc-0.2.9/intecomm_subject/models/hiv_initial_review.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/hiv_review.py` & `intecomm-edc-0.2.9/intecomm_subject/models/hiv_review.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/htn_initial_review.py` & `intecomm-edc-0.2.9/intecomm_subject/models/htn_initial_review.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/htn_medication_adherence.py` & `intecomm-edc-0.2.9/intecomm_subject/models/htn_medication_adherence.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/htn_review.py` & `intecomm-edc-0.2.9/intecomm_subject/models/htn_review.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/location_update.py` & `intecomm-edc-0.2.9/intecomm_subject/models/location_update.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/medications.py` & `intecomm-edc-0.2.9/intecomm_subject/models/medications.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/other_baseline_data.py` & `intecomm-edc-0.2.9/intecomm_subject/models/other_baseline_data.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/patient_history.py` & `intecomm-edc-0.2.9/intecomm_subject/models/patient_history.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/reason_for_visit.py` & `intecomm-edc-0.2.9/intecomm_subject/models/reason_for_visit.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/social_harms/model_factories.py` & `intecomm-edc-0.2.9/intecomm_subject/models/social_harms/model_factories.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/social_harms/social_harms.py` & `intecomm-edc-0.2.9/intecomm_subject/models/social_harms/social_harms.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/subject_visit.py` & `intecomm-edc-0.2.9/intecomm_subject/models/subject_visit.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/subject_visit_missed.py` & `intecomm-edc-0.2.9/intecomm_subject/models/subject_visit_missed.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/urine_dipstick_test.py` & `intecomm-edc-0.2.9/intecomm_subject/models/urine_dipstick_test.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/urine_pregnancy.py` & `intecomm-edc-0.2.9/intecomm_subject/models/urine_pregnancy.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/models/vitals.py` & `intecomm-edc-0.2.9/intecomm_subject/models/vitals.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/reference_model_configs.py` & `intecomm-edc-0.2.9/intecomm_subject/reference_model_configs.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/tests/tests/test_admin.py` & `intecomm-edc-0.2.9/intecomm_subject/tests/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/tests/tests/test_appointment.py` & `intecomm-edc-0.2.9/intecomm_subject/tests/tests/test_appointment.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/tests/tests/test_he.py` & `intecomm-edc-0.2.9/intecomm_subject/tests/tests/test_he.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/tests/tests/test_hiv_initial_and_review.py` & `intecomm-edc-0.2.9/intecomm_subject/tests/tests/test_hiv_initial_and_review.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_subject/tests/tests/test_location_update.py` & `intecomm-edc-0.2.9/intecomm_subject/tests/tests/test_location_update.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_visit_schedule/visit_schedules/community_schedule.py` & `intecomm-edc-0.2.9/intecomm_visit_schedule/visit_schedules/community_schedule.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_visit_schedule/visit_schedules/crfs.py` & `intecomm-edc-0.2.9/intecomm_visit_schedule/visit_schedules/crfs.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_visit_schedule/visit_schedules/facility_schedule.py` & `intecomm-edc-0.2.9/intecomm_visit_schedule/visit_schedules/facility_schedule.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_visit_schedule/visit_schedules/requisitions.py` & `intecomm-edc-0.2.9/intecomm_visit_schedule/visit_schedules/requisitions.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_visit_schedule/visit_schedules/visit_schedule.py` & `intecomm-edc-0.2.9/intecomm_visit_schedule/visit_schedules/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/intecomm_visit_schedule/visit_schedules/visits.py` & `intecomm-edc-0.2.9/intecomm_visit_schedule/visit_schedules/visits.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/manage.py` & `intecomm-edc-0.2.9/manage.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/pyproject.toml` & `intecomm-edc-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/runtests.py` & `intecomm-edc-0.2.9/runtests.py`

 * *Files identical despite different names*

### Comparing `intecomm-edc-0.2.8/setup.cfg` & `intecomm-edc-0.2.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 [options]
 python_requires = >=3.11
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
-	edc==0.5.69
+	edc==0.5.70
 	beautifulsoup4
 	intecomm-eligibility==0.1.10
 	intecomm-form-validators==0.1.53
 	intecomm-rando==0.1.24
 	edc_microscopy
 
 [options.packages.find]
```

