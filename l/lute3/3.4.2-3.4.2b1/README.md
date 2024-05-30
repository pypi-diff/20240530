# Comparing `tmp/lute3-3.4.2.tar.gz` & `tmp/lute3-3.4.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lute3-3.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lute3-3.4.2b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lute3-3.4.2.tar` & `lute3-3.4.2b1.tar`

### file list

```diff
@@ -1,653 +1,652 @@
--rw-r--r--   0        0        0      170 2023-11-09 08:26:12.050479 lute3-3.4.2/.dockerignore
--rw-r--r--   0        0        0     1280 2024-03-08 03:05:01.842902 lute3-3.4.2/.github/ISSUE_TEMPLATE/add_language.md
--rw-r--r--   0        0        0      590 2024-03-08 03:05:01.843291 lute3-3.4.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      649 2024-04-28 00:44:07.948708 lute3-3.4.2/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0        0        0      578 2024-03-08 03:05:01.843637 lute3-3.4.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0    10714 2024-05-19 18:38:13.894853 lute3-3.4.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2663 2024-04-28 00:44:07.949318 lute3-3.4.2/.github/workflows/coverage.yml
--rw-r--r--   0        0        0     2172 2024-04-05 03:40:57.739326 lute3-3.4.2/.gitignore
--rw-r--r--   0        0        0      119 2024-04-28 00:44:07.949499 lute3-3.4.2/.gitmodules
--rw-r--r--   0        0        0      395 2024-01-13 04:05:05.193611 lute3-3.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    24735 2023-11-20 01:37:46.796733 lute3-3.4.2/.pylintrc
--rw-r--r--   0        0        0     1076 2024-01-13 04:05:05.194389 lute3-3.4.2/.pytest.ini
--rw-r--r--   0        0        0     1068 2023-11-09 05:33:09.100157 lute3-3.4.2/LICENSE.txt
--rw-r--r--   0        0        0     1641 2024-04-28 00:44:07.949766 lute3-3.4.2/README.md
--rw-r--r--   0        0        0     1145 2024-04-28 00:44:07.950030 lute3-3.4.2/README_PyPi.md
--rw-r--r--   0        0        0     1664 2024-05-18 03:42:18.960922 lute3-3.4.2/devstart.py
--rw-r--r--   0        0        0      965 2023-11-10 18:48:16.706091 lute3-3.4.2/docker/Dockerfile
--rw-r--r--   0        0        0      496 2024-01-13 04:05:05.195405 lute3-3.4.2/docker/README.md
--rwxr-xr-x   0        0        0     1545 2024-01-13 04:05:05.195617 lute3-3.4.2/docker/build_all.sh
--rwxr-xr-x   0        0        0       89 2024-01-13 04:05:05.195716 lute3-3.4.2/docker/build_test.sh
--rw-r--r--   0        0        0     1076 2023-11-09 08:26:12.052441 lute3-3.4.2/docker/check_mounts_and_start.sh
--rw-r--r--   0        0        0      309 2023-11-09 08:26:12.052717 lute3-3.4.2/docker/docker-compose.yml.example
--rw-r--r--   0        0        0     3249 2024-04-28 00:44:07.950509 lute3-3.4.2/docker/docker_hub_overview.md
--rwxr-xr-x   0        0        0     1127 2024-01-13 04:05:05.195822 lute3-3.4.2/docker/try_build_multi.sh
--rw-r--r--   0        0        0    16003 2024-05-30 03:05:58.260077 lute3-3.4.2/docs/CHANGELOG.md
--rw-r--r--   0        0        0       71 2024-01-13 04:05:05.196786 lute3-3.4.2/docs/README.md
--rw-r--r--   0        0        0     1068 2023-11-09 05:33:09.101369 lute3-3.4.2/lute/LICENSE.txt
--rw-r--r--   0        0        0      380 2024-05-30 03:06:17.811482 lute3-3.4.2/lute/__init__.py
--rw-r--r--   0        0        0    12536 2024-05-28 14:17:46.258987 lute3-3.4.2/lute/app_factory.py
--rw-r--r--   0        0        0        0 2023-10-30 00:38:51.292984 lute3-3.4.2/lute/backup/__init__.py
--rw-r--r--   0        0        0     2300 2024-03-15 03:25:40.865078 lute3-3.4.2/lute/backup/routes.py
--rw-r--r--   0        0        0     5303 2024-03-15 03:25:40.865445 lute3-3.4.2/lute/backup/service.py
--rw-r--r--   0        0        0        0 2023-10-24 05:43:55.066190 lute3-3.4.2/lute/bing/__init__.py
--rw-r--r--   0        0        0     3736 2024-03-13 16:30:50.197607 lute3-3.4.2/lute/bing/routes.py
--rw-r--r--   0        0        0        0 2023-10-16 06:20:14.169949 lute3-3.4.2/lute/book/__init__.py
--rw-r--r--   0        0        0     2541 2024-03-15 03:25:40.865805 lute3-3.4.2/lute/book/datatables.py
--rw-r--r--   0        0        0     5146 2024-05-18 03:42:18.962171 lute3-3.4.2/lute/book/forms.py
--rw-r--r--   0        0        0     3633 2024-04-28 00:44:07.951451 lute3-3.4.2/lute/book/model.py
--rw-r--r--   0        0        0     5021 2024-03-25 09:32:17.257357 lute3-3.4.2/lute/book/routes.py
--rw-r--r--   0        0        0     6395 2024-03-25 09:32:17.258143 lute3-3.4.2/lute/book/service.py
--rw-r--r--   0        0        0     3598 2024-02-07 07:50:18.749346 lute3-3.4.2/lute/book/stats.py
--rw-r--r--   0        0        0      475 2024-01-13 04:05:05.200591 lute3-3.4.2/lute/cli/README.md
--rw-r--r--   0        0        0        0 2024-01-13 04:05:05.200653 lute3-3.4.2/lute/cli/__init__.py
--rw-r--r--   0        0        0      807 2024-01-13 04:05:05.200788 lute3-3.4.2/lute/cli/commands.py
--rw-r--r--   0        0        0     6340 2024-05-11 22:55:05.262438 lute3-3.4.2/lute/cli/language_term_export.py
--rw-r--r--   0        0        0        0 2023-11-04 21:50:44.080272 lute3-3.4.2/lute/config/__init__.py
--rw-r--r--   0        0        0     3093 2024-05-27 23:47:17.824218 lute3-3.4.2/lute/config/app_config.py
--rw-r--r--   0        0        0      265 2024-01-13 04:05:05.201516 lute3-3.4.2/lute/config/config.yml.docker
--rw-r--r--   0        0        0      667 2024-01-13 04:05:05.201703 lute3-3.4.2/lute/config/config.yml.example
--rw-r--r--   0        0        0      280 2024-01-13 04:05:05.201898 lute3-3.4.2/lute/config/config.yml.prod
--rw-r--r--   0        0        0      108 2023-10-20 18:48:10.167405 lute3-3.4.2/lute/db/__init__.py
--rw-r--r--   0        0        0     1021 2024-02-07 07:50:18.750797 lute3-3.4.2/lute/db/data_cleanup.py
--rw-r--r--   0        0        0     3032 2024-04-28 00:44:07.951712 lute3-3.4.2/lute/db/demo.py
--rw-r--r--   0        0        0      525 2024-04-28 00:58:20.367519 lute3-3.4.2/lute/db/language_defs/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1799 2024-04-28 00:58:20.367921 lute3-3.4.2/lute/db/language_defs/README.md
--rw-r--r--   0        0        0      379 2024-04-28 00:58:20.368228 lute3-3.4.2/lute/db/language_defs/_templates/definition.yaml.example
--rw-r--r--   0        0        0       35 2024-04-28 00:58:20.368382 lute3-3.4.2/lute/db/language_defs/_templates/story.txt.example
--rw-r--r--   0        0        0      820 2024-04-28 00:58:20.369000 lute3-3.4.2/lute/db/language_defs/afrikaans/definition.yaml
--rw-r--r--   0        0        0      582 2024-04-28 00:58:20.369554 lute3-3.4.2/lute/db/language_defs/afrikaans/die_diere_grawe_n_put.txt
--rw-r--r--   0        0        0      816 2024-04-28 00:58:20.370260 lute3-3.4.2/lute/db/language_defs/albanian/definition.yaml
--rw-r--r--   0        0        0      791 2024-04-28 00:58:20.370623 lute3-3.4.2/lute/db/language_defs/albanian/shqiponja_dhe_mbreti.txt
--rw-r--r--   0        0        0      943 2024-04-28 00:58:20.371105 lute3-3.4.2/lute/db/language_defs/amharic/definition.yaml
--rw-r--r--   0        0        0      898 2024-04-28 00:58:20.371501 lute3-3.4.2/lute/db/language_defs/amharic/story_1.txt
--rw-r--r--   0        0        0     1147 2024-04-28 00:58:20.371719 lute3-3.4.2/lute/db/language_defs/arabic/ar_demo.txt
--rw-r--r--   0        0        0      555 2024-04-28 00:58:20.371868 lute3-3.4.2/lute/db/language_defs/arabic/definition.yaml
--rw-r--r--   0        0        0     1453 2024-04-28 00:58:20.372285 lute3-3.4.2/lute/db/language_defs/armenian/definition.yaml
--rw-r--r--   0        0        0     3063 2024-04-28 00:58:20.372760 lute3-3.4.2/lute/db/language_defs/armenian/story_1.txt
--rw-r--r--   0        0        0     1473 2024-04-28 00:58:20.373153 lute3-3.4.2/lute/db/language_defs/azerbaijani/definition.yaml
--rw-r--r--   0        0        0     2742 2024-04-28 00:58:20.373423 lute3-3.4.2/lute/db/language_defs/azerbaijani/story_1.txt
--rw-r--r--   0        0        0      885 2024-04-28 00:58:20.373817 lute3-3.4.2/lute/db/language_defs/basque/definition.yaml
--rw-r--r--   0        0        0      663 2024-04-28 00:58:20.374076 lute3-3.4.2/lute/db/language_defs/basque/story_1.txt
--rw-r--r--   0        0        0     1024 2024-04-28 00:58:20.374525 lute3-3.4.2/lute/db/language_defs/belarusian/definition.yaml
--rw-r--r--   0        0        0     2573 2024-04-28 00:58:20.374843 lute3-3.4.2/lute/db/language_defs/belarusian/story_1.txt
--rw-r--r--   0        0        0     2176 2024-04-28 00:58:20.375301 lute3-3.4.2/lute/db/language_defs/bengali/aharshi_the_bengal_tiger.txt
--rw-r--r--   0        0        0      988 2024-04-28 00:58:20.375609 lute3-3.4.2/lute/db/language_defs/bengali/definition.yaml
--rw-r--r--   0        0        0     1220 2024-04-28 00:58:20.375973 lute3-3.4.2/lute/db/language_defs/breton/definition.yaml
--rw-r--r--   0        0        0     1991 2024-04-28 00:58:20.376271 lute3-3.4.2/lute/db/language_defs/breton/story_1.txt
--rw-r--r--   0        0        0     1499 2024-04-28 00:58:20.376643 lute3-3.4.2/lute/db/language_defs/bulgarian/definition.yaml
--rw-r--r--   0        0        0      731 2024-04-28 00:58:20.376952 lute3-3.4.2/lute/db/language_defs/bulgarian/yesterday_film_description.txt
--rw-r--r--   0        0        0     1991 2024-04-28 00:58:20.377555 lute3-3.4.2/lute/db/language_defs/catalan/definition.yaml
--rw-r--r--   0        0        0      718 2024-04-28 00:58:20.377855 lute3-3.4.2/lute/db/language_defs/catalan/merlí_series_description.txt
--rw-r--r--   0        0        0     1412 2024-04-28 00:58:20.378088 lute3-3.4.2/lute/db/language_defs/classical_chinese/cc_demo.txt
--rw-r--r--   0        0        0      416 2024-04-28 00:58:20.378221 lute3-3.4.2/lute/db/language_defs/classical_chinese/definition.yaml
--rw-r--r--   0        0        0      948 2024-04-28 00:58:20.378797 lute3-3.4.2/lute/db/language_defs/croatian/definition.yaml
--rw-r--r--   0        0        0      530 2024-04-28 00:58:20.379041 lute3-3.4.2/lute/db/language_defs/croatian/story_1.txt
--rw-r--r--   0        0        0      518 2024-04-28 00:58:20.379330 lute3-3.4.2/lute/db/language_defs/czech/czech.txt
--rw-r--r--   0        0        0      377 2024-04-28 00:58:20.379456 lute3-3.4.2/lute/db/language_defs/czech/definition.yaml
--rw-r--r--   0        0        0     1093 2024-04-28 00:58:20.379770 lute3-3.4.2/lute/db/language_defs/danish/definition.yaml
--rw-r--r--   0        0        0      670 2024-04-28 00:58:20.380012 lute3-3.4.2/lute/db/language_defs/danish/prinsessen_pa_arten.txt
--rw-r--r--   0        0        0      474 2024-04-28 00:58:20.380500 lute3-3.4.2/lute/db/language_defs/dutch/de_doortocht.txt
--rw-r--r--   0        0        0     1127 2024-04-28 00:58:20.381065 lute3-3.4.2/lute/db/language_defs/dutch/definition.yaml
--rw-r--r--   0        0        0      468 2024-04-28 00:58:20.381348 lute3-3.4.2/lute/db/language_defs/english/definition.yaml
--rw-r--r--   0        0        0     7159 2024-04-28 00:58:20.381753 lute3-3.4.2/lute/db/language_defs/english/tutorial.txt
--rw-r--r--   0        0        0     3534 2024-04-28 00:58:20.381883 lute3-3.4.2/lute/db/language_defs/english/tutorial_follow_up.txt
--rw-r--r--   0        0        0      858 2024-04-28 00:58:20.382235 lute3-3.4.2/lute/db/language_defs/esperanto/definition.yaml
--rw-r--r--   0        0        0      535 2024-04-28 00:58:20.382495 lute3-3.4.2/lute/db/language_defs/esperanto/story_1.txt
--rw-r--r--   0        0        0     2043 2024-04-28 00:58:20.382830 lute3-3.4.2/lute/db/language_defs/estonian/definition.yaml
--rw-r--r--   0        0        0      746 2024-04-28 00:58:20.383067 lute3-3.4.2/lute/db/language_defs/estonian/story_1.txt
--rw-r--r--   0        0        0     1000 2024-04-28 00:58:20.383513 lute3-3.4.2/lute/db/language_defs/farsi/definition.yaml
--rw-r--r--   0        0        0      951 2024-04-28 00:58:20.383824 lute3-3.4.2/lute/db/language_defs/farsi/story_1.txt
--rw-r--r--   0        0        0     2450 2024-04-28 00:58:20.384190 lute3-3.4.2/lute/db/language_defs/finnish/definition.yaml
--rw-r--r--   0        0        0      537 2024-04-28 00:58:20.384443 lute3-3.4.2/lute/db/language_defs/finnish/story_1.txt
--rw-r--r--   0        0        0      370 2024-04-28 00:58:20.384728 lute3-3.4.2/lute/db/language_defs/french/definition.yaml
--rw-r--r--   0        0        0      469 2024-04-28 00:58:20.385090 lute3-3.4.2/lute/db/language_defs/french/fr_goldilocks.txt
--rw-r--r--   0        0        0     1672 2024-04-28 00:58:20.385735 lute3-3.4.2/lute/db/language_defs/galician/definition.yaml
--rw-r--r--   0        0        0      544 2024-04-28 00:58:20.386025 lute3-3.4.2/lute/db/language_defs/galician/story_1.txt
--rw-r--r--   0        0        0      513 2024-04-29 04:26:18.411489 lute3-3.4.2/lute/db/language_defs/generic/definition.yaml
--rw-r--r--   0        0        0     3882 2024-04-29 04:26:18.411940 lute3-3.4.2/lute/db/language_defs/generic/story_1.txt
--rw-r--r--   0        0        0     1306 2024-04-28 00:58:20.386531 lute3-3.4.2/lute/db/language_defs/georgian/definition.yaml
--rw-r--r--   0        0        0      953 2024-04-28 00:58:20.386759 lute3-3.4.2/lute/db/language_defs/georgian/story_1.txt
--rw-r--r--   0        0        0     1058 2024-04-28 00:58:20.386961 lute3-3.4.2/lute/db/language_defs/german/de_Stadtmusikanten.txt
--rw-r--r--   0        0        0      522 2024-04-28 00:58:20.387058 lute3-3.4.2/lute/db/language_defs/german/definition.yaml
--rw-r--r--   0        0        0      858 2024-04-28 00:58:20.387591 lute3-3.4.2/lute/db/language_defs/gothic/definition.yaml
--rw-r--r--   0        0        0     1317 2024-04-28 00:58:20.387839 lute3-3.4.2/lute/db/language_defs/gothic/story_1.txt
--rw-r--r--   0        0        0      635 2024-04-28 00:58:20.388044 lute3-3.4.2/lute/db/language_defs/greek/definition.yaml
--rw-r--r--   0        0        0     1649 2024-04-28 00:58:20.388167 lute3-3.4.2/lute/db/language_defs/greek/gr_demo.txt
--rw-r--r--   0        0        0     2165 2024-04-28 00:58:20.388512 lute3-3.4.2/lute/db/language_defs/hebrew/definition.yaml
--rw-r--r--   0        0        0      945 2024-04-28 00:58:20.388804 lute3-3.4.2/lute/db/language_defs/hebrew/story_1.txt
--rw-r--r--   0        0        0      566 2024-04-28 00:58:20.389048 lute3-3.4.2/lute/db/language_defs/hindi/definition.yaml
--rw-r--r--   0        0        0      587 2024-04-28 00:58:20.389500 lute3-3.4.2/lute/db/language_defs/hindi/hi_wikipedia.txt
--rw-r--r--   0        0        0     2484 2024-04-28 00:58:20.389944 lute3-3.4.2/lute/db/language_defs/hungarian/definition.yaml
--rw-r--r--   0        0        0      308 2024-04-28 00:58:20.390708 lute3-3.4.2/lute/db/language_defs/hungarian/satantango_film_description.txt
--rw-r--r--   0        0        0     1505 2024-04-28 00:58:20.391114 lute3-3.4.2/lute/db/language_defs/icelandic/definition.yaml
--rw-r--r--   0        0        0     1262 2024-04-28 00:58:20.391519 lute3-3.4.2/lute/db/language_defs/icelandic/story_1.txt
--rw-r--r--   0        0        0      868 2024-04-28 00:58:20.392430 lute3-3.4.2/lute/db/language_defs/indonesian/definition.yaml
--rw-r--r--   0        0        0      643 2024-04-28 00:58:20.393006 lute3-3.4.2/lute/db/language_defs/indonesian/kura-kura_yang_sombong.txt
--rw-r--r--   0        0        0     3101 2024-04-28 00:58:20.394776 lute3-3.4.2/lute/db/language_defs/italian/definition.yaml
--rw-r--r--   0        0        0      905 2024-04-28 00:58:20.395281 lute3-3.4.2/lute/db/language_defs/italian/le_avventure_di_pinocchio.txt
--rw-r--r--   0        0        0      539 2024-04-28 00:58:20.395499 lute3-3.4.2/lute/db/language_defs/japanese/definition.yaml
--rw-r--r--   0        0        0      428 2024-04-28 00:58:20.398623 lute3-3.4.2/lute/db/language_defs/japanese/jp_kitakaze_to_taiyou.txt
--rw-r--r--   0        0        0     2188 2024-04-28 00:58:20.399079 lute3-3.4.2/lute/db/language_defs/latin/definition.yaml
--rw-r--r--   0        0        0      497 2024-04-28 00:58:20.399384 lute3-3.4.2/lute/db/language_defs/latin/story_1.txt
--rw-r--r--   0        0        0     1796 2024-04-28 00:58:20.400015 lute3-3.4.2/lute/db/language_defs/latvian/definition.yaml
--rw-r--r--   0        0        0      562 2024-04-28 00:58:20.415069 lute3-3.4.2/lute/db/language_defs/latvian/story_1.txt
--rw-r--r--   0        0        0     1850 2024-04-28 00:58:20.424530 lute3-3.4.2/lute/db/language_defs/lithuanian/definition.yaml
--rw-r--r--   0        0        0     1104 2024-04-28 00:58:20.425240 lute3-3.4.2/lute/db/language_defs/lithuanian/story_1.txt
--rw-r--r--   0        0        0      416 2024-05-17 21:40:35.334109 lute3-3.4.2/lute/db/language_defs/mandarin_chinese/definition.yaml
--rw-r--r--   0        0        0     1064 2024-05-17 21:40:35.334787 lute3-3.4.2/lute/db/language_defs/mandarin_chinese/story_1.txt
--rw-r--r--   0        0        0      800 2024-04-28 00:58:20.427807 lute3-3.4.2/lute/db/language_defs/norwegian/definition.yaml
--rw-r--r--   0        0        0      955 2024-04-28 00:58:20.428215 lute3-3.4.2/lute/db/language_defs/norwegian/vildanden.txt
--rw-r--r--   0        0        0     1141 2024-04-28 00:58:20.428571 lute3-3.4.2/lute/db/language_defs/polish/adam_i_smoczy_skarb.txt
--rw-r--r--   0        0        0     2903 2024-04-28 00:58:20.428846 lute3-3.4.2/lute/db/language_defs/polish/definition.yaml
--rw-r--r--   0        0        0     1047 2024-04-28 00:58:20.429230 lute3-3.4.2/lute/db/language_defs/portuguese/a_maldicao.txt
--rw-r--r--   0        0        0     3471 2024-04-28 00:58:20.429552 lute3-3.4.2/lute/db/language_defs/portuguese/definition.yaml
--rw-r--r--   0        0        0     1143 2024-04-28 00:58:20.430104 lute3-3.4.2/lute/db/language_defs/punjabi/definition.yaml
--rw-r--r--   0        0        0     1390 2024-04-28 00:58:20.431321 lute3-3.4.2/lute/db/language_defs/punjabi/story_1.txt
--rw-r--r--   0        0        0       14 2024-04-28 00:58:20.431532 lute3-3.4.2/lute/db/language_defs/requirements.txt
--rw-r--r--   0        0        0     2898 2024-04-28 00:58:20.433435 lute3-3.4.2/lute/db/language_defs/romanian/definition.yaml
--rw-r--r--   0        0        0      472 2024-04-28 00:58:20.475856 lute3-3.4.2/lute/db/language_defs/romanian/story_1.txt
--rw-r--r--   0        0        0      470 2024-04-28 00:58:20.476336 lute3-3.4.2/lute/db/language_defs/russian/definition.yaml
--rw-r--r--   0        0        0      546 2024-04-28 00:58:20.476620 lute3-3.4.2/lute/db/language_defs/russian/ru_medved.txt
--rw-r--r--   0        0        0      477 2024-04-28 00:58:20.476859 lute3-3.4.2/lute/db/language_defs/sanskrit/definition.yaml
--rw-r--r--   0        0        0     1027 2024-04-28 00:58:20.477000 lute3-3.4.2/lute/db/language_defs/sanskrit/sanskrit.txt
--rw-r--r--   0        0        0     1028 2024-04-28 00:58:20.477572 lute3-3.4.2/lute/db/language_defs/serbian/definition.yaml
--rw-r--r--   0        0        0      740 2024-04-28 00:58:20.478677 lute3-3.4.2/lute/db/language_defs/serbian/story_1.txt
--rw-r--r--   0        0        0     2055 2024-04-28 00:58:20.479331 lute3-3.4.2/lute/db/language_defs/slovak/definition.yaml
--rw-r--r--   0        0        0      729 2024-04-28 00:58:20.479609 lute3-3.4.2/lute/db/language_defs/slovak/story_1.txt
--rw-r--r--   0        0        0     1644 2024-04-28 00:58:20.479985 lute3-3.4.2/lute/db/language_defs/slovene/definition.yaml
--rw-r--r--   0        0        0      464 2024-04-28 00:58:20.480514 lute3-3.4.2/lute/db/language_defs/slovene/story_1.txt
--rw-r--r--   0        0        0      526 2024-04-28 00:58:20.480755 lute3-3.4.2/lute/db/language_defs/spanish/definition.yaml
--rw-r--r--   0        0        0      534 2024-04-28 00:58:20.480873 lute3-3.4.2/lute/db/language_defs/spanish/es_aladino.txt
--rw-r--r--   0        0        0     1302 2024-04-28 00:58:20.481695 lute3-3.4.2/lute/db/language_defs/swahili/definition.yaml
--rw-r--r--   0        0        0      755 2024-04-28 00:58:20.482368 lute3-3.4.2/lute/db/language_defs/swahili/story_1.txt
--rw-r--r--   0        0        0     2821 2024-04-28 00:58:20.482938 lute3-3.4.2/lute/db/language_defs/swedish/definition.yaml
--rw-r--r--   0        0        0      566 2024-04-28 00:58:20.483259 lute3-3.4.2/lute/db/language_defs/swedish/story_1.txt
--rw-r--r--   0        0        0     1858 2024-04-28 00:58:20.483690 lute3-3.4.2/lute/db/language_defs/tibetan/definition.yaml
--rw-r--r--   0        0        0     1464 2024-04-28 00:58:20.484308 lute3-3.4.2/lute/db/language_defs/tibetan/story_1.txt
--rw-r--r--   0        0        0      497 2024-04-28 00:58:20.484692 lute3-3.4.2/lute/db/language_defs/turkish/definition.yaml
--rw-r--r--   0        0        0      941 2024-04-28 00:58:20.484816 lute3-3.4.2/lute/db/language_defs/turkish/tr_demo.txt
--rw-r--r--   0        0        0     2211 2024-04-28 00:58:20.485815 lute3-3.4.2/lute/db/language_defs/ukrainian/definition.yaml
--rw-r--r--   0        0        0     1034 2024-04-28 00:58:20.486326 lute3-3.4.2/lute/db/language_defs/ukrainian/story_1.txt
--rw-r--r--   0        0        0     1773 2024-04-28 00:58:20.486478 lute3-3.4.2/lute/db/language_defs/verify_files.py
--rw-r--r--   0        0        0      798 2024-04-28 00:58:20.487001 lute3-3.4.2/lute/db/language_defs/vietnamese/definition.yaml
--rw-r--r--   0        0        0      658 2024-04-28 00:58:20.487378 lute3-3.4.2/lute/db/language_defs/vietnamese/lan_bien.txt
--rw-r--r--   0        0        0      615 2023-11-09 09:07:06.767671 lute3-3.4.2/lute/db/management.py
--rw-r--r--   0        0        0     1620 2023-10-26 01:04:31.825247 lute3-3.4.2/lute/db/schema/README.md
--rw-r--r--   0        0        0    42817 2024-05-30 03:00:27.948552 lute3-3.4.2/lute/db/schema/baseline.sql
--rw-r--r--   0        0        0     8817 2024-03-08 03:05:01.856057 lute3-3.4.2/lute/db/schema/empty.sql
--rw-r--r--   0        0        0      246 2023-10-20 18:48:10.168442 lute3-3.4.2/lute/db/schema/migrations/20230409_224327_load_statuses.sql
--rw-r--r--   0        0        0      178 2023-10-20 18:48:10.168634 lute3-3.4.2/lute/db/schema/migrations/20230414_225828_add_texttokens_TokTextLC.sql
--rw-r--r--   0        0        0      245 2023-10-20 18:48:10.168826 lute3-3.4.2/lute/db/schema/migrations/20230428_224656_create_wordflashmessages_table.sql
--rw-r--r--   0        0        0     2067 2023-10-20 18:48:10.169209 lute3-3.4.2/lute/db/schema/migrations/20230518_190000_remove_old_words_fields.sql
--rw-r--r--   0        0        0      680 2023-10-20 18:48:10.169512 lute3-3.4.2/lute/db/schema/migrations/20230519_194627_add_TxDateRead.sql
--rw-r--r--   0        0        0       96 2023-10-20 18:48:10.169708 lute3-3.4.2/lute/db/schema/migrations/20230621_010000_drop_texttags_table.sql
--rw-r--r--   0        0        0     1143 2023-10-20 18:48:10.169918 lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_01_booktags.sql
--rw-r--r--   0        0        0     1141 2023-10-20 18:48:10.170132 lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_02_wordtags.sql
--rw-r--r--   0        0        0     1226 2023-10-20 18:48:10.170317 lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_03_sentences.sql
--rw-r--r--   0        0        0     1214 2023-10-20 18:48:10.170503 lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_04_texttokens.sql
--rw-r--r--   0        0        0     1559 2023-10-20 18:48:10.170690 lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_05_texts.sql
--rw-r--r--   0        0        0     1147 2023-10-20 18:48:10.170868 lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_06_bookstats.sql
--rw-r--r--   0        0        0     1038 2023-10-20 18:48:10.171044 lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_07_termimages.sql
--rw-r--r--   0        0        0     1044 2023-10-20 18:48:10.171217 lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_08_wordflashmessages.sql
--rw-r--r--   0        0        0     1213 2023-10-20 18:48:10.171396 lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_09_wordparents.sql
--rw-r--r--   0        0        0     2022 2023-10-20 18:48:10.171568 lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_10_words.sql
--rw-r--r--   0        0        0     1227 2023-10-20 18:48:10.171723 lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_11_books.sql
--rw-r--r--   0        0        0       56 2023-10-20 18:48:10.171870 lute3-3.4.2/lute/db/schema/migrations/20230623_234104_drop_TxTitle.sql
--rw-r--r--   0        0        0       38 2023-10-20 18:48:10.172012 lute3-3.4.2/lute/db/schema/migrations/20230624_182104_drop_index_TxBkIDTxOrder.sql
--rw-r--r--   0        0        0      908 2023-10-20 18:48:10.172172 lute3-3.4.2/lute/db/schema/migrations/20230818_201200_add_BkWordCount.sql
--rw-r--r--   0        0        0       87 2023-10-20 18:48:10.172337 lute3-3.4.2/lute/db/schema/migrations/20230819_044107_drop_texttokens.sql
--rw-r--r--   0        0        0      168 2023-10-20 18:48:10.172618 lute3-3.4.2/lute/db/schema/migrations/20230819_050036_vacuum.sql
--rw-r--r--   0        0        0      736 2023-10-20 18:48:10.172795 lute3-3.4.2/lute/db/schema/migrations/20230827_052154_allow_multiple_word_parents.sql
--rw-r--r--   0        0        0     1031 2023-10-20 18:48:10.173096 lute3-3.4.2/lute/db/schema/migrations/20231018_211236_remove_excess_texts_fields.sql
--rw-r--r--   0        0        0      930 2023-11-03 01:33:16.686624 lute3-3.4.2/lute/db/schema/migrations/20231101_203811_modify_settings_schema.sql
--rw-r--r--   0        0        0      114 2024-01-13 04:05:05.209858 lute3-3.4.2/lute/db/schema/migrations/20231130_141236_add_TxWordCount.sql
--rw-r--r--   0        0        0      194 2024-01-13 04:05:05.210324 lute3-3.4.2/lute/db/schema/migrations/20231210_103924_add_book_audio_fields.sql
--rw-r--r--   0        0        0       65 2024-02-07 07:50:18.754352 lute3-3.4.2/lute/db/schema/migrations/20240101_122610_add_bookstats_status_distribution.sql
--rw-r--r--   0        0        0       70 2024-02-07 07:50:18.754640 lute3-3.4.2/lute/db/schema/migrations/20240113_215142_add_term_follow_parent_bool.sql
--rw-r--r--   0        0        0      194 2024-02-07 07:50:18.754951 lute3-3.4.2/lute/db/schema/migrations/20240118_154258_change_status_abbrev.sql
--rw-r--r--   0        0        0     1487 2024-02-07 07:50:18.755302 lute3-3.4.2/lute/db/schema/migrations/20240125_drop_BkWordCount.sql
--rw-r--r--   0        0        0     1188 2024-02-07 07:50:18.755674 lute3-3.4.2/lute/db/schema/migrations/20240125_drop_bookstats_wordcount.sql
--rw-r--r--   0        0        0     1877 2024-02-19 02:42:49.355669 lute3-3.4.2/lute/db/schema/migrations/20240207_01_create_languagedicts.sql
--rw-r--r--   0        0        0     1570 2024-02-19 02:42:49.355795 lute3-3.4.2/lute/db/schema/migrations/20240207_02_drop_old_language_fields.sql
--rw-r--r--   0        0        0      224 2023-10-20 18:48:10.173345 lute3-3.4.2/lute/db/schema/migrations/README.md
--rw-r--r--   0        0        0      222 2023-11-03 01:33:16.686865 lute3-3.4.2/lute/db/schema/migrations_repeatable/README.md
--rw-r--r--   0        0        0      992 2024-02-07 07:50:18.756034 lute3-3.4.2/lute/db/schema/migrations_repeatable/trig_wordparents.sql
--rw-r--r--   0        0        0     1751 2024-03-25 09:32:17.264354 lute3-3.4.2/lute/db/schema/migrations_repeatable/trig_words.sql
--rw-r--r--   0        0        0       36 2023-11-03 01:33:16.687020 lute3-3.4.2/lute/db/schema/migrations_repeatable/vacuum.sql
--rw-r--r--   0        0        0        0 2023-10-20 18:48:10.173889 lute3-3.4.2/lute/db/setup/__init__.py
--rw-r--r--   0        0        0     5201 2023-11-11 22:05:26.094785 lute3-3.4.2/lute/db/setup/main.py
--rw-r--r--   0        0        0     3726 2023-11-08 00:06:31.606907 lute3-3.4.2/lute/db/setup/migrator.py
--rw-r--r--   0        0        0        0 2023-11-01 07:45:01.506123 lute3-3.4.2/lute/dev_api/__init__.py
--rw-r--r--   0        0        0     5105 2024-05-18 03:42:18.963958 lute3-3.4.2/lute/dev_api/routes.py
--rw-r--r--   0        0        0        0 2023-10-16 06:20:14.170764 lute3-3.4.2/lute/language/__init__.py
--rw-r--r--   0        0        0     3129 2024-05-06 03:26:32.112645 lute3-3.4.2/lute/language/forms.py
--rw-r--r--   0        0        0     6556 2024-05-27 23:47:17.824457 lute3-3.4.2/lute/language/routes.py
--rw-r--r--   0        0        0     2315 2024-05-18 03:42:18.964238 lute3-3.4.2/lute/language/service.py
--rw-r--r--   0        0        0     3946 2024-05-19 18:38:13.896119 lute3-3.4.2/lute/main.py
--rw-r--r--   0        0        0        0 2023-10-04 05:48:35.020519 lute3-3.4.2/lute/models/__init__.py
--rw-r--r--   0        0        0    11122 2024-03-15 03:25:40.869518 lute3-3.4.2/lute/models/book.py
--rw-r--r--   0        0        0     8838 2024-05-27 23:47:17.824713 lute3-3.4.2/lute/models/language.py
--rw-r--r--   0        0        0     8672 2024-03-13 16:31:06.436856 lute3-3.4.2/lute/models/setting.py
--rw-r--r--   0        0        0    11351 2024-04-28 00:44:07.954290 lute3-3.4.2/lute/models/term.py
--rw-r--r--   0        0        0        0 2023-10-07 05:09:39.898452 lute3-3.4.2/lute/parse/__init__.py
--rw-r--r--   0        0        0     4429 2024-05-27 23:47:17.824945 lute3-3.4.2/lute/parse/base.py
--rw-r--r--   0        0        0     1646 2023-11-08 00:06:31.610408 lute3-3.4.2/lute/parse/character_parser.py
--rw-r--r--   0        0        0     4735 2024-03-08 03:05:01.859524 lute3-3.4.2/lute/parse/mecab_parser.py
--rw-r--r--   0        0        0     2619 2024-05-27 23:47:17.825152 lute3-3.4.2/lute/parse/registry.py
--rw-r--r--   0        0        0     9245 2024-05-18 17:10:47.841027 lute3-3.4.2/lute/parse/space_delimited_parser.py
--rw-r--r--   0        0        0        0 2023-10-16 06:20:14.172648 lute3-3.4.2/lute/read/__init__.py
--rw-r--r--   0        0        0      211 2023-11-08 00:06:31.611930 lute3-3.4.2/lute/read/forms.py
--rw-r--r--   0        0        0        0 2023-10-18 06:43:42.367570 lute3-3.4.2/lute/read/render/__init__.py
--rw-r--r--   0        0        0    17309 2024-05-06 03:26:32.113398 lute3-3.4.2/lute/read/render/renderable_calculator.py
--rw-r--r--   0        0        0     5678 2024-05-28 16:43:48.081846 lute3-3.4.2/lute/read/render/service.py
--rw-r--r--   0        0        0     7010 2024-05-18 17:10:47.841748 lute3-3.4.2/lute/read/routes.py
--rw-r--r--   0        0        0     6636 2024-05-28 14:59:34.117162 lute3-3.4.2/lute/read/service.py
--rw-r--r--   0        0        0        0 2023-11-03 06:31:15.939906 lute3-3.4.2/lute/settings/__init__.py
--rw-r--r--   0        0        0     5329 2024-05-06 03:26:32.114141 lute3-3.4.2/lute/settings/routes.py
--rw-r--r--   0        0        0     1738 2023-10-04 05:48:35.022956 lute3-3.4.2/lute/static/css/images/animated-overlay.gif
--rw-r--r--   0        0        0     2434 2023-10-04 05:48:35.023257 lute3-3.4.2/lute/static/css/images/jplayer-black-and-yellow.png
--rw-r--r--   0        0        0    14525 2023-10-04 05:48:35.023672 lute3-3.4.2/lute/static/css/images/jplayer.blue.monday.jpg
--rw-r--r--   0        0        0   304064 2023-10-04 05:48:35.024510 lute3-3.4.2/lute/static/css/images/pbar-ani.gif
--rw-r--r--   0        0        0      212 2023-10-04 05:48:35.024852 lute3-3.4.2/lute/static/css/images/ui-bg_flat_0_555555_40x100.png
--rw-r--r--   0        0        0      180 2023-10-04 05:48:35.025123 lute3-3.4.2/lute/static/css/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-r--r--   0        0        0      220 2023-10-04 05:48:35.025729 lute3-3.4.2/lute/static/css/images/ui-bg_flat_75_222222_40x100.png
--rw-r--r--   0        0        0      220 2023-10-04 05:48:35.026029 lute3-3.4.2/lute/static/css/images/ui-bg_flat_75_444444_40x100.png
--rw-r--r--   0        0        0      178 2023-10-04 05:48:35.026359 lute3-3.4.2/lute/static/css/images/ui-bg_flat_75_ffffff_40x100.png
--rw-r--r--   0        0        0      120 2023-10-04 05:48:35.026642 lute3-3.4.2/lute/static/css/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0        0        0      105 2023-10-04 05:48:35.026929 lute3-3.4.2/lute/static/css/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0        0        0      111 2023-10-04 05:48:35.027288 lute3-3.4.2/lute/static/css/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0        0        0      110 2023-10-04 05:48:35.027566 lute3-3.4.2/lute/static/css/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0        0        0      119 2023-10-04 05:48:35.027847 lute3-3.4.2/lute/static/css/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0        0        0      277 2023-10-04 05:48:35.028257 lute3-3.4.2/lute/static/css/images/ui-bg_highlight-soft_75_222222_1x100.png
--rw-r--r--   0        0        0      101 2023-10-04 05:48:35.028513 lute3-3.4.2/lute/static/css/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0        0        0      251 2023-10-04 05:48:35.028793 lute3-3.4.2/lute/static/css/images/ui-bg_inset-hard_55_333333_1x100.png
--rw-r--r--   0        0        0      251 2023-10-04 05:48:35.029316 lute3-3.4.2/lute/static/css/images/ui-bg_inset-hard_95_444444_1x100.png
--rw-r--r--   0        0        0     4369 2023-10-04 05:48:35.029681 lute3-3.4.2/lute/static/css/images/ui-icons_222222_256x240.png
--rw-r--r--   0        0        0     4369 2023-10-04 05:48:35.030066 lute3-3.4.2/lute/static/css/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0        0        0     6992 2023-10-04 05:48:35.030537 lute3-3.4.2/lute/static/css/images/ui-icons_444444_256x240.png
--rw-r--r--   0        0        0     4369 2023-10-04 05:48:35.030833 lute3-3.4.2/lute/static/css/images/ui-icons_454545_256x240.png
--rw-r--r--   0        0        0     6988 2023-10-04 05:48:35.031207 lute3-3.4.2/lute/static/css/images/ui-icons_555555_256x240.png
--rw-r--r--   0        0        0     4549 2023-10-04 05:48:35.031493 lute3-3.4.2/lute/static/css/images/ui-icons_777620_256x240.png
--rw-r--r--   0        0        0     6999 2023-10-04 05:48:35.031792 lute3-3.4.2/lute/static/css/images/ui-icons_777777_256x240.png
--rw-r--r--   0        0        0     4369 2023-10-04 05:48:35.032071 lute3-3.4.2/lute/static/css/images/ui-icons_888888_256x240.png
--rw-r--r--   0        0        0     6991 2023-10-04 05:48:35.032366 lute3-3.4.2/lute/static/css/images/ui-icons_BBBBBB_256x240.png
--rw-r--r--   0        0        0     4549 2023-10-04 05:48:35.032703 lute3-3.4.2/lute/static/css/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0        0        0     4369 2023-10-04 05:48:35.033223 lute3-3.4.2/lute/static/css/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0        0        0     6299 2023-10-04 05:48:35.033571 lute3-3.4.2/lute/static/css/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0     8434 2024-04-28 00:44:07.956083 lute3-3.4.2/lute/static/css/player-styles.css
--rw-r--r--   0        0        0    40959 2024-05-18 03:42:18.965669 lute3-3.4.2/lute/static/css/styles.css
--rw-r--r--   0        0        0    15406 2023-10-04 05:48:35.035622 lute3-3.4.2/lute/static/favicon.ico
--rw-r--r--   0        0        0    15406 2023-10-04 05:48:35.036140 lute3-3.4.2/lute/static/favicon_dev.ico
--rw-r--r--   0        0        0      485 2023-10-04 05:48:35.036488 lute3-3.4.2/lute/static/icn/arrow-000-medium.png
--rw-r--r--   0        0        0      479 2023-10-04 05:48:35.036809 lute3-3.4.2/lute/static/icn/arrow-180-medium.png
--rw-r--r--   0        0        0      811 2023-10-04 05:48:35.037131 lute3-3.4.2/lute/static/icn/arrow-circle-135.png
--rw-r--r--   0        0        0      790 2023-10-04 05:48:35.037385 lute3-3.4.2/lute/static/icn/arrow-circle-225-left.png
--rw-r--r--   0        0        0      786 2023-10-04 05:48:35.037680 lute3-3.4.2/lute/static/icn/arrow-circle-315.png
--rw-r--r--   0        0        0      485 2023-10-04 05:48:35.037925 lute3-3.4.2/lute/static/icn/arrow-norepeat.png
--rw-r--r--   0        0        0      587 2023-10-04 05:48:35.038190 lute3-3.4.2/lute/static/icn/arrow-repeat.png
--rw-r--r--   0        0        0      601 2023-10-04 05:48:35.038457 lute3-3.4.2/lute/static/icn/arrow-stop.png
--rw-r--r--   0        0        0      622 2023-10-04 05:48:35.038703 lute3-3.4.2/lute/static/icn/book--pencil.png
--rw-r--r--   0        0        0      650 2023-10-04 05:48:35.038940 lute3-3.4.2/lute/static/icn/book-open-bookmark.png
--rw-r--r--   0        0        0      613 2023-10-04 05:48:35.039204 lute3-3.4.2/lute/static/icn/book-open-text.png
--rw-r--r--   0        0        0      600 2024-02-19 02:42:49.358289 lute3-3.4.2/lute/static/icn/book-open-text.svg
--rw-r--r--   0        0        0      552 2024-01-13 04:05:05.217231 lute3-3.4.2/lute/static/icn/bookmark-off.svg
--rw-r--r--   0        0        0      414 2024-01-13 04:05:05.217572 lute3-3.4.2/lute/static/icn/bookmark-on.svg
--rw-r--r--   0        0        0      784 2023-10-04 05:48:35.039508 lute3-3.4.2/lute/static/icn/broom.png
--rw-r--r--   0        0        0      398 2023-10-04 05:48:35.039745 lute3-3.4.2/lute/static/icn/calculator.png
--rw-r--r--   0        0        0      405 2023-10-04 05:48:35.040009 lute3-3.4.2/lute/static/icn/card--minus.png
--rw-r--r--   0        0        0      556 2023-10-04 05:48:35.040231 lute3-3.4.2/lute/static/icn/card--pencil.png
--rw-r--r--   0        0        0      504 2023-10-04 05:48:35.040493 lute3-3.4.2/lute/static/icn/card--plus.png
--rw-r--r--   0        0        0      473 2023-10-04 05:48:35.040762 lute3-3.4.2/lute/static/icn/cards-stack.png
--rw-r--r--   0        0        0      434 2024-01-13 04:05:05.218143 lute3-3.4.2/lute/static/icn/caret-left.svg
--rw-r--r--   0        0        0      427 2024-01-13 04:05:05.218284 lute3-3.4.2/lute/static/icn/caret-right.svg
--rw-r--r--   0        0        0      369 2023-10-04 05:48:35.041070 lute3-3.4.2/lute/static/icn/chain.png
--rw-r--r--   0        0        0      624 2023-10-04 05:48:35.041330 lute3-3.4.2/lute/static/icn/clock.png
--rw-r--r--   0        0        0      952 2024-02-07 07:50:18.763469 lute3-3.4.2/lute/static/icn/close-white.svg
--rw-r--r--   0        0        0     1438 2024-01-13 04:05:05.219492 lute3-3.4.2/lute/static/icn/close.svg
--rw-r--r--   0        0        0      404 2023-10-04 05:48:35.041576 lute3-3.4.2/lute/static/icn/control-180.png
--rw-r--r--   0        0        0      511 2023-10-04 05:48:35.041944 lute3-3.4.2/lute/static/icn/control-stop-180.png
--rw-r--r--   0        0        0      523 2023-10-04 05:48:35.042219 lute3-3.4.2/lute/static/icn/control-stop.png
--rw-r--r--   0        0        0      405 2023-10-04 05:48:35.042485 lute3-3.4.2/lute/static/icn/control.png
--rw-r--r--   0        0        0      920 2023-10-04 05:48:35.042813 lute3-3.4.2/lute/static/icn/cross-big.png
--rw-r--r--   0        0        0      555 2023-10-04 05:48:35.043135 lute3-3.4.2/lute/static/icn/cross-button.png
--rw-r--r--   0        0        0      544 2023-10-04 05:48:35.043410 lute3-3.4.2/lute/static/icn/cross.png
--rw-r--r--   0        0        0      658 2023-10-04 05:48:35.043716 lute3-3.4.2/lute/static/icn/document--pencil.png
--rw-r--r--   0        0        0     1761 2024-02-07 07:50:18.763842 lute3-3.4.2/lute/static/icn/drag-handle.svg
--rw-r--r--   0        0        0      674 2023-10-04 05:48:35.043952 lute3-3.4.2/lute/static/icn/drawer--minus.png
--rw-r--r--   0        0        0      717 2023-10-04 05:48:35.044272 lute3-3.4.2/lute/static/icn/drawer--plus.png
--rwxr-xr-x   0        0        0       55 2023-10-04 05:48:35.044638 lute3-3.4.2/lute/static/icn/empty.gif
--rw-r--r--   0        0        0      680 2023-10-04 05:48:35.044851 lute3-3.4.2/lute/static/icn/eraser.png
--rw-r--r--   0        0        0      539 2023-10-04 05:48:35.045049 lute3-3.4.2/lute/static/icn/exclamation-button.png
--rw-r--r--   0        0        0      658 2023-10-04 05:48:35.045241 lute3-3.4.2/lute/static/icn/exclamation-red.png
--rw-r--r--   0        0        0      685 2023-10-04 05:48:35.045451 lute3-3.4.2/lute/static/icn/external.png
--rw-r--r--   0        0        0      536 2023-10-04 05:48:35.045663 lute3-3.4.2/lute/static/icn/eye.png
--rw-r--r--   0        0        0      792 2023-10-04 05:48:35.045884 lute3-3.4.2/lute/static/icn/feed--pencil.png
--rw-r--r--   0        0        0      737 2023-10-04 05:48:35.046102 lute3-3.4.2/lute/static/icn/feed--plus.png
--rw-r--r--   0        0        0      566 2024-01-13 04:05:05.221040 lute3-3.4.2/lute/static/icn/ff.svg
--rw-r--r--   0        0        0     1297 2024-01-13 04:05:05.221203 lute3-3.4.2/lute/static/icn/font-decrease.svg
--rw-r--r--   0        0        0     1378 2024-01-13 04:05:05.221326 lute3-3.4.2/lute/static/icn/font-increase.svg
--rw-r--r--   0        0        0      630 2023-10-04 05:48:35.046306 lute3-3.4.2/lute/static/icn/funnel--minus.png
--rw-r--r--   0        0        0      543 2023-10-04 05:48:35.046715 lute3-3.4.2/lute/static/icn/funnel.png
--rw-r--r--   0        0        0      617 2024-02-19 02:42:49.358629 lute3-3.4.2/lute/static/icn/images.svg
--rw-r--r--   0        0        0      692 2023-10-04 05:48:35.047033 lute3-3.4.2/lute/static/icn/inbox-download.png
--rw-r--r--   0        0        0      674 2023-10-04 05:48:35.047235 lute3-3.4.2/lute/static/icn/inbox-upload.png
--rw-r--r--   0        0        0     1553 2023-10-04 05:48:35.047472 lute3-3.4.2/lute/static/icn/indicator.gif
--rw-r--r--   0        0        0     1039 2023-10-04 05:48:35.047683 lute3-3.4.2/lute/static/icn/light-bulb-A.png
--rw-r--r--   0        0        0     1037 2023-10-04 05:48:35.047913 lute3-3.4.2/lute/static/icn/light-bulb-T.png
--rw-r--r--   0        0        0     1010 2023-10-04 05:48:35.048117 lute3-3.4.2/lute/static/icn/light-bulb-off-A.png
--rw-r--r--   0        0        0     1001 2023-10-04 05:48:35.048320 lute3-3.4.2/lute/static/icn/light-bulb-off-T.png
--rw-r--r--   0        0        0      943 2023-10-04 05:48:35.048686 lute3-3.4.2/lute/static/icn/light-bulb-off.png
--rw-r--r--   0        0        0      947 2023-10-04 05:48:35.048956 lute3-3.4.2/lute/static/icn/light-bulb.png
--rw-r--r--   0        0        0      631 2023-10-04 05:48:35.049160 lute3-3.4.2/lute/static/icn/lightning.png
--rw-r--r--   0        0        0     1687 2024-01-13 04:05:05.222154 lute3-3.4.2/lute/static/icn/line-spacing-decrease.svg
--rw-r--r--   0        0        0     2575 2024-01-13 04:05:05.222293 lute3-3.4.2/lute/static/icn/line-spacing-increase.svg
--rw-r--r--   0        0        0      277 2024-02-19 02:42:49.358831 lute3-3.4.2/lute/static/icn/list.svg
--rw-r--r--   0        0        0      451 2023-10-04 05:48:35.049360 lute3-3.4.2/lute/static/icn/minus-button.png
--rw-r--r--   0        0        0      259 2023-10-04 05:48:35.049740 lute3-3.4.2/lute/static/icn/minus.png
--rw-r--r--   0        0        0      489 2023-10-04 05:48:35.049931 lute3-3.4.2/lute/static/icn/navigation-000-button-light.png
--rw-r--r--   0        0        0      614 2023-10-04 05:48:35.050311 lute3-3.4.2/lute/static/icn/navigation-000-button.png
--rw-r--r--   0        0        0      486 2023-10-04 05:48:35.050548 lute3-3.4.2/lute/static/icn/navigation-180-button-light.png
--rw-r--r--   0        0        0      620 2023-10-04 05:48:35.050750 lute3-3.4.2/lute/static/icn/navigation-180-button.png
--rw-r--r--   0        0        0      607 2023-10-04 05:48:35.050975 lute3-3.4.2/lute/static/icn/new_line.png
--rw-r--r--   0        0        0      458 2024-01-13 04:05:05.222661 lute3-3.4.2/lute/static/icn/next.svg
--rw-r--r--   0        0        0      633 2023-10-04 05:48:35.051264 lute3-3.4.2/lute/static/icn/notebook--minus.png
--rw-r--r--   0        0        0      723 2023-10-04 05:48:35.051477 lute3-3.4.2/lute/static/icn/notebook--pencil.png
--rw-r--r--   0        0        0      664 2023-10-04 05:48:35.051850 lute3-3.4.2/lute/static/icn/notebook--plus.png
--rw-r--r--   0        0        0      541 2023-10-04 05:48:35.052045 lute3-3.4.2/lute/static/icn/notebook.png
--rw-r--r--   0        0        0      790 2024-01-13 04:05:05.223020 lute3-3.4.2/lute/static/icn/open.svg
--rw-r--r--   0        0        0      428 2024-01-13 04:05:05.223265 lute3-3.4.2/lute/static/icn/pause.svg
--rw-r--r--   0        0        0      475 2023-10-04 05:48:35.052249 lute3-3.4.2/lute/static/icn/pencil.png
--rw-r--r--   0        0        0     1154 2023-10-04 05:48:35.052521 lute3-3.4.2/lute/static/icn/photo-album.png
--rw-r--r--   0        0        0      591 2024-01-13 04:05:05.223508 lute3-3.4.2/lute/static/icn/pin.svg
--rw-r--r--   0        0        0      142 2023-10-04 05:48:35.052720 lute3-3.4.2/lute/static/icn/placeholder.png
--rw-r--r--   0        0        0      461 2024-01-13 04:05:05.223871 lute3-3.4.2/lute/static/icn/play.svg
--rw-r--r--   0        0        0      583 2023-10-04 05:48:35.052918 lute3-3.4.2/lute/static/icn/plus-button.png
--rw-r--r--   0        0        0      521 2023-10-04 05:48:35.053238 lute3-3.4.2/lute/static/icn/plus.png
--rw-r--r--   0        0        0      445 2024-01-13 04:05:05.224128 lute3-3.4.2/lute/static/icn/prev.svg
--rw-r--r--   0        0        0      722 2023-10-04 05:48:35.053446 lute3-3.4.2/lute/static/icn/printer.png
--rw-r--r--   0        0        0      722 2023-10-04 05:48:35.053709 lute3-3.4.2/lute/static/icn/question-balloon.png
--rw-r--r--   0        0        0      924 2023-10-04 05:48:35.053893 lute3-3.4.2/lute/static/icn/question-frame.png
--rw-r--r--   0        0        0     1921 2024-02-07 07:50:18.764174 lute3-3.4.2/lute/static/icn/reload.png
--rw-r--r--   0        0        0      558 2024-01-13 04:05:05.224511 lute3-3.4.2/lute/static/icn/rewind.svg
--rw-r--r--   0        0        0      837 2023-10-04 05:48:35.054103 lute3-3.4.2/lute/static/icn/script-import.png
--rw-r--r--   0        0        0     1041 2024-03-13 16:31:06.440554 lute3-3.4.2/lute/static/icn/settings-gear-icon.svg
--rw-r--r--   0        0        0      526 2024-01-13 04:05:05.224876 lute3-3.4.2/lute/static/icn/skip-back.svg
--rw-r--r--   0        0        0      755 2023-10-04 05:48:35.054284 lute3-3.4.2/lute/static/icn/smiley-sad.png
--rw-r--r--   0        0        0      811 2023-10-04 05:48:35.054463 lute3-3.4.2/lute/static/icn/smiley.png
--rw-r--r--   0        0        0      452 2023-10-04 05:48:35.054648 lute3-3.4.2/lute/static/icn/speaker-volume-none.png
--rw-r--r--   0        0        0      543 2023-10-04 05:48:35.054955 lute3-3.4.2/lute/static/icn/speaker-volume.png
--rw-r--r--   0        0        0      757 2023-10-04 05:48:35.055365 lute3-3.4.2/lute/static/icn/star.png
--rw-r--r--   0        0        0      432 2023-10-04 05:48:35.055719 lute3-3.4.2/lute/static/icn/status-away.png
--rw-r--r--   0        0        0      407 2023-10-04 05:48:35.056570 lute3-3.4.2/lute/static/icn/status-busy.png
--rw-r--r--   0        0        0      401 2023-10-04 05:48:35.056940 lute3-3.4.2/lute/static/icn/status.png
--rw-r--r--   0        0        0      466 2023-10-04 05:48:35.057163 lute3-3.4.2/lute/static/icn/sticky-note--minus.png
--rw-r--r--   0        0        0      638 2023-10-04 05:48:35.057670 lute3-3.4.2/lute/static/icn/sticky-note--pencil.png
--rw-r--r--   0        0        0      571 2023-10-04 05:48:35.057865 lute3-3.4.2/lute/static/icn/sticky-note--plus.png
--rw-r--r--   0        0        0      520 2023-10-04 05:48:35.058304 lute3-3.4.2/lute/static/icn/sticky-note-text.png
--rw-r--r--   0        0        0      425 2023-10-04 05:48:35.058599 lute3-3.4.2/lute/static/icn/sticky-note.png
--rw-r--r--   0        0        0      533 2023-10-04 05:48:35.058808 lute3-3.4.2/lute/static/icn/sticky-notes-stack.png
--rw-r--r--   0        0        0      618 2023-10-04 05:48:35.059020 lute3-3.4.2/lute/static/icn/sticky-notes-text.png
--rw-r--r--   0        0        0      546 2023-10-04 05:48:35.059221 lute3-3.4.2/lute/static/icn/sticky-notes.png
--rw-r--r--   0        0        0     2805 2023-10-04 05:48:35.059585 lute3-3.4.2/lute/static/icn/test_correct.png
--rw-r--r--   0        0        0     2805 2023-10-04 05:48:35.059871 lute3-3.4.2/lute/static/icn/test_notyet.png
--rw-r--r--   0        0        0     2805 2023-10-04 05:48:35.060061 lute3-3.4.2/lute/static/icn/test_wrong.png
--rw-r--r--   0        0        0      803 2024-01-13 04:05:05.225875 lute3-3.4.2/lute/static/icn/text-column-one.svg
--rw-r--r--   0        0        0     1613 2024-01-13 04:05:05.226200 lute3-3.4.2/lute/static/icn/text-column-two.svg
--rw-r--r--   0        0        0      732 2023-10-04 05:48:35.060251 lute3-3.4.2/lute/static/icn/thumb-up.png
--rw-r--r--   0        0        0      751 2023-10-04 05:48:35.060509 lute3-3.4.2/lute/static/icn/thumb.png
--rwxr-xr-x   0        0        0      620 2023-10-04 05:48:35.060685 lute3-3.4.2/lute/static/icn/tick-button-small.png
--rw-r--r--   0        0        0      568 2023-10-04 05:48:35.060894 lute3-3.4.2/lute/static/icn/tick-button.png
--rw-r--r--   0        0        0      582 2023-10-04 05:48:35.061228 lute3-3.4.2/lute/static/icn/tick.png
--rw-r--r--   0        0        0      521 2024-01-13 04:05:05.226487 lute3-3.4.2/lute/static/icn/volume.svg
--rw-r--r--   0        0        0     3208 2023-10-04 05:48:35.061448 lute3-3.4.2/lute/static/icn/waiting.gif
--rw-r--r--   0        0        0      847 2023-10-04 05:48:35.061633 lute3-3.4.2/lute/static/icn/waiting2.gif
--rw-r--r--   0        0        0     5450 2023-10-04 05:48:35.061895 lute3-3.4.2/lute/static/icn/wizard.png
--rw-r--r--   0        0        0      916 2023-10-04 05:48:35.062193 lute3-3.4.2/lute/static/icn/wrench-screwdriver.png
--rw-r--r--   0        0        0    19567 2023-10-04 05:48:35.062586 lute3-3.4.2/lute/static/img/apple-touch-icon-114x114.png
--rw-r--r--   0        0        0     5618 2023-10-04 05:48:35.062872 lute3-3.4.2/lute/static/img/apple-touch-icon-57x57.png
--rw-r--r--   0        0        0     8461 2023-10-04 05:48:35.063084 lute3-3.4.2/lute/static/img/apple-touch-icon-72x72.png
--rw-r--r--   0        0        0    34198 2023-10-04 05:48:35.063762 lute3-3.4.2/lute/static/img/apple-touch-startup.png
--rw-r--r--   0        0        0    49403 2024-01-13 04:05:05.227551 lute3-3.4.2/lute/static/img/lute.png
--rw-r--r--   0        0        0     1405 2023-10-04 05:48:35.065233 lute3-3.4.2/lute/static/img/public_domain.png
--rw-r--r--   0        0        0     3764 2023-10-04 05:48:35.065440 lute3-3.4.2/lute/static/img/ui-icons_444444_256x240.png
--rw-r--r--   0        0        0     3767 2023-10-04 05:48:35.065634 lute3-3.4.2/lute/static/img/ui-icons_555555_256x240.png
--rw-r--r--   0        0        0     3767 2023-10-04 05:48:35.065982 lute3-3.4.2/lute/static/img/ui-icons_777620_256x240.png
--rw-r--r--   0        0        0     3764 2023-10-04 05:48:35.066190 lute3-3.4.2/lute/static/img/ui-icons_777777_256x240.png
--rw-r--r--   0        0        0     3764 2023-10-04 05:48:35.066397 lute3-3.4.2/lute/static/img/ui-icons_cc0000_256x240.png
--rw-r--r--   0        0        0     3764 2023-10-04 05:48:35.069007 lute3-3.4.2/lute/static/img/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    11246 2024-03-13 16:31:06.443010 lute3-3.4.2/lute/static/js/dict-tabs.js
--rw-r--r--   0        0        0    28222 2024-05-18 03:42:18.966179 lute3-3.4.2/lute/static/js/lute.js
--rw-r--r--   0        0        0    12092 2024-04-28 00:44:07.956926 lute3-3.4.2/lute/static/js/player.js
--rw-r--r--   0        0        0     8002 2024-05-06 03:26:32.114878 lute3-3.4.2/lute/static/js/resize.js
--rw-r--r--   0        0        0     4346 2024-02-07 07:50:18.767242 lute3-3.4.2/lute/static/js/text-options.js
--rw-r--r--   0        0        0   202357 2024-03-15 03:25:40.872972 lute3-3.4.2/lute/static/vendor/chartjs/chart.umd.js
--rw-r--r--   0        0        0    50650 2024-03-15 03:25:40.873223 lute3-3.4.2/lute/static/vendor/chartjs/chartjs-adapter-date-fns.js
--rw-r--r--   0        0        0      624 2024-03-15 03:25:40.873755 lute3-3.4.2/lute/static/vendor/datatables/README.md
--rw-r--r--   0        0        0     4145 2024-03-15 03:25:40.873884 lute3-3.4.2/lute/static/vendor/datatables/datatables.button.download.js
--rw-r--r--   0        0        0    41393 2024-03-15 03:25:40.874305 lute3-3.4.2/lute/static/vendor/datatables/datatables.min.css
--rw-r--r--   0        0        0   164670 2024-03-15 03:25:40.875473 lute3-3.4.2/lute/static/vendor/datatables/datatables.min.js
--rw-r--r--   0        0        0     5253 2024-03-15 03:25:40.876688 lute3-3.4.2/lute/static/vendor/jquery/jplayer.css
--rw-r--r--   0        0        0    34497 2024-03-15 03:25:40.876886 lute3-3.4.2/lute/static/vendor/jquery/jquery-ui.css
--rw-r--r--   0        0        0   240422 2024-03-15 03:25:40.879055 lute3-3.4.2/lute/static/vendor/jquery/jquery-ui.min.js
--rw-r--r--   0        0        0     1753 2024-03-15 03:25:40.879212 lute3-3.4.2/lute/static/vendor/jquery/jquery.hoverIntent.js
--rw-r--r--   0        0        0     8067 2024-03-15 03:25:40.879335 lute3-3.4.2/lute/static/vendor/jquery/jquery.jeditable.mini.js
--rw-r--r--   0        0        0    69303 2024-03-15 03:25:40.879593 lute3-3.4.2/lute/static/vendor/jquery/jquery.jplayer.js
--rw-r--r--   0        0        0    60951 2024-03-15 03:25:40.880095 lute3-3.4.2/lute/static/vendor/jquery/jquery.jplayer.min.js
--rw-r--r--   0        0        0    13714 2024-03-15 03:25:40.880340 lute3-3.4.2/lute/static/vendor/jquery/jquery.jplayer.swf
--rw-r--r--   0        0        0    97163 2024-03-15 03:25:40.880764 lute3-3.4.2/lute/static/vendor/jquery/jquery.js
--rwxr-xr-x   0        0        0     2442 2024-03-15 03:25:40.880893 lute3-3.4.2/lute/static/vendor/jquery/jquery.scrollTo.min.js
--rw-r--r--   0        0        0    80119 2024-03-15 03:25:40.881202 lute3-3.4.2/lute/static/vendor/jquery/jquery.xpath.min.js
--rw-r--r--   0        0        0    11207 2024-03-15 03:25:40.881421 lute3-3.4.2/lute/static/vendor/tagify/tagify.css
--rw-r--r--   0        0        0    60507 2024-03-15 03:25:40.881716 lute3-3.4.2/lute/static/vendor/tagify/tagify.min.js
--rw-r--r--   0        0        0    23275 2024-03-15 03:25:40.881883 lute3-3.4.2/lute/static/vendor/tagify/tagify.polyfills.min.js
--rw-r--r--   0        0        0     1723 2024-03-15 03:25:40.882103 lute3-3.4.2/lute/static/vendor/tagify/tagify_overrides.css
--rw-r--r--   0        0        0        0 2024-01-13 04:05:05.232444 lute3-3.4.2/lute/stats/__init__.py
--rw-r--r--   0        0        0      482 2024-01-13 04:05:05.232852 lute3-3.4.2/lute/stats/routes.py
--rw-r--r--   0        0        0     2702 2024-02-07 07:50:18.767674 lute3-3.4.2/lute/stats/service.py
--rw-r--r--   0        0        0     1134 2024-03-15 03:25:40.883026 lute3-3.4.2/lute/templates/backup/backup.html
--rw-r--r--   0        0        0      872 2024-02-19 02:42:49.360741 lute3-3.4.2/lute/templates/backup/index.html
--rw-r--r--   0        0        0     6842 2024-05-04 17:37:40.694306 lute3-3.4.2/lute/templates/base.html
--rw-r--r--   0        0        0     3080 2024-04-28 00:44:07.957672 lute3-3.4.2/lute/templates/book/create_new.html
--rw-r--r--   0        0        0     2503 2024-03-13 16:31:06.446279 lute3-3.4.2/lute/templates/book/edit.html
--rw-r--r--   0        0        0      627 2024-04-28 00:44:07.958136 lute3-3.4.2/lute/templates/book/import_webpage.html
--rw-r--r--   0        0        0      204 2023-11-09 21:55:59.870577 lute3-3.4.2/lute/templates/book/index.html
--rw-r--r--   0        0        0    10771 2024-05-18 01:00:02.776449 lute3-3.4.2/lute/templates/book/tablelisting.html
--rw-r--r--   0        0        0      651 2024-01-13 04:05:05.236118 lute3-3.4.2/lute/templates/errors/404_error.html
--rw-r--r--   0        0        0     1185 2024-01-13 04:05:05.236533 lute3-3.4.2/lute/templates/errors/500_error.html
--rw-r--r--   0        0        0     2278 2024-03-03 03:12:19.455018 lute3-3.4.2/lute/templates/hotkeys.html
--rw-r--r--   0        0        0     5206 2024-03-15 03:25:40.899605 lute3-3.4.2/lute/templates/imagesearch/index.html
--rw-r--r--   0        0        0     1278 2024-04-28 00:44:07.958527 lute3-3.4.2/lute/templates/index.html
--rw-r--r--   0        0        0     7009 2024-02-19 02:42:49.361906 lute3-3.4.2/lute/templates/language/_form.html
--rw-r--r--   0        0        0      131 2023-11-01 07:45:01.587557 lute3-3.4.2/lute/templates/language/edit.html
--rw-r--r--   0        0        0     1427 2024-04-28 00:44:07.958885 lute3-3.4.2/lute/templates/language/index.html
--rw-r--r--   0        0        0     1024 2024-04-28 00:44:07.959127 lute3-3.4.2/lute/templates/language/list_predefined.html
--rw-r--r--   0        0        0      533 2024-02-07 07:50:18.771534 lute3-3.4.2/lute/templates/language/new.html
--rw-r--r--   0        0        0     2522 2024-04-28 00:44:07.959518 lute3-3.4.2/lute/templates/read/audio_player.html
--rw-r--r--   0        0        0      551 2024-03-15 03:25:40.900713 lute3-3.4.2/lute/templates/read/flashcopied.html
--rw-r--r--   0        0        0     1885 2024-03-25 08:52:45.544428 lute3-3.4.2/lute/templates/read/frameform.html
--rw-r--r--   0        0        0    17938 2024-05-17 16:44:15.101791 lute3-3.4.2/lute/templates/read/index.html
--rw-r--r--   0        0        0      605 2024-02-07 07:50:18.773525 lute3-3.4.2/lute/templates/read/page_content.html
--rw-r--r--   0        0        0      755 2024-02-19 02:42:49.362657 lute3-3.4.2/lute/templates/read/page_edit_form.html
--rw-r--r--   0        0        0     4513 2024-05-18 03:42:18.966638 lute3-3.4.2/lute/templates/read/reading_menu.html
--rw-r--r--   0        0        0     1742 2024-03-15 03:25:40.903466 lute3-3.4.2/lute/templates/read/termpopup.html
--rw-r--r--   0        0        0      499 2024-03-08 03:05:01.875375 lute3-3.4.2/lute/templates/read/textitem.html
--rw-r--r--   0        0        0      643 2024-03-15 03:25:40.903763 lute3-3.4.2/lute/templates/read/updated.html
--rw-r--r--   0        0        0     4862 2024-04-28 00:44:07.959944 lute3-3.4.2/lute/templates/settings/form.html
--rw-r--r--   0        0        0     3807 2024-03-15 03:25:40.904464 lute3-3.4.2/lute/templates/stats/index.html
--rw-r--r--   0        0        0    12956 2024-04-28 00:44:07.960314 lute3-3.4.2/lute/templates/term/_form.html
--rw-r--r--   0        0        0     2215 2024-03-13 16:31:06.452196 lute3-3.4.2/lute/templates/term/formframes.html
--rw-r--r--   0        0        0    16104 2024-05-03 16:31:45.659974 lute3-3.4.2/lute/templates/term/index.html
--rw-r--r--   0        0        0     1579 2024-04-28 00:44:07.961040 lute3-3.4.2/lute/templates/term/sentences.html
--rw-r--r--   0        0        0      502 2024-03-15 03:25:40.905825 lute3-3.4.2/lute/templates/term_parent_map/index.html
--rw-r--r--   0        0        0     1093 2024-04-28 00:44:07.961536 lute3-3.4.2/lute/templates/termimport/index.html
--rw-r--r--   0        0        0      755 2024-04-28 00:44:07.961865 lute3-3.4.2/lute/templates/termtag/_form.html
--rw-r--r--   0        0        0      119 2023-10-30 05:47:07.311779 lute3-3.4.2/lute/templates/termtag/edit.html
--rw-r--r--   0        0        0     2654 2024-04-28 00:44:07.962237 lute3-3.4.2/lute/templates/termtag/index.html
--rw-r--r--   0        0        0      170 2023-10-30 05:47:07.312798 lute3-3.4.2/lute/templates/termtag/new.html
--rw-r--r--   0        0        0      654 2024-03-08 03:05:01.878803 lute3-3.4.2/lute/templates/version.html
--rw-r--r--   0        0        0        0 2023-10-21 00:58:40.674085 lute3-3.4.2/lute/term/__init__.py
--rw-r--r--   0        0        0     3353 2024-03-25 09:32:17.277337 lute3-3.4.2/lute/term/datatables.py
--rw-r--r--   0        0        0     4130 2024-03-25 09:32:17.278674 lute3-3.4.2/lute/term/forms.py
--rw-r--r--   0        0        0    16216 2024-04-28 00:44:07.962642 lute3-3.4.2/lute/term/model.py
--rw-r--r--   0        0        0     9475 2024-05-03 16:31:45.660379 lute3-3.4.2/lute/term/routes.py
--rw-r--r--   0        0        0        0 2023-10-28 20:14:27.720594 lute3-3.4.2/lute/term_parent_map/__init__.py
--rw-r--r--   0        0        0     1459 2024-03-15 03:25:40.907485 lute3-3.4.2/lute/term_parent_map/routes.py
--rw-r--r--   0        0        0      866 2024-03-15 03:25:40.907878 lute3-3.4.2/lute/term_parent_map/service.py
--rw-r--r--   0        0        0        0 2023-10-27 22:52:35.310439 lute3-3.4.2/lute/termimport/__init__.py
--rw-r--r--   0        0        0     1793 2024-03-25 09:32:17.280829 lute3-3.4.2/lute/termimport/routes.py
--rw-r--r--   0        0        0     9066 2024-05-11 22:55:05.266422 lute3-3.4.2/lute/termimport/service.py
--rw-r--r--   0        0        0        0 2023-10-30 05:47:07.312889 lute3-3.4.2/lute/termtag/__init__.py
--rw-r--r--   0        0        0      652 2023-11-08 00:06:31.617316 lute3-3.4.2/lute/termtag/datatables.py
--rw-r--r--   0        0        0      309 2023-11-08 00:06:31.617623 lute3-3.4.2/lute/termtag/forms.py
--rw-r--r--   0        0        0     1857 2023-11-08 00:06:31.617959 lute3-3.4.2/lute/termtag/routes.py
--rw-r--r--   0        0        0        0 2024-01-13 04:05:05.250549 lute3-3.4.2/lute/themes/__init__.py
--rw-r--r--   0        0        0     1021 2024-03-08 03:05:01.881349 lute3-3.4.2/lute/themes/css/Apple_Books.css
--rw-r--r--   0        0        0     2603 2024-03-15 03:25:40.908418 lute3-3.4.2/lute/themes/css/Dark_slate.css
--rw-r--r--   0        0        0      949 2024-03-13 16:30:50.208931 lute3-3.4.2/lute/themes/css/LWT.css
--rw-r--r--   0        0        0     1096 2024-03-13 16:30:50.209490 lute3-3.4.2/lute/themes/css/LingQ.css
--rw-r--r--   0        0        0     2835 2024-03-15 03:25:40.909175 lute3-3.4.2/lute/themes/css/Night.css
--rw-r--r--   0        0        0      174 2024-01-13 04:05:05.252115 lute3-3.4.2/lute/themes/css/README.md
--rw-r--r--   0        0        0     1153 2024-03-08 03:05:01.882428 lute3-3.4.2/lute/themes/routes.py
--rw-r--r--   0        0        0     2409 2024-05-06 03:26:32.116432 lute3-3.4.2/lute/themes/service.py
--rw-r--r--   0        0        0        0 2024-01-13 04:05:05.253134 lute3-3.4.2/lute/useraudio/__init__.py
--rw-r--r--   0        0        0      545 2024-01-13 04:05:05.253460 lute3-3.4.2/lute/useraudio/routes.py
--rw-r--r--   0        0        0        0 2023-10-24 05:43:55.069141 lute3-3.4.2/lute/userimage/__init__.py
--rw-r--r--   0        0        0      656 2023-11-08 00:06:31.618260 lute3-3.4.2/lute/userimage/routes.py
--rw-r--r--   0        0        0        0 2023-10-09 03:35:20.090603 lute3-3.4.2/lute/utils/__init__.py
--rw-r--r--   0        0        0     7072 2024-03-13 16:31:06.454810 lute3-3.4.2/lute/utils/data_tables.py
--rw-r--r--   0        0        0     2043 2024-02-07 07:50:18.794729 lute3-3.4.2/lute/utils/debug_helpers.py
--rw-r--r--   0        0        0     1326 2024-03-13 16:30:50.210892 lute3-3.4.2/lute/utils/formutils.py
--rw-r--r--   0        0        0      313 2024-05-18 03:42:18.966723 lute3-3.4.2/plugins/lute-mandarin/.pytest.ini
--rw-r--r--   0        0        0      205 2024-05-27 23:47:17.825356 lute3-3.4.2/plugins/lute-mandarin/README.md
--rw-r--r--   0        0        0     1365 2024-05-27 23:47:17.825551 lute3-3.4.2/plugins/lute-mandarin/README_PyPi.md
--rw-r--r--   0        0        0      416 2024-05-18 03:42:18.966791 lute3-3.4.2/plugins/lute-mandarin/definition.yaml
--rw-r--r--   0        0        0       52 2024-05-30 03:06:17.811546 lute3-3.4.2/plugins/lute-mandarin/lute_mandarin_parser/__init__.py
--rw-r--r--   0        0        0     4772 2024-05-27 23:47:17.826015 lute3-3.4.2/plugins/lute-mandarin/lute_mandarin_parser/parser.py
--rw-r--r--   0        0        0      523 2024-05-30 03:06:17.811596 lute3-3.4.2/plugins/lute-mandarin/pyproject.toml
--rw-r--r--   0        0        0     1538 2024-05-18 03:42:18.967830 lute3-3.4.2/plugins/lute-mandarin/requirements.txt
--rw-r--r--   0        0        0        0 2024-05-27 23:47:17.826244 lute3-3.4.2/plugins/lute-mandarin/tests/__init__.py
--rw-r--r--   0        0        0      823 2024-05-18 03:42:18.968199 lute3-3.4.2/plugins/lute-mandarin/tests/conftest.py
--rw-r--r--   0        0        0     4608 2024-05-27 23:47:17.826704 lute3-3.4.2/plugins/lute-mandarin/tests/test_MandarinParser.py
--rw-r--r--   0        0        0     1226 2024-05-11 22:55:05.266985 lute3-3.4.2/pyproject.toml
--rw-r--r--   0        0        0     1507 2024-05-18 03:42:18.968813 lute3-3.4.2/requirements.txt
--rw-r--r--   0        0        0        0 2024-04-28 00:44:07.964320 lute3-3.4.2/scripts/__init__.py
--rw-r--r--   0        0        0     2564 2024-04-28 00:44:07.964527 lute3-3.4.2/scripts/dump_lang_data.py
--rw-r--r--   0        0        0    10316 2024-05-17 20:10:21.330476 lute3-3.4.2/tasks.py
--rw-r--r--   0        0        0      160 2023-10-22 05:50:12.570821 lute3-3.4.2/tests/__init__.py
--rw-r--r--   0        0        0      442 2023-10-31 05:25:17.232229 lute3-3.4.2/tests/acceptance/README.md
--rw-r--r--   0        0        0      132 2023-11-01 07:45:01.591037 lute3-3.4.2/tests/acceptance/__init__.py
--rw-r--r--   0        0        0     6294 2024-04-28 00:44:07.965096 lute3-3.4.2/tests/acceptance/book.feature
--rw-r--r--   0        0        0    14168 2024-05-18 03:42:18.969323 lute3-3.4.2/tests/acceptance/conftest.py
--rw-r--r--   0        0        0        3 2023-10-31 05:25:17.232861 lute3-3.4.2/tests/acceptance/failure_screenshots/.gitignore
--rw-r--r--   0        0        0       78 2023-10-31 05:25:17.233099 lute3-3.4.2/tests/acceptance/failure_screenshots/README.md
--rw-r--r--   0        0        0    13194 2024-05-18 01:00:02.776994 lute3-3.4.2/tests/acceptance/lute_test_client.py
--rw-r--r--   0        0        0    10086 2024-05-17 21:21:19.865419 lute3-3.4.2/tests/acceptance/reading.feature
--rw-r--r--   0        0        0     1282 2024-02-07 07:50:18.801083 lute3-3.4.2/tests/acceptance/sample_files/Hola.epub
--rw-r--r--   0        0        0     1433 2024-02-07 07:50:18.801387 lute3-3.4.2/tests/acceptance/sample_files/Hola.pdf
--rw-r--r--   0        0        0       48 2024-03-15 03:25:40.913611 lute3-3.4.2/tests/acceptance/sample_files/Hola.srt
--rw-r--r--   0        0        0       56 2024-03-15 03:25:40.913905 lute3-3.4.2/tests/acceptance/sample_files/Hola.vtt
--rw-r--r--   0        0        0       16 2024-01-13 04:05:05.265704 lute3-3.4.2/tests/acceptance/sample_files/hola.txt
--rw-r--r--   0        0        0       16 2024-02-07 07:50:18.801723 lute3-3.4.2/tests/acceptance/sample_files/invalid.epub
--rw-r--r--   0        0        0       16 2024-02-07 07:50:18.801856 lute3-3.4.2/tests/acceptance/sample_files/invalid.pdf
--rw-r--r--   0        0        0       16 2024-03-15 03:25:40.914165 lute3-3.4.2/tests/acceptance/sample_files/invalid.srt
--rw-r--r--   0        0        0       16 2024-03-15 03:25:40.914274 lute3-3.4.2/tests/acceptance/sample_files/invalid.vtt
--rw-r--r--   0        0        0     1417 2024-03-25 09:32:17.283465 lute3-3.4.2/tests/acceptance/sample_files/invalid_empty.epub
--rw-r--r--   0        0        0       74 2024-02-07 07:50:18.802571 lute3-3.4.2/tests/acceptance/sample_files/non_utf_8.txt
--rw-r--r--   0        0        0     2256 2024-03-25 09:32:17.283950 lute3-3.4.2/tests/acceptance/smoke.feature
--rw-r--r--   0        0        0      630 2024-03-08 03:05:01.891609 lute3-3.4.2/tests/acceptance/start_acceptance_app.py
--rw-r--r--   0        0        0     2102 2024-05-18 03:42:18.969654 lute3-3.4.2/tests/acceptance/sync_status.feature
--rw-r--r--   0        0        0     2153 2024-03-15 03:25:40.915397 lute3-3.4.2/tests/acceptance/term.feature
--rw-r--r--   0        0        0       92 2023-11-08 00:06:31.621311 lute3-3.4.2/tests/acceptance/test_book.py
--rw-r--r--   0        0        0       98 2023-11-08 00:06:31.621627 lute3-3.4.2/tests/acceptance/test_reading.py
--rw-r--r--   0        0        0       83 2024-03-25 09:32:17.285207 lute3-3.4.2/tests/acceptance/test_smoke.py
--rw-r--r--   0        0        0      102 2024-05-18 03:42:18.969722 lute3-3.4.2/tests/acceptance/test_sync_status.py
--rw-r--r--   0        0        0       92 2023-11-08 00:06:31.622287 lute3-3.4.2/tests/acceptance/test_term.py
--rw-r--r--   0        0        0      109 2023-11-08 00:06:31.622737 lute3-3.4.2/tests/acceptance/test_unsupported_parser.py
--rw-r--r--   0        0        0     1304 2024-03-25 09:32:17.285870 lute3-3.4.2/tests/acceptance/unsupported_parser.feature
--rw-r--r--   0        0        0     3953 2024-05-18 03:42:18.970148 lute3-3.4.2/tests/conftest.py
--rw-r--r--   0        0        0     1771 2023-11-08 00:06:31.623664 lute3-3.4.2/tests/dbasserts.py
--rw-r--r--   0        0        0      676 2023-10-22 17:27:11.801049 lute3-3.4.2/tests/features/README.md
--rw-r--r--   0        0        0    15205 2024-03-08 03:05:01.894503 lute3-3.4.2/tests/features/rendering.feature
--rw-r--r--   0        0        0    18630 2024-05-11 22:55:05.269192 lute3-3.4.2/tests/features/term_import.feature
--rw-r--r--   0        0        0     2907 2024-03-25 09:32:17.287963 lute3-3.4.2/tests/features/term_import_status_0.feature
--rw-r--r--   0        0        0     3696 2024-03-23 10:37:45.604972 lute3-3.4.2/tests/features/test_rendering.py
--rw-r--r--   0        0        0     3760 2024-03-25 09:32:17.288599 lute3-3.4.2/tests/features/test_term_import.py
--rw-r--r--   0        0        0        0 2023-09-20 06:21:29.988625 lute3-3.4.2/tests/integration/__init__.py
--rw-r--r--   0        0        0     1206 2024-01-13 04:05:05.275517 lute3-3.4.2/tests/integration/test_main.py
--rw-r--r--   0        0        0       97 2023-10-20 06:39:27.112890 lute3-3.4.2/tests/orm/README.md
--rw-r--r--   0        0        0        0 2023-10-20 06:39:27.113017 lute3-3.4.2/tests/orm/__init__.py
--rw-r--r--   0        0        0     2808 2024-02-07 07:50:18.812178 lute3-3.4.2/tests/orm/test_Book.py
--rw-r--r--   0        0        0     3659 2024-02-19 02:42:49.366795 lute3-3.4.2/tests/orm/test_Language.py
--rw-r--r--   0        0        0     8881 2024-04-28 00:44:07.966312 lute3-3.4.2/tests/orm/test_Term.py
--rw-r--r--   0        0        0      871 2023-11-08 00:06:31.626423 lute3-3.4.2/tests/orm/test_Text.py
--rw-r--r--   0        0        0        0 2024-01-13 04:05:05.275609 lute3-3.4.2/tests/playwright/__init__.py
--rw-r--r--   0        0        0     8255 2024-05-04 23:50:35.709807 lute3-3.4.2/tests/playwright/playwright.py
--rw-r--r--   0        0        0        0 2023-09-10 06:10:01.992940 lute3-3.4.2/tests/unit/__init__.py
--rw-r--r--   0        0        0        0 2023-10-30 00:38:51.297976 lute3-3.4.2/tests/unit/backup/__init__.py
--rw-r--r--   0        0        0     9602 2024-02-19 02:42:49.368373 lute3-3.4.2/tests/unit/backup/test_backup.py
--rw-r--r--   0        0        0        0 2023-10-20 18:52:22.684248 lute3-3.4.2/tests/unit/book/__init__.py
--rw-r--r--   0        0        0     3884 2024-04-28 00:44:07.966859 lute3-3.4.2/tests/unit/book/test_Repository.py
--rw-r--r--   0        0        0     2241 2024-03-13 16:30:50.212038 lute3-3.4.2/tests/unit/book/test_datatables.py
--rw-r--r--   0        0        0     4124 2024-02-07 07:50:18.815696 lute3-3.4.2/tests/unit/book/test_stats.py
--rw-r--r--   0        0        0        0 2024-01-13 04:05:05.277883 lute3-3.4.2/tests/unit/cli/__init__.py
--rw-r--r--   0        0        0      867 2024-05-11 22:55:05.269819 lute3-3.4.2/tests/unit/cli/test_language_term_export.py
--rw-r--r--   0        0        0        0 2023-11-04 21:50:44.092388 lute3-3.4.2/tests/unit/config/__init__.py
--rw-r--r--   0        0        0     3035 2024-01-13 04:05:05.278929 lute3-3.4.2/tests/unit/config/test_app_config.py
--rw-r--r--   0        0        0        0 2023-10-26 01:04:31.832624 lute3-3.4.2/tests/unit/db/__init__.py
--rw-r--r--   0        0        0        0 2023-10-20 18:48:10.174878 lute3-3.4.2/tests/unit/db/setup/__init__.py
--rw-r--r--   0        0        0       28 2023-10-20 18:48:10.175186 lute3-3.4.2/tests/unit/db/setup/schema/README.md
--rw-r--r--   0        0        0      134 2023-10-20 18:48:10.175437 lute3-3.4.2/tests/unit/db/setup/schema/baseline/schema.sql
--rw-r--r--   0        0        0       24 2023-10-20 18:48:10.175796 lute3-3.4.2/tests/unit/db/setup/schema/migrations/123_create_B.sql
--rw-r--r--   0        0        0       68 2023-10-20 18:48:10.176170 lute3-3.4.2/tests/unit/db/setup/schema/repeatable/view_A.sql
--rw-r--r--   0        0        0     1241 2023-11-08 00:06:31.628181 lute3-3.4.2/tests/unit/db/setup/test_BackupManager.py
--rw-r--r--   0        0        0     8127 2023-11-08 00:06:31.628506 lute3-3.4.2/tests/unit/db/setup/test_Setup.py
--rw-r--r--   0        0        0     3681 2023-11-08 00:06:31.628800 lute3-3.4.2/tests/unit/db/setup/test_SqliteMigrator.py
--rw-r--r--   0        0        0     3107 2024-05-18 03:42:18.971519 lute3-3.4.2/tests/unit/db/test_demo.py
--rw-r--r--   0        0        0     1534 2023-11-11 22:05:26.100552 lute3-3.4.2/tests/unit/db/test_management.py
--rw-r--r--   0        0        0        0 2024-04-28 00:44:07.967194 lute3-3.4.2/tests/unit/language/__init__.py
--rw-r--r--   0        0        0     2396 2024-05-18 03:42:18.971891 lute3-3.4.2/tests/unit/language/test_service.py
--rw-r--r--   0        0        0        0 2023-10-04 05:48:35.085848 lute3-3.4.2/tests/unit/models/__init__.py
--rw-r--r--   0        0        0     1820 2024-03-13 16:30:50.212544 lute3-3.4.2/tests/unit/models/test_Book.py
--rw-r--r--   0        0        0     3102 2024-03-15 03:25:40.916767 lute3-3.4.2/tests/unit/models/test_Book_add_remove_pages.py
--rw-r--r--   0        0        0     2420 2024-04-28 00:44:07.967649 lute3-3.4.2/tests/unit/models/test_Language.py
--rw-r--r--   0        0        0     6167 2024-02-19 02:42:49.368998 lute3-3.4.2/tests/unit/models/test_Setting.py
--rw-r--r--   0        0        0     8034 2024-03-25 09:32:17.290517 lute3-3.4.2/tests/unit/models/test_Term.py
--rw-r--r--   0        0        0     1398 2023-11-08 00:06:31.630600 lute3-3.4.2/tests/unit/models/test_TermTag.py
--rw-r--r--   0        0        0      970 2024-02-07 07:50:18.820113 lute3-3.4.2/tests/unit/models/test_Text.py
--rw-r--r--   0        0        0        0 2023-10-07 05:09:39.900041 lute3-3.4.2/tests/unit/parse/__init__.py
--rw-r--r--   0        0        0     1806 2023-11-08 00:06:31.631135 lute3-3.4.2/tests/unit/parse/test_ClassicalChineseParser.py
--rw-r--r--   0        0        0     2655 2024-03-08 03:05:01.896542 lute3-3.4.2/tests/unit/parse/test_JapaneseParser.py
--rw-r--r--   0        0        0     1452 2023-11-08 00:06:31.631582 lute3-3.4.2/tests/unit/parse/test_SentenceGroupIterator.py
--rw-r--r--   0        0        0     9044 2024-05-06 03:26:32.117861 lute3-3.4.2/tests/unit/parse/test_SpaceDelimitedParser.py
--rw-r--r--   0        0        0      437 2023-11-08 00:06:31.632019 lute3-3.4.2/tests/unit/parse/test_TurkishParser.py
--rw-r--r--   0        0        0     2070 2024-05-27 23:47:17.826999 lute3-3.4.2/tests/unit/parse/test_registry.py
--rw-r--r--   0        0        0        0 2023-10-18 06:43:42.369680 lute3-3.4.2/tests/unit/read/__init__.py
--rw-r--r--   0        0        0        0 2023-10-18 06:43:42.370116 lute3-3.4.2/tests/unit/read/render/__init__.py
--rw-r--r--   0        0        0     4830 2024-05-06 03:26:32.118133 lute3-3.4.2/tests/unit/read/render/test_RenderableCalculator.py
--rw-r--r--   0        0        0     1965 2023-11-08 00:06:31.632694 lute3-3.4.2/tests/unit/read/render/test_TokenLocator.py
--rw-r--r--   0        0        0     5317 2024-05-28 16:43:48.082243 lute3-3.4.2/tests/unit/read/render/test_service.py
--rw-r--r--   0        0        0     1580 2024-05-28 16:43:48.082605 lute3-3.4.2/tests/unit/read/test_service.py
--rw-r--r--   0        0        0     4892 2024-05-06 03:26:32.118479 lute3-3.4.2/tests/unit/read/test_service_popup_data.py
--rw-r--r--   0        0        0        0 2024-01-13 04:05:05.283732 lute3-3.4.2/tests/unit/stats/__init__.py
--rw-r--r--   0        0        0     2467 2024-02-07 07:50:18.821867 lute3-3.4.2/tests/unit/stats/test_service.py
--rw-r--r--   0        0        0        0 2023-10-21 00:58:40.675868 lute3-3.4.2/tests/unit/term/__init__.py
--rw-r--r--   0        0        0    23300 2024-04-28 00:44:07.968765 lute3-3.4.2/tests/unit/term/test_Repository.py
--rw-r--r--   0        0        0     2082 2024-02-07 07:50:18.824210 lute3-3.4.2/tests/unit/term/test_TermForm.py
--rw-r--r--   0        0        0     6766 2024-02-07 07:50:18.824963 lute3-3.4.2/tests/unit/term/test_Term_status_follow.py
--rw-r--r--   0        0        0     1629 2024-01-13 04:05:05.285150 lute3-3.4.2/tests/unit/term/test_datatables.py
--rw-r--r--   0        0        0        0 2023-10-30 23:02:04.731925 lute3-3.4.2/tests/unit/term_parent_map/__init__.py
--rw-r--r--   0        0        0     1255 2024-03-15 03:25:40.918632 lute3-3.4.2/tests/unit/term_parent_map/test_service.py
--rw-r--r--   0        0        0        0 2024-01-13 04:05:05.285261 lute3-3.4.2/tests/unit/termtag/__init__.py
--rw-r--r--   0        0        0      679 2023-11-08 00:06:31.633834 lute3-3.4.2/tests/unit/termtag/test_datatables.py
--rw-r--r--   0        0        0        0 2024-01-13 04:05:05.285353 lute3-3.4.2/tests/unit/themes/__init__.py
--rw-r--r--   0        0        0     3416 2024-05-06 03:26:32.118714 lute3-3.4.2/tests/unit/themes/test_service.py
--rw-r--r--   0        0        0        0 2023-10-09 03:35:20.091806 lute3-3.4.2/tests/unit/utils/__init__.py
--rw-r--r--   0        0        0     5151 2024-01-18 07:46:16.382578 lute3-3.4.2/tests/unit/utils/test_DataTablesSqliteQuery.py
--rw-r--r--   0        0        0      786 2024-03-13 16:30:50.213297 lute3-3.4.2/tests/unit/utils/test_formutils.py
--rw-r--r--   0        0        0     1629 2024-02-07 07:50:18.825866 lute3-3.4.2/tests/utils.py
--rwxr-xr-x   0        0        0     1575 2024-02-19 02:42:49.369401 lute3-3.4.2/utils/dump_changelog.sh
--rwxr-xr-x   0        0        0      565 2024-03-15 03:25:40.919140 lute3-3.4.2/utils/findstring.sh
--rw-r--r--   0        0        0     4820 2023-11-22 00:36:49.803896 lute3-3.4.2/utils/todos.py
--rw-r--r--   0        0        0      698 2023-11-09 08:26:12.057924 lute3-3.4.2/utils/verify.py
--rw-r--r--   0        0        0     2328 1970-01-01 00:00:00.000000 lute3-3.4.2/PKG-INFO
+-rw-r--r--   0        0        0      170 2023-11-09 08:26:12.050479 lute3-3.4.2b1/.dockerignore
+-rw-r--r--   0        0        0     1280 2024-03-08 03:05:01.842902 lute3-3.4.2b1/.github/ISSUE_TEMPLATE/add_language.md
+-rw-r--r--   0        0        0      590 2024-03-08 03:05:01.843291 lute3-3.4.2b1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      649 2024-04-28 00:44:07.948708 lute3-3.4.2b1/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0        0        0      578 2024-03-08 03:05:01.843637 lute3-3.4.2b1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0    10714 2024-05-19 18:38:13.894853 lute3-3.4.2b1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2663 2024-04-28 00:44:07.949318 lute3-3.4.2b1/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     2172 2024-04-05 03:40:57.739326 lute3-3.4.2b1/.gitignore
+-rw-r--r--   0        0        0      119 2024-04-28 00:44:07.949499 lute3-3.4.2b1/.gitmodules
+-rw-r--r--   0        0        0      395 2024-01-13 04:05:05.193611 lute3-3.4.2b1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    24735 2023-11-20 01:37:46.796733 lute3-3.4.2b1/.pylintrc
+-rw-r--r--   0        0        0     1076 2024-01-13 04:05:05.194389 lute3-3.4.2b1/.pytest.ini
+-rw-r--r--   0        0        0     1068 2023-11-09 05:33:09.100157 lute3-3.4.2b1/LICENSE.txt
+-rw-r--r--   0        0        0     1641 2024-04-28 00:44:07.949766 lute3-3.4.2b1/README.md
+-rw-r--r--   0        0        0     1145 2024-04-28 00:44:07.950030 lute3-3.4.2b1/README_PyPi.md
+-rw-r--r--   0        0        0     1664 2024-05-18 03:42:18.960922 lute3-3.4.2b1/devstart.py
+-rw-r--r--   0        0        0      965 2023-11-10 18:48:16.706091 lute3-3.4.2b1/docker/Dockerfile
+-rw-r--r--   0        0        0      496 2024-01-13 04:05:05.195405 lute3-3.4.2b1/docker/README.md
+-rwxr-xr-x   0        0        0     1545 2024-01-13 04:05:05.195617 lute3-3.4.2b1/docker/build_all.sh
+-rwxr-xr-x   0        0        0       89 2024-01-13 04:05:05.195716 lute3-3.4.2b1/docker/build_test.sh
+-rw-r--r--   0        0        0     1076 2023-11-09 08:26:12.052441 lute3-3.4.2b1/docker/check_mounts_and_start.sh
+-rw-r--r--   0        0        0      309 2023-11-09 08:26:12.052717 lute3-3.4.2b1/docker/docker-compose.yml.example
+-rw-r--r--   0        0        0     3249 2024-04-28 00:44:07.950509 lute3-3.4.2b1/docker/docker_hub_overview.md
+-rwxr-xr-x   0        0        0     1127 2024-01-13 04:05:05.195822 lute3-3.4.2b1/docker/try_build_multi.sh
+-rw-r--r--   0        0        0    15768 2024-05-19 18:38:13.895271 lute3-3.4.2b1/docs/CHANGELOG.md
+-rw-r--r--   0        0        0       71 2024-01-13 04:05:05.196786 lute3-3.4.2b1/docs/README.md
+-rw-r--r--   0        0        0     1068 2023-11-09 05:33:09.101369 lute3-3.4.2b1/lute/LICENSE.txt
+-rw-r--r--   0        0        0      382 2024-05-27 23:47:54.258613 lute3-3.4.2b1/lute/__init__.py
+-rw-r--r--   0        0        0    12532 2024-05-27 23:47:17.824003 lute3-3.4.2b1/lute/app_factory.py
+-rw-r--r--   0        0        0        0 2023-10-30 00:38:51.292984 lute3-3.4.2b1/lute/backup/__init__.py
+-rw-r--r--   0        0        0     2300 2024-03-15 03:25:40.865078 lute3-3.4.2b1/lute/backup/routes.py
+-rw-r--r--   0        0        0     5303 2024-03-15 03:25:40.865445 lute3-3.4.2b1/lute/backup/service.py
+-rw-r--r--   0        0        0        0 2023-10-24 05:43:55.066190 lute3-3.4.2b1/lute/bing/__init__.py
+-rw-r--r--   0        0        0     3736 2024-03-13 16:30:50.197607 lute3-3.4.2b1/lute/bing/routes.py
+-rw-r--r--   0        0        0        0 2023-10-16 06:20:14.169949 lute3-3.4.2b1/lute/book/__init__.py
+-rw-r--r--   0        0        0     2541 2024-03-15 03:25:40.865805 lute3-3.4.2b1/lute/book/datatables.py
+-rw-r--r--   0        0        0     5146 2024-05-18 03:42:18.962171 lute3-3.4.2b1/lute/book/forms.py
+-rw-r--r--   0        0        0     3633 2024-04-28 00:44:07.951451 lute3-3.4.2b1/lute/book/model.py
+-rw-r--r--   0        0        0     5021 2024-03-25 09:32:17.257357 lute3-3.4.2b1/lute/book/routes.py
+-rw-r--r--   0        0        0     6395 2024-03-25 09:32:17.258143 lute3-3.4.2b1/lute/book/service.py
+-rw-r--r--   0        0        0     3598 2024-02-07 07:50:18.749346 lute3-3.4.2b1/lute/book/stats.py
+-rw-r--r--   0        0        0      475 2024-01-13 04:05:05.200591 lute3-3.4.2b1/lute/cli/README.md
+-rw-r--r--   0        0        0        0 2024-01-13 04:05:05.200653 lute3-3.4.2b1/lute/cli/__init__.py
+-rw-r--r--   0        0        0      807 2024-01-13 04:05:05.200788 lute3-3.4.2b1/lute/cli/commands.py
+-rw-r--r--   0        0        0     6340 2024-05-11 22:55:05.262438 lute3-3.4.2b1/lute/cli/language_term_export.py
+-rw-r--r--   0        0        0        0 2023-11-04 21:50:44.080272 lute3-3.4.2b1/lute/config/__init__.py
+-rw-r--r--   0        0        0     3093 2024-05-27 23:47:17.824218 lute3-3.4.2b1/lute/config/app_config.py
+-rw-r--r--   0        0        0      265 2024-01-13 04:05:05.201516 lute3-3.4.2b1/lute/config/config.yml.docker
+-rw-r--r--   0        0        0      667 2024-01-13 04:05:05.201703 lute3-3.4.2b1/lute/config/config.yml.example
+-rw-r--r--   0        0        0      280 2024-01-13 04:05:05.201898 lute3-3.4.2b1/lute/config/config.yml.prod
+-rw-r--r--   0        0        0      108 2023-10-20 18:48:10.167405 lute3-3.4.2b1/lute/db/__init__.py
+-rw-r--r--   0        0        0     1021 2024-02-07 07:50:18.750797 lute3-3.4.2b1/lute/db/data_cleanup.py
+-rw-r--r--   0        0        0     3032 2024-04-28 00:44:07.951712 lute3-3.4.2b1/lute/db/demo.py
+-rw-r--r--   0        0        0      525 2024-04-28 00:58:20.367519 lute3-3.4.2b1/lute/db/language_defs/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1799 2024-04-28 00:58:20.367921 lute3-3.4.2b1/lute/db/language_defs/README.md
+-rw-r--r--   0        0        0      379 2024-04-28 00:58:20.368228 lute3-3.4.2b1/lute/db/language_defs/_templates/definition.yaml.example
+-rw-r--r--   0        0        0       35 2024-04-28 00:58:20.368382 lute3-3.4.2b1/lute/db/language_defs/_templates/story.txt.example
+-rw-r--r--   0        0        0      820 2024-04-28 00:58:20.369000 lute3-3.4.2b1/lute/db/language_defs/afrikaans/definition.yaml
+-rw-r--r--   0        0        0      582 2024-04-28 00:58:20.369554 lute3-3.4.2b1/lute/db/language_defs/afrikaans/die_diere_grawe_n_put.txt
+-rw-r--r--   0        0        0      816 2024-04-28 00:58:20.370260 lute3-3.4.2b1/lute/db/language_defs/albanian/definition.yaml
+-rw-r--r--   0        0        0      791 2024-04-28 00:58:20.370623 lute3-3.4.2b1/lute/db/language_defs/albanian/shqiponja_dhe_mbreti.txt
+-rw-r--r--   0        0        0      943 2024-04-28 00:58:20.371105 lute3-3.4.2b1/lute/db/language_defs/amharic/definition.yaml
+-rw-r--r--   0        0        0      898 2024-04-28 00:58:20.371501 lute3-3.4.2b1/lute/db/language_defs/amharic/story_1.txt
+-rw-r--r--   0        0        0     1147 2024-04-28 00:58:20.371719 lute3-3.4.2b1/lute/db/language_defs/arabic/ar_demo.txt
+-rw-r--r--   0        0        0      555 2024-04-28 00:58:20.371868 lute3-3.4.2b1/lute/db/language_defs/arabic/definition.yaml
+-rw-r--r--   0        0        0     1453 2024-04-28 00:58:20.372285 lute3-3.4.2b1/lute/db/language_defs/armenian/definition.yaml
+-rw-r--r--   0        0        0     3063 2024-04-28 00:58:20.372760 lute3-3.4.2b1/lute/db/language_defs/armenian/story_1.txt
+-rw-r--r--   0        0        0     1473 2024-04-28 00:58:20.373153 lute3-3.4.2b1/lute/db/language_defs/azerbaijani/definition.yaml
+-rw-r--r--   0        0        0     2742 2024-04-28 00:58:20.373423 lute3-3.4.2b1/lute/db/language_defs/azerbaijani/story_1.txt
+-rw-r--r--   0        0        0      885 2024-04-28 00:58:20.373817 lute3-3.4.2b1/lute/db/language_defs/basque/definition.yaml
+-rw-r--r--   0        0        0      663 2024-04-28 00:58:20.374076 lute3-3.4.2b1/lute/db/language_defs/basque/story_1.txt
+-rw-r--r--   0        0        0     1024 2024-04-28 00:58:20.374525 lute3-3.4.2b1/lute/db/language_defs/belarusian/definition.yaml
+-rw-r--r--   0        0        0     2573 2024-04-28 00:58:20.374843 lute3-3.4.2b1/lute/db/language_defs/belarusian/story_1.txt
+-rw-r--r--   0        0        0     2176 2024-04-28 00:58:20.375301 lute3-3.4.2b1/lute/db/language_defs/bengali/aharshi_the_bengal_tiger.txt
+-rw-r--r--   0        0        0      988 2024-04-28 00:58:20.375609 lute3-3.4.2b1/lute/db/language_defs/bengali/definition.yaml
+-rw-r--r--   0        0        0     1220 2024-04-28 00:58:20.375973 lute3-3.4.2b1/lute/db/language_defs/breton/definition.yaml
+-rw-r--r--   0        0        0     1991 2024-04-28 00:58:20.376271 lute3-3.4.2b1/lute/db/language_defs/breton/story_1.txt
+-rw-r--r--   0        0        0     1499 2024-04-28 00:58:20.376643 lute3-3.4.2b1/lute/db/language_defs/bulgarian/definition.yaml
+-rw-r--r--   0        0        0      731 2024-04-28 00:58:20.376952 lute3-3.4.2b1/lute/db/language_defs/bulgarian/yesterday_film_description.txt
+-rw-r--r--   0        0        0     1991 2024-04-28 00:58:20.377555 lute3-3.4.2b1/lute/db/language_defs/catalan/definition.yaml
+-rw-r--r--   0        0        0      718 2024-04-28 00:58:20.377855 lute3-3.4.2b1/lute/db/language_defs/catalan/merlí_series_description.txt
+-rw-r--r--   0        0        0     1412 2024-04-28 00:58:20.378088 lute3-3.4.2b1/lute/db/language_defs/classical_chinese/cc_demo.txt
+-rw-r--r--   0        0        0      416 2024-04-28 00:58:20.378221 lute3-3.4.2b1/lute/db/language_defs/classical_chinese/definition.yaml
+-rw-r--r--   0        0        0      948 2024-04-28 00:58:20.378797 lute3-3.4.2b1/lute/db/language_defs/croatian/definition.yaml
+-rw-r--r--   0        0        0      530 2024-04-28 00:58:20.379041 lute3-3.4.2b1/lute/db/language_defs/croatian/story_1.txt
+-rw-r--r--   0        0        0      518 2024-04-28 00:58:20.379330 lute3-3.4.2b1/lute/db/language_defs/czech/czech.txt
+-rw-r--r--   0        0        0      377 2024-04-28 00:58:20.379456 lute3-3.4.2b1/lute/db/language_defs/czech/definition.yaml
+-rw-r--r--   0        0        0     1093 2024-04-28 00:58:20.379770 lute3-3.4.2b1/lute/db/language_defs/danish/definition.yaml
+-rw-r--r--   0        0        0      670 2024-04-28 00:58:20.380012 lute3-3.4.2b1/lute/db/language_defs/danish/prinsessen_pa_arten.txt
+-rw-r--r--   0        0        0      474 2024-04-28 00:58:20.380500 lute3-3.4.2b1/lute/db/language_defs/dutch/de_doortocht.txt
+-rw-r--r--   0        0        0     1127 2024-04-28 00:58:20.381065 lute3-3.4.2b1/lute/db/language_defs/dutch/definition.yaml
+-rw-r--r--   0        0        0      468 2024-04-28 00:58:20.381348 lute3-3.4.2b1/lute/db/language_defs/english/definition.yaml
+-rw-r--r--   0        0        0     7159 2024-04-28 00:58:20.381753 lute3-3.4.2b1/lute/db/language_defs/english/tutorial.txt
+-rw-r--r--   0        0        0     3534 2024-04-28 00:58:20.381883 lute3-3.4.2b1/lute/db/language_defs/english/tutorial_follow_up.txt
+-rw-r--r--   0        0        0      858 2024-04-28 00:58:20.382235 lute3-3.4.2b1/lute/db/language_defs/esperanto/definition.yaml
+-rw-r--r--   0        0        0      535 2024-04-28 00:58:20.382495 lute3-3.4.2b1/lute/db/language_defs/esperanto/story_1.txt
+-rw-r--r--   0        0        0     2043 2024-04-28 00:58:20.382830 lute3-3.4.2b1/lute/db/language_defs/estonian/definition.yaml
+-rw-r--r--   0        0        0      746 2024-04-28 00:58:20.383067 lute3-3.4.2b1/lute/db/language_defs/estonian/story_1.txt
+-rw-r--r--   0        0        0     1000 2024-04-28 00:58:20.383513 lute3-3.4.2b1/lute/db/language_defs/farsi/definition.yaml
+-rw-r--r--   0        0        0      951 2024-04-28 00:58:20.383824 lute3-3.4.2b1/lute/db/language_defs/farsi/story_1.txt
+-rw-r--r--   0        0        0     2450 2024-04-28 00:58:20.384190 lute3-3.4.2b1/lute/db/language_defs/finnish/definition.yaml
+-rw-r--r--   0        0        0      537 2024-04-28 00:58:20.384443 lute3-3.4.2b1/lute/db/language_defs/finnish/story_1.txt
+-rw-r--r--   0        0        0      370 2024-04-28 00:58:20.384728 lute3-3.4.2b1/lute/db/language_defs/french/definition.yaml
+-rw-r--r--   0        0        0      469 2024-04-28 00:58:20.385090 lute3-3.4.2b1/lute/db/language_defs/french/fr_goldilocks.txt
+-rw-r--r--   0        0        0     1672 2024-04-28 00:58:20.385735 lute3-3.4.2b1/lute/db/language_defs/galician/definition.yaml
+-rw-r--r--   0        0        0      544 2024-04-28 00:58:20.386025 lute3-3.4.2b1/lute/db/language_defs/galician/story_1.txt
+-rw-r--r--   0        0        0      513 2024-04-29 04:26:18.411489 lute3-3.4.2b1/lute/db/language_defs/generic/definition.yaml
+-rw-r--r--   0        0        0     3882 2024-04-29 04:26:18.411940 lute3-3.4.2b1/lute/db/language_defs/generic/story_1.txt
+-rw-r--r--   0        0        0     1306 2024-04-28 00:58:20.386531 lute3-3.4.2b1/lute/db/language_defs/georgian/definition.yaml
+-rw-r--r--   0        0        0      953 2024-04-28 00:58:20.386759 lute3-3.4.2b1/lute/db/language_defs/georgian/story_1.txt
+-rw-r--r--   0        0        0     1058 2024-04-28 00:58:20.386961 lute3-3.4.2b1/lute/db/language_defs/german/de_Stadtmusikanten.txt
+-rw-r--r--   0        0        0      522 2024-04-28 00:58:20.387058 lute3-3.4.2b1/lute/db/language_defs/german/definition.yaml
+-rw-r--r--   0        0        0      858 2024-04-28 00:58:20.387591 lute3-3.4.2b1/lute/db/language_defs/gothic/definition.yaml
+-rw-r--r--   0        0        0     1317 2024-04-28 00:58:20.387839 lute3-3.4.2b1/lute/db/language_defs/gothic/story_1.txt
+-rw-r--r--   0        0        0      635 2024-04-28 00:58:20.388044 lute3-3.4.2b1/lute/db/language_defs/greek/definition.yaml
+-rw-r--r--   0        0        0     1649 2024-04-28 00:58:20.388167 lute3-3.4.2b1/lute/db/language_defs/greek/gr_demo.txt
+-rw-r--r--   0        0        0     2165 2024-04-28 00:58:20.388512 lute3-3.4.2b1/lute/db/language_defs/hebrew/definition.yaml
+-rw-r--r--   0        0        0      945 2024-04-28 00:58:20.388804 lute3-3.4.2b1/lute/db/language_defs/hebrew/story_1.txt
+-rw-r--r--   0        0        0      566 2024-04-28 00:58:20.389048 lute3-3.4.2b1/lute/db/language_defs/hindi/definition.yaml
+-rw-r--r--   0        0        0      587 2024-04-28 00:58:20.389500 lute3-3.4.2b1/lute/db/language_defs/hindi/hi_wikipedia.txt
+-rw-r--r--   0        0        0     2484 2024-04-28 00:58:20.389944 lute3-3.4.2b1/lute/db/language_defs/hungarian/definition.yaml
+-rw-r--r--   0        0        0      308 2024-04-28 00:58:20.390708 lute3-3.4.2b1/lute/db/language_defs/hungarian/satantango_film_description.txt
+-rw-r--r--   0        0        0     1505 2024-04-28 00:58:20.391114 lute3-3.4.2b1/lute/db/language_defs/icelandic/definition.yaml
+-rw-r--r--   0        0        0     1262 2024-04-28 00:58:20.391519 lute3-3.4.2b1/lute/db/language_defs/icelandic/story_1.txt
+-rw-r--r--   0        0        0      868 2024-04-28 00:58:20.392430 lute3-3.4.2b1/lute/db/language_defs/indonesian/definition.yaml
+-rw-r--r--   0        0        0      643 2024-04-28 00:58:20.393006 lute3-3.4.2b1/lute/db/language_defs/indonesian/kura-kura_yang_sombong.txt
+-rw-r--r--   0        0        0     3101 2024-04-28 00:58:20.394776 lute3-3.4.2b1/lute/db/language_defs/italian/definition.yaml
+-rw-r--r--   0        0        0      905 2024-04-28 00:58:20.395281 lute3-3.4.2b1/lute/db/language_defs/italian/le_avventure_di_pinocchio.txt
+-rw-r--r--   0        0        0      539 2024-04-28 00:58:20.395499 lute3-3.4.2b1/lute/db/language_defs/japanese/definition.yaml
+-rw-r--r--   0        0        0      428 2024-04-28 00:58:20.398623 lute3-3.4.2b1/lute/db/language_defs/japanese/jp_kitakaze_to_taiyou.txt
+-rw-r--r--   0        0        0     2188 2024-04-28 00:58:20.399079 lute3-3.4.2b1/lute/db/language_defs/latin/definition.yaml
+-rw-r--r--   0        0        0      497 2024-04-28 00:58:20.399384 lute3-3.4.2b1/lute/db/language_defs/latin/story_1.txt
+-rw-r--r--   0        0        0     1796 2024-04-28 00:58:20.400015 lute3-3.4.2b1/lute/db/language_defs/latvian/definition.yaml
+-rw-r--r--   0        0        0      562 2024-04-28 00:58:20.415069 lute3-3.4.2b1/lute/db/language_defs/latvian/story_1.txt
+-rw-r--r--   0        0        0     1850 2024-04-28 00:58:20.424530 lute3-3.4.2b1/lute/db/language_defs/lithuanian/definition.yaml
+-rw-r--r--   0        0        0     1104 2024-04-28 00:58:20.425240 lute3-3.4.2b1/lute/db/language_defs/lithuanian/story_1.txt
+-rw-r--r--   0        0        0      416 2024-05-17 21:40:35.334109 lute3-3.4.2b1/lute/db/language_defs/mandarin_chinese/definition.yaml
+-rw-r--r--   0        0        0     1064 2024-05-17 21:40:35.334787 lute3-3.4.2b1/lute/db/language_defs/mandarin_chinese/story_1.txt
+-rw-r--r--   0        0        0      800 2024-04-28 00:58:20.427807 lute3-3.4.2b1/lute/db/language_defs/norwegian/definition.yaml
+-rw-r--r--   0        0        0      955 2024-04-28 00:58:20.428215 lute3-3.4.2b1/lute/db/language_defs/norwegian/vildanden.txt
+-rw-r--r--   0        0        0     1141 2024-04-28 00:58:20.428571 lute3-3.4.2b1/lute/db/language_defs/polish/adam_i_smoczy_skarb.txt
+-rw-r--r--   0        0        0     2903 2024-04-28 00:58:20.428846 lute3-3.4.2b1/lute/db/language_defs/polish/definition.yaml
+-rw-r--r--   0        0        0     1047 2024-04-28 00:58:20.429230 lute3-3.4.2b1/lute/db/language_defs/portuguese/a_maldicao.txt
+-rw-r--r--   0        0        0     3471 2024-04-28 00:58:20.429552 lute3-3.4.2b1/lute/db/language_defs/portuguese/definition.yaml
+-rw-r--r--   0        0        0     1143 2024-04-28 00:58:20.430104 lute3-3.4.2b1/lute/db/language_defs/punjabi/definition.yaml
+-rw-r--r--   0        0        0     1390 2024-04-28 00:58:20.431321 lute3-3.4.2b1/lute/db/language_defs/punjabi/story_1.txt
+-rw-r--r--   0        0        0       14 2024-04-28 00:58:20.431532 lute3-3.4.2b1/lute/db/language_defs/requirements.txt
+-rw-r--r--   0        0        0     2898 2024-04-28 00:58:20.433435 lute3-3.4.2b1/lute/db/language_defs/romanian/definition.yaml
+-rw-r--r--   0        0        0      472 2024-04-28 00:58:20.475856 lute3-3.4.2b1/lute/db/language_defs/romanian/story_1.txt
+-rw-r--r--   0        0        0      470 2024-04-28 00:58:20.476336 lute3-3.4.2b1/lute/db/language_defs/russian/definition.yaml
+-rw-r--r--   0        0        0      546 2024-04-28 00:58:20.476620 lute3-3.4.2b1/lute/db/language_defs/russian/ru_medved.txt
+-rw-r--r--   0        0        0      477 2024-04-28 00:58:20.476859 lute3-3.4.2b1/lute/db/language_defs/sanskrit/definition.yaml
+-rw-r--r--   0        0        0     1027 2024-04-28 00:58:20.477000 lute3-3.4.2b1/lute/db/language_defs/sanskrit/sanskrit.txt
+-rw-r--r--   0        0        0     1028 2024-04-28 00:58:20.477572 lute3-3.4.2b1/lute/db/language_defs/serbian/definition.yaml
+-rw-r--r--   0        0        0      740 2024-04-28 00:58:20.478677 lute3-3.4.2b1/lute/db/language_defs/serbian/story_1.txt
+-rw-r--r--   0        0        0     2055 2024-04-28 00:58:20.479331 lute3-3.4.2b1/lute/db/language_defs/slovak/definition.yaml
+-rw-r--r--   0        0        0      729 2024-04-28 00:58:20.479609 lute3-3.4.2b1/lute/db/language_defs/slovak/story_1.txt
+-rw-r--r--   0        0        0     1644 2024-04-28 00:58:20.479985 lute3-3.4.2b1/lute/db/language_defs/slovene/definition.yaml
+-rw-r--r--   0        0        0      464 2024-04-28 00:58:20.480514 lute3-3.4.2b1/lute/db/language_defs/slovene/story_1.txt
+-rw-r--r--   0        0        0      526 2024-04-28 00:58:20.480755 lute3-3.4.2b1/lute/db/language_defs/spanish/definition.yaml
+-rw-r--r--   0        0        0      534 2024-04-28 00:58:20.480873 lute3-3.4.2b1/lute/db/language_defs/spanish/es_aladino.txt
+-rw-r--r--   0        0        0     1302 2024-04-28 00:58:20.481695 lute3-3.4.2b1/lute/db/language_defs/swahili/definition.yaml
+-rw-r--r--   0        0        0      755 2024-04-28 00:58:20.482368 lute3-3.4.2b1/lute/db/language_defs/swahili/story_1.txt
+-rw-r--r--   0        0        0     2821 2024-04-28 00:58:20.482938 lute3-3.4.2b1/lute/db/language_defs/swedish/definition.yaml
+-rw-r--r--   0        0        0      566 2024-04-28 00:58:20.483259 lute3-3.4.2b1/lute/db/language_defs/swedish/story_1.txt
+-rw-r--r--   0        0        0     1858 2024-04-28 00:58:20.483690 lute3-3.4.2b1/lute/db/language_defs/tibetan/definition.yaml
+-rw-r--r--   0        0        0     1464 2024-04-28 00:58:20.484308 lute3-3.4.2b1/lute/db/language_defs/tibetan/story_1.txt
+-rw-r--r--   0        0        0      497 2024-04-28 00:58:20.484692 lute3-3.4.2b1/lute/db/language_defs/turkish/definition.yaml
+-rw-r--r--   0        0        0      941 2024-04-28 00:58:20.484816 lute3-3.4.2b1/lute/db/language_defs/turkish/tr_demo.txt
+-rw-r--r--   0        0        0     2211 2024-04-28 00:58:20.485815 lute3-3.4.2b1/lute/db/language_defs/ukrainian/definition.yaml
+-rw-r--r--   0        0        0     1034 2024-04-28 00:58:20.486326 lute3-3.4.2b1/lute/db/language_defs/ukrainian/story_1.txt
+-rw-r--r--   0        0        0     1773 2024-04-28 00:58:20.486478 lute3-3.4.2b1/lute/db/language_defs/verify_files.py
+-rw-r--r--   0        0        0      798 2024-04-28 00:58:20.487001 lute3-3.4.2b1/lute/db/language_defs/vietnamese/definition.yaml
+-rw-r--r--   0        0        0      658 2024-04-28 00:58:20.487378 lute3-3.4.2b1/lute/db/language_defs/vietnamese/lan_bien.txt
+-rw-r--r--   0        0        0      615 2023-11-09 09:07:06.767671 lute3-3.4.2b1/lute/db/management.py
+-rw-r--r--   0        0        0     1620 2023-10-26 01:04:31.825247 lute3-3.4.2b1/lute/db/schema/README.md
+-rw-r--r--   0        0        0    42817 2024-05-27 23:45:25.165770 lute3-3.4.2b1/lute/db/schema/baseline.sql
+-rw-r--r--   0        0        0     8817 2024-03-08 03:05:01.856057 lute3-3.4.2b1/lute/db/schema/empty.sql
+-rw-r--r--   0        0        0      246 2023-10-20 18:48:10.168442 lute3-3.4.2b1/lute/db/schema/migrations/20230409_224327_load_statuses.sql
+-rw-r--r--   0        0        0      178 2023-10-20 18:48:10.168634 lute3-3.4.2b1/lute/db/schema/migrations/20230414_225828_add_texttokens_TokTextLC.sql
+-rw-r--r--   0        0        0      245 2023-10-20 18:48:10.168826 lute3-3.4.2b1/lute/db/schema/migrations/20230428_224656_create_wordflashmessages_table.sql
+-rw-r--r--   0        0        0     2067 2023-10-20 18:48:10.169209 lute3-3.4.2b1/lute/db/schema/migrations/20230518_190000_remove_old_words_fields.sql
+-rw-r--r--   0        0        0      680 2023-10-20 18:48:10.169512 lute3-3.4.2b1/lute/db/schema/migrations/20230519_194627_add_TxDateRead.sql
+-rw-r--r--   0        0        0       96 2023-10-20 18:48:10.169708 lute3-3.4.2b1/lute/db/schema/migrations/20230621_010000_drop_texttags_table.sql
+-rw-r--r--   0        0        0     1143 2023-10-20 18:48:10.169918 lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_01_booktags.sql
+-rw-r--r--   0        0        0     1141 2023-10-20 18:48:10.170132 lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_02_wordtags.sql
+-rw-r--r--   0        0        0     1226 2023-10-20 18:48:10.170317 lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_03_sentences.sql
+-rw-r--r--   0        0        0     1214 2023-10-20 18:48:10.170503 lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_04_texttokens.sql
+-rw-r--r--   0        0        0     1559 2023-10-20 18:48:10.170690 lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_05_texts.sql
+-rw-r--r--   0        0        0     1147 2023-10-20 18:48:10.170868 lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_06_bookstats.sql
+-rw-r--r--   0        0        0     1038 2023-10-20 18:48:10.171044 lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_07_termimages.sql
+-rw-r--r--   0        0        0     1044 2023-10-20 18:48:10.171217 lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_08_wordflashmessages.sql
+-rw-r--r--   0        0        0     1213 2023-10-20 18:48:10.171396 lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_09_wordparents.sql
+-rw-r--r--   0        0        0     2022 2023-10-20 18:48:10.171568 lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_10_words.sql
+-rw-r--r--   0        0        0     1227 2023-10-20 18:48:10.171723 lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_11_books.sql
+-rw-r--r--   0        0        0       56 2023-10-20 18:48:10.171870 lute3-3.4.2b1/lute/db/schema/migrations/20230623_234104_drop_TxTitle.sql
+-rw-r--r--   0        0        0       38 2023-10-20 18:48:10.172012 lute3-3.4.2b1/lute/db/schema/migrations/20230624_182104_drop_index_TxBkIDTxOrder.sql
+-rw-r--r--   0        0        0      908 2023-10-20 18:48:10.172172 lute3-3.4.2b1/lute/db/schema/migrations/20230818_201200_add_BkWordCount.sql
+-rw-r--r--   0        0        0       87 2023-10-20 18:48:10.172337 lute3-3.4.2b1/lute/db/schema/migrations/20230819_044107_drop_texttokens.sql
+-rw-r--r--   0        0        0      168 2023-10-20 18:48:10.172618 lute3-3.4.2b1/lute/db/schema/migrations/20230819_050036_vacuum.sql
+-rw-r--r--   0        0        0      736 2023-10-20 18:48:10.172795 lute3-3.4.2b1/lute/db/schema/migrations/20230827_052154_allow_multiple_word_parents.sql
+-rw-r--r--   0        0        0     1031 2023-10-20 18:48:10.173096 lute3-3.4.2b1/lute/db/schema/migrations/20231018_211236_remove_excess_texts_fields.sql
+-rw-r--r--   0        0        0      930 2023-11-03 01:33:16.686624 lute3-3.4.2b1/lute/db/schema/migrations/20231101_203811_modify_settings_schema.sql
+-rw-r--r--   0        0        0      114 2024-01-13 04:05:05.209858 lute3-3.4.2b1/lute/db/schema/migrations/20231130_141236_add_TxWordCount.sql
+-rw-r--r--   0        0        0      194 2024-01-13 04:05:05.210324 lute3-3.4.2b1/lute/db/schema/migrations/20231210_103924_add_book_audio_fields.sql
+-rw-r--r--   0        0        0       65 2024-02-07 07:50:18.754352 lute3-3.4.2b1/lute/db/schema/migrations/20240101_122610_add_bookstats_status_distribution.sql
+-rw-r--r--   0        0        0       70 2024-02-07 07:50:18.754640 lute3-3.4.2b1/lute/db/schema/migrations/20240113_215142_add_term_follow_parent_bool.sql
+-rw-r--r--   0        0        0      194 2024-02-07 07:50:18.754951 lute3-3.4.2b1/lute/db/schema/migrations/20240118_154258_change_status_abbrev.sql
+-rw-r--r--   0        0        0     1487 2024-02-07 07:50:18.755302 lute3-3.4.2b1/lute/db/schema/migrations/20240125_drop_BkWordCount.sql
+-rw-r--r--   0        0        0     1188 2024-02-07 07:50:18.755674 lute3-3.4.2b1/lute/db/schema/migrations/20240125_drop_bookstats_wordcount.sql
+-rw-r--r--   0        0        0     1877 2024-02-19 02:42:49.355669 lute3-3.4.2b1/lute/db/schema/migrations/20240207_01_create_languagedicts.sql
+-rw-r--r--   0        0        0     1570 2024-02-19 02:42:49.355795 lute3-3.4.2b1/lute/db/schema/migrations/20240207_02_drop_old_language_fields.sql
+-rw-r--r--   0        0        0      224 2023-10-20 18:48:10.173345 lute3-3.4.2b1/lute/db/schema/migrations/README.md
+-rw-r--r--   0        0        0      222 2023-11-03 01:33:16.686865 lute3-3.4.2b1/lute/db/schema/migrations_repeatable/README.md
+-rw-r--r--   0        0        0      992 2024-02-07 07:50:18.756034 lute3-3.4.2b1/lute/db/schema/migrations_repeatable/trig_wordparents.sql
+-rw-r--r--   0        0        0     1751 2024-03-25 09:32:17.264354 lute3-3.4.2b1/lute/db/schema/migrations_repeatable/trig_words.sql
+-rw-r--r--   0        0        0       36 2023-11-03 01:33:16.687020 lute3-3.4.2b1/lute/db/schema/migrations_repeatable/vacuum.sql
+-rw-r--r--   0        0        0        0 2023-10-20 18:48:10.173889 lute3-3.4.2b1/lute/db/setup/__init__.py
+-rw-r--r--   0        0        0     5201 2023-11-11 22:05:26.094785 lute3-3.4.2b1/lute/db/setup/main.py
+-rw-r--r--   0        0        0     3726 2023-11-08 00:06:31.606907 lute3-3.4.2b1/lute/db/setup/migrator.py
+-rw-r--r--   0        0        0        0 2023-11-01 07:45:01.506123 lute3-3.4.2b1/lute/dev_api/__init__.py
+-rw-r--r--   0        0        0     5105 2024-05-18 03:42:18.963958 lute3-3.4.2b1/lute/dev_api/routes.py
+-rw-r--r--   0        0        0        0 2023-10-16 06:20:14.170764 lute3-3.4.2b1/lute/language/__init__.py
+-rw-r--r--   0        0        0     3129 2024-05-06 03:26:32.112645 lute3-3.4.2b1/lute/language/forms.py
+-rw-r--r--   0        0        0     6556 2024-05-27 23:47:17.824457 lute3-3.4.2b1/lute/language/routes.py
+-rw-r--r--   0        0        0     2315 2024-05-18 03:42:18.964238 lute3-3.4.2b1/lute/language/service.py
+-rw-r--r--   0        0        0     3946 2024-05-19 18:38:13.896119 lute3-3.4.2b1/lute/main.py
+-rw-r--r--   0        0        0        0 2023-10-04 05:48:35.020519 lute3-3.4.2b1/lute/models/__init__.py
+-rw-r--r--   0        0        0    11122 2024-03-15 03:25:40.869518 lute3-3.4.2b1/lute/models/book.py
+-rw-r--r--   0        0        0     8838 2024-05-27 23:47:17.824713 lute3-3.4.2b1/lute/models/language.py
+-rw-r--r--   0        0        0     8672 2024-03-13 16:31:06.436856 lute3-3.4.2b1/lute/models/setting.py
+-rw-r--r--   0        0        0    11351 2024-04-28 00:44:07.954290 lute3-3.4.2b1/lute/models/term.py
+-rw-r--r--   0        0        0        0 2023-10-07 05:09:39.898452 lute3-3.4.2b1/lute/parse/__init__.py
+-rw-r--r--   0        0        0     4429 2024-05-27 23:47:17.824945 lute3-3.4.2b1/lute/parse/base.py
+-rw-r--r--   0        0        0     1646 2023-11-08 00:06:31.610408 lute3-3.4.2b1/lute/parse/character_parser.py
+-rw-r--r--   0        0        0     4735 2024-03-08 03:05:01.859524 lute3-3.4.2b1/lute/parse/mecab_parser.py
+-rw-r--r--   0        0        0     2619 2024-05-27 23:47:17.825152 lute3-3.4.2b1/lute/parse/registry.py
+-rw-r--r--   0        0        0     9245 2024-05-18 17:10:47.841027 lute3-3.4.2b1/lute/parse/space_delimited_parser.py
+-rw-r--r--   0        0        0        0 2023-10-16 06:20:14.172648 lute3-3.4.2b1/lute/read/__init__.py
+-rw-r--r--   0        0        0      211 2023-11-08 00:06:31.611930 lute3-3.4.2b1/lute/read/forms.py
+-rw-r--r--   0        0        0        0 2023-10-18 06:43:42.367570 lute3-3.4.2b1/lute/read/render/__init__.py
+-rw-r--r--   0        0        0    17309 2024-05-06 03:26:32.113398 lute3-3.4.2b1/lute/read/render/renderable_calculator.py
+-rw-r--r--   0        0        0     5653 2024-05-18 17:10:47.841457 lute3-3.4.2b1/lute/read/render/service.py
+-rw-r--r--   0        0        0     7010 2024-05-18 17:10:47.841748 lute3-3.4.2b1/lute/read/routes.py
+-rw-r--r--   0        0        0     6636 2024-05-06 03:26:32.113753 lute3-3.4.2b1/lute/read/service.py
+-rw-r--r--   0        0        0        0 2023-11-03 06:31:15.939906 lute3-3.4.2b1/lute/settings/__init__.py
+-rw-r--r--   0        0        0     5329 2024-05-06 03:26:32.114141 lute3-3.4.2b1/lute/settings/routes.py
+-rw-r--r--   0        0        0     1738 2023-10-04 05:48:35.022956 lute3-3.4.2b1/lute/static/css/images/animated-overlay.gif
+-rw-r--r--   0        0        0     2434 2023-10-04 05:48:35.023257 lute3-3.4.2b1/lute/static/css/images/jplayer-black-and-yellow.png
+-rw-r--r--   0        0        0    14525 2023-10-04 05:48:35.023672 lute3-3.4.2b1/lute/static/css/images/jplayer.blue.monday.jpg
+-rw-r--r--   0        0        0   304064 2023-10-04 05:48:35.024510 lute3-3.4.2b1/lute/static/css/images/pbar-ani.gif
+-rw-r--r--   0        0        0      212 2023-10-04 05:48:35.024852 lute3-3.4.2b1/lute/static/css/images/ui-bg_flat_0_555555_40x100.png
+-rw-r--r--   0        0        0      180 2023-10-04 05:48:35.025123 lute3-3.4.2b1/lute/static/css/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rw-r--r--   0        0        0      220 2023-10-04 05:48:35.025729 lute3-3.4.2b1/lute/static/css/images/ui-bg_flat_75_222222_40x100.png
+-rw-r--r--   0        0        0      220 2023-10-04 05:48:35.026029 lute3-3.4.2b1/lute/static/css/images/ui-bg_flat_75_444444_40x100.png
+-rw-r--r--   0        0        0      178 2023-10-04 05:48:35.026359 lute3-3.4.2b1/lute/static/css/images/ui-bg_flat_75_ffffff_40x100.png
+-rw-r--r--   0        0        0      120 2023-10-04 05:48:35.026642 lute3-3.4.2b1/lute/static/css/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0        0        0      105 2023-10-04 05:48:35.026929 lute3-3.4.2b1/lute/static/css/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0        0        0      111 2023-10-04 05:48:35.027288 lute3-3.4.2b1/lute/static/css/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0        0        0      110 2023-10-04 05:48:35.027566 lute3-3.4.2b1/lute/static/css/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0        0        0      119 2023-10-04 05:48:35.027847 lute3-3.4.2b1/lute/static/css/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0        0        0      277 2023-10-04 05:48:35.028257 lute3-3.4.2b1/lute/static/css/images/ui-bg_highlight-soft_75_222222_1x100.png
+-rw-r--r--   0        0        0      101 2023-10-04 05:48:35.028513 lute3-3.4.2b1/lute/static/css/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0        0        0      251 2023-10-04 05:48:35.028793 lute3-3.4.2b1/lute/static/css/images/ui-bg_inset-hard_55_333333_1x100.png
+-rw-r--r--   0        0        0      251 2023-10-04 05:48:35.029316 lute3-3.4.2b1/lute/static/css/images/ui-bg_inset-hard_95_444444_1x100.png
+-rw-r--r--   0        0        0     4369 2023-10-04 05:48:35.029681 lute3-3.4.2b1/lute/static/css/images/ui-icons_222222_256x240.png
+-rw-r--r--   0        0        0     4369 2023-10-04 05:48:35.030066 lute3-3.4.2b1/lute/static/css/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0        0        0     6992 2023-10-04 05:48:35.030537 lute3-3.4.2b1/lute/static/css/images/ui-icons_444444_256x240.png
+-rw-r--r--   0        0        0     4369 2023-10-04 05:48:35.030833 lute3-3.4.2b1/lute/static/css/images/ui-icons_454545_256x240.png
+-rw-r--r--   0        0        0     6988 2023-10-04 05:48:35.031207 lute3-3.4.2b1/lute/static/css/images/ui-icons_555555_256x240.png
+-rw-r--r--   0        0        0     4549 2023-10-04 05:48:35.031493 lute3-3.4.2b1/lute/static/css/images/ui-icons_777620_256x240.png
+-rw-r--r--   0        0        0     6999 2023-10-04 05:48:35.031792 lute3-3.4.2b1/lute/static/css/images/ui-icons_777777_256x240.png
+-rw-r--r--   0        0        0     4369 2023-10-04 05:48:35.032071 lute3-3.4.2b1/lute/static/css/images/ui-icons_888888_256x240.png
+-rw-r--r--   0        0        0     6991 2023-10-04 05:48:35.032366 lute3-3.4.2b1/lute/static/css/images/ui-icons_BBBBBB_256x240.png
+-rw-r--r--   0        0        0     4549 2023-10-04 05:48:35.032703 lute3-3.4.2b1/lute/static/css/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0        0        0     4369 2023-10-04 05:48:35.033223 lute3-3.4.2b1/lute/static/css/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0        0        0     6299 2023-10-04 05:48:35.033571 lute3-3.4.2b1/lute/static/css/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0     8434 2024-04-28 00:44:07.956083 lute3-3.4.2b1/lute/static/css/player-styles.css
+-rw-r--r--   0        0        0    40959 2024-05-18 03:42:18.965669 lute3-3.4.2b1/lute/static/css/styles.css
+-rw-r--r--   0        0        0    15406 2023-10-04 05:48:35.035622 lute3-3.4.2b1/lute/static/favicon.ico
+-rw-r--r--   0        0        0    15406 2023-10-04 05:48:35.036140 lute3-3.4.2b1/lute/static/favicon_dev.ico
+-rw-r--r--   0        0        0      485 2023-10-04 05:48:35.036488 lute3-3.4.2b1/lute/static/icn/arrow-000-medium.png
+-rw-r--r--   0        0        0      479 2023-10-04 05:48:35.036809 lute3-3.4.2b1/lute/static/icn/arrow-180-medium.png
+-rw-r--r--   0        0        0      811 2023-10-04 05:48:35.037131 lute3-3.4.2b1/lute/static/icn/arrow-circle-135.png
+-rw-r--r--   0        0        0      790 2023-10-04 05:48:35.037385 lute3-3.4.2b1/lute/static/icn/arrow-circle-225-left.png
+-rw-r--r--   0        0        0      786 2023-10-04 05:48:35.037680 lute3-3.4.2b1/lute/static/icn/arrow-circle-315.png
+-rw-r--r--   0        0        0      485 2023-10-04 05:48:35.037925 lute3-3.4.2b1/lute/static/icn/arrow-norepeat.png
+-rw-r--r--   0        0        0      587 2023-10-04 05:48:35.038190 lute3-3.4.2b1/lute/static/icn/arrow-repeat.png
+-rw-r--r--   0        0        0      601 2023-10-04 05:48:35.038457 lute3-3.4.2b1/lute/static/icn/arrow-stop.png
+-rw-r--r--   0        0        0      622 2023-10-04 05:48:35.038703 lute3-3.4.2b1/lute/static/icn/book--pencil.png
+-rw-r--r--   0        0        0      650 2023-10-04 05:48:35.038940 lute3-3.4.2b1/lute/static/icn/book-open-bookmark.png
+-rw-r--r--   0        0        0      613 2023-10-04 05:48:35.039204 lute3-3.4.2b1/lute/static/icn/book-open-text.png
+-rw-r--r--   0        0        0      600 2024-02-19 02:42:49.358289 lute3-3.4.2b1/lute/static/icn/book-open-text.svg
+-rw-r--r--   0        0        0      552 2024-01-13 04:05:05.217231 lute3-3.4.2b1/lute/static/icn/bookmark-off.svg
+-rw-r--r--   0        0        0      414 2024-01-13 04:05:05.217572 lute3-3.4.2b1/lute/static/icn/bookmark-on.svg
+-rw-r--r--   0        0        0      784 2023-10-04 05:48:35.039508 lute3-3.4.2b1/lute/static/icn/broom.png
+-rw-r--r--   0        0        0      398 2023-10-04 05:48:35.039745 lute3-3.4.2b1/lute/static/icn/calculator.png
+-rw-r--r--   0        0        0      405 2023-10-04 05:48:35.040009 lute3-3.4.2b1/lute/static/icn/card--minus.png
+-rw-r--r--   0        0        0      556 2023-10-04 05:48:35.040231 lute3-3.4.2b1/lute/static/icn/card--pencil.png
+-rw-r--r--   0        0        0      504 2023-10-04 05:48:35.040493 lute3-3.4.2b1/lute/static/icn/card--plus.png
+-rw-r--r--   0        0        0      473 2023-10-04 05:48:35.040762 lute3-3.4.2b1/lute/static/icn/cards-stack.png
+-rw-r--r--   0        0        0      434 2024-01-13 04:05:05.218143 lute3-3.4.2b1/lute/static/icn/caret-left.svg
+-rw-r--r--   0        0        0      427 2024-01-13 04:05:05.218284 lute3-3.4.2b1/lute/static/icn/caret-right.svg
+-rw-r--r--   0        0        0      369 2023-10-04 05:48:35.041070 lute3-3.4.2b1/lute/static/icn/chain.png
+-rw-r--r--   0        0        0      624 2023-10-04 05:48:35.041330 lute3-3.4.2b1/lute/static/icn/clock.png
+-rw-r--r--   0        0        0      952 2024-02-07 07:50:18.763469 lute3-3.4.2b1/lute/static/icn/close-white.svg
+-rw-r--r--   0        0        0     1438 2024-01-13 04:05:05.219492 lute3-3.4.2b1/lute/static/icn/close.svg
+-rw-r--r--   0        0        0      404 2023-10-04 05:48:35.041576 lute3-3.4.2b1/lute/static/icn/control-180.png
+-rw-r--r--   0        0        0      511 2023-10-04 05:48:35.041944 lute3-3.4.2b1/lute/static/icn/control-stop-180.png
+-rw-r--r--   0        0        0      523 2023-10-04 05:48:35.042219 lute3-3.4.2b1/lute/static/icn/control-stop.png
+-rw-r--r--   0        0        0      405 2023-10-04 05:48:35.042485 lute3-3.4.2b1/lute/static/icn/control.png
+-rw-r--r--   0        0        0      920 2023-10-04 05:48:35.042813 lute3-3.4.2b1/lute/static/icn/cross-big.png
+-rw-r--r--   0        0        0      555 2023-10-04 05:48:35.043135 lute3-3.4.2b1/lute/static/icn/cross-button.png
+-rw-r--r--   0        0        0      544 2023-10-04 05:48:35.043410 lute3-3.4.2b1/lute/static/icn/cross.png
+-rw-r--r--   0        0        0      658 2023-10-04 05:48:35.043716 lute3-3.4.2b1/lute/static/icn/document--pencil.png
+-rw-r--r--   0        0        0     1761 2024-02-07 07:50:18.763842 lute3-3.4.2b1/lute/static/icn/drag-handle.svg
+-rw-r--r--   0        0        0      674 2023-10-04 05:48:35.043952 lute3-3.4.2b1/lute/static/icn/drawer--minus.png
+-rw-r--r--   0        0        0      717 2023-10-04 05:48:35.044272 lute3-3.4.2b1/lute/static/icn/drawer--plus.png
+-rwxr-xr-x   0        0        0       55 2023-10-04 05:48:35.044638 lute3-3.4.2b1/lute/static/icn/empty.gif
+-rw-r--r--   0        0        0      680 2023-10-04 05:48:35.044851 lute3-3.4.2b1/lute/static/icn/eraser.png
+-rw-r--r--   0        0        0      539 2023-10-04 05:48:35.045049 lute3-3.4.2b1/lute/static/icn/exclamation-button.png
+-rw-r--r--   0        0        0      658 2023-10-04 05:48:35.045241 lute3-3.4.2b1/lute/static/icn/exclamation-red.png
+-rw-r--r--   0        0        0      685 2023-10-04 05:48:35.045451 lute3-3.4.2b1/lute/static/icn/external.png
+-rw-r--r--   0        0        0      536 2023-10-04 05:48:35.045663 lute3-3.4.2b1/lute/static/icn/eye.png
+-rw-r--r--   0        0        0      792 2023-10-04 05:48:35.045884 lute3-3.4.2b1/lute/static/icn/feed--pencil.png
+-rw-r--r--   0        0        0      737 2023-10-04 05:48:35.046102 lute3-3.4.2b1/lute/static/icn/feed--plus.png
+-rw-r--r--   0        0        0      566 2024-01-13 04:05:05.221040 lute3-3.4.2b1/lute/static/icn/ff.svg
+-rw-r--r--   0        0        0     1297 2024-01-13 04:05:05.221203 lute3-3.4.2b1/lute/static/icn/font-decrease.svg
+-rw-r--r--   0        0        0     1378 2024-01-13 04:05:05.221326 lute3-3.4.2b1/lute/static/icn/font-increase.svg
+-rw-r--r--   0        0        0      630 2023-10-04 05:48:35.046306 lute3-3.4.2b1/lute/static/icn/funnel--minus.png
+-rw-r--r--   0        0        0      543 2023-10-04 05:48:35.046715 lute3-3.4.2b1/lute/static/icn/funnel.png
+-rw-r--r--   0        0        0      617 2024-02-19 02:42:49.358629 lute3-3.4.2b1/lute/static/icn/images.svg
+-rw-r--r--   0        0        0      692 2023-10-04 05:48:35.047033 lute3-3.4.2b1/lute/static/icn/inbox-download.png
+-rw-r--r--   0        0        0      674 2023-10-04 05:48:35.047235 lute3-3.4.2b1/lute/static/icn/inbox-upload.png
+-rw-r--r--   0        0        0     1553 2023-10-04 05:48:35.047472 lute3-3.4.2b1/lute/static/icn/indicator.gif
+-rw-r--r--   0        0        0     1039 2023-10-04 05:48:35.047683 lute3-3.4.2b1/lute/static/icn/light-bulb-A.png
+-rw-r--r--   0        0        0     1037 2023-10-04 05:48:35.047913 lute3-3.4.2b1/lute/static/icn/light-bulb-T.png
+-rw-r--r--   0        0        0     1010 2023-10-04 05:48:35.048117 lute3-3.4.2b1/lute/static/icn/light-bulb-off-A.png
+-rw-r--r--   0        0        0     1001 2023-10-04 05:48:35.048320 lute3-3.4.2b1/lute/static/icn/light-bulb-off-T.png
+-rw-r--r--   0        0        0      943 2023-10-04 05:48:35.048686 lute3-3.4.2b1/lute/static/icn/light-bulb-off.png
+-rw-r--r--   0        0        0      947 2023-10-04 05:48:35.048956 lute3-3.4.2b1/lute/static/icn/light-bulb.png
+-rw-r--r--   0        0        0      631 2023-10-04 05:48:35.049160 lute3-3.4.2b1/lute/static/icn/lightning.png
+-rw-r--r--   0        0        0     1687 2024-01-13 04:05:05.222154 lute3-3.4.2b1/lute/static/icn/line-spacing-decrease.svg
+-rw-r--r--   0        0        0     2575 2024-01-13 04:05:05.222293 lute3-3.4.2b1/lute/static/icn/line-spacing-increase.svg
+-rw-r--r--   0        0        0      277 2024-02-19 02:42:49.358831 lute3-3.4.2b1/lute/static/icn/list.svg
+-rw-r--r--   0        0        0      451 2023-10-04 05:48:35.049360 lute3-3.4.2b1/lute/static/icn/minus-button.png
+-rw-r--r--   0        0        0      259 2023-10-04 05:48:35.049740 lute3-3.4.2b1/lute/static/icn/minus.png
+-rw-r--r--   0        0        0      489 2023-10-04 05:48:35.049931 lute3-3.4.2b1/lute/static/icn/navigation-000-button-light.png
+-rw-r--r--   0        0        0      614 2023-10-04 05:48:35.050311 lute3-3.4.2b1/lute/static/icn/navigation-000-button.png
+-rw-r--r--   0        0        0      486 2023-10-04 05:48:35.050548 lute3-3.4.2b1/lute/static/icn/navigation-180-button-light.png
+-rw-r--r--   0        0        0      620 2023-10-04 05:48:35.050750 lute3-3.4.2b1/lute/static/icn/navigation-180-button.png
+-rw-r--r--   0        0        0      607 2023-10-04 05:48:35.050975 lute3-3.4.2b1/lute/static/icn/new_line.png
+-rw-r--r--   0        0        0      458 2024-01-13 04:05:05.222661 lute3-3.4.2b1/lute/static/icn/next.svg
+-rw-r--r--   0        0        0      633 2023-10-04 05:48:35.051264 lute3-3.4.2b1/lute/static/icn/notebook--minus.png
+-rw-r--r--   0        0        0      723 2023-10-04 05:48:35.051477 lute3-3.4.2b1/lute/static/icn/notebook--pencil.png
+-rw-r--r--   0        0        0      664 2023-10-04 05:48:35.051850 lute3-3.4.2b1/lute/static/icn/notebook--plus.png
+-rw-r--r--   0        0        0      541 2023-10-04 05:48:35.052045 lute3-3.4.2b1/lute/static/icn/notebook.png
+-rw-r--r--   0        0        0      790 2024-01-13 04:05:05.223020 lute3-3.4.2b1/lute/static/icn/open.svg
+-rw-r--r--   0        0        0      428 2024-01-13 04:05:05.223265 lute3-3.4.2b1/lute/static/icn/pause.svg
+-rw-r--r--   0        0        0      475 2023-10-04 05:48:35.052249 lute3-3.4.2b1/lute/static/icn/pencil.png
+-rw-r--r--   0        0        0     1154 2023-10-04 05:48:35.052521 lute3-3.4.2b1/lute/static/icn/photo-album.png
+-rw-r--r--   0        0        0      591 2024-01-13 04:05:05.223508 lute3-3.4.2b1/lute/static/icn/pin.svg
+-rw-r--r--   0        0        0      142 2023-10-04 05:48:35.052720 lute3-3.4.2b1/lute/static/icn/placeholder.png
+-rw-r--r--   0        0        0      461 2024-01-13 04:05:05.223871 lute3-3.4.2b1/lute/static/icn/play.svg
+-rw-r--r--   0        0        0      583 2023-10-04 05:48:35.052918 lute3-3.4.2b1/lute/static/icn/plus-button.png
+-rw-r--r--   0        0        0      521 2023-10-04 05:48:35.053238 lute3-3.4.2b1/lute/static/icn/plus.png
+-rw-r--r--   0        0        0      445 2024-01-13 04:05:05.224128 lute3-3.4.2b1/lute/static/icn/prev.svg
+-rw-r--r--   0        0        0      722 2023-10-04 05:48:35.053446 lute3-3.4.2b1/lute/static/icn/printer.png
+-rw-r--r--   0        0        0      722 2023-10-04 05:48:35.053709 lute3-3.4.2b1/lute/static/icn/question-balloon.png
+-rw-r--r--   0        0        0      924 2023-10-04 05:48:35.053893 lute3-3.4.2b1/lute/static/icn/question-frame.png
+-rw-r--r--   0        0        0     1921 2024-02-07 07:50:18.764174 lute3-3.4.2b1/lute/static/icn/reload.png
+-rw-r--r--   0        0        0      558 2024-01-13 04:05:05.224511 lute3-3.4.2b1/lute/static/icn/rewind.svg
+-rw-r--r--   0        0        0      837 2023-10-04 05:48:35.054103 lute3-3.4.2b1/lute/static/icn/script-import.png
+-rw-r--r--   0        0        0     1041 2024-03-13 16:31:06.440554 lute3-3.4.2b1/lute/static/icn/settings-gear-icon.svg
+-rw-r--r--   0        0        0      526 2024-01-13 04:05:05.224876 lute3-3.4.2b1/lute/static/icn/skip-back.svg
+-rw-r--r--   0        0        0      755 2023-10-04 05:48:35.054284 lute3-3.4.2b1/lute/static/icn/smiley-sad.png
+-rw-r--r--   0        0        0      811 2023-10-04 05:48:35.054463 lute3-3.4.2b1/lute/static/icn/smiley.png
+-rw-r--r--   0        0        0      452 2023-10-04 05:48:35.054648 lute3-3.4.2b1/lute/static/icn/speaker-volume-none.png
+-rw-r--r--   0        0        0      543 2023-10-04 05:48:35.054955 lute3-3.4.2b1/lute/static/icn/speaker-volume.png
+-rw-r--r--   0        0        0      757 2023-10-04 05:48:35.055365 lute3-3.4.2b1/lute/static/icn/star.png
+-rw-r--r--   0        0        0      432 2023-10-04 05:48:35.055719 lute3-3.4.2b1/lute/static/icn/status-away.png
+-rw-r--r--   0        0        0      407 2023-10-04 05:48:35.056570 lute3-3.4.2b1/lute/static/icn/status-busy.png
+-rw-r--r--   0        0        0      401 2023-10-04 05:48:35.056940 lute3-3.4.2b1/lute/static/icn/status.png
+-rw-r--r--   0        0        0      466 2023-10-04 05:48:35.057163 lute3-3.4.2b1/lute/static/icn/sticky-note--minus.png
+-rw-r--r--   0        0        0      638 2023-10-04 05:48:35.057670 lute3-3.4.2b1/lute/static/icn/sticky-note--pencil.png
+-rw-r--r--   0        0        0      571 2023-10-04 05:48:35.057865 lute3-3.4.2b1/lute/static/icn/sticky-note--plus.png
+-rw-r--r--   0        0        0      520 2023-10-04 05:48:35.058304 lute3-3.4.2b1/lute/static/icn/sticky-note-text.png
+-rw-r--r--   0        0        0      425 2023-10-04 05:48:35.058599 lute3-3.4.2b1/lute/static/icn/sticky-note.png
+-rw-r--r--   0        0        0      533 2023-10-04 05:48:35.058808 lute3-3.4.2b1/lute/static/icn/sticky-notes-stack.png
+-rw-r--r--   0        0        0      618 2023-10-04 05:48:35.059020 lute3-3.4.2b1/lute/static/icn/sticky-notes-text.png
+-rw-r--r--   0        0        0      546 2023-10-04 05:48:35.059221 lute3-3.4.2b1/lute/static/icn/sticky-notes.png
+-rw-r--r--   0        0        0     2805 2023-10-04 05:48:35.059585 lute3-3.4.2b1/lute/static/icn/test_correct.png
+-rw-r--r--   0        0        0     2805 2023-10-04 05:48:35.059871 lute3-3.4.2b1/lute/static/icn/test_notyet.png
+-rw-r--r--   0        0        0     2805 2023-10-04 05:48:35.060061 lute3-3.4.2b1/lute/static/icn/test_wrong.png
+-rw-r--r--   0        0        0      803 2024-01-13 04:05:05.225875 lute3-3.4.2b1/lute/static/icn/text-column-one.svg
+-rw-r--r--   0        0        0     1613 2024-01-13 04:05:05.226200 lute3-3.4.2b1/lute/static/icn/text-column-two.svg
+-rw-r--r--   0        0        0      732 2023-10-04 05:48:35.060251 lute3-3.4.2b1/lute/static/icn/thumb-up.png
+-rw-r--r--   0        0        0      751 2023-10-04 05:48:35.060509 lute3-3.4.2b1/lute/static/icn/thumb.png
+-rwxr-xr-x   0        0        0      620 2023-10-04 05:48:35.060685 lute3-3.4.2b1/lute/static/icn/tick-button-small.png
+-rw-r--r--   0        0        0      568 2023-10-04 05:48:35.060894 lute3-3.4.2b1/lute/static/icn/tick-button.png
+-rw-r--r--   0        0        0      582 2023-10-04 05:48:35.061228 lute3-3.4.2b1/lute/static/icn/tick.png
+-rw-r--r--   0        0        0      521 2024-01-13 04:05:05.226487 lute3-3.4.2b1/lute/static/icn/volume.svg
+-rw-r--r--   0        0        0     3208 2023-10-04 05:48:35.061448 lute3-3.4.2b1/lute/static/icn/waiting.gif
+-rw-r--r--   0        0        0      847 2023-10-04 05:48:35.061633 lute3-3.4.2b1/lute/static/icn/waiting2.gif
+-rw-r--r--   0        0        0     5450 2023-10-04 05:48:35.061895 lute3-3.4.2b1/lute/static/icn/wizard.png
+-rw-r--r--   0        0        0      916 2023-10-04 05:48:35.062193 lute3-3.4.2b1/lute/static/icn/wrench-screwdriver.png
+-rw-r--r--   0        0        0    19567 2023-10-04 05:48:35.062586 lute3-3.4.2b1/lute/static/img/apple-touch-icon-114x114.png
+-rw-r--r--   0        0        0     5618 2023-10-04 05:48:35.062872 lute3-3.4.2b1/lute/static/img/apple-touch-icon-57x57.png
+-rw-r--r--   0        0        0     8461 2023-10-04 05:48:35.063084 lute3-3.4.2b1/lute/static/img/apple-touch-icon-72x72.png
+-rw-r--r--   0        0        0    34198 2023-10-04 05:48:35.063762 lute3-3.4.2b1/lute/static/img/apple-touch-startup.png
+-rw-r--r--   0        0        0    49403 2024-01-13 04:05:05.227551 lute3-3.4.2b1/lute/static/img/lute.png
+-rw-r--r--   0        0        0     1405 2023-10-04 05:48:35.065233 lute3-3.4.2b1/lute/static/img/public_domain.png
+-rw-r--r--   0        0        0     3764 2023-10-04 05:48:35.065440 lute3-3.4.2b1/lute/static/img/ui-icons_444444_256x240.png
+-rw-r--r--   0        0        0     3767 2023-10-04 05:48:35.065634 lute3-3.4.2b1/lute/static/img/ui-icons_555555_256x240.png
+-rw-r--r--   0        0        0     3767 2023-10-04 05:48:35.065982 lute3-3.4.2b1/lute/static/img/ui-icons_777620_256x240.png
+-rw-r--r--   0        0        0     3764 2023-10-04 05:48:35.066190 lute3-3.4.2b1/lute/static/img/ui-icons_777777_256x240.png
+-rw-r--r--   0        0        0     3764 2023-10-04 05:48:35.066397 lute3-3.4.2b1/lute/static/img/ui-icons_cc0000_256x240.png
+-rw-r--r--   0        0        0     3764 2023-10-04 05:48:35.069007 lute3-3.4.2b1/lute/static/img/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    11246 2024-03-13 16:31:06.443010 lute3-3.4.2b1/lute/static/js/dict-tabs.js
+-rw-r--r--   0        0        0    28222 2024-05-18 03:42:18.966179 lute3-3.4.2b1/lute/static/js/lute.js
+-rw-r--r--   0        0        0    12092 2024-04-28 00:44:07.956926 lute3-3.4.2b1/lute/static/js/player.js
+-rw-r--r--   0        0        0     8002 2024-05-06 03:26:32.114878 lute3-3.4.2b1/lute/static/js/resize.js
+-rw-r--r--   0        0        0     4346 2024-02-07 07:50:18.767242 lute3-3.4.2b1/lute/static/js/text-options.js
+-rw-r--r--   0        0        0   202357 2024-03-15 03:25:40.872972 lute3-3.4.2b1/lute/static/vendor/chartjs/chart.umd.js
+-rw-r--r--   0        0        0    50650 2024-03-15 03:25:40.873223 lute3-3.4.2b1/lute/static/vendor/chartjs/chartjs-adapter-date-fns.js
+-rw-r--r--   0        0        0      624 2024-03-15 03:25:40.873755 lute3-3.4.2b1/lute/static/vendor/datatables/README.md
+-rw-r--r--   0        0        0     4145 2024-03-15 03:25:40.873884 lute3-3.4.2b1/lute/static/vendor/datatables/datatables.button.download.js
+-rw-r--r--   0        0        0    41393 2024-03-15 03:25:40.874305 lute3-3.4.2b1/lute/static/vendor/datatables/datatables.min.css
+-rw-r--r--   0        0        0   164670 2024-03-15 03:25:40.875473 lute3-3.4.2b1/lute/static/vendor/datatables/datatables.min.js
+-rw-r--r--   0        0        0     5253 2024-03-15 03:25:40.876688 lute3-3.4.2b1/lute/static/vendor/jquery/jplayer.css
+-rw-r--r--   0        0        0    34497 2024-03-15 03:25:40.876886 lute3-3.4.2b1/lute/static/vendor/jquery/jquery-ui.css
+-rw-r--r--   0        0        0   240422 2024-03-15 03:25:40.879055 lute3-3.4.2b1/lute/static/vendor/jquery/jquery-ui.min.js
+-rw-r--r--   0        0        0     1753 2024-03-15 03:25:40.879212 lute3-3.4.2b1/lute/static/vendor/jquery/jquery.hoverIntent.js
+-rw-r--r--   0        0        0     8067 2024-03-15 03:25:40.879335 lute3-3.4.2b1/lute/static/vendor/jquery/jquery.jeditable.mini.js
+-rw-r--r--   0        0        0    69303 2024-03-15 03:25:40.879593 lute3-3.4.2b1/lute/static/vendor/jquery/jquery.jplayer.js
+-rw-r--r--   0        0        0    60951 2024-03-15 03:25:40.880095 lute3-3.4.2b1/lute/static/vendor/jquery/jquery.jplayer.min.js
+-rw-r--r--   0        0        0    13714 2024-03-15 03:25:40.880340 lute3-3.4.2b1/lute/static/vendor/jquery/jquery.jplayer.swf
+-rw-r--r--   0        0        0    97163 2024-03-15 03:25:40.880764 lute3-3.4.2b1/lute/static/vendor/jquery/jquery.js
+-rwxr-xr-x   0        0        0     2442 2024-03-15 03:25:40.880893 lute3-3.4.2b1/lute/static/vendor/jquery/jquery.scrollTo.min.js
+-rw-r--r--   0        0        0    80119 2024-03-15 03:25:40.881202 lute3-3.4.2b1/lute/static/vendor/jquery/jquery.xpath.min.js
+-rw-r--r--   0        0        0    11207 2024-03-15 03:25:40.881421 lute3-3.4.2b1/lute/static/vendor/tagify/tagify.css
+-rw-r--r--   0        0        0    60507 2024-03-15 03:25:40.881716 lute3-3.4.2b1/lute/static/vendor/tagify/tagify.min.js
+-rw-r--r--   0        0        0    23275 2024-03-15 03:25:40.881883 lute3-3.4.2b1/lute/static/vendor/tagify/tagify.polyfills.min.js
+-rw-r--r--   0        0        0     1723 2024-03-15 03:25:40.882103 lute3-3.4.2b1/lute/static/vendor/tagify/tagify_overrides.css
+-rw-r--r--   0        0        0        0 2024-01-13 04:05:05.232444 lute3-3.4.2b1/lute/stats/__init__.py
+-rw-r--r--   0        0        0      482 2024-01-13 04:05:05.232852 lute3-3.4.2b1/lute/stats/routes.py
+-rw-r--r--   0        0        0     2702 2024-02-07 07:50:18.767674 lute3-3.4.2b1/lute/stats/service.py
+-rw-r--r--   0        0        0     1134 2024-03-15 03:25:40.883026 lute3-3.4.2b1/lute/templates/backup/backup.html
+-rw-r--r--   0        0        0      872 2024-02-19 02:42:49.360741 lute3-3.4.2b1/lute/templates/backup/index.html
+-rw-r--r--   0        0        0     6842 2024-05-04 17:37:40.694306 lute3-3.4.2b1/lute/templates/base.html
+-rw-r--r--   0        0        0     3080 2024-04-28 00:44:07.957672 lute3-3.4.2b1/lute/templates/book/create_new.html
+-rw-r--r--   0        0        0     2503 2024-03-13 16:31:06.446279 lute3-3.4.2b1/lute/templates/book/edit.html
+-rw-r--r--   0        0        0      627 2024-04-28 00:44:07.958136 lute3-3.4.2b1/lute/templates/book/import_webpage.html
+-rw-r--r--   0        0        0      204 2023-11-09 21:55:59.870577 lute3-3.4.2b1/lute/templates/book/index.html
+-rw-r--r--   0        0        0    10771 2024-05-18 01:00:02.776449 lute3-3.4.2b1/lute/templates/book/tablelisting.html
+-rw-r--r--   0        0        0      651 2024-01-13 04:05:05.236118 lute3-3.4.2b1/lute/templates/errors/404_error.html
+-rw-r--r--   0        0        0     1185 2024-01-13 04:05:05.236533 lute3-3.4.2b1/lute/templates/errors/500_error.html
+-rw-r--r--   0        0        0     2278 2024-03-03 03:12:19.455018 lute3-3.4.2b1/lute/templates/hotkeys.html
+-rw-r--r--   0        0        0     5206 2024-03-15 03:25:40.899605 lute3-3.4.2b1/lute/templates/imagesearch/index.html
+-rw-r--r--   0        0        0     1278 2024-04-28 00:44:07.958527 lute3-3.4.2b1/lute/templates/index.html
+-rw-r--r--   0        0        0     7009 2024-02-19 02:42:49.361906 lute3-3.4.2b1/lute/templates/language/_form.html
+-rw-r--r--   0        0        0      131 2023-11-01 07:45:01.587557 lute3-3.4.2b1/lute/templates/language/edit.html
+-rw-r--r--   0        0        0     1427 2024-04-28 00:44:07.958885 lute3-3.4.2b1/lute/templates/language/index.html
+-rw-r--r--   0        0        0     1024 2024-04-28 00:44:07.959127 lute3-3.4.2b1/lute/templates/language/list_predefined.html
+-rw-r--r--   0        0        0      533 2024-02-07 07:50:18.771534 lute3-3.4.2b1/lute/templates/language/new.html
+-rw-r--r--   0        0        0     2522 2024-04-28 00:44:07.959518 lute3-3.4.2b1/lute/templates/read/audio_player.html
+-rw-r--r--   0        0        0      551 2024-03-15 03:25:40.900713 lute3-3.4.2b1/lute/templates/read/flashcopied.html
+-rw-r--r--   0        0        0     1885 2024-03-25 08:52:45.544428 lute3-3.4.2b1/lute/templates/read/frameform.html
+-rw-r--r--   0        0        0    17938 2024-05-17 16:44:15.101791 lute3-3.4.2b1/lute/templates/read/index.html
+-rw-r--r--   0        0        0      605 2024-02-07 07:50:18.773525 lute3-3.4.2b1/lute/templates/read/page_content.html
+-rw-r--r--   0        0        0      755 2024-02-19 02:42:49.362657 lute3-3.4.2b1/lute/templates/read/page_edit_form.html
+-rw-r--r--   0        0        0     4513 2024-05-18 03:42:18.966638 lute3-3.4.2b1/lute/templates/read/reading_menu.html
+-rw-r--r--   0        0        0     1742 2024-03-15 03:25:40.903466 lute3-3.4.2b1/lute/templates/read/termpopup.html
+-rw-r--r--   0        0        0      499 2024-03-08 03:05:01.875375 lute3-3.4.2b1/lute/templates/read/textitem.html
+-rw-r--r--   0        0        0      643 2024-03-15 03:25:40.903763 lute3-3.4.2b1/lute/templates/read/updated.html
+-rw-r--r--   0        0        0     4862 2024-04-28 00:44:07.959944 lute3-3.4.2b1/lute/templates/settings/form.html
+-rw-r--r--   0        0        0     3807 2024-03-15 03:25:40.904464 lute3-3.4.2b1/lute/templates/stats/index.html
+-rw-r--r--   0        0        0    12956 2024-04-28 00:44:07.960314 lute3-3.4.2b1/lute/templates/term/_form.html
+-rw-r--r--   0        0        0     2215 2024-03-13 16:31:06.452196 lute3-3.4.2b1/lute/templates/term/formframes.html
+-rw-r--r--   0        0        0    16104 2024-05-03 16:31:45.659974 lute3-3.4.2b1/lute/templates/term/index.html
+-rw-r--r--   0        0        0     1579 2024-04-28 00:44:07.961040 lute3-3.4.2b1/lute/templates/term/sentences.html
+-rw-r--r--   0        0        0      502 2024-03-15 03:25:40.905825 lute3-3.4.2b1/lute/templates/term_parent_map/index.html
+-rw-r--r--   0        0        0     1093 2024-04-28 00:44:07.961536 lute3-3.4.2b1/lute/templates/termimport/index.html
+-rw-r--r--   0        0        0      755 2024-04-28 00:44:07.961865 lute3-3.4.2b1/lute/templates/termtag/_form.html
+-rw-r--r--   0        0        0      119 2023-10-30 05:47:07.311779 lute3-3.4.2b1/lute/templates/termtag/edit.html
+-rw-r--r--   0        0        0     2654 2024-04-28 00:44:07.962237 lute3-3.4.2b1/lute/templates/termtag/index.html
+-rw-r--r--   0        0        0      170 2023-10-30 05:47:07.312798 lute3-3.4.2b1/lute/templates/termtag/new.html
+-rw-r--r--   0        0        0      654 2024-03-08 03:05:01.878803 lute3-3.4.2b1/lute/templates/version.html
+-rw-r--r--   0        0        0        0 2023-10-21 00:58:40.674085 lute3-3.4.2b1/lute/term/__init__.py
+-rw-r--r--   0        0        0     3353 2024-03-25 09:32:17.277337 lute3-3.4.2b1/lute/term/datatables.py
+-rw-r--r--   0        0        0     4130 2024-03-25 09:32:17.278674 lute3-3.4.2b1/lute/term/forms.py
+-rw-r--r--   0        0        0    16216 2024-04-28 00:44:07.962642 lute3-3.4.2b1/lute/term/model.py
+-rw-r--r--   0        0        0     9475 2024-05-03 16:31:45.660379 lute3-3.4.2b1/lute/term/routes.py
+-rw-r--r--   0        0        0        0 2023-10-28 20:14:27.720594 lute3-3.4.2b1/lute/term_parent_map/__init__.py
+-rw-r--r--   0        0        0     1459 2024-03-15 03:25:40.907485 lute3-3.4.2b1/lute/term_parent_map/routes.py
+-rw-r--r--   0        0        0      866 2024-03-15 03:25:40.907878 lute3-3.4.2b1/lute/term_parent_map/service.py
+-rw-r--r--   0        0        0        0 2023-10-27 22:52:35.310439 lute3-3.4.2b1/lute/termimport/__init__.py
+-rw-r--r--   0        0        0     1793 2024-03-25 09:32:17.280829 lute3-3.4.2b1/lute/termimport/routes.py
+-rw-r--r--   0        0        0     9066 2024-05-11 22:55:05.266422 lute3-3.4.2b1/lute/termimport/service.py
+-rw-r--r--   0        0        0        0 2023-10-30 05:47:07.312889 lute3-3.4.2b1/lute/termtag/__init__.py
+-rw-r--r--   0        0        0      652 2023-11-08 00:06:31.617316 lute3-3.4.2b1/lute/termtag/datatables.py
+-rw-r--r--   0        0        0      309 2023-11-08 00:06:31.617623 lute3-3.4.2b1/lute/termtag/forms.py
+-rw-r--r--   0        0        0     1857 2023-11-08 00:06:31.617959 lute3-3.4.2b1/lute/termtag/routes.py
+-rw-r--r--   0        0        0        0 2024-01-13 04:05:05.250549 lute3-3.4.2b1/lute/themes/__init__.py
+-rw-r--r--   0        0        0     1021 2024-03-08 03:05:01.881349 lute3-3.4.2b1/lute/themes/css/Apple_Books.css
+-rw-r--r--   0        0        0     2603 2024-03-15 03:25:40.908418 lute3-3.4.2b1/lute/themes/css/Dark_slate.css
+-rw-r--r--   0        0        0      949 2024-03-13 16:30:50.208931 lute3-3.4.2b1/lute/themes/css/LWT.css
+-rw-r--r--   0        0        0     1096 2024-03-13 16:30:50.209490 lute3-3.4.2b1/lute/themes/css/LingQ.css
+-rw-r--r--   0        0        0     2835 2024-03-15 03:25:40.909175 lute3-3.4.2b1/lute/themes/css/Night.css
+-rw-r--r--   0        0        0      174 2024-01-13 04:05:05.252115 lute3-3.4.2b1/lute/themes/css/README.md
+-rw-r--r--   0        0        0     1153 2024-03-08 03:05:01.882428 lute3-3.4.2b1/lute/themes/routes.py
+-rw-r--r--   0        0        0     2409 2024-05-06 03:26:32.116432 lute3-3.4.2b1/lute/themes/service.py
+-rw-r--r--   0        0        0        0 2024-01-13 04:05:05.253134 lute3-3.4.2b1/lute/useraudio/__init__.py
+-rw-r--r--   0        0        0      545 2024-01-13 04:05:05.253460 lute3-3.4.2b1/lute/useraudio/routes.py
+-rw-r--r--   0        0        0        0 2023-10-24 05:43:55.069141 lute3-3.4.2b1/lute/userimage/__init__.py
+-rw-r--r--   0        0        0      656 2023-11-08 00:06:31.618260 lute3-3.4.2b1/lute/userimage/routes.py
+-rw-r--r--   0        0        0        0 2023-10-09 03:35:20.090603 lute3-3.4.2b1/lute/utils/__init__.py
+-rw-r--r--   0        0        0     7072 2024-03-13 16:31:06.454810 lute3-3.4.2b1/lute/utils/data_tables.py
+-rw-r--r--   0        0        0     2043 2024-02-07 07:50:18.794729 lute3-3.4.2b1/lute/utils/debug_helpers.py
+-rw-r--r--   0        0        0     1326 2024-03-13 16:30:50.210892 lute3-3.4.2b1/lute/utils/formutils.py
+-rw-r--r--   0        0        0      313 2024-05-18 03:42:18.966723 lute3-3.4.2b1/plugins/lute-mandarin/.pytest.ini
+-rw-r--r--   0        0        0      205 2024-05-27 23:47:17.825356 lute3-3.4.2b1/plugins/lute-mandarin/README.md
+-rw-r--r--   0        0        0     1365 2024-05-27 23:47:17.825551 lute3-3.4.2b1/plugins/lute-mandarin/README_PyPi.md
+-rw-r--r--   0        0        0      416 2024-05-18 03:42:18.966791 lute3-3.4.2b1/plugins/lute-mandarin/definition.yaml
+-rw-r--r--   0        0        0       54 2024-05-27 23:53:11.681963 lute3-3.4.2b1/plugins/lute-mandarin/lute_mandarin_parser/__init__.py
+-rw-r--r--   0        0        0     4772 2024-05-27 23:47:17.826015 lute3-3.4.2b1/plugins/lute-mandarin/lute_mandarin_parser/parser.py
+-rw-r--r--   0        0        0      525 2024-05-27 23:53:11.682082 lute3-3.4.2b1/plugins/lute-mandarin/pyproject.toml
+-rw-r--r--   0        0        0     1538 2024-05-18 03:42:18.967830 lute3-3.4.2b1/plugins/lute-mandarin/requirements.txt
+-rw-r--r--   0        0        0        0 2024-05-27 23:47:17.826244 lute3-3.4.2b1/plugins/lute-mandarin/tests/__init__.py
+-rw-r--r--   0        0        0      823 2024-05-18 03:42:18.968199 lute3-3.4.2b1/plugins/lute-mandarin/tests/conftest.py
+-rw-r--r--   0        0        0     4608 2024-05-27 23:47:17.826704 lute3-3.4.2b1/plugins/lute-mandarin/tests/test_MandarinParser.py
+-rw-r--r--   0        0        0     1226 2024-05-11 22:55:05.266985 lute3-3.4.2b1/pyproject.toml
+-rw-r--r--   0        0        0     1507 2024-05-18 03:42:18.968813 lute3-3.4.2b1/requirements.txt
+-rw-r--r--   0        0        0        0 2024-04-28 00:44:07.964320 lute3-3.4.2b1/scripts/__init__.py
+-rw-r--r--   0        0        0     2564 2024-04-28 00:44:07.964527 lute3-3.4.2b1/scripts/dump_lang_data.py
+-rw-r--r--   0        0        0    10316 2024-05-17 20:10:21.330476 lute3-3.4.2b1/tasks.py
+-rw-r--r--   0        0        0      160 2023-10-22 05:50:12.570821 lute3-3.4.2b1/tests/__init__.py
+-rw-r--r--   0        0        0      442 2023-10-31 05:25:17.232229 lute3-3.4.2b1/tests/acceptance/README.md
+-rw-r--r--   0        0        0      132 2023-11-01 07:45:01.591037 lute3-3.4.2b1/tests/acceptance/__init__.py
+-rw-r--r--   0        0        0     6294 2024-04-28 00:44:07.965096 lute3-3.4.2b1/tests/acceptance/book.feature
+-rw-r--r--   0        0        0    14168 2024-05-18 03:42:18.969323 lute3-3.4.2b1/tests/acceptance/conftest.py
+-rw-r--r--   0        0        0        3 2023-10-31 05:25:17.232861 lute3-3.4.2b1/tests/acceptance/failure_screenshots/.gitignore
+-rw-r--r--   0        0        0       78 2023-10-31 05:25:17.233099 lute3-3.4.2b1/tests/acceptance/failure_screenshots/README.md
+-rw-r--r--   0        0        0    13194 2024-05-18 01:00:02.776994 lute3-3.4.2b1/tests/acceptance/lute_test_client.py
+-rw-r--r--   0        0        0    10086 2024-05-17 21:21:19.865419 lute3-3.4.2b1/tests/acceptance/reading.feature
+-rw-r--r--   0        0        0     1282 2024-02-07 07:50:18.801083 lute3-3.4.2b1/tests/acceptance/sample_files/Hola.epub
+-rw-r--r--   0        0        0     1433 2024-02-07 07:50:18.801387 lute3-3.4.2b1/tests/acceptance/sample_files/Hola.pdf
+-rw-r--r--   0        0        0       48 2024-03-15 03:25:40.913611 lute3-3.4.2b1/tests/acceptance/sample_files/Hola.srt
+-rw-r--r--   0        0        0       56 2024-03-15 03:25:40.913905 lute3-3.4.2b1/tests/acceptance/sample_files/Hola.vtt
+-rw-r--r--   0        0        0       16 2024-01-13 04:05:05.265704 lute3-3.4.2b1/tests/acceptance/sample_files/hola.txt
+-rw-r--r--   0        0        0       16 2024-02-07 07:50:18.801723 lute3-3.4.2b1/tests/acceptance/sample_files/invalid.epub
+-rw-r--r--   0        0        0       16 2024-02-07 07:50:18.801856 lute3-3.4.2b1/tests/acceptance/sample_files/invalid.pdf
+-rw-r--r--   0        0        0       16 2024-03-15 03:25:40.914165 lute3-3.4.2b1/tests/acceptance/sample_files/invalid.srt
+-rw-r--r--   0        0        0       16 2024-03-15 03:25:40.914274 lute3-3.4.2b1/tests/acceptance/sample_files/invalid.vtt
+-rw-r--r--   0        0        0     1417 2024-03-25 09:32:17.283465 lute3-3.4.2b1/tests/acceptance/sample_files/invalid_empty.epub
+-rw-r--r--   0        0        0       74 2024-02-07 07:50:18.802571 lute3-3.4.2b1/tests/acceptance/sample_files/non_utf_8.txt
+-rw-r--r--   0        0        0     2256 2024-03-25 09:32:17.283950 lute3-3.4.2b1/tests/acceptance/smoke.feature
+-rw-r--r--   0        0        0      630 2024-03-08 03:05:01.891609 lute3-3.4.2b1/tests/acceptance/start_acceptance_app.py
+-rw-r--r--   0        0        0     2102 2024-05-18 03:42:18.969654 lute3-3.4.2b1/tests/acceptance/sync_status.feature
+-rw-r--r--   0        0        0     2153 2024-03-15 03:25:40.915397 lute3-3.4.2b1/tests/acceptance/term.feature
+-rw-r--r--   0        0        0       92 2023-11-08 00:06:31.621311 lute3-3.4.2b1/tests/acceptance/test_book.py
+-rw-r--r--   0        0        0       98 2023-11-08 00:06:31.621627 lute3-3.4.2b1/tests/acceptance/test_reading.py
+-rw-r--r--   0        0        0       83 2024-03-25 09:32:17.285207 lute3-3.4.2b1/tests/acceptance/test_smoke.py
+-rw-r--r--   0        0        0      102 2024-05-18 03:42:18.969722 lute3-3.4.2b1/tests/acceptance/test_sync_status.py
+-rw-r--r--   0        0        0       92 2023-11-08 00:06:31.622287 lute3-3.4.2b1/tests/acceptance/test_term.py
+-rw-r--r--   0        0        0      109 2023-11-08 00:06:31.622737 lute3-3.4.2b1/tests/acceptance/test_unsupported_parser.py
+-rw-r--r--   0        0        0     1304 2024-03-25 09:32:17.285870 lute3-3.4.2b1/tests/acceptance/unsupported_parser.feature
+-rw-r--r--   0        0        0     3953 2024-05-18 03:42:18.970148 lute3-3.4.2b1/tests/conftest.py
+-rw-r--r--   0        0        0     1771 2023-11-08 00:06:31.623664 lute3-3.4.2b1/tests/dbasserts.py
+-rw-r--r--   0        0        0      676 2023-10-22 17:27:11.801049 lute3-3.4.2b1/tests/features/README.md
+-rw-r--r--   0        0        0    15205 2024-03-08 03:05:01.894503 lute3-3.4.2b1/tests/features/rendering.feature
+-rw-r--r--   0        0        0    18630 2024-05-11 22:55:05.269192 lute3-3.4.2b1/tests/features/term_import.feature
+-rw-r--r--   0        0        0     2907 2024-03-25 09:32:17.287963 lute3-3.4.2b1/tests/features/term_import_status_0.feature
+-rw-r--r--   0        0        0     3696 2024-03-23 10:37:45.604972 lute3-3.4.2b1/tests/features/test_rendering.py
+-rw-r--r--   0        0        0     3760 2024-03-25 09:32:17.288599 lute3-3.4.2b1/tests/features/test_term_import.py
+-rw-r--r--   0        0        0        0 2023-09-20 06:21:29.988625 lute3-3.4.2b1/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1206 2024-01-13 04:05:05.275517 lute3-3.4.2b1/tests/integration/test_main.py
+-rw-r--r--   0        0        0       97 2023-10-20 06:39:27.112890 lute3-3.4.2b1/tests/orm/README.md
+-rw-r--r--   0        0        0        0 2023-10-20 06:39:27.113017 lute3-3.4.2b1/tests/orm/__init__.py
+-rw-r--r--   0        0        0     2808 2024-02-07 07:50:18.812178 lute3-3.4.2b1/tests/orm/test_Book.py
+-rw-r--r--   0        0        0     3659 2024-02-19 02:42:49.366795 lute3-3.4.2b1/tests/orm/test_Language.py
+-rw-r--r--   0        0        0     8881 2024-04-28 00:44:07.966312 lute3-3.4.2b1/tests/orm/test_Term.py
+-rw-r--r--   0        0        0      871 2023-11-08 00:06:31.626423 lute3-3.4.2b1/tests/orm/test_Text.py
+-rw-r--r--   0        0        0        0 2024-01-13 04:05:05.275609 lute3-3.4.2b1/tests/playwright/__init__.py
+-rw-r--r--   0        0        0     8255 2024-05-04 23:50:35.709807 lute3-3.4.2b1/tests/playwright/playwright.py
+-rw-r--r--   0        0        0        0 2023-09-10 06:10:01.992940 lute3-3.4.2b1/tests/unit/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-30 00:38:51.297976 lute3-3.4.2b1/tests/unit/backup/__init__.py
+-rw-r--r--   0        0        0     9602 2024-02-19 02:42:49.368373 lute3-3.4.2b1/tests/unit/backup/test_backup.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:52:22.684248 lute3-3.4.2b1/tests/unit/book/__init__.py
+-rw-r--r--   0        0        0     3884 2024-04-28 00:44:07.966859 lute3-3.4.2b1/tests/unit/book/test_Repository.py
+-rw-r--r--   0        0        0     2241 2024-03-13 16:30:50.212038 lute3-3.4.2b1/tests/unit/book/test_datatables.py
+-rw-r--r--   0        0        0     4124 2024-02-07 07:50:18.815696 lute3-3.4.2b1/tests/unit/book/test_stats.py
+-rw-r--r--   0        0        0        0 2024-01-13 04:05:05.277883 lute3-3.4.2b1/tests/unit/cli/__init__.py
+-rw-r--r--   0        0        0      867 2024-05-11 22:55:05.269819 lute3-3.4.2b1/tests/unit/cli/test_language_term_export.py
+-rw-r--r--   0        0        0        0 2023-11-04 21:50:44.092388 lute3-3.4.2b1/tests/unit/config/__init__.py
+-rw-r--r--   0        0        0     3035 2024-01-13 04:05:05.278929 lute3-3.4.2b1/tests/unit/config/test_app_config.py
+-rw-r--r--   0        0        0        0 2023-10-26 01:04:31.832624 lute3-3.4.2b1/tests/unit/db/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:48:10.174878 lute3-3.4.2b1/tests/unit/db/setup/__init__.py
+-rw-r--r--   0        0        0       28 2023-10-20 18:48:10.175186 lute3-3.4.2b1/tests/unit/db/setup/schema/README.md
+-rw-r--r--   0        0        0      134 2023-10-20 18:48:10.175437 lute3-3.4.2b1/tests/unit/db/setup/schema/baseline/schema.sql
+-rw-r--r--   0        0        0       24 2023-10-20 18:48:10.175796 lute3-3.4.2b1/tests/unit/db/setup/schema/migrations/123_create_B.sql
+-rw-r--r--   0        0        0       68 2023-10-20 18:48:10.176170 lute3-3.4.2b1/tests/unit/db/setup/schema/repeatable/view_A.sql
+-rw-r--r--   0        0        0     1241 2023-11-08 00:06:31.628181 lute3-3.4.2b1/tests/unit/db/setup/test_BackupManager.py
+-rw-r--r--   0        0        0     8127 2023-11-08 00:06:31.628506 lute3-3.4.2b1/tests/unit/db/setup/test_Setup.py
+-rw-r--r--   0        0        0     3681 2023-11-08 00:06:31.628800 lute3-3.4.2b1/tests/unit/db/setup/test_SqliteMigrator.py
+-rw-r--r--   0        0        0     3107 2024-05-18 03:42:18.971519 lute3-3.4.2b1/tests/unit/db/test_demo.py
+-rw-r--r--   0        0        0     1534 2023-11-11 22:05:26.100552 lute3-3.4.2b1/tests/unit/db/test_management.py
+-rw-r--r--   0        0        0        0 2024-04-28 00:44:07.967194 lute3-3.4.2b1/tests/unit/language/__init__.py
+-rw-r--r--   0        0        0     2396 2024-05-18 03:42:18.971891 lute3-3.4.2b1/tests/unit/language/test_service.py
+-rw-r--r--   0        0        0        0 2023-10-04 05:48:35.085848 lute3-3.4.2b1/tests/unit/models/__init__.py
+-rw-r--r--   0        0        0     1820 2024-03-13 16:30:50.212544 lute3-3.4.2b1/tests/unit/models/test_Book.py
+-rw-r--r--   0        0        0     3102 2024-03-15 03:25:40.916767 lute3-3.4.2b1/tests/unit/models/test_Book_add_remove_pages.py
+-rw-r--r--   0        0        0     2420 2024-04-28 00:44:07.967649 lute3-3.4.2b1/tests/unit/models/test_Language.py
+-rw-r--r--   0        0        0     6167 2024-02-19 02:42:49.368998 lute3-3.4.2b1/tests/unit/models/test_Setting.py
+-rw-r--r--   0        0        0     8034 2024-03-25 09:32:17.290517 lute3-3.4.2b1/tests/unit/models/test_Term.py
+-rw-r--r--   0        0        0     1398 2023-11-08 00:06:31.630600 lute3-3.4.2b1/tests/unit/models/test_TermTag.py
+-rw-r--r--   0        0        0      970 2024-02-07 07:50:18.820113 lute3-3.4.2b1/tests/unit/models/test_Text.py
+-rw-r--r--   0        0        0        0 2023-10-07 05:09:39.900041 lute3-3.4.2b1/tests/unit/parse/__init__.py
+-rw-r--r--   0        0        0     1806 2023-11-08 00:06:31.631135 lute3-3.4.2b1/tests/unit/parse/test_ClassicalChineseParser.py
+-rw-r--r--   0        0        0     2655 2024-03-08 03:05:01.896542 lute3-3.4.2b1/tests/unit/parse/test_JapaneseParser.py
+-rw-r--r--   0        0        0     1452 2023-11-08 00:06:31.631582 lute3-3.4.2b1/tests/unit/parse/test_SentenceGroupIterator.py
+-rw-r--r--   0        0        0     9044 2024-05-06 03:26:32.117861 lute3-3.4.2b1/tests/unit/parse/test_SpaceDelimitedParser.py
+-rw-r--r--   0        0        0      437 2023-11-08 00:06:31.632019 lute3-3.4.2b1/tests/unit/parse/test_TurkishParser.py
+-rw-r--r--   0        0        0     2070 2024-05-27 23:47:17.826999 lute3-3.4.2b1/tests/unit/parse/test_registry.py
+-rw-r--r--   0        0        0        0 2023-10-18 06:43:42.369680 lute3-3.4.2b1/tests/unit/read/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-18 06:43:42.370116 lute3-3.4.2b1/tests/unit/read/render/__init__.py
+-rw-r--r--   0        0        0     4830 2024-05-06 03:26:32.118133 lute3-3.4.2b1/tests/unit/read/render/test_RenderableCalculator.py
+-rw-r--r--   0        0        0     1965 2023-11-08 00:06:31.632694 lute3-3.4.2b1/tests/unit/read/render/test_TokenLocator.py
+-rw-r--r--   0        0        0     5991 2024-03-25 09:32:17.291177 lute3-3.4.2b1/tests/unit/read/test_service.py
+-rw-r--r--   0        0        0     4892 2024-05-06 03:26:32.118479 lute3-3.4.2b1/tests/unit/read/test_service_popup_data.py
+-rw-r--r--   0        0        0        0 2024-01-13 04:05:05.283732 lute3-3.4.2b1/tests/unit/stats/__init__.py
+-rw-r--r--   0        0        0     2467 2024-02-07 07:50:18.821867 lute3-3.4.2b1/tests/unit/stats/test_service.py
+-rw-r--r--   0        0        0        0 2023-10-21 00:58:40.675868 lute3-3.4.2b1/tests/unit/term/__init__.py
+-rw-r--r--   0        0        0    23300 2024-04-28 00:44:07.968765 lute3-3.4.2b1/tests/unit/term/test_Repository.py
+-rw-r--r--   0        0        0     2082 2024-02-07 07:50:18.824210 lute3-3.4.2b1/tests/unit/term/test_TermForm.py
+-rw-r--r--   0        0        0     6766 2024-02-07 07:50:18.824963 lute3-3.4.2b1/tests/unit/term/test_Term_status_follow.py
+-rw-r--r--   0        0        0     1629 2024-01-13 04:05:05.285150 lute3-3.4.2b1/tests/unit/term/test_datatables.py
+-rw-r--r--   0        0        0        0 2023-10-30 23:02:04.731925 lute3-3.4.2b1/tests/unit/term_parent_map/__init__.py
+-rw-r--r--   0        0        0     1255 2024-03-15 03:25:40.918632 lute3-3.4.2b1/tests/unit/term_parent_map/test_service.py
+-rw-r--r--   0        0        0        0 2024-01-13 04:05:05.285261 lute3-3.4.2b1/tests/unit/termtag/__init__.py
+-rw-r--r--   0        0        0      679 2023-11-08 00:06:31.633834 lute3-3.4.2b1/tests/unit/termtag/test_datatables.py
+-rw-r--r--   0        0        0        0 2024-01-13 04:05:05.285353 lute3-3.4.2b1/tests/unit/themes/__init__.py
+-rw-r--r--   0        0        0     3416 2024-05-06 03:26:32.118714 lute3-3.4.2b1/tests/unit/themes/test_service.py
+-rw-r--r--   0        0        0        0 2023-10-09 03:35:20.091806 lute3-3.4.2b1/tests/unit/utils/__init__.py
+-rw-r--r--   0        0        0     5151 2024-01-18 07:46:16.382578 lute3-3.4.2b1/tests/unit/utils/test_DataTablesSqliteQuery.py
+-rw-r--r--   0        0        0      786 2024-03-13 16:30:50.213297 lute3-3.4.2b1/tests/unit/utils/test_formutils.py
+-rw-r--r--   0        0        0     1629 2024-02-07 07:50:18.825866 lute3-3.4.2b1/tests/utils.py
+-rwxr-xr-x   0        0        0     1575 2024-02-19 02:42:49.369401 lute3-3.4.2b1/utils/dump_changelog.sh
+-rwxr-xr-x   0        0        0      565 2024-03-15 03:25:40.919140 lute3-3.4.2b1/utils/findstring.sh
+-rw-r--r--   0        0        0     4820 2023-11-22 00:36:49.803896 lute3-3.4.2b1/utils/todos.py
+-rw-r--r--   0        0        0      698 2023-11-09 08:26:12.057924 lute3-3.4.2b1/utils/verify.py
+-rw-r--r--   0        0        0     2330 1970-01-01 00:00:00.000000 lute3-3.4.2b1/PKG-INFO
```

