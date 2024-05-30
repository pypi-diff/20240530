# Comparing `tmp/blastpipe-2024.9.2.tar.gz` & `tmp/blastpipe-2024.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blastpipe-2024.9.2.tar", last modified: Thu May 23 02:12:41 2024, max compression
+gzip compressed data, was "blastpipe-2024.9.3.tar", last modified: Mon May 27 21:02:53 2024, max compression
```

## Comparing `blastpipe-2024.9.2.tar` & `blastpipe-2024.9.3.tar`

### file list

```diff
@@ -1,310 +1,310 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.944339 blastpipe-2024.9.2/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.884339 blastpipe-2024.9.2/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.888339 blastpipe-2024.9.2/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     7630 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/.github/workflows/ozi.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/.github/workflows/scorecards.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/.pre-commit-config.yaml
--rw-rw-r--   0 runner    (1001) docker     (127)   120245 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12458 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/LICENSE.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-05-23 02:12:32.604339 blastpipe-2024.9.2/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     3542 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/README.rst
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.940339 blastpipe-2024.9.2/blastpipe/
--rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/__init__.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/backports.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/buffer.py
--rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/buffer.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/loop.py
--rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/loop.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/malloc.py
--rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/malloc.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1250 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/mixin.py
--rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/mixin.pyi
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.940339 blastpipe-2024.9.2/blastpipe/ozi_templates/
--rw-rw-r--   0 runner    (1001) docker     (127)      361 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/.gitignore.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      212 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/CHANGELOG.md.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      344 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/LICENSE.txt.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      114 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/PKG-INFO.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      353 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/README.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      523 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/README.md.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      628 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/README.rst.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      490 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/README.txt.j2
--rw-rw-r--   0 runner    (1001) docker     (127)     1867 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      663 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/__init__.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)      271 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/bandit.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      269 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/bandit.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      268 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/black.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      230 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/black.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      629 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/coverage.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      222 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/doc8.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      126 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/doc8.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     2801 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/filter.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1379 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/filter.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)      387 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/flake8.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/flake8.pyproject.toml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.896339 blastpipe-2024.9.2/blastpipe/ozi_templates/github_workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     1745 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/github_workflows/checkpoint.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      880 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/github_workflows/draft.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      807 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/github_workflows/generate_provenance.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/github_workflows/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      651 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/github_workflows/ozi.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      766 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/github_workflows/publish.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)     1314 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/github_workflows/release.yml.j2
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.900339 blastpipe-2024.9.2/blastpipe/ozi_templates/gitlab_workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)      337 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/gitlab_workflows/ozi.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      351 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/isort.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/isort.pyproject.toml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.932339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.900339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/cc0-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      357 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.904339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/agpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/agpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/apache-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/artistic-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/bsd-3-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    18660 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/cc-by-4.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    20141 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/cc-by-sa-4.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/epl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/gpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/gpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/gpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/gpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/isc.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.1-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/lgpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/lgpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      849 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/mit.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/ofl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      485 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/wtfpl.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/zlib.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.904339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/
--rw-rw-r--   0 runner    (1001) docker     (127)    11067 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      373 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ncsa.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.924339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.904339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/
--rw-rw-r--   0 runner    (1001) docker     (127)    10315 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.904339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/
--rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/apache-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      374 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.908339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/
--rw-rw-r--   0 runner    (1001) docker     (127)    19765 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    20209 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    19902 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    21198 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      433 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.908339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/
--rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/artistic-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      376 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.908339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/
--rw-rw-r--   0 runner    (1001) docker     (127)      710 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/0bsd.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1346 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-3-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1713 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.908339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)     1340 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.912339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/
--rw-rw-r--   0 runner    (1001) docker     (127)    22960 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      374 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.912339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/epl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.912339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)    14199 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.912339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/
--rw-rw-r--   0 runner    (1001) docker     (127)    13154 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      372 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.912339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/
--rw-rw-r--   0 runner    (1001) docker     (127)    13831 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      372 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.912339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.912339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/agpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.916339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.916339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      457 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.916339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      405 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.916339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/gpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.916339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      405 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.916339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/gpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.920339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.1-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.920339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.1-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.920339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.920339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/lgpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.920339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.1-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      461 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.920339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/isc.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      367 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.924339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/
--rw-rw-r--   0 runner    (1001) docker     (127)      367 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/mit.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.924339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      952 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.924339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       88 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/mpl-2.0.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.924339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)      477 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     9269 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.924339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)      456 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    10302 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.924339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/
--rw-rw-r--   0 runner    (1001) docker     (127)      374 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.924339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/
--rw-rw-r--   0 runner    (1001) docker     (127)      456 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/ofl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1641 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.924339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/
--rw-rw-r--   0 runner    (1001) docker     (127)      437 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/zlib.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.928339 blastpipe-2024.9.2/blastpipe/ozi_templates/license/Public_Domain/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/Public_Domain/cc0-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/Public_Domain/licenseref-public-domain.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      414 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/Public_Domain/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1213 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/Public_Domain/unlicense.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    34525 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/agpl-3.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    11359 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/apache-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     8896 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/artistic-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1544 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/bsd-3-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     7050 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/cc0-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    11587 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/epl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    22965 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/gfdl-1.3.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    18094 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/gpl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    35151 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/gpl-3.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      788 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/isc.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    25381 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/lgpl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    26528 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/lgpl-2.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     7654 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/lgpl-3.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1185 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1114 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/mit.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      260 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/ofl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      901 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/license/zlib.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1973 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      420 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/meson.build.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      931 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/meson.options.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      170 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/mypy.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      248 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/mypy.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     1153 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/new_child.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      355 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/ozi.wrap.j2
--rw-rw-r--   0 runner    (1001) docker     (127)     2769 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/project.PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     1140 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/project.array.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      623 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/project.feature.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      546 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/project.integer.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     3698 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/project.meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.936339 blastpipe-2024.9.2/blastpipe/ozi_templates/project.name/
--rw-rw-r--   0 runner    (1001) docker     (127)      280 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/project.name/__init__.py.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      291 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/project.name/__init__.pyi.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/project.name/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1127 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/project.name/meson.build.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/project.name/new_ext.pyx.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/project.name/new_module.py.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      131 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/project.name/py.typed.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      212 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/project.ozi.wrap.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      253 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/pydocstyle.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      280 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/pylint.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      682 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/pyproject.toml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      233 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/pyright.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      247 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/pyright.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      394 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/pytest.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      424 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/pytest.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      196 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/readme-renderer.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      152 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/requirements.in.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      231 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/restructuredtext-lint.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     1221 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/root.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     1128 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/ruff.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     1204 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/semantic_release.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      343 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/setuptools_scm.pyproject.toml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.940339 blastpipe-2024.9.2/blastpipe/ozi_templates/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      723 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/tests/meson.build.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      262 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/tests/new_test.py.j2
--rw-rw-r--   0 runner    (1001) docker     (127)     1713 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/ozi_templates/tox.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/sequence.py
--rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/sequence.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/tailcall.py
--rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/blastpipe/tailcall.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3291 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4520 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     8453 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)       33 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.944339 blastpipe-2024.9.2/subprojects/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.944339 blastpipe-2024.9.2/subprojects/docs/
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/subprojects/docs/LICENSE.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.940339 blastpipe-2024.9.2/subprojects/docs/_static/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.940339 blastpipe-2024.9.2/subprojects/docs/_static/css/
--rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/subprojects/docs/_static/css/custom.css
--rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/subprojects/docs/_static/css/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/subprojects/docs/_static/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.944339 blastpipe-2024.9.2/subprojects/docs/_templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/subprojects/docs/_templates/layout.html
--rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/subprojects/docs/_templates/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/subprojects/docs/conf.cfg
--rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/subprojects/docs/index.rst
--rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/subprojects/docs/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/subprojects/docs/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      115 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/subprojects/ozi.wrap
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:12:32.944339 blastpipe-2024.9.2/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      832 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/tests/test_backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1072 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/tests/test_filter.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/tests/test_fuzz.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-05-23 02:09:16.000000 blastpipe-2024.9.2/tests/test_tailcall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.440571 blastpipe-2024.9.3/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.380572 blastpipe-2024.9.3/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.384572 blastpipe-2024.9.3/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     7630 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/.github/workflows/ozi.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/.github/workflows/scorecards.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/.pre-commit-config.yaml
+-rw-rw-r--   0 runner    (1001) docker     (127)   122174 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12458 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/LICENSE.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-05-27 21:02:44.096572 blastpipe-2024.9.3/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     3542 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/README.rst
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.436571 blastpipe-2024.9.3/blastpipe/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/__init__.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/backports.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/buffer.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/buffer.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/loop.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/loop.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/malloc.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/malloc.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1250 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/mixin.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/mixin.pyi
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.436571 blastpipe-2024.9.3/blastpipe/ozi_templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)      361 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/.gitignore.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      212 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/CHANGELOG.md.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      344 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/LICENSE.txt.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      114 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/PKG-INFO.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      353 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/README.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      523 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/README.md.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      628 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/README.rst.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      490 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/README.txt.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     1867 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      663 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/__init__.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)      271 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/bandit.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      269 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/bandit.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      268 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/black.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      230 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/black.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      629 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/coverage.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      222 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/doc8.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      126 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/doc8.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     2801 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/filter.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1379 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/filter.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)      387 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/flake8.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/flake8.pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.392572 blastpipe-2024.9.3/blastpipe/ozi_templates/github_workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1745 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/github_workflows/checkpoint.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      880 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/github_workflows/draft.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      807 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/github_workflows/generate_provenance.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/github_workflows/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      651 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/github_workflows/ozi.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      766 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/github_workflows/publish.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     1314 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/github_workflows/release.yml.j2
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.392572 blastpipe-2024.9.3/blastpipe/ozi_templates/gitlab_workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)      337 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/gitlab_workflows/ozi.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      351 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/isort.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/isort.pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.428572 blastpipe-2024.9.3/blastpipe/ozi_templates/license/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.396571 blastpipe-2024.9.3/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/cc0-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      357 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.400571 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/agpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/agpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/apache-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/artistic-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/bsd-3-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    18660 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/cc-by-4.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    20141 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/cc-by-sa-4.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/epl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/gpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/gpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/isc.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/lgpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      849 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/mit.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/ofl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      485 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/wtfpl.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/zlib.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.400571 blastpipe-2024.9.3/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/
+-rw-rw-r--   0 runner    (1001) docker     (127)    11067 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      373 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ncsa.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.420571 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.400571 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    10315 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.400571 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/apache-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      374 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.404572 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)    19765 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    20209 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    19902 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    21198 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      433 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.404572 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/artistic-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      376 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.404572 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      710 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/0bsd.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1346 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-3-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1713 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.404572 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1340 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.408572 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    22960 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      374 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.408572 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/epl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.408572 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    14199 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.408572 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    13154 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      372 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.408572 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    13831 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      372 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.408572 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.408572 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/agpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.412572 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.412572 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      457 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.412572 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      405 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.412572 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.412572 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      405 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.412572 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.416571 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.416571 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.416571 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.416571 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.416571 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      461 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.416571 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/isc.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      367 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.420571 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      367 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/mit.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.420571 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      952 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.420571 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       88 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/mpl-2.0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.420571 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      477 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     9269 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.420571 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      456 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    10302 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.420571 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      374 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.420571 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      456 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/ofl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1641 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.424572 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      437 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/zlib.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.424572 blastpipe-2024.9.3/blastpipe/ozi_templates/license/Public_Domain/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/Public_Domain/cc0-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/Public_Domain/licenseref-public-domain.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      414 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/Public_Domain/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1213 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/Public_Domain/unlicense.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    34525 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/agpl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    11359 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/apache-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     8896 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/artistic-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1544 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/bsd-3-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7050 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/cc0-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    11587 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/epl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    22965 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/gfdl-1.3.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    18094 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/gpl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    35151 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/gpl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      788 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/isc.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    25381 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/lgpl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    26528 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/lgpl-2.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7654 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/lgpl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1185 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1114 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/mit.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      260 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/ofl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      901 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/license/zlib.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1973 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      420 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/meson.build.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      931 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/meson.options.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      170 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/mypy.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      248 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/mypy.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1153 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/new_child.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      355 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/ozi.wrap.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     2769 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/project.PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     1140 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/project.array.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      623 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/project.feature.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      546 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/project.integer.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     3698 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/project.meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.432572 blastpipe-2024.9.3/blastpipe/ozi_templates/project.name/
+-rw-rw-r--   0 runner    (1001) docker     (127)      280 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/project.name/__init__.py.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      291 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/project.name/__init__.pyi.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/project.name/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1127 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/project.name/meson.build.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/project.name/new_ext.pyx.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/project.name/new_module.py.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      131 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/project.name/py.typed.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      212 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/project.ozi.wrap.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      253 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/pydocstyle.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      280 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/pylint.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      682 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/pyproject.toml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      233 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/pyright.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      247 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/pyright.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      394 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/pytest.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      424 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/pytest.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      196 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/readme-renderer.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      152 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/requirements.in.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      231 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/restructuredtext-lint.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     1221 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/root.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1128 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/ruff.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1204 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/semantic_release.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      343 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/setuptools_scm.pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.436571 blastpipe-2024.9.3/blastpipe/ozi_templates/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      723 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/tests/meson.build.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      262 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/tests/new_test.py.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     1713 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/ozi_templates/tox.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/sequence.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/sequence.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/tailcall.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/blastpipe/tailcall.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3291 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4520 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     8453 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)       33 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.440571 blastpipe-2024.9.3/subprojects/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.440571 blastpipe-2024.9.3/subprojects/docs/
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/subprojects/docs/LICENSE.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.440571 blastpipe-2024.9.3/subprojects/docs/_static/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.440571 blastpipe-2024.9.3/subprojects/docs/_static/css/
+-rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/subprojects/docs/_static/css/custom.css
+-rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/subprojects/docs/_static/css/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/subprojects/docs/_static/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.440571 blastpipe-2024.9.3/subprojects/docs/_templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/subprojects/docs/_templates/layout.html
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/subprojects/docs/_templates/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/subprojects/docs/conf.cfg
+-rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/subprojects/docs/index.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/subprojects/docs/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/subprojects/docs/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      115 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/subprojects/ozi.wrap
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:02:44.440571 blastpipe-2024.9.3/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      832 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/tests/test_backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1072 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/tests/test_filter.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/tests/test_fuzz.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-05-27 20:59:31.000000 blastpipe-2024.9.3/tests/test_tailcall.py
```

### Comparing `blastpipe-2024.9.2/.github/workflows/codeql.yml` & `blastpipe-2024.9.3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/.github/workflows/dependency-review.yml` & `blastpipe-2024.9.3/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/.github/workflows/ozi.yml` & `blastpipe-2024.9.3/.github/workflows/ozi.yml`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             pypi.org:443
             registry.npmjs.org:443
             objects.githubusercontent.com:443
             fulcio.sigstore.dev:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/checkpoint@0c54a8e9bbbe5817b8c75a97b4cd6871a64f65f7
+      - uses: OZI-Project/checkpoint@64e790c506ba8df435c545f0d4135fbfde23f6a0
         with:
           python-version: "3.10"
 
   checkpoint-cp311-ubuntu-latest:
     name: checkpoint (Python 3.11 on ubuntu-latest)
     runs-on: ubuntu-latest
     strategy:
@@ -64,15 +64,15 @@
             pypi.org:443
             registry.npmjs.org:443
             objects.githubusercontent.com:443
             fulcio.sigstore.dev:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/checkpoint@0c54a8e9bbbe5817b8c75a97b4cd6871a64f65f7
+      - uses: OZI-Project/checkpoint@64e790c506ba8df435c545f0d4135fbfde23f6a0
         with:
           python-version: "3.11"
 
   checkpoint-cp312-ubuntu-latest:
     name: checkpoint (Python 3.12 on ubuntu-latest)
     runs-on: ubuntu-latest
     strategy:
@@ -93,15 +93,15 @@
             pypi.org:443
             registry.npmjs.org:443
             objects.githubusercontent.com:443
             fulcio.sigstore.dev:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/checkpoint@0c54a8e9bbbe5817b8c75a97b4cd6871a64f65f7
+      - uses: OZI-Project/checkpoint@64e790c506ba8df435c545f0d4135fbfde23f6a0
         with:
           python-version: "3.12"
 
   checkpoint-cp313-ubuntu-latest:
     name: checkpoint (Python 3.13 on ubuntu-latest)
     runs-on: ubuntu-latest
     strategy:
@@ -122,15 +122,15 @@
             pypi.org:443
             registry.npmjs.org:443
             objects.githubusercontent.com:443
             fulcio.sigstore.dev:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/checkpoint@0c54a8e9bbbe5817b8c75a97b4cd6871a64f65f7
+      - uses: OZI-Project/checkpoint@64e790c506ba8df435c545f0d4135fbfde23f6a0
         with:
           python-version: "3.13"
 
   checkpoint:
     runs-on: ubuntu-latest
     needs: [checkpoint-cp310-ubuntu-latest, checkpoint-cp311-ubuntu-latest, checkpoint-cp312-ubuntu-latest]
     steps:
@@ -239,10 +239,10 @@
         disable-sudo: true
         egress-policy: block
         allowed-endpoints: >
           api.github.com:443
           upload.pypi.org:443
           uploads.github.com:443
 
-    - uses: OZI-Project/publish@e0a606616e2ff69a1b564f151f1061601683668f
+    - uses: OZI-Project/publish@f5d14bfb29fd5daa0fd3002a9c57f863e86ddf93
       with:
         github-token: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `blastpipe-2024.9.2/.github/workflows/scorecards.yml` & `blastpipe-2024.9.3/.github/workflows/scorecards.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/.gitignore` & `blastpipe-2024.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/CHANGELOG.md` & `blastpipe-2024.9.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,56 @@
 # CHANGELOG
 
 
 
