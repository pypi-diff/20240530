# Comparing `tmp/botoolkit-1.2.0.tar.gz` & `tmp/botoolkit-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botoolkit-1.2.0.tar", last modified: Wed Feb 14 19:57:19 2024, max compression
+gzip compressed data, was "botoolkit-1.2.1.tar", last modified: Thu May 30 11:30:07 2024, max compression
```

## Comparing `botoolkit-1.2.0.tar` & `botoolkit-1.2.1.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.912895 botoolkit-1.2.0/
--rw-r--r--   0 toor      (1000) toor      (1000)    36571 2024-02-14 19:57:12.000000 botoolkit-1.2.0/CHANGES.md
--rw-r--r--   0 toor      (1000) toor      (1000)      309 2022-04-27 09:28:05.000000 botoolkit-1.2.0/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)    38912 2024-02-14 19:57:19.912895 botoolkit-1.2.0/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     1320 2024-02-06 10:14:23.000000 botoolkit-1.2.0/README.md
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.760894 botoolkit-1.2.0/botoolkit/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.770894 botoolkit-1.2.0/botoolkit/bo_barsdock/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_barsdock/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1215 2023-07-18 12:59:11.000000 botoolkit-1.2.0/botoolkit/bo_barsdock/commands.py
--rw-r--r--   0 toor      (1000) toor      (1000)      112 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_barsdock/enums.py
--rw-r--r--   0 toor      (1000) toor      (1000)      681 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_barsdock/main.py
--rw-r--r--   0 toor      (1000) toor      (1000)      512 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_barsdock/mixins.py
--rw-r--r--   0 toor      (1000) toor      (1000)      382 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_barsdock/settings.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.772894 botoolkit-1.2.0/botoolkit/bo_barsdock/templates/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_barsdock/templates/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)       26 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_barsdock/templates/bobarsdock.conf
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.784895 botoolkit-1.2.0/botoolkit/bo_conf/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_conf/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    20002 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_conf/api.py
--rw-r--r--   0 toor      (1000) toor      (1000)    26830 2022-06-14 20:15:50.000000 botoolkit-1.2.0/botoolkit/bo_conf/commands.py
--rw-r--r--   0 toor      (1000) toor      (1000)       42 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_conf/consts.py
--rw-r--r--   0 toor      (1000) toor      (1000)    43260 2023-06-26 08:08:15.000000 botoolkit-1.2.0/botoolkit/bo_conf/enums.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1891 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_conf/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1063 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_conf/main.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6165 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_conf/mixins.py
--rw-r--r--   0 toor      (1000) toor      (1000)      897 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_conf/settings.py
--rw-r--r--   0 toor      (1000) toor      (1000)      287 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_conf/strings.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.784895 botoolkit-1.2.0/botoolkit/bo_conf/templates/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_conf/templates/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      230 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_conf/templates/boconf.conf
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.792894 botoolkit-1.2.0/botoolkit/bo_databaser/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_databaser/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    29262 2023-04-20 08:09:33.000000 botoolkit-1.2.0/botoolkit/bo_databaser/commands.py
--rw-r--r--   0 toor      (1000) toor      (1000)       34 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_databaser/consts.py
--rw-r--r--   0 toor      (1000) toor      (1000)      695 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_databaser/main.py
--rw-r--r--   0 toor      (1000) toor      (1000)    19465 2023-04-20 08:09:33.000000 botoolkit-1.2.0/botoolkit/bo_databaser/mixins.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3612 2023-04-20 08:09:33.000000 botoolkit-1.2.0/botoolkit/bo_databaser/services.py
--rw-r--r--   0 toor      (1000) toor      (1000)      787 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_databaser/settings.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.795894 botoolkit-1.2.0/botoolkit/bo_databaser/templates/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_databaser/templates/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      563 2023-04-20 08:09:33.000000 botoolkit-1.2.0/botoolkit/bo_databaser/templates/bodatabaser.conf
--rw-r--r--   0 toor      (1000) toor      (1000)     1148 2023-04-20 08:09:33.000000 botoolkit-1.2.0/botoolkit/bo_databaser/templates/bodatabaser_build.conf
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.804895 botoolkit-1.2.0/botoolkit/bo_git/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_git/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    13294 2024-02-14 19:57:12.000000 botoolkit-1.2.0/botoolkit/bo_git/commands.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1248 2023-04-17 20:09:24.000000 botoolkit-1.2.0/botoolkit/bo_git/enums.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1367 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_git/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      641 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_git/main.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5700 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_git/mixins.py
--rw-r--r--   0 toor      (1000) toor      (1000)      561 2022-05-24 12:11:37.000000 botoolkit-1.2.0/botoolkit/bo_git/settings.py
--rw-r--r--   0 toor      (1000) toor      (1000)      470 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_git/strings.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.806894 botoolkit-1.2.0/botoolkit/bo_git/templates/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_git/templates/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      102 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_git/templates/bogit.conf
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.811895 botoolkit-1.2.0/botoolkit/bo_guide/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_guide/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7730 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_guide/commands.py
--rw-r--r--   0 toor      (1000) toor      (1000)      270 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_guide/consts.py
--rw-r--r--   0 toor      (1000) toor      (1000)      667 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_guide/main.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6816 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_guide/mixins.py
--rw-r--r--   0 toor      (1000) toor      (1000)      465 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_guide/settings.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.813894 botoolkit-1.2.0/botoolkit/bo_guide/templates/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_guide/templates/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      213 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_guide/templates/boguide.conf
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.829894 botoolkit-1.2.0/botoolkit/bo_ip/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_ip/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5165 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_ip/api.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5076 2022-06-14 20:15:50.000000 botoolkit-1.2.0/botoolkit/bo_ip/commands.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_ip/enums.py
--rw-r--r--   0 toor      (1000) toor      (1000)      689 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_ip/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      643 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_ip/main.py
--rw-r--r--   0 toor      (1000) toor      (1000)      208 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_ip/settings.py
--rw-r--r--   0 toor      (1000) toor      (1000)       28 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_ip/strings.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.842894 botoolkit-1.2.0/botoolkit/bo_jenkins/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_jenkins/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    37335 2023-02-14 13:23:35.000000 botoolkit-1.2.0/botoolkit/bo_jenkins/commands.py
--rw-r--r--   0 toor      (1000) toor      (1000)      156 2022-06-14 20:15:50.000000 botoolkit-1.2.0/botoolkit/bo_jenkins/consts.py
--rw-r--r--   0 toor      (1000) toor      (1000)      421 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_jenkins/enums.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4044 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_jenkins/generators.py
--rw-r--r--   0 toor      (1000) toor      (1000)      987 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_jenkins/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      704 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_jenkins/main.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7779 2022-06-14 21:31:44.000000 botoolkit-1.2.0/botoolkit/bo_jenkins/mixins.py
--rw-r--r--   0 toor      (1000) toor      (1000)    11584 2022-06-14 20:15:50.000000 botoolkit-1.2.0/botoolkit/bo_jenkins/parsers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      741 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_jenkins/settings.py
--rw-r--r--   0 toor      (1000) toor      (1000)      764 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_jenkins/strings.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.844895 botoolkit-1.2.0/botoolkit/bo_jenkins/templates/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_jenkins/templates/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      313 2022-06-14 21:31:44.000000 botoolkit-1.2.0/botoolkit/bo_jenkins/templates/bojenkins.conf
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.855894 botoolkit-1.2.0/botoolkit/bo_jira/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_jira/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1504 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_jira/api.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5447 2022-05-26 12:27:22.000000 botoolkit-1.2.0/botoolkit/bo_jira/commands.py
--rw-r--r--   0 toor      (1000) toor      (1000)      589 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_jira/consts.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1064 2022-05-24 12:11:37.000000 botoolkit-1.2.0/botoolkit/bo_jira/enums.py
--rw-r--r--   0 toor      (1000) toor      (1000)      172 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_jira/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      677 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_jira/main.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3995 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_jira/mixins.py
--rw-r--r--   0 toor      (1000) toor      (1000)      487 2022-05-25 12:29:29.000000 botoolkit-1.2.0/botoolkit/bo_jira/settings.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.856895 botoolkit-1.2.0/botoolkit/bo_jira/templates/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_jira/templates/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)       34 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_jira/templates/bojira.conf
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.867895 botoolkit-1.2.0/botoolkit/bo_postgres/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_postgres/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2014 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_postgres/command_validators.py
--rw-r--r--   0 toor      (1000) toor      (1000)    41628 2023-04-11 19:37:47.000000 botoolkit-1.2.0/botoolkit/bo_postgres/commands.py
--rw-r--r--   0 toor      (1000) toor      (1000)      158 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_postgres/consts.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3626 2023-04-17 20:09:24.000000 botoolkit-1.2.0/botoolkit/bo_postgres/entities.py
--rw-r--r--   0 toor      (1000) toor      (1000)      191 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_postgres/enums.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2344 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_postgres/exporters.py
--rw-r--r--   0 toor      (1000) toor      (1000)    11901 2023-04-17 20:09:24.000000 botoolkit-1.2.0/botoolkit/bo_postgres/generators.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3838 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_postgres/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      686 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_postgres/main.py
--rw-r--r--   0 toor      (1000) toor      (1000)    18966 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_postgres/mixins.py
--rw-r--r--   0 toor      (1000) toor      (1000)      645 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_postgres/repositories.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2944 2023-10-26 16:04:55.000000 botoolkit-1.2.0/botoolkit/bo_postgres/services.py
--rw-r--r--   0 toor      (1000) toor      (1000)      942 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_postgres/settings.py
--rw-r--r--   0 toor      (1000) toor      (1000)      301 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_postgres/strings.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.868894 botoolkit-1.2.0/botoolkit/bo_postgres/templates/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_postgres/templates/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      510 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_postgres/templates/bopostgres.conf
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.872894 botoolkit-1.2.0/botoolkit/bo_registry/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_registry/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9946 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_registry/commands.py
--rw-r--r--   0 toor      (1000) toor      (1000)     8424 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_registry/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      686 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_registry/main.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4096 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_registry/mixins.py
--rw-r--r--   0 toor      (1000) toor      (1000)      664 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_registry/settings.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.872894 botoolkit-1.2.0/botoolkit/bo_registry/templates/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_registry/templates/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)       77 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_registry/templates/boregistry.conf
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.876895 botoolkit-1.2.0/botoolkit/bo_telegram/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_telegram/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1257 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_telegram/commands.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1177 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_telegram/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      680 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_telegram/main.py
--rw-r--r--   0 toor      (1000) toor      (1000)      464 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_telegram/mixins.py
--rw-r--r--   0 toor      (1000) toor      (1000)      382 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_telegram/settings.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.877894 botoolkit-1.2.0/botoolkit/bo_telegram/templates/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_telegram/templates/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)       25 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_telegram/templates/botelegram.conf
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.881894 botoolkit-1.2.0/botoolkit/bo_toolkit/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_toolkit/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    24990 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_toolkit/commands.py
--rw-r--r--   0 toor      (1000) toor      (1000)      124 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_toolkit/consts.py
--rw-r--r--   0 toor      (1000) toor      (1000)      608 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_toolkit/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      721 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_toolkit/main.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5081 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_toolkit/mixins.py
--rw-r--r--   0 toor      (1000) toor      (1000)      528 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_toolkit/settings.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_toolkit/strings.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.882894 botoolkit-1.2.0/botoolkit/bo_toolkit/templates/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_toolkit/templates/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4523 2023-04-20 08:09:33.000000 botoolkit-1.2.0/botoolkit/bo_toolkit/templates/botoolkit.conf
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.892894 botoolkit-1.2.0/botoolkit/bo_web_bb/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1388 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/api.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3698 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/commands.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1011 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/consts.py
--rw-r--r--   0 toor      (1000) toor      (1000)    43359 2023-07-18 13:15:27.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/enums.py
--rw-r--r--   0 toor      (1000) toor      (1000)      175 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/exceptions.py
--rw-r--r--   0 toor      (1000) toor      (1000)      849 2022-06-01 18:43:21.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/helpers.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.893895 botoolkit-1.2.0/botoolkit/bo_web_bb/images/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/images/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.896895 botoolkit-1.2.0/botoolkit/bo_web_bb/images/base_web_bb_app/
--rwxr-xr-x   0 toor      (1000) toor      (1000)     2038 2022-07-21 15:07:55.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/images/base_web_bb_app/Dockerfile
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/images/base_web_bb_app/__init__.py
--rwxr-xr-x   0 toor      (1000) toor      (1000)     2485 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/images/base_web_bb_app/add_generic_tables.py
--rwxr-xr-x   0 toor      (1000) toor      (1000)     4306 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/images/base_web_bb_app/app.conf.tmpl
--rwxr-xr-x   0 toor      (1000) toor      (1000)      793 2024-02-06 10:14:23.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/images/base_web_bb_app/app_requirements_ssh.txt.tmpl
--rw-r--r--   0 toor      (1000) toor      (1000)     1477 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/images/base_web_bb_app/create_default_date_range_partition.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.898894 botoolkit-1.2.0/botoolkit/bo_web_bb/images/web_bb_app/
--rwxr-xr-x   0 toor      (1000) toor      (1000)      534 2022-07-21 15:07:55.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/images/web_bb_app/Dockerfile
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/images/web_bb_app/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      680 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/main.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6161 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/mixins.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6429 2022-07-21 15:07:55.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/services.py
--rw-r--r--   0 toor      (1000) toor      (1000)      972 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/settings.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/strings.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.899895 botoolkit-1.2.0/botoolkit/bo_web_bb/templates/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/templates/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)       63 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/bo_web_bb/templates/bowebbb.conf
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.909895 botoolkit-1.2.0/botoolkit/core/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/core/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    26495 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/core/commands.py
--rw-r--r--   0 toor      (1000) toor      (1000)      132 2022-07-21 15:07:55.000000 botoolkit-1.2.0/botoolkit/core/consts.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1253 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/core/enums.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2565 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/core/exporters.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9972 2022-06-01 18:43:21.000000 botoolkit-1.2.0/botoolkit/core/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      364 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/core/loggers.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3531 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/core/mixins.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4279 2022-07-21 15:07:55.000000 botoolkit-1.2.0/botoolkit/core/services.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1961 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/core/strings.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1923 2022-04-27 09:28:05.000000 botoolkit-1.2.0/botoolkit/settings.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.911894 botoolkit-1.2.0/botoolkit.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)    38912 2024-02-14 19:57:19.000000 botoolkit-1.2.0/botoolkit.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     5737 2024-02-14 19:57:19.000000 botoolkit-1.2.0/botoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-02-14 19:57:19.000000 botoolkit-1.2.0/botoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)     3650 2024-02-14 19:57:19.000000 botoolkit-1.2.0/botoolkit.egg-info/entry_points.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-02-14 19:57:19.000000 botoolkit-1.2.0/botoolkit.egg-info/namespace_packages.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2022-04-27 09:28:14.000000 botoolkit-1.2.0/botoolkit.egg-info/not-zip-safe
--rw-r--r--   0 toor      (1000) toor      (1000)      248 2024-02-14 19:57:19.000000 botoolkit-1.2.0/botoolkit.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       15 2024-02-14 19:57:19.000000 botoolkit-1.2.0/botoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-14 19:57:19.911894 botoolkit-1.2.0/docs/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.0/docs/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      391 2022-04-27 09:28:05.000000 botoolkit-1.2.0/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2024-02-14 19:57:19.912895 botoolkit-1.2.0/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     1913 2024-02-14 19:57:12.000000 botoolkit-1.2.0/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.547608 botoolkit-1.2.1/
+-rw-r--r--   0 toor      (1000) toor      (1000)    36784 2024-05-30 11:30:02.000000 botoolkit-1.2.1/CHANGES.md
+-rw-r--r--   0 toor      (1000) toor      (1000)      309 2022-04-27 09:28:05.000000 botoolkit-1.2.1/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)    39125 2024-05-30 11:30:07.546609 botoolkit-1.2.1/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     1320 2024-02-06 10:14:23.000000 botoolkit-1.2.1/README.md
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.348609 botoolkit-1.2.1/botoolkit/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.368609 botoolkit-1.2.1/botoolkit/bo_barsdock/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_barsdock/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1215 2023-07-18 12:59:11.000000 botoolkit-1.2.1/botoolkit/bo_barsdock/commands.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      112 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_barsdock/enums.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      681 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_barsdock/main.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      512 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_barsdock/mixins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      382 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_barsdock/settings.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.370608 botoolkit-1.2.1/botoolkit/bo_barsdock/templates/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_barsdock/templates/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       26 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_barsdock/templates/bobarsdock.conf
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.387609 botoolkit-1.2.1/botoolkit/bo_conf/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_conf/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    20002 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_conf/api.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    26830 2022-06-14 20:15:50.000000 botoolkit-1.2.1/botoolkit/bo_conf/commands.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       42 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_conf/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    43260 2023-06-26 08:08:15.000000 botoolkit-1.2.1/botoolkit/bo_conf/enums.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1891 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_conf/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1063 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_conf/main.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6165 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_conf/mixins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      897 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_conf/settings.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      287 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_conf/strings.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.389608 botoolkit-1.2.1/botoolkit/bo_conf/templates/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_conf/templates/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      230 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_conf/templates/boconf.conf
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.404609 botoolkit-1.2.1/botoolkit/bo_databaser/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_databaser/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    29446 2024-05-30 11:30:02.000000 botoolkit-1.2.1/botoolkit/bo_databaser/commands.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       34 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_databaser/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      695 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_databaser/main.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    19465 2023-04-20 08:09:33.000000 botoolkit-1.2.1/botoolkit/bo_databaser/mixins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3612 2023-04-20 08:09:33.000000 botoolkit-1.2.1/botoolkit/bo_databaser/services.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      787 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_databaser/settings.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.413609 botoolkit-1.2.1/botoolkit/bo_databaser/templates/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_databaser/templates/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      563 2023-04-20 08:09:33.000000 botoolkit-1.2.1/botoolkit/bo_databaser/templates/bodatabaser.conf
+-rw-r--r--   0 toor      (1000) toor      (1000)     1148 2023-04-20 08:09:33.000000 botoolkit-1.2.1/botoolkit/bo_databaser/templates/bodatabaser_build.conf
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.423609 botoolkit-1.2.1/botoolkit/bo_git/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_git/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    13294 2024-02-14 19:57:12.000000 botoolkit-1.2.1/botoolkit/bo_git/commands.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1248 2023-04-17 20:09:24.000000 botoolkit-1.2.1/botoolkit/bo_git/enums.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1367 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_git/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      641 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_git/main.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5700 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_git/mixins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      561 2022-05-24 12:11:37.000000 botoolkit-1.2.1/botoolkit/bo_git/settings.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      470 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_git/strings.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.424609 botoolkit-1.2.1/botoolkit/bo_git/templates/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_git/templates/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      102 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_git/templates/bogit.conf
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.432608 botoolkit-1.2.1/botoolkit/bo_guide/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_guide/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7730 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_guide/commands.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      270 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_guide/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      667 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_guide/main.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6816 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_guide/mixins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      465 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_guide/settings.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.434609 botoolkit-1.2.1/botoolkit/bo_guide/templates/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_guide/templates/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      213 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_guide/templates/boguide.conf
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.445608 botoolkit-1.2.1/botoolkit/bo_ip/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_ip/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5165 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_ip/api.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5076 2022-06-14 20:15:50.000000 botoolkit-1.2.1/botoolkit/bo_ip/commands.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_ip/enums.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      689 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_ip/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      643 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_ip/main.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      208 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_ip/settings.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       28 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_ip/strings.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.469609 botoolkit-1.2.1/botoolkit/bo_jenkins/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_jenkins/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    37335 2023-02-14 13:23:35.000000 botoolkit-1.2.1/botoolkit/bo_jenkins/commands.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      156 2022-06-14 20:15:50.000000 botoolkit-1.2.1/botoolkit/bo_jenkins/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      421 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_jenkins/enums.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4044 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_jenkins/generators.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      987 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_jenkins/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      704 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_jenkins/main.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7779 2022-06-14 21:31:44.000000 botoolkit-1.2.1/botoolkit/bo_jenkins/mixins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11584 2022-06-14 20:15:50.000000 botoolkit-1.2.1/botoolkit/bo_jenkins/parsers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      741 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_jenkins/settings.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      764 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_jenkins/strings.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.470609 botoolkit-1.2.1/botoolkit/bo_jenkins/templates/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_jenkins/templates/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      313 2022-06-14 21:31:44.000000 botoolkit-1.2.1/botoolkit/bo_jenkins/templates/bojenkins.conf
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.478608 botoolkit-1.2.1/botoolkit/bo_jira/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_jira/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1504 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_jira/api.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5447 2022-05-26 12:27:22.000000 botoolkit-1.2.1/botoolkit/bo_jira/commands.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      589 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_jira/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1064 2022-05-24 12:11:37.000000 botoolkit-1.2.1/botoolkit/bo_jira/enums.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      172 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_jira/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      677 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_jira/main.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3995 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_jira/mixins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      487 2022-05-25 12:29:29.000000 botoolkit-1.2.1/botoolkit/bo_jira/settings.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.479609 botoolkit-1.2.1/botoolkit/bo_jira/templates/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_jira/templates/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       34 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_jira/templates/bojira.conf
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.488608 botoolkit-1.2.1/botoolkit/bo_postgres/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_postgres/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2014 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_postgres/command_validators.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    41628 2023-04-11 19:37:47.000000 botoolkit-1.2.1/botoolkit/bo_postgres/commands.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      158 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_postgres/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3626 2023-04-17 20:09:24.000000 botoolkit-1.2.1/botoolkit/bo_postgres/entities.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      191 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_postgres/enums.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2344 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_postgres/exporters.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11901 2023-04-17 20:09:24.000000 botoolkit-1.2.1/botoolkit/bo_postgres/generators.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3838 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_postgres/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      686 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_postgres/main.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    18966 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_postgres/mixins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      645 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_postgres/repositories.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2944 2023-10-26 16:04:55.000000 botoolkit-1.2.1/botoolkit/bo_postgres/services.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      942 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_postgres/settings.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      301 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_postgres/strings.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.490609 botoolkit-1.2.1/botoolkit/bo_postgres/templates/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_postgres/templates/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      510 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_postgres/templates/bopostgres.conf
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.493609 botoolkit-1.2.1/botoolkit/bo_registry/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_registry/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9946 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_registry/commands.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     8424 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_registry/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      686 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_registry/main.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4096 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_registry/mixins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      664 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_registry/settings.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.494608 botoolkit-1.2.1/botoolkit/bo_registry/templates/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_registry/templates/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       77 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_registry/templates/boregistry.conf
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.498608 botoolkit-1.2.1/botoolkit/bo_telegram/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_telegram/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1257 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_telegram/commands.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1177 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_telegram/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      680 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_telegram/main.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      464 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_telegram/mixins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      382 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_telegram/settings.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.498608 botoolkit-1.2.1/botoolkit/bo_telegram/templates/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_telegram/templates/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       25 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_telegram/templates/botelegram.conf
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.509609 botoolkit-1.2.1/botoolkit/bo_toolkit/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_toolkit/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    24990 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_toolkit/commands.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      124 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_toolkit/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      608 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_toolkit/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      721 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_toolkit/main.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5081 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_toolkit/mixins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      528 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_toolkit/settings.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_toolkit/strings.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.510609 botoolkit-1.2.1/botoolkit/bo_toolkit/templates/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_toolkit/templates/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4523 2023-04-20 08:09:33.000000 botoolkit-1.2.1/botoolkit/bo_toolkit/templates/botoolkit.conf
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.519609 botoolkit-1.2.1/botoolkit/bo_web_bb/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1388 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/api.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3698 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/commands.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1011 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    43359 2023-07-18 13:15:27.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/enums.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      175 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/exceptions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      849 2022-06-01 18:43:21.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/helpers.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.520609 botoolkit-1.2.1/botoolkit/bo_web_bb/images/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/images/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.524608 botoolkit-1.2.1/botoolkit/bo_web_bb/images/base_web_bb_app/
+-rwxr-xr-x   0 toor      (1000) toor      (1000)     2038 2022-07-21 15:07:55.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/images/base_web_bb_app/Dockerfile
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/images/base_web_bb_app/__init__.py
+-rwxr-xr-x   0 toor      (1000) toor      (1000)     2485 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/images/base_web_bb_app/add_generic_tables.py
+-rwxr-xr-x   0 toor      (1000) toor      (1000)     4306 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/images/base_web_bb_app/app.conf.tmpl
+-rwxr-xr-x   0 toor      (1000) toor      (1000)      793 2024-02-06 10:14:23.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/images/base_web_bb_app/app_requirements_ssh.txt.tmpl
+-rw-r--r--   0 toor      (1000) toor      (1000)     1477 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/images/base_web_bb_app/create_default_date_range_partition.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.526609 botoolkit-1.2.1/botoolkit/bo_web_bb/images/web_bb_app/
+-rwxr-xr-x   0 toor      (1000) toor      (1000)      534 2022-07-21 15:07:55.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/images/web_bb_app/Dockerfile
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/images/web_bb_app/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      680 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/main.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6161 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/mixins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6429 2022-07-21 15:07:55.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/services.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      972 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/settings.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/strings.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.527608 botoolkit-1.2.1/botoolkit/bo_web_bb/templates/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/templates/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       63 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/bo_web_bb/templates/bowebbb.conf
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.542609 botoolkit-1.2.1/botoolkit/core/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/core/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    26495 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/core/commands.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      132 2022-07-21 15:07:55.000000 botoolkit-1.2.1/botoolkit/core/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1253 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/core/enums.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2565 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/core/exporters.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9972 2022-06-01 18:43:21.000000 botoolkit-1.2.1/botoolkit/core/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      364 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/core/loggers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3531 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/core/mixins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4279 2022-07-21 15:07:55.000000 botoolkit-1.2.1/botoolkit/core/services.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1961 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/core/strings.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1923 2022-04-27 09:28:05.000000 botoolkit-1.2.1/botoolkit/settings.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.546609 botoolkit-1.2.1/botoolkit.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)    39125 2024-05-30 11:30:07.000000 botoolkit-1.2.1/botoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     5737 2024-05-30 11:30:07.000000 botoolkit-1.2.1/botoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-05-30 11:30:07.000000 botoolkit-1.2.1/botoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)     3650 2024-05-30 11:30:07.000000 botoolkit-1.2.1/botoolkit.egg-info/entry_points.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-05-30 11:30:07.000000 botoolkit-1.2.1/botoolkit.egg-info/namespace_packages.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2022-04-27 09:28:14.000000 botoolkit-1.2.1/botoolkit.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)      248 2024-05-30 11:30:07.000000 botoolkit-1.2.1/botoolkit.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       15 2024-05-30 11:30:07.000000 botoolkit-1.2.1/botoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-05-30 11:30:07.545609 botoolkit-1.2.1/docs/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-04-27 09:28:05.000000 botoolkit-1.2.1/docs/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      391 2022-04-27 09:28:05.000000 botoolkit-1.2.1/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2024-05-30 11:30:07.547608 botoolkit-1.2.1/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     1913 2024-05-30 11:30:02.000000 botoolkit-1.2.1/setup.py
```

### Comparing `botoolkit-1.2.0/CHANGES.md` & `botoolkit-1.2.1/CHANGES.md`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 ### Изменено
 
 ### Исправлено
 
 ### Удалено
 
 
+## [1.2.1] - 2024-05-30
+
+### Добавлено
+- В databaser, если не получилось сделать pull образа - пробуем его взять из локального хранилища
+
 ## [1.2.0] - 2024-02-14
 
 Доработка команды по анализу и зачистке веток в репозитории. Добавлена возможность указания нескольких проектов, обход 
 поддиректорий с проектами.
 
 ### Добавлено
```