### Comparing `lute3-3.4.2/.github/ISSUE_TEMPLATE/add_language.md` & `lute3-3.4.2b1/.github/ISSUE_TEMPLATE/add_language.md`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/.github/ISSUE_TEMPLATE/bug_report.md` & `lute3-3.4.2b1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/.github/ISSUE_TEMPLATE/documentation.md` & `lute3-3.4.2b1/.github/ISSUE_TEMPLATE/documentation.md`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/.github/ISSUE_TEMPLATE/feature_request.md` & `lute3-3.4.2b1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/.github/workflows/ci.yml` & `lute3-3.4.2b1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/.github/workflows/coverage.yml` & `lute3-3.4.2b1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/.gitignore` & `lute3-3.4.2b1/.gitignore`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/.pylintrc` & `lute3-3.4.2b1/.pylintrc`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/.pytest.ini` & `lute3-3.4.2b1/.pytest.ini`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/LICENSE.txt` & `lute3-3.4.2b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/README.md` & `lute3-3.4.2b1/README.md`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/README_PyPi.md` & `lute3-3.4.2b1/README_PyPi.md`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/devstart.py` & `lute3-3.4.2b1/devstart.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/docker/Dockerfile` & `lute3-3.4.2b1/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/docker/build_all.sh` & `lute3-3.4.2b1/docker/build_all.sh`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/docker/check_mounts_and_start.sh` & `lute3-3.4.2b1/docker/check_mounts_and_start.sh`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/docker/docker_hub_overview.md` & `lute3-3.4.2b1/docker/docker_hub_overview.md`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/docker/try_build_multi.sh` & `lute3-3.4.2b1/docker/try_build_multi.sh`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/docs/CHANGELOG.md` & `lute3-3.4.2b1/docs/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,8 @@
 