+## v2024.9.3 (2024-05-27)
+
+### :arrow_up:
+
+* :arrow_up: Bump OZI-Project/publish from 0.1.2 to 0.1.3
+
+Bumps [OZI-Project/publish](https://github.com/ozi-project/publish) from 0.1.2 to 0.1.3.
+- [Release notes](https://github.com/ozi-project/publish/releases)
+- [Commits](https://github.com/ozi-project/publish/compare/e0a606616e2ff69a1b564f151f1061601683668f...f5d14bfb29fd5daa0fd3002a9c57f863e86ddf93)
+
+---
+updated-dependencies:
+- dependency-name: OZI-Project/publish
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`6ab4af6`](https://github.com/OZI-Project/blastpipe/commit/6ab4af6d5b34b8e6d54f1930cf6491e7fb413824))
+
+* :arrow_up: Bump OZI-Project/checkpoint from 0.3.1 to 0.4.0
+
+Bumps [OZI-Project/checkpoint](https://github.com/ozi-project/checkpoint) from 0.3.1 to 0.4.0.
+- [Release notes](https://github.com/ozi-project/checkpoint/releases)
+- [Commits](https://github.com/ozi-project/checkpoint/compare/0c54a8e9bbbe5817b8c75a97b4cd6871a64f65f7...64e790c506ba8df435c545f0d4135fbfde23f6a0)
+
+---
+updated-dependencies:
+- dependency-name: OZI-Project/checkpoint
+  dependency-type: direct:production
+  update-type: version-update:semver-minor
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`3dd0525`](https://github.com/OZI-Project/blastpipe/commit/3dd0525e3cac3b53049e6c6768b74883a6fefac0))
+
+### Other
+
+* Merge pull request #96 from OZI-Project/dependabot/github_actions/OZI-Project/checkpoint-0.4.0
+
+⬆️ Bump OZI-Project/checkpoint from 0.3.1 to 0.4.0 ([`00b12b3`](https://github.com/OZI-Project/blastpipe/commit/00b12b3ffe60f11ac4b0f64ad635fc541cdb6b0d))
+
+* Merge pull request #97 from OZI-Project/dependabot/github_actions/OZI-Project/publish-0.1.3
+
+⬆️ Bump OZI-Project/publish from 0.1.2 to 0.1.3 ([`ec9feb8`](https://github.com/OZI-Project/blastpipe/commit/ec9feb8d5b663efd5f3c146b38f431decf015802))
+
+
 ## v2024.9.2 (2024-05-23)
 
 ### :bug:
 
 * :wrench::bug: Add 3.13 support
 
 Signed-off-by: rjdbcm &lt;rjdbcm@outlook.com&gt; ([`42fc53d`](https://github.com/OZI-Project/blastpipe/commit/42fc53d8887b318bfc088d90d051ad4372a96f41))
```

### Comparing `blastpipe-2024.9.2/LICENSE.txt` & `blastpipe-2024.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/NOTICE.md` & `blastpipe-2024.9.3/NOTICE.md`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/PKG-INFO` & `blastpipe-2024.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: blastpipe
-Version: 2024.9.2
+Version: 2024.9.3
 Summary: OZI integrated test library.
 Home-page: https://oziproject.dev
 Author: Eden Ross Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
-Download-URL: https://github.com/OZI-Project/blastpipe/archive/refs/tags/2024.9.2.tar.gz
+Download-URL: https://github.com/OZI-Project/blastpipe/archive/refs/tags/2024.9.3.tar.gz
 Requires-Python: >=3.10, <3.14
 Keywords: ozi,meson
 Provides-Dist: ozi-templates
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `blastpipe-2024.9.2/README.rst` & `blastpipe-2024.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/__init__.py` & `blastpipe-2024.9.3/blastpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/backports.py` & `blastpipe-2024.9.3/blastpipe/backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/backports.pyi` & `blastpipe-2024.9.3/blastpipe/backports.pyi`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/buffer.py` & `blastpipe-2024.9.3/blastpipe/buffer.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/loop.py` & `blastpipe-2024.9.3/blastpipe/loop.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/malloc.py` & `blastpipe-2024.9.3/blastpipe/malloc.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/meson.build` & `blastpipe-2024.9.3/blastpipe/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/mixin.py` & `blastpipe-2024.9.3/blastpipe/mixin.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/README.md.j2` & `blastpipe-2024.9.3/blastpipe/ozi_templates/README.md.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/README.rst.j2` & `blastpipe-2024.9.3/blastpipe/ozi_templates/README.rst.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/__init__.py` & `blastpipe-2024.9.3/blastpipe/ozi_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/__init__.pyi` & `blastpipe-2024.9.3/blastpipe/ozi_templates/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/coverage.pyproject.toml` & `blastpipe-2024.9.3/blastpipe/ozi_templates/coverage.pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/filter.py` & `blastpipe-2024.9.3/blastpipe/ozi_templates/filter.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/filter.pyi` & `blastpipe-2024.9.3/blastpipe/ozi_templates/filter.pyi`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/github_workflows/checkpoint.yml.j2` & `blastpipe-2024.9.3/blastpipe/ozi_templates/github_workflows/checkpoint.yml.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/github_workflows/draft.yml.j2` & `blastpipe-2024.9.3/blastpipe/ozi_templates/github_workflows/draft.yml.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/github_workflows/generate_provenance.yml.j2` & `blastpipe-2024.9.3/blastpipe/ozi_templates/github_workflows/generate_provenance.yml.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/github_workflows/meson.build` & `blastpipe-2024.9.3/blastpipe/ozi_templates/github_workflows/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/github_workflows/ozi.yml.j2` & `blastpipe-2024.9.3/blastpipe/ozi_templates/github_workflows/ozi.yml.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/github_workflows/publish.yml.j2` & `blastpipe-2024.9.3/blastpipe/ozi_templates/github_workflows/publish.yml.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/github_workflows/release.yml.j2` & `blastpipe-2024.9.3/blastpipe/ozi_templates/github_workflows/release.yml.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/cc-by-4.0.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/cc-by-4.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/cc-by-sa-4.0.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/cc-by-sa-4.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/DFSG_approved/meson.build` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/DFSG_approved/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ncsa.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ncsa.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/0bsd.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/0bsd.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/OSI_Approved/meson.build` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/OSI_Approved/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/Public_Domain/unlicense.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/Public_Domain/unlicense.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/agpl-3.0.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/apache-2.0.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/artistic-2.0.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/artistic-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/bsd-3-clause.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/bsd-3-clause.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/cc0-1.0.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/cc0-1.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/epl-1.0.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/epl-1.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/gfdl-1.3.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/gfdl-1.3.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/gpl-2.0.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/gpl-3.0.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/gpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/isc.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/isc.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/lgpl-2.0.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/lgpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/lgpl-2.1.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/lgpl-2.1.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/lgpl-3.0.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/lgpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/meson.build` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/mit.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/mit.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/license/zlib.txt` & `blastpipe-2024.9.3/blastpipe/ozi_templates/license/zlib.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/meson.build` & `blastpipe-2024.9.3/blastpipe/ozi_templates/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/meson.options.j2` & `blastpipe-2024.9.3/blastpipe/ozi_templates/meson.options.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/new_child.j2` & `blastpipe-2024.9.3/blastpipe/ozi_templates/new_child.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/project.PKG-INFO` & `blastpipe-2024.9.3/blastpipe/ozi_templates/project.PKG-INFO`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/project.array.meson.options` & `blastpipe-2024.9.3/blastpipe/ozi_templates/project.array.meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/project.feature.meson.options` & `blastpipe-2024.9.3/blastpipe/ozi_templates/project.feature.meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/project.integer.meson.options` & `blastpipe-2024.9.3/blastpipe/ozi_templates/project.integer.meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/project.meson.build` & `blastpipe-2024.9.3/blastpipe/ozi_templates/project.meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/project.name/meson.build.j2` & `blastpipe-2024.9.3/blastpipe/ozi_templates/project.name/meson.build.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/pyproject.toml.j2` & `blastpipe-2024.9.3/blastpipe/ozi_templates/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/root.pyproject.toml` & `blastpipe-2024.9.3/blastpipe/ozi_templates/root.pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/ruff.pyproject.toml` & `blastpipe-2024.9.3/blastpipe/ozi_templates/ruff.pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/semantic_release.pyproject.toml` & `blastpipe-2024.9.3/blastpipe/ozi_templates/semantic_release.pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/tests/meson.build.j2` & `blastpipe-2024.9.3/blastpipe/ozi_templates/tests/meson.build.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/ozi_templates/tox.pyproject.toml` & `blastpipe-2024.9.3/blastpipe/ozi_templates/tox.pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/sequence.py` & `blastpipe-2024.9.3/blastpipe/sequence.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/blastpipe/tailcall.py` & `blastpipe-2024.9.3/blastpipe/tailcall.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/meson.build` & `blastpipe-2024.9.3/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/meson.options` & `blastpipe-2024.9.3/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/pyproject.toml` & `blastpipe-2024.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/subprojects/docs/LICENSE.txt` & `blastpipe-2024.9.3/subprojects/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/subprojects/docs/_static/css/custom.css` & `blastpipe-2024.9.3/subprojects/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/subprojects/docs/_static/css/meson.build` & `blastpipe-2024.9.3/subprojects/docs/_static/css/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/subprojects/docs/_static/meson.build` & `blastpipe-2024.9.3/subprojects/docs/_static/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/subprojects/docs/_templates/layout.html` & `blastpipe-2024.9.3/subprojects/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/subprojects/docs/_templates/meson.build` & `blastpipe-2024.9.3/subprojects/docs/_templates/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/subprojects/docs/conf.cfg` & `blastpipe-2024.9.3/subprojects/docs/conf.cfg`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/subprojects/docs/index.rst` & `blastpipe-2024.9.3/subprojects/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/subprojects/docs/meson.build` & `blastpipe-2024.9.3/subprojects/docs/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/subprojects/docs/meson.options` & `blastpipe-2024.9.3/subprojects/docs/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/tests/meson.build` & `blastpipe-2024.9.3/tests/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/tests/test_backports.py` & `blastpipe-2024.9.3/tests/test_backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/tests/test_filter.py` & `blastpipe-2024.9.3/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/tests/test_fuzz.py` & `blastpipe-2024.9.3/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.9.2/tests/test_tailcall.py` & `blastpipe-2024.9.3/tests/test_tailcall.py`

 * *Files identical despite different names*