### Comparing `botoolkit-1.2.0/PKG-INFO` & `botoolkit-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botoolkit
-Version: 1.2.0
+Version: 1.2.1
 Summary: BO toolkit
 Home-page: 
 Download-URL: 
 Author: Alexander Danilenko
 Author-email: a.danilenko@bars.group
 Platform: Any
 Classifier: Development Status :: 3 - Alpha
@@ -86,14 +86,19 @@
 ### Изменено
 
 ### Исправлено
 
 ### Удалено
 
 
+## [1.2.1] - 2024-05-30
+
+### Добавлено
+- В databaser, если не получилось сделать pull образа - пробуем его взять из локального хранилища
+
 ## [1.2.0] - 2024-02-14
 
 Доработка команды по анализу и зачистке веток в репозитории. Добавлена возможность указания нескольких проектов, обход 
 поддиректорий с проектами.
 
 ### Добавлено
```

### Comparing `botoolkit-1.2.0/README.md` & `botoolkit-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_barsdock/commands.py` & `botoolkit-1.2.1/botoolkit/bo_barsdock/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_barsdock/main.py` & `botoolkit-1.2.1/botoolkit/bo_barsdock/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_barsdock/mixins.py` & `botoolkit-1.2.1/botoolkit/bo_barsdock/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_conf/api.py` & `botoolkit-1.2.1/botoolkit/bo_conf/api.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_conf/commands.py` & `botoolkit-1.2.1/botoolkit/bo_conf/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_conf/enums.py` & `botoolkit-1.2.1/botoolkit/bo_conf/enums.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_conf/helpers.py` & `botoolkit-1.2.1/botoolkit/bo_conf/helpers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_conf/main.py` & `botoolkit-1.2.1/botoolkit/bo_conf/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_conf/mixins.py` & `botoolkit-1.2.1/botoolkit/bo_conf/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_conf/settings.py` & `botoolkit-1.2.1/botoolkit/bo_conf/settings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_databaser/commands.py` & `botoolkit-1.2.1/botoolkit/bo_databaser/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -659,17 +659,22 @@
         Запуск Databaser
         """
         logger.write(
             f'pulling Databaser image '
             f'{self._parsed_args.databaser_build_image}..\n'
         )
 
-        databaser_image = self._docker_client.images.pull(
-            repository=self._parsed_args.databaser_build_image,
-        )
+        try:
+            databaser_image = self._docker_client.images.pull(
+                repository=self._parsed_args.databaser_build_image,
+            )
+        except Exception:
+            databaser_image = self._docker_client.images.get(
+                self._parsed_args.databaser_build_image,
+            )
 
         databaser_manager = DatabaserServiceManager(
             docker_client=self._docker_client,
             network=self._parsed_args.docker_network,
         )
 
         logger.write(
```

### Comparing `botoolkit-1.2.0/botoolkit/bo_databaser/main.py` & `botoolkit-1.2.1/botoolkit/bo_databaser/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_databaser/mixins.py` & `botoolkit-1.2.1/botoolkit/bo_databaser/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_databaser/services.py` & `botoolkit-1.2.1/botoolkit/bo_databaser/services.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_databaser/settings.py` & `botoolkit-1.2.1/botoolkit/bo_databaser/settings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_databaser/templates/bodatabaser.conf` & `botoolkit-1.2.1/botoolkit/bo_databaser/templates/bodatabaser.conf`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_databaser/templates/bodatabaser_build.conf` & `botoolkit-1.2.1/botoolkit/bo_databaser/templates/bodatabaser_build.conf`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_git/commands.py` & `botoolkit-1.2.1/botoolkit/bo_git/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_git/enums.py` & `botoolkit-1.2.1/botoolkit/bo_git/enums.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_git/helpers.py` & `botoolkit-1.2.1/botoolkit/bo_git/helpers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_git/main.py` & `botoolkit-1.2.1/botoolkit/bo_git/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_git/mixins.py` & `botoolkit-1.2.1/botoolkit/bo_git/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_git/settings.py` & `botoolkit-1.2.1/botoolkit/bo_git/settings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_guide/commands.py` & `botoolkit-1.2.1/botoolkit/bo_guide/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_guide/main.py` & `botoolkit-1.2.1/botoolkit/bo_guide/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_guide/mixins.py` & `botoolkit-1.2.1/botoolkit/bo_guide/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_ip/api.py` & `botoolkit-1.2.1/botoolkit/bo_ip/api.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_ip/commands.py` & `botoolkit-1.2.1/botoolkit/bo_ip/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_ip/helpers.py` & `botoolkit-1.2.1/botoolkit/bo_ip/helpers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_ip/main.py` & `botoolkit-1.2.1/botoolkit/bo_ip/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_jenkins/commands.py` & `botoolkit-1.2.1/botoolkit/bo_jenkins/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_jenkins/generators.py` & `botoolkit-1.2.1/botoolkit/bo_jenkins/generators.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_jenkins/helpers.py` & `botoolkit-1.2.1/botoolkit/bo_jenkins/helpers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_jenkins/main.py` & `botoolkit-1.2.1/botoolkit/bo_jenkins/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_jenkins/mixins.py` & `botoolkit-1.2.1/botoolkit/bo_jenkins/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_jenkins/parsers.py` & `botoolkit-1.2.1/botoolkit/bo_jenkins/parsers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_jenkins/settings.py` & `botoolkit-1.2.1/botoolkit/bo_jenkins/settings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_jenkins/strings.py` & `botoolkit-1.2.1/botoolkit/bo_jenkins/strings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_jira/api.py` & `botoolkit-1.2.1/botoolkit/bo_jira/api.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_jira/commands.py` & `botoolkit-1.2.1/botoolkit/bo_jira/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_jira/consts.py` & `botoolkit-1.2.1/botoolkit/bo_jira/consts.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_jira/enums.py` & `botoolkit-1.2.1/botoolkit/bo_jira/enums.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_jira/main.py` & `botoolkit-1.2.1/botoolkit/bo_jira/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_jira/mixins.py` & `botoolkit-1.2.1/botoolkit/bo_jira/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_postgres/command_validators.py` & `botoolkit-1.2.1/botoolkit/bo_postgres/command_validators.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_postgres/commands.py` & `botoolkit-1.2.1/botoolkit/bo_postgres/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_postgres/entities.py` & `botoolkit-1.2.1/botoolkit/bo_postgres/entities.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_postgres/exporters.py` & `botoolkit-1.2.1/botoolkit/bo_postgres/exporters.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_postgres/generators.py` & `botoolkit-1.2.1/botoolkit/bo_postgres/generators.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_postgres/helpers.py` & `botoolkit-1.2.1/botoolkit/bo_postgres/helpers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_postgres/main.py` & `botoolkit-1.2.1/botoolkit/bo_postgres/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_postgres/mixins.py` & `botoolkit-1.2.1/botoolkit/bo_postgres/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_postgres/repositories.py` & `botoolkit-1.2.1/botoolkit/bo_postgres/repositories.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_postgres/services.py` & `botoolkit-1.2.1/botoolkit/bo_postgres/services.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_postgres/settings.py` & `botoolkit-1.2.1/botoolkit/bo_postgres/settings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_registry/commands.py` & `botoolkit-1.2.1/botoolkit/bo_registry/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_registry/helpers.py` & `botoolkit-1.2.1/botoolkit/bo_registry/helpers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_registry/main.py` & `botoolkit-1.2.1/botoolkit/bo_registry/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_registry/mixins.py` & `botoolkit-1.2.1/botoolkit/bo_registry/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_registry/settings.py` & `botoolkit-1.2.1/botoolkit/bo_registry/settings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_telegram/commands.py` & `botoolkit-1.2.1/botoolkit/bo_telegram/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_telegram/helpers.py` & `botoolkit-1.2.1/botoolkit/bo_telegram/helpers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_telegram/main.py` & `botoolkit-1.2.1/botoolkit/bo_telegram/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_toolkit/commands.py` & `botoolkit-1.2.1/botoolkit/bo_toolkit/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_toolkit/helpers.py` & `botoolkit-1.2.1/botoolkit/bo_toolkit/helpers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_toolkit/main.py` & `botoolkit-1.2.1/botoolkit/bo_toolkit/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_toolkit/mixins.py` & `botoolkit-1.2.1/botoolkit/bo_toolkit/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_toolkit/settings.py` & `botoolkit-1.2.1/botoolkit/bo_toolkit/settings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_toolkit/templates/botoolkit.conf` & `botoolkit-1.2.1/botoolkit/bo_toolkit/templates/botoolkit.conf`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_web_bb/api.py` & `botoolkit-1.2.1/botoolkit/bo_web_bb/api.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_web_bb/commands.py` & `botoolkit-1.2.1/botoolkit/bo_web_bb/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_web_bb/consts.py` & `botoolkit-1.2.1/botoolkit/bo_web_bb/consts.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_web_bb/enums.py` & `botoolkit-1.2.1/botoolkit/bo_web_bb/enums.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_web_bb/helpers.py` & `botoolkit-1.2.1/botoolkit/bo_web_bb/helpers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_web_bb/images/base_web_bb_app/Dockerfile` & `botoolkit-1.2.1/botoolkit/bo_web_bb/images/base_web_bb_app/Dockerfile`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_web_bb/images/base_web_bb_app/add_generic_tables.py` & `botoolkit-1.2.1/botoolkit/bo_web_bb/images/base_web_bb_app/add_generic_tables.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_web_bb/images/base_web_bb_app/app.conf.tmpl` & `botoolkit-1.2.1/botoolkit/bo_web_bb/images/base_web_bb_app/app.conf.tmpl`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_web_bb/images/base_web_bb_app/app_requirements_ssh.txt.tmpl` & `botoolkit-1.2.1/botoolkit/bo_web_bb/images/base_web_bb_app/app_requirements_ssh.txt.tmpl`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_web_bb/images/base_web_bb_app/create_default_date_range_partition.py` & `botoolkit-1.2.1/botoolkit/bo_web_bb/images/base_web_bb_app/create_default_date_range_partition.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_web_bb/images/web_bb_app/Dockerfile` & `botoolkit-1.2.1/botoolkit/bo_web_bb/images/web_bb_app/Dockerfile`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_web_bb/main.py` & `botoolkit-1.2.1/botoolkit/bo_web_bb/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_web_bb/mixins.py` & `botoolkit-1.2.1/botoolkit/bo_web_bb/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_web_bb/services.py` & `botoolkit-1.2.1/botoolkit/bo_web_bb/services.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/bo_web_bb/settings.py` & `botoolkit-1.2.1/botoolkit/bo_web_bb/settings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/core/commands.py` & `botoolkit-1.2.1/botoolkit/core/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/core/enums.py` & `botoolkit-1.2.1/botoolkit/core/enums.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/core/exporters.py` & `botoolkit-1.2.1/botoolkit/core/exporters.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/core/helpers.py` & `botoolkit-1.2.1/botoolkit/core/helpers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/core/mixins.py` & `botoolkit-1.2.1/botoolkit/core/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/core/services.py` & `botoolkit-1.2.1/botoolkit/core/services.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/core/strings.py` & `botoolkit-1.2.1/botoolkit/core/strings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit/settings.py` & `botoolkit-1.2.1/botoolkit/settings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit.egg-info/PKG-INFO` & `botoolkit-1.2.1/botoolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botoolkit
-Version: 1.2.0
+Version: 1.2.1
 Summary: BO toolkit
 Home-page: 
 Download-URL: 
 Author: Alexander Danilenko
 Author-email: a.danilenko@bars.group
 Platform: Any
 Classifier: Development Status :: 3 - Alpha
@@ -86,14 +86,19 @@
 ### Изменено
 
 ### Исправлено
 
 ### Удалено
 
 
+## [1.2.1] - 2024-05-30
+
+### Добавлено
+- В databaser, если не получилось сделать pull образа - пробуем его взять из локального хранилища
+
 ## [1.2.0] - 2024-02-14
 
 Доработка команды по анализу и зачистке веток в репозитории. Добавлена возможность указания нескольких проектов, обход 
 поддиректорий с проектами.
 
 ### Добавлено
```

### Comparing `botoolkit-1.2.0/botoolkit.egg-info/SOURCES.txt` & `botoolkit-1.2.1/botoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/botoolkit.egg-info/entry_points.txt` & `botoolkit-1.2.1/botoolkit.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `botoolkit-1.2.0/setup.py` & `botoolkit-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from botoolkit.settings import (
     ENTRY_POINTS,
 )
 
 
 PROJECT = 'botoolkit'
 
-VERSION = '1.2.0'
+VERSION = '1.2.1'
 
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
```