-# 3.4.2 (2024-05-28)
-
-Feature changes:
-
-* #430: add "parser exceptions file" for Mandarin.  See the [Readme on pypi](https://pypi.org/project/lute3-mandarin/) for notes.
-
-Bug fix:
-
-* #436: popup not showing due to Term search error.
-
-
 # 3.4.1 (2024-05-19)
 
 Tweaks/fixes:
 
 * #424: Fix parser plugin loads for python 3.12.  By @cghyzel in #426.
 * #414: Add better startup error message if port already in use.  By @barash-asenov in #423.
```

### Comparing `lute3-3.4.2/lute/LICENSE.txt` & `lute3-3.4.2b1/lute/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/app_factory.py` & `lute3-3.4.2b1/lute/app_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,25 +338,25 @@
     init_parser_plugins()
 
     parsers = supported_parsers()
     parsers_with_extra_data = [
         (typename, klass) for typename, klass in parsers if klass.uses_data_directory()
     ]
     if len(parsers_with_extra_data) > 0:
-        # outfunc("Creating data folders for plugins ...")
+        outfunc("Creating data folders for plugins ...")
         _setup_app_dir(plugin_data_path, "Data files for plugins.")
     for pair in parsers_with_extra_data:
         typename, klass = pair
         dirname = os.path.join(plugin_data_path, typename)
         klass.data_directory = dirname
 
         readme_content = f"Extra data for {klass.name()} plugin."
         _setup_app_dir(dirname, readme_content)
         klass.init_data_directory()
-        # outfunc(f"  * {klass.name()}: {dirname}")
+        outfunc(f"  * {klass.name()}: {dirname}")
 
     outfunc("Enabled parsers:")
     for _, v in supported_parsers():
         outfunc(f"  * {v.name()}")
 
 
 def create_app(
```

### Comparing `lute3-3.4.2/lute/backup/routes.py` & `lute3-3.4.2b1/lute/backup/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/backup/service.py` & `lute3-3.4.2b1/lute/backup/service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/bing/routes.py` & `lute3-3.4.2b1/lute/bing/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/book/datatables.py` & `lute3-3.4.2b1/lute/book/datatables.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/book/forms.py` & `lute3-3.4.2b1/lute/book/forms.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/book/model.py` & `lute3-3.4.2b1/lute/book/model.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/book/routes.py` & `lute3-3.4.2b1/lute/book/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/book/service.py` & `lute3-3.4.2b1/lute/book/service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/book/stats.py` & `lute3-3.4.2b1/lute/book/stats.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/cli/commands.py` & `lute3-3.4.2b1/lute/cli/commands.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/cli/language_term_export.py` & `lute3-3.4.2b1/lute/cli/language_term_export.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/config/app_config.py` & `lute3-3.4.2b1/lute/config/app_config.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/config/config.yml.example` & `lute3-3.4.2b1/lute/config/config.yml.example`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/data_cleanup.py` & `lute3-3.4.2b1/lute/db/data_cleanup.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/demo.py` & `lute3-3.4.2b1/lute/db/demo.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/.github/workflows/ci.yml` & `lute3-3.4.2b1/lute/db/language_defs/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/README.md` & `lute3-3.4.2b1/lute/db/language_defs/README.md`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/afrikaans/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/afrikaans/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/afrikaans/die_diere_grawe_n_put.txt` & `lute3-3.4.2b1/lute/db/language_defs/afrikaans/die_diere_grawe_n_put.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/albanian/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/albanian/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/albanian/shqiponja_dhe_mbreti.txt` & `lute3-3.4.2b1/lute/db/language_defs/albanian/shqiponja_dhe_mbreti.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/amharic/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/amharic/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/amharic/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/amharic/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/arabic/ar_demo.txt` & `lute3-3.4.2b1/lute/db/language_defs/arabic/ar_demo.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/arabic/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/arabic/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/armenian/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/armenian/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/armenian/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/armenian/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/azerbaijani/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/azerbaijani/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/azerbaijani/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/azerbaijani/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/basque/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/basque/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/basque/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/basque/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/belarusian/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/belarusian/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/belarusian/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/belarusian/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/bengali/aharshi_the_bengal_tiger.txt` & `lute3-3.4.2b1/lute/db/language_defs/bengali/aharshi_the_bengal_tiger.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/bengali/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/bengali/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/breton/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/breton/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/breton/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/breton/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/bulgarian/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/bulgarian/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/bulgarian/yesterday_film_description.txt` & `lute3-3.4.2b1/lute/db/language_defs/bulgarian/yesterday_film_description.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/catalan/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/catalan/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/catalan/merlí_series_description.txt` & `lute3-3.4.2b1/lute/db/language_defs/catalan/merlí_series_description.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/classical_chinese/cc_demo.txt` & `lute3-3.4.2b1/lute/db/language_defs/classical_chinese/cc_demo.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/croatian/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/croatian/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/croatian/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/croatian/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/czech/czech.txt` & `lute3-3.4.2b1/lute/db/language_defs/czech/czech.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/danish/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/danish/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/danish/prinsessen_pa_arten.txt` & `lute3-3.4.2b1/lute/db/language_defs/danish/prinsessen_pa_arten.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/dutch/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/dutch/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/english/tutorial.txt` & `lute3-3.4.2b1/lute/db/language_defs/english/tutorial.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/english/tutorial_follow_up.txt` & `lute3-3.4.2b1/lute/db/language_defs/english/tutorial_follow_up.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/esperanto/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/esperanto/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/esperanto/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/esperanto/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/estonian/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/estonian/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/estonian/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/estonian/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/farsi/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/farsi/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/farsi/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/farsi/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/finnish/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/finnish/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/finnish/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/finnish/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/galician/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/galician/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/galician/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/galician/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/generic/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/generic/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/generic/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/generic/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/georgian/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/georgian/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/georgian/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/georgian/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/german/de_Stadtmusikanten.txt` & `lute3-3.4.2b1/lute/db/language_defs/german/de_Stadtmusikanten.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/german/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/german/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/gothic/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/gothic/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/gothic/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/gothic/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/greek/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/greek/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/greek/gr_demo.txt` & `lute3-3.4.2b1/lute/db/language_defs/greek/gr_demo.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/hebrew/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/hebrew/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/hebrew/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/hebrew/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/hindi/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/hindi/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/hindi/hi_wikipedia.txt` & `lute3-3.4.2b1/lute/db/language_defs/hindi/hi_wikipedia.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/hungarian/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/hungarian/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/icelandic/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/icelandic/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/icelandic/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/icelandic/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/indonesian/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/indonesian/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/indonesian/kura-kura_yang_sombong.txt` & `lute3-3.4.2b1/lute/db/language_defs/indonesian/kura-kura_yang_sombong.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/italian/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/italian/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/italian/le_avventure_di_pinocchio.txt` & `lute3-3.4.2b1/lute/db/language_defs/italian/le_avventure_di_pinocchio.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/japanese/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/japanese/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/latin/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/latin/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/latvian/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/latvian/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/latvian/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/latvian/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/lithuanian/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/lithuanian/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/lithuanian/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/lithuanian/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/mandarin_chinese/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/mandarin_chinese/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/norwegian/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/norwegian/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/norwegian/vildanden.txt` & `lute3-3.4.2b1/lute/db/language_defs/norwegian/vildanden.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/polish/adam_i_smoczy_skarb.txt` & `lute3-3.4.2b1/lute/db/language_defs/polish/adam_i_smoczy_skarb.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/polish/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/polish/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/portuguese/a_maldicao.txt` & `lute3-3.4.2b1/lute/db/language_defs/portuguese/a_maldicao.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/portuguese/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/portuguese/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/punjabi/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/punjabi/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/punjabi/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/punjabi/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/romanian/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/romanian/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/russian/ru_medved.txt` & `lute3-3.4.2b1/lute/db/language_defs/russian/ru_medved.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/sanskrit/sanskrit.txt` & `lute3-3.4.2b1/lute/db/language_defs/sanskrit/sanskrit.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/serbian/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/serbian/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/serbian/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/serbian/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/slovak/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/slovak/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/slovak/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/slovak/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/slovene/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/slovene/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/spanish/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/spanish/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/spanish/es_aladino.txt` & `lute3-3.4.2b1/lute/db/language_defs/spanish/es_aladino.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/swahili/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/swahili/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/swahili/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/swahili/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/swedish/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/swedish/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/swedish/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/swedish/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/tibetan/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/tibetan/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/tibetan/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/tibetan/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/turkish/tr_demo.txt` & `lute3-3.4.2b1/lute/db/language_defs/turkish/tr_demo.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/ukrainian/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/ukrainian/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/ukrainian/story_1.txt` & `lute3-3.4.2b1/lute/db/language_defs/ukrainian/story_1.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/verify_files.py` & `lute3-3.4.2b1/lute/db/language_defs/verify_files.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/vietnamese/definition.yaml` & `lute3-3.4.2b1/lute/db/language_defs/vietnamese/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/language_defs/vietnamese/lan_bien.txt` & `lute3-3.4.2b1/lute/db/language_defs/vietnamese/lan_bien.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/management.py` & `lute3-3.4.2b1/lute/db/management.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/README.md` & `lute3-3.4.2b1/lute/db/schema/README.md`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/baseline.sql` & `lute3-3.4.2b1/lute/db/schema/baseline.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/empty.sql` & `lute3-3.4.2b1/lute/db/schema/empty.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20230518_190000_remove_old_words_fields.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20230518_190000_remove_old_words_fields.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20230519_194627_add_TxDateRead.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20230519_194627_add_TxDateRead.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_01_booktags.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_01_booktags.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_02_wordtags.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_02_wordtags.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_03_sentences.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_03_sentences.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_04_texttokens.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_04_texttokens.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_05_texts.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_05_texts.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_06_bookstats.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_06_bookstats.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_07_termimages.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_07_termimages.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_08_wordflashmessages.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_08_wordflashmessages.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_09_wordparents.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_09_wordparents.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_10_words.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_10_words.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20230621_224416_fk_11_books.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20230621_224416_fk_11_books.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20230818_201200_add_BkWordCount.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20230818_201200_add_BkWordCount.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20230827_052154_allow_multiple_word_parents.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20230827_052154_allow_multiple_word_parents.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20231018_211236_remove_excess_texts_fields.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20231018_211236_remove_excess_texts_fields.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20231101_203811_modify_settings_schema.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20231101_203811_modify_settings_schema.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20240125_drop_BkWordCount.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20240125_drop_BkWordCount.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20240125_drop_bookstats_wordcount.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20240125_drop_bookstats_wordcount.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20240207_01_create_languagedicts.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20240207_01_create_languagedicts.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations/20240207_02_drop_old_language_fields.sql` & `lute3-3.4.2b1/lute/db/schema/migrations/20240207_02_drop_old_language_fields.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations_repeatable/trig_wordparents.sql` & `lute3-3.4.2b1/lute/db/schema/migrations_repeatable/trig_wordparents.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/schema/migrations_repeatable/trig_words.sql` & `lute3-3.4.2b1/lute/db/schema/migrations_repeatable/trig_words.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/setup/main.py` & `lute3-3.4.2b1/lute/db/setup/main.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/db/setup/migrator.py` & `lute3-3.4.2b1/lute/db/setup/migrator.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/dev_api/routes.py` & `lute3-3.4.2b1/lute/dev_api/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/language/forms.py` & `lute3-3.4.2b1/lute/language/forms.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/language/routes.py` & `lute3-3.4.2b1/lute/language/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/language/service.py` & `lute3-3.4.2b1/lute/language/service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/main.py` & `lute3-3.4.2b1/lute/main.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/models/book.py` & `lute3-3.4.2b1/lute/models/book.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/models/language.py` & `lute3-3.4.2b1/lute/models/language.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/models/setting.py` & `lute3-3.4.2b1/lute/models/setting.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/models/term.py` & `lute3-3.4.2b1/lute/models/term.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/parse/base.py` & `lute3-3.4.2b1/lute/parse/base.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/parse/character_parser.py` & `lute3-3.4.2b1/lute/parse/character_parser.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/parse/mecab_parser.py` & `lute3-3.4.2b1/lute/parse/mecab_parser.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/parse/registry.py` & `lute3-3.4.2b1/lute/parse/registry.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/parse/space_delimited_parser.py` & `lute3-3.4.2b1/lute/parse/space_delimited_parser.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/read/render/renderable_calculator.py` & `lute3-3.4.2b1/lute/read/render/renderable_calculator.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/read/render/service.py` & `lute3-3.4.2b1/lute/read/render/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,18 +68,18 @@
     lctokens = [parser.get_lowercase(t.token) for t in tokens]
     content = zws + zws.join(lctokens) + zws
 
     sql = sqltext(
         """
         SELECT WoID FROM words
         WHERE WoLgID=:language_id and WoTokenCount>1
-        AND :content LIKE '%' || :zws || WoTextLC || :zws || '%'
+        AND :content LIKE '%' || WoTextLC || '%'
         """
     )
-    sql = sql.bindparams(language_id=language.id, content=content, zws=zws)
+    sql = sql.bindparams(language_id=language.id, content=content)
     idlist = db.session.execute(sql).all()
     woids = [int(p[0]) for p in idlist]
     contained_terms = db.session.query(Term).filter(Term.id.in_(woids)).all()
 
     # Note that the above method (querying for ids, then getting terms)
     # is faster than using the model as shown below!
     ### contained_term_query = db.session.query(Term).filter(
```

### Comparing `lute3-3.4.2/lute/read/routes.py` & `lute3-3.4.2b1/lute/read/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/read/service.py` & `lute3-3.4.2b1/lute/read/service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/settings/routes.py` & `lute3-3.4.2b1/lute/settings/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/css/images/animated-overlay.gif` & `lute3-3.4.2b1/lute/static/css/images/animated-overlay.gif`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/css/images/jplayer-black-and-yellow.png` & `lute3-3.4.2b1/lute/static/css/images/jplayer-black-and-yellow.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/css/images/jplayer.blue.monday.jpg` & `lute3-3.4.2b1/lute/static/css/images/jplayer.blue.monday.jpg`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/css/images/pbar-ani.gif` & `lute3-3.4.2b1/lute/static/css/images/pbar-ani.gif`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/css/images/ui-icons_222222_256x240.png` & `lute3-3.4.2b1/lute/static/css/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/css/images/ui-icons_2e83ff_256x240.png` & `lute3-3.4.2b1/lute/static/css/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/css/images/ui-icons_444444_256x240.png` & `lute3-3.4.2b1/lute/static/css/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/css/images/ui-icons_454545_256x240.png` & `lute3-3.4.2b1/lute/static/css/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/css/images/ui-icons_555555_256x240.png` & `lute3-3.4.2b1/lute/static/css/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/css/images/ui-icons_777620_256x240.png` & `lute3-3.4.2b1/lute/static/css/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/css/images/ui-icons_777777_256x240.png` & `lute3-3.4.2b1/lute/static/css/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/css/images/ui-icons_888888_256x240.png` & `lute3-3.4.2b1/lute/static/css/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/css/images/ui-icons_BBBBBB_256x240.png` & `lute3-3.4.2b1/lute/static/css/images/ui-icons_BBBBBB_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/css/images/ui-icons_cc0000_256x240.png` & `lute3-3.4.2b1/lute/static/css/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/css/images/ui-icons_cd0a0a_256x240.png` & `lute3-3.4.2b1/lute/static/css/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/css/images/ui-icons_ffffff_256x240.png` & `lute3-3.4.2b1/lute/static/css/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/css/player-styles.css` & `lute3-3.4.2b1/lute/static/css/player-styles.css`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/css/styles.css` & `lute3-3.4.2b1/lute/static/css/styles.css`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/favicon.ico` & `lute3-3.4.2b1/lute/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/favicon_dev.ico` & `lute3-3.4.2b1/lute/static/favicon_dev.ico`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/arrow-circle-135.png` & `lute3-3.4.2b1/lute/static/icn/arrow-circle-135.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/arrow-circle-225-left.png` & `lute3-3.4.2b1/lute/static/icn/arrow-circle-225-left.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/arrow-circle-315.png` & `lute3-3.4.2b1/lute/static/icn/arrow-circle-315.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/arrow-repeat.png` & `lute3-3.4.2b1/lute/static/icn/arrow-repeat.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/arrow-stop.png` & `lute3-3.4.2b1/lute/static/icn/arrow-stop.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/book--pencil.png` & `lute3-3.4.2b1/lute/static/icn/book--pencil.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/book-open-bookmark.png` & `lute3-3.4.2b1/lute/static/icn/book-open-bookmark.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/book-open-text.png` & `lute3-3.4.2b1/lute/static/icn/book-open-text.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/book-open-text.svg` & `lute3-3.4.2b1/lute/static/icn/book-open-text.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/bookmark-off.svg` & `lute3-3.4.2b1/lute/static/icn/bookmark-off.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/broom.png` & `lute3-3.4.2b1/lute/static/icn/broom.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/card--pencil.png` & `lute3-3.4.2b1/lute/static/icn/card--pencil.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/clock.png` & `lute3-3.4.2b1/lute/static/icn/clock.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/close-white.svg` & `lute3-3.4.2b1/lute/static/icn/close-white.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/close.svg` & `lute3-3.4.2b1/lute/static/icn/close.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/control-stop.png` & `lute3-3.4.2b1/lute/static/icn/control-stop.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/cross-big.png` & `lute3-3.4.2b1/lute/static/icn/cross-big.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/cross-button.png` & `lute3-3.4.2b1/lute/static/icn/cross-button.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/cross.png` & `lute3-3.4.2b1/lute/static/icn/cross.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/document--pencil.png` & `lute3-3.4.2b1/lute/static/icn/document--pencil.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/drag-handle.svg` & `lute3-3.4.2b1/lute/static/icn/drag-handle.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/drawer--minus.png` & `lute3-3.4.2b1/lute/static/icn/drawer--minus.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/drawer--plus.png` & `lute3-3.4.2b1/lute/static/icn/drawer--plus.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/eraser.png` & `lute3-3.4.2b1/lute/static/icn/eraser.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/exclamation-button.png` & `lute3-3.4.2b1/lute/static/icn/exclamation-button.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/exclamation-red.png` & `lute3-3.4.2b1/lute/static/icn/exclamation-red.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/external.png` & `lute3-3.4.2b1/lute/static/icn/external.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/eye.png` & `lute3-3.4.2b1/lute/static/icn/eye.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/feed--pencil.png` & `lute3-3.4.2b1/lute/static/icn/feed--pencil.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/feed--plus.png` & `lute3-3.4.2b1/lute/static/icn/feed--plus.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/ff.svg` & `lute3-3.4.2b1/lute/static/icn/ff.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/font-decrease.svg` & `lute3-3.4.2b1/lute/static/icn/font-decrease.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/font-increase.svg` & `lute3-3.4.2b1/lute/static/icn/font-increase.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/funnel--minus.png` & `lute3-3.4.2b1/lute/static/icn/funnel--minus.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/funnel.png` & `lute3-3.4.2b1/lute/static/icn/funnel.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/images.svg` & `lute3-3.4.2b1/lute/static/icn/images.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/inbox-download.png` & `lute3-3.4.2b1/lute/static/icn/inbox-download.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/inbox-upload.png` & `lute3-3.4.2b1/lute/static/icn/inbox-upload.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/indicator.gif` & `lute3-3.4.2b1/lute/static/icn/indicator.gif`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/light-bulb-A.png` & `lute3-3.4.2b1/lute/static/icn/light-bulb-A.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/light-bulb-T.png` & `lute3-3.4.2b1/lute/static/icn/light-bulb-T.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/light-bulb-off-A.png` & `lute3-3.4.2b1/lute/static/icn/light-bulb-off-A.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/light-bulb-off-T.png` & `lute3-3.4.2b1/lute/static/icn/light-bulb-off-T.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/light-bulb-off.png` & `lute3-3.4.2b1/lute/static/icn/light-bulb-off.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/light-bulb.png` & `lute3-3.4.2b1/lute/static/icn/light-bulb.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/lightning.png` & `lute3-3.4.2b1/lute/static/icn/lightning.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/line-spacing-decrease.svg` & `lute3-3.4.2b1/lute/static/icn/line-spacing-decrease.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/line-spacing-increase.svg` & `lute3-3.4.2b1/lute/static/icn/line-spacing-increase.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/navigation-000-button.png` & `lute3-3.4.2b1/lute/static/icn/navigation-000-button.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/navigation-180-button.png` & `lute3-3.4.2b1/lute/static/icn/navigation-180-button.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/new_line.png` & `lute3-3.4.2b1/lute/static/icn/new_line.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/notebook--minus.png` & `lute3-3.4.2b1/lute/static/icn/notebook--minus.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/notebook--pencil.png` & `lute3-3.4.2b1/lute/static/icn/notebook--pencil.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/notebook--plus.png` & `lute3-3.4.2b1/lute/static/icn/notebook--plus.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/notebook.png` & `lute3-3.4.2b1/lute/static/icn/notebook.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/open.svg` & `lute3-3.4.2b1/lute/static/icn/open.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/photo-album.png` & `lute3-3.4.2b1/lute/static/icn/photo-album.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/pin.svg` & `lute3-3.4.2b1/lute/static/icn/pin.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/plus-button.png` & `lute3-3.4.2b1/lute/static/icn/plus-button.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/plus.png` & `lute3-3.4.2b1/lute/static/icn/plus.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/printer.png` & `lute3-3.4.2b1/lute/static/icn/printer.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/question-balloon.png` & `lute3-3.4.2b1/lute/static/icn/question-balloon.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/question-frame.png` & `lute3-3.4.2b1/lute/static/icn/question-frame.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/reload.png` & `lute3-3.4.2b1/lute/static/icn/reload.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/rewind.svg` & `lute3-3.4.2b1/lute/static/icn/rewind.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/script-import.png` & `lute3-3.4.2b1/lute/static/icn/script-import.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/settings-gear-icon.svg` & `lute3-3.4.2b1/lute/static/icn/settings-gear-icon.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/skip-back.svg` & `lute3-3.4.2b1/lute/static/icn/skip-back.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/smiley-sad.png` & `lute3-3.4.2b1/lute/static/icn/smiley-sad.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/smiley.png` & `lute3-3.4.2b1/lute/static/icn/smiley.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/speaker-volume.png` & `lute3-3.4.2b1/lute/static/icn/speaker-volume.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/star.png` & `lute3-3.4.2b1/lute/static/icn/star.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/sticky-note--pencil.png` & `lute3-3.4.2b1/lute/static/icn/sticky-note--pencil.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/sticky-note--plus.png` & `lute3-3.4.2b1/lute/static/icn/sticky-note--plus.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/sticky-note-text.png` & `lute3-3.4.2b1/lute/static/icn/sticky-note-text.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/sticky-notes-stack.png` & `lute3-3.4.2b1/lute/static/icn/sticky-notes-stack.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/sticky-notes-text.png` & `lute3-3.4.2b1/lute/static/icn/sticky-notes-text.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/sticky-notes.png` & `lute3-3.4.2b1/lute/static/icn/sticky-notes.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/test_correct.png` & `lute3-3.4.2b1/lute/static/icn/test_correct.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/test_notyet.png` & `lute3-3.4.2b1/lute/static/icn/test_notyet.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/test_wrong.png` & `lute3-3.4.2b1/lute/static/icn/test_wrong.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/text-column-one.svg` & `lute3-3.4.2b1/lute/static/icn/text-column-one.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/text-column-two.svg` & `lute3-3.4.2b1/lute/static/icn/text-column-two.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/thumb-up.png` & `lute3-3.4.2b1/lute/static/icn/thumb-up.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/thumb.png` & `lute3-3.4.2b1/lute/static/icn/thumb.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/tick-button-small.png` & `lute3-3.4.2b1/lute/static/icn/tick-button-small.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/tick-button.png` & `lute3-3.4.2b1/lute/static/icn/tick-button.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/tick.png` & `lute3-3.4.2b1/lute/static/icn/tick.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/volume.svg` & `lute3-3.4.2b1/lute/static/icn/volume.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/waiting.gif` & `lute3-3.4.2b1/lute/static/icn/waiting.gif`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/waiting2.gif` & `lute3-3.4.2b1/lute/static/icn/waiting2.gif`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/wizard.png` & `lute3-3.4.2b1/lute/static/icn/wizard.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/icn/wrench-screwdriver.png` & `lute3-3.4.2b1/lute/static/icn/wrench-screwdriver.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/img/apple-touch-icon-114x114.png` & `lute3-3.4.2b1/lute/static/img/apple-touch-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/img/apple-touch-icon-57x57.png` & `lute3-3.4.2b1/lute/static/img/apple-touch-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/img/apple-touch-icon-72x72.png` & `lute3-3.4.2b1/lute/static/img/apple-touch-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/img/apple-touch-startup.png` & `lute3-3.4.2b1/lute/static/img/apple-touch-startup.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/img/lute.png` & `lute3-3.4.2b1/lute/static/img/lute.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/img/public_domain.png` & `lute3-3.4.2b1/lute/static/img/public_domain.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/img/ui-icons_444444_256x240.png` & `lute3-3.4.2b1/lute/static/img/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/img/ui-icons_555555_256x240.png` & `lute3-3.4.2b1/lute/static/img/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/img/ui-icons_777620_256x240.png` & `lute3-3.4.2b1/lute/static/img/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/img/ui-icons_777777_256x240.png` & `lute3-3.4.2b1/lute/static/img/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/img/ui-icons_cc0000_256x240.png` & `lute3-3.4.2b1/lute/static/img/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/img/ui-icons_ffffff_256x240.png` & `lute3-3.4.2b1/lute/static/img/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/js/dict-tabs.js` & `lute3-3.4.2b1/lute/static/js/dict-tabs.js`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/js/lute.js` & `lute3-3.4.2b1/lute/static/js/lute.js`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/js/player.js` & `lute3-3.4.2b1/lute/static/js/player.js`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/js/resize.js` & `lute3-3.4.2b1/lute/static/js/resize.js`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/js/text-options.js` & `lute3-3.4.2b1/lute/static/js/text-options.js`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/chartjs/chart.umd.js` & `lute3-3.4.2b1/lute/static/vendor/chartjs/chart.umd.js`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/chartjs/chartjs-adapter-date-fns.js` & `lute3-3.4.2b1/lute/static/vendor/chartjs/chartjs-adapter-date-fns.js`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/datatables/README.md` & `lute3-3.4.2b1/lute/static/vendor/datatables/README.md`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/datatables/datatables.button.download.js` & `lute3-3.4.2b1/lute/static/vendor/datatables/datatables.button.download.js`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/datatables/datatables.min.css` & `lute3-3.4.2b1/lute/static/vendor/datatables/datatables.min.css`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/datatables/datatables.min.js` & `lute3-3.4.2b1/lute/static/vendor/datatables/datatables.min.js`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/jquery/jplayer.css` & `lute3-3.4.2b1/lute/static/vendor/jquery/jplayer.css`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/jquery/jquery-ui.css` & `lute3-3.4.2b1/lute/static/vendor/jquery/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/jquery/jquery-ui.min.js` & `lute3-3.4.2b1/lute/static/vendor/jquery/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/jquery/jquery.hoverIntent.js` & `lute3-3.4.2b1/lute/static/vendor/jquery/jquery.hoverIntent.js`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/jquery/jquery.jeditable.mini.js` & `lute3-3.4.2b1/lute/static/vendor/jquery/jquery.jeditable.mini.js`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/jquery/jquery.jplayer.js` & `lute3-3.4.2b1/lute/static/vendor/jquery/jquery.jplayer.js`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/jquery/jquery.jplayer.min.js` & `lute3-3.4.2b1/lute/static/vendor/jquery/jquery.jplayer.min.js`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/jquery/jquery.jplayer.swf` & `lute3-3.4.2b1/lute/static/vendor/jquery/jquery.jplayer.swf`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/jquery/jquery.js` & `lute3-3.4.2b1/lute/static/vendor/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/jquery/jquery.scrollTo.min.js` & `lute3-3.4.2b1/lute/static/vendor/jquery/jquery.scrollTo.min.js`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/jquery/jquery.xpath.min.js` & `lute3-3.4.2b1/lute/static/vendor/jquery/jquery.xpath.min.js`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/tagify/tagify.css` & `lute3-3.4.2b1/lute/static/vendor/tagify/tagify.css`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/tagify/tagify.min.js` & `lute3-3.4.2b1/lute/static/vendor/tagify/tagify.min.js`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/tagify/tagify.polyfills.min.js` & `lute3-3.4.2b1/lute/static/vendor/tagify/tagify.polyfills.min.js`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/static/vendor/tagify/tagify_overrides.css` & `lute3-3.4.2b1/lute/static/vendor/tagify/tagify_overrides.css`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/stats/service.py` & `lute3-3.4.2b1/lute/stats/service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/backup/backup.html` & `lute3-3.4.2b1/lute/templates/backup/backup.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/backup/index.html` & `lute3-3.4.2b1/lute/templates/backup/index.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/base.html` & `lute3-3.4.2b1/lute/templates/base.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/book/create_new.html` & `lute3-3.4.2b1/lute/templates/book/create_new.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/book/edit.html` & `lute3-3.4.2b1/lute/templates/book/edit.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/book/import_webpage.html` & `lute3-3.4.2b1/lute/templates/book/import_webpage.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/book/tablelisting.html` & `lute3-3.4.2b1/lute/templates/book/tablelisting.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/errors/404_error.html` & `lute3-3.4.2b1/lute/templates/errors/404_error.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/errors/500_error.html` & `lute3-3.4.2b1/lute/templates/errors/500_error.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/hotkeys.html` & `lute3-3.4.2b1/lute/templates/hotkeys.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/imagesearch/index.html` & `lute3-3.4.2b1/lute/templates/imagesearch/index.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/index.html` & `lute3-3.4.2b1/lute/templates/index.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/language/_form.html` & `lute3-3.4.2b1/lute/templates/language/_form.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/language/index.html` & `lute3-3.4.2b1/lute/templates/language/index.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/language/list_predefined.html` & `lute3-3.4.2b1/lute/templates/language/list_predefined.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/language/new.html` & `lute3-3.4.2b1/lute/templates/language/new.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/read/audio_player.html` & `lute3-3.4.2b1/lute/templates/read/audio_player.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/read/flashcopied.html` & `lute3-3.4.2b1/lute/templates/read/flashcopied.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/read/frameform.html` & `lute3-3.4.2b1/lute/templates/read/frameform.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/read/index.html` & `lute3-3.4.2b1/lute/templates/read/index.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/read/page_content.html` & `lute3-3.4.2b1/lute/templates/read/page_content.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/read/page_edit_form.html` & `lute3-3.4.2b1/lute/templates/read/page_edit_form.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/read/reading_menu.html` & `lute3-3.4.2b1/lute/templates/read/reading_menu.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/read/termpopup.html` & `lute3-3.4.2b1/lute/templates/read/termpopup.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/read/updated.html` & `lute3-3.4.2b1/lute/templates/read/updated.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/settings/form.html` & `lute3-3.4.2b1/lute/templates/settings/form.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/stats/index.html` & `lute3-3.4.2b1/lute/templates/stats/index.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/term/_form.html` & `lute3-3.4.2b1/lute/templates/term/_form.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/term/formframes.html` & `lute3-3.4.2b1/lute/templates/term/formframes.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/term/index.html` & `lute3-3.4.2b1/lute/templates/term/index.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/term/sentences.html` & `lute3-3.4.2b1/lute/templates/term/sentences.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/termimport/index.html` & `lute3-3.4.2b1/lute/templates/termimport/index.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/termtag/_form.html` & `lute3-3.4.2b1/lute/templates/termtag/_form.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/termtag/index.html` & `lute3-3.4.2b1/lute/templates/termtag/index.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/templates/version.html` & `lute3-3.4.2b1/lute/templates/version.html`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/term/datatables.py` & `lute3-3.4.2b1/lute/term/datatables.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/term/forms.py` & `lute3-3.4.2b1/lute/term/forms.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/term/model.py` & `lute3-3.4.2b1/lute/term/model.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/term/routes.py` & `lute3-3.4.2b1/lute/term/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/term_parent_map/routes.py` & `lute3-3.4.2b1/lute/term_parent_map/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/term_parent_map/service.py` & `lute3-3.4.2b1/lute/term_parent_map/service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/termimport/routes.py` & `lute3-3.4.2b1/lute/termimport/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/termimport/service.py` & `lute3-3.4.2b1/lute/termimport/service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/termtag/datatables.py` & `lute3-3.4.2b1/lute/termtag/datatables.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/termtag/routes.py` & `lute3-3.4.2b1/lute/termtag/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/themes/css/Apple_Books.css` & `lute3-3.4.2b1/lute/themes/css/Apple_Books.css`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/themes/css/Dark_slate.css` & `lute3-3.4.2b1/lute/themes/css/Dark_slate.css`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/themes/css/LWT.css` & `lute3-3.4.2b1/lute/themes/css/LWT.css`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/themes/css/LingQ.css` & `lute3-3.4.2b1/lute/themes/css/LingQ.css`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/themes/css/Night.css` & `lute3-3.4.2b1/lute/themes/css/Night.css`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/themes/routes.py` & `lute3-3.4.2b1/lute/themes/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/themes/service.py` & `lute3-3.4.2b1/lute/themes/service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/useraudio/routes.py` & `lute3-3.4.2b1/lute/useraudio/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/userimage/routes.py` & `lute3-3.4.2b1/lute/userimage/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/utils/data_tables.py` & `lute3-3.4.2b1/lute/utils/data_tables.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/utils/debug_helpers.py` & `lute3-3.4.2b1/lute/utils/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/lute/utils/formutils.py` & `lute3-3.4.2b1/lute/utils/formutils.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/plugins/lute-mandarin/README_PyPi.md` & `lute3-3.4.2b1/plugins/lute-mandarin/README_PyPi.md`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/plugins/lute-mandarin/lute_mandarin_parser/parser.py` & `lute3-3.4.2b1/plugins/lute-mandarin/lute_mandarin_parser/parser.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/plugins/lute-mandarin/pyproject.toml` & `lute3-3.4.2b1/plugins/lute-mandarin/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 requires-python = ">=3.8"
 authors = [
   {name = "Chris Ghyzel"}
 ]
 readme = "README_PyPi.md"
 
 dependencies = [
-  "lute3>=3.4.2",
+  "lute3>=3.4.2b1",
   "jieba>=0.42.1",
   "pypinyin>=0.51.0"
 ]
 
 
 [project.entry-points."lute.plugin.parse"]
 lute_mandarin = "lute_mandarin_parser.parser:MandarinParser"
```

### Comparing `lute3-3.4.2/plugins/lute-mandarin/requirements.txt` & `lute3-3.4.2b1/plugins/lute-mandarin/requirements.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/plugins/lute-mandarin/tests/conftest.py` & `lute3-3.4.2b1/plugins/lute-mandarin/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/plugins/lute-mandarin/tests/test_MandarinParser.py` & `lute3-3.4.2b1/plugins/lute-mandarin/tests/test_MandarinParser.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/pyproject.toml` & `lute3-3.4.2b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/requirements.txt` & `lute3-3.4.2b1/requirements.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/scripts/dump_lang_data.py` & `lute3-3.4.2b1/scripts/dump_lang_data.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tasks.py` & `lute3-3.4.2b1/tasks.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/acceptance/book.feature` & `lute3-3.4.2b1/tests/acceptance/book.feature`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/acceptance/conftest.py` & `lute3-3.4.2b1/tests/acceptance/conftest.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/acceptance/lute_test_client.py` & `lute3-3.4.2b1/tests/acceptance/lute_test_client.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/acceptance/reading.feature` & `lute3-3.4.2b1/tests/acceptance/reading.feature`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/acceptance/sample_files/Hola.epub` & `lute3-3.4.2b1/tests/acceptance/sample_files/Hola.epub`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/acceptance/sample_files/Hola.pdf` & `lute3-3.4.2b1/tests/acceptance/sample_files/Hola.pdf`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/acceptance/sample_files/invalid_empty.epub` & `lute3-3.4.2b1/tests/acceptance/sample_files/invalid_empty.epub`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/acceptance/smoke.feature` & `lute3-3.4.2b1/tests/acceptance/smoke.feature`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/acceptance/start_acceptance_app.py` & `lute3-3.4.2b1/tests/acceptance/start_acceptance_app.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/acceptance/sync_status.feature` & `lute3-3.4.2b1/tests/acceptance/sync_status.feature`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/acceptance/term.feature` & `lute3-3.4.2b1/tests/acceptance/term.feature`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/acceptance/unsupported_parser.feature` & `lute3-3.4.2b1/tests/acceptance/unsupported_parser.feature`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/conftest.py` & `lute3-3.4.2b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/dbasserts.py` & `lute3-3.4.2b1/tests/dbasserts.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/features/README.md` & `lute3-3.4.2b1/tests/features/README.md`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/features/rendering.feature` & `lute3-3.4.2b1/tests/features/rendering.feature`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/features/term_import.feature` & `lute3-3.4.2b1/tests/features/term_import.feature`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/features/term_import_status_0.feature` & `lute3-3.4.2b1/tests/features/term_import_status_0.feature`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/features/test_rendering.py` & `lute3-3.4.2b1/tests/features/test_rendering.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/features/test_term_import.py` & `lute3-3.4.2b1/tests/features/test_term_import.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/integration/test_main.py` & `lute3-3.4.2b1/tests/integration/test_main.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/orm/test_Book.py` & `lute3-3.4.2b1/tests/orm/test_Book.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/orm/test_Language.py` & `lute3-3.4.2b1/tests/orm/test_Language.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/orm/test_Term.py` & `lute3-3.4.2b1/tests/orm/test_Term.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/orm/test_Text.py` & `lute3-3.4.2b1/tests/orm/test_Text.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/playwright/playwright.py` & `lute3-3.4.2b1/tests/playwright/playwright.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/backup/test_backup.py` & `lute3-3.4.2b1/tests/unit/backup/test_backup.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/book/test_Repository.py` & `lute3-3.4.2b1/tests/unit/book/test_Repository.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/book/test_datatables.py` & `lute3-3.4.2b1/tests/unit/book/test_datatables.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/book/test_stats.py` & `lute3-3.4.2b1/tests/unit/book/test_stats.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/cli/test_language_term_export.py` & `lute3-3.4.2b1/tests/unit/cli/test_language_term_export.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/config/test_app_config.py` & `lute3-3.4.2b1/tests/unit/config/test_app_config.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/db/setup/test_BackupManager.py` & `lute3-3.4.2b1/tests/unit/db/setup/test_BackupManager.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/db/setup/test_Setup.py` & `lute3-3.4.2b1/tests/unit/db/setup/test_Setup.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/db/setup/test_SqliteMigrator.py` & `lute3-3.4.2b1/tests/unit/db/setup/test_SqliteMigrator.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/db/test_demo.py` & `lute3-3.4.2b1/tests/unit/db/test_demo.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/db/test_management.py` & `lute3-3.4.2b1/tests/unit/db/test_management.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/language/test_service.py` & `lute3-3.4.2b1/tests/unit/language/test_service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/models/test_Book.py` & `lute3-3.4.2b1/tests/unit/models/test_Book.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/models/test_Book_add_remove_pages.py` & `lute3-3.4.2b1/tests/unit/models/test_Book_add_remove_pages.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/models/test_Language.py` & `lute3-3.4.2b1/tests/unit/models/test_Language.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/models/test_Setting.py` & `lute3-3.4.2b1/tests/unit/models/test_Setting.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/models/test_Term.py` & `lute3-3.4.2b1/tests/unit/models/test_Term.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/models/test_TermTag.py` & `lute3-3.4.2b1/tests/unit/models/test_TermTag.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/models/test_Text.py` & `lute3-3.4.2b1/tests/unit/models/test_Text.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/parse/test_ClassicalChineseParser.py` & `lute3-3.4.2b1/tests/unit/parse/test_ClassicalChineseParser.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/parse/test_JapaneseParser.py` & `lute3-3.4.2b1/tests/unit/parse/test_JapaneseParser.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/parse/test_SentenceGroupIterator.py` & `lute3-3.4.2b1/tests/unit/parse/test_SentenceGroupIterator.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/parse/test_SpaceDelimitedParser.py` & `lute3-3.4.2b1/tests/unit/parse/test_SpaceDelimitedParser.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/parse/test_registry.py` & `lute3-3.4.2b1/tests/unit/parse/test_registry.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/read/render/test_RenderableCalculator.py` & `lute3-3.4.2b1/tests/unit/read/render/test_RenderableCalculator.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/read/render/test_TokenLocator.py` & `lute3-3.4.2b1/tests/unit/read/render/test_TokenLocator.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/read/render/test_service.py` & `lute3-3.4.2b1/tests/unit/read/test_service.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,84 @@
 """
-Render service tests.
+Read service tests.
 """
 
+from lute.models.term import Term
 from lute.parse.base import ParsedToken
+from lute.book.model import Book, Repository
 from lute.read.render.service import find_all_Terms_in_string, get_paragraphs
+from lute.read.service import start_reading
 from lute.db import db
 
 from tests.utils import add_terms, make_text, assert_rendered_text_equals
+from tests.dbasserts import assert_record_count_equals, assert_sql_result
 
 
-def _run_scenario(language, content, expected_found, msg=""):
+def _run_scenario(language, content, expected_found):
     """
     Given some pre-saved terms in language,
     find_all method returns the expected_found terms that
     exist in the content string.
     """
     found_terms = find_all_Terms_in_string(content, language)
-    assert len(found_terms) == len(expected_found), "found count, " + msg
+    assert len(found_terms) == len(expected_found), "found count"
     zws = "\u200B"  # zero-width space
     found_terms = [t.text.replace(zws, "") for t in found_terms]
-    assert found_terms is not None, msg
-    assert expected_found is not None, msg
+    assert found_terms is not None
+    assert expected_found is not None
     found_terms.sort()
     expected_found.sort()
-    assert found_terms == expected_found, msg
-
-
-def test_smoke_tests(english, app_context):
-    "Check bounds, ensure no false matches, etc."
-    add_terms(english, ["a", "at", "xyz"])
-
-    _run_scenario(english, "attack cat", [], "no matches, not standalone")
-    _run_scenario(english, "at", ["at"], "a doesn't match, not standalone")
-    _run_scenario(english, "A", ["a"], "case ignored")
-    _run_scenario(english, "AT A", ["a", "at"], "case, order ignored")
-    _run_scenario(english, "aatt", [], "no match")
-    _run_scenario(english, "Xyz", ["xyz"], "case ignored 2")
-    _run_scenario(english, "XyZ", ["xyz"], "case ignored 3")
-    _run_scenario(english, "      A     at    x", ["a", "at"], "spaces ignored")
-
-    _run_scenario(english, "a dog here", ["a"], "bounds check, found at start")
-    _run_scenario(english, "dog a here", ["a"], "bounds check, found at start")
-    _run_scenario(english, "dog here a", ["a"], "bounds check, found at end")
-    _run_scenario(english, "a a a a a a a", ["a"], "return once only")
-
-    add_terms(english, ["ab xy"])
-    _run_scenario(english, "ab xy", ["ab xy"], "with space")
-    _run_scenario(english, "cab xy", [], "extra at start")
-    _run_scenario(english, "cab xyq", [], "no match, not the same")
-    _run_scenario(english, "ab xyq", [], "extra stuff at end")
+    assert found_terms == expected_found
 
 
 def test_spanish_find_all_in_string(spanish, app_context):
     "Given various pre-saved terms, find_all returns those in the string."
-    add_terms(spanish, ["perro", "gato", "un gato"])
+    terms = ["perro", "gato", "un gato"]
+    for term in terms:
+        t = Term(spanish, term)
+        db.session.add(t)
+    db.session.commit()
 
     _run_scenario(spanish, "Hola tengo un gato", ["gato", "un gato"])
     _run_scenario(spanish, "gato gato gato", ["gato"])
     _run_scenario(spanish, "No tengo UN PERRO", ["perro"])
     _run_scenario(spanish, "Hola tengo un    gato", ["gato", "un gato"])
     _run_scenario(spanish, "No tengo nada", [])
 
-    add_terms(spanish, ["échalo", "ábrela"])
+    terms = ["échalo", "ábrela"]
+    for term in terms:
+        t = Term(spanish, term)
+        db.session.add(t)
+    db.session.commit()
 
     _run_scenario(spanish, '"Échalo", me dijo.', ["échalo"])
     _run_scenario(spanish, "gato ábrela Ábrela", ["gato", "ábrela"])
 
 
 def test_english_find_all_in_string(english, app_context):
     "Can find a term with an apostrophe in string."
-    add_terms(english, ["the cat's pyjamas"])
+    terms = ["the cat's pyjamas"]
+    for term in terms:
+        t = Term(english, term)
+        db.session.add(t)
+    db.session.commit()
 
     _run_scenario(english, "This is the cat's pyjamas.", ["the cat's pyjamas"])
 
 
 def test_turkish_find_all_in_string(turkish, app_context):
     "Finds terms, handling case conversion."
-    add_terms(turkish, ["ışık", "için"])
+    terms = ["ışık", "için"]
+    for term in terms:
+        t = Term(turkish, term)
+        db.session.add(t)
+    db.session.commit()
 
-    _run_scenario(turkish, "Işık İçin.", ["ışık", "için"])
+    content = "Işık İçin."
+    _run_scenario(turkish, content, ["ışık", "için"])
 
 
 def test_smoke_get_paragraphs(spanish, app_context):
     """
     Smoke test to get paragraph information.
     """
     add_terms(spanish, ["tengo un", "un gato"])
@@ -144,7 +140,56 @@
 
     expected = [
         "Tengo un(1)/ gato(1)/. /Hay/ /un/ /perro/.",
         "",
         "Tengo un(1)/ /perro/.",
     ]
     assert_rendered_text_equals(text, expected)
+
+
+## Start reading tests. ##########################
+
+
+def test_smoke_start_reading(english, app_context):
+    "Smoke test book."
+    b = Book()
+    b.title = "blah"
+    b.language_id = english.id
+    b.text = "Here is some content.  Here is more."
+    r = Repository(db)
+    dbbook = r.add(b)
+    r.commit()
+
+    assert_record_count_equals("select * from sentences", 0, "before start")
+    start_reading(dbbook, 1, db.session)
+    assert_record_count_equals("select * from sentences", 2, "after start")
+
+
+def test_start_reading_creates_Terms_for_unknown_words(english, app_context):
+    "Unknown (status 0) terms are created for all new words."
+    t = Term(english, "dog")
+    db.session.add(t)
+    db.session.commit()
+
+    b = Book()
+    b.title = "blah"
+    b.language_id = english.id
+    b.text = "Dog CAT dog cat."
+    r = Repository(db)
+    dbbook = r.add(b)
+    r.commit()
+
+    sql = "select WoTextLC from words order by WoText"
+    assert_sql_result(sql, ["dog"], "before start")
+
+    paragraphs = start_reading(dbbook, 1, db.session)
+    textitems = [
+        ti
+        for para in paragraphs
+        for sentence in para
+        for ti in sentence.textitems
+        if ti.is_word and ti.wo_id is None
+    ]
+    assert (
+        len(textitems) == 0
+    ), f"All text items should have a term, but got {textitems}"
+    assert_sql_result(sql, ["cat", "dog"], "after start")
```

### Comparing `lute3-3.4.2/tests/unit/read/test_service_popup_data.py` & `lute3-3.4.2b1/tests/unit/read/test_service_popup_data.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/stats/test_service.py` & `lute3-3.4.2b1/tests/unit/stats/test_service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/term/test_Repository.py` & `lute3-3.4.2b1/tests/unit/term/test_Repository.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/term/test_TermForm.py` & `lute3-3.4.2b1/tests/unit/term/test_TermForm.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/term/test_Term_status_follow.py` & `lute3-3.4.2b1/tests/unit/term/test_Term_status_follow.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/term/test_datatables.py` & `lute3-3.4.2b1/tests/unit/term/test_datatables.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/term_parent_map/test_service.py` & `lute3-3.4.2b1/tests/unit/term_parent_map/test_service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/termtag/test_datatables.py` & `lute3-3.4.2b1/tests/unit/termtag/test_datatables.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/themes/test_service.py` & `lute3-3.4.2b1/tests/unit/themes/test_service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/utils/test_DataTablesSqliteQuery.py` & `lute3-3.4.2b1/tests/unit/utils/test_DataTablesSqliteQuery.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/unit/utils/test_formutils.py` & `lute3-3.4.2b1/tests/unit/utils/test_formutils.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/tests/utils.py` & `lute3-3.4.2b1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/utils/dump_changelog.sh` & `lute3-3.4.2b1/utils/dump_changelog.sh`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/utils/findstring.sh` & `lute3-3.4.2b1/utils/findstring.sh`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/utils/todos.py` & `lute3-3.4.2b1/utils/todos.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/utils/verify.py` & `lute3-3.4.2b1/utils/verify.py`

 * *Files identical despite different names*

### Comparing `lute3-3.4.2/PKG-INFO` & `lute3-3.4.2b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lute3
-Version: 3.4.2
+Version: 3.4.2b1
 Summary: Learning Using Texts
 Author-email: Jeff Zohrab <jzohrab@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: Flask-SQLAlchemy>=3.1.1,<4
 Requires-Dist: Flask-WTF>=1.2.1,<2
 Requires-Dist: natto-py>=1.0.1,<2
```

