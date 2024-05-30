# Comparing `tmp/anitya-1.8.1.tar.gz` & `tmp/anitya-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anitya-1.8.1.tar", max compression
+gzip compressed data, was "anitya-1.9.0.tar", max compression
```

## Comparing `anitya-1.8.1.tar` & `anitya-1.9.0.tar`

### file list

```diff
@@ -1,2085 +1,189 @@
--rw-r--r--   0        0        0    18002 2020-12-02 09:02:04.975902 anitya-1.8.1/LICENSE
--rw-r--r--   0        0        0     2016 2023-05-26 06:47:55.369117 anitya-1.8.1/README.rst
--rw-r--r--   0        0        0     1184 2020-12-02 09:02:04.975902 anitya-1.8.1/alembic.ini
--rw-r--r--   0        0        0      147 2023-05-26 06:47:55.369117 anitya-1.8.1/anitya/__init__.py
--rw-r--r--   0        0        0    18625 2023-05-26 06:47:55.376117 anitya-1.8.1/anitya/admin.py
--rw-r--r--   0        0        0    15352 2023-05-26 06:47:55.376117 anitya-1.8.1/anitya/api.py
--rw-r--r--   0        0        0    31952 2023-05-26 06:47:55.376117 anitya-1.8.1/anitya/api_v2.py
--rw-r--r--   0        0        0     7664 2023-05-26 06:47:55.376117 anitya-1.8.1/anitya/app.py
--rw-r--r--   0        0        0     4449 2023-05-26 06:47:55.376117 anitya-1.8.1/anitya/authentication.py
--rw-r--r--   0        0        0    11974 2023-05-26 06:47:55.376117 anitya-1.8.1/anitya/check_service.py
--rw-r--r--   0        0        0     1112 2023-05-26 06:47:55.377117 anitya-1.8.1/anitya/compat.py
--rw-r--r--   0        0        0     5893 2023-05-26 06:47:55.377117 anitya-1.8.1/anitya/config.py
--rw-r--r--   0        0        0     1396 2023-05-26 06:47:55.377117 anitya-1.8.1/anitya/db/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-26 06:47:55.377117 anitya-1.8.1/anitya/db/events.py
--rw-r--r--   0        0        0     5802 2023-05-26 06:47:55.377117 anitya-1.8.1/anitya/db/meta.py
--rw-r--r--   0        0        0      464 2020-12-02 09:02:04.976902 anitya-1.8.1/anitya/db/migrations/README.md
--rw-r--r--   0        0        0        0 2020-12-02 09:02:04.976902 anitya-1.8.1/anitya/db/migrations/__init__.py
--rw-r--r--   0        0        0     2105 2023-05-26 06:47:55.377117 anitya-1.8.1/anitya/db/migrations/env.py
--rw-r--r--   0        0        0      413 2020-12-02 09:02:04.976902 anitya-1.8.1/anitya/db/migrations/script.py.mako
--rw-r--r--   0        0        0      657 2023-05-26 06:47:55.377117 anitya-1.8.1/anitya/db/migrations/versions/136d119ab015_rename_project_latest_known_cursor_to_.py
--rw-r--r--   0        0        0      541 2023-05-26 06:47:55.377117 anitya-1.8.1/anitya/db/migrations/versions/16aa7da2764c_add_projectversion_commit_url.py
--rw-r--r--   0        0        0      591 2023-05-26 06:47:55.377117 anitya-1.8.1/anitya/db/migrations/versions/1ab95561edae_convert_date_to_rpm.py
--rw-r--r--   0        0        0     1390 2023-05-26 06:47:55.377117 anitya-1.8.1/anitya/db/migrations/versions/1bf8aead6179_add_check_times.py
--rw-r--r--   0        0        0      662 2023-05-26 06:47:55.377117 anitya-1.8.1/anitya/db/migrations/versions/1f839c54e428_add_archive_flag.py
--rw-r--r--   0        0        0      634 2023-05-26 06:47:55.377117 anitya-1.8.1/anitya/db/migrations/versions/24b6734e8565_creation_date_on_version.py
--rw-r--r--   0        0        0      746 2023-05-26 06:47:55.377117 anitya-1.8.1/anitya/db/migrations/versions/27342bce1d0f_populate_project_version_scheme.py
--rw-r--r--   0        0        0      591 2023-05-26 06:47:55.378117 anitya-1.8.1/anitya/db/migrations/versions/2925648d8cc3_add_a_version_prefix_field.py
--rw-r--r--   0        0        0      556 2023-05-26 06:47:55.378117 anitya-1.8.1/anitya/db/migrations/versions/2d1aa7ff82a5_remove_code_google_backend.py
--rw-r--r--   0        0        0      802 2023-05-26 06:47:55.378117 anitya-1.8.1/anitya/db/migrations/versions/314651690dc7_add_error_counter_to_project.py
--rw-r--r--   0        0        0     1809 2023-05-26 06:47:55.378117 anitya-1.8.1/anitya/db/migrations/versions/34b9bb5fa388_make_ecosystem_non_nullable.py
--rw-r--r--   0        0        0     3721 2023-05-26 06:47:55.378117 anitya-1.8.1/anitya/db/migrations/versions/3fae8239eeec_add_an_api_token_table.py
--rw-r--r--   0        0        0      881 2023-05-26 06:47:55.378117 anitya-1.8.1/anitya/db/migrations/versions/540bdcf7edbc_convert_github_url_to_owner_project.py
--rw-r--r--   0        0        0      676 2023-05-26 06:47:55.378117 anitya-1.8.1/anitya/db/migrations/versions/571bd07533a9_add_insecure_column_to_projects_table.py
--rw-r--r--   0        0        0      589 2023-05-26 06:47:55.378117 anitya-1.8.1/anitya/db/migrations/versions/5b8b587d7dbe_add_version_filter_column.py
--rw-r--r--   0        0        0      694 2023-05-26 06:47:55.378117 anitya-1.8.1/anitya/db/migrations/versions/5e209766aead_add_release_check_to_project.py
--rw-r--r--   0        0        0     1737 2023-05-26 06:47:55.378117 anitya-1.8.1/anitya/db/migrations/versions/6ac0e42df937_drop_logs_table.py
--rw-r--r--   0        0        0      556 2023-05-26 06:47:55.378117 anitya-1.8.1/anitya/db/migrations/versions/708f6f26b4b6_add_version_pattern.py
--rw-r--r--   0        0        0     1022 2023-05-26 06:47:55.378117 anitya-1.8.1/anitya/db/migrations/versions/7a8c4aa92678_add_missing_github_owner_project_pairs.py
--rw-r--r--   0        0        0      610 2023-05-26 06:47:55.378117 anitya-1.8.1/anitya/db/migrations/versions/8040ef9a9dda_add_a_version_scheme_column_to_projects.py
--rw-r--r--   0        0        0      683 2023-05-26 06:47:55.378117 anitya-1.8.1/anitya/db/migrations/versions/8be6e153962c_remove_cursor.py
--rw-r--r--   0        0        0      970 2023-05-26 06:47:55.378117 anitya-1.8.1/anitya/db/migrations/versions/921c612ba0da_model_upstream_ecosystems.py
--rw-r--r--   0        0        0      543 2023-05-26 06:47:55.379117 anitya-1.8.1/anitya/db/migrations/versions/92a2e9eba0a7_add_project_latest_known_cursor.py
--rw-r--r--   0        0        0      928 2020-12-02 09:02:04.977902 anitya-1.8.1/anitya/db/migrations/versions/9c29da0af3af_populate_ecosystem_data.py
--rw-r--r--   0        0        0        0 2020-12-02 09:02:04.977902 anitya-1.8.1/anitya/db/migrations/versions/__init__.py
--rw-r--r--   0        0        0     3125 2023-05-26 06:47:55.379117 anitya-1.8.1/anitya/db/migrations/versions/a52d2fe99d4f_users.py
--rw-r--r--   0        0        0      301 2020-12-02 09:02:04.977902 anitya-1.8.1/anitya/db/migrations/versions/ac10bf3f974c_.py
--rw-r--r--   0        0        0      494 2023-05-26 06:47:55.379117 anitya-1.8.1/anitya/db/migrations/versions/b13662e5d288_add_admin_flag.py
--rw-r--r--   0        0        0     2881 2023-05-26 06:47:55.379117 anitya-1.8.1/anitya/db/migrations/versions/b9201d816075_remove_the_backends_and_ecosystems_.py
--rw-r--r--   0        0        0      408 2023-05-26 06:47:55.379117 anitya-1.8.1/anitya/db/migrations/versions/c8735fa14a0a_add_cascade_delete.py
--rw-r--r--   0        0        0      595 2023-05-26 06:47:55.379117 anitya-1.8.1/anitya/db/migrations/versions/d6170cfc2814_add_pre_release_flag.py
--rw-r--r--   0        0        0     1147 2023-05-26 06:47:55.379117 anitya-1.8.1/anitya/db/migrations/versions/e34988f3e2f4_add_statistics_to_run.py
--rw-r--r--   0        0        0     6581 2023-05-26 06:47:55.379117 anitya-1.8.1/anitya/db/migrations/versions/feeaa70ead67_social_authentication_table.py
--rw-r--r--   0        0        0    35192 2023-05-26 06:47:55.379117 anitya-1.8.1/anitya/db/models.py
--rw-r--r--   0        0        0     3488 2023-05-26 06:47:55.379117 anitya-1.8.1/anitya/forms.py
--rw-r--r--   0        0        0      152 2020-12-02 09:02:04.977902 anitya-1.8.1/anitya/lib/__init__.py
--rw-r--r--   0        0        0    15819 2023-05-26 06:47:55.380118 anitya-1.8.1/anitya/lib/backends/__init__.py
--rw-r--r--   0        0        0     2494 2023-05-26 06:47:55.380118 anitya-1.8.1/anitya/lib/backends/bitbucket.py
--rw-r--r--   0        0        0     2580 2023-05-26 06:47:55.380118 anitya-1.8.1/anitya/lib/backends/cgit.py
--rw-r--r--   0        0        0     3059 2023-05-26 06:47:55.380118 anitya-1.8.1/anitya/lib/backends/cpan.py
--rw-r--r--   0        0        0     7766 2020-12-16 13:18:27.989536 anitya-1.8.1/anitya/lib/backends/cran.py
--rw-r--r--   0        0        0     8182 2022-06-22 14:20:39.936825 anitya-1.8.1/anitya/lib/backends/crates.py
--rw-r--r--   0        0        0     2345 2023-05-26 06:47:55.380118 anitya-1.8.1/anitya/lib/backends/custom.py
--rw-r--r--   0        0        0     2459 2023-05-26 06:47:55.380118 anitya-1.8.1/anitya/lib/backends/debian.py
--rw-r--r--   0        0        0     2699 2023-05-26 06:47:55.380118 anitya-1.8.1/anitya/lib/backends/drupal6.py
--rw-r--r--   0        0        0     2699 2023-05-26 06:47:55.380118 anitya-1.8.1/anitya/lib/backends/drupal7.py
--rw-r--r--   0        0        0     2738 2023-05-26 06:47:55.381117 anitya-1.8.1/anitya/lib/backends/folder.py
--rw-r--r--   0        0        0     1946 2023-05-26 06:47:55.381117 anitya-1.8.1/anitya/lib/backends/freshmeat.py
--rw-r--r--   0        0        0     9389 2023-05-26 06:47:55.381117 anitya-1.8.1/anitya/lib/backends/github.py
--rw-r--r--   0        0        0     4313 2023-05-26 06:47:55.381117 anitya-1.8.1/anitya/lib/backends/gitlab.py
--rw-r--r--   0        0        0     3088 2023-05-26 06:47:55.381117 anitya-1.8.1/anitya/lib/backends/gnome.py
--rw-r--r--   0        0        0     2646 2023-05-26 06:47:55.381117 anitya-1.8.1/anitya/lib/backends/gnu.py
--rw-r--r--   0        0        0     2992 2023-05-26 06:47:55.381117 anitya-1.8.1/anitya/lib/backends/gogs.py
--rw-r--r--   0        0        0     2237 2023-05-26 06:47:55.381117 anitya-1.8.1/anitya/lib/backends/hackage.py
--rw-r--r--   0        0        0     1869 2023-05-26 06:47:55.381117 anitya-1.8.1/anitya/lib/backends/launchpad.py
--rw-r--r--   0        0        0     2630 2023-05-26 06:47:55.381117 anitya-1.8.1/anitya/lib/backends/maven.py
--rw-r--r--   0        0        0     5116 2020-12-16 13:18:27.990536 anitya-1.8.1/anitya/lib/backends/npmjs.py
--rw-r--r--   0        0        0     3263 2022-12-14 14:15:40.090732 anitya-1.8.1/anitya/lib/backends/packagist.py
--rw-r--r--   0        0        0     3122 2023-05-26 06:47:55.382117 anitya-1.8.1/anitya/lib/backends/pagure.py
--rw-r--r--   0        0        0     4417 2023-05-26 06:47:55.382117 anitya-1.8.1/anitya/lib/backends/pear.py
--rw-r--r--   0        0        0     4406 2023-05-26 06:47:55.382117 anitya-1.8.1/anitya/lib/backends/pecl.py
--rw-r--r--   0        0        0     5058 2023-05-26 06:47:55.382117 anitya-1.8.1/anitya/lib/backends/pypi.py
--rw-r--r--   0        0        0     3465 2022-12-14 14:15:40.091732 anitya-1.8.1/anitya/lib/backends/rubygems.py
--rw-r--r--   0        0        0     2066 2023-05-26 06:47:55.382117 anitya-1.8.1/anitya/lib/backends/sourceforge.py
--rw-r--r--   0        0        0     4289 2023-05-26 06:47:55.382117 anitya-1.8.1/anitya/lib/backends/sourceforge_git.py
--rw-r--r--   0        0        0     3524 2023-05-26 06:47:55.382117 anitya-1.8.1/anitya/lib/backends/sourcehut.py
--rw-r--r--   0        0        0     2030 2022-12-14 14:15:40.093732 anitya-1.8.1/anitya/lib/backends/stackage.py
--rw-r--r--   0        0        0     1087 2023-05-26 06:47:55.382117 anitya-1.8.1/anitya/lib/ecosystems/__init__.py
--rw-r--r--   0        0        0     1072 2022-06-22 14:20:39.939825 anitya-1.8.1/anitya/lib/ecosystems/crates.py
--rw-r--r--   0        0        0      278 2022-06-22 14:20:39.939825 anitya-1.8.1/anitya/lib/ecosystems/maven.py
--rw-r--r--   0        0        0      264 2022-06-22 14:20:39.939825 anitya-1.8.1/anitya/lib/ecosystems/npm.py
--rw-r--r--   0        0        0      266 2022-06-22 14:20:39.939825 anitya-1.8.1/anitya/lib/ecosystems/pypi.py
--rw-r--r--   0        0        0      282 2022-06-22 14:20:39.939825 anitya-1.8.1/anitya/lib/ecosystems/rubygems.py
--rw-r--r--   0        0        0     4084 2022-06-22 14:20:39.940825 anitya-1.8.1/anitya/lib/exceptions.py
--rw-r--r--   0        0        0     3430 2022-06-22 14:20:39.940825 anitya-1.8.1/anitya/lib/plugins.py
--rw-r--r--   0        0        0    18437 2023-05-26 06:47:55.382117 anitya-1.8.1/anitya/lib/utilities.py
--rw-r--r--   0        0        0     2185 2023-05-26 06:47:55.382117 anitya-1.8.1/anitya/lib/versions/__init__.py
--rw-r--r--   0        0        0     7345 2023-05-26 06:47:55.383118 anitya-1.8.1/anitya/lib/versions/base.py
--rw-r--r--   0        0        0    15319 2022-06-22 14:20:39.941825 anitya-1.8.1/anitya/lib/versions/calver.py
--rw-r--r--   0        0        0     6418 2023-05-26 06:47:55.383118 anitya-1.8.1/anitya/lib/versions/python.py
--rw-r--r--   0        0        0     7546 2023-05-26 06:47:55.383118 anitya-1.8.1/anitya/lib/versions/rpm.py
--rw-r--r--   0        0        0     3766 2020-12-02 09:04:10.567083 anitya-1.8.1/anitya/lib/versions/semver.py
--rw-r--r--   0        0        0     2822 2023-05-26 06:47:55.383118 anitya-1.8.1/anitya/lib/xml2dict.py
--rw-r--r--   0        0        0     7366 2023-05-26 06:47:55.383118 anitya-1.8.1/anitya/librariesio_consumer.py
--rw-r--r--   0        0        0     6250 2023-05-26 06:47:55.383118 anitya-1.8.1/anitya/mail_logging.py
--rw-r--r--   0        0        0     2946 2023-05-26 06:47:55.383118 anitya-1.8.1/anitya/sar.py
--rw-r--r--   0        0        0       54 2022-11-14 14:56:56.902921 anitya-1.8.1/anitya/static/css/avatars.css
--rw-r--r--   0        0        0      888 2022-11-14 14:57:00.636935 anitya-1.8.1/anitya/static/css/cnucnu.css
--rw-r--r--   0        0        0    24734 2022-11-14 14:57:06.871959 anitya-1.8.1/anitya/static/css/fonts/Cantarell-Bold-webfont.eot
--rw-r--r--   0        0        0    28113 2022-11-14 14:57:06.871959 anitya-1.8.1/anitya/static/css/fonts/Cantarell-Bold-webfont.svg
--rw-r--r--   0        0        0    49276 2022-11-14 14:57:06.872959 anitya-1.8.1/anitya/static/css/fonts/Cantarell-Bold-webfont.ttf
--rw-r--r--   0        0        0    16708 2022-11-14 14:57:06.872959 anitya-1.8.1/anitya/static/css/fonts/Cantarell-Bold-webfont.woff
--rw-r--r--   0        0        0    27450 2022-11-14 14:57:06.872959 anitya-1.8.1/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.eot
--rw-r--r--   0        0        0    29130 2022-11-14 14:57:06.873959 anitya-1.8.1/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.svg
--rw-r--r--   0        0        0    52200 2022-11-14 14:57:06.873959 anitya-1.8.1/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.ttf
--rw-r--r--   0        0        0    17988 2022-11-14 14:57:06.873959 anitya-1.8.1/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.woff
--rw-r--r--   0        0        0    27610 2022-11-14 14:57:06.873959 anitya-1.8.1/anitya/static/css/fonts/Cantarell-Oblique-webfont.eot
--rw-r--r--   0        0        0    29402 2022-11-14 14:57:06.874959 anitya-1.8.1/anitya/static/css/fonts/Cantarell-Oblique-webfont.svg
--rw-r--r--   0        0        0    50068 2022-11-14 14:57:06.874959 anitya-1.8.1/anitya/static/css/fonts/Cantarell-Oblique-webfont.ttf
--rw-r--r--   0        0        0    17980 2022-11-14 14:57:06.874959 anitya-1.8.1/anitya/static/css/fonts/Cantarell-Oblique-webfont.woff
--rw-r--r--   0        0        0    24350 2022-11-14 14:57:06.874959 anitya-1.8.1/anitya/static/css/fonts/Cantarell-Regular-webfont.eot
--rw-r--r--   0        0        0    28095 2022-11-14 14:57:06.874959 anitya-1.8.1/anitya/static/css/fonts/Cantarell-Regular-webfont.svg
--rw-r--r--   0        0        0    47504 2022-11-14 14:57:06.875959 anitya-1.8.1/anitya/static/css/fonts/Cantarell-Regular-webfont.ttf
--rw-r--r--   0        0        0    16400 2022-11-14 14:57:06.875959 anitya-1.8.1/anitya/static/css/fonts/Cantarell-Regular-webfont.woff
--rw-r--r--   0        0        0    94588 2022-11-14 14:57:06.876959 anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Bold-webfont.eot
--rw-r--r--   0        0        0   171329 2022-11-14 14:57:06.876959 anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Bold-webfont.svg
--rw-r--r--   0        0        0   170608 2022-11-14 14:57:06.878960 anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Bold-webfont.ttf
--rw-r--r--   0        0        0    56608 2022-11-14 14:57:06.878960 anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Bold-webfont.woff
--rw-r--r--   0        0        0    91164 2022-11-14 14:57:06.878960 anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Regular-webfont.eot
--rw-r--r--   0        0        0   169419 2022-11-14 14:57:06.879959 anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Regular-webfont.svg
--rw-r--r--   0        0        0   170388 2022-11-14 14:57:06.880959 anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Regular-webfont.ttf
--rw-r--r--   0        0        0    54684 2022-11-14 14:57:06.880959 anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Regular-webfont.woff
--rw-r--r--   0        0        0    95020 2022-11-14 14:57:06.881960 anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Thin-webfont.eot
--rw-r--r--   0        0        0   167898 2022-11-14 14:57:06.882959 anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Thin-webfont.svg
--rw-r--r--   0        0        0   170308 2022-11-14 14:57:06.883959 anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Thin-webfont.ttf
--rw-r--r--   0        0        0    56100 2022-11-14 14:57:06.883959 anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Thin-webfont.woff
--rw-r--r--   0        0        0      279 2022-11-14 14:57:22.414019 anitya-1.8.1/anitya/static/css/footer.css
--rw-r--r--   0        0        0      212 2022-11-14 14:57:16.686997 anitya-1.8.1/anitya/static/css/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-r--r--   0        0        0      220 2022-11-14 14:57:16.686997 anitya-1.8.1/anitya/static/css/images/ui-bg_flat_0_eeeeee_40x100.png
--rw-r--r--   0        0        0      208 2022-11-14 14:57:16.686997 anitya-1.8.1/anitya/static/css/images/ui-bg_flat_55_ffffff_40x100.png
--rw-r--r--   0        0        0      208 2022-11-14 14:57:16.686997 anitya-1.8.1/anitya/static/css/images/ui-bg_flat_75_ffffff_40x100.png
--rw-r--r--   0        0        0      207 2022-11-14 14:57:16.686997 anitya-1.8.1/anitya/static/css/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0        0        0      277 2022-11-14 14:57:16.686997 anitya-1.8.1/anitya/static/css/images/ui-bg_highlight-soft_100_f6f6f6_1x100.png
--rw-r--r--   0        0        0      338 2022-11-14 14:57:16.687997 anitya-1.8.1/anitya/static/css/images/ui-bg_highlight-soft_25_0073ea_1x100.png
--rw-r--r--   0        0        0      280 2022-11-14 14:57:16.687997 anitya-1.8.1/anitya/static/css/images/ui-bg_highlight-soft_50_dddddd_1x100.png
--rw-r--r--   0        0        0     4549 2022-11-14 14:57:16.687997 anitya-1.8.1/anitya/static/css/images/ui-icons_0073ea_256x240.png
--rw-r--r--   0        0        0     6992 2022-11-14 14:57:16.687997 anitya-1.8.1/anitya/static/css/images/ui-icons_454545_256x240.png
--rw-r--r--   0        0        0     6988 2022-11-14 14:57:16.688997 anitya-1.8.1/anitya/static/css/images/ui-icons_666666_256x240.png
--rw-r--r--   0        0        0     4549 2022-11-14 14:57:16.688997 anitya-1.8.1/anitya/static/css/images/ui-icons_ff0084_256x240.png
--rw-r--r--   0        0        0     6299 2022-11-14 14:57:16.688997 anitya-1.8.1/anitya/static/css/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0      125 2022-11-14 14:57:29.052045 anitya-1.8.1/anitya/static/css/navbar.css
--rw-r--r--   0        0        0     2519 2022-11-14 14:57:32.802060 anitya-1.8.1/anitya/static/css/text.css
--rw-r--r--   0        0        0    33392 2021-01-15 12:47:19.805568 anitya-1.8.1/anitya/static/docs/_images/database.png
--rw-r--r--   0        0        0    13224 2021-01-15 12:47:19.813568 anitya-1.8.1/anitya/static/docs/_modules/anitya/db/events.html
--rw-r--r--   0        0        0    20589 2021-01-15 12:47:19.814568 anitya-1.8.1/anitya/static/docs/_modules/anitya/db/meta.html
--rw-r--r--   0        0        0   150267 2021-01-15 12:47:19.816568 anitya-1.8.1/anitya/static/docs/_modules/anitya/db/models.html
--rw-r--r--   0        0        0    52067 2021-01-15 12:47:19.818568 anitya-1.8.1/anitya/static/docs/_modules/anitya/lib/backends.html
--rw-r--r--   0        0        0     6469 2021-01-15 12:47:19.819568 anitya-1.8.1/anitya/static/docs/_modules/anitya/lib/ecosystems.html
--rw-r--r--   0        0        0    18072 2021-01-15 12:47:19.821568 anitya-1.8.1/anitya/static/docs/_modules/anitya/lib/exceptions.html
--rw-r--r--   0        0        0    15350 2021-01-15 12:47:19.822568 anitya-1.8.1/anitya/static/docs/_modules/anitya/lib/plugins.html
--rw-r--r--   0        0        0    26768 2021-01-15 12:47:19.824568 anitya-1.8.1/anitya/static/docs/_modules/anitya/lib/versions/base.html
--rw-r--r--   0        0        0     5081 2021-01-15 12:47:19.841568 anitya-1.8.1/anitya/static/docs/_modules/index.html
--rw-r--r--   0        0        0    76032 2021-01-15 12:47:19.827568 anitya-1.8.1/anitya/static/docs/_modules/sqlalchemy/ext/declarative/api.html
--rw-r--r--   0        0        0   245360 2021-01-15 12:47:19.830568 anitya-1.8.1/anitya/static/docs/_modules/sqlalchemy/orm/attributes.html
--rw-r--r--   0        0        0    23324 2021-01-15 12:47:19.832568 anitya-1.8.1/anitya/static/docs/_modules/sqlalchemy/orm/scoping.html
--rw-r--r--   0        0        0   500489 2021-01-15 12:47:19.837568 anitya-1.8.1/anitya/static/docs/_modules/sqlalchemy/sql/schema.html
--rw-r--r--   0        0        0   296008 2021-01-15 12:47:19.840568 anitya-1.8.1/anitya/static/docs/_modules/sqlalchemy/sql/sqltypes.html
--rw-r--r--   0        0        0     5095 2021-01-15 12:47:19.850568 anitya-1.8.1/anitya/static/docs/_sources/admin-guide.rst.txt
--rw-r--r--   0        0        0     8467 2021-01-15 12:47:19.851568 anitya-1.8.1/anitya/static/docs/_sources/admin-user-guide.rst.txt
--rw-r--r--   0        0        0     1756 2021-01-15 12:47:19.852568 anitya-1.8.1/anitya/static/docs/_sources/api.rst.txt
--rw-r--r--   0        0        0     9534 2021-01-15 12:47:19.853568 anitya-1.8.1/anitya/static/docs/_sources/contributing.rst.txt
--rw-r--r--   0        0        0      314 2021-01-15 12:47:19.854568 anitya-1.8.1/anitya/static/docs/_sources/database.rst.txt
--rw-r--r--   0        0        0      306 2021-01-15 12:47:19.856568 anitya-1.8.1/anitya/static/docs/_sources/docblocks/anitya.db.models.rst.txt
--rw-r--r--   0        0        0      510 2021-01-15 12:47:19.857568 anitya-1.8.1/anitya/static/docs/_sources/glossary.rst.txt
--rw-r--r--   0        0        0     1279 2021-01-15 12:47:19.858568 anitya-1.8.1/anitya/static/docs/_sources/index.rst.txt
--rw-r--r--   0        0        0     2624 2021-01-15 12:47:19.859568 anitya-1.8.1/anitya/static/docs/_sources/integrating-with-anitya.rst.txt
--rw-r--r--   0        0        0     2229 2020-12-02 12:47:56.984892 anitya-1.8.1/anitya/static/docs/_sources/release-monitoring-admin-guide.rst.txt
--rw-r--r--   0        0        0    23367 2021-01-15 12:47:19.860568 anitya-1.8.1/anitya/static/docs/_sources/release-notes.rst.txt
--rw-r--r--   0        0        0    19248 2021-01-15 12:47:19.861568 anitya-1.8.1/anitya/static/docs/_sources/user-guide.rst.txt
--rw-r--r--   0        0        0    11187 2021-01-15 12:47:19.881568 anitya-1.8.1/anitya/static/docs/_static/alabaster.css
--rw-r--r--   0        0        0    12171 2021-01-15 12:47:19.864568 anitya-1.8.1/anitya/static/docs/_static/basic.css
--rw-r--r--   0        0        0       42 2021-01-15 12:47:19.880568 anitya-1.8.1/anitya/static/docs/_static/custom.css
--rw-r--r--   0        0        0     9270 2021-01-15 12:47:19.874568 anitya-1.8.1/anitya/static/docs/_static/doctools.js
--rw-r--r--   0        0        0      307 2021-01-15 12:47:19.873568 anitya-1.8.1/anitya/static/docs/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2021-01-15 12:47:19.866568 anitya-1.8.1/anitya/static/docs/_static/file.png
--rw-r--r--   0        0        0   280364 2021-01-15 12:47:19.884568 anitya-1.8.1/anitya/static/docs/_static/jquery-3.4.1.js
--rw-r--r--   0        0        0   287630 2021-01-15 12:47:19.871568 anitya-1.8.1/anitya/static/docs/_static/jquery-3.5.1.js
--rw-r--r--   0        0        0    88145 2021-01-15 12:47:19.868568 anitya-1.8.1/anitya/static/docs/_static/jquery.js
--rw-r--r--   0        0        0    10847 2021-01-15 12:47:19.879568 anitya-1.8.1/anitya/static/docs/_static/language_data.js
--rw-r--r--   0        0        0       90 2021-01-15 12:47:19.878568 anitya-1.8.1/anitya/static/docs/_static/minus.png
--rw-r--r--   0        0        0       90 2021-01-15 12:47:19.877568 anitya-1.8.1/anitya/static/docs/_static/plus.png
--rw-r--r--   0        0        0     4395 2021-01-15 12:47:19.863568 anitya-1.8.1/anitya/static/docs/_static/pygments.css
--rw-r--r--   0        0        0    15987 2021-01-15 12:47:19.875568 anitya-1.8.1/anitya/static/docs/_static/searchtools.js
--rw-r--r--   0        0        0    35168 2021-01-15 12:47:19.876568 anitya-1.8.1/anitya/static/docs/_static/underscore-1.3.1.js
--rw-r--r--   0        0        0    12140 2021-01-15 12:47:19.865568 anitya-1.8.1/anitya/static/docs/_static/underscore.js
--rw-r--r--   0        0        0    17984 2021-01-15 12:47:19.782568 anitya-1.8.1/anitya/static/docs/admin-guide.html
--rw-r--r--   0        0        0    19172 2021-01-15 12:47:19.785568 anitya-1.8.1/anitya/static/docs/admin-user-guide.html
--rw-r--r--   0        0        0   186318 2021-01-15 12:47:19.790568 anitya-1.8.1/anitya/static/docs/api.html
--rw-r--r--   0        0        0    24463 2021-01-15 12:47:19.792568 anitya-1.8.1/anitya/static/docs/contributing.html
--rw-r--r--   0        0        0     5793 2021-01-15 12:47:19.794568 anitya-1.8.1/anitya/static/docs/database.html
--rw-r--r--   0        0        0     6755 2021-01-15 12:47:19.797568 anitya-1.8.1/anitya/static/docs/docblocks/anitya.db.models.html
--rw-r--r--   0        0        0    21157 2021-01-15 12:47:19.799568 anitya-1.8.1/anitya/static/docs/genindex.html
--rw-r--r--   0        0        0     5045 2021-01-15 12:47:19.801568 anitya-1.8.1/anitya/static/docs/glossary.html
--rw-r--r--   0        0        0     9045 2021-01-15 12:47:19.803568 anitya-1.8.1/anitya/static/docs/http-routingtable.html
--rw-r--r--   0        0        0    13545 2021-01-15 12:47:19.807568 anitya-1.8.1/anitya/static/docs/index.html
--rw-r--r--   0        0        0     8658 2021-01-15 12:47:19.809568 anitya-1.8.1/anitya/static/docs/integrating-with-anitya.html
--rw-r--r--   0        0        0     1672 2021-01-15 12:47:19.842568 anitya-1.8.1/anitya/static/docs/objects.inv
--rw-r--r--   0        0        0     6028 2021-01-15 12:47:19.844568 anitya-1.8.1/anitya/static/docs/py-modindex.html
--rw-r--r--   0        0        0     8309 2020-12-02 12:47:56.964892 anitya-1.8.1/anitya/static/docs/release-monitoring-admin-guide.html
--rw-r--r--   0        0        0    48756 2021-01-15 12:47:19.846568 anitya-1.8.1/anitya/static/docs/release-notes.html
--rw-r--r--   0        0        0     4548 2021-01-15 12:47:19.847568 anitya-1.8.1/anitya/static/docs/search.html
--rw-r--r--   0        0        0    24161 2021-01-15 12:47:19.848568 anitya-1.8.1/anitya/static/docs/searchindex.js
--rw-r--r--   0        0        0    38361 2021-01-15 12:47:19.885568 anitya-1.8.1/anitya/static/docs/user-guide.html
--rw-r--r--   0        0        0     4683 2020-12-02 09:02:04.991902 anitya-1.8.1/anitya/static/google_logo.png
--rw-r--r--   0        0        0     5430 2022-11-14 16:27:56.526971 anitya-1.8.1/anitya/static/ico/favicon.ico
--rw-r--r--   0        0        0     4077 2022-11-14 14:58:19.913241 anitya-1.8.1/anitya/static/img/spinner.gif
--rw-r--r--   0        0        0     1957 2023-04-26 13:29:52.891981 anitya-1.8.1/anitya/static/node_modules/.package-lock.json
--rw-r--r--   0        0        0     1082 2022-11-14 15:08:03.408809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/LICENSE.md
--rw-r--r--   0        0        0    13561 2022-11-14 15:08:03.409809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/README.md
--rw-r--r--   0        0        0     2037 2022-11-14 15:08:03.426809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/cjs/enums.js
--rw-r--r--   0        0        0       45 2022-11-14 15:08:03.426809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/cjs/enums.js.flow
--rw-r--r--   0        0        0     4234 2022-11-14 15:08:03.427809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/cjs/enums.js.map
--rw-r--r--   0        0        0    36698 2022-11-14 15:08:03.428809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-base.js
--rw-r--r--   0        0        0       51 2022-11-14 15:08:03.429809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-base.js.flow
--rw-r--r--   0        0        0    87394 2022-11-14 15:08:03.433809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-base.js.map
--rw-r--r--   0        0        0    47193 2022-11-14 15:08:03.436809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-lite.js
--rw-r--r--   0        0        0       51 2022-11-14 15:08:03.437809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-lite.js.flow
--rw-r--r--   0        0        0   110974 2022-11-14 15:08:03.441809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-lite.js.map
--rw-r--r--   0        0        0    67554 2022-11-14 15:08:03.449809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/cjs/popper.js
--rw-r--r--   0        0        0       46 2022-11-14 15:08:03.450809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/cjs/popper.js.flow
--rw-r--r--   0        0        0   158154 2022-11-14 15:08:03.455809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/cjs/popper.js.map
--rw-r--r--   0        0        0    10007 2022-11-14 15:08:03.457809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/createPopper.js
--rw-r--r--   0        0        0      677 2022-11-14 15:08:03.578809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/contains.js
--rw-r--r--   0        0        0     1371 2022-11-14 15:08:03.579810 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getBoundingClientRect.js
--rw-r--r--   0        0        0     3400 2022-11-14 15:08:03.579810 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getClippingRect.js
--rw-r--r--   0        0        0     2072 2022-11-14 15:08:03.579810 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getCompositeRect.js
--rw-r--r--   0        0        0      148 2022-11-14 15:08:03.579810 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getComputedStyle.js
--rw-r--r--   0        0        0      311 2022-11-14 15:08:03.580809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getDocumentElement.js
--rw-r--r--   0        0        0     1227 2022-11-14 15:08:03.580809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getDocumentRect.js
--rw-r--r--   0        0        0      142 2022-11-14 15:08:03.580809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getHTMLElementScroll.js
--rw-r--r--   0        0        0      767 2022-11-14 15:08:03.581809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getLayoutRect.js
--rw-r--r--   0        0        0      114 2022-11-14 15:08:03.581809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getNodeName.js
--rw-r--r--   0        0        0      396 2022-11-14 15:08:03.581809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getNodeScroll.js
--rw-r--r--   0        0        0     2613 2022-11-14 15:08:03.582810 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getOffsetParent.js
--rw-r--r--   0        0        0      759 2022-11-14 15:08:03.582810 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getParentNode.js
--rw-r--r--   0        0        0      546 2022-11-14 15:08:03.582810 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getScrollParent.js
--rw-r--r--   0        0        0      881 2022-11-14 15:08:03.583809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getViewportRect.js
--rw-r--r--   0        0        0      273 2022-11-14 15:08:03.583809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getWindow.js
--rw-r--r--   0        0        0      258 2022-11-14 15:08:03.583809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getWindowScroll.js
--rw-r--r--   0        0        0      721 2022-11-14 15:08:03.583809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getWindowScrollBarX.js
--rw-r--r--   0        0        0      621 2022-11-14 15:08:03.584809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/instanceOf.js
--rw-r--r--   0        0        0      159 2022-11-14 15:08:03.584809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/isLayoutViewport.js
--rw-r--r--   0        0        0      440 2022-11-14 15:08:03.584809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/isScrollParent.js
--rw-r--r--   0        0        0      162 2022-11-14 15:08:03.585809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/isTableElement.js
--rw-r--r--   0        0        0     1177 2022-11-14 15:08:03.585809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/listScrollParents.js
--rw-r--r--   0        0        0     1335 2022-11-14 15:08:03.457809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/enums.js
--rw-r--r--   0        0        0      443 2022-11-14 15:08:03.458809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/index.js
--rw-r--r--   0        0        0     2527 2022-11-14 15:08:03.586809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/applyStyles.js
--rw-r--r--   0        0        0     3878 2022-11-14 15:08:03.586809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/arrow.js
--rw-r--r--   0        0        0     6566 2022-11-14 15:08:03.587809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/computeStyles.js
--rw-r--r--   0        0        0     1330 2022-11-14 15:08:03.587809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/eventListeners.js
--rw-r--r--   0        0        0     4910 2022-11-14 15:08:03.587809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/flip.js
--rw-r--r--   0        0        0     1954 2022-11-14 15:08:03.588809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/hide.js
--rw-r--r--   0        0        0      502 2022-11-14 15:08:03.588809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/index.js
--rw-r--r--   0        0        0     1613 2022-11-14 15:08:03.589810 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/offset.js
--rw-r--r--   0        0        0      706 2022-11-14 15:08:03.589810 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/popperOffsets.js
--rw-r--r--   0        0        0     6585 2022-11-14 15:08:03.589810 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/preventOverflow.js
--rw-r--r--   0        0        0      193 2022-11-14 15:08:03.458809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/popper-base.js
--rw-r--r--   0        0        0      603 2022-11-14 15:08:03.459809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/popper-lite.js
--rw-r--r--   0        0        0     1090 2022-11-14 15:08:03.459809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/popper.js
--rw-r--r--   0        0        0        0 2022-11-14 15:08:03.459809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/types.js
--rw-r--r--   0        0        0     1991 2022-11-14 15:08:03.590809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/computeAutoPlacement.js
--rw-r--r--   0        0        0     1738 2022-11-14 15:08:03.591809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/computeOffsets.js
--rw-r--r--   0        0        0      302 2022-11-14 15:08:03.591809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/debounce.js
--rw-r--r--   0        0        0     3528 2022-11-14 15:08:03.591809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/detectOverflow.js
--rw-r--r--   0        0        0      159 2022-11-14 15:08:03.592810 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/expandToHashMap.js
--rw-r--r--   0        0        0      286 2022-11-14 15:08:03.592810 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/format.js
--rw-r--r--   0        0        0       79 2022-11-14 15:08:03.592810 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getAltAxis.js
--rw-r--r--   0        0        0       89 2022-11-14 15:08:03.592810 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getAltLen.js
--rw-r--r--   0        0        0      125 2022-11-14 15:08:03.593809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getBasePlacement.js
--rw-r--r--   0        0        0      117 2022-11-14 15:08:03.593809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getFreshSideObject.js
--rw-r--r--   0        0        0      127 2022-11-14 15:08:03.593809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getMainAxisFromPlacement.js
--rw-r--r--   0        0        0      248 2022-11-14 15:08:03.594809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getOppositePlacement.js
--rw-r--r--   0        0        0      209 2022-11-14 15:08:03.594809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getOppositeVariationPlacement.js
--rw-r--r--   0        0        0       85 2022-11-14 15:08:03.594809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getVariation.js
--rw-r--r--   0        0        0       84 2022-11-14 15:08:03.595810 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/math.js
--rw-r--r--   0        0        0      524 2022-11-14 15:08:03.595810 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/mergeByName.js
--rw-r--r--   0        0        0      184 2022-11-14 15:08:03.595810 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/mergePaddingObject.js
--rw-r--r--   0        0        0     1240 2022-11-14 15:08:03.596809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/orderModifiers.js
--rw-r--r--   0        0        0      191 2022-11-14 15:08:03.596809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/rectToClientRect.js
--rw-r--r--   0        0        0      252 2022-11-14 15:08:03.597809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/uniqueBy.js
--rw-r--r--   0        0        0      269 2022-11-14 15:08:03.597809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/userAgent.js
--rw-r--r--   0        0        0     3261 2022-11-14 15:08:03.597809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/validateModifiers.js
--rw-r--r--   0        0        0      262 2022-11-14 15:08:03.597809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/esm/utils/within.js
--rw-r--r--   0        0        0     2479 2022-11-14 15:08:03.461809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/umd/enums.js
--rw-r--r--   0        0        0     4240 2022-11-14 15:08:03.461809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/umd/enums.js.map
--rw-r--r--   0        0        0     1108 2022-11-14 15:08:03.462809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/umd/enums.min.js
--rw-r--r--   0        0        0       45 2022-11-14 15:08:03.463809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/umd/enums.min.js.flow
--rw-r--r--   0        0        0     3736 2022-11-14 15:08:03.464809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/umd/enums.min.js.map
--rw-r--r--   0        0        0    38668 2022-11-14 15:08:03.465809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.js
--rw-r--r--   0        0        0    87396 2022-11-14 15:08:03.467809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.js.map
--rw-r--r--   0        0        0     9755 2022-11-14 15:08:03.467809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.min.js
--rw-r--r--   0        0        0       51 2022-11-14 15:08:03.467809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.min.js.flow
--rw-r--r--   0        0        0    60851 2022-11-14 15:08:03.468809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.min.js.map
--rw-r--r--   0        0        0    49678 2022-11-14 15:08:03.471809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.js
--rw-r--r--   0        0        0   110975 2022-11-14 15:08:03.474809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.js.map
--rw-r--r--   0        0        0    13539 2022-11-14 15:08:03.475809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.min.js
--rw-r--r--   0        0        0       51 2022-11-14 15:08:03.476809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.min.js.flow
--rw-r--r--   0        0        0    78475 2022-11-14 15:08:03.477809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.min.js.map
--rw-r--r--   0        0        0    70878 2022-11-14 15:08:03.479809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/umd/popper.js
--rw-r--r--   0        0        0   158154 2022-11-14 15:08:03.482809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/umd/popper.js.map
--rw-r--r--   0        0        0    20095 2022-11-14 15:08:03.484809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/umd/popper.min.js
--rw-r--r--   0        0        0       46 2022-11-14 15:08:03.485809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/umd/popper.min.js.flow
--rw-r--r--   0        0        0   114779 2022-11-14 15:08:03.487809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/dist/umd/popper.min.js.map
--rw-r--r--   0        0        0       23 2022-11-14 15:08:03.411809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/index.d.ts
--rw-r--r--   0        0        0      750 2022-11-14 15:08:03.412809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/createPopper.d.ts
--rw-r--r--   0        0        0    10135 2022-11-14 15:08:03.413809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/createPopper.js
--rw-r--r--   0        0        0     9415 2022-11-14 15:08:03.414809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/createPopper.js.flow
--rw-r--r--   0        0        0       76 2022-11-14 15:08:03.488809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/contains.d.ts
--rw-r--r--   0        0        0      677 2022-11-14 15:08:03.489809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/contains.js
--rw-r--r--   0        0        0      697 2022-11-14 15:08:03.490809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/contains.js.flow
--rw-r--r--   0        0        0      217 2022-11-14 15:08:03.490809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getBoundingClientRect.d.ts
--rw-r--r--   0        0        0     1371 2022-11-14 15:08:03.491809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getBoundingClientRect.js
--rw-r--r--   0        0        0     1485 2022-11-14 15:08:03.491809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getBoundingClientRect.js.flow
--rw-r--r--   0        0        0      283 2022-11-14 15:08:03.492809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getClippingRect.d.ts
--rw-r--r--   0        0        0     3400 2022-11-14 15:08:03.492809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getClippingRect.js
--rw-r--r--   0        0        0     3782 2022-11-14 15:08:03.493809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getClippingRect.js.flow
--rw-r--r--   0        0        0      212 2022-11-14 15:08:03.493809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getCompositeRect.d.ts
--rw-r--r--   0        0        0     2072 2022-11-14 15:08:03.494809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getCompositeRect.js
--rw-r--r--   0        0        0     2192 2022-11-14 15:08:03.494809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getCompositeRect.js.flow
--rw-r--r--   0        0        0       81 2022-11-14 15:08:03.496809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getComputedStyle.d.ts
--rw-r--r--   0        0        0      148 2022-11-14 15:08:03.496809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getComputedStyle.js
--rw-r--r--   0        0        0      190 2022-11-14 15:08:03.497809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getComputedStyle.js.flow
--rw-r--r--   0        0        0      124 2022-11-14 15:08:03.497809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentElement.d.ts
--rw-r--r--   0        0        0      311 2022-11-14 15:08:03.498809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentElement.js
--rw-r--r--   0        0        0      420 2022-11-14 15:08:03.498809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentElement.js.flow
--rw-r--r--   0        0        0      107 2022-11-14 15:08:03.499809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentRect.d.ts
--rw-r--r--   0        0        0     1227 2022-11-14 15:08:03.501809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentRect.js
--rw-r--r--   0        0        0     1198 2022-11-14 15:08:03.502809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentRect.js.flow
--rw-r--r--   0        0        0      120 2022-11-14 15:08:03.502809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getHTMLElementScroll.d.ts
--rw-r--r--   0        0        0      142 2022-11-14 15:08:03.503809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getHTMLElementScroll.js
--rw-r--r--   0        0        0      167 2022-11-14 15:08:03.504809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getHTMLElementScroll.js.flow
--rw-r--r--   0        0        0      105 2022-11-14 15:08:03.505809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getLayoutRect.d.ts
--rw-r--r--   0        0        0      767 2022-11-14 15:08:03.509809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getLayoutRect.js
--rw-r--r--   0        0        0      821 2022-11-14 15:08:03.509809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getLayoutRect.js.flow
--rw-r--r--   0        0        0      149 2022-11-14 15:08:03.510809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getNodeName.d.ts
--rw-r--r--   0        0        0      114 2022-11-14 15:08:03.511809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getNodeName.js
--rw-r--r--   0        0        0      190 2022-11-14 15:08:03.511809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getNodeName.js.flow
--rw-r--r--   0        0        0      146 2022-11-14 15:08:03.512809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getNodeScroll.d.ts
--rw-r--r--   0        0        0      396 2022-11-14 15:08:03.512809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getNodeScroll.js
--rw-r--r--   0        0        0      450 2022-11-14 15:08:03.513809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getNodeScroll.js.flow
--rw-r--r--   0        0        0       64 2022-11-14 15:08:03.513809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getOffsetParent.d.ts
--rw-r--r--   0        0        0     2613 2022-11-14 15:08:03.514809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getOffsetParent.js
--rw-r--r--   0        0        0     2767 2022-11-14 15:08:03.514809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getOffsetParent.js.flow
--rw-r--r--   0        0        0       73 2022-11-14 15:08:03.515809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getParentNode.d.ts
--rw-r--r--   0        0        0      759 2022-11-14 15:08:03.515809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getParentNode.js
--rw-r--r--   0        0        0      789 2022-11-14 15:08:03.515809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getParentNode.js.flow
--rw-r--r--   0        0        0       66 2022-11-14 15:08:03.516809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getScrollParent.d.ts
--rw-r--r--   0        0        0      546 2022-11-14 15:08:03.516809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getScrollParent.js
--rw-r--r--   0        0        0      564 2022-11-14 15:08:03.517809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getScrollParent.js.flow
--rw-r--r--   0        0        0      217 2022-11-14 15:08:03.517809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getViewportRect.d.ts
--rw-r--r--   0        0        0      881 2022-11-14 15:08:03.518809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getViewportRect.js
--rw-r--r--   0        0        0      964 2022-11-14 15:08:03.518809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getViewportRect.js.flow
--rw-r--r--   0        0        0       51 2022-11-14 15:08:03.519809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindow.d.ts
--rw-r--r--   0        0        0      273 2022-11-14 15:08:03.519809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindow.js
--rw-r--r--   0        0        0      383 2022-11-14 15:08:03.520809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindow.js.flow
--rw-r--r--   0        0        0      148 2022-11-14 15:08:03.520809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScroll.d.ts
--rw-r--r--   0        0        0      258 2022-11-14 15:08:03.521809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScroll.js
--rw-r--r--   0        0        0      306 2022-11-14 15:08:03.521809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScroll.js.flow
--rw-r--r--   0        0        0       71 2022-11-14 15:08:03.521809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScrollBarX.d.ts
--rw-r--r--   0        0        0      721 2022-11-14 15:08:03.522809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScrollBarX.js
--rw-r--r--   0        0        0      754 2022-11-14 15:08:03.522809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScrollBarX.js.flow
--rw-r--r--   0        0        0      214 2022-11-14 15:08:03.523809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/instanceOf.d.ts
--rw-r--r--   0        0        0      621 2022-11-14 15:08:03.523809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/instanceOf.js
--rw-r--r--   0        0        0      902 2022-11-14 15:08:03.524809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/instanceOf.js.flow
--rw-r--r--   0        0        0       53 2022-11-14 15:08:03.525809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isLayoutViewport.d.ts
--rw-r--r--   0        0        0      159 2022-11-14 15:08:03.525809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isLayoutViewport.js
--rw-r--r--   0        0        0      167 2022-11-14 15:08:03.525809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isLayoutViewport.js.flow
--rw-r--r--   0        0        0       71 2022-11-14 15:08:03.526809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isScrollParent.d.ts
--rw-r--r--   0        0        0      440 2022-11-14 15:08:03.526809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isScrollParent.js
--rw-r--r--   0        0        0      349 2022-11-14 15:08:03.527809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isScrollParent.js.flow
--rw-r--r--   0        0        0       67 2022-11-14 15:08:03.527809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isTableElement.d.ts
--rw-r--r--   0        0        0      162 2022-11-14 15:08:03.527809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isTableElement.js
--rw-r--r--   0        0        0      188 2022-11-14 15:08:03.528809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isTableElement.js.flow
--rw-r--r--   0        0        0      188 2022-11-14 15:08:03.528809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/listScrollParents.d.ts
--rw-r--r--   0        0        0     1177 2022-11-14 15:08:03.529809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/listScrollParents.js
--rw-r--r--   0        0        0     1227 2022-11-14 15:08:03.529809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/dom-utils/listScrollParents.js.flow
--rw-r--r--   0        0        0     2008 2022-11-14 15:08:03.414809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/enums.d.ts
--rw-r--r--   0        0        0     1335 2022-11-14 15:08:03.415809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/enums.js
--rw-r--r--   0        0        0     2763 2022-11-14 15:08:03.416809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/enums.js.flow
--rw-r--r--   0        0        0      286 2022-11-14 15:08:03.417809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/index.d.ts
--rw-r--r--   0        0        0      443 2022-11-14 15:08:03.417809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/index.js
--rw-r--r--   0        0        0      462 2022-11-14 15:08:03.418809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/index.js.flow
--rw-r--r--   0        0        0      183 2022-11-14 15:08:03.530809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/applyStyles.d.ts
--rw-r--r--   0        0        0     2527 2022-11-14 15:08:03.530809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/applyStyles.js
--rw-r--r--   0        0        0     2723 2022-11-14 15:08:03.531809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/applyStyles.js.flow
--rw-r--r--   0        0        0      435 2022-11-14 15:08:03.532809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/arrow.d.ts
--rw-r--r--   0        0        0     3942 2022-11-14 15:08:03.534809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/arrow.js
--rw-r--r--   0        0        0     4208 2022-11-14 15:08:03.536809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/arrow.js.flow
--rw-r--r--   0        0        0     1208 2022-11-14 15:08:03.537809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/computeStyles.d.ts
--rw-r--r--   0        0        0     6598 2022-11-14 15:08:03.537809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/computeStyles.js
--rw-r--r--   0        0        0     6945 2022-11-14 15:08:03.538809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/computeStyles.js.flow
--rw-r--r--   0        0        0      274 2022-11-14 15:08:03.539809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/eventListeners.d.ts
--rw-r--r--   0        0        0     1330 2022-11-14 15:08:03.540809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/eventListeners.js
--rw-r--r--   0        0        0     1341 2022-11-14 15:08:03.540809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/eventListeners.js.flow
--rw-r--r--   0        0        0      543 2022-11-14 15:08:03.540809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/flip.d.ts
--rw-r--r--   0        0        0     4910 2022-11-14 15:08:03.541809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/flip.js
--rw-r--r--   0        0        0     4893 2022-11-14 15:08:03.542809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/flip.js.flow
--rw-r--r--   0        0        0      162 2022-11-14 15:08:03.542809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/hide.d.ts
--rw-r--r--   0        0        0     1954 2022-11-14 15:08:03.543809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/hide.js
--rw-r--r--   0        0        0     2034 2022-11-14 15:08:03.543809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/hide.js.flow
--rw-r--r--   0        0        0      476 2022-11-14 15:08:03.544809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/index.d.ts
--rw-r--r--   0        0        0      502 2022-11-14 15:08:03.544809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/index.js
--rw-r--r--   0        0        0      485 2022-11-14 15:08:03.544809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/index.js.flow
--rw-r--r--   0        0        0      703 2022-11-14 15:08:03.545809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/offset.d.ts
--rw-r--r--   0        0        0     1613 2022-11-14 15:08:03.545809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/offset.js
--rw-r--r--   0        0        0     1933 2022-11-14 15:08:03.546809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/offset.js.flow
--rw-r--r--   0        0        0      189 2022-11-14 15:08:03.547809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/popperOffsets.d.ts
--rw-r--r--   0        0        0      706 2022-11-14 15:08:03.547809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/popperOffsets.js
--rw-r--r--   0        0        0      855 2022-11-14 15:08:03.547809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/popperOffsets.js.flow
--rw-r--r--   0        0        0      862 2022-11-14 15:08:03.548809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/preventOverflow.d.ts
--rw-r--r--   0        0        0     6585 2022-11-14 15:08:03.548809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/preventOverflow.js
--rw-r--r--   0        0        0     7439 2022-11-14 15:08:03.548809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/modifiers/preventOverflow.js.flow
--rw-r--r--   0        0        0      163 2022-11-14 15:08:03.419809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/popper-base.d.ts
--rw-r--r--   0        0        0      193 2022-11-14 15:08:03.419809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/popper-base.js
--rw-r--r--   0        0        0      232 2022-11-14 15:08:03.420809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/popper-base.js.flow
--rw-r--r--   0        0        0      705 2022-11-14 15:08:03.420809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/popper-lite.d.ts
--rw-r--r--   0        0        0      603 2022-11-14 15:08:03.420809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/popper-lite.js
--rw-r--r--   0        0        0      614 2022-11-14 15:08:03.421809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/popper-lite.js.flow
--rw-r--r--   0        0        0     1038 2022-11-14 15:08:03.421809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/popper.d.ts
--rw-r--r--   0        0        0     1090 2022-11-14 15:08:03.422809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/popper.js
--rw-r--r--   0        0        0     1082 2022-11-14 15:08:03.422809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/popper.js.flow
--rw-r--r--   0        0        0     5224 2022-11-14 15:08:03.422809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/types.d.ts
--rw-r--r--   0        0        0        0 2022-11-14 15:08:03.422809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/types.js
--rw-r--r--   0        0        0     4933 2022-11-14 15:08:03.424809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/types.js.flow
--rw-r--r--   0        0        0      466 2022-11-14 15:08:03.549809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/computeAutoPlacement.d.ts
--rw-r--r--   0        0        0     2023 2022-11-14 15:08:03.549809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/computeAutoPlacement.js
--rw-r--r--   0        0        0     2178 2022-11-14 15:08:03.550809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/computeAutoPlacement.js.flow
--rw-r--r--   0        0        0      353 2022-11-14 15:08:03.550809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/computeOffsets.d.ts
--rw-r--r--   0        0        0     1738 2022-11-14 15:08:03.550809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/computeOffsets.js
--rw-r--r--   0        0        0     1971 2022-11-14 15:08:03.550809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/computeOffsets.js.flow
--rw-r--r--   0        0        0       89 2022-11-14 15:08:03.551809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/debounce.d.ts
--rw-r--r--   0        0        0      302 2022-11-14 15:08:03.551809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/debounce.js
--rw-r--r--   0        0        0      327 2022-11-14 15:08:03.551809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/debounce.js.flow
--rw-r--r--   0        0        0      480 2022-11-14 15:08:03.551809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/detectOverflow.d.ts
--rw-r--r--   0        0        0     3528 2022-11-14 15:08:03.552809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/detectOverflow.js
--rw-r--r--   0        0        0     3265 2022-11-14 15:08:03.552809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/detectOverflow.js.flow
--rw-r--r--   0        0        0      149 2022-11-14 15:08:03.555809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/expandToHashMap.d.ts
--rw-r--r--   0        0        0      159 2022-11-14 15:08:03.555809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/expandToHashMap.js
--rw-r--r--   0        0        0      246 2022-11-14 15:08:03.555809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/expandToHashMap.js.flow
--rw-r--r--   0        0        0       77 2022-11-14 15:08:03.556809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/format.d.ts
--rw-r--r--   0        0        0      286 2022-11-14 15:08:03.556809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/format.js
--rw-r--r--   0        0        0      144 2022-11-14 15:08:03.556809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/format.js.flow
--rw-r--r--   0        0        0       64 2022-11-14 15:08:03.557809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getAltAxis.d.ts
--rw-r--r--   0        0        0       79 2022-11-14 15:08:03.557809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getAltAxis.js
--rw-r--r--   0        0        0      112 2022-11-14 15:08:03.558809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getAltAxis.js.flow
--rw-r--r--   0        0        0       80 2022-11-14 15:08:03.558809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getAltLen.d.ts
--rw-r--r--   0        0        0       89 2022-11-14 15:08:03.558809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getAltLen.js
--rw-r--r--   0        0        0      140 2022-11-14 15:08:03.559809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getAltLen.js.flow
--rw-r--r--   0        0        0      152 2022-11-14 15:08:03.559809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getBasePlacement.d.ts
--rw-r--r--   0        0        0      125 2022-11-14 15:08:03.559809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getBasePlacement.js
--rw-r--r--   0        0        0      220 2022-11-14 15:08:03.559809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getBasePlacement.js.flow
--rw-r--r--   0        0        0      102 2022-11-14 15:08:03.560809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getFreshSideObject.d.ts
--rw-r--r--   0        0        0      117 2022-11-14 15:08:03.560809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getFreshSideObject.js
--rw-r--r--   0        0        0      185 2022-11-14 15:08:03.560809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getFreshSideObject.js.flow
--rw-r--r--   0        0        0      126 2022-11-14 15:08:03.561809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getMainAxisFromPlacement.d.ts
--rw-r--r--   0        0        0      127 2022-11-14 15:08:03.561809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getMainAxisFromPlacement.js
--rw-r--r--   0        0        0      207 2022-11-14 15:08:03.562809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getMainAxisFromPlacement.js.flow
--rw-r--r--   0        0        0      122 2022-11-14 15:08:03.562809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getOppositePlacement.d.ts
--rw-r--r--   0        0        0      248 2022-11-14 15:08:03.563809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getOppositePlacement.js
--rw-r--r--   0        0        0      312 2022-11-14 15:08:03.564809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getOppositePlacement.js.flow
--rw-r--r--   0        0        0      131 2022-11-14 15:08:03.564809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getOppositeVariationPlacement.d.ts
--rw-r--r--   0        0        0      209 2022-11-14 15:08:03.564809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getOppositeVariationPlacement.js
--rw-r--r--   0        0        0      269 2022-11-14 15:08:03.565809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getOppositeVariationPlacement.js.flow
--rw-r--r--   0        0        0      139 2022-11-14 15:08:03.565809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getVariation.d.ts
--rw-r--r--   0        0        0       85 2022-11-14 15:08:03.565809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getVariation.js
--rw-r--r--   0        0        0      185 2022-11-14 15:08:03.566809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/getVariation.js.flow
--rw-r--r--   0        0        0      169 2022-11-14 15:08:03.566809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/math.d.ts
--rw-r--r--   0        0        0       84 2022-11-14 15:08:03.567809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/math.js
--rw-r--r--   0        0        0      100 2022-11-14 15:08:03.567809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/math.js.flow
--rw-r--r--   0        0        0      162 2022-11-14 15:08:03.568809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/mergeByName.d.ts
--rw-r--r--   0        0        0      524 2022-11-14 15:08:03.568809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/mergeByName.js
--rw-r--r--   0        0        0      639 2022-11-14 15:08:03.569809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/mergeByName.js.flow
--rw-r--r--   0        0        0      136 2022-11-14 15:08:03.569809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/mergePaddingObject.d.ts
--rw-r--r--   0        0        0      184 2022-11-14 15:08:03.570809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/mergePaddingObject.js
--rw-r--r--   0        0        0      274 2022-11-14 15:08:03.571809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/mergePaddingObject.js.flow
--rw-r--r--   0        0        0      147 2022-11-14 15:08:03.571809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/orderModifiers.d.ts
--rw-r--r--   0        0        0     1240 2022-11-14 15:08:03.571809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/orderModifiers.js
--rw-r--r--   0        0        0     1360 2022-11-14 15:08:03.572809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/orderModifiers.js.flow
--rw-r--r--   0        0        0      128 2022-11-14 15:08:03.572809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/rectToClientRect.d.ts
--rw-r--r--   0        0        0      191 2022-11-14 15:08:03.572809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/rectToClientRect.js
--rw-r--r--   0        0        0      271 2022-11-14 15:08:03.573809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/rectToClientRect.js.flow
--rw-r--r--   0        0        0       84 2022-11-14 15:08:03.573809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/uniqueBy.d.ts
--rw-r--r--   0        0        0      252 2022-11-14 15:08:03.573809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/uniqueBy.js
--rw-r--r--   0        0        0      293 2022-11-14 15:08:03.574809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/uniqueBy.js.flow
--rw-r--r--   0        0        0       47 2022-11-14 15:08:03.574809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/userAgent.d.ts
--rw-r--r--   0        0        0      269 2022-11-14 15:08:03.575809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/userAgent.js
--rw-r--r--   0        0        0      461 2022-11-14 15:08:03.575809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/userAgent.js.flow
--rw-r--r--   0        0        0       72 2022-11-14 15:08:03.575809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/validateModifiers.d.ts
--rw-r--r--   0        0        0     3261 2022-11-14 15:08:03.576810 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/validateModifiers.js
--rw-r--r--   0        0        0     4504 2022-11-14 15:08:03.576810 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/validateModifiers.js.flow
--rw-r--r--   0        0        0      170 2022-11-14 15:08:03.577809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/within.d.ts
--rw-r--r--   0        0        0      262 2022-11-14 15:08:03.577809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/within.js
--rw-r--r--   0        0        0      329 2022-11-14 15:08:03.577809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/lib/utils/within.js.flow
--rw-r--r--   0        0        0     4230 2022-11-14 15:08:03.411809 anitya-1.8.1/anitya/static/node_modules/@popperjs/core/package.json
--rw-r--r--   0        0        0     1131 2022-11-16 11:34:15.722286 anitya-1.8.1/anitya/static/node_modules/bootstrap/LICENSE
--rw-r--r--   0        0        0    13659 2022-11-16 11:34:15.764286 anitya-1.8.1/anitya/static/node_modules/bootstrap/README.md
--rw-r--r--   0        0        0    71861 2022-11-16 11:34:15.723286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.css
--rw-r--r--   0        0        0   210357 2022-11-16 11:34:15.745286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.css.map
--rw-r--r--   0        0        0    53265 2022-11-16 11:34:15.724286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.min.css
--rw-r--r--   0        0        0   131395 2022-11-16 11:34:15.746286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.min.css.map
--rw-r--r--   0        0        0    71935 2022-11-16 11:34:15.725286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.css
--rw-r--r--   0        0        0   210361 2022-11-16 11:34:15.746286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0        0        0    53340 2022-11-16 11:34:15.725286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0        0        0   131472 2022-11-16 11:34:15.747286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0        0        0     7965 2022-11-16 11:34:15.725286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.css
--rw-r--r--   0        0        0   110875 2022-11-16 11:34:15.747286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.css.map
--rw-r--r--   0        0        0     6490 2022-11-16 11:34:15.726286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css
--rw-r--r--   0        0        0    40331 2022-11-16 11:34:15.747286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css.map
--rw-r--r--   0        0        0     7958 2022-11-16 11:34:15.726286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.css
--rw-r--r--   0        0        0   110888 2022-11-16 11:34:15.748286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0        0        0     6562 2022-11-16 11:34:15.727286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0        0        0    48693 2022-11-16 11:34:15.748286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0        0        0    74135 2022-11-16 11:34:15.727286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.css
--rw-r--r--   0        0        0   196435 2022-11-16 11:34:15.748286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.css.map
--rw-r--r--   0        0        0    56365 2022-11-16 11:34:15.728286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.min.css
--rw-r--r--   0        0        0   115588 2022-11-16 11:34:15.749286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.min.css.map
--rw-r--r--   0        0        0    74002 2022-11-16 11:34:15.728286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.css
--rw-r--r--   0        0        0   196378 2022-11-16 11:34:15.749286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0        0        0    56293 2022-11-16 11:34:15.729286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0        0        0   115423 2022-11-16 11:34:15.750286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0        0        0   237994 2022-11-16 11:34:15.729286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap.css
--rw-r--r--   0        0        0   608416 2022-11-16 11:34:15.753286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap.css.map
--rw-r--r--   0        0        0   194901 2022-11-16 11:34:15.730286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap.min.css
--rw-r--r--   0        0        0   522733 2022-11-16 11:34:15.756286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap.min.css.map
--rw-r--r--   0        0        0   237526 2022-11-16 11:34:15.731286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap.rtl.css
--rw-r--r--   0        0        0   608236 2022-11-16 11:34:15.758286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap.rtl.css.map
--rw-r--r--   0        0        0   195007 2022-11-16 11:34:15.731286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap.rtl.min.css
--rw-r--r--   0        0        0   767573 2022-11-16 11:34:15.760286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/css/bootstrap.rtl.min.css.map
--rw-r--r--   0        0        0   208123 2022-11-16 11:34:15.734286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/js/bootstrap.bundle.js
--rw-r--r--   0        0        0   452089 2022-11-16 11:34:15.751286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/js/bootstrap.bundle.js.map
--rw-r--r--   0        0        0    80496 2022-11-16 11:34:15.734286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   333304 2022-11-16 11:34:15.752286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0   136335 2022-11-16 11:34:15.735286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/js/bootstrap.esm.js
--rw-r--r--   0        0        0   308526 2022-11-16 11:34:15.754286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/js/bootstrap.esm.js.map
--rw-r--r--   0        0        0    74054 2022-11-16 11:34:15.735286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/js/bootstrap.esm.min.js
--rw-r--r--   0        0        0   221402 2022-11-16 11:34:15.755286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/js/bootstrap.esm.min.js.map
--rw-r--r--   0        0        0   145677 2022-11-16 11:34:15.736286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/js/bootstrap.js
--rw-r--r--   0        0        0   309667 2022-11-16 11:34:15.755286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/js/bootstrap.js.map
--rw-r--r--   0        0        0    60480 2022-11-16 11:34:15.736286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/js/bootstrap.min.js
--rw-r--r--   0        0        0   217134 2022-11-16 11:34:15.757286 anitya-1.8.1/anitya/static/node_modules/bootstrap/dist/js/bootstrap.min.js.map
--rw-r--r--   0        0        0     3140 2022-11-16 11:34:15.732286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/alert.js
--rw-r--r--   0        0        0     4294 2022-11-16 11:34:15.744286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/alert.js.map
--rw-r--r--   0        0        0     3224 2022-11-16 11:34:15.733286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/base-component.js
--rw-r--r--   0        0        0     4602 2022-11-16 11:34:15.745286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/base-component.js.map
--rw-r--r--   0        0        0     2756 2022-11-16 11:34:15.736286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/button.js
--rw-r--r--   0        0        0     3466 2022-11-16 11:34:15.761286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/button.js.map
--rw-r--r--   0        0        0    14281 2022-11-16 11:34:15.737286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/carousel.js
--rw-r--r--   0        0        0    27442 2022-11-16 11:34:15.761286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/carousel.js.map
--rw-r--r--   0        0        0     9455 2022-11-16 11:34:15.737286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/collapse.js
--rw-r--r--   0        0        0    18212 2022-11-16 11:34:15.761286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/collapse.js.map
--rw-r--r--   0        0        0     2119 2022-11-16 11:34:15.738286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/dom/data.js
--rw-r--r--   0        0        0     3047 2022-11-16 11:34:15.761286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/dom/data.js.map
--rw-r--r--   0        0        0     9578 2022-11-16 11:34:15.739286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/dom/event-handler.js
--rw-r--r--   0        0        0    19800 2022-11-16 11:34:15.762286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/dom/event-handler.js.map
--rw-r--r--   0        0        0     2438 2022-11-16 11:34:15.740286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/dom/manipulator.js
--rw-r--r--   0        0        0     4319 2022-11-16 11:34:15.762286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/dom/manipulator.js.map
--rw-r--r--   0        0        0     2700 2022-11-16 11:34:15.742286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/dom/selector-engine.js
--rw-r--r--   0        0        0     4619 2022-11-16 11:34:15.763286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/dom/selector-engine.js.map
--rw-r--r--   0        0        0    16199 2022-11-16 11:34:15.739286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/dropdown.js
--rw-r--r--   0        0        0    29448 2022-11-16 11:34:15.762286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/dropdown.js.map
--rw-r--r--   0        0        0    12194 2022-11-16 11:34:15.741286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/modal.js
--rw-r--r--   0        0        0    22634 2022-11-16 11:34:15.762286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/modal.js.map
--rw-r--r--   0        0        0     9166 2022-11-16 11:34:15.741286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/offcanvas.js
--rw-r--r--   0        0        0    16142 2022-11-16 11:34:15.763286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/offcanvas.js.map
--rw-r--r--   0        0        0     2883 2022-11-16 11:34:15.741286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/popover.js
--rw-r--r--   0        0        0     4053 2022-11-16 11:34:15.763286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/popover.js.map
--rw-r--r--   0        0        0    10303 2022-11-16 11:34:15.742286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/scrollspy.js
--rw-r--r--   0        0        0    18973 2022-11-16 11:34:15.763286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/scrollspy.js.map
--rw-r--r--   0        0        0    10647 2022-11-16 11:34:15.743286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/tab.js
--rw-r--r--   0        0        0    19947 2022-11-16 11:34:15.764286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/tab.js.map
--rw-r--r--   0        0        0     6632 2022-11-16 11:34:15.744286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/toast.js
--rw-r--r--   0        0        0    12018 2022-11-16 11:34:15.764286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/toast.js.map
--rw-r--r--   0        0        0    19359 2022-11-16 11:34:15.744286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/tooltip.js
--rw-r--r--   0        0        0    37922 2022-11-16 11:34:15.764286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/tooltip.js.map
--rw-r--r--   0        0        0     4413 2022-11-16 11:34:15.732286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/util/backdrop.js
--rw-r--r--   0        0        0     7172 2022-11-16 11:34:15.745286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/util/backdrop.js.map
--rw-r--r--   0        0        0     2174 2022-11-16 11:34:15.738286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/util/component-functions.js
--rw-r--r--   0        0        0     2310 2022-11-16 11:34:15.761286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/util/component-functions.js.map
--rw-r--r--   0        0        0     2808 2022-11-16 11:34:15.738286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/util/config.js
--rw-r--r--   0        0        0     4073 2022-11-16 11:34:15.761286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/util/config.js.map
--rw-r--r--   0        0        0     3913 2022-11-16 11:34:15.740286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/util/focustrap.js
--rw-r--r--   0        0        0     5891 2022-11-16 11:34:15.762286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/util/focustrap.js.map
--rw-r--r--   0        0        0    10248 2022-11-16 11:34:15.740286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/util/index.js
--rw-r--r--   0        0        0    18675 2022-11-16 11:34:15.762286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/util/index.js.map
--rw-r--r--   0        0        0     4253 2022-11-16 11:34:15.742286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/util/sanitizer.js
--rw-r--r--   0        0        0     7572 2022-11-16 11:34:15.763286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/util/sanitizer.js.map
--rw-r--r--   0        0        0     5031 2022-11-16 11:34:15.742286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/util/scrollbar.js
--rw-r--r--   0        0        0     8041 2022-11-16 11:34:15.763286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/util/scrollbar.js.map
--rw-r--r--   0        0        0     4733 2022-11-16 11:34:15.743286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/util/swipe.js
--rw-r--r--   0        0        0     8335 2022-11-16 11:34:15.763286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/util/swipe.js.map
--rw-r--r--   0        0        0     4980 2022-11-16 11:34:15.743286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/util/template-factory.js
--rw-r--r--   0        0        0     8655 2022-11-16 11:34:15.764286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/dist/util/template-factory.js.map
--rw-r--r--   0        0        0     1901 2022-11-16 11:34:15.732286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/alert.js
--rw-r--r--   0        0        0     1930 2022-11-16 11:34:15.733286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/base-component.js
--rw-r--r--   0        0        0     1626 2022-11-16 11:34:15.737286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/button.js
--rw-r--r--   0        0        0    11820 2022-11-16 11:34:15.737286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/carousel.js
--rw-r--r--   0        0        0     7669 2022-11-16 11:34:15.737286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/collapse.js
--rw-r--r--   0        0        0     1405 2022-11-16 11:34:15.739286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/dom/data.js
--rw-r--r--   0        0        0     8450 2022-11-16 11:34:15.739286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/dom/event-handler.js
--rw-r--r--   0        0        0     1668 2022-11-16 11:34:15.740286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/dom/manipulator.js
--rw-r--r--   0        0        0     1968 2022-11-16 11:34:15.743286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/dom/selector-engine.js
--rw-r--r--   0        0        0    13257 2022-11-16 11:34:15.739286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/dropdown.js
--rw-r--r--   0        0        0     9629 2022-11-16 11:34:15.741286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/modal.js
--rw-r--r--   0        0        0     6804 2022-11-16 11:34:15.741286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/offcanvas.js
--rw-r--r--   0        0        0     1874 2022-11-16 11:34:15.741286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/popover.js
--rw-r--r--   0        0        0     8448 2022-11-16 11:34:15.742286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/scrollspy.js
--rw-r--r--   0        0        0     8756 2022-11-16 11:34:15.743286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/tab.js
--rw-r--r--   0        0        0     5037 2022-11-16 11:34:15.744286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/toast.js
--rw-r--r--   0        0        0    16305 2022-11-16 11:34:15.744286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/tooltip.js
--rw-r--r--   0        0        0     3126 2022-11-16 11:34:15.733286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/util/backdrop.js
--rw-r--r--   0        0        0     1072 2022-11-16 11:34:15.738286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/util/component-functions.js
--rw-r--r--   0        0        0     1818 2022-11-16 11:34:15.738286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/util/config.js
--rw-r--r--   0        0        0     2519 2022-11-16 11:34:15.740286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/util/focustrap.js
--rw-r--r--   0        0        0     8436 2022-11-16 11:34:15.740286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/util/index.js
--rw-r--r--   0        0        0     3253 2022-11-16 11:34:15.742286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/util/sanitizer.js
--rw-r--r--   0        0        0     3755 2022-11-16 11:34:15.742286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/util/scrollbar.js
--rw-r--r--   0        0        0     3410 2022-11-16 11:34:15.743286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/util/swipe.js
--rw-r--r--   0        0        0     3630 2022-11-16 11:34:15.743286 anitya-1.8.1/anitya/static/node_modules/bootstrap/js/src/util/template-factory.js
--rw-r--r--   0        0        0     9330 2022-11-16 11:34:15.744286 anitya-1.8.1/anitya/static/node_modules/bootstrap/package.json
--rw-r--r--   0        0        0     4790 2022-11-16 11:34:15.765286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_accordion.scss
--rw-r--r--   0        0        0     2126 2022-11-16 11:34:15.765286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_alert.scss
--rw-r--r--   0        0        0     1118 2022-11-16 11:34:15.765286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_badge.scss
--rw-r--r--   0        0        0     1751 2022-11-16 11:34:15.766286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_breadcrumb.scss
--rw-r--r--   0        0        0     3073 2022-11-16 11:34:15.766286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_button-group.scss
--rw-r--r--   0        0        0     6685 2022-11-16 11:34:15.766286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_buttons.scss
--rw-r--r--   0        0        0     6736 2022-11-16 11:34:15.766286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_card.scss
--rw-r--r--   0        0        0     5625 2022-11-16 11:34:15.767286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_carousel.scss
--rw-r--r--   0        0        0     1127 2022-11-16 11:34:15.767286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_close.scss
--rw-r--r--   0        0        0     1201 2022-11-16 11:34:15.769286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_containers.scss
--rw-r--r--   0        0        0     8018 2022-11-16 11:34:15.770286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_dropdown.scss
--rw-r--r--   0        0        0      256 2022-11-16 11:34:15.773286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_forms.scss
--rw-r--r--   0        0        0    10553 2022-11-16 11:34:15.773286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_functions.scss
--rw-r--r--   0        0        0      575 2022-11-16 11:34:15.774286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_grid.scss
--rw-r--r--   0        0        0      294 2022-11-16 11:34:15.774286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_helpers.scss
--rw-r--r--   0        0        0     1158 2022-11-16 11:34:15.774286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_images.scss
--rw-r--r--   0        0        0     6475 2022-11-16 11:34:15.775287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_list-group.scss
--rw-r--r--   0        0        0     1648 2022-11-16 11:34:15.776286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_maps.scss
--rw-r--r--   0        0        0      899 2022-11-16 11:34:15.776286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_mixins.scss
--rw-r--r--   0        0        0     7762 2022-11-16 11:34:15.776286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_modal.scss
--rw-r--r--   0        0        0     4665 2022-11-16 11:34:15.777286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_nav.scss
--rw-r--r--   0        0        0     8936 2022-11-16 11:34:15.777286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_navbar.scss
--rw-r--r--   0        0        0     4555 2022-11-16 11:34:15.777286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_offcanvas.scss
--rw-r--r--   0        0        0     3940 2022-11-16 11:34:15.777286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_pagination.scss
--rw-r--r--   0        0        0      859 2022-11-16 11:34:15.778287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_placeholders.scss
--rw-r--r--   0        0        0     6907 2022-11-16 11:34:15.778287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_popover.scss
--rw-r--r--   0        0        0     1875 2022-11-16 11:34:15.778287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_progress.scss
--rw-r--r--   0        0        0    12311 2022-11-16 11:34:15.779286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_reboot.scss
--rw-r--r--   0        0        0     2395 2022-11-16 11:34:15.780286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_root.scss
--rw-r--r--   0        0        0     2429 2022-11-16 11:34:15.780286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_spinners.scss
--rw-r--r--   0        0        0     4358 2022-11-16 11:34:15.780286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_tables.scss
--rw-r--r--   0        0        0     2490 2022-11-16 11:34:15.781287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_toasts.scss
--rw-r--r--   0        0        0     3939 2022-11-16 11:34:15.781287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_tooltip.scss
--rw-r--r--   0        0        0      425 2022-11-16 11:34:15.782287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_transitions.scss
--rw-r--r--   0        0        0     1420 2022-11-16 11:34:15.782287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_type.scss
--rw-r--r--   0        0        0    14817 2022-11-16 11:34:15.782287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_utilities.scss
--rw-r--r--   0        0        0    68610 2022-11-16 11:34:15.783286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/_variables.scss
--rw-r--r--   0        0        0     1198 2022-11-16 11:34:15.783286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/bootstrap-grid.scss
--rw-r--r--   0        0        0      163 2022-11-16 11:34:15.784287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/bootstrap-reboot.scss
--rw-r--r--   0        0        0      240 2022-11-16 11:34:15.784287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/bootstrap-utilities.scss
--rw-r--r--   0        0        0      912 2022-11-16 11:34:15.784287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/bootstrap.scss
--rw-r--r--   0        0        0     2030 2022-11-16 11:34:15.771286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/forms/_floating-labels.scss
--rw-r--r--   0        0        0     4287 2022-11-16 11:34:15.771286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/forms/_form-check.scss
--rw-r--r--   0        0        0     5695 2022-11-16 11:34:15.771286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/forms/_form-control.scss
--rw-r--r--   0        0        0     2796 2022-11-16 11:34:15.771286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/forms/_form-range.scss
--rw-r--r--   0        0        0     2316 2022-11-16 11:34:15.771286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/forms/_form-select.scss
--rw-r--r--   0        0        0      219 2022-11-16 11:34:15.771286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/forms/_form-text.scss
--rw-r--r--   0        0        0     3835 2022-11-16 11:34:15.775287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/forms/_input-group.scss
--rw-r--r--   0        0        0     1142 2022-11-16 11:34:15.775287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/forms/_labels.scss
--rw-r--r--   0        0        0      478 2022-11-16 11:34:15.782287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/forms/_validation.scss
--rw-r--r--   0        0        0       37 2022-11-16 11:34:15.767286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/helpers/_clearfix.scss
--rw-r--r--   0        0        0      454 2022-11-16 11:34:15.767286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/helpers/_color-bg.scss
--rw-r--r--   0        0        0      450 2022-11-16 11:34:15.769286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/helpers/_colored-links.scss
--rw-r--r--   0        0        0      621 2022-11-16 11:34:15.778287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/helpers/_position.scss
--rw-r--r--   0        0        0      399 2022-11-16 11:34:15.779286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/helpers/_ratio.scss
--rw-r--r--   0        0        0      245 2022-11-16 11:34:15.780286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/helpers/_stacks.scss
--rw-r--r--   0        0        0      223 2022-11-16 11:34:15.780286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/helpers/_stretched-link.scss
--rw-r--r--   0        0        0       73 2022-11-16 11:34:15.781287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/helpers/_text-truncation.scss
--rw-r--r--   0        0        0      136 2022-11-16 11:34:15.783286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/helpers/_visually-hidden.scss
--rw-r--r--   0        0        0      147 2022-11-16 11:34:15.783286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/helpers/_vr.scss
--rw-r--r--   0        0        0      393 2022-11-16 11:34:15.765286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_alert.scss
--rw-r--r--   0        0        0      328 2022-11-16 11:34:15.765286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_backdrop.scss
--rw-r--r--   0        0        0      263 2022-11-16 11:34:15.765286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_banner.scss
--rw-r--r--   0        0        0     2031 2022-11-16 11:34:15.766286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_border-radius.scss
--rw-r--r--   0        0        0      398 2022-11-16 11:34:15.766286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_box-shadow.scss
--rw-r--r--   0        0        0     4580 2022-11-16 11:34:15.766286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_breakpoints.scss
--rw-r--r--   0        0        0     3220 2022-11-16 11:34:15.766286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_buttons.scss
--rw-r--r--   0        0        0     1473 2022-11-16 11:34:15.767286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_caret.scss
--rw-r--r--   0        0        0      147 2022-11-16 11:34:15.767286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_clearfix.scss
--rw-r--r--   0        0        0      167 2022-11-16 11:34:15.769286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_color-scheme.scss
--rw-r--r--   0        0        0      410 2022-11-16 11:34:15.769286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_container.scss
--rw-r--r--   0        0        0      613 2022-11-16 11:34:15.770286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_deprecate.scss
--rw-r--r--   0        0        0     4122 2022-11-16 11:34:15.773286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_forms.scss
--rw-r--r--   0        0        0     1956 2022-11-16 11:34:15.773286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_gradients.scss
--rw-r--r--   0        0        0     4726 2022-11-16 11:34:15.774286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_grid.scss
--rw-r--r--   0        0        0      395 2022-11-16 11:34:15.774286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_image.scss
--rw-r--r--   0        0        0      509 2022-11-16 11:34:15.776286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_list-group.scss
--rw-r--r--   0        0        0      168 2022-11-16 11:34:15.776286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_lists.scss
--rw-r--r--   0        0        0      387 2022-11-16 11:34:15.778287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_pagination.scss
--rw-r--r--   0        0        0      495 2022-11-16 11:34:15.779286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_reset-text.scss
--rw-r--r--   0        0        0      202 2022-11-16 11:34:15.779286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_resize.scss
--rw-r--r--   0        0        0     1101 2022-11-16 11:34:15.780286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_table-variants.scss
--rw-r--r--   0        0        0      168 2022-11-16 11:34:15.781287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_text-truncate.scss
--rw-r--r--   0        0        0      661 2022-11-16 11:34:15.781287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_transition.scss
--rw-r--r--   0        0        0     3380 2022-11-16 11:34:15.782287 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_utilities.scss
--rw-r--r--   0        0        0     1012 2022-11-16 11:34:15.783286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/mixins/_visually-hidden.scss
--rw-r--r--   0        0        0     1737 2022-11-16 11:34:15.765286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/utilities/_api.scss
--rw-r--r--   0        0        0    10029 2022-11-16 11:34:15.779286 anitya-1.8.1/anitya/static/node_modules/bootstrap/scss/vendor/_rfs.scss
--rw-r--r--   0        0        0    12631 2022-11-14 15:08:03.532809 anitya-1.8.1/anitya/static/node_modules/jquery/AUTHORS.txt
--rw-r--r--   0        0        0     1097 2022-11-14 15:08:03.538809 anitya-1.8.1/anitya/static/node_modules/jquery/LICENSE.txt
--rw-r--r--   0        0        0     2004 2022-11-14 15:08:03.531809 anitya-1.8.1/anitya/static/node_modules/jquery/README.md
--rw-r--r--   0        0        0      190 2022-11-14 15:08:03.522809 anitya-1.8.1/anitya/static/node_modules/jquery/bower.json
--rw-r--r--   0        0        0   289812 2022-11-14 15:08:03.468809 anitya-1.8.1/anitya/static/node_modules/jquery/dist/jquery.js
--rw-r--r--   0        0        0    89664 2022-11-14 15:08:03.472809 anitya-1.8.1/anitya/static/node_modules/jquery/dist/jquery.min.js
--rw-r--r--   0        0        0   138161 2022-11-14 15:08:03.526809 anitya-1.8.1/anitya/static/node_modules/jquery/dist/jquery.min.map
--rw-r--r--   0        0        0   236513 2022-11-14 15:08:03.477809 anitya-1.8.1/anitya/static/node_modules/jquery/dist/jquery.slim.js
--rw-r--r--   0        0        0    72535 2022-11-14 15:08:03.479809 anitya-1.8.1/anitya/static/node_modules/jquery/dist/jquery.slim.min.js
--rw-r--r--   0        0        0   110515 2022-11-14 15:08:03.529809 anitya-1.8.1/anitya/static/node_modules/jquery/dist/jquery.slim.min.map
--rw-r--r--   0        0        0     1605 2022-11-14 15:08:03.537809 anitya-1.8.1/anitya/static/node_modules/jquery/external/sizzle/LICENSE.txt
--rw-r--r--   0        0        0    70555 2022-11-14 15:08:03.509809 anitya-1.8.1/anitya/static/node_modules/jquery/external/sizzle/dist/sizzle.js
--rw-r--r--   0        0        0    20245 2022-11-14 15:08:03.510809 anitya-1.8.1/anitya/static/node_modules/jquery/external/sizzle/dist/sizzle.min.js
--rw-r--r--   0        0        0    31112 2022-11-14 15:08:03.530809 anitya-1.8.1/anitya/static/node_modules/jquery/external/sizzle/dist/sizzle.min.map
--rw-r--r--   0        0        0     3284 2022-11-14 15:08:03.523809 anitya-1.8.1/anitya/static/node_modules/jquery/package.json
--rw-r--r--   0        0        0     2753 2022-11-14 15:08:03.480809 anitya-1.8.1/anitya/static/node_modules/jquery/src/ajax/jsonp.js
--rw-r--r--   0        0        0     1904 2022-11-14 15:08:03.480809 anitya-1.8.1/anitya/static/node_modules/jquery/src/ajax/load.js
--rw-r--r--   0        0        0     1637 2022-11-14 15:08:03.496809 anitya-1.8.1/anitya/static/node_modules/jquery/src/ajax/script.js
--rw-r--r--   0        0        0       67 2022-11-14 15:08:03.481809 anitya-1.8.1/anitya/static/node_modules/jquery/src/ajax/var/location.js
--rw-r--r--   0        0        0       72 2022-11-14 15:08:03.482809 anitya-1.8.1/anitya/static/node_modules/jquery/src/ajax/var/nonce.js
--rw-r--r--   0        0        0       60 2022-11-14 15:08:03.492809 anitya-1.8.1/anitya/static/node_modules/jquery/src/ajax/var/rquery.js
--rw-r--r--   0        0        0     4355 2022-11-14 15:08:03.521809 anitya-1.8.1/anitya/static/node_modules/jquery/src/ajax/xhr.js
--rw-r--r--   0        0        0    22924 2022-11-14 15:08:03.421809 anitya-1.8.1/anitya/static/node_modules/jquery/src/ajax.js
--rw-r--r--   0        0        0     3272 2022-11-14 15:08:03.425809 anitya-1.8.1/anitya/static/node_modules/jquery/src/attributes/attr.js
--rw-r--r--   0        0        0     4527 2022-11-14 15:08:03.428809 anitya-1.8.1/anitya/static/node_modules/jquery/src/attributes/classes.js
--rw-r--r--   0        0        0     2857 2022-11-14 15:08:03.486809 anitya-1.8.1/anitya/static/node_modules/jquery/src/attributes/prop.js
--rw-r--r--   0        0        0      786 2022-11-14 15:08:03.513809 anitya-1.8.1/anitya/static/node_modules/jquery/src/attributes/support.js
--rw-r--r--   0        0        0     4261 2022-11-14 15:08:03.519809 anitya-1.8.1/anitya/static/node_modules/jquery/src/attributes/val.js
--rw-r--r--   0        0        0      217 2022-11-14 15:08:03.425809 anitya-1.8.1/anitya/static/node_modules/jquery/src/attributes.js
--rw-r--r--   0        0        0     5552 2022-11-14 15:08:03.427809 anitya-1.8.1/anitya/static/node_modules/jquery/src/callbacks.js
--rw-r--r--   0        0        0     1160 2022-11-14 15:08:03.449809 anitya-1.8.1/anitya/static/node_modules/jquery/src/core/DOMEval.js
--rw-r--r--   0        0        0     1314 2022-11-14 15:08:03.414809 anitya-1.8.1/anitya/static/node_modules/jquery/src/core/access.js
--rw-r--r--   0        0        0      550 2022-11-14 15:08:03.427809 anitya-1.8.1/anitya/static/node_modules/jquery/src/core/camelCase.js
--rw-r--r--   0        0        0     3345 2022-11-14 15:08:03.460809 anitya-1.8.1/anitya/static/node_modules/jquery/src/core/init.js
--rw-r--r--   0        0        0      789 2022-11-14 15:08:03.461809 anitya-1.8.1/anitya/static/node_modules/jquery/src/core/isAttached.js
--rw-r--r--   0        0        0      176 2022-11-14 15:08:03.482809 anitya-1.8.1/anitya/static/node_modules/jquery/src/core/nodeName.js
--rw-r--r--   0        0        0     1604 2022-11-14 15:08:03.485809 anitya-1.8.1/anitya/static/node_modules/jquery/src/core/parseHTML.js
--rw-r--r--   0        0        0      739 2022-11-14 15:08:03.486809 anitya-1.8.1/anitya/static/node_modules/jquery/src/core/parseXML.js
--rw-r--r--   0        0        0     2268 2022-11-14 15:08:03.489809 anitya-1.8.1/anitya/static/node_modules/jquery/src/core/ready-no-deferred.js
--rw-r--r--   0        0        0     2101 2022-11-14 15:08:03.490809 anitya-1.8.1/anitya/static/node_modules/jquery/src/core/ready.js
--rw-r--r--   0        0        0      168 2022-11-14 15:08:03.490809 anitya-1.8.1/anitya/static/node_modules/jquery/src/core/readyException.js
--rw-r--r--   0        0        0      362 2022-11-14 15:08:03.512809 anitya-1.8.1/anitya/static/node_modules/jquery/src/core/stripAndCollapse.js
--rw-r--r--   0        0        0      631 2022-11-14 15:08:03.513809 anitya-1.8.1/anitya/static/node_modules/jquery/src/core/support.js
--rw-r--r--   0        0        0      379 2022-11-14 15:08:03.516809 anitya-1.8.1/anitya/static/node_modules/jquery/src/core/toType.js
--rw-r--r--   0        0        0      244 2022-11-14 15:08:03.494809 anitya-1.8.1/anitya/static/node_modules/jquery/src/core/var/rsingleTag.js
--rw-r--r--   0        0        0     9183 2022-11-14 15:08:03.429809 anitya-1.8.1/anitya/static/node_modules/jquery/src/core.js
--rw-r--r--   0        0        0      530 2022-11-14 15:08:03.416809 anitya-1.8.1/anitya/static/node_modules/jquery/src/css/addGetHookIf.js
--rw-r--r--   0        0        0     2002 2022-11-14 15:08:03.417809 anitya-1.8.1/anitya/static/node_modules/jquery/src/css/adjustCSS.js
--rw-r--r--   0        0        0     2191 2022-11-14 15:08:03.434809 anitya-1.8.1/anitya/static/node_modules/jquery/src/css/curCSS.js
--rw-r--r--   0        0        0      870 2022-11-14 15:08:03.454809 anitya-1.8.1/anitya/static/node_modules/jquery/src/css/finalPropName.js
--rw-r--r--   0        0        0      317 2022-11-14 15:08:03.460809 anitya-1.8.1/anitya/static/node_modules/jquery/src/css/hiddenVisibleSelectors.js
--rw-r--r--   0        0        0     2304 2022-11-14 15:08:03.499809 anitya-1.8.1/anitya/static/node_modules/jquery/src/css/showHide.js
--rw-r--r--   0        0        0     4829 2022-11-14 15:08:03.514809 anitya-1.8.1/anitya/static/node_modules/jquery/src/css/support.js
--rw-r--r--   0        0        0       88 2022-11-14 15:08:03.433809 anitya-1.8.1/anitya/static/node_modules/jquery/src/css/var/cssExpand.js
--rw-r--r--   0        0        0      409 2022-11-14 15:08:03.458809 anitya-1.8.1/anitya/static/node_modules/jquery/src/css/var/getStyles.js
--rw-r--r--   0        0        0     1284 2022-11-14 15:08:03.461809 anitya-1.8.1/anitya/static/node_modules/jquery/src/css/var/isHiddenWithinTree.js
--rw-r--r--   0        0        0      123 2022-11-14 15:08:03.487809 anitya-1.8.1/anitya/static/node_modules/jquery/src/css/var/rboxStyle.js
--rw-r--r--   0        0        0       57 2022-11-14 15:08:03.489809 anitya-1.8.1/anitya/static/node_modules/jquery/src/css/var/rcustomProp.js
--rw-r--r--   0        0        0      131 2022-11-14 15:08:03.492809 anitya-1.8.1/anitya/static/node_modules/jquery/src/css/var/rnumnonpx.js
--rw-r--r--   0        0        0      501 2022-11-14 15:08:03.515809 anitya-1.8.1/anitya/static/node_modules/jquery/src/css/var/swap.js
--rw-r--r--   0        0        0    14195 2022-11-14 15:08:03.430809 anitya-1.8.1/anitya/static/node_modules/jquery/src/css.js
--rw-r--r--   0        0        0     3956 2022-11-14 15:08:03.436809 anitya-1.8.1/anitya/static/node_modules/jquery/src/data/Data.js
--rw-r--r--   0        0        0      318 2022-11-14 15:08:03.412809 anitya-1.8.1/anitya/static/node_modules/jquery/src/data/var/acceptData.js
--rw-r--r--   0        0        0       84 2022-11-14 15:08:03.437809 anitya-1.8.1/anitya/static/node_modules/jquery/src/data/var/dataPriv.js
--rw-r--r--   0        0        0       84 2022-11-14 15:08:03.437809 anitya-1.8.1/anitya/static/node_modules/jquery/src/data/var/dataUser.js
--rw-r--r--   0        0        0     4325 2022-11-14 15:08:03.435809 anitya-1.8.1/anitya/static/node_modules/jquery/src/data.js
--rw-r--r--   0        0        0      640 2022-11-14 15:08:03.452809 anitya-1.8.1/anitya/static/node_modules/jquery/src/deferred/exceptionHook.js
--rw-r--r--   0        0        0    11007 2022-11-14 15:08:03.438809 anitya-1.8.1/anitya/static/node_modules/jquery/src/deferred.js
--rw-r--r--   0        0        0      296 2022-11-14 15:08:03.419809 anitya-1.8.1/anitya/static/node_modules/jquery/src/deprecated/ajax-event-alias.js
--rw-r--r--   0        0        0     1140 2022-11-14 15:08:03.451809 anitya-1.8.1/anitya/static/node_modules/jquery/src/deprecated/event.js
--rw-r--r--   0        0        0     2406 2022-11-14 15:08:03.440809 anitya-1.8.1/anitya/static/node_modules/jquery/src/deprecated.js
--rw-r--r--   0        0        0     1756 2022-11-14 15:08:03.441809 anitya-1.8.1/anitya/static/node_modules/jquery/src/dimensions.js
--rw-r--r--   0        0        0     3291 2022-11-14 15:08:03.518809 anitya-1.8.1/anitya/static/node_modules/jquery/src/effects/Tween.js
--rw-r--r--   0        0        0      244 2022-11-14 15:08:03.423809 anitya-1.8.1/anitya/static/node_modules/jquery/src/effects/animatedSelector.js
--rw-r--r--   0        0        0    17417 2022-11-14 15:08:03.450809 anitya-1.8.1/anitya/static/node_modules/jquery/src/effects.js
--rw-r--r--   0        0        0     1665 2022-11-14 15:08:03.457809 anitya-1.8.1/anitya/static/node_modules/jquery/src/event/focusin.js
--rw-r--r--   0        0        0      133 2022-11-14 15:08:03.514809 anitya-1.8.1/anitya/static/node_modules/jquery/src/event/support.js
--rw-r--r--   0        0        0     5438 2022-11-14 15:08:03.518809 anitya-1.8.1/anitya/static/node_modules/jquery/src/event/trigger.js
--rw-r--r--   0        0        0    24505 2022-11-14 15:08:03.452809 anitya-1.8.1/anitya/static/node_modules/jquery/src/event.js
--rw-r--r--   0        0        0     1024 2022-11-14 15:08:03.422809 anitya-1.8.1/anitya/static/node_modules/jquery/src/exports/amd.js
--rw-r--r--   0        0        0      628 2022-11-14 15:08:03.459809 anitya-1.8.1/anitya/static/node_modules/jquery/src/exports/global.js
--rw-r--r--   0        0        0      646 2022-11-14 15:08:03.470809 anitya-1.8.1/anitya/static/node_modules/jquery/src/jquery.js
--rw-r--r--   0        0        0      690 2022-11-14 15:08:03.409809 anitya-1.8.1/anitya/static/node_modules/jquery/src/manipulation/_evalUrl.js
--rw-r--r--   0        0        0     2490 2022-11-14 15:08:03.426809 anitya-1.8.1/anitya/static/node_modules/jquery/src/manipulation/buildFragment.js
--rw-r--r--   0        0        0      654 2022-11-14 15:08:03.457809 anitya-1.8.1/anitya/static/node_modules/jquery/src/manipulation/getAll.js
--rw-r--r--   0        0        0      381 2022-11-14 15:08:03.499809 anitya-1.8.1/anitya/static/node_modules/jquery/src/manipulation/setGlobalEval.js
--rw-r--r--   0        0        0     1244 2022-11-14 15:08:03.514809 anitya-1.8.1/anitya/static/node_modules/jquery/src/manipulation/support.js
--rw-r--r--   0        0        0       92 2022-11-14 15:08:03.493809 anitya-1.8.1/anitya/static/node_modules/jquery/src/manipulation/var/rscriptType.js
--rw-r--r--   0        0        0      304 2022-11-14 15:08:03.494809 anitya-1.8.1/anitya/static/node_modules/jquery/src/manipulation/var/rtagName.js
--rw-r--r--   0        0        0      823 2022-11-14 15:08:03.520809 anitya-1.8.1/anitya/static/node_modules/jquery/src/manipulation/wrapMap.js
--rw-r--r--   0        0        0    12674 2022-11-14 15:08:03.481809 anitya-1.8.1/anitya/static/node_modules/jquery/src/manipulation.js
--rw-r--r--   0        0        0     6828 2022-11-14 15:08:03.484809 anitya-1.8.1/anitya/static/node_modules/jquery/src/offset.js
--rw-r--r--   0        0        0      534 2022-11-14 15:08:03.439809 anitya-1.8.1/anitya/static/node_modules/jquery/src/queue/delay.js
--rw-r--r--   0        0        0     3091 2022-11-14 15:08:03.487809 anitya-1.8.1/anitya/static/node_modules/jquery/src/queue.js
--rw-r--r--   0        0        0     6463 2022-11-14 15:08:03.497809 anitya-1.8.1/anitya/static/node_modules/jquery/src/selector-native.js
--rw-r--r--   0        0        0      411 2022-11-14 15:08:03.497809 anitya-1.8.1/anitya/static/node_modules/jquery/src/selector-sizzle.js
--rw-r--r--   0        0        0       66 2022-11-14 15:08:03.498809 anitya-1.8.1/anitya/static/node_modules/jquery/src/selector.js
--rw-r--r--   0        0        0     3236 2022-11-14 15:08:03.498809 anitya-1.8.1/anitya/static/node_modules/jquery/src/serialize.js
--rw-r--r--   0        0        0     2352 2022-11-14 15:08:03.455809 anitya-1.8.1/anitya/static/node_modules/jquery/src/traversing/findFilter.js
--rw-r--r--   0        0        0      371 2022-11-14 15:08:03.447809 anitya-1.8.1/anitya/static/node_modules/jquery/src/traversing/var/dir.js
--rw-r--r--   0        0        0      128 2022-11-14 15:08:03.491809 anitya-1.8.1/anitya/static/node_modules/jquery/src/traversing/var/rneedsContext.js
--rw-r--r--   0        0        0      218 2022-11-14 15:08:03.500809 anitya-1.8.1/anitya/static/node_modules/jquery/src/traversing/var/siblings.js
--rw-r--r--   0        0        0     4692 2022-11-14 15:08:03.517809 anitya-1.8.1/anitya/static/node_modules/jquery/src/traversing.js
--rw-r--r--   0        0        0      110 2022-11-14 15:08:03.483809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/ObjectFunctionString.js
--rw-r--r--   0        0        0       54 2022-11-14 15:08:03.424809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/arr.js
--rw-r--r--   0        0        0       82 2022-11-14 15:08:03.428809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/class2type.js
--rw-r--r--   0        0        0       67 2022-11-14 15:08:03.448809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/document.js
--rw-r--r--   0        0        0      105 2022-11-14 15:08:03.448809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/documentElement.js
--rw-r--r--   0        0        0      372 2022-11-14 15:08:03.455809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/flat.js
--rw-r--r--   0        0        0       92 2022-11-14 15:08:03.456809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/fnToString.js
--rw-r--r--   0        0        0       73 2022-11-14 15:08:03.458809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/getProto.js
--rw-r--r--   0        0        0      110 2022-11-14 15:08:03.459809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/hasOwn.js
--rw-r--r--   0        0        0       82 2022-11-14 15:08:03.460809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/indexOf.js
--rw-r--r--   0        0        0      674 2022-11-14 15:08:03.461809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/isFunction.js
--rw-r--r--   0        0        0      126 2022-11-14 15:08:03.462809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/isWindow.js
--rw-r--r--   0        0        0      100 2022-11-14 15:08:03.486809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/pnum.js
--rw-r--r--   0        0        0       79 2022-11-14 15:08:03.486809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/push.js
--rw-r--r--   0        0        0       79 2022-11-14 15:08:03.488809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/rcheckableType.js
--rw-r--r--   0        0        0      136 2022-11-14 15:08:03.488809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/rcssNum.js
--rw-r--r--   0        0        0      202 2022-11-14 15:08:03.491809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/rnothtmlwhite.js
--rw-r--r--   0        0        0      174 2022-11-14 15:08:03.494809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/rtrimCSS.js
--rw-r--r--   0        0        0       80 2022-11-14 15:08:03.512809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/slice.js
--rw-r--r--   0        0        0      117 2022-11-14 15:08:03.515809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/support.js
--rw-r--r--   0        0        0      104 2022-11-14 15:08:03.516809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/toString.js
--rw-r--r--   0        0        0      125 2022-11-14 15:08:03.519809 anitya-1.8.1/anitya/static/node_modules/jquery/src/var/whitespace.js
--rw-r--r--   0        0        0     1477 2022-11-14 15:08:03.520809 anitya-1.8.1/anitya/static/node_modules/jquery/src/wrap.js
--rw-r--r--   0        0        0      115 2022-11-14 15:08:03.829810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/.github/dependabot.yml
--rw-r--r--   0        0        0     1484 2022-11-14 15:08:03.829810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/.github/workflows/test.yml
--rw-r--r--   0        0        0    14243 2022-11-14 15:08:03.819810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/AUTHORS.txt
--rw-r--r--   0        0        0     4545 2022-11-14 15:08:03.751810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/CONTRIBUTING.md
--rw-r--r--   0        0        0     1817 2022-11-14 15:08:03.824810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/LICENSE.txt
--rw-r--r--   0        0        0     2470 2022-11-14 15:08:03.751810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/README.md
--rw-r--r--   0        0        0     2262 2022-11-14 15:08:03.751810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/bower.json
--rw-r--r--   0        0        0     1241 2022-11-14 15:08:03.746810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/build/release-test.js
--rw-r--r--   0        0        0     4749 2022-11-14 15:08:03.746810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/build/release.js
--rw-r--r--   0        0        0     1108 2022-11-14 15:08:03.593809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/build/tasks/build.js
--rw-r--r--   0        0        0     3110 2022-11-14 15:08:03.750810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/build/tasks/testswarm.js
--rw-r--r--   0        0        0    60060 2022-11-14 15:08:03.413809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/build/themes
--rw-r--r--   0        0        0   529159 2022-11-14 15:08:03.637810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/jquery-ui.js
--rw-r--r--   0        0        0   255084 2022-11-14 15:08:03.640810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/jquery-ui.min.js
--rw-r--r--   0        0        0     7142 2022-11-14 15:08:03.792810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_444444_256x240.png
--rw-r--r--   0        0        0     7126 2022-11-14 15:08:03.795810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_555555_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.797810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_777620_256x240.png
--rw-r--r--   0        0        0     7163 2022-11-14 15:08:03.797810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_777777_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.806810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.814810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36099 2022-11-14 15:08:03.424809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/base/jquery-ui.css
--rw-r--r--   0        0        0    30778 2022-11-14 15:08:03.525809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/base/jquery-ui.min.css
--rw-r--r--   0        0        0    17432 2022-11-14 15:08:03.565809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/base/theme.css
--rw-r--r--   0        0        0      435 2022-11-14 15:08:03.756810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_diagonals-thick_8_333333_40x40.png
--rw-r--r--   0        0        0      375 2022-11-14 15:08:03.768810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_glass_40_111111_1x400.png
--rw-r--r--   0        0        0      375 2022-11-14 15:08:03.769810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_glass_55_1c1c1c_1x400.png
--rw-r--r--   0        0        0      367 2022-11-14 15:08:03.778810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_highlight-hard_100_f9f9f9_1x100.png
--rw-r--r--   0        0        0      368 2022-11-14 15:08:03.779810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_highlight-hard_40_aaaaaa_1x100.png
--rw-r--r--   0        0        0      379 2022-11-14 15:08:03.783810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_highlight-soft_50_aaaaaa_1x100.png
--rw-r--r--   0        0        0      434 2022-11-14 15:08:03.785810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_inset-hard_45_cd0a0a_1x100.png
--rw-r--r--   0        0        0      419 2022-11-14 15:08:03.785810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_inset-hard_55_ffeb80_1x100.png
--rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.789810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_222222_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.794810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_4ca300_256x240.png
--rw-r--r--   0        0        0     7144 2022-11-14 15:08:03.802810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_bbbbbb_256x240.png
--rw-r--r--   0        0        0     7063 2022-11-14 15:08:03.810810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_ededed_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.813810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_ffcf29_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.814810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36800 2022-11-14 15:08:03.427809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/jquery-ui.css
--rw-r--r--   0        0        0    31457 2022-11-14 15:08:03.526809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/jquery-ui.min.css
--rw-r--r--   0        0        0    18133 2022-11-14 15:08:03.566809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/theme.css
--rw-r--r--   0        0        0      523 2022-11-14 15:08:03.756810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-bg_diagonals-thick_75_f3d8d8_40x40.png
--rw-r--r--   0        0        0      318 2022-11-14 15:08:03.760810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-bg_dots-small_65_a6a6a6_2x2.png
--rw-r--r--   0        0        0      450 2022-11-14 15:08:03.770810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-bg_glass_55_fbf8ee_1x400.png
--rw-r--r--   0        0        0      368 2022-11-14 15:08:03.778810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-bg_highlight-hard_100_eeeeee_1x100.png
--rw-r--r--   0        0        0      368 2022-11-14 15:08:03.778810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-bg_highlight-hard_100_f6f6f6_1x100.png
--rw-r--r--   0        0        0      437 2022-11-14 15:08:03.781810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-bg_highlight-soft_15_cc0000_1x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.787810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-icons_004276_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.806810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.814810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36693 2022-11-14 15:08:03.430809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/jquery-ui.css
--rw-r--r--   0        0        0    31359 2022-11-14 15:08:03.527809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/jquery-ui.min.css
--rw-r--r--   0        0        0    18026 2022-11-14 15:08:03.568809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/theme.css
--rw-r--r--   0        0        0      432 2022-11-14 15:08:03.757810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_diagonals-thick_90_eeeeee_40x40.png
--rw-r--r--   0        0        0      460 2022-11-14 15:08:03.765810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_glass_100_e4f1fb_1x400.png
--rw-r--r--   0        0        0      446 2022-11-14 15:08:03.769810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_glass_50_3baae3_1x400.png
--rw-r--r--   0        0        0      456 2022-11-14 15:08:03.772810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_glass_80_d7ebf9_1x400.png
--rw-r--r--   0        0        0      442 2022-11-14 15:08:03.778810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_highlight-hard_100_f2f5f7_1x100.png
--rw-r--r--   0        0        0      362 2022-11-14 15:08:03.780810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_highlight-hard_70_000000_1x100.png
--rw-r--r--   0        0        0      497 2022-11-14 15:08:03.780810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_highlight-soft_100_deedf7_1x100.png
--rw-r--r--   0        0        0      419 2022-11-14 15:08:03.782810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_highlight-soft_25_ffef8f_1x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.790810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_2694e8_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.791810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.791810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_3d80b3_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.796810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_72a7cf_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.814810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36850 2022-11-14 15:08:03.437809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/jquery-ui.css
--rw-r--r--   0        0        0    31543 2022-11-14 15:08:03.528809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/jquery-ui.min.css
--rw-r--r--   0        0        0    18183 2022-11-14 15:08:03.570809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/theme.css
--rw-r--r--   0        0        0      426 2022-11-14 15:08:03.768810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_glass_40_ffc73d_1x400.png
--rw-r--r--   0        0        0      433 2022-11-14 15:08:03.779810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_highlight-hard_20_0972a5_1x100.png
--rw-r--r--   0        0        0      453 2022-11-14 15:08:03.782810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_highlight-soft_33_003147_1x100.png
--rw-r--r--   0        0        0      394 2022-11-14 15:08:03.783810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_highlight-soft_35_222222_1x100.png
--rw-r--r--   0        0        0      380 2022-11-14 15:08:03.783810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_highlight-soft_44_444444_1x100.png
--rw-r--r--   0        0        0      387 2022-11-14 15:08:03.784810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_highlight-soft_80_eeeeee_1x100.png
--rw-r--r--   0        0        0      430 2022-11-14 15:08:03.787810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_loop_25_000000_21x21.png
--rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.789810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_222222_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.794810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_4b8e0b_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.800810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_a83300_256x240.png
--rw-r--r--   0        0        0     7086 2022-11-14 15:08:03.806810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_cccccc_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.815810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36796 2022-11-14 15:08:03.441809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/jquery-ui.css
--rw-r--r--   0        0        0    31444 2022-11-14 15:08:03.530809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/jquery-ui.min.css
--rw-r--r--   0        0        0    18129 2022-11-14 15:08:03.571809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/theme.css
--rw-r--r--   0        0        0      534 2022-11-14 15:08:03.755810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_diagonals-thick_15_0b3e6f_40x40.png
--rw-r--r--   0        0        0      347 2022-11-14 15:08:03.759810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_dots-medium_30_0b58a2_4x4.png
--rw-r--r--   0        0        0      318 2022-11-14 15:08:03.759810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_dots-small_20_333333_2x2.png
--rw-r--r--   0        0        0      328 2022-11-14 15:08:03.759810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_dots-small_30_a32d00_2x2.png
--rw-r--r--   0        0        0      334 2022-11-14 15:08:03.760810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_dots-small_40_00498f_2x2.png
--rw-r--r--   0        0        0     4042 2022-11-14 15:08:03.774810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_gloss-wave_20_111111_500x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.787810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-icons_00498f_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.799810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-icons_98d2fb_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.799810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-icons_9ccdfc_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.815810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36666 2022-11-14 15:08:03.451809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/jquery-ui.css
--rw-r--r--   0        0        0    31341 2022-11-14 15:08:03.531809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/jquery-ui.min.css
--rw-r--r--   0        0        0    17999 2022-11-14 15:08:03.572809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/theme.css
--rw-r--r--   0        0        0     6051 2022-11-14 15:08:03.774810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-bg_gloss-wave_30_3d3644_500x100.png
--rw-r--r--   0        0        0      452 2022-11-14 15:08:03.780810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-bg_highlight-soft_100_dcd9de_1x100.png
--rw-r--r--   0        0        0      483 2022-11-14 15:08:03.781810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-bg_highlight-soft_100_eae6ea_1x100.png
--rw-r--r--   0        0        0      472 2022-11-14 15:08:03.782810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-bg_highlight-soft_25_30273a_1x100.png
--rw-r--r--   0        0        0      457 2022-11-14 15:08:03.783810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-bg_highlight-soft_45_5f5964_1x100.png
--rw-r--r--   0        0        0     7142 2022-11-14 15:08:03.792810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_454545_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.796810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_734d99_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.799810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_8d78a5_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.800810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_a8a3ae_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.809810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_ebccce_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.815810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36720 2022-11-14 15:08:03.455809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/jquery-ui.css
--rw-r--r--   0        0        0    31404 2022-11-14 15:08:03.534809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/jquery-ui.min.css
--rw-r--r--   0        0        0    18053 2022-11-14 15:08:03.573809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/theme.css
--rw-r--r--   0        0        0      452 2022-11-14 15:08:03.753810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_diagonals-small_25_c5ddfc_40x40.png
--rw-r--r--   0        0        0      527 2022-11-14 15:08:03.755810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_diagonals-thick_20_e69700_40x40.png
--rw-r--r--   0        0        0      519 2022-11-14 15:08:03.756810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_diagonals-thick_22_1484e6_40x40.png
--rw-r--r--   0        0        0      516 2022-11-14 15:08:03.756810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_diagonals-thick_26_2293f7_40x40.png
--rw-r--r--   0        0        0      377 2022-11-14 15:08:03.781810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_highlight-soft_100_f9f9f9_1x100.png
--rw-r--r--   0        0        0      366 2022-11-14 15:08:03.785810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_inset-hard_100_eeeeee_1x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.788810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_0a82eb_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.788810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_0b54d5_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.795810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_5fa5e3_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.813810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_fcdd4a_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.815810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36824 2022-11-14 15:08:03.459809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/jquery-ui.css
--rw-r--r--   0        0        0    31486 2022-11-14 15:08:03.536809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/jquery-ui.min.css
--rw-r--r--   0        0        0    18157 2022-11-14 15:08:03.575809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/theme.css
--rw-r--r--   0        0        0      317 2022-11-14 15:08:03.771810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0        0        0      382 2022-11-14 15:08:03.781810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-bg_highlight-soft_100_f6f6f6_1x100.png
--rw-r--r--   0        0        0      445 2022-11-14 15:08:03.782810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-bg_highlight-soft_25_0073ea_1x100.png
--rw-r--r--   0        0        0      391 2022-11-14 15:08:03.783810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-bg_highlight-soft_50_dddddd_1x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.788810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_0073ea_256x240.png
--rw-r--r--   0        0        0     7142 2022-11-14 15:08:03.792810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_454545_256x240.png
--rw-r--r--   0        0        0     7163 2022-11-14 15:08:03.795810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_666666_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.813810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_ff0084_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.816810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36570 2022-11-14 15:08:03.462809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/flick/jquery-ui.css
--rw-r--r--   0        0        0    31215 2022-11-14 15:08:03.538809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/flick/jquery-ui.min.css
--rw-r--r--   0        0        0    17903 2022-11-14 15:08:03.575809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/flick/theme.css
--rw-r--r--   0        0        0      442 2022-11-14 15:08:03.754810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_diagonals-small_40_db4865_40x40.png
--rw-r--r--   0        0        0      443 2022-11-14 15:08:03.754810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_diagonals-small_50_93c3cd_40x40.png
--rw-r--r--   0        0        0      440 2022-11-14 15:08:03.754810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_diagonals-small_50_ff3853_40x40.png
--rw-r--r--   0        0        0      443 2022-11-14 15:08:03.754810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_diagonals-small_75_ccd232_40x40.png
--rw-r--r--   0        0        0      335 2022-11-14 15:08:03.759810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_dots-medium_80_ffff38_4x4.png
--rw-r--r--   0        0        0      333 2022-11-14 15:08:03.760810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_dots-small_35_35414f_2x2.png
--rw-r--r--   0        0        0      474 2022-11-14 15:08:03.787810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_white-lines_85_f7f7ba_40x100.png
--rw-r--r--   0        0        0     7142 2022-11-14 15:08:03.793810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_454545_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.798810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_88a206_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.804810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_c02669_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.808810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_e1e463_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.814810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_ffeb33_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.817810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36804 2022-11-14 15:08:03.466809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/jquery-ui.css
--rw-r--r--   0        0        0    31500 2022-11-14 15:08:03.540809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/jquery-ui.min.css
--rw-r--r--   0        0        0    18137 2022-11-14 15:08:03.576810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/theme.css
--rw-r--r--   0        0        0      464 2022-11-14 15:08:03.766810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_glass_100_f5f0e5_1x400.png
--rw-r--r--   0        0        0      445 2022-11-14 15:08:03.767810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_glass_25_cb842e_1x400.png
--rw-r--r--   0        0        0      464 2022-11-14 15:08:03.772810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_glass_70_ede4d4_1x400.png
--rw-r--r--   0        0        0      437 2022-11-14 15:08:03.778810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_highlight-hard_100_f4f0ec_1x100.png
--rw-r--r--   0        0        0      424 2022-11-14 15:08:03.780810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_highlight-hard_65_fee4bd_1x100.png
--rw-r--r--   0        0        0      433 2022-11-14 15:08:03.780810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_highlight-hard_75_f5f5b5_1x100.png
--rw-r--r--   0        0        0      513 2022-11-14 15:08:03.786810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_inset-soft_100_f4f0ec_1x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.805810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_c47a23_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.805810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_cb672b_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.810810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_f08000_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.811810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_f35f07_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.813810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_ff7519_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.817810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36789 2022-11-14 15:08:03.468809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/humanity/jquery-ui.css
--rw-r--r--   0        0        0    31503 2022-11-14 15:08:03.541809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/humanity/jquery-ui.min.css
--rw-r--r--   0        0        0    18122 2022-11-14 15:08:03.577809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/humanity/theme.css
--rw-r--r--   0        0        0      317 2022-11-14 15:08:03.752810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_diagonals-small_0_aaaaaa_40x40.png
--rw-r--r--   0        0        0      435 2022-11-14 15:08:03.755810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_diagonals-thick_15_444444_40x40.png
--rw-r--r--   0        0        0      521 2022-11-14 15:08:03.757810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_diagonals-thick_95_ffdc2e_40x40.png
--rw-r--r--   0        0        0      446 2022-11-14 15:08:03.770810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_glass_55_fbf5d0_1x400.png
--rw-r--r--   0        0        0      434 2022-11-14 15:08:03.779810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_highlight-hard_30_285c00_1x100.png
--rw-r--r--   0        0        0      455 2022-11-14 15:08:03.782810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_highlight-soft_33_3a8104_1x100.png
--rw-r--r--   0        0        0      461 2022-11-14 15:08:03.783810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_highlight-soft_50_4eb305_1x100.png
--rw-r--r--   0        0        0      469 2022-11-14 15:08:03.783810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_highlight-soft_60_4ca20b_1x100.png
--rw-r--r--   0        0        0      476 2022-11-14 15:08:03.786810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_inset-soft_10_285c00_1x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.794810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-icons_4eb305_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.796810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-icons_72b42d_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.807810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.817810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36964 2022-11-14 15:08:03.471809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/jquery-ui.css
--rw-r--r--   0        0        0    31647 2022-11-14 15:08:03.542809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/jquery-ui.min.css
--rw-r--r--   0        0        0    18297 2022-11-14 15:08:03.578809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/theme.css
--rw-r--r--   0        0        0      445 2022-11-14 15:08:03.767810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_glass_15_5f391b_1x400.png
--rw-r--r--   0        0        0     5903 2022-11-14 15:08:03.774810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_gloss-wave_20_1c160d_500x100.png
--rw-r--r--   0        0        0     5962 2022-11-14 15:08:03.774810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_gloss-wave_25_453326_500x100.png
--rw-r--r--   0        0        0     6024 2022-11-14 15:08:03.775810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_gloss-wave_30_44372c_500x100.png
--rw-r--r--   0        0        0      485 2022-11-14 15:08:03.781810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_highlight-soft_20_201913_1x100.png
--rw-r--r--   0        0        0      453 2022-11-14 15:08:03.782810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_highlight-soft_20_619226_1x100.png
--rw-r--r--   0        0        0      490 2022-11-14 15:08:03.786810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_inset-soft_10_201913_1x100.png
--rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.789810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_222222_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.799810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_9bcc60_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.800810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_add978_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.809810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_e3ddc9_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.811810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_f1fd86_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.817810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36822 2022-11-14 15:08:03.474809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/jquery-ui.css
--rw-r--r--   0        0        0    31521 2022-11-14 15:08:03.543809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/jquery-ui.min.css
--rw-r--r--   0        0        0    18155 2022-11-14 15:08:03.579810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/theme.css
--rw-r--r--   0        0        0      376 2022-11-14 15:08:03.766810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-bg_glass_100_f8f8f8_1x400.png
--rw-r--r--   0        0        0      375 2022-11-14 15:08:03.767810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-bg_glass_35_dddddd_1x400.png
--rw-r--r--   0        0        0      375 2022-11-14 15:08:03.771810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-bg_glass_60_eeeeee_1x400.png
--rw-r--r--   0        0        0      362 2022-11-14 15:08:03.785810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-bg_inset-hard_75_999999_1x100.png
--rw-r--r--   0        0        0      381 2022-11-14 15:08:03.787810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-bg_inset-soft_50_c9c9c9_1x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.791810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_3383bb_256x240.png
--rw-r--r--   0        0        0     7142 2022-11-14 15:08:03.793810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_454545_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.796810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_70b2e1_256x240.png
--rw-r--r--   0        0        0     7163 2022-11-14 15:08:03.799810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_999999_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.812810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_fbc856_256x240.png
--rw-r--r--   0        0        0    36646 2022-11-14 15:08:03.477809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/overcast/jquery-ui.css
--rw-r--r--   0        0        0    31288 2022-11-14 15:08:03.544809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/overcast/jquery-ui.min.css
--rw-r--r--   0        0        0    17979 2022-11-14 15:08:03.579810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/overcast/theme.css
--rw-r--r--   0        0        0      406 2022-11-14 15:08:03.752810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_diagonal-maze_20_6e4f1c_10x10.png
--rw-r--r--   0        0        0      353 2022-11-14 15:08:03.752810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_diagonal-maze_40_000000_10x10.png
--rw-r--r--   0        0        0    10869 2022-11-14 15:08:03.760810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_10_eceadf_60x60.png
--rw-r--r--   0        0        0    10014 2022-11-14 15:08:03.762810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_10_f8f7f6_60x60.png
--rw-r--r--   0        0        0    10639 2022-11-14 15:08:03.763810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_15_eceadf_60x60.png
--rw-r--r--   0        0        0    11001 2022-11-14 15:08:03.764810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_15_f7f3de_60x60.png
--rw-r--r--   0        0        0     4314 2022-11-14 15:08:03.764810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_15_ffffff_60x60.png
--rw-r--r--   0        0        0    14555 2022-11-14 15:08:03.764810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_65_654b24_60x60.png
--rw-r--r--   0        0        0    11987 2022-11-14 15:08:03.764810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_68_b83400_60x60.png
--rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.789810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_222222_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.791810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_3572ac_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.798810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_8c291d_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.802810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_b83400_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.812810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_fbdb93_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.817810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36906 2022-11-14 15:08:03.480809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/jquery-ui.css
--rw-r--r--   0        0        0    31611 2022-11-14 15:08:03.545809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/jquery-ui.min.css
--rw-r--r--   0        0        0    18239 2022-11-14 15:08:03.580809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/theme.css
--rw-r--r--   0        0        0      446 2022-11-14 15:08:03.772810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-bg_glass_75_d0e5f5_1x400.png
--rw-r--r--   0        0        0      451 2022-11-14 15:08:03.773810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-bg_glass_85_dfeffc_1x400.png
--rw-r--r--   0        0        0      442 2022-11-14 15:08:03.773810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0        0        0     5934 2022-11-14 15:08:03.776810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-bg_gloss-wave_55_5c9ccc_500x100.png
--rw-r--r--   0        0        0      443 2022-11-14 15:08:03.785810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-bg_inset-hard_100_f5f8f9_1x100.png
--rw-r--r--   0        0        0      402 2022-11-14 15:08:03.785810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-bg_inset-hard_100_fcfdfd_1x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.789810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_217bc0_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.791810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.794810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_469bdd_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.796810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_6da8d5_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.807810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.808810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_d8e7f3_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.812810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_f9bd01_256x240.png
--rw-r--r--   0        0        0    36735 2022-11-14 15:08:03.482809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/redmond/jquery-ui.css
--rw-r--r--   0        0        0    31443 2022-11-14 15:08:03.547809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/redmond/jquery-ui.min.css
--rw-r--r--   0        0        0    18068 2022-11-14 15:08:03.581809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/redmond/theme.css
--rw-r--r--   0        0        0      445 2022-11-14 15:08:03.770810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0        0        0      317 2022-11-14 15:08:03.771810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0        0        0      375 2022-11-14 15:08:03.772810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0        0        0      376 2022-11-14 15:08:03.772810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0        0        0      442 2022-11-14 15:08:03.773810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0        0        0      377 2022-11-14 15:08:03.784810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.790810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_222222_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.791810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0        0        0     7142 2022-11-14 15:08:03.794810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_454545_256x240.png
--rw-r--r--   0        0        0     7163 2022-11-14 15:08:03.798810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_888888_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.807810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0        0        0    36662 2022-11-14 15:08:03.486809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/jquery-ui.css
--rw-r--r--   0        0        0    31340 2022-11-14 15:08:03.548809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/jquery-ui.min.css
--rw-r--r--   0        0        0    17995 2022-11-14 15:08:03.582810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/theme.css
--rw-r--r--   0        0        0      443 2022-11-14 15:08:03.771810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_glass_55_fcf0ba_1x400.png
--rw-r--r--   0        0        0     5869 2022-11-14 15:08:03.773810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_gloss-wave_100_ece8da_500x100.png
--rw-r--r--   0        0        0      446 2022-11-14 15:08:03.778810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_highlight-hard_100_f5f3e5_1x100.png
--rw-r--r--   0        0        0      431 2022-11-14 15:08:03.779810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_highlight-hard_100_fafaf4_1x100.png
--rw-r--r--   0        0        0      432 2022-11-14 15:08:03.779810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_highlight-hard_15_459e00_1x100.png
--rw-r--r--   0        0        0      369 2022-11-14 15:08:03.780810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_highlight-hard_95_cccccc_1x100.png
--rw-r--r--   0        0        0      463 2022-11-14 15:08:03.782810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_highlight-soft_25_67b021_1x100.png
--rw-r--r--   0        0        0      461 2022-11-14 15:08:03.784810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_highlight-soft_95_ffedad_1x100.png
--rw-r--r--   0        0        0      432 2022-11-14 15:08:03.786810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_inset-soft_15_2b2922_1x100.png
--rw-r--r--   0        0        0     7169 2022-11-14 15:08:03.798810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_808080_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.798810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_847e71_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.799810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_8DC262_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.807810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0        0        0     7062 2022-11-14 15:08:03.810810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_eeeeee_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.818810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36912 2022-11-14 15:08:03.489809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/south-street/jquery-ui.css
--rw-r--r--   0        0        0    31623 2022-11-14 15:08:03.549809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/south-street/jquery-ui.min.css
--rw-r--r--   0        0        0    18245 2022-11-14 15:08:03.583809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/south-street/theme.css
--rw-r--r--   0        0        0      455 2022-11-14 15:08:03.769810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_glass_45_0078ae_1x400.png
--rw-r--r--   0        0        0      455 2022-11-14 15:08:03.770810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_glass_55_f8da4e_1x400.png
--rw-r--r--   0        0        0      458 2022-11-14 15:08:03.772810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_glass_75_79c9ec_1x400.png
--rw-r--r--   0        0        0     5974 2022-11-14 15:08:03.775810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_gloss-wave_45_e14f1c_500x100.png
--rw-r--r--   0        0        0     6016 2022-11-14 15:08:03.776810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_gloss-wave_50_6eac2c_500x100.png
--rw-r--r--   0        0        0     6087 2022-11-14 15:08:03.777810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_gloss-wave_75_2191c0_500x100.png
--rw-r--r--   0        0        0      402 2022-11-14 15:08:03.785810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_inset-hard_100_fcfdfd_1x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.788810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_0078ae_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.788810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_056b93_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.808810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_d8e7f3_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.808810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_e0fdff_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.811810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_f5e175_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.811810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_f7a50d_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.812810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_fcd113_256x240.png
--rw-r--r--   0        0        0    36755 2022-11-14 15:08:03.493809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/start/jquery-ui.css
--rw-r--r--   0        0        0    31441 2022-11-14 15:08:03.550809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/start/jquery-ui.min.css
--rw-r--r--   0        0        0    18088 2022-11-14 15:08:03.584809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/start/theme.css
--rw-r--r--   0        0        0      492 2022-11-14 15:08:03.752810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_diagonals-medium_20_d34d17_40x40.png
--rw-r--r--   0        0        0     6000 2022-11-14 15:08:03.775810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_gloss-wave_45_817865_500x100.png
--rw-r--r--   0        0        0     5960 2022-11-14 15:08:03.777810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_gloss-wave_60_fece2f_500x100.png
--rw-r--r--   0        0        0     5653 2022-11-14 15:08:03.777810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_gloss-wave_70_ffdd57_500x100.png
--rw-r--r--   0        0        0     5499 2022-11-14 15:08:03.777810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_gloss-wave_90_fff9e5_500x100.png
--rw-r--r--   0        0        0      453 2022-11-14 15:08:03.781810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_highlight-soft_100_feeebd_1x100.png
--rw-r--r--   0        0        0      313 2022-11-14 15:08:03.787810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_inset-soft_30_ffffff_1x100.png
--rw-r--r--   0        0        0     7126 2022-11-14 15:08:03.791810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_3d3d3d_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.804810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_bd7b00_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.808810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_d19405_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.809810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_eb990f_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.810810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_ed9f26_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.812810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_fadc7a_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.814810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_ffe180_256x240.png
--rw-r--r--   0        0        0    36805 2022-11-14 15:08:03.498809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/sunny/jquery-ui.css
--rw-r--r--   0        0        0    31510 2022-11-14 15:08:03.550809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/sunny/jquery-ui.min.css
--rw-r--r--   0        0        0    18138 2022-11-14 15:08:03.585809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/sunny/theme.css
--rw-r--r--   0        0        0      417 2022-11-14 15:08:03.757810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_diamond_10_4f4221_10x8.png
--rw-r--r--   0        0        0      420 2022-11-14 15:08:03.758810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_diamond_20_372806_10x8.png
--rw-r--r--   0        0        0      422 2022-11-14 15:08:03.758810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_diamond_25_675423_10x8.png
--rw-r--r--   0        0        0      423 2022-11-14 15:08:03.758810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_diamond_25_d5ac5d_10x8.png
--rw-r--r--   0        0        0      420 2022-11-14 15:08:03.758810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_diamond_8_261803_10x8.png
--rw-r--r--   0        0        0      420 2022-11-14 15:08:03.758810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_diamond_8_443113_10x8.png
--rw-r--r--   0        0        0      424 2022-11-14 15:08:03.780810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_highlight-hard_65_fee4bd_1x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.788810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_070603_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.809810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_e8e2b5_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.809810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_e9cd86_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.810810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_efec9f_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.811810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_f2ec64_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.812810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_f9f2bd_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.813810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_ff7519_256x240.png
--rw-r--r--   0        0        0    36812 2022-11-14 15:08:03.504809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/jquery-ui.css
--rw-r--r--   0        0        0    31541 2022-11-14 15:08:03.551809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/jquery-ui.min.css
--rw-r--r--   0        0        0    18145 2022-11-14 15:08:03.586809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/theme.css
--rw-r--r--   0        0        0      373 2022-11-14 15:08:03.754810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_diagonals-small_50_262626_40x40.png
--rw-r--r--   0        0        0      374 2022-11-14 15:08:03.768810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_glass_40_0a0a0a_1x400.png
--rw-r--r--   0        0        0      458 2022-11-14 15:08:03.770810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_glass_55_f1fbe5_1x400.png
--rw-r--r--   0        0        0      375 2022-11-14 15:08:03.771810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_glass_60_000000_1x400.png
--rw-r--r--   0        0        0     4412 2022-11-14 15:08:03.776810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_gloss-wave_55_000000_500x100.png
--rw-r--r--   0        0        0     6050 2022-11-14 15:08:03.777810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_gloss-wave_85_9fda58_500x100.png
--rw-r--r--   0        0        0     5908 2022-11-14 15:08:03.778810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_gloss-wave_95_f6ecd5_500x100.png
--rw-r--r--   0        0        0     5634 2022-11-14 15:08:03.787810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_000000_256x240.png
--rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.789810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_1f1f1f_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.800810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_9fda58_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.802810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_b8ec79_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.807810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.818810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36792 2022-11-14 15:08:03.513809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/jquery-ui.css
--rw-r--r--   0        0        0    31488 2022-11-14 15:08:03.552809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/jquery-ui.min.css
--rw-r--r--   0        0        0    18125 2022-11-14 15:08:03.587809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/theme.css
--rw-r--r--   0        0        0      370 2022-11-14 15:08:03.767810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_glass_20_555555_1x400.png
--rw-r--r--   0        0        0      452 2022-11-14 15:08:03.767810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_glass_40_0078a3_1x400.png
--rw-r--r--   0        0        0      426 2022-11-14 15:08:03.768810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_glass_40_ffc73d_1x400.png
--rw-r--r--   0        0        0     4028 2022-11-14 15:08:03.774810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_gloss-wave_25_333333_500x100.png
--rw-r--r--   0        0        0      387 2022-11-14 15:08:03.784810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_highlight-soft_80_eeeeee_1x100.png
--rw-r--r--   0        0        0      364 2022-11-14 15:08:03.786810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_inset-soft_25_000000_1x100.png
--rw-r--r--   0        0        0      450 2022-11-14 15:08:03.786810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_inset-soft_30_f58400_1x100.png
--rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.790810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_222222_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.794810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_4b8e0b_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.800810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_a83300_256x240.png
--rw-r--r--   0        0        0     7086 2022-11-14 15:08:03.806810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_cccccc_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.818810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36760 2022-11-14 15:08:03.517809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/jquery-ui.css
--rw-r--r--   0        0        0    31408 2022-11-14 15:08:03.555809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/jquery-ui.min.css
--rw-r--r--   0        0        0    18093 2022-11-14 15:08:03.588809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/theme.css
--rw-r--r--   0        0        0      528 2022-11-14 15:08:03.755810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_diagonals-thick_18_b81900_40x40.png
--rw-r--r--   0        0        0      436 2022-11-14 15:08:03.755810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_diagonals-thick_20_666666_40x40.png
--rw-r--r--   0        0        0      376 2022-11-14 15:08:03.766810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_glass_100_f6f6f6_1x400.png
--rw-r--r--   0        0        0      458 2022-11-14 15:08:03.766810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_glass_100_fdf5ce_1x400.png
--rw-r--r--   0        0        0      317 2022-11-14 15:08:03.771810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0        0        0     5925 2022-11-14 15:08:03.775810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_gloss-wave_35_f6a828_500x100.png
--rw-r--r--   0        0        0      394 2022-11-14 15:08:03.781810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_highlight-soft_100_eeeeee_1x100.png
--rw-r--r--   0        0        0      438 2022-11-14 15:08:03.784810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_highlight-soft_75_ffe45c_1x100.png
--rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.790810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_222222_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.790810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_228ef1_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.810810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_ef8c08_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.813810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_ffd27a_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.819810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36922 2022-11-14 15:08:03.520809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/jquery-ui.css
--rw-r--r--   0        0        0    31606 2022-11-14 15:08:03.556809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/jquery-ui.min.css
--rw-r--r--   0        0        0    18255 2022-11-14 15:08:03.588809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/theme.css
--rw-r--r--   0        0        0      442 2022-11-14 15:08:03.773810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0        0        0     4083 2022-11-14 15:08:03.774810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_gloss-wave_16_121212_500x100.png
--rw-r--r--   0        0        0      363 2022-11-14 15:08:03.779810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_highlight-hard_15_888888_1x100.png
--rw-r--r--   0        0        0      363 2022-11-14 15:08:03.779810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_highlight-hard_55_555555_1x100.png
--rw-r--r--   0        0        0      378 2022-11-14 15:08:03.783810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_highlight-soft_35_adadad_1x100.png
--rw-r--r--   0        0        0      394 2022-11-14 15:08:03.784810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_highlight-soft_60_dddddd_1x100.png
--rw-r--r--   0        0        0      374 2022-11-14 15:08:03.786810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_inset-soft_15_121212_1x100.png
--rw-r--r--   0        0        0     7163 2022-11-14 15:08:03.795810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_666666_256x240.png
--rw-r--r--   0        0        0     7163 2022-11-14 15:08:03.797810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_777777_256x240.png
--rw-r--r--   0        0        0     7127 2022-11-14 15:08:03.800810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_aaaaaa_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.805810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_c98000_256x240.png
--rw-r--r--   0        0        0     7086 2022-11-14 15:08:03.806810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_cccccc_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.808810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.811810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_f29a00_256x240.png
--rw-r--r--   0        0        0    36802 2022-11-14 15:08:03.524809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/vader/jquery-ui.css
--rw-r--r--   0        0        0    31448 2022-11-14 15:08:03.557809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/vader/jquery-ui.min.css
--rw-r--r--   0        0        0    18135 2022-11-14 15:08:03.589810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/dist/themes/vader/theme.css
--rw-r--r--   0        0        0     1095 2022-11-14 15:08:03.410809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/globalize/LICENSE
--rw-r--r--   0        0        0     1898 2022-11-14 15:08:03.633810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/globalize/globalize.culture.de-DE.js
--rw-r--r--   0        0        0     2859 2022-11-14 15:08:03.633810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/globalize/globalize.culture.ja-JP.js
--rw-r--r--   0        0        0    45705 2022-11-14 15:08:03.633810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/globalize/globalize.js
--rw-r--r--   0        0        0     1097 2022-11-14 15:08:03.823810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery/LICENSE.txt
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery/MIT-LICENSE.txt
--rw-r--r--   0        0        0   288580 2022-11-14 15:08:03.741810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.824810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.10.0/MIT-LICENSE.txt
--rw-r--r--   0        0        0   273809 2022-11-14 15:08:03.644810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.10.0/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.824810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.10.1/MIT-LICENSE.txt
--rw-r--r--   0        0        0   274080 2022-11-14 15:08:03.650810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.10.1/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.824810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.10.2/MIT-LICENSE.txt
--rw-r--r--   0        0        0   273199 2022-11-14 15:08:03.655810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.10.2/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.11.0/MIT-LICENSE.txt
--rw-r--r--   0        0        0   282944 2022-11-14 15:08:03.658810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.11.0/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.11.1/MIT-LICENSE.txt
--rw-r--r--   0        0        0   282766 2022-11-14 15:08:03.662810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.11.1/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.11.2/MIT-LICENSE.txt
--rw-r--r--   0        0        0   284184 2022-11-14 15:08:03.666810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.11.2/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.11.3/MIT-LICENSE.txt
--rw-r--r--   0        0        0   284394 2022-11-14 15:08:03.671810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.11.3/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.819810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.12.0/LICENSE.txt
--rw-r--r--   0        0        0   294161 2022-11-14 15:08:03.688810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.12.0/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.819810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.12.1/LICENSE.txt
--rw-r--r--   0        0        0   294199 2022-11-14 15:08:03.693810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.12.1/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.820810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.12.2/LICENSE.txt
--rw-r--r--   0        0        0   293840 2022-11-14 15:08:03.700810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.12.2/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.820810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.12.3/LICENSE.txt
--rw-r--r--   0        0        0   293650 2022-11-14 15:08:03.702810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.12.3/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.820810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.12.4/LICENSE.txt
--rw-r--r--   0        0        0   293430 2022-11-14 15:08:03.705810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.12.4/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.8.0/MIT-LICENSE.txt
--rw-r--r--   0        0        0   258377 2022-11-14 15:08:03.706810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.8.0/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.8.1/MIT-LICENSE.txt
--rw-r--r--   0        0        0   259996 2022-11-14 15:08:03.707810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.8.1/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.8.2/MIT-LICENSE.txt
--rw-r--r--   0        0        0   265217 2022-11-14 15:08:03.707810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.8.2/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.8.3/MIT-LICENSE.txt
--rw-r--r--   0        0        0   418275 2022-11-14 15:08:03.709810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.8.3/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.9.0/MIT-LICENSE.txt
--rw-r--r--   0        0        0   267320 2022-11-14 15:08:03.710810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.9.0/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.9.1/MIT-LICENSE.txt
--rw-r--r--   0        0        0   268380 2022-11-14 15:08:03.711810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-1.9.1/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.0.0/MIT-LICENSE.txt
--rw-r--r--   0        0        0   240196 2022-11-14 15:08:03.711810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.0.0/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.0.1/MIT-LICENSE.txt
--rw-r--r--   0        0        0   242727 2022-11-14 15:08:03.712810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.0.1/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.0.2/MIT-LICENSE.txt
--rw-r--r--   0        0        0   242915 2022-11-14 15:08:03.713810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.0.2/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.0.3/MIT-LICENSE.txt
--rw-r--r--   0        0        0   242142 2022-11-14 15:08:03.714810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.0.3/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.1.0/MIT-LICENSE.txt
--rw-r--r--   0        0        0   244963 2022-11-14 15:08:03.715810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.1.0/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.1.1/MIT-LICENSE.txt
--rw-r--r--   0        0        0   247351 2022-11-14 15:08:03.715810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.1.1/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.1.2/MIT-LICENSE.txt
--rw-r--r--   0        0        0   247380 2022-11-14 15:08:03.716810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.1.2/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.1.3/MIT-LICENSE.txt
--rw-r--r--   0        0        0   247387 2022-11-14 15:08:03.717810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.1.3/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.1.4/MIT-LICENSE.txt
--rw-r--r--   0        0        0   247597 2022-11-14 15:08:03.718810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.1.4/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.820810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.2.0/LICENSE.txt
--rw-r--r--   0        0        0   258388 2022-11-14 15:08:03.719810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.2.0/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.820810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.2.1/LICENSE.txt
--rw-r--r--   0        0        0   258549 2022-11-14 15:08:03.720810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.2.1/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.820810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.2.2/LICENSE.txt
--rw-r--r--   0        0        0   258648 2022-11-14 15:08:03.721810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.2.2/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.821810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.2.3/LICENSE.txt
--rw-r--r--   0        0        0   258648 2022-11-14 15:08:03.722810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.2.3/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.821810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.2.4/LICENSE.txt
--rw-r--r--   0        0        0   257551 2022-11-14 15:08:03.723810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-2.2.4/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.821810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.0.0/LICENSE.txt
--rw-r--r--   0        0        0   263268 2022-11-14 15:08:03.723810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.0.0/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.821810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.1.0/LICENSE.txt
--rw-r--r--   0        0        0   263767 2022-11-14 15:08:03.724810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.1.0/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.821810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.1.1/LICENSE.txt
--rw-r--r--   0        0        0   267194 2022-11-14 15:08:03.725810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.1.1/jquery.js
--rw-r--r--   0        0        0     1605 2022-11-14 15:08:03.821810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.2.0/LICENSE.txt
--rw-r--r--   0        0        0   267686 2022-11-14 15:08:03.726810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.2.0/jquery.js
--rw-r--r--   0        0        0     1605 2022-11-14 15:08:03.821810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.2.1/LICENSE.txt
--rw-r--r--   0        0        0   268039 2022-11-14 15:08:03.727810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.2.1/jquery.js
--rw-r--r--   0        0        0     1605 2022-11-14 15:08:03.822810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.3.0/LICENSE.txt
--rw-r--r--   0        0        0   271751 2022-11-14 15:08:03.728810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.3.0/jquery.js
--rw-r--r--   0        0        0     1605 2022-11-14 15:08:03.822810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.3.1/LICENSE.txt
--rw-r--r--   0        0        0   271751 2022-11-14 15:08:03.728810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.3.1/jquery.js
--rw-r--r--   0        0        0     1095 2022-11-14 15:08:03.822810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.4.0/LICENSE.txt
--rw-r--r--   0        0        0   279860 2022-11-14 15:08:03.729810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.4.0/jquery.js
--rw-r--r--   0        0        0     1095 2022-11-14 15:08:03.822810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.4.1/LICENSE.txt
--rw-r--r--   0        0        0   280364 2022-11-14 15:08:03.730810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.4.1/jquery.js
--rw-r--r--   0        0        0     1095 2022-11-14 15:08:03.822810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.5.0/LICENSE.txt
--rw-r--r--   0        0        0   287649 2022-11-14 15:08:03.734810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.5.0/jquery.js
--rw-r--r--   0        0        0     1095 2022-11-14 15:08:03.822810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.5.1/LICENSE.txt
--rw-r--r--   0        0        0   287630 2022-11-14 15:08:03.735810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.5.1/jquery.js
--rw-r--r--   0        0        0     1097 2022-11-14 15:08:03.822810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.6.0/LICENSE.txt
--rw-r--r--   0        0        0   288580 2022-11-14 15:08:03.737810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-3.6.0/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-custom/MIT-LICENSE.txt
--rw-r--r--   0        0        0   283248 2022-11-14 15:08:03.739810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-custom/jquery.js
--rw-r--r--   0        0        0     1614 2022-11-14 15:08:03.822810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-migrate-1.4.1/LICENSE.txt
--rw-r--r--   0        0        0    23497 2022-11-14 15:08:03.634810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-migrate-1.4.1/jquery-migrate.js
--rw-r--r--   0        0        0     1615 2022-11-14 15:08:03.823810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-migrate-3.3.2/LICENSE.txt
--rw-r--r--   0        0        0    25300 2022-11-14 15:08:03.635810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-migrate-3.3.2/jquery-migrate.js
--rw-r--r--   0        0        0     1084 2022-11-14 15:08:03.823810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-mousewheel/LICENSE.txt
--rw-r--r--   0        0        0     8279 2022-11-14 15:08:03.741810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-mousewheel/jquery.mousewheel.js
--rw-r--r--   0        0        0     1615 2022-11-14 15:08:03.823810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-simulate/LICENSE.txt
--rw-r--r--   0        0        0     8710 2022-11-14 15:08:03.742810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/jquery-simulate/jquery.simulate.js
--rw-r--r--   0        0        0     1590 2022-11-14 15:08:03.824810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/qunit/LICENSE.txt
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.828810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/qunit/MIT-LICENSE.txt
--rw-r--r--   0        0        0     5146 2022-11-14 15:08:03.560809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/qunit/qunit.css
--rw-r--r--   0        0        0   115758 2022-11-14 15:08:03.746810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/qunit/qunit.js
--rw-r--r--   0        0        0     1085 2022-11-14 15:08:03.823810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/qunit-assert-classes/LICENSE.txt
--rw-r--r--   0        0        0     5295 2022-11-14 15:08:03.744810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/qunit-assert-classes/qunit-assert-classes.js
--rw-r--r--   0        0        0     1094 2022-11-14 15:08:03.828810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/qunit-assert-close/MIT-LICENSE.txt
--rw-r--r--   0        0        0     4181 2022-11-14 15:08:03.745810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/qunit-assert-close/qunit-assert-close.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.823810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/qunit-composite/LICENSE.txt
--rw-r--r--   0        0        0      196 2022-11-14 15:08:03.559809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/qunit-composite/qunit-composite.css
--rw-r--r--   0        0        0     4768 2022-11-14 15:08:03.745810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/qunit-composite/qunit-composite.js
--rw-r--r--   0        0        0    83083 2022-11-14 15:08:03.746810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/external/requirejs/require.js
--rw-r--r--   0        0        0     1812 2022-11-14 15:08:03.751810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/package.json
--rw-r--r--   0        0        0      489 2022-11-14 15:08:03.414809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/accordion.css
--rw-r--r--   0        0        0      275 2022-11-14 15:08:03.415809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/all.css
--rw-r--r--   0        0        0      316 2022-11-14 15:08:03.415809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/autocomplete.css
--rw-r--r--   0        0        0      791 2022-11-14 15:08:03.417809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/base.css
--rw-r--r--   0        0        0     1497 2022-11-14 15:08:03.417809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/button.css
--rw-r--r--   0        0        0      789 2022-11-14 15:08:03.418809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/checkboxradio.css
--rw-r--r--   0        0        0     1526 2022-11-14 15:08:03.419809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/controlgroup.css
--rw-r--r--   0        0        0     1581 2022-11-14 15:08:03.419809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/core.css
--rw-r--r--   0        0        0     3788 2022-11-14 15:08:03.420809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/datepicker.css
--rw-r--r--   0        0        0     1753 2022-11-14 15:08:03.420809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/dialog.css
--rw-r--r--   0        0        0      253 2022-11-14 15:08:03.421809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/draggable.css
--rw-r--r--   0        0        0       86 2022-11-14 15:08:03.765810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-r--r--   0        0        0     3266 2022-11-14 15:08:03.792810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_444444_256x240.png
--rw-r--r--   0        0        0     3274 2022-11-14 15:08:03.795810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_555555_256x240.png
--rw-r--r--   0        0        0     3262 2022-11-14 15:08:03.797810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_777620_256x240.png
--rw-r--r--   0        0        0     3266 2022-11-14 15:08:03.797810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_777777_256x240.png
--rw-r--r--   0        0        0     3262 2022-11-14 15:08:03.806810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0        0        0     3264 2022-11-14 15:08:03.819810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0     1124 2022-11-14 15:08:03.557809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/menu.css
--rw-r--r--   0        0        0     2952 2022-11-14 15:08:03.558809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/progressbar.css
--rw-r--r--   0        0        0     1198 2022-11-14 15:08:03.561809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/resizable.css
--rw-r--r--   0        0        0      337 2022-11-14 15:08:03.562809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/selectable.css
--rw-r--r--   0        0        0      916 2022-11-14 15:08:03.563809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/selectmenu.css
--rw-r--r--   0        0        0     1359 2022-11-14 15:08:03.563809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/slider.css
--rw-r--r--   0        0        0      251 2022-11-14 15:08:03.564809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/sortable.css
--rw-r--r--   0        0        0      964 2022-11-14 15:08:03.564809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/spinner.css
--rw-r--r--   0        0        0     1217 2022-11-14 15:08:03.565809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/tabs.css
--rw-r--r--   0        0        0    18128 2022-11-14 15:08:03.590809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/theme.css
--rw-r--r--   0        0        0      355 2022-11-14 15:08:03.591809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/themes/base/tooltip.css
--rw-r--r--   0        0        0      361 2022-11-14 15:08:03.596809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/core.js
--rw-r--r--   0        0        0      934 2022-11-14 15:08:03.597809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/data.js
--rw-r--r--   0        0        0     1079 2022-11-14 15:08:03.623810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/disable-selection.js
--rw-r--r--   0        0        0    24612 2022-11-14 15:08:03.629810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/effect.js
--rw-r--r--   0        0        0     1640 2022-11-14 15:08:03.624810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/effects/effect-blind.js
--rw-r--r--   0        0        0     2656 2022-11-14 15:08:03.624810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/effects/effect-bounce.js
--rw-r--r--   0        0        0     1573 2022-11-14 15:08:03.625810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/effects/effect-clip.js
--rw-r--r--   0        0        0     1591 2022-11-14 15:08:03.625810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/effects/effect-drop.js
--rw-r--r--   0        0        0     2920 2022-11-14 15:08:03.625810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/effects/effect-explode.js
--rw-r--r--   0        0        0      964 2022-11-14 15:08:03.625810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/effects/effect-fade.js
--rw-r--r--   0        0        0     2181 2022-11-14 15:08:03.625810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/effects/effect-fold.js
--rw-r--r--   0        0        0     1239 2022-11-14 15:08:03.626810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/effects/effect-highlight.js
--rw-r--r--   0        0        0      991 2022-11-14 15:08:03.626810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/effects/effect-puff.js
--rw-r--r--   0        0        0     1563 2022-11-14 15:08:03.626810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/effects/effect-pulsate.js
--rw-r--r--   0        0        0     1369 2022-11-14 15:08:03.626810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/effects/effect-scale.js
--rw-r--r--   0        0        0     1880 2022-11-14 15:08:03.628810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/effects/effect-shake.js
--rw-r--r--   0        0        0     5414 2022-11-14 15:08:03.628810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/effects/effect-size.js
--rw-r--r--   0        0        0     1963 2022-11-14 15:08:03.628810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/effects/effect-slide.js
--rw-r--r--   0        0        0      884 2022-11-14 15:08:03.628810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/effects/effect-transfer.js
--rw-r--r--   0        0        0     2295 2022-11-14 15:08:03.629810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/focusable.js
--rw-r--r--   0        0        0     1827 2022-11-14 15:08:03.629810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/form-reset-mixin.js
--rw-r--r--   0        0        0      581 2022-11-14 15:08:03.629810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/form.js
--rw-r--r--   0        0        0     1207 2022-11-14 15:08:03.597809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-af.js
--rw-r--r--   0        0        0     1532 2022-11-14 15:08:03.597809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ar-DZ.js
--rw-r--r--   0        0        0     1499 2022-11-14 15:08:03.598810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ar.js
--rw-r--r--   0        0        0     1241 2022-11-14 15:08:03.598810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-az.js
--rw-r--r--   0        0        0     1467 2022-11-14 15:08:03.598810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-be.js
--rw-r--r--   0        0        0     1444 2022-11-14 15:08:03.599810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-bg.js
--rw-r--r--   0        0        0     1183 2022-11-14 15:08:03.599810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-bs.js
--rw-r--r--   0        0        0     1207 2022-11-14 15:08:03.599810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ca.js
--rw-r--r--   0        0        0     1232 2022-11-14 15:08:03.599810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-cs.js
--rw-r--r--   0        0        0     1248 2022-11-14 15:08:03.599810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-cy-GB.js
--rw-r--r--   0        0        0     1212 2022-11-14 15:08:03.600809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-da.js
--rw-r--r--   0        0        0     1227 2022-11-14 15:08:03.600809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-de-AT.js
--rw-r--r--   0        0        0     1202 2022-11-14 15:08:03.600809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-de.js
--rw-r--r--   0        0        0     1521 2022-11-14 15:08:03.600809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-el.js
--rw-r--r--   0        0        0     1226 2022-11-14 15:08:03.600809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-en-AU.js
--rw-r--r--   0        0        0     1203 2022-11-14 15:08:03.601810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-en-GB.js
--rw-r--r--   0        0        0     1228 2022-11-14 15:08:03.601810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-en-NZ.js
--rw-r--r--   0        0        0     1214 2022-11-14 15:08:03.601810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-eo.js
--rw-r--r--   0        0        0     1209 2022-11-14 15:08:03.601810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-es.js
--rw-r--r--   0        0        0     1277 2022-11-14 15:08:03.601810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-et.js
--rw-r--r--   0        0        0     1164 2022-11-14 15:08:03.601810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-eu.js
--rw-r--r--   0        0        0     1420 2022-11-14 15:08:03.602810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fa.js
--rw-r--r--   0        0        0     1266 2022-11-14 15:08:03.602810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fi.js
--rw-r--r--   0        0        0     1254 2022-11-14 15:08:03.602810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fo.js
--rw-r--r--   0        0        0     1221 2022-11-14 15:08:03.602810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fr-CA.js
--rw-r--r--   0        0        0     1258 2022-11-14 15:08:03.603809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fr-CH.js
--rw-r--r--   0        0        0     1341 2022-11-14 15:08:03.604810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fr.js
--rw-r--r--   0        0        0     1211 2022-11-14 15:08:03.604810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-gl.js
--rw-r--r--   0        0        0     1325 2022-11-14 15:08:03.604810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-he.js
--rw-r--r--   0        0        0     1618 2022-11-14 15:08:03.604810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-hi.js
--rw-r--r--   0        0        0     1208 2022-11-14 15:08:03.604810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-hr.js
--rw-r--r--   0        0        0     1187 2022-11-14 15:08:03.605810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-hu.js
--rw-r--r--   0        0        0     1495 2022-11-14 15:08:03.605810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-hy.js
--rw-r--r--   0        0        0     1266 2022-11-14 15:08:03.605810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-id.js
--rw-r--r--   0        0        0     1281 2022-11-14 15:08:03.605810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-is.js
--rw-r--r--   0        0        0     1257 2022-11-14 15:08:03.605810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-it-CH.js
--rw-r--r--   0        0        0     1233 2022-11-14 15:08:03.606809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-it.js
--rw-r--r--   0        0        0     1223 2022-11-14 15:08:03.606809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ja.js
--rw-r--r--   0        0        0     1761 2022-11-14 15:08:03.606809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ka.js
--rw-r--r--   0        0        0     1438 2022-11-14 15:08:03.606809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-kk.js
--rw-r--r--   0        0        0     1645 2022-11-14 15:08:03.608810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-km.js
--rw-r--r--   0        0        0     1264 2022-11-14 15:08:03.609809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ko.js
--rw-r--r--   0        0        0     1416 2022-11-14 15:08:03.609809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ky.js
--rw-r--r--   0        0        0     1260 2022-11-14 15:08:03.609809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-lb.js
--rw-r--r--   0        0        0     1297 2022-11-14 15:08:03.609809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-lt.js
--rw-r--r--   0        0        0     1290 2022-11-14 15:08:03.610809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-lv.js
--rw-r--r--   0        0        0     1408 2022-11-14 15:08:03.610809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-mk.js
--rw-r--r--   0        0        0     1747 2022-11-14 15:08:03.610809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ml.js
--rw-r--r--   0        0        0     1212 2022-11-14 15:08:03.611810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ms.js
--rw-r--r--   0        0        0     1244 2022-11-14 15:08:03.612810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-nb.js
--rw-r--r--   0        0        0     1238 2022-11-14 15:08:03.612810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-nl-BE.js
--rw-r--r--   0        0        0     1230 2022-11-14 15:08:03.612810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-nl.js
--rw-r--r--   0        0        0     1241 2022-11-14 15:08:03.613809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-nn.js
--rw-r--r--   0        0        0     1236 2022-11-14 15:08:03.613809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-no.js
--rw-r--r--   0        0        0     1238 2022-11-14 15:08:03.614810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-pl.js
--rw-r--r--   0        0        0     1299 2022-11-14 15:08:03.614810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-pt-BR.js
--rw-r--r--   0        0        0     1216 2022-11-14 15:08:03.615810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-pt.js
--rw-r--r--   0        0        0     1278 2022-11-14 15:08:03.615810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-rm.js
--rw-r--r--   0        0        0     1287 2022-11-14 15:08:03.615810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ro.js
--rw-r--r--   0        0        0     1438 2022-11-14 15:08:03.615810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ru.js
--rw-r--r--   0        0        0     1226 2022-11-14 15:08:03.616809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sk.js
--rw-r--r--   0        0        0     1264 2022-11-14 15:08:03.617810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sl.js
--rw-r--r--   0        0        0     1208 2022-11-14 15:08:03.617810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sq.js
--rw-r--r--   0        0        0     1205 2022-11-14 15:08:03.617810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sr-SR.js
--rw-r--r--   0        0        0     1390 2022-11-14 15:08:03.618810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sr.js
--rw-r--r--   0        0        0     1222 2022-11-14 15:08:03.618810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sv.js
--rw-r--r--   0        0        0     1859 2022-11-14 15:08:03.618810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ta.js
--rw-r--r--   0        0        0     1583 2022-11-14 15:08:03.619809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-th.js
--rw-r--r--   0        0        0     1395 2022-11-14 15:08:03.619809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-tj.js
--rw-r--r--   0        0        0     1205 2022-11-14 15:08:03.619809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-tr.js
--rw-r--r--   0        0        0     1544 2022-11-14 15:08:03.620810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-uk.js
--rw-r--r--   0        0        0     1377 2022-11-14 15:08:03.620810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-vi.js
--rw-r--r--   0        0        0     1322 2022-11-14 15:08:03.621810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-zh-CN.js
--rw-r--r--   0        0        0     1320 2022-11-14 15:08:03.621810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-zh-HK.js
--rw-r--r--   0        0        0     1322 2022-11-14 15:08:03.621810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-zh-TW.js
--rw-r--r--   0        0        0      385 2022-11-14 15:08:03.633810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/ie.js
--rw-r--r--   0        0        0     2168 2022-11-14 15:08:03.635810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/jquery-patch.js
--rw-r--r--   0        0        0      530 2022-11-14 15:08:03.640810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/jquery-var-for-color.js
--rw-r--r--   0        0        0      820 2022-11-14 15:08:03.742810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/keycode.js
--rw-r--r--   0        0        0     1775 2022-11-14 15:08:03.742810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/labels.js
--rw-r--r--   0        0        0     1020 2022-11-14 15:08:03.743810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/plugin.js
--rw-r--r--   0        0        0    15125 2022-11-14 15:08:03.743810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/position.js
--rw-r--r--   0        0        0     1014 2022-11-14 15:08:03.747810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/safe-active-element.js
--rw-r--r--   0        0        0      523 2022-11-14 15:08:03.747810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/safe-blur.js
--rw-r--r--   0        0        0     1280 2022-11-14 15:08:03.747810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/scroll-parent.js
--rw-r--r--   0        0        0      883 2022-11-14 15:08:03.749810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/tabbable.js
--rw-r--r--   0        0        0      976 2022-11-14 15:08:03.750810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/unique-id.js
--rw-r--r--   0        0        0     1811 2022-11-14 15:08:03.824810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/vendor/jquery-color/LICENSE.txt
--rw-r--r--   0        0        0    17418 2022-11-14 15:08:03.641810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/vendor/jquery-color/jquery.color.js
--rw-r--r--   0        0        0      322 2022-11-14 15:08:03.750810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/version.js
--rw-r--r--   0        0        0    20283 2022-11-14 15:08:03.751810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widget.js
--rw-r--r--   0        0        0    16134 2022-11-14 15:08:03.592810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widgets/accordion.js
--rw-r--r--   0        0        0    17526 2022-11-14 15:08:03.593809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widgets/autocomplete.js
--rw-r--r--   0        0        0    11702 2022-11-14 15:08:03.594809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widgets/button.js
--rw-r--r--   0        0        0     7585 2022-11-14 15:08:03.594809 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widgets/checkboxradio.js
--rw-r--r--   0        0        0     8622 2022-11-14 15:08:03.595810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widgets/controlgroup.js
--rw-r--r--   0        0        0    82518 2022-11-14 15:08:03.622810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widgets/datepicker.js
--rw-r--r--   0        0        0    23738 2022-11-14 15:08:03.622810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widgets/dialog.js
--rw-r--r--   0        0        0    35541 2022-11-14 15:08:03.623810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widgets/draggable.js
--rw-r--r--   0        0        0    12895 2022-11-14 15:08:03.624810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widgets/droppable.js
--rw-r--r--   0        0        0    18956 2022-11-14 15:08:03.743810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widgets/menu.js
--rw-r--r--   0        0        0     6224 2022-11-14 15:08:03.743810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widgets/mouse.js
--rw-r--r--   0        0        0     4235 2022-11-14 15:08:03.744810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widgets/progressbar.js
--rw-r--r--   0        0        0    30395 2022-11-14 15:08:03.747810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widgets/resizable.js
--rw-r--r--   0        0        0     8125 2022-11-14 15:08:03.748810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widgets/selectable.js
--rw-r--r--   0        0        0    16249 2022-11-14 15:08:03.748810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widgets/selectmenu.js
--rw-r--r--   0        0        0    19595 2022-11-14 15:08:03.748810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widgets/slider.js
--rw-r--r--   0        0        0    47637 2022-11-14 15:08:03.749810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widgets/sortable.js
--rw-r--r--   0        0        0    14430 2022-11-14 15:08:03.749810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widgets/spinner.js
--rw-r--r--   0        0        0    23658 2022-11-14 15:08:03.750810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widgets/tabs.js
--rw-r--r--   0        0        0    14472 2022-11-14 15:08:03.750810 anitya-1.8.1/anitya/static/node_modules/jquery-ui/ui/widgets/tooltip.js
--rw-r--r--   0        0        0    45726 2022-11-14 15:08:03.705810 anitya-1.8.1/anitya/static/node_modules/moment/CHANGELOG.md
--rw-r--r--   0        0        0     1075 2022-11-14 15:08:03.408809 anitya-1.8.1/anitya/static/node_modules/moment/LICENSE
--rw-r--r--   0        0        0     2468 2022-11-14 15:08:03.705810 anitya-1.8.1/anitya/static/node_modules/moment/README.md
--rw-r--r--   0        0        0     2149 2022-11-14 15:08:03.420809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/af.js
--rw-r--r--   0        0        0     4449 2022-11-14 15:08:03.427809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ar-dz.js
--rw-r--r--   0        0        0     1934 2022-11-14 15:08:03.428809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ar-kw.js
--rw-r--r--   0        0        0     4648 2022-11-14 15:08:03.429809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ar-ly.js
--rw-r--r--   0        0        0     1989 2022-11-14 15:08:03.433809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ar-ma.js
--rw-r--r--   0        0        0     3042 2022-11-14 15:08:03.436809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ar-sa.js
--rw-r--r--   0        0        0     1936 2022-11-14 15:08:03.439809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ar-tn.js
--rw-r--r--   0        0        0     5072 2022-11-14 15:08:03.440809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ar.js
--rw-r--r--   0        0        0     2846 2022-11-14 15:08:03.448809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/az.js
--rw-r--r--   0        0        0     5154 2022-11-14 15:08:03.452809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/be.js
--rw-r--r--   0        0        0     2955 2022-11-14 15:08:03.455809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/bg.js
--rw-r--r--   0        0        0     1784 2022-11-14 15:08:03.457809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/bm.js
--rw-r--r--   0        0        0     4349 2022-11-14 15:08:03.459809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/bn-bd.js
--rw-r--r--   0        0        0     3898 2022-11-14 15:08:03.461809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/bn.js
--rw-r--r--   0        0        0     4399 2022-11-14 15:08:03.462809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/bo.js
--rw-r--r--   0        0        0     4544 2022-11-14 15:08:03.464809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/br.js
--rw-r--r--   0        0        0     4475 2022-11-14 15:08:03.466809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/bs.js
--rw-r--r--   0        0        0     3031 2022-11-14 15:08:03.466809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ca.js
--rw-r--r--   0        0        0     6718 2022-11-14 15:08:03.475809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/cs.js
--rw-r--r--   0        0        0     2341 2022-11-14 15:08:03.476809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/cv.js
--rw-r--r--   0        0        0     2834 2022-11-14 15:08:03.477809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/cy.js
--rw-r--r--   0        0        0     1629 2022-11-14 15:08:03.478809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/da.js
--rw-r--r--   0        0        0     2635 2022-11-14 15:08:03.480809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/de-at.js
--rw-r--r--   0        0        0     2563 2022-11-14 15:08:03.482809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/de-ch.js
--rw-r--r--   0        0        0     2562 2022-11-14 15:08:03.484809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/de.js
--rw-r--r--   0        0        0     2464 2022-11-14 15:08:03.487809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/dv.js
--rw-r--r--   0        0        0     3877 2022-11-14 15:08:03.488809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/el.js
--rw-r--r--   0        0        0     2029 2022-11-14 15:08:03.490809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/en-au.js
--rw-r--r--   0        0        0     1878 2022-11-14 15:08:03.491809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/en-ca.js
--rw-r--r--   0        0        0     2035 2022-11-14 15:08:03.493809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/en-gb.js
--rw-r--r--   0        0        0     2033 2022-11-14 15:08:03.496809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/en-ie.js
--rw-r--r--   0        0        0     1871 2022-11-14 15:08:03.498809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/en-il.js
--rw-r--r--   0        0        0     2029 2022-11-14 15:08:03.500809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/en-in.js
--rw-r--r--   0        0        0     2038 2022-11-14 15:08:03.502809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/en-nz.js
--rw-r--r--   0        0        0     2047 2022-11-14 15:08:03.505809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/en-sg.js
--rw-r--r--   0        0        0     2338 2022-11-14 15:08:03.512809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/eo.js
--rw-r--r--   0        0        0     3441 2022-11-14 15:08:03.515809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/es-do.js
--rw-r--r--   0        0        0     3510 2022-11-14 15:08:03.517809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/es-mx.js
--rw-r--r--   0        0        0     3538 2022-11-14 15:08:03.519809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/es-us.js
--rw-r--r--   0        0        0     3498 2022-11-14 15:08:03.521809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/es.js
--rw-r--r--   0        0        0     2631 2022-11-14 15:08:03.523809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/et.js
--rw-r--r--   0        0        0     1964 2022-11-14 15:08:03.525809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/eu.js
--rw-r--r--   0        0        0     3230 2022-11-14 15:08:03.526809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/fa.js
--rw-r--r--   0        0        0     3632 2022-11-14 15:08:03.528809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/fi.js
--rw-r--r--   0        0        0     1776 2022-11-14 15:08:03.530809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/fil.js
--rw-r--r--   0        0        0     1772 2022-11-14 15:08:03.531809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/fo.js
--rw-r--r--   0        0        0     2104 2022-11-14 15:08:03.540809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/fr-ca.js
--rw-r--r--   0        0        0     2263 2022-11-14 15:08:03.542809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/fr-ch.js
--rw-r--r--   0        0        0     3471 2022-11-14 15:08:03.543809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/fr.js
--rw-r--r--   0        0        0     2275 2022-11-14 15:08:03.548809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/fy.js
--rw-r--r--   0        0        0     2360 2022-11-14 15:08:03.549809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ga.js
--rw-r--r--   0        0        0     2380 2022-11-14 15:08:03.551809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/gd.js
--rw-r--r--   0        0        0     2347 2022-11-14 15:08:03.552809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/gl.js
--rw-r--r--   0        0        0     5506 2022-11-14 15:08:03.555809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/gom-deva.js
--rw-r--r--   0        0        0     4130 2022-11-14 15:08:03.557809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/gom-latn.js
--rw-r--r--   0        0        0     4132 2022-11-14 15:08:03.559809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/gu.js
--rw-r--r--   0        0        0     3211 2022-11-14 15:08:03.560809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/he.js
--rw-r--r--   0        0        0     6421 2022-11-14 15:08:03.562809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/hi.js
--rw-r--r--   0        0        0     4718 2022-11-14 15:08:03.564809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/hr.js
--rw-r--r--   0        0        0     3815 2022-11-14 15:08:03.566809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/hu.js
--rw-r--r--   0        0        0     3236 2022-11-14 15:08:03.568809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/hy-am.js
--rw-r--r--   0        0        0     2375 2022-11-14 15:08:03.571809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/id.js
--rw-r--r--   0        0        0     4458 2022-11-14 15:08:03.577809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/is.js
--rw-r--r--   0        0        0     1941 2022-11-14 15:08:03.578809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/it-ch.js
--rw-r--r--   0        0        0     3251 2022-11-14 15:08:03.579810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/it.js
--rw-r--r--   0        0        0     3955 2022-11-14 15:08:03.580809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ja.js
--rw-r--r--   0        0        0     2384 2022-11-14 15:08:03.582810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/jv.js
--rw-r--r--   0        0        0     3504 2022-11-14 15:08:03.583809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ka.js
--rw-r--r--   0        0        0     2495 2022-11-14 15:08:03.584809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/kk.js
--rw-r--r--   0        0        0     3362 2022-11-14 15:08:03.586809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/km.js
--rw-r--r--   0        0        0     4252 2022-11-14 15:08:03.587809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/kn.js
--rw-r--r--   0        0        0     2223 2022-11-14 15:08:03.589810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ko.js
--rw-r--r--   0        0        0     3330 2022-11-14 15:08:03.590809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ku.js
--rw-r--r--   0        0        0     2521 2022-11-14 15:08:03.591809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ky.js
--rw-r--r--   0        0        0     4269 2022-11-14 15:08:03.593809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/lb.js
--rw-r--r--   0        0        0     2585 2022-11-14 15:08:03.595810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/lo.js
--rw-r--r--   0        0        0     4005 2022-11-14 15:08:03.610809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/lt.js
--rw-r--r--   0        0        0     3449 2022-11-14 15:08:03.612810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/lv.js
--rw-r--r--   0        0        0     3661 2022-11-14 15:08:03.613809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/me.js
--rw-r--r--   0        0        0     2023 2022-11-14 15:08:03.615810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/mi.js
--rw-r--r--   0        0        0     3021 2022-11-14 15:08:03.617810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/mk.js
--rw-r--r--   0        0        0     3287 2022-11-14 15:08:03.619809 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ml.js
--rw-r--r--   0        0        0     3414 2022-11-14 15:08:03.620810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/mn.js
--rw-r--r--   0        0        0     6574 2022-11-14 15:08:03.637810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/mr.js
--rw-r--r--   0        0        0     2330 2022-11-14 15:08:03.637810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ms-my.js
--rw-r--r--   0        0        0     2277 2022-11-14 15:08:03.638810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ms.js
--rw-r--r--   0        0        0     1684 2022-11-14 15:08:03.639810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/mt.js
--rw-r--r--   0        0        0     3094 2022-11-14 15:08:03.639810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/my.js
--rw-r--r--   0        0        0     1899 2022-11-14 15:08:03.640810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/nb.js
--rw-r--r--   0        0        0     4031 2022-11-14 15:08:03.640810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ne.js
--rw-r--r--   0        0        0     3169 2022-11-14 15:08:03.641810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/nl-be.js
--rw-r--r--   0        0        0     3202 2022-11-14 15:08:03.642810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/nl.js
--rw-r--r--   0        0        0     1828 2022-11-14 15:08:03.642810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/nn.js
--rw-r--r--   0        0        0     2472 2022-11-14 15:08:03.643810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/oc-lnc.js
--rw-r--r--   0        0        0     4198 2022-11-14 15:08:03.644810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/pa-in.js
--rw-r--r--   0        0        0     4166 2022-11-14 15:08:03.647810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/pl.js
--rw-r--r--   0        0        0     1854 2022-11-14 15:08:03.649810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/pt-br.js
--rw-r--r--   0        0        0     1968 2022-11-14 15:08:03.650810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/pt.js
--rw-r--r--   0        0        0     2319 2022-11-14 15:08:03.652810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ro.js
--rw-r--r--   0        0        0     8418 2022-11-14 15:08:03.654810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ru.js
--rw-r--r--   0        0        0     2153 2022-11-14 15:08:03.655810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/sd.js
--rw-r--r--   0        0        0     1849 2022-11-14 15:08:03.655810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/se.js
--rw-r--r--   0        0        0     2681 2022-11-14 15:08:03.656810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/si.js
--rw-r--r--   0        0        0     5173 2022-11-14 15:08:03.657810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/sk.js
--rw-r--r--   0        0        0     6115 2022-11-14 15:08:03.657810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/sl.js
--rw-r--r--   0        0        0     1987 2022-11-14 15:08:03.658810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/sq.js
--rw-r--r--   0        0        0     4762 2022-11-14 15:08:03.659810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/sr-cyrl.js
--rw-r--r--   0        0        0     4209 2022-11-14 15:08:03.659810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/sr.js
--rw-r--r--   0        0        0     2572 2022-11-14 15:08:03.660810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ss.js
--rw-r--r--   0        0        0     2066 2022-11-14 15:08:03.662810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/sv.js
--rw-r--r--   0        0        0     1651 2022-11-14 15:08:03.663810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/sw.js
--rw-r--r--   0        0        0     4800 2022-11-14 15:08:03.663810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ta.js
--rw-r--r--   0        0        0     3392 2022-11-14 15:08:03.664810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/te.js
--rw-r--r--   0        0        0     2155 2022-11-14 15:08:03.665810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/tet.js
--rw-r--r--   0        0        0     3604 2022-11-14 15:08:03.666810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/tg.js
--rw-r--r--   0        0        0     2736 2022-11-14 15:08:03.667810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/th.js
--rw-r--r--   0        0        0     2488 2022-11-14 15:08:03.668810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/tk.js
--rw-r--r--   0        0        0     1735 2022-11-14 15:08:03.669810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/tl-ph.js
--rw-r--r--   0        0        0     3755 2022-11-14 15:08:03.670810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/tlh.js
--rw-r--r--   0        0        0     2927 2022-11-14 15:08:03.672810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/tr.js
--rw-r--r--   0        0        0     3109 2022-11-14 15:08:03.674810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/tzl.js
--rw-r--r--   0        0        0     1691 2022-11-14 15:08:03.674810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/tzm-latn.js
--rw-r--r--   0        0        0     2322 2022-11-14 15:08:03.675810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/tzm.js
--rw-r--r--   0        0        0     3880 2022-11-14 15:08:03.687810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ug-cn.js
--rw-r--r--   0        0        0     5955 2022-11-14 15:08:03.688810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/uk.js
--rw-r--r--   0        0        0     2200 2022-11-14 15:08:03.689810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/ur.js
--rw-r--r--   0        0        0     1639 2022-11-14 15:08:03.691810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/uz-latn.js
--rw-r--r--   0        0        0     1885 2022-11-14 15:08:03.692810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/uz.js
--rw-r--r--   0        0        0     2430 2022-11-14 15:08:03.693810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/vi.js
--rw-r--r--   0        0        0     2348 2022-11-14 15:08:03.695810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/x-pseudo.js
--rw-r--r--   0        0        0     1887 2022-11-14 15:08:03.696810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/yo.js
--rw-r--r--   0        0        0     3711 2022-11-14 15:08:03.698810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/zh-cn.js
--rw-r--r--   0        0        0     3116 2022-11-14 15:08:03.700810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/zh-hk.js
--rw-r--r--   0        0        0     3066 2022-11-14 15:08:03.701810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/zh-mo.js
--rw-r--r--   0        0        0     3013 2022-11-14 15:08:03.701810 anitya-1.8.1/anitya/static/node_modules/moment/dist/locale/zh-tw.js
--rw-r--r--   0        0        0   154671 2022-11-14 15:08:03.635810 anitya-1.8.1/anitya/static/node_modules/moment/dist/moment.js
--rw-r--r--   0        0        0       39 2022-11-14 15:08:03.512809 anitya-1.8.1/anitya/static/node_modules/moment/ender.js
--rw-r--r--   0        0        0     2753 2022-11-14 15:08:03.421809 anitya-1.8.1/anitya/static/node_modules/moment/locale/af.js
--rw-r--r--   0        0        0     5377 2022-11-14 15:08:03.427809 anitya-1.8.1/anitya/static/node_modules/moment/locale/ar-dz.js
--rw-r--r--   0        0        0     2478 2022-11-14 15:08:03.428809 anitya-1.8.1/anitya/static/node_modules/moment/locale/ar-kw.js
--rw-r--r--   0        0        0     5652 2022-11-14 15:08:03.430809 anitya-1.8.1/anitya/static/node_modules/moment/locale/ar-ly.js
--rw-r--r--   0        0        0     2533 2022-11-14 15:08:03.435809 anitya-1.8.1/anitya/static/node_modules/moment/locale/ar-ma.js
--rw-r--r--   0        0        0     3782 2022-11-14 15:08:03.437809 anitya-1.8.1/anitya/static/node_modules/moment/locale/ar-sa.js
--rw-r--r--   0        0        0     2480 2022-11-14 15:08:03.439809 anitya-1.8.1/anitya/static/node_modules/moment/locale/ar-tn.js
--rw-r--r--   0        0        0     6136 2022-11-14 15:08:03.440809 anitya-1.8.1/anitya/static/node_modules/moment/locale/ar.js
--rw-r--r--   0        0        0     3570 2022-11-14 15:08:03.449809 anitya-1.8.1/anitya/static/node_modules/moment/locale/az.js
--rw-r--r--   0        0        0     6030 2022-11-14 15:08:03.454809 anitya-1.8.1/anitya/static/node_modules/moment/locale/be.js
--rw-r--r--   0        0        0     3623 2022-11-14 15:08:03.456809 anitya-1.8.1/anitya/static/node_modules/moment/locale/bg.js
--rw-r--r--   0        0        0     2233 2022-11-14 15:08:03.457809 anitya-1.8.1/anitya/static/node_modules/moment/locale/bm.js
--rw-r--r--   0        0        0     5177 2022-11-14 15:08:03.460809 anitya-1.8.1/anitya/static/node_modules/moment/locale/bn-bd.js
--rw-r--r--   0        0        0     4690 2022-11-14 15:08:03.461809 anitya-1.8.1/anitya/static/node_modules/moment/locale/bn.js
--rw-r--r--   0        0        0     5211 2022-11-14 15:08:03.463809 anitya-1.8.1/anitya/static/node_modules/moment/locale/bo.js
--rw-r--r--   0        0        0     5520 2022-11-14 15:08:03.465809 anitya-1.8.1/anitya/static/node_modules/moment/locale/br.js
--rw-r--r--   0        0        0     5387 2022-11-14 15:08:03.466809 anitya-1.8.1/anitya/static/node_modules/moment/locale/bs.js
--rw-r--r--   0        0        0     3751 2022-11-14 15:08:03.467809 anitya-1.8.1/anitya/static/node_modules/moment/locale/ca.js
--rw-r--r--   0        0        0     7750 2022-11-14 15:08:03.475809 anitya-1.8.1/anitya/static/node_modules/moment/locale/cs.js
--rw-r--r--   0        0        0     2913 2022-11-14 15:08:03.476809 anitya-1.8.1/anitya/static/node_modules/moment/locale/cv.js
--rw-r--r--   0        0        0     3542 2022-11-14 15:08:03.477809 anitya-1.8.1/anitya/static/node_modules/moment/locale/cy.js
--rw-r--r--   0        0        0     2161 2022-11-14 15:08:03.478809 anitya-1.8.1/anitya/static/node_modules/moment/locale/da.js
--rw-r--r--   0        0        0     3259 2022-11-14 15:08:03.481809 anitya-1.8.1/anitya/static/node_modules/moment/locale/de-at.js
--rw-r--r--   0        0        0     3094 2022-11-14 15:08:03.482809 anitya-1.8.1/anitya/static/node_modules/moment/locale/de-ch.js
--rw-r--r--   0        0        0     3182 2022-11-14 15:08:03.485809 anitya-1.8.1/anitya/static/node_modules/moment/locale/de.js
--rw-r--r--   0        0        0     3140 2022-11-14 15:08:03.487809 anitya-1.8.1/anitya/static/node_modules/moment/locale/dv.js
--rw-r--r--   0        0        0     4617 2022-11-14 15:08:03.489809 anitya-1.8.1/anitya/static/node_modules/moment/locale/el.js
--rw-r--r--   0        0        0     2625 2022-11-14 15:08:03.490809 anitya-1.8.1/anitya/static/node_modules/moment/locale/en-au.js
--rw-r--r--   0        0        0     2458 2022-11-14 15:08:03.492809 anitya-1.8.1/anitya/static/node_modules/moment/locale/en-ca.js
--rw-r--r--   0        0        0     2631 2022-11-14 15:08:03.494809 anitya-1.8.1/anitya/static/node_modules/moment/locale/en-gb.js
--rw-r--r--   0        0        0     2629 2022-11-14 15:08:03.496809 anitya-1.8.1/anitya/static/node_modules/moment/locale/en-ie.js
--rw-r--r--   0        0        0     2451 2022-11-14 15:08:03.499809 anitya-1.8.1/anitya/static/node_modules/moment/locale/en-il.js
--rw-r--r--   0        0        0     2625 2022-11-14 15:08:03.501809 anitya-1.8.1/anitya/static/node_modules/moment/locale/en-in.js
--rw-r--r--   0        0        0     2634 2022-11-14 15:08:03.503809 anitya-1.8.1/anitya/static/node_modules/moment/locale/en-nz.js
--rw-r--r--   0        0        0     2643 2022-11-14 15:08:03.509809 anitya-1.8.1/anitya/static/node_modules/moment/locale/en-sg.js
--rw-r--r--   0        0        0     2918 2022-11-14 15:08:03.513809 anitya-1.8.1/anitya/static/node_modules/moment/locale/eo.js
--rw-r--r--   0        0        0     4197 2022-11-14 15:08:03.516809 anitya-1.8.1/anitya/static/node_modules/moment/locale/es-do.js
--rw-r--r--   0        0        0     4270 2022-11-14 15:08:03.518809 anitya-1.8.1/anitya/static/node_modules/moment/locale/es-mx.js
--rw-r--r--   0        0        0     4294 2022-11-14 15:08:03.520809 anitya-1.8.1/anitya/static/node_modules/moment/locale/es-us.js
--rw-r--r--   0        0        0     4254 2022-11-14 15:08:03.522809 anitya-1.8.1/anitya/static/node_modules/moment/locale/es.js
--rw-r--r--   0        0        0     3255 2022-11-14 15:08:03.524809 anitya-1.8.1/anitya/static/node_modules/moment/locale/et.js
--rw-r--r--   0        0        0     2544 2022-11-14 15:08:03.525809 anitya-1.8.1/anitya/static/node_modules/moment/locale/eu.js
--rw-r--r--   0        0        0     3998 2022-11-14 15:08:03.527809 anitya-1.8.1/anitya/static/node_modules/moment/locale/fa.js
--rw-r--r--   0        0        0     4444 2022-11-14 15:08:03.529809 anitya-1.8.1/anitya/static/node_modules/moment/locale/fi.js
--rw-r--r--   0        0        0     2326 2022-11-14 15:08:03.530809 anitya-1.8.1/anitya/static/node_modules/moment/locale/fil.js
--rw-r--r--   0        0        0     2316 2022-11-14 15:08:03.534809 anitya-1.8.1/anitya/static/node_modules/moment/locale/fo.js
--rw-r--r--   0        0        0     2704 2022-11-14 15:08:03.541809 anitya-1.8.1/anitya/static/node_modules/moment/locale/fr-ca.js
--rw-r--r--   0        0        0     2879 2022-11-14 15:08:03.542809 anitya-1.8.1/anitya/static/node_modules/moment/locale/fr-ch.js
--rw-r--r--   0        0        0     4211 2022-11-14 15:08:03.544809 anitya-1.8.1/anitya/static/node_modules/moment/locale/fr.js
--rw-r--r--   0        0        0     2891 2022-11-14 15:08:03.549809 anitya-1.8.1/anitya/static/node_modules/moment/locale/fy.js
--rw-r--r--   0        0        0     3056 2022-11-14 15:08:03.550809 anitya-1.8.1/anitya/static/node_modules/moment/locale/ga.js
--rw-r--r--   0        0        0     3076 2022-11-14 15:08:03.551809 anitya-1.8.1/anitya/static/node_modules/moment/locale/gd.js
--rw-r--r--   0        0        0     2967 2022-11-14 15:08:03.552809 anitya-1.8.1/anitya/static/node_modules/moment/locale/gl.js
--rw-r--r--   0        0        0     6336 2022-11-14 15:08:03.556809 anitya-1.8.1/anitya/static/node_modules/moment/locale/gom-deva.js
--rw-r--r--   0        0        0     4952 2022-11-14 15:08:03.558809 anitya-1.8.1/anitya/static/node_modules/moment/locale/gom-latn.js
--rw-r--r--   0        0        0     4936 2022-11-14 15:08:03.559809 anitya-1.8.1/anitya/static/node_modules/moment/locale/gu.js
--rw-r--r--   0        0        0     3899 2022-11-14 15:08:03.560809 anitya-1.8.1/anitya/static/node_modules/moment/locale/he.js
--rw-r--r--   0        0        0     7385 2022-11-14 15:08:03.562809 anitya-1.8.1/anitya/static/node_modules/moment/locale/hi.js
--rw-r--r--   0        0        0     5658 2022-11-14 15:08:03.565809 anitya-1.8.1/anitya/static/node_modules/moment/locale/hr.js
--rw-r--r--   0        0        0     4599 2022-11-14 15:08:03.566809 anitya-1.8.1/anitya/static/node_modules/moment/locale/hu.js
--rw-r--r--   0        0        0     3936 2022-11-14 15:08:03.569809 anitya-1.8.1/anitya/static/node_modules/moment/locale/hy-am.js
--rw-r--r--   0        0        0     2995 2022-11-14 15:08:03.571809 anitya-1.8.1/anitya/static/node_modules/moment/locale/id.js
--rw-r--r--   0        0        0     5334 2022-11-14 15:08:03.577809 anitya-1.8.1/anitya/static/node_modules/moment/locale/is.js
--rw-r--r--   0        0        0     2521 2022-11-14 15:08:03.578809 anitya-1.8.1/anitya/static/node_modules/moment/locale/it-ch.js
--rw-r--r--   0        0        0     3987 2022-11-14 15:08:03.579810 anitya-1.8.1/anitya/static/node_modules/moment/locale/it.js
--rw-r--r--   0        0        0     4867 2022-11-14 15:08:03.581809 anitya-1.8.1/anitya/static/node_modules/moment/locale/ja.js
--rw-r--r--   0        0        0     3004 2022-11-14 15:08:03.582810 anitya-1.8.1/anitya/static/node_modules/moment/locale/jv.js
--rw-r--r--   0        0        0     4192 2022-11-14 15:08:03.583809 anitya-1.8.1/anitya/static/node_modules/moment/locale/ka.js
--rw-r--r--   0        0        0     3139 2022-11-14 15:08:03.585809 anitya-1.8.1/anitya/static/node_modules/moment/locale/kk.js
--rw-r--r--   0        0        0     4090 2022-11-14 15:08:03.586809 anitya-1.8.1/anitya/static/node_modules/moment/locale/km.js
--rw-r--r--   0        0        0     5064 2022-11-14 15:08:03.588809 anitya-1.8.1/anitya/static/node_modules/moment/locale/kn.js
--rw-r--r--   0        0        0     2839 2022-11-14 15:08:03.589810 anitya-1.8.1/anitya/static/node_modules/moment/locale/ko.js
--rw-r--r--   0        0        0     4118 2022-11-14 15:08:03.590809 anitya-1.8.1/anitya/static/node_modules/moment/locale/ku.js
--rw-r--r--   0        0        0     3173 2022-11-14 15:08:03.591809 anitya-1.8.1/anitya/static/node_modules/moment/locale/ky.js
--rw-r--r--   0        0        0     5129 2022-11-14 15:08:03.593809 anitya-1.8.1/anitya/static/node_modules/moment/locale/lb.js
--rw-r--r--   0        0        0     3169 2022-11-14 15:08:03.595810 anitya-1.8.1/anitya/static/node_modules/moment/locale/lo.js
--rw-r--r--   0        0        0     4825 2022-11-14 15:08:03.610809 anitya-1.8.1/anitya/static/node_modules/moment/locale/lt.js
--rw-r--r--   0        0        0     4137 2022-11-14 15:08:03.612810 anitya-1.8.1/anitya/static/node_modules/moment/locale/lv.js
--rw-r--r--   0        0        0     4441 2022-11-14 15:08:03.614810 anitya-1.8.1/anitya/static/node_modules/moment/locale/me.js
--rw-r--r--   0        0        0     2583 2022-11-14 15:08:03.615810 anitya-1.8.1/anitya/static/node_modules/moment/locale/mi.js
--rw-r--r--   0        0        0     3682 2022-11-14 15:08:03.618810 anitya-1.8.1/anitya/static/node_modules/moment/locale/mk.js
--rw-r--r--   0        0        0     3935 2022-11-14 15:08:03.619809 anitya-1.8.1/anitya/static/node_modules/moment/locale/ml.js
--rw-r--r--   0        0        0     4130 2022-11-14 15:08:03.621810 anitya-1.8.1/anitya/static/node_modules/moment/locale/mn.js
--rw-r--r--   0        0        0     7694 2022-11-14 15:08:03.637810 anitya-1.8.1/anitya/static/node_modules/moment/locale/mr.js
--rw-r--r--   0        0        0     2954 2022-11-14 15:08:03.638810 anitya-1.8.1/anitya/static/node_modules/moment/locale/ms-my.js
--rw-r--r--   0        0        0     2897 2022-11-14 15:08:03.638810 anitya-1.8.1/anitya/static/node_modules/moment/locale/ms.js
--rw-r--r--   0        0        0     2228 2022-11-14 15:08:03.639810 anitya-1.8.1/anitya/static/node_modules/moment/locale/mt.js
--rw-r--r--   0        0        0     3762 2022-11-14 15:08:03.639810 anitya-1.8.1/anitya/static/node_modules/moment/locale/my.js
--rw-r--r--   0        0        0     2451 2022-11-14 15:08:03.640810 anitya-1.8.1/anitya/static/node_modules/moment/locale/nb.js
--rw-r--r--   0        0        0     4831 2022-11-14 15:08:03.641810 anitya-1.8.1/anitya/static/node_modules/moment/locale/ne.js
--rw-r--r--   0        0        0     3881 2022-11-14 15:08:03.641810 anitya-1.8.1/anitya/static/node_modules/moment/locale/nl-be.js
--rw-r--r--   0        0        0     3918 2022-11-14 15:08:03.642810 anitya-1.8.1/anitya/static/node_modules/moment/locale/nl.js
--rw-r--r--   0        0        0     2380 2022-11-14 15:08:03.642810 anitya-1.8.1/anitya/static/node_modules/moment/locale/nn.js
--rw-r--r--   0        0        0     3138 2022-11-14 15:08:03.643810 anitya-1.8.1/anitya/static/node_modules/moment/locale/oc-lnc.js
--rw-r--r--   0        0        0     5006 2022-11-14 15:08:03.646810 anitya-1.8.1/anitya/static/node_modules/moment/locale/pa-in.js
--rw-r--r--   0        0        0     5026 2022-11-14 15:08:03.647810 anitya-1.8.1/anitya/static/node_modules/moment/locale/pl.js
--rw-r--r--   0        0        0     2410 2022-11-14 15:08:03.649810 anitya-1.8.1/anitya/static/node_modules/moment/locale/pt-br.js
--rw-r--r--   0        0        0     2540 2022-11-14 15:08:03.650810 anitya-1.8.1/anitya/static/node_modules/moment/locale/pt.js
--rw-r--r--   0        0        0     2931 2022-11-14 15:08:03.652810 anitya-1.8.1/anitya/static/node_modules/moment/locale/ro.js
--rw-r--r--   0        0        0     9562 2022-11-14 15:08:03.654810 anitya-1.8.1/anitya/static/node_modules/moment/locale/ru.js
--rw-r--r--   0        0        0     2793 2022-11-14 15:08:03.655810 anitya-1.8.1/anitya/static/node_modules/moment/locale/sd.js
--rw-r--r--   0        0        0     2397 2022-11-14 15:08:03.655810 anitya-1.8.1/anitya/static/node_modules/moment/locale/se.js
--rw-r--r--   0        0        0     3277 2022-11-14 15:08:03.656810 anitya-1.8.1/anitya/static/node_modules/moment/locale/si.js
--rw-r--r--   0        0        0     6065 2022-11-14 15:08:03.657810 anitya-1.8.1/anitya/static/node_modules/moment/locale/sk.js
--rw-r--r--   0        0        0     7111 2022-11-14 15:08:03.657810 anitya-1.8.1/anitya/static/node_modules/moment/locale/sl.js
--rw-r--r--   0        0        0     2559 2022-11-14 15:08:03.658810 anitya-1.8.1/anitya/static/node_modules/moment/locale/sq.js
--rw-r--r--   0        0        0     5578 2022-11-14 15:08:03.659810 anitya-1.8.1/anitya/static/node_modules/moment/locale/sr-cyrl.js
--rw-r--r--   0        0        0     5025 2022-11-14 15:08:03.660810 anitya-1.8.1/anitya/static/node_modules/moment/locale/sr.js
--rw-r--r--   0        0        0     3228 2022-11-14 15:08:03.661810 anitya-1.8.1/anitya/static/node_modules/moment/locale/ss.js
--rw-r--r--   0        0        0     2658 2022-11-14 15:08:03.662810 anitya-1.8.1/anitya/static/node_modules/moment/locale/sv.js
--rw-r--r--   0        0        0     2191 2022-11-14 15:08:03.663810 anitya-1.8.1/anitya/static/node_modules/moment/locale/sw.js
--rw-r--r--   0        0        0     5640 2022-11-14 15:08:03.664810 anitya-1.8.1/anitya/static/node_modules/moment/locale/ta.js
--rw-r--r--   0        0        0     4064 2022-11-14 15:08:03.665810 anitya-1.8.1/anitya/static/node_modules/moment/locale/te.js
--rw-r--r--   0        0        0     2741 2022-11-14 15:08:03.666810 anitya-1.8.1/anitya/static/node_modules/moment/locale/tet.js
--rw-r--r--   0        0        0     4388 2022-11-14 15:08:03.667810 anitya-1.8.1/anitya/static/node_modules/moment/locale/tg.js
--rw-r--r--   0        0        0     3316 2022-11-14 15:08:03.667810 anitya-1.8.1/anitya/static/node_modules/moment/locale/th.js
--rw-r--r--   0        0        0     3168 2022-11-14 15:08:03.669810 anitya-1.8.1/anitya/static/node_modules/moment/locale/tk.js
--rw-r--r--   0        0        0     2287 2022-11-14 15:08:03.670810 anitya-1.8.1/anitya/static/node_modules/moment/locale/tl-ph.js
--rw-r--r--   0        0        0     4553 2022-11-14 15:08:03.670810 anitya-1.8.1/anitya/static/node_modules/moment/locale/tlh.js
--rw-r--r--   0        0        0     3663 2022-11-14 15:08:03.673810 anitya-1.8.1/anitya/static/node_modules/moment/locale/tr.js
--rw-r--r--   0        0        0     3779 2022-11-14 15:08:03.674810 anitya-1.8.1/anitya/static/node_modules/moment/locale/tzl.js
--rw-r--r--   0        0        0     2237 2022-11-14 15:08:03.675810 anitya-1.8.1/anitya/static/node_modules/moment/locale/tzm-latn.js
--rw-r--r--   0        0        0     2860 2022-11-14 15:08:03.676810 anitya-1.8.1/anitya/static/node_modules/moment/locale/tzm.js
--rw-r--r--   0        0        0     4644 2022-11-14 15:08:03.688810 anitya-1.8.1/anitya/static/node_modules/moment/locale/ug-cn.js
--rw-r--r--   0        0        0     6927 2022-11-14 15:08:03.689810 anitya-1.8.1/anitya/static/node_modules/moment/locale/uk.js
--rw-r--r--   0        0        0     2840 2022-11-14 15:08:03.690810 anitya-1.8.1/anitya/static/node_modules/moment/locale/ur.js
--rw-r--r--   0        0        0     2183 2022-11-14 15:08:03.691810 anitya-1.8.1/anitya/static/node_modules/moment/locale/uz-latn.js
--rw-r--r--   0        0        0     2409 2022-11-14 15:08:03.692810 anitya-1.8.1/anitya/static/node_modules/moment/locale/uz.js
--rw-r--r--   0        0        0     3066 2022-11-14 15:08:03.694810 anitya-1.8.1/anitya/static/node_modules/moment/locale/vi.js
--rw-r--r--   0        0        0     2970 2022-11-14 15:08:03.695810 anitya-1.8.1/anitya/static/node_modules/moment/locale/x-pseudo.js
--rw-r--r--   0        0        0     2419 2022-11-14 15:08:03.696810 anitya-1.8.1/anitya/static/node_modules/moment/locale/yo.js
--rw-r--r--   0        0        0     4507 2022-11-14 15:08:03.699810 anitya-1.8.1/anitya/static/node_modules/moment/locale/zh-cn.js
--rw-r--r--   0        0        0     3832 2022-11-14 15:08:03.700810 anitya-1.8.1/anitya/static/node_modules/moment/locale/zh-hk.js
--rw-r--r--   0        0        0     3782 2022-11-14 15:08:03.701810 anitya-1.8.1/anitya/static/node_modules/moment/locale/zh-mo.js
--rw-r--r--   0        0        0     3729 2022-11-14 15:08:03.701810 anitya-1.8.1/anitya/static/node_modules/moment/locale/zh-tw.js
--rw-r--r--   0        0        0   448027 2022-11-14 15:08:03.602810 anitya-1.8.1/anitya/static/node_modules/moment/min/locales.js
--rw-r--r--   0        0        0   310773 2022-11-14 15:08:03.609809 anitya-1.8.1/anitya/static/node_modules/moment/min/locales.min.js
--rw-r--r--   0        0        0   140130 2022-11-14 15:08:03.702810 anitya-1.8.1/anitya/static/node_modules/moment/min/locales.min.js.map
--rw-r--r--   0        0        0   622045 2022-11-14 15:08:03.629810 anitya-1.8.1/anitya/static/node_modules/moment/min/moment-with-locales.js
--rw-r--r--   0        0        0   369019 2022-11-14 15:08:03.634810 anitya-1.8.1/anitya/static/node_modules/moment/min/moment-with-locales.min.js
--rw-r--r--   0        0        0   230173 2022-11-14 15:08:03.704810 anitya-1.8.1/anitya/static/node_modules/moment/min/moment-with-locales.min.js.map
--rw-r--r--   0        0        0    58103 2022-11-14 15:08:03.636810 anitya-1.8.1/anitya/static/node_modules/moment/min/moment.min.js
--rw-r--r--   0        0        0    86041 2022-11-14 15:08:03.705810 anitya-1.8.1/anitya/static/node_modules/moment/min/moment.min.js.map
--rw-r--r--   0        0        0    23820 2022-11-14 15:08:03.705810 anitya-1.8.1/anitya/static/node_modules/moment/moment.d.ts
--rw-r--r--   0        0        0   174604 2022-11-14 15:08:03.636810 anitya-1.8.1/anitya/static/node_modules/moment/moment.js
--rw-r--r--   0        0        0      273 2022-11-14 15:08:03.646810 anitya-1.8.1/anitya/static/node_modules/moment/package.js
--rw-r--r--   0        0        0     3418 2022-11-14 15:08:03.702810 anitya-1.8.1/anitya/static/node_modules/moment/package.json
--rw-r--r--   0        0        0     1542 2022-11-14 15:08:03.470809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/create/check-overflow.js
--rw-r--r--   0        0        0     1076 2022-11-14 15:08:03.479809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/create/date-from-array.js
--rw-r--r--   0        0        0     3351 2022-11-14 15:08:03.545809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/create/from-anything.js
--rw-r--r--   0        0        0     5585 2022-11-14 15:08:03.546809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/create/from-array.js
--rw-r--r--   0        0        0      549 2022-11-14 15:08:03.546809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/create/from-object.js
--rw-r--r--   0        0        0     2011 2022-11-14 15:08:03.546809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/create/from-string-and-array.js
--rw-r--r--   0        0        0     4092 2022-11-14 15:08:03.547809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/create/from-string-and-format.js
--rw-r--r--   0        0        0     8007 2022-11-14 15:08:03.547809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/create/from-string.js
--rw-r--r--   0        0        0      183 2022-11-14 15:08:03.596809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/create/local.js
--rw-r--r--   0        0        0      644 2022-11-14 15:08:03.646810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/create/parsing-flags.js
--rw-r--r--   0        0        0      186 2022-11-14 15:08:03.690810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/create/utc.js
--rw-r--r--   0        0        0     1514 2022-11-14 15:08:03.692810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/create/valid.js
--rw-r--r--   0        0        0      484 2022-11-14 15:08:03.414809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/duration/abs.js
--rw-r--r--   0        0        0      644 2022-11-14 15:08:03.415809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/duration/add-subtract.js
--rw-r--r--   0        0        0     2360 2022-11-14 15:08:03.441809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/duration/as.js
--rw-r--r--   0        0        0     1774 2022-11-14 15:08:03.466809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/duration/bubble.js
--rw-r--r--   0        0        0      105 2022-11-14 15:08:03.470809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/duration/clone.js
--rw-r--r--   0        0        0     1593 2022-11-14 15:08:03.472809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/duration/constructor.js
--rw-r--r--   0        0        0     4335 2022-11-14 15:08:03.474809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/duration/create.js
--rw-r--r--   0        0        0      342 2022-11-14 15:08:03.487809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/duration/duration.js
--rw-r--r--   0        0        0      728 2022-11-14 15:08:03.552809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/duration/get.js
--rw-r--r--   0        0        0     3493 2022-11-14 15:08:03.567809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/duration/humanize.js
--rw-r--r--   0        0        0     2078 2022-11-14 15:08:03.578809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/duration/iso-string.js
--rw-r--r--   0        0        0     1739 2022-11-14 15:08:03.647810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/duration/prototype.js
--rw-r--r--   0        0        0     1184 2022-11-14 15:08:03.693810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/duration/valid.js
--rw-r--r--   0        0        0     2911 2022-11-14 15:08:03.538809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/format/format.js
--rw-r--r--   0        0        0     1187 2022-11-14 15:08:03.452809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/locale/base-config.js
--rw-r--r--   0        0        0      442 2022-11-14 15:08:03.467809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/locale/calendar.js
--rw-r--r--   0        0        0       93 2022-11-14 15:08:03.472809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/locale/constructor.js
--rw-r--r--   0        0        0      989 2022-11-14 15:08:03.511809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/locale/en.js
--rw-r--r--   0        0        0      876 2022-11-14 15:08:03.540809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/locale/formats.js
--rw-r--r--   0        0        0      113 2022-11-14 15:08:03.572809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/locale/invalid.js
--rw-r--r--   0        0        0     2188 2022-11-14 15:08:03.594809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/locale/lists.js
--rw-r--r--   0        0        0      829 2022-11-14 15:08:03.596809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/locale/locale.js
--rw-r--r--   0        0        0     7728 2022-11-14 15:08:03.602810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/locale/locales.js
--rw-r--r--   0        0        0      218 2022-11-14 15:08:03.643810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/locale/ordinal.js
--rw-r--r--   0        0        0       66 2022-11-14 15:08:03.647810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/locale/pre-post-format.js
--rw-r--r--   0        0        0     2229 2022-11-14 15:08:03.648810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/locale/prototype.js
--rw-r--r--   0        0        0      842 2022-11-14 15:08:03.652810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/locale/relative.js
--rw-r--r--   0        0        0     1831 2022-11-14 15:08:03.656810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/locale/set.js
--rw-r--r--   0        0        0     1869 2022-11-14 15:08:03.419809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/moment/add-subtract.js
--rw-r--r--   0        0        0     1737 2022-11-14 15:08:03.467809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/moment/calendar.js
--rw-r--r--   0        0        0       98 2022-11-14 15:08:03.471809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/moment/clone.js
--rw-r--r--   0        0        0     2379 2022-11-14 15:08:03.471809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/moment/compare.js
--rw-r--r--   0        0        0     2106 2022-11-14 15:08:03.473809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/moment/constructor.js
--rw-r--r--   0        0        0      192 2022-11-14 15:08:03.475809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/moment/creation-data.js
--rw-r--r--   0        0        0     2345 2022-11-14 15:08:03.486809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/moment/diff.js
--rw-r--r--   0        0        0     2340 2022-11-14 15:08:03.539809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/moment/format.js
--rw-r--r--   0        0        0      609 2022-11-14 15:08:03.547809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/moment/from.js
--rw-r--r--   0        0        0     2041 2022-11-14 15:08:03.552809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/moment/get-set.js
--rw-r--r--   0        0        0      946 2022-11-14 15:08:03.596809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/moment/locale.js
--rw-r--r--   0        0        0     1922 2022-11-14 15:08:03.617810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/moment/min-max.js
--rw-r--r--   0        0        0      609 2022-11-14 15:08:03.636810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/moment/moment.js
--rw-r--r--   0        0        0       82 2022-11-14 15:08:03.643810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/moment/now.js
--rw-r--r--   0        0        0     5511 2022-11-14 15:08:03.648810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/moment/prototype.js
--rw-r--r--   0        0        0     4819 2022-11-14 15:08:03.661810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/moment/start-end-of.js
--rw-r--r--   0        0        0      834 2022-11-14 15:08:03.672810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/moment/to-type.js
--rw-r--r--   0        0        0      603 2022-11-14 15:08:03.672810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/moment/to.js
--rw-r--r--   0        0        0      364 2022-11-14 15:08:03.693810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/moment/valid.js
--rw-r--r--   0        0        0     2500 2022-11-14 15:08:03.652810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/parse/regex.js
--rw-r--r--   0        0        0      958 2022-11-14 15:08:03.672810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/parse/token.js
--rw-r--r--   0        0        0      809 2022-11-14 15:08:03.426809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/aliases.js
--rw-r--r--   0        0        0      148 2022-11-14 15:08:03.471809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/constants.js
--rw-r--r--   0        0        0     1065 2022-11-14 15:08:03.479809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/day-of-month.js
--rw-r--r--   0        0        0    12904 2022-11-14 15:08:03.480809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/day-of-week.js
--rw-r--r--   0        0        0      920 2022-11-14 15:08:03.480809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/day-of-year.js
--rw-r--r--   0        0        0     7984 2022-11-14 15:08:03.514809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/era.js
--rw-r--r--   0        0        0     4475 2022-11-14 15:08:03.564809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/hour.js
--rw-r--r--   0        0        0     1870 2022-11-14 15:08:03.616809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/millisecond.js
--rw-r--r--   0        0        0      679 2022-11-14 15:08:03.617810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/minute.js
--rw-r--r--   0        0        0    10021 2022-11-14 15:08:03.637810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/month.js
--rw-r--r--   0        0        0     7070 2022-11-14 15:08:03.643810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/offset.js
--rw-r--r--   0        0        0      480 2022-11-14 15:08:03.647810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/priorities.js
--rw-r--r--   0        0        0      780 2022-11-14 15:08:03.651810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/quarter.js
--rw-r--r--   0        0        0      679 2022-11-14 15:08:03.656810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/second.js
--rw-r--r--   0        0        0      590 2022-11-14 15:08:03.668810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/timestamp.js
--rw-r--r--   0        0        0      325 2022-11-14 15:08:03.668810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/timezone.js
--rw-r--r--   0        0        0      404 2022-11-14 15:08:03.689810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/units.js
--rw-r--r--   0        0        0     2107 2022-11-14 15:08:03.694810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/week-calendar-utils.js
--rw-r--r--   0        0        0     3483 2022-11-14 15:08:03.694810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/week-year.js
--rw-r--r--   0        0        0     1664 2022-11-14 15:08:03.694810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/week.js
--rw-r--r--   0        0        0     2001 2022-11-14 15:08:03.695810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/units/year.js
--rw-r--r--   0        0        0      154 2022-11-14 15:08:03.411809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/abs-ceil.js
--rw-r--r--   0        0        0      179 2022-11-14 15:08:03.411809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/abs-floor.js
--rw-r--r--   0        0        0      166 2022-11-14 15:08:03.412809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/abs-round.js
--rw-r--r--   0        0        0      553 2022-11-14 15:08:03.471809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/compare-arrays.js
--rw-r--r--   0        0        0      203 2022-11-14 15:08:03.486809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/defaults.js
--rw-r--r--   0        0        0     1946 2022-11-14 15:08:03.486809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/deprecate.js
--rw-r--r--   0        0        0      345 2022-11-14 15:08:03.526809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/extend.js
--rw-r--r--   0        0        0      100 2022-11-14 15:08:03.560809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/has-own-prop.js
--rw-r--r--   0        0        0      296 2022-11-14 15:08:03.563809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/hooks.js
--rw-r--r--   0        0        0      342 2022-11-14 15:08:03.572809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/index-of.js
--rw-r--r--   0        0        0      164 2022-11-14 15:08:03.573809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/is-array.js
--rw-r--r--   0        0        0      670 2022-11-14 15:08:03.573809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/is-calendar-spec.js
--rw-r--r--   0        0        0      161 2022-11-14 15:08:03.573809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/is-date.js
--rw-r--r--   0        0        0      210 2022-11-14 15:08:03.574809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/is-function.js
--rw-r--r--   0        0        0      106 2022-11-14 15:08:03.574809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/is-leap-year.js
--rw-r--r--   0        0        0     1988 2022-11-14 15:08:03.574809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/is-moment-input.js
--rw-r--r--   0        0        0      169 2022-11-14 15:08:03.575809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/is-number.js
--rw-r--r--   0        0        0      360 2022-11-14 15:08:03.575809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/is-object-empty.js
--rw-r--r--   0        0        0      246 2022-11-14 15:08:03.576810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/is-object.js
--rw-r--r--   0        0        0      109 2022-11-14 15:08:03.576810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/is-string.js
--rw-r--r--   0        0        0       76 2022-11-14 15:08:03.576810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/is-undefined.js
--rw-r--r--   0        0        0      344 2022-11-14 15:08:03.584809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/keys.js
--rw-r--r--   0        0        0      189 2022-11-14 15:08:03.613809 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/map.js
--rw-r--r--   0        0        0       68 2022-11-14 15:08:03.622810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/mod.js
--rw-r--r--   0        0        0      394 2022-11-14 15:08:03.658810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/some.js
--rw-r--r--   0        0        0      282 2022-11-14 15:08:03.671810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/to-int.js
--rw-r--r--   0        0        0      352 2022-11-14 15:08:03.697810 anitya-1.8.1/anitya/static/node_modules/moment/src/lib/utils/zero-fill.js
--rw-r--r--   0        0        0     2149 2022-11-14 15:08:03.424809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/af.js
--rw-r--r--   0        0        0     4449 2022-11-14 15:08:03.428809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ar-dz.js
--rw-r--r--   0        0        0     1934 2022-11-14 15:08:03.429809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ar-kw.js
--rw-r--r--   0        0        0     4648 2022-11-14 15:08:03.432809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ar-ly.js
--rw-r--r--   0        0        0     1989 2022-11-14 15:08:03.436809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ar-ma.js
--rw-r--r--   0        0        0     3042 2022-11-14 15:08:03.438809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ar-sa.js
--rw-r--r--   0        0        0     1936 2022-11-14 15:08:03.439809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ar-tn.js
--rw-r--r--   0        0        0     5072 2022-11-14 15:08:03.441809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ar.js
--rw-r--r--   0        0        0     2846 2022-11-14 15:08:03.449809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/az.js
--rw-r--r--   0        0        0     5154 2022-11-14 15:08:03.454809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/be.js
--rw-r--r--   0        0        0     2955 2022-11-14 15:08:03.456809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/bg.js
--rw-r--r--   0        0        0     1784 2022-11-14 15:08:03.459809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/bm.js
--rw-r--r--   0        0        0     4349 2022-11-14 15:08:03.460809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/bn-bd.js
--rw-r--r--   0        0        0     3898 2022-11-14 15:08:03.462809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/bn.js
--rw-r--r--   0        0        0     4399 2022-11-14 15:08:03.464809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/bo.js
--rw-r--r--   0        0        0     4544 2022-11-14 15:08:03.465809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/br.js
--rw-r--r--   0        0        0     4475 2022-11-14 15:08:03.466809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/bs.js
--rw-r--r--   0        0        0     3031 2022-11-14 15:08:03.467809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ca.js
--rw-r--r--   0        0        0     6718 2022-11-14 15:08:03.476809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/cs.js
--rw-r--r--   0        0        0     2341 2022-11-14 15:08:03.476809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/cv.js
--rw-r--r--   0        0        0     2834 2022-11-14 15:08:03.478809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/cy.js
--rw-r--r--   0        0        0     1629 2022-11-14 15:08:03.478809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/da.js
--rw-r--r--   0        0        0     2635 2022-11-14 15:08:03.481809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/de-at.js
--rw-r--r--   0        0        0     2563 2022-11-14 15:08:03.483809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/de-ch.js
--rw-r--r--   0        0        0     2562 2022-11-14 15:08:03.485809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/de.js
--rw-r--r--   0        0        0     2464 2022-11-14 15:08:03.488809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/dv.js
--rw-r--r--   0        0        0     3877 2022-11-14 15:08:03.489809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/el.js
--rw-r--r--   0        0        0     2029 2022-11-14 15:08:03.491809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/en-au.js
--rw-r--r--   0        0        0     1878 2022-11-14 15:08:03.492809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/en-ca.js
--rw-r--r--   0        0        0     2035 2022-11-14 15:08:03.494809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/en-gb.js
--rw-r--r--   0        0        0     2033 2022-11-14 15:08:03.497809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/en-ie.js
--rw-r--r--   0        0        0     1871 2022-11-14 15:08:03.500809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/en-il.js
--rw-r--r--   0        0        0     2029 2022-11-14 15:08:03.502809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/en-in.js
--rw-r--r--   0        0        0     2038 2022-11-14 15:08:03.504809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/en-nz.js
--rw-r--r--   0        0        0     2047 2022-11-14 15:08:03.510809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/en-sg.js
--rw-r--r--   0        0        0     2338 2022-11-14 15:08:03.513809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/eo.js
--rw-r--r--   0        0        0     3441 2022-11-14 15:08:03.517809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/es-do.js
--rw-r--r--   0        0        0     3510 2022-11-14 15:08:03.518809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/es-mx.js
--rw-r--r--   0        0        0     3538 2022-11-14 15:08:03.521809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/es-us.js
--rw-r--r--   0        0        0     3498 2022-11-14 15:08:03.523809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/es.js
--rw-r--r--   0        0        0     2631 2022-11-14 15:08:03.524809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/et.js
--rw-r--r--   0        0        0     1964 2022-11-14 15:08:03.526809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/eu.js
--rw-r--r--   0        0        0     3230 2022-11-14 15:08:03.527809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/fa.js
--rw-r--r--   0        0        0     3632 2022-11-14 15:08:03.529809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/fi.js
--rw-r--r--   0        0        0     1776 2022-11-14 15:08:03.531809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/fil.js
--rw-r--r--   0        0        0     1772 2022-11-14 15:08:03.534809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/fo.js
--rw-r--r--   0        0        0     2104 2022-11-14 15:08:03.541809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/fr-ca.js
--rw-r--r--   0        0        0     2263 2022-11-14 15:08:03.543809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/fr-ch.js
--rw-r--r--   0        0        0     3471 2022-11-14 15:08:03.544809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/fr.js
--rw-r--r--   0        0        0     2275 2022-11-14 15:08:03.549809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/fy.js
--rw-r--r--   0        0        0     2360 2022-11-14 15:08:03.550809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ga.js
--rw-r--r--   0        0        0     2380 2022-11-14 15:08:03.551809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/gd.js
--rw-r--r--   0        0        0     2347 2022-11-14 15:08:03.555809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/gl.js
--rw-r--r--   0        0        0     5506 2022-11-14 15:08:03.556809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/gom-deva.js
--rw-r--r--   0        0        0     4130 2022-11-14 15:08:03.558809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/gom-latn.js
--rw-r--r--   0        0        0     4132 2022-11-14 15:08:03.559809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/gu.js
--rw-r--r--   0        0        0     3211 2022-11-14 15:08:03.561809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/he.js
--rw-r--r--   0        0        0     6421 2022-11-14 15:08:03.563809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/hi.js
--rw-r--r--   0        0        0     4718 2022-11-14 15:08:03.566809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/hr.js
--rw-r--r--   0        0        0     3815 2022-11-14 15:08:03.567809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/hu.js
--rw-r--r--   0        0        0     3236 2022-11-14 15:08:03.570809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/hy-am.js
--rw-r--r--   0        0        0     2375 2022-11-14 15:08:03.571809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/id.js
--rw-r--r--   0        0        0     4458 2022-11-14 15:08:03.577809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/is.js
--rw-r--r--   0        0        0     1941 2022-11-14 15:08:03.579810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/it-ch.js
--rw-r--r--   0        0        0     3251 2022-11-14 15:08:03.580809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/it.js
--rw-r--r--   0        0        0     3955 2022-11-14 15:08:03.581809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ja.js
--rw-r--r--   0        0        0     2384 2022-11-14 15:08:03.583809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/jv.js
--rw-r--r--   0        0        0     3504 2022-11-14 15:08:03.584809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ka.js
--rw-r--r--   0        0        0     2495 2022-11-14 15:08:03.585809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/kk.js
--rw-r--r--   0        0        0     3362 2022-11-14 15:08:03.587809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/km.js
--rw-r--r--   0        0        0     4252 2022-11-14 15:08:03.588809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/kn.js
--rw-r--r--   0        0        0     2223 2022-11-14 15:08:03.590809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ko.js
--rw-r--r--   0        0        0     3330 2022-11-14 15:08:03.591809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ku.js
--rw-r--r--   0        0        0     2521 2022-11-14 15:08:03.592810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ky.js
--rw-r--r--   0        0        0     4269 2022-11-14 15:08:03.594809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/lb.js
--rw-r--r--   0        0        0     2585 2022-11-14 15:08:03.595810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/lo.js
--rw-r--r--   0        0        0     4005 2022-11-14 15:08:03.610809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/lt.js
--rw-r--r--   0        0        0     3449 2022-11-14 15:08:03.613809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/lv.js
--rw-r--r--   0        0        0     3661 2022-11-14 15:08:03.614810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/me.js
--rw-r--r--   0        0        0     2023 2022-11-14 15:08:03.616809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/mi.js
--rw-r--r--   0        0        0     3021 2022-11-14 15:08:03.619809 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/mk.js
--rw-r--r--   0        0        0     3287 2022-11-14 15:08:03.620810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ml.js
--rw-r--r--   0        0        0     3414 2022-11-14 15:08:03.621810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/mn.js
--rw-r--r--   0        0        0     6574 2022-11-14 15:08:03.637810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/mr.js
--rw-r--r--   0        0        0     2330 2022-11-14 15:08:03.638810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ms-my.js
--rw-r--r--   0        0        0     2277 2022-11-14 15:08:03.638810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ms.js
--rw-r--r--   0        0        0     1684 2022-11-14 15:08:03.639810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/mt.js
--rw-r--r--   0        0        0     3094 2022-11-14 15:08:03.640810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/my.js
--rw-r--r--   0        0        0     1899 2022-11-14 15:08:03.640810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/nb.js
--rw-r--r--   0        0        0     4031 2022-11-14 15:08:03.641810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ne.js
--rw-r--r--   0        0        0     3169 2022-11-14 15:08:03.641810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/nl-be.js
--rw-r--r--   0        0        0     3202 2022-11-14 15:08:03.642810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/nl.js
--rw-r--r--   0        0        0     1828 2022-11-14 15:08:03.642810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/nn.js
--rw-r--r--   0        0        0     2472 2022-11-14 15:08:03.643810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/oc-lnc.js
--rw-r--r--   0        0        0     4198 2022-11-14 15:08:03.646810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/pa-in.js
--rw-r--r--   0        0        0     4166 2022-11-14 15:08:03.647810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/pl.js
--rw-r--r--   0        0        0     1854 2022-11-14 15:08:03.650810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/pt-br.js
--rw-r--r--   0        0        0     1968 2022-11-14 15:08:03.650810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/pt.js
--rw-r--r--   0        0        0     2319 2022-11-14 15:08:03.652810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ro.js
--rw-r--r--   0        0        0     8418 2022-11-14 15:08:03.654810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ru.js
--rw-r--r--   0        0        0     2153 2022-11-14 15:08:03.655810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/sd.js
--rw-r--r--   0        0        0     1849 2022-11-14 15:08:03.656810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/se.js
--rw-r--r--   0        0        0     2681 2022-11-14 15:08:03.656810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/si.js
--rw-r--r--   0        0        0     5173 2022-11-14 15:08:03.657810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/sk.js
--rw-r--r--   0        0        0     6115 2022-11-14 15:08:03.658810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/sl.js
--rw-r--r--   0        0        0     1987 2022-11-14 15:08:03.658810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/sq.js
--rw-r--r--   0        0        0     4762 2022-11-14 15:08:03.659810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/sr-cyrl.js
--rw-r--r--   0        0        0     4209 2022-11-14 15:08:03.660810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/sr.js
--rw-r--r--   0        0        0     2572 2022-11-14 15:08:03.661810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ss.js
--rw-r--r--   0        0        0     2066 2022-11-14 15:08:03.663810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/sv.js
--rw-r--r--   0        0        0     1651 2022-11-14 15:08:03.663810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/sw.js
--rw-r--r--   0        0        0     4800 2022-11-14 15:08:03.664810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ta.js
--rw-r--r--   0        0        0     3392 2022-11-14 15:08:03.665810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/te.js
--rw-r--r--   0        0        0     2155 2022-11-14 15:08:03.666810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/tet.js
--rw-r--r--   0        0        0     3604 2022-11-14 15:08:03.667810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/tg.js
--rw-r--r--   0        0        0     2736 2022-11-14 15:08:03.668810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/th.js
--rw-r--r--   0        0        0     2488 2022-11-14 15:08:03.669810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/tk.js
--rw-r--r--   0        0        0     1735 2022-11-14 15:08:03.670810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/tl-ph.js
--rw-r--r--   0        0        0     3755 2022-11-14 15:08:03.671810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/tlh.js
--rw-r--r--   0        0        0     2927 2022-11-14 15:08:03.673810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/tr.js
--rw-r--r--   0        0        0     3109 2022-11-14 15:08:03.674810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/tzl.js
--rw-r--r--   0        0        0     1691 2022-11-14 15:08:03.675810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/tzm-latn.js
--rw-r--r--   0        0        0     2322 2022-11-14 15:08:03.681810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/tzm.js
--rw-r--r--   0        0        0     3880 2022-11-14 15:08:03.688810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ug-cn.js
--rw-r--r--   0        0        0     5955 2022-11-14 15:08:03.689810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/uk.js
--rw-r--r--   0        0        0     2200 2022-11-14 15:08:03.690810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/ur.js
--rw-r--r--   0        0        0     1639 2022-11-14 15:08:03.691810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/uz-latn.js
--rw-r--r--   0        0        0     1885 2022-11-14 15:08:03.692810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/uz.js
--rw-r--r--   0        0        0     2430 2022-11-14 15:08:03.694810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/vi.js
--rw-r--r--   0        0        0     2348 2022-11-14 15:08:03.695810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/x-pseudo.js
--rw-r--r--   0        0        0     1887 2022-11-14 15:08:03.696810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/yo.js
--rw-r--r--   0        0        0     3711 2022-11-14 15:08:03.700810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/zh-cn.js
--rw-r--r--   0        0        0     3116 2022-11-14 15:08:03.701810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/zh-hk.js
--rw-r--r--   0        0        0     3066 2022-11-14 15:08:03.701810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/zh-mo.js
--rw-r--r--   0        0        0     3013 2022-11-14 15:08:03.702810 anitya-1.8.1/anitya/static/node_modules/moment/src/locale/zh-tw.js
--rw-r--r--   0        0        0     2694 2022-11-14 15:08:03.636810 anitya-1.8.1/anitya/static/node_modules/moment/src/moment.js
--rw-r--r--   0        0        0    23327 2022-11-14 15:08:03.705810 anitya-1.8.1/anitya/static/node_modules/moment/ts3.1-typings/moment.d.ts
--rw-r--r--   0        0        0     3584 2023-04-26 13:29:52.886981 anitya-1.8.1/anitya/static/package-lock.json
--rw-r--r--   0        0        0      765 2023-01-26 12:16:19.281657 anitya-1.8.1/anitya/static/package.json
--rw-r--r--   0        0        0     2970 2020-12-02 09:02:04.993902 anitya-1.8.1/anitya/static/yahoo_logo.png
--rw-r--r--   0        0        0        0 2020-12-02 09:02:04.993902 anitya-1.8.1/anitya/templates/__init__.py
--rw-r--r--   0        0        0     3236 2023-01-26 12:16:19.281657 anitya-1.8.1/anitya/templates/distro_add_edit.html
--rw-r--r--   0        0        0      596 2023-01-26 12:16:19.282657 anitya-1.8.1/anitya/templates/distro_delete.html
--rw-r--r--   0        0        0     2293 2023-01-26 12:16:19.282657 anitya-1.8.1/anitya/templates/distros.html
--rw-r--r--   0        0        0     4148 2023-01-26 12:16:19.282657 anitya-1.8.1/anitya/templates/flags.html
--rw-r--r--   0        0        0      438 2020-12-02 09:02:04.994902 anitya-1.8.1/anitya/templates/functions.html
--rw-r--r--   0        0        0     1626 2023-01-26 12:16:19.282657 anitya-1.8.1/anitya/templates/index.html
--rw-r--r--   0        0        0     1019 2023-01-26 12:16:19.283657 anitya-1.8.1/anitya/templates/login.html
--rw-r--r--   0        0        0     2388 2023-01-26 12:16:19.283657 anitya-1.8.1/anitya/templates/logs.html
--rw-r--r--   0        0        0     1762 2023-01-26 12:16:19.283657 anitya-1.8.1/anitya/templates/mapping.html
--rw-r--r--   0        0        0     9973 2023-05-26 06:47:55.383118 anitya-1.8.1/anitya/templates/master.html
--rw-r--r--   0        0        0    14996 2023-05-26 06:47:55.384117 anitya-1.8.1/anitya/templates/project.html
--rw-r--r--   0        0        0     3734 2023-01-26 12:16:19.284657 anitya-1.8.1/anitya/templates/project_archive.html
--rw-r--r--   0        0        0     3053 2023-01-26 12:16:19.285657 anitya-1.8.1/anitya/templates/project_delete.html
--rw-r--r--   0        0        0     1134 2023-01-26 12:16:19.285657 anitya-1.8.1/anitya/templates/project_flag.html
--rw-r--r--   0        0        0    17245 2023-01-26 12:16:19.285657 anitya-1.8.1/anitya/templates/project_new.html
--rw-r--r--   0        0        0      999 2023-01-26 12:16:19.286657 anitya-1.8.1/anitya/templates/project_versions_delete.html
--rw-r--r--   0        0        0     3751 2023-01-26 12:16:19.286657 anitya-1.8.1/anitya/templates/projects.html
--rw-r--r--   0        0        0     1354 2023-01-26 12:16:19.286657 anitya-1.8.1/anitya/templates/regex_delete.html
--rw-r--r--   0        0        0     3543 2023-01-26 12:16:19.286657 anitya-1.8.1/anitya/templates/search.html
--rw-r--r--   0        0        0     2101 2023-01-26 12:16:19.286657 anitya-1.8.1/anitya/templates/settings.html
--rw-r--r--   0        0        0     4848 2023-01-26 12:16:19.286657 anitya-1.8.1/anitya/templates/updates.html
--rw-r--r--   0        0        0     4393 2023-01-26 12:16:19.286657 anitya-1.8.1/anitya/templates/users.html
--rw-r--r--   0        0        0     1250 2023-01-26 12:16:19.286657 anitya-1.8.1/anitya/templates/version_delete.html
--rw-r--r--   0        0        0    24109 2023-05-26 06:47:55.389117 anitya-1.8.1/anitya/ui.py
--rw-r--r--   0        0        0      834 2023-05-26 06:47:55.389117 anitya-1.8.1/anitya/wsgi.py
--rw-r--r--   0        0        0     1866 2020-12-02 09:02:05.011902 anitya-1.8.1/createdb.py
--rw-r--r--   0        0        0     3954 2022-12-14 14:15:41.913739 anitya-1.8.1/files/anitya.toml.sample
--rw-r--r--   0        0        0      364 2020-12-02 09:02:05.012902 anitya-1.8.1/files/config.toml.sample
--rw-r--r--   0        0        0     3801 2023-05-26 07:00:42.382882 anitya-1.8.1/pyproject.toml
--rw-r--r--   0        0        0    16729 1970-01-01 00:00:00.000000 anitya-1.8.1/setup.py
--rw-r--r--   0        0        0     4006 1970-01-01 00:00:00.000000 anitya-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0    18002 2023-07-24 10:27:37.622622 anitya-1.9.0/LICENSE
+-rw-r--r--   0        0        0     1617 2024-01-30 14:15:57.692727 anitya-1.9.0/README.rst
+-rw-r--r--   0        0        0     1184 2023-07-24 10:27:37.622622 anitya-1.9.0/alembic.ini
+-rw-r--r--   0        0        0      147 2023-07-24 10:27:37.622622 anitya-1.9.0/anitya/__init__.py
+-rw-r--r--   0        0        0    18625 2023-07-24 10:27:37.622622 anitya-1.9.0/anitya/admin.py
+-rw-r--r--   0        0        0    15210 2024-01-15 14:30:42.753709 anitya-1.9.0/anitya/api.py
+-rw-r--r--   0        0        0    31914 2024-01-15 14:30:42.753709 anitya-1.9.0/anitya/api_v2.py
+-rw-r--r--   0        0        0     7673 2024-01-15 14:30:42.754709 anitya-1.9.0/anitya/app.py
+-rw-r--r--   0        0        0     4449 2023-07-24 10:27:37.622622 anitya-1.9.0/anitya/authentication.py
+-rw-r--r--   0        0        0    11780 2024-01-15 14:30:42.754709 anitya-1.9.0/anitya/check_service.py
+-rw-r--r--   0        0        0     1203 2024-01-15 14:30:42.754709 anitya-1.9.0/anitya/compat.py
+-rw-r--r--   0        0        0     6092 2024-01-15 14:30:42.754709 anitya-1.9.0/anitya/config.py
+-rw-r--r--   0        0        0     1396 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/__init__.py
+-rw-r--r--   0        0        0     3132 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/events.py
+-rw-r--r--   0        0        0     5817 2024-01-15 14:30:42.754709 anitya-1.9.0/anitya/db/meta.py
+-rw-r--r--   0        0        0      464 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/README.md
+-rw-r--r--   0        0        0        0 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/__init__.py
+-rw-r--r--   0        0        0     2116 2024-01-30 14:15:57.692727 anitya-1.9.0/anitya/db/migrations/env.py
+-rw-r--r--   0        0        0      413 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/script.py.mako
+-rw-r--r--   0        0        0      745 2024-01-15 14:30:42.754709 anitya-1.9.0/anitya/db/migrations/versions/136d119ab015_rename_project_latest_known_cursor_to_.py
+-rw-r--r--   0        0        0      579 2024-01-15 14:30:42.754709 anitya-1.9.0/anitya/db/migrations/versions/16aa7da2764c_add_projectversion_commit_url.py
+-rw-r--r--   0        0        0      591 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/1ab95561edae_convert_date_to_rpm.py
+-rw-r--r--   0        0        0     1390 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/1bf8aead6179_add_check_times.py
+-rw-r--r--   0        0        0      662 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/1f839c54e428_add_archive_flag.py
+-rw-r--r--   0        0        0      634 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/24b6734e8565_creation_date_on_version.py
+-rw-r--r--   0        0        0      746 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/27342bce1d0f_populate_project_version_scheme.py
+-rw-r--r--   0        0        0      591 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/2925648d8cc3_add_a_version_prefix_field.py
+-rw-r--r--   0        0        0      556 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/2d1aa7ff82a5_remove_code_google_backend.py
+-rw-r--r--   0        0        0      802 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/314651690dc7_add_error_counter_to_project.py
+-rw-r--r--   0        0        0     1809 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/34b9bb5fa388_make_ecosystem_non_nullable.py
+-rw-r--r--   0        0        0     3746 2024-01-15 14:30:42.754709 anitya-1.9.0/anitya/db/migrations/versions/3fae8239eeec_add_an_api_token_table.py
+-rw-r--r--   0        0        0      881 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/540bdcf7edbc_convert_github_url_to_owner_project.py
+-rw-r--r--   0        0        0      676 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/571bd07533a9_add_insecure_column_to_projects_table.py
+-rw-r--r--   0        0        0      589 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/5b8b587d7dbe_add_version_filter_column.py
+-rw-r--r--   0        0        0      694 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/5e209766aead_add_release_check_to_project.py
+-rw-r--r--   0        0        0     1737 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/6ac0e42df937_drop_logs_table.py
+-rw-r--r--   0        0        0      556 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/708f6f26b4b6_add_version_pattern.py
+-rw-r--r--   0        0        0     1022 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/7a8c4aa92678_add_missing_github_owner_project_pairs.py
+-rw-r--r--   0        0        0      610 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/8040ef9a9dda_add_a_version_scheme_column_to_projects.py
+-rw-r--r--   0        0        0      683 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/8be6e153962c_remove_cursor.py
+-rw-r--r--   0        0        0     1008 2024-01-15 14:30:42.754709 anitya-1.9.0/anitya/db/migrations/versions/921c612ba0da_model_upstream_ecosystems.py
+-rw-r--r--   0        0        0      581 2024-01-15 14:30:42.754709 anitya-1.9.0/anitya/db/migrations/versions/92a2e9eba0a7_add_project_latest_known_cursor.py
+-rw-r--r--   0        0        0      966 2024-01-15 14:30:42.754709 anitya-1.9.0/anitya/db/migrations/versions/9c29da0af3af_populate_ecosystem_data.py
+-rw-r--r--   0        0        0        0 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/__init__.py
+-rw-r--r--   0        0        0     3151 2024-01-30 14:15:57.692727 anitya-1.9.0/anitya/db/migrations/versions/a52d2fe99d4f_users.py
+-rw-r--r--   0        0        0      339 2024-01-15 14:30:42.754709 anitya-1.9.0/anitya/db/migrations/versions/ac10bf3f974c_.py
+-rw-r--r--   0        0        0      494 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/b13662e5d288_add_admin_flag.py
+-rw-r--r--   0        0        0     2809 2024-01-15 14:30:42.754709 anitya-1.9.0/anitya/db/migrations/versions/b9201d816075_remove_the_backends_and_ecosystems_.py
+-rw-r--r--   0        0        0      429 2024-01-15 14:30:42.754709 anitya-1.9.0/anitya/db/migrations/versions/c8735fa14a0a_add_cascade_delete.py
+-rw-r--r--   0        0        0      595 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/d6170cfc2814_add_pre_release_flag.py
+-rw-r--r--   0        0        0     1147 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/db/migrations/versions/e34988f3e2f4_add_statistics_to_run.py
+-rw-r--r--   0        0        0     6606 2024-01-15 14:30:42.754709 anitya-1.9.0/anitya/db/migrations/versions/feeaa70ead67_social_authentication_table.py
+-rw-r--r--   0        0        0    36764 2024-01-30 14:15:57.692727 anitya-1.9.0/anitya/db/models.py
+-rw-r--r--   0        0        0     3577 2024-01-15 14:30:42.754709 anitya-1.9.0/anitya/forms.py
+-rw-r--r--   0        0        0      152 2023-07-24 10:27:37.623622 anitya-1.9.0/anitya/lib/__init__.py
+-rw-r--r--   0        0        0    15797 2024-01-15 14:30:42.755710 anitya-1.9.0/anitya/lib/backends/__init__.py
+-rw-r--r--   0        0        0     2927 2024-01-15 14:30:42.755710 anitya-1.9.0/anitya/lib/backends/bitbucket.py
+-rw-r--r--   0        0        0     3113 2024-01-15 14:30:42.755710 anitya-1.9.0/anitya/lib/backends/cgit.py
+-rw-r--r--   0        0        0     3067 2024-01-15 14:30:42.755710 anitya-1.9.0/anitya/lib/backends/cpan.py
+-rw-r--r--   0        0        0     7633 2024-01-15 14:30:42.755710 anitya-1.9.0/anitya/lib/backends/cran.py
+-rw-r--r--   0        0        0     8623 2024-01-15 14:30:42.755710 anitya-1.9.0/anitya/lib/backends/crates.py
+-rw-r--r--   0        0        0     2851 2024-01-15 14:30:42.755710 anitya-1.9.0/anitya/lib/backends/custom.py
+-rw-r--r--   0        0        0     2871 2024-01-15 14:30:42.755710 anitya-1.9.0/anitya/lib/backends/debian.py
+-rw-r--r--   0        0        0     3441 2024-01-15 14:30:42.755710 anitya-1.9.0/anitya/lib/backends/drupal6.py
+-rw-r--r--   0        0        0     3128 2024-01-15 14:30:42.755710 anitya-1.9.0/anitya/lib/backends/drupal7.py
+-rw-r--r--   0        0        0     3229 2024-01-15 14:30:42.755710 anitya-1.9.0/anitya/lib/backends/folder.py
+-rw-r--r--   0        0        0     2432 2024-01-15 14:30:42.755710 anitya-1.9.0/anitya/lib/backends/freshmeat.py
+-rw-r--r--   0        0        0     3997 2024-01-15 14:30:42.755710 anitya-1.9.0/anitya/lib/backends/gitea.py
+-rw-r--r--   0        0        0     9851 2024-01-15 14:30:42.755710 anitya-1.9.0/anitya/lib/backends/github.py
+-rw-r--r--   0        0        0     4776 2024-01-15 14:30:42.755710 anitya-1.9.0/anitya/lib/backends/gitlab.py
+-rw-r--r--   0        0        0     3576 2024-01-15 14:30:42.755710 anitya-1.9.0/anitya/lib/backends/gnome.py
+-rw-r--r--   0        0        0     3144 2024-01-15 14:30:42.755710 anitya-1.9.0/anitya/lib/backends/gnu.py
+-rw-r--r--   0        0        0     3506 2024-01-15 14:30:42.755710 anitya-1.9.0/anitya/lib/backends/gogs.py
+-rw-r--r--   0        0        0     2219 2024-01-15 14:30:42.756709 anitya-1.9.0/anitya/lib/backends/hackage.py
+-rw-r--r--   0        0        0     2357 2024-01-15 14:30:42.756709 anitya-1.9.0/anitya/lib/backends/launchpad.py
+-rw-r--r--   0        0        0     3107 2024-01-15 14:30:42.756709 anitya-1.9.0/anitya/lib/backends/maven.py
+-rw-r--r--   0        0        0     5196 2024-01-15 14:30:42.756709 anitya-1.9.0/anitya/lib/backends/npmjs.py
+-rw-r--r--   0        0        0     4081 2024-01-15 14:30:42.756709 anitya-1.9.0/anitya/lib/backends/packagist.py
+-rw-r--r--   0        0        0     3643 2024-01-15 14:30:42.756709 anitya-1.9.0/anitya/lib/backends/pagure.py
+-rw-r--r--   0        0        0     4418 2024-01-15 14:30:42.756709 anitya-1.9.0/anitya/lib/backends/pear.py
+-rw-r--r--   0        0        0     4407 2024-01-15 14:30:42.756709 anitya-1.9.0/anitya/lib/backends/pecl.py
+-rw-r--r--   0        0        0     5131 2024-01-15 14:30:42.756709 anitya-1.9.0/anitya/lib/backends/pypi.py
+-rw-r--r--   0        0        0     3527 2024-01-15 14:30:42.756709 anitya-1.9.0/anitya/lib/backends/rubygems.py
+-rw-r--r--   0        0        0     2866 2024-01-15 14:30:42.756709 anitya-1.9.0/anitya/lib/backends/sourceforge.py
+-rw-r--r--   0        0        0     4837 2024-01-15 14:30:42.756709 anitya-1.9.0/anitya/lib/backends/sourceforge_git.py
+-rw-r--r--   0        0        0     3991 2024-01-15 14:30:42.756709 anitya-1.9.0/anitya/lib/backends/sourcehut.py
+-rw-r--r--   0        0        0     2516 2024-01-15 14:30:42.756709 anitya-1.9.0/anitya/lib/backends/stackage.py
+-rw-r--r--   0        0        0     1087 2023-07-24 10:27:37.625622 anitya-1.9.0/anitya/lib/ecosystems/__init__.py
+-rw-r--r--   0        0        0     1072 2023-07-24 10:27:37.625622 anitya-1.9.0/anitya/lib/ecosystems/crates.py
+-rw-r--r--   0        0        0      278 2023-07-24 10:27:37.625622 anitya-1.9.0/anitya/lib/ecosystems/maven.py
+-rw-r--r--   0        0        0      264 2023-07-24 10:27:37.625622 anitya-1.9.0/anitya/lib/ecosystems/npm.py
+-rw-r--r--   0        0        0      266 2023-07-24 10:27:37.625622 anitya-1.9.0/anitya/lib/ecosystems/pypi.py
+-rw-r--r--   0        0        0      282 2023-07-24 10:27:37.625622 anitya-1.9.0/anitya/lib/ecosystems/rubygems.py
+-rw-r--r--   0        0        0     3800 2024-01-15 14:30:42.756709 anitya-1.9.0/anitya/lib/exceptions.py
+-rw-r--r--   0        0        0     3430 2023-07-24 10:27:37.625622 anitya-1.9.0/anitya/lib/plugins.py
+-rw-r--r--   0        0        0    18431 2024-01-15 14:30:42.756709 anitya-1.9.0/anitya/lib/utilities.py
+-rw-r--r--   0        0        0     2185 2023-07-24 10:27:37.625622 anitya-1.9.0/anitya/lib/versions/__init__.py
+-rw-r--r--   0        0        0     9347 2024-01-30 14:15:57.692727 anitya-1.9.0/anitya/lib/versions/base.py
+-rw-r--r--   0        0        0    15187 2024-01-30 14:15:57.692727 anitya-1.9.0/anitya/lib/versions/calver.py
+-rw-r--r--   0        0        0     6349 2024-01-30 14:15:57.692727 anitya-1.9.0/anitya/lib/versions/python.py
+-rw-r--r--   0        0        0     7352 2024-01-30 14:15:57.692727 anitya-1.9.0/anitya/lib/versions/rpm.py
+-rw-r--r--   0        0        0     3626 2024-01-30 14:15:57.692727 anitya-1.9.0/anitya/lib/versions/semver.py
+-rw-r--r--   0        0        0     2879 2024-01-15 14:30:42.756709 anitya-1.9.0/anitya/lib/xml2dict.py
+-rw-r--r--   0        0        0     6250 2024-01-15 14:30:42.756709 anitya-1.9.0/anitya/mail_logging.py
+-rw-r--r--   0        0        0     2932 2024-01-15 14:30:42.756709 anitya-1.9.0/anitya/sar.py
+-rw-r--r--   0        0        0       54 2023-07-24 10:27:37.625622 anitya-1.9.0/anitya/static/css/avatars.css
+-rw-r--r--   0        0        0      888 2023-07-24 10:27:37.625622 anitya-1.9.0/anitya/static/css/cnucnu.css
+-rw-r--r--   0        0        0    24734 2023-07-24 10:27:37.625622 anitya-1.9.0/anitya/static/css/fonts/Cantarell-Bold-webfont.eot
+-rw-r--r--   0        0        0    28113 2023-07-24 10:27:37.625622 anitya-1.9.0/anitya/static/css/fonts/Cantarell-Bold-webfont.svg
+-rw-r--r--   0        0        0    49276 2023-07-24 10:27:37.626622 anitya-1.9.0/anitya/static/css/fonts/Cantarell-Bold-webfont.ttf
+-rw-r--r--   0        0        0    16708 2023-07-24 10:27:37.626622 anitya-1.9.0/anitya/static/css/fonts/Cantarell-Bold-webfont.woff
+-rw-r--r--   0        0        0    27450 2023-07-24 10:27:37.626622 anitya-1.9.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.eot
+-rw-r--r--   0        0        0    29130 2023-07-24 10:27:37.626622 anitya-1.9.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.svg
+-rw-r--r--   0        0        0    52200 2023-07-24 10:27:37.626622 anitya-1.9.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.ttf
+-rw-r--r--   0        0        0    17988 2023-07-24 10:27:37.626622 anitya-1.9.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.woff
+-rw-r--r--   0        0        0    27610 2023-07-24 10:27:37.626622 anitya-1.9.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.eot
+-rw-r--r--   0        0        0    29402 2023-07-24 10:27:37.627622 anitya-1.9.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.svg
+-rw-r--r--   0        0        0    50068 2023-07-24 10:27:37.627622 anitya-1.9.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.ttf
+-rw-r--r--   0        0        0    17980 2023-07-24 10:27:37.627622 anitya-1.9.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.woff
+-rw-r--r--   0        0        0    24350 2023-07-24 10:27:37.627622 anitya-1.9.0/anitya/static/css/fonts/Cantarell-Regular-webfont.eot
+-rw-r--r--   0        0        0    28095 2023-07-24 10:27:37.627622 anitya-1.9.0/anitya/static/css/fonts/Cantarell-Regular-webfont.svg
+-rw-r--r--   0        0        0    47504 2023-07-24 10:27:37.627622 anitya-1.9.0/anitya/static/css/fonts/Cantarell-Regular-webfont.ttf
+-rw-r--r--   0        0        0    16400 2023-07-24 10:27:37.627622 anitya-1.9.0/anitya/static/css/fonts/Cantarell-Regular-webfont.woff
+-rw-r--r--   0        0        0    94588 2023-07-24 10:27:37.628622 anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.eot
+-rw-r--r--   0        0        0   171329 2023-07-24 10:27:37.628622 anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.svg
+-rw-r--r--   0        0        0   170608 2023-07-24 10:27:37.629622 anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.ttf
+-rw-r--r--   0        0        0    56608 2023-07-24 10:27:37.629622 anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.woff
+-rw-r--r--   0        0        0    91164 2023-07-24 10:27:37.629622 anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.eot
+-rw-r--r--   0        0        0   169419 2023-07-24 10:27:37.630622 anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.svg
+-rw-r--r--   0        0        0   170388 2023-07-24 10:27:37.630622 anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.ttf
+-rw-r--r--   0        0        0    54684 2023-07-24 10:27:37.630622 anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.woff
+-rw-r--r--   0        0        0    95020 2023-07-24 10:27:37.631622 anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.eot
+-rw-r--r--   0        0        0   167898 2023-07-24 10:27:37.631622 anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.svg
+-rw-r--r--   0        0        0   170308 2023-07-24 10:27:37.632622 anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.ttf
+-rw-r--r--   0        0        0    56100 2023-07-24 10:27:37.632622 anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.woff
+-rw-r--r--   0        0        0      279 2023-07-24 10:27:37.632622 anitya-1.9.0/anitya/static/css/footer.css
+-rw-r--r--   0        0        0      212 2023-07-24 10:27:37.632622 anitya-1.9.0/anitya/static/css/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rw-r--r--   0        0        0      220 2023-07-24 10:27:37.632622 anitya-1.9.0/anitya/static/css/images/ui-bg_flat_0_eeeeee_40x100.png
+-rw-r--r--   0        0        0      208 2023-07-24 10:27:37.632622 anitya-1.9.0/anitya/static/css/images/ui-bg_flat_55_ffffff_40x100.png
+-rw-r--r--   0        0        0      208 2023-07-24 10:27:37.632622 anitya-1.9.0/anitya/static/css/images/ui-bg_flat_75_ffffff_40x100.png
+-rw-r--r--   0        0        0      207 2023-07-24 10:27:37.632622 anitya-1.9.0/anitya/static/css/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0        0        0      277 2023-07-24 10:27:37.632622 anitya-1.9.0/anitya/static/css/images/ui-bg_highlight-soft_100_f6f6f6_1x100.png
+-rw-r--r--   0        0        0      338 2023-07-24 10:27:37.632622 anitya-1.9.0/anitya/static/css/images/ui-bg_highlight-soft_25_0073ea_1x100.png
+-rw-r--r--   0        0        0      280 2023-07-24 10:27:37.632622 anitya-1.9.0/anitya/static/css/images/ui-bg_highlight-soft_50_dddddd_1x100.png
+-rw-r--r--   0        0        0     4549 2023-07-24 10:27:37.632622 anitya-1.9.0/anitya/static/css/images/ui-icons_0073ea_256x240.png
+-rw-r--r--   0        0        0     6992 2023-07-24 10:27:37.632622 anitya-1.9.0/anitya/static/css/images/ui-icons_454545_256x240.png
+-rw-r--r--   0        0        0     6988 2023-07-24 10:27:37.632622 anitya-1.9.0/anitya/static/css/images/ui-icons_666666_256x240.png
+-rw-r--r--   0        0        0     4549 2023-07-24 10:27:37.632622 anitya-1.9.0/anitya/static/css/images/ui-icons_ff0084_256x240.png
+-rw-r--r--   0        0        0     6299 2023-07-24 10:27:37.632622 anitya-1.9.0/anitya/static/css/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0      125 2023-07-24 10:27:37.632622 anitya-1.9.0/anitya/static/css/navbar.css
+-rw-r--r--   0        0        0     2519 2023-07-24 10:27:37.632622 anitya-1.9.0/anitya/static/css/text.css
+-rw-r--r--   0        0        0     4683 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/static/google_logo.png
+-rw-r--r--   0        0        0     5430 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/static/ico/favicon.ico
+-rw-r--r--   0        0        0     4077 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/static/img/spinner.gif
+-rw-r--r--   0        0        0     3584 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/static/package-lock.json
+-rw-r--r--   0        0        0      765 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/static/package.json
+-rw-r--r--   0        0        0     2970 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/static/yahoo_logo.png
+-rw-r--r--   0        0        0        0 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/__init__.py
+-rw-r--r--   0        0        0     3236 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/distro_add_edit.html
+-rw-r--r--   0        0        0      596 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/distro_delete.html
+-rw-r--r--   0        0        0     2293 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/distros.html
+-rw-r--r--   0        0        0     4148 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/flags.html
+-rw-r--r--   0        0        0      438 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/functions.html
+-rw-r--r--   0        0        0     1626 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/index.html
+-rw-r--r--   0        0        0     1019 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/login.html
+-rw-r--r--   0        0        0     2388 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/logs.html
+-rw-r--r--   0        0        0     1762 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/mapping.html
+-rw-r--r--   0        0        0     9973 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/master.html
+-rw-r--r--   0        0        0    14996 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/project.html
+-rw-r--r--   0        0        0     3734 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/project_archive.html
+-rw-r--r--   0        0        0     3053 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/project_delete.html
+-rw-r--r--   0        0        0     1134 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/project_flag.html
+-rw-r--r--   0        0        0    17556 2024-01-15 14:30:42.757709 anitya-1.9.0/anitya/templates/project_new.html
+-rw-r--r--   0        0        0      999 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/project_versions_delete.html
+-rw-r--r--   0        0        0     3751 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/projects.html
+-rw-r--r--   0        0        0     1354 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/regex_delete.html
+-rw-r--r--   0        0        0     3543 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/search.html
+-rw-r--r--   0        0        0     2101 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/settings.html
+-rw-r--r--   0        0        0     4848 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/updates.html
+-rw-r--r--   0        0        0     4393 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/users.html
+-rw-r--r--   0        0        0     1250 2023-07-24 10:27:37.633622 anitya-1.9.0/anitya/templates/version_delete.html
+-rw-r--r--   0        0        0    24858 2024-01-30 14:15:57.692727 anitya-1.9.0/anitya/ui.py
+-rw-r--r--   0        0        0      845 2024-01-15 14:30:42.760709 anitya-1.9.0/anitya/wsgi.py
+-rw-r--r--   0        0        0     1872 2024-01-15 14:30:42.761710 anitya-1.9.0/createdb.py
+-rw-r--r--   0        0        0     3610 2024-01-15 14:30:42.761710 anitya-1.9.0/files/anitya.toml.sample
+-rw-r--r--   0        0        0      364 2023-07-24 10:27:37.647622 anitya-1.9.0/files/config.toml.sample
+-rw-r--r--   0        0        0     4232 2024-01-30 14:26:43.228052 anitya-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3511 1970-01-01 00:00:00.000000 anitya-1.9.0/setup.py
+-rw-r--r--   0        0        0     3564 1970-01-01 00:00:00.000000 anitya-1.9.0/PKG-INFO
```

### Comparing `anitya-1.8.1/LICENSE` & `anitya-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/README.rst` & `anitya-1.9.0/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -8,22 +8,16 @@
 .. image:: https://readthedocs.org/projects/anitya/badge/?version=latest
   :alt: Documentation Status
   :target: https://anitya.readthedocs.io/en/latest/?badge=latest
   
 .. image:: https://img.shields.io/badge/renovate-enabled-brightgreen.svg
   :target: https://renovatebot.com/
 
-.. image:: https://img.shields.io/lgtm/alerts/g/fedora-infra/anitya.svg?logo=lgtm&logoWidth=18
-  :target: https://lgtm.com/projects/g/fedora-infra/anitya/alerts/
-
-.. image:: https://img.shields.io/lgtm/grade/javascript/g/fedora-infra/anitya.svg?logo=lgtm&logoWidth=18
-  :target: https://lgtm.com/projects/g/fedora-infra/anitya/context:javascript
-  
-.. image:: https://img.shields.io/lgtm/grade/python/g/fedora-infra/anitya.svg?logo=lgtm&logoWidth=18
-  :target: https://lgtm.com/projects/g/fedora-infra/anitya/context:python
+.. image::  https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
+  :target:  https://pre-commit.com/
   
 
 ======
 Anitya
 ======
 
 Anitya is a release monitoring project. It provides a user-friendly interface
```

### Comparing `anitya-1.8.1/alembic.ini` & `anitya-1.9.0/alembic.ini`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/admin.py` & `anitya-1.9.0/anitya/admin.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/api.py` & `anitya-1.9.0/anitya/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,19 +189,15 @@
     """
 
     project_objs = models.Project.all(Session)
 
     projects = []
     for project in project_objs:
         for package in project.packages:
-            tmp = "* {name} {regex} {version_url}".format(
-                name=package.package_name,
-                regex=project.regex,
-                version_url=project.version_url,
-            )
+            tmp = f"* {package.package_name} {project.regex} {project.version_url}"
             projects.append(tmp)
 
     return flask.Response("\n".join(projects), content_type="text/plain;charset=UTF-8")
 
 
 @api_blueprint.route("/api/projects/names/")
 @api_blueprint.route("/api/projects/names")
@@ -491,15 +487,15 @@
     package_name = package_name.rstrip("/")
 
     package = models.Packages.by_package_name_distro(Session, package_name, distro)
 
     if not package:
         output = {
             "output": "notok",
-            "error": 'No package "%s" found in distro "%s"' % (package_name, distro),
+            "error": f'No package "{package_name}" found in distro "{distro}"',
         }
         httpcode = 404
 
     else:
         project = models.Project.get(Session, project_id=package.project.id)
 
         output = project.__json__(detailed=True)
@@ -566,16 +562,15 @@
     """
 
     project = models.Project.by_name_and_ecosystem(Session, project_name, ecosystem)
 
     if not project:
         output = {
             "output": "notok",
-            "error": 'No project "%s" found in ecosystem "%s"'
-            % (project_name, ecosystem),
+            "error": f'No project "{project_name}" found in ecosystem "{ecosystem}"',
         }
         httpcode = 404
 
     else:
         output = project.__json__(detailed=True)
         httpcode = 200
```

### Comparing `anitya-1.8.1/anitya/api_v2.py` & `anitya-1.9.0/anitya/api_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,28 +246,27 @@
                 func.lower(models.Project.name) == func.lower(args["project_name"]),
                 func.lower(models.Project.ecosystem_name)
                 == func.lower(args["project_ecosystem"]),
             ).one()
         except NoResultFound:
             return (
                 {
-                    "error": 'Project "{}" in ecosystem "{}" not found'.format(
-                        args["project_name"], args["project_ecosystem"]
-                    )
+                    "error": f'Project "{args["project_name"]}" in ecosystem '
+                    f'"{args["project_ecosystem"]}" not found'
                 },
                 400,
             )
 
         try:
             distro = models.Distro.query.filter(
                 func.lower(models.Distro.name) == func.lower(args["distribution"])
             ).one()
         except NoResultFound:
             return (
-                {"error": 'Distribution "{}" not found'.format(args["distribution"])},
+                {"error": f"Distribution \"{args['distribution']}\" not found"},
                 400,
             )
 
         try:
             package = models.Packages(
                 distro_name=distro.name,
                 project=project,
```

### Comparing `anitya-1.8.1/anitya/app.py` & `anitya-1.9.0/anitya/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         )
 
     return app
 
 
 def global_user():
     """Set the flask.g variables using the session information if the user is logged in."""
-    flask.g.user = current_user._get_current_object()
+    flask.g.user = current_user._get_current_object()  # pylint: disable=W0212
 
 
 def shutdown_session(exception=None):
     """Remove the DB session at the end of each request."""
     Session.remove()
 
 
@@ -165,15 +165,15 @@
         other_user = models.User.query.filter_by(email=error.params["email"]).one()
         try:
             social_auth_user = other_user.social_auth.filter_by(
                 user_id=other_user.id
             ).one()
             msg = (
                 "Error: There's already an account associated with your email, "
-                "authenticate with {}.".format(social_auth_user.provider)
+                f"authenticate with {social_auth_user.provider}."
             )
             return msg, 400
         # This error happens only if there is account without provider info
         except NoResultFound:
             Session.delete(other_user)
             Session.commit()
             msg = (
@@ -195,16 +195,16 @@
 
     Returns:
         tuple: A tuple of (message, HTTP error code).
     """
     # Because social auth openId backend provides route and raises the exceptions,
     # this is the simplest way to turn error into nicely formatted error message.
     msg = (
-        "Error: There was an error during authentication '{}', "
-        "please check the provided url.".format(error)
+        f"Error: There was an error during authentication '{error}', "
+        "please check the provided url."
     )
     return msg, 400
 
 
 def when_user_log_in(sender, user):
     """
     This catches the signal when user is logged in.
```

### Comparing `anitya-1.8.1/anitya/authentication.py` & `anitya-1.9.0/anitya/authentication.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/check_service.py` & `anitya-1.9.0/anitya/check_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 """
 This is a service that is checking for new releases in projects added to Anitya.
 """
 
 import logging
-from concurrent.futures import ThreadPoolExecutor, TimeoutError, as_completed
+from concurrent.futures import ThreadPoolExecutor, as_completed
 from datetime import datetime
 from threading import Lock
 from time import sleep
 from typing import List
 
 import arrow
 import sqlalchemy as sa
@@ -89,30 +89,30 @@
             project_id: Id of project to check
         """
         session = db.Session()
         project = db.Project.query.filter(db.Project.id == project_id).one()
         if project.backend in self.blacklist_dict:
             self.blacklist_project(project, self.blacklist_dict[project.backend])
             _log.info(
-                "{}: Backend is blacklisted. Rescheduling to {}".format(
-                    project.name, self.blacklist_dict[project.backend]
-                )
+                "%s: Backend is blacklisted. Rescheduling to %s",
+                project.name,
+                self.blacklist_dict[project.backend],
             )
             project.next_check = self.blacklist_dict[project.backend]
             session.add(project)
             session.commit()
             return
         try:
-            _log.debug(f"Checking project {project.name}")
+            _log.debug("Checking project %s", project.name)
             utilities.check_project_release(project, session)
         except RateLimitException as err:
             self.blacklist_project(project, err.reset_time)
             return
         except AnityaException as err:
-            _log.info(f"{project.name} : {str(err)}")
+            _log.info("%s : %s", project.name, str(err))
             with self.error_counter_lock:
                 self.error_counter += 1
             if self.is_delete_candidate(project):
                 session.delete(project)
                 utilities.publish_message(
                     project=project.__json__(),
                     topic="project.remove",
@@ -140,18 +140,15 @@
         Returns:
             True if project is candidate for deletion, False otherwise.
         """
         if project.error_counter < config.get("CHECK_ERROR_THRESHOLD"):
             return False
         packages = db.Packages.query.filter(db.Packages.project_id == project.id).all()
         if packages:
-            if not project.versions:
-                return True
-            else:
-                return False
+            return bool(not project.versions)
 
         return True
 
     def blacklist_project(self, project: db.Project, reset_time: arrow.Arrow):
         """
         Add specified project to `self.ratelimit_queue`, add backend to
         `self.blacklist_dict` and increment `self.ratelimit_counter`.
@@ -159,17 +156,16 @@
         Args:
             project: Project to blacklist
             reset_time: Time when the ratelimit will be reset
         """
         with self.blacklist_dict_lock:
             if project.backend not in self.blacklist_dict:
                 _log.debug(
-                    "Rate limit threshold reached. Adding {} to blacklist.".format(
-                        project.backend
-                    )
+                    "Rate limit threshold reached. Adding %s to blacklist",
+                    project.backend,
                 )
                 self.blacklist_dict[project.backend] = reset_time.to("utc").datetime
         with self.ratelimit_queue_lock:
             if project.backend not in self.ratelimit_queue:
                 self.ratelimit_queue[project.backend] = []
 
             self.ratelimit_queue[project.backend].append(project.id)
@@ -195,17 +191,15 @@
         projects_left = len(queue)
         projects_iter = iter(queue)
 
         if not queue:
             return
 
         # 2. Execution
-        _log.info(
-            "Starting check on {} for total of {} projects".format(time, total_count)
-        )
+        _log.info("Starting check on %s for total of %s projects", time, total_count)
 
         futures = {}
         pool_size = config.get("CRON_POOL")
         timeout = config.get("CHECK_TIMEOUT")
         with ThreadPoolExecutor(pool_size) as pool:
             # Wait till every project in queue is checked
             while projects_left:
@@ -234,20 +228,19 @@
                     projects_left -= 1
                     _log.info("Thread was killed because the execution took too long.")
                     with self.error_counter_lock:
                         self.error_counter += 1
 
         # 3. Finalize
         _log.info(
-            "Check done. Checked ({}): error ({}), success ({}), limit ({})".format(
-                total_count,
-                self.error_counter,
-                self.success_counter,
-                self.ratelimit_counter,
-            )
+            "Check done. Checked (%s): error (%s), success (%s), limit (%s)",
+            total_count,
+            self.error_counter,
+            self.success_counter,
+            self.ratelimit_counter,
         )
 
         run = db.Run(
             created_on=time,
             total_count=total_count,
             error_count=self.error_counter,
             ratelimit_count=self.ratelimit_counter,
@@ -302,15 +295,15 @@
             .filter(db.Project.next_check < time, db.Project.archived.is_(False))
             .all()
         )
 
         # Create list of projects that should be checked but belong to blacklisted backend
         blacklisted_projects = []
         for project in projects:
-            if project.backend in self.blacklist_dict.keys():
+            if project.backend in self.blacklist_dict:
                 blacklisted_projects.append(project)
 
         queue += [
             project.id for project in projects if project not in blacklisted_projects
         ]
 
         # Use ordered set to have the order of the elements, but still have uniqueness
```

### Comparing `anitya-1.8.1/anitya/compat.py` & `anitya-1.9.0/anitya/compat.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,10 +19,12 @@
 Handles compatibility imports for Anitya.
 """
 from __future__ import absolute_import, unicode_literals
 
 # flask_wtf.Form was renamed to flask_wtf.FlaskForm
 # flask_wtf.Form will be removed in flask_wtf-1.0.
 try:
-    from flask_wtf import FlaskForm
+    from flask_wtf import FlaskForm  # pylint: disable=W0611
 except ImportError:
-    from flask_wtf import Form as FlaskForm  # NOQA
+    from flask_wtf import (  # pylint: disable=W0611 # pragma: no cover # noqa: F401
+        Form as FlaskForm,
+    )
```

### Comparing `anitya-1.8.1/anitya/config.py` & `anitya-1.9.0/anitya/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,21 +75,19 @@
     SOCIAL_AUTH_STORAGE="social_flask_sqlalchemy.models.FlaskStorage",
     SOCIAL_AUTH_USER_MODEL="anitya.db.models.User",
     # Force the application to require HTTPS on authentication redirects.
     SOCIAL_AUTH_REDIRECT_IS_HTTPS=True,
     SOCIAL_AUTH_LOGIN_URL="/login/",
     SOCIAL_AUTH_LOGIN_REDIRECT_URL="/",
     SOCIAL_AUTH_LOGIN_ERROR_URL="/login-error/",
-    LIBRARIESIO_PLATFORM_WHITELIST=[],
     DEFAULT_REGEX=r"(?i)%(name)s(?:[-_]?(?:minsrc|src|source))?[-_]([^-/_\s]+?(?:[-_]"
     r"(?:rc|devel|dev|alpha|beta)\d+)?)(?:[-_](?:minsrc|src|source|asc|release))?"
     r"\.(?:tar|t[bglx]z|tbz2|zip)",
     # Token for GitHub API
     GITHUB_ACCESS_TOKEN=None,
-    SSE_FEED="http://firehose.libraries.io/events",
     CRON_POOL=10,  # Number of workers for check service
     CHECK_TIMEOUT=600,  # Timeout for check service
     # When this number of failed checks is reached,
     # project will be automatically removed, if no version was retrieved yet
     CHECK_ERROR_THRESHOLD=100,
     DISTRO_MAPPING_LINKS={},
 )
@@ -112,25 +110,35 @@
 
     if "ANITYA_WEB_CONFIG" in os.environ:
         config_path = os.environ["ANITYA_WEB_CONFIG"]
     else:
         config_path = "/etc/anitya/anitya.toml"
 
     if os.path.exists(config_path):
-        _log.info("Loading Anitya configuration from {}".format(config_path))
-        with open(config_path) as fd:
+        _log.info(
+            "Loading Anitya configuration from {}".format(  # pylint: disable=C0209,W1202
+                config_path
+            )
+        )
+        with open(config_path, encoding="utf-8") as fd:
             try:
                 file_config = toml.loads(fd.read())
                 for key in file_config:
                     config[key.upper()] = file_config[key]
             except toml.TomlDecodeError as e:
-                _log.error("Failed to parse {}: {}".format(config_path, str(e)))
+                _log.error(
+                    "Failed to parse {}: {}".format(  # pylint: disable=C0209,W1202
+                        config_path, str(e)
+                    )
+                )
     else:
         _log.info(
-            "The Anitya configuration file, {}, does not exist.".format(config_path)
+            "The Anitya configuration file, {}, does not exist.".format(  # pylint: disable=C0209,W1202 # noqa: E501
+                config_path
+            )
         )
 
     if not isinstance(config["PERMANENT_SESSION_LIFETIME"], timedelta):
         config["PERMANENT_SESSION_LIFETIME"] = timedelta(
             seconds=config["PERMANENT_SESSION_LIFETIME"]
         )
```

### Comparing `anitya-1.8.1/anitya/db/__init__.py` & `anitya-1.9.0/anitya/db/__init__.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/events.py` & `anitya-1.9.0/anitya/db/events.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/meta.py` & `anitya-1.9.0/anitya/db/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,17 +133,17 @@
             raise ValueError("page must be 1 or greater.")
         if items_per_page < 1:
             raise ValueError("items_per_page must be 1 or greater.")
 
         if not isinstance(order_by, tuple):
             order_by = (order_by,)
 
-        q = self.order_by(*order_by)
-        total_items = q.count()
-        items = q.limit(items_per_page).offset(items_per_page * (page - 1)).all()
+        result = self.order_by(*order_by)
+        total_items = result.count()
+        items = result.limit(items_per_page).offset(items_per_page * (page - 1)).all()
         return Page(
             items=items,
             page=page,
             total_items=total_items,
             items_per_page=items_per_page,
         )
```

### Comparing `anitya-1.8.1/anitya/db/migrations/env.py` & `anitya-1.9.0/anitya/db/migrations/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""env"""
+
 from __future__ import with_statement
 
 import sys
 from logging.config import fileConfig
 from os.path import dirname
 
 from alembic import context
```

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/16aa7da2764c_add_projectversion_commit_url.py` & `anitya-1.9.0/anitya/db/migrations/versions/16aa7da2764c_add_projectversion_commit_url.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 
 # revision identifiers, used by Alembic.
 revision = "16aa7da2764c"
 down_revision = "314651690dc7"
 
 
 def upgrade():
+    """Upgrade"""
     op.add_column(
         "projects_versions",
         sa.Column("commit_url", sa.String(length=200), nullable=True),
     )
 
 
 def downgrade():
+    """Downgrade"""
     with op.batch_alter_table("projects_versions") as batch_op:
         batch_op.drop_column("commit_url")
```

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/1ab95561edae_convert_date_to_rpm.py` & `anitya-1.9.0/anitya/db/migrations/versions/1ab95561edae_convert_date_to_rpm.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/1bf8aead6179_add_check_times.py` & `anitya-1.9.0/anitya/db/migrations/versions/1bf8aead6179_add_check_times.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/1f839c54e428_add_archive_flag.py` & `anitya-1.9.0/anitya/db/migrations/versions/1f839c54e428_add_archive_flag.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/24b6734e8565_creation_date_on_version.py` & `anitya-1.9.0/anitya/db/migrations/versions/24b6734e8565_creation_date_on_version.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/27342bce1d0f_populate_project_version_scheme.py` & `anitya-1.9.0/anitya/db/migrations/versions/27342bce1d0f_populate_project_version_scheme.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/2925648d8cc3_add_a_version_prefix_field.py` & `anitya-1.9.0/anitya/db/migrations/versions/2925648d8cc3_add_a_version_prefix_field.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/2d1aa7ff82a5_remove_code_google_backend.py` & `anitya-1.9.0/anitya/db/migrations/versions/2d1aa7ff82a5_remove_code_google_backend.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/314651690dc7_add_error_counter_to_project.py` & `anitya-1.9.0/anitya/db/migrations/versions/314651690dc7_add_error_counter_to_project.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/34b9bb5fa388_make_ecosystem_non_nullable.py` & `anitya-1.9.0/anitya/db/migrations/versions/34b9bb5fa388_make_ecosystem_non_nullable.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/3fae8239eeec_add_an_api_token_table.py` & `anitya-1.9.0/anitya/db/migrations/versions/3fae8239eeec_add_an_api_token_table.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from sqlalchemy.types import CHAR, TypeDecorator
 
 # revision identifiers, used by Alembic.
 revision = "3fae8239eeec"
 down_revision = "feeaa70ead67"
 
 
-class GUID(TypeDecorator):
+class GUID(TypeDecorator):  # pylint: disable=W0223
     """
     Platform-independent GUID type.
 
     If PostgreSQL is being used, use its native UUID type, otherwise use a CHAR(32) type.
     """
 
     impl = CHAR
@@ -75,18 +75,18 @@
         """
         if value is None:
             return value
         elif dialect.name == "postgresql":
             return str(value)
         else:
             if not isinstance(value, uuid.UUID):
-                return "%.32x" % uuid.UUID(value).int
+                return f"{uuid.UUID(value).int:032x}"
             else:
                 # hexstring
-                return "%.32x" % value.int
+                return f"{value.int:032x}"
 
     def process_result_value(self, value, dialect):
         """
         Casts the UUID value to the native Python type.
 
         Args:
             value (object): The database value.
```

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/540bdcf7edbc_convert_github_url_to_owner_project.py` & `anitya-1.9.0/anitya/db/migrations/versions/540bdcf7edbc_convert_github_url_to_owner_project.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/571bd07533a9_add_insecure_column_to_projects_table.py` & `anitya-1.9.0/anitya/db/migrations/versions/571bd07533a9_add_insecure_column_to_projects_table.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/5b8b587d7dbe_add_version_filter_column.py` & `anitya-1.9.0/anitya/db/migrations/versions/5b8b587d7dbe_add_version_filter_column.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/5e209766aead_add_release_check_to_project.py` & `anitya-1.9.0/anitya/db/migrations/versions/5e209766aead_add_release_check_to_project.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/6ac0e42df937_drop_logs_table.py` & `anitya-1.9.0/anitya/db/migrations/versions/6ac0e42df937_drop_logs_table.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/708f6f26b4b6_add_version_pattern.py` & `anitya-1.9.0/anitya/db/migrations/versions/708f6f26b4b6_add_version_pattern.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/7a8c4aa92678_add_missing_github_owner_project_pairs.py` & `anitya-1.9.0/anitya/db/migrations/versions/7a8c4aa92678_add_missing_github_owner_project_pairs.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/8040ef9a9dda_add_a_version_scheme_column_to_projects.py` & `anitya-1.9.0/anitya/db/migrations/versions/8040ef9a9dda_add_a_version_scheme_column_to_projects.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/8be6e153962c_remove_cursor.py` & `anitya-1.9.0/anitya/db/migrations/versions/8be6e153962c_remove_cursor.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/921c612ba0da_model_upstream_ecosystems.py` & `anitya-1.9.0/anitya/db/migrations/versions/921c612ba0da_model_upstream_ecosystems.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 # revision identifiers, used by Alembic.
 revision = "921c612ba0da"
 down_revision = "2925648d8cc3"
 
 
 def upgrade():
+    """Upgrade"""
     op.add_column(
         "projects", sa.Column("ecosystem_name", sa.String(length=200), nullable=True)
     )
     op.create_unique_constraint(
         "UNIQ_PROJECT_NAME_PER_ECOSYSTEM", "projects", ["name", "ecosystem_name"]
     )
     op.create_foreign_key(
@@ -29,10 +30,11 @@
         ["name"],
         onupdate="cascade",
         ondelete="set null",
     )
 
 
 def downgrade():
+    """Downgrade"""
     op.drop_constraint("FK_ECOSYSTEM_FOR_PROJECT", "projects", type_="foreignkey")
     op.drop_constraint("UNIQ_PROJECT_NAME_PER_ECOSYSTEM", "projects", type_="unique")
     op.drop_column("projects", "ecosystem_name")
```

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/92a2e9eba0a7_add_project_latest_known_cursor.py` & `anitya-1.9.0/anitya/db/migrations/versions/92a2e9eba0a7_add_project_latest_known_cursor.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 
 # revision identifiers, used by Alembic.
 revision = "92a2e9eba0a7"
 down_revision = "5e209766aead"
 
 
 def upgrade():
+    """Upgrade"""
     op.add_column(
         "projects",
         sa.Column("latest_known_cursor", sa.String(length=200), nullable=True),
     )
 
 
 def downgrade():
+    """Downgrade"""
     with op.batch_alter_table("projects") as batch_op:
         batch_op.drop_column("latest_known_cursor")
```

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/9c29da0af3af_populate_ecosystem_data.py` & `anitya-1.9.0/anitya/db/migrations/versions/9c29da0af3af_populate_ecosystem_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 # revision identifiers, used by Alembic.
 revision = "9c29da0af3af"
 down_revision = "921c612ba0da"
 
 
 def upgrade():
+    """Upgrade"""
     # We use a subquery instead of an UPDATE FROM with a table join
     # due to the fact that SQLite doesn't allow joins in update statements
     op.execute(
         """
         UPDATE projects
         SET ecosystem_name=(
             SELECT ecosystems.name
@@ -28,10 +29,11 @@
         )
         WHERE ecosystem_name is null
     """
     )
 
 
 def downgrade():
+    """Downgrade"""
     # Do nothing on downgrade - column removal will be handled by previous
     # revision
     pass
```

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/a52d2fe99d4f_users.py` & `anitya-1.9.0/anitya/db/migrations/versions/a52d2fe99d4f_users.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """
 Add a table for Users.
 
 Revision ID: a52d2fe99d4f
 Revises: 8040ef9a9dda
 Create Date: 2017-07-06 18:08:56.027650
 """
+
 import uuid
 
 import sqlalchemy as sa
 from alembic import op
 from sqlalchemy.dialects.postgresql import UUID
 from sqlalchemy.types import CHAR, TypeDecorator
 
 # revision identifiers, used by Alembic.
 revision = "a52d2fe99d4f"
 down_revision = "8040ef9a9dda"
 
 
-class GUID(TypeDecorator):
+class GUID(TypeDecorator):  # pylint: disable=W0223
     """
     Platform-independent GUID type.
 
     If PostgreSQL is being used, use its native UUID type, otherwise use a CHAR(32) type.
     """
 
     impl = CHAR
@@ -58,18 +59,18 @@
         """
         if value is None:
             return value
         elif dialect.name == "postgresql":
             return str(value)
         else:
             if not isinstance(value, uuid.UUID):
-                return "%.32x" % uuid.UUID(value).int
+                return f"{uuid.UUID(value).int:032x}"
             else:
                 # hexstring
-                return "%.32x" % value.int
+                return f"{value.int:032x}"
 
     def process_result_value(self, value, dialect):
         """
         Casts the UUID value to the native Python type.
 
         Args:
             value (object): The database value.
```

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/b9201d816075_remove_the_backends_and_ecosystems_.py` & `anitya-1.9.0/anitya/db/migrations/versions/b9201d816075_remove_the_backends_and_ecosystems_.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         sa.Column("name", sa.VARCHAR(length=200), autoincrement=False, nullable=False),
         sa.PrimaryKeyConstraint("name", name="backends_pkey"),
         postgresql_ignore_search_path=False,
     )
     # We have to populate the backends table before we can add the ecosystems
     # table with its foreign key constraint.
     for backend in plugins.BACKEND_PLUGINS.get_plugins():
-        op.execute("INSERT INTO backends (name) VALUES ('{}');".format(backend.name))
+        op.execute(f"INSERT INTO backends (name) VALUES ('{backend.name}');")
 
     op.create_table(
         "ecosystems",
         sa.Column("name", sa.VARCHAR(length=200), autoincrement=False, nullable=False),
         sa.Column(
             "default_backend_name",
             sa.VARCHAR(length=200),
@@ -61,19 +61,17 @@
         sa.PrimaryKeyConstraint("name", name="ecosystems_pkey"),
         sa.UniqueConstraint(
             "default_backend_name", name="ecosystems_default_backend_name_key"
         ),
     )
     for ecosystem in plugins.ECOSYSTEM_PLUGINS.get_plugins():
         op.execute(
-            """
+            f"""
             INSERT INTO ecosystems (name, default_backend_name)
-            VALUES ('{name}', '{default}');""".format(
-                name=ecosystem.name, default=ecosystem.default_backend
-            )
+            VALUES ('{ecosystem.name}', '{ecosystem.default_backend}');"""
         )
 
     op.create_foreign_key(
         "FK_ECOSYSTEM_FOR_PROJECT",
         "projects",
         "ecosystems",
         ["ecosystem_name"],
```

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/d6170cfc2814_add_pre_release_flag.py` & `anitya-1.9.0/anitya/db/migrations/versions/d6170cfc2814_add_pre_release_flag.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/e34988f3e2f4_add_statistics_to_run.py` & `anitya-1.9.0/anitya/db/migrations/versions/e34988f3e2f4_add_statistics_to_run.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/db/migrations/versions/feeaa70ead67_social_authentication_table.py` & `anitya-1.9.0/anitya/db/migrations/versions/feeaa70ead67_social_authentication_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from sqlalchemy.types import CHAR, TypeDecorator
 
 # revision identifiers, used by Alembic.
 revision = "feeaa70ead67"
 down_revision = "a52d2fe99d4f"
 
 
-class GUID(TypeDecorator):
+class GUID(TypeDecorator):  # pylint: disable=W0223
     """
     Platform-independent GUID type.
 
     If PostgreSQL is being used, use its native UUID type, otherwise use a CHAR(32) type.
     """
 
     impl = CHAR
@@ -76,18 +76,18 @@
         """
         if value is None:
             return value
         elif dialect.name == "postgresql":
             return str(value)
         else:
             if not isinstance(value, uuid.UUID):
-                return "%.32x" % uuid.UUID(value).int
+                return f"{uuid.UUID(value).int:032x}"
             else:
                 # hexstring
-                return "%.32x" % value.int
+                return f"{value.int:032x}"
 
     def process_result_value(self, value, dialect):
         """
         Casts the UUID value to the native Python type.
 
         Args:
             value (object): The database value.
```

### Comparing `anitya-1.8.1/anitya/db/models.py` & `anitya-1.9.0/anitya/db/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,37 +58,41 @@
         offset = (page - 1) * limit
         query = query.offset(offset).limit(limit)
 
     return query
 
 
 class Distro(Base):
+    """Class Distro"""
+
     __tablename__ = "distros"
 
     name = sa.Column(sa.String(200), primary_key=True)
 
     def __init__(self, name):
         """Constructor."""
         self.name = name
 
     def __json__(self):
         return dict(name=self.name)
 
     @classmethod
     def by_name(cls, session, name):
+        """Get Distro name"""
         query = session.query(cls).filter(
             sa.func.lower(cls.name) == sa.func.lower(name)
         )
 
         return query.first()
 
     get = by_name
 
     @classmethod
     def all(cls, session, page=None, count=False):
+        """Distro all"""
         query = session.query(cls).order_by(cls.name)
 
         query = _paginate_query(query, page)
 
         if count:
             return query.count()
         else:
@@ -113,23 +117,26 @@
         if count:
             return query.count()
         else:
             return query.all()
 
     @classmethod
     def get_or_create(cls, session, name):
+        """Get distro or create it"""
         distro = cls.by_name(session, name)
         if not distro:
             distro = cls(name=name)
             session.add(distro)
             session.flush()
         return distro
 
 
 class Packages(Base):
+    """Class Packages"""
+
     __tablename__ = "packages"
 
     id = sa.Column(sa.Integer, primary_key=True)
     distro_name = sa.Column(
         sa.String(200),
         sa.ForeignKey("distros.name", ondelete="cascade", onupdate="cascade"),
     )
@@ -146,39 +153,38 @@
     )
 
     distro = sa.orm.relationship(
         "Distro", backref=sa.orm.backref("package", cascade="all, delete-orphan")
     )
 
     def __repr__(self):
-        return "<Packages(%s, %s: %s)>" % (
-            self.project_id,
-            self.distro_name,
-            self.package_name,
-        )
+        return f"<Packages({self.project_id}, {self.distro_name}: {self.package_name})>"
 
     def __json__(self):
         return dict(package_name=self.package_name, distro=self.distro_name)
 
     @classmethod
     def by_id(cls, session, pkg_id):
+        """Packages by id"""
         return session.query(cls).filter_by(id=pkg_id).first()
 
     @classmethod
     def get(cls, session, project_id, distro_name, package_name):
+        """Get Packages"""
         query = (
             session.query(cls)
             .filter(cls.project_id == project_id)
             .filter(sa.func.lower(cls.distro_name) == sa.func.lower(distro_name))
             .filter(cls.package_name == package_name)
         )
         return query.first()
 
     @classmethod
     def by_package_name_distro(cls, session, package_name, distro_name):
+        """Get package by package name distro"""
         query = (
             session.query(cls)
             .filter(cls.package_name == package_name)
             .filter(sa.func.lower(cls.distro_name) == sa.func.lower(distro_name))
         )
         return query.first()
 
@@ -275,16 +281,17 @@
         sa.UniqueConstraint(
             "name", "ecosystem_name", name="UNIQ_PROJECT_NAME_PER_ECOSYSTEM"
         ),
     )
 
     @validates("backend")
     def validate_backend(self, key, value):
+        """Validate backend"""
         if value not in BACKEND_PLUGINS.get_plugin_names():
-            raise ValueError('Backend "{}" is not supported.'.format(value))
+            raise ValueError(f"Backend '{value}' is not supported.")
         return value
 
     @property
     def versions(self):
         """Return list of all versions stored, sorted from newest to oldest.
 
         Returns:
@@ -415,14 +422,15 @@
             for v_obj in self.versions_obj
         ]
         sorted_versions = list(reversed(sorted(versions)))
         return sorted_versions
 
     @property
     def latest_version_object(self):
+        """Latest version object"""
         sorted_versions = self.get_sorted_version_objects()
         if sorted_versions:
             return sorted_versions[0]
         return None
 
     def get_version_class(self):
         """
@@ -453,92 +461,100 @@
             version_scheme = backend.default_version_scheme
         if not version_scheme:
             version_scheme = DEFAULT_VERSION_SCHEME
 
         return VERSION_PLUGINS.get_plugin(version_scheme)
 
     def __repr__(self):
-        return "<Project(%s, %s)>" % (self.name, self.homepage)
+        return f"<Project({self.name}, {self.homepage})>"
 
     def __json__(self, detailed=False):
         output = dict(
             id=self.id,
             name=self.name,
             homepage=self.homepage,
             regex=self.regex,
             backend=self.backend,
             version_url=self.version_url,
             version=self.latest_version,
             versions=self.versions,
             stable_versions=[str(v) for v in self.stable_versions],
-            created_on=time.mktime(self.created_on.timetuple())
-            if self.created_on
-            else None,
-            updated_on=time.mktime(self.updated_on.timetuple())
-            if self.updated_on
-            else None,
+            created_on=(
+                time.mktime(self.created_on.timetuple()) if self.created_on else None
+            ),
+            updated_on=(
+                time.mktime(self.updated_on.timetuple()) if self.updated_on else None
+            ),
             ecosystem=self.ecosystem_name,
         )
         if detailed:
             output["packages"] = [pkg.__json__() for pkg in self.packages]
 
         return output
 
     @classmethod
     def get_or_create(cls, session, name, homepage, backend="custom"):
+        """Get or Create"""
         project = cls.by_name_and_homepage(session, name, homepage)
         if not project:
             project = cls(name=name, homepage=homepage, backend=backend)
             session.add(project)
             session.flush()
         return project
 
     @classmethod
     def by_name(cls, session, name):
+        """By name"""
         return session.query(cls).filter_by(name=name).all()
 
     @classmethod
     def by_id(cls, session, project_id):
+        """By id"""
         return session.query(cls).filter_by(id=project_id).first()
 
     get = by_id
 
     @classmethod
     def by_homepage(cls, session, homepage):
+        """By homepage"""
         return session.query(cls).filter_by(homepage=homepage).all()
 
     @classmethod
     def by_name_and_homepage(cls, session, name, homepage):
+        """By  name and homepage"""
         query = (
             session.query(cls).filter(cls.name == name).filter(cls.homepage == homepage)
         )
         return query.first()
 
     @classmethod
     def by_name_and_ecosystem(cls, session, name, ecosystem):
+        """By name and ecosystem"""
         try:
             query = session.query(cls)
             query = query.filter(cls.name == name, cls.ecosystem_name == ecosystem)
             return query.one()
         except NoResultFound:
             return None
 
     @classmethod
     def all(cls, session, page=None, count=False):
+        """all"""
         query = session.query(Project).order_by(sa.func.lower(Project.name))
 
         query = _paginate_query(query, page)
 
         if count:
             return query.count()
         else:
             return query.all()
 
     @classmethod
     def by_distro(cls, session, distro, page=None, count=False):
+        """By distro"""
         query = (
             session.query(Project)
             .filter(Project.id == Packages.project_id)
             .filter(sa.func.lower(Packages.distro_name) == sa.func.lower(distro))
             .order_by(sa.func.lower(Project.name))
         )
 
@@ -700,14 +716,16 @@
             pattern=self.project.version_pattern,
             commit_url=self.commit_url,
         )
         return version.prerelease()
 
 
 class ProjectFlag(Base):
+    """Class ProjectFlag"""
+
     __tablename__ = "projects_flags"
 
     id = sa.Column(sa.Integer, primary_key=True)
 
     project_id = sa.Column(
         sa.Integer, sa.ForeignKey("projects.id", ondelete="cascade", onupdate="cascade")
     )
@@ -721,15 +739,15 @@
     )
 
     project = sa.orm.relationship(
         "Project", backref=sa.orm.backref("flags", cascade="all, delete-orphan")
     )
 
     def __repr__(self):
-        return "<ProjectFlag(%s, %s, %s)>" % (self.project.name, self.user, self.state)
+        return f"<ProjectFlag({self.project.name}, {self.user}, {self.state})>"
 
     def __json__(self, detailed=False):
         output = dict(
             id=self.id,
             project=self.project.name,
             user=self.user,
             state=self.state,
@@ -739,14 +757,15 @@
         if detailed:
             output["reason"] = self.reason
 
         return output
 
     @classmethod
     def all(cls, session, page=None, count=False):
+        """all"""
         query = session.query(ProjectFlag).order_by(ProjectFlag.created_on)
 
         return query.all()
 
     @classmethod
     def search(
         cls,
@@ -799,19 +818,22 @@
         if limit:
             query = query.limit(limit)
 
         return query.all()
 
     @classmethod
     def get(cls, session, flag_id):
+        """get"""
         query = session.query(cls).filter(cls.id == flag_id)
         return query.first()
 
 
 class Run(Base):
+    """Class Run"""
+
     __tablename__ = "runs"
 
     total_count = sa.Column(sa.Integer)
     error_count = sa.Column(sa.Integer)
     ratelimit_count = sa.Column(sa.Integer)
     success_count = sa.Column(sa.Integer)
     created_on = sa.Column(
@@ -867,18 +889,18 @@
         """
         if value is None:
             return value
         elif dialect.name == "postgresql":
             return str(value)
         else:
             if not isinstance(value, uuid.UUID):
-                return "%.32x" % uuid.UUID(value).int
+                return f"{uuid.UUID(value).int:032x}"
             else:
                 # hexstring
-                return "%.32x" % value.int
+                return f"{value.int:032x}"
 
     def process_result_value(self, value, dialect):
         """
         Casts the UUID value to the native Python type.
 
         Args:
             value (object): The database value.
@@ -888,14 +910,37 @@
             uuid.UUID: The value as a Python :class:`uuid.UUID`.
         """
         if value is None:
             return value
         else:
             return uuid.UUID(value)
 
+    def process_literal_param(self, value, dialect):
+        """Receive a literal parameter value to be rendered inline within
+        a statement.
+
+        .. note::
+
+            This method is called during the **SQL compilation** phase of a
+            statement, when rendering a SQL string. Unlike other SQL
+            compilation methods, it is passed a specific Python value to be
+            rendered as a string. However it should not be confused with the
+            :meth:`_types.TypeDecorator.process_bind_param` method, which is
+            the more typical method that processes the actual value passed to a
+            particular parameter at statement execution time.
+
+        Custom subclasses of :class:`_types.TypeDecorator` should override
+        this method to provide custom behaviors for incoming data values
+        that are in the special case of being rendered as literals.
+
+        The returned string will be rendered into the output string.
+
+        """
+        raise NotImplementedError()
+
 
 class User(Base):
     """
     A table for Anitya users.
 
     This table is intended to work with a table of third-party authentication
     providers. Anitya does not support local users.
```

### Comparing `anitya-1.8.1/anitya/forms.py` & `anitya-1.9.0/anitya/forms.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,16 @@
             for users to describe the token's purpose.
     """
 
     description = StringField("Token description", [validators.optional()])
 
 
 class ProjectForm(FlaskForm):
+    """ProjectForm"""
+
     name = StringField("Project name", [validators.DataRequired()])
     homepage = StringField("Homepage", [validators.DataRequired(), validators.URL()])
     backend = SelectField("Backend", [validators.DataRequired()], choices=[])
     version_url = StringField("Version URL", [validators.optional()])
     version_prefix = StringField("Version prefix", [validators.optional()])
     pre_release_filter = StringField("Pre-release filter", [validators.optional()])
     version_filter = StringField("Version filter", [validators.optional()])
@@ -44,15 +46,15 @@
     )
 
     def __init__(self, *args, **kwargs):
         """Calls the default constructor with the normal argument but
         uses the list of backends provided to fill the choices of the
         drop-down list.
         """
-        super(ProjectForm, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         if "backends" in kwargs:
             self.backend.choices = [
                 (backend, backend) for backend in sorted(kwargs["backends"])
             ]
         if "version_schemes" in kwargs:
             self.version_scheme.choices = [
                 (version_scheme, version_scheme)
@@ -63,31 +65,39 @@
                 (distro, distro)
                 for distro in sorted(kwargs["distros"], key=lambda s: s.lower())
             ]
             self.distro.choices.insert(0, ("", ""))
 
 
 class FlagProjectForm(FlaskForm):
+    """FlagProjectForm"""
+
     reason = TextAreaField("Reason for flagging", [validators.DataRequired()])
 
 
 class MappingForm(FlaskForm):
+    """MappingForm"""
+
     distro = SelectField("Distribution", [validators.DataRequired()], choices=[])
     package_name = StringField("Package name", [validators.DataRequired()])
 
     def __init__(self, *args, **kwargs):
         """Calls the default constructor and fill in additional information."""
-        super(MappingForm, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
         if "distros" in kwargs:
             self.distro.choices = [
                 (distro, distro)
                 for distro in sorted(kwargs["distros"], key=lambda s: s.lower())
             ]
 
 
 class ConfirmationForm(FlaskForm):
+    """ConfirmationForm"""
+
     pass
 
 
 class DistroForm(FlaskForm):
+    """DistroForm"""
+
     name = StringField("Distribution name", [validators.DataRequired()])
```

### Comparing `anitya-1.8.1/anitya/lib/backends/__init__.py` & `anitya-1.9.0/anitya/lib/backends/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import fnmatch
 import logging
 import re
 import socket
 
 # sre_constants contains re exceptions
-import sre_constants
+import sre_constants  # pylint: disable=W4901
 import urllib.request as urllib
 from datetime import timedelta
 from typing import List
 from urllib.error import URLError
 
 import arrow
 import pkg_resources
@@ -39,16 +39,16 @@
 from anitya.lib.exceptions import AnityaPluginException
 from anitya.lib.versions import GLOBAL_DEFAULT, RpmVersion
 
 REGEX = anitya_config["DEFAULT_REGEX"]
 
 # Default headers for requests
 REQUEST_HEADERS = {
-    "User-Agent": "Anitya %s at release-monitoring.org"
-    % pkg_resources.get_distribution("anitya").version,
+    "User-Agent": f"Anitya {pkg_resources.get_distribution('anitya').version} "
+    "at release-monitoring.org",
     "From": anitya_config.get("ADMIN_EMAIL"),
     "If-modified-since": arrow.Arrow(1970, 1, 1).format("ddd, DD MMM YYYY HH:mm:ss")
     + " GMT",
 }
 
 _log = logging.getLogger(__name__)
 
@@ -84,26 +84,26 @@
     examples: List[str]
     default_regex: str
     more_info: str
     default_version_scheme = GLOBAL_DEFAULT
     check_interval = timedelta(hours=1)
 
     @classmethod
-    def expand_subdirs(self, url, last_change=None, glob_char="*"):
+    def expand_subdirs(cls, url, last_change=None, glob_char="*"):
         """Expand dirs containing ``glob_char`` in the given URL with the latest
         Example URL: ``https://www.example.com/foo/*/``
 
         The globbing char can be bundled with other characters enclosed within
         the same slashes in the URL like ``/rel*/``.
 
         Code originally from Till Maas as part of
         `cnucnu <https://fedorapeople.org/cgit/till/public_git/cnucnu.git/>`_
 
         """
-        glob_pattern = "/([^/]*%s[^/]*)/" % re.escape(glob_char)
+        glob_pattern = f"/([^/]*{re.escape(glob_char)}[^/]*)/"
         glob_match = re.search(glob_pattern, url)
         if not glob_match:
             return url
         glob_str = glob_match.group(1)
 
         # url until first slash before glob_match
         url_prefix = url[0 : glob_match.start() + 1]
@@ -111,15 +111,15 @@
         # everything after the slash after glob_match
         url_suffix = url[glob_match.end() :]
 
         html_regex = re.compile(r'\bhref\s*=\s*["\']([^"\'/]+)/["\']', re.I)
         text_regex = re.compile(r"^d.+\s(\S+)\s*$", re.I | re.M)
 
         if url_prefix != "":
-            resp = self.call_url(url_prefix, last_change=last_change)
+            resp = cls.call_url(url_prefix, last_change=last_change)
             # When FTP server is called, Response object is not created
             # and we get binary string instead
             try:
                 dir_listing = resp.text
             except AttributeError:
                 dir_listing = resp
             if not dir_listing:
@@ -131,16 +131,16 @@
                 if subdir not in (".", "..") and fnmatch.fnmatch(subdir, glob_str):
                     subdirs.append(subdir)
             if not subdirs:
                 return url
             sorted_subdirs = sorted([RpmVersion(s) for s in subdirs])
             latest = sorted_subdirs[-1].version
 
-            url = "%s%s/%s" % (url_prefix, latest, url_suffix)
-            return self.expand_subdirs(url, glob_char)
+            url = f"{url_prefix}{latest}/{url_suffix}"
+            return cls.expand_subdirs(url, glob_char)
         return url
 
     @classmethod
     def get_version(cls, project):  # pragma: no cover
         """Method called to retrieve the latest version of the projects
         provided, project that relies on the backend of this plugin.
 
@@ -170,15 +170,15 @@
 
         Returns:
             str: url used for version checking
         """
         pass
 
     @classmethod
-    def get_versions(self, project):  # pragma: no cover
+    def get_versions(cls, project):  # pragma: no cover
         """Method called to retrieve all the versions (that can be found)
         of the projects provided, project that relies on the backend of
         this plugin.
 
         Attributes:
             project (:obj:`anitya.db.models.Project`): Project object whose backend
                 corresponds to the current plugin.
@@ -193,15 +193,15 @@
                 :obj:`anitya.lib.exceptions.AnityaPluginException` exception
                 when the versions cannot be retrieved correctly
 
         """
         pass
 
     @classmethod
-    def check_feed(self):
+    def check_feed(cls):
         """Method called to retrieve the latest uploads to a given backend,
         via, for example, RSS or an API.
 
         Not all backends may support this.  It can be used to look for updates
         much more quickly than scanning all known projects.
 
         Returns:
@@ -215,15 +215,15 @@
             NotImplementedError: If backend does not
                 support batch updates.
 
         """
         raise NotImplementedError()
 
     @classmethod
-    def get_ordered_versions(self, project):
+    def get_ordered_versions(cls, project):
         """Method called to retrieve all the versions (that can be found)
         of the projects provided, ordered from the oldest to the newest.
 
         Attributes:
             project (:obj:`anitya.db.models.Project`): Project object whose backend
                 corresponds to the current plugin.
 
@@ -232,20 +232,20 @@
 
         Raises:
             AnityaPluginException: A
                 :obj:`anitya.lib.exceptions.AnityaPluginException` exception
                 when the versions cannot be retrieved correctly
 
         """
-        vlist = self.get_versions(project)
+        vlist = cls.get_versions(project)
         sorted_versions = project.create_version_objects(vlist)
         return [v.version for v in sorted_versions]
 
     @classmethod
-    def _filter_versions(self, version, filter_list):
+    def _filter_versions(cls, version, filter_list):
         """
         Method used to call as argument of Python filter function.
 
         Attributes:
             version (:obj:`list`): List of versions. For example ["1.0.0, 1.0.0-alpha"]
             filter_list (:obj:`list`): List of strings to use as filter.
 
@@ -254,45 +254,43 @@
         """
         for filter_str in filter_list:
             if filter_str and filter_str in version:
                 return True
         return False
 
     @classmethod
-    def filter_versions(self, versions, filter_string):
+    def filter_versions(cls, versions, filter_string):
         """Method called to filter versions list by filter_string.
         Filter string is first parsed by delimiter and then applied on list of versions.
         For example: list of versions ["1.0.0", "1.0.0-alpha", "1.0.0-beta"]
         when filtered by "alpha;beta" will return ["1.0.0"].
 
         Attributes:
             versions (:obj:`list`): List of versions. For example ["1.0.0, 1.0.0-alpha"]
             filter_string (str): String to use for filtering.
                 It contains list of strings delimited by ";".
 
         Returns:
             :obj:`list`: A list of filtered versions.
         """
-        _log.debug(
-            "Filtering versions '{}' by filter '{}'".format(versions, filter_string)
-        )
+        _log.debug("Filtering versions '%s' by filter '%s'", versions, filter_string)
         filtered_versions = versions
         if filter_string:
             filter_list = filter_string.split(";")
             filtered_versions = [
                 version
                 for version in versions
-                if not self._filter_versions(version, filter_list)
+                if not cls._filter_versions(version, filter_list)
             ]
 
-        _log.debug("Filtered versions '{}'".format(filtered_versions))
+        _log.debug("Filtered versions '%s'", filtered_versions)
         return filtered_versions
 
     @classmethod
-    def call_url(self, url, last_change=None, insecure=False):
+    def call_url(cls, url, last_change=None, insecure=False):
         """Dedicated method to query a URL.
 
         It is important to use this method as it allows to query them with
         a defined user-agent header thus informing the projects we are
         querying what our intentions are.
 
         To prevent downloading the whole content of the page each time the url is called.
@@ -313,34 +311,34 @@
         """
         headers = REQUEST_HEADERS.copy()
         if last_change:
             headers["If-modified-since"] = (
                 last_change.format("ddd, DD MMM YYYY HH:mm:ss") + " GMT"
             )
         if "*" in url:
-            url = self.expand_subdirs(url, last_change)
+            url = cls.expand_subdirs(url, last_change)  # pragma: no cover
 
         if url.startswith("ftp://") or url.startswith("ftps://"):
             socket.setdefaulttimeout(30)
 
             req = urllib.Request(url)
             req.add_header("User-Agent", headers["User-Agent"])
             req.add_header("From", headers["From"])
             try:
                 # Ignore this bandit issue, the url is checked above
-                resp = urllib.urlopen(req)  # nosec
+                resp = urllib.urlopen(req)  # nosec # pylint: disable=R1732
                 content = resp.read().decode()
             except URLError as e:
                 raise AnityaPluginException(
-                    'Could not call "%s" with error: %s' % (url, e.reason)
-                )
-            except UnicodeDecodeError:
+                    f'Could not call "{url}" with error: {e.reason}'
+                ) from e
+            except UnicodeDecodeError as e:
                 raise AnityaPluginException(
-                    "FTP response cannot be decoded with UTF-8: %s" % url
-                )
+                    f"FTP response cannot be decoded with UTF-8: {url}"
+                ) from e
 
             return content
 
         else:
             # Works around https://github.com/kennethreitz/requests/issues/2863
             # Currently, requests does not start new TCP connections based on
             # TLS settings. This means that if a connection is ever started to
@@ -367,19 +365,18 @@
 
     """
 
     last_change = project.get_time_last_created_version()
     try:
         req = BaseBackend.call_url(url, last_change=last_change, insecure=insecure)
     except Exception as err:
-        _log.debug("%s ERROR: %s" % (project.name, str(err)))
+        _log.debug("%s ERROR: %s", project.name, str(err))
         raise AnityaPluginException(
-            'Could not call : "%s" of "%s", with error: %s'
-            % (url, project.name, str(err))
-        )
+            f'Could not call : "{url}" of "{project.name}", with error: {str(err)}'
+        ) from err
 
     if not isinstance(req, six.string_types):
         # Not modified
         if req.status_code == 304:
             return []
         req = req.text
 
@@ -390,33 +387,34 @@
     """For the provided text, return all the version retrieved via the
     specified regular expression.
 
     """
 
     try:
         upstream_versions = list(set(re.findall(regex, text)))
-    except sre_constants.error:  # pragma: no cover
-        raise AnityaPluginException("%s: invalid regular expression" % project.name)
+    except sre_constants.error as err:  # pragma: no cover
+        raise AnityaPluginException(
+            f"{project.name}: invalid regular expression"
+        ) from err
 
     for index, version in enumerate(upstream_versions):
         # If the version retrieved is a tuple, re-constitute it
-        if type(version) == tuple:
+        if isinstance(version, tuple):
             version = ".".join([v for v in version if not v == ""])
 
         upstream_versions[index] = version
 
         if " " in version:
             raise AnityaPluginException(
-                "%s: invalid upstream version:>%s< - %s - %s "
-                % (project.name, version, url, regex)
+                f"{project.name}: invalid upstream version:>{version}< - {url} "
+                f"- {regex} "
             )
     if len(upstream_versions) == 0:
         raise AnityaPluginException(
-            "%(name)s: no upstream version found. - %(url)s -  "
-            "%(regex)s" % {"name": project.name, "url": url, "regex": regex}
+            f"{project.name}: no upstream version found. - {url} -  {regex}"
         )
     # Filter retrieved versions
     filtered_versions = BaseBackend.filter_versions(
         upstream_versions, project.version_filter
     )
 
     return filtered_versions
```

### Comparing `anitya-1.8.1/anitya/lib/backends/bitbucket.py` & `anitya-1.9.0/anitya/lib/backends/bitbucket.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,26 +35,25 @@
         Attributes:
             project (:obj:`anitya.db.models.Project`): Project object whose backend
                 corresponds to the current plugin.
 
         Returns:
             str: url used for version checking
         """
-        url_template = "https://bitbucket.org/%(version_url)s/" "downloads?tab=tags"
         url = ""
         if project.version_url:
             url = project.version_url.replace("https://bitbucket.org/", "")
         elif project.homepage.startswith("https://bitbucket.org/"):
             url = project.homepage.replace("https://bitbucket.org/", "")
 
         if url.endswith("/"):
             url = url[:-1]
 
         if url:
-            url = url_template % {"version_url": url}
+            url = f"https://bitbucket.org/{url}/downloads?tab=tags"
 
         return url
 
     @classmethod
     def get_versions(cls, project):
         """Method called to retrieve all the versions (that can be found)
         of the projects provided, project that relies on the backend of
@@ -68,11 +67,29 @@
             :class:`anitya.lib.exceptions.AnityaPluginException` exception
             when the versions cannot be retrieved correctly
 
         """
         url = cls.get_version_url(project)
         if not url:
             raise AnityaPluginException(
-                "Project %s was incorrectly set up." % project.name
+                f"Project {project.name} was incorrectly set up."
             )
 
         return get_versions_by_regex(url, REGEX, project)
+
+    @classmethod
+    def check_feed(cls):  # pragma: no cover
+        """Method called to retrieve the latest uploads to a given backend,
+        via, for example, RSS or an API.
+
+        Not Supported
+
+        Returns:
+            :obj:`list`: A list of 4-tuples, containing the project name, homepage, the
+            backend, and the version.
+
+        Raises:
+             NotImplementedError: If backend does not
+                support batch updates.
+
+        """
+        raise NotImplementedError()
```

### Comparing `anitya-1.8.1/anitya/lib/backends/cgit.py` & `anitya-1.9.0/anitya/lib/backends/cgit.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 # implied warranties of MERCHANTABILITY or FITNESS FOR A PARTICULAR
 # PURPOSE.  See the GNU General Public License for more details.  You
 # should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301, USA.
 #
 
+"""
+A backend for cgit
+"""
 from anitya.lib.backends import BaseBackend, get_versions_by_regex
 
 REGEX = r"<a href='.*'>(?:%(name)s-)?(.*)\.(?:tar|tar\.[bglx]z|tbz2|zip)</a>"
 
 
 class CgitBackend(BaseBackend):
     """The custom class for projects hosted on Cgit
@@ -61,7 +64,25 @@
 
         Returns:
             str: a list of all the possible releases found
         """
         url = cls.get_version_url(project)
         regex = REGEX % {"name": project.name.lower()}
         return get_versions_by_regex(url, regex, project, url.startswith("http://"))
+
+    @classmethod
+    def check_feed(cls):  # pragma: no cover
+        """Method called to retrieve the latest uploads to a given backend,
+        via, for example, RSS or an API.
+
+        Not Supported
+
+        Returns:
+            :obj:`list`: A list of 4-tuples, containing the project name, homepage, the
+            backend, and the version.
+
+        Raises:
+             NotImplementedError: If backend does not
+                support batch updates.
+
+        """
+        raise NotImplementedError()
```

### Comparing `anitya-1.8.1/anitya/lib/backends/cpan.py` & `anitya-1.9.0/anitya/lib/backends/cpan.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         Attributes:
             project (:obj:`anitya.db.models.Project`): Project object whose backend
                 corresponds to the current plugin.
 
         Returns:
             str: url used for version checking
         """
-        url = "https://metacpan.org/release/%(name)s/" % {"name": project.name}
+        url = f"https://metacpan.org/release/{project.name}/"
 
         return url
 
     @classmethod
     def get_versions(cls, project):
         """Method called to retrieve all the versions (that can be found)
         of the projects provided, project that relies on the backend of
@@ -76,23 +76,23 @@
         by querying an RSS feed.
         """
 
         url = "https://metacpan.org/feed/recent"
 
         try:
             response = cls.call_url(url)
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("Could not contact %s" % url)
+        except Exception as exc:  # pragma: no cover
+            raise AnityaPluginException(f"Could not contact {url}") from exc
 
         try:
             root = ET.fromstring(response.text)
-        except ET.ParseError:
-            raise AnityaPluginException("No XML returned by %s" % url)
+        except ET.ParseError as exc:
+            raise AnityaPluginException(f"No XML returned by {url}") from exc
 
         for item in root.iter(tag="{http://purl.org/rss/1.0/}item"):
             title = item.find("{http://purl.org/rss/1.0/}title")
             try:
                 name, version = title.text.rsplit("-", 1)
             except ValueError:
                 _log.info("Unable to parse CPAN package %s into a name and version")
-            homepage = "https://metacpan.org/release/%s/" % name
+            homepage = f"https://metacpan.org/release/{name}/"
             yield name, homepage, cls.name, version
```

### Comparing `anitya-1.8.1/anitya/lib/backends/cran.py` & `anitya-1.9.0/anitya/lib/backends/cran.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,39 +66,38 @@
             str: The latest version found upstream.
 
         Raises:
             AnityaPluginException: If the URL was unreachable or the response was in an unexpected
                 format.
 
         """
-        url = "https://crandb.r-pkg.org/{name}".format(name=project.name)
+        url = f"https://crandb.r-pkg.org/{project.name}"
 
         last_change = project.get_time_last_created_version()
         try:
             response = cls.call_url(url, last_change=last_change)
         except requests.RequestException as e:  # pragma: no cover
-            raise AnityaPluginException("Could not contact {}: {}".format(url, str(e)))
+            raise AnityaPluginException(f"Could not contact {url}: {str(e)}") from e
 
         if response.status_code != 200:
             # Not modified
             if response.status_code == 304:
                 return None
             raise AnityaPluginException(
-                "Failed to download from {}: {} {}".format(
-                    url, response.status_code, response.reason
-                )
+                f"Failed to download from {url}: {response.status_code} "
+                f"{response.reason}"
             )
 
         try:
             data = response.json()
-        except json.JSONDecodeError:  # pragma: no cover
-            raise AnityaPluginException("No JSON returned by {}".format(url))
+        except json.JSONDecodeError as e:  # pragma: no cover
+            raise AnityaPluginException(f"No JSON returned by {url}") from e
 
         if "error" in data or "Version" not in data:  # pragma: no cover
-            raise AnityaPluginException("No versions found at {}".format(url))
+            raise AnityaPluginException(f"No versions found at {url}")
 
         return data["Version"]
 
     @classmethod
     def get_version_url(cls, project):
         """Method called to retrieve the url used to check for new version
         of the project provided, project that relies on the backend of this plugin.
@@ -106,15 +105,15 @@
         Attributes:
             project (:obj:`anitya.db.models.Project`): Project object whose backend
                 corresponds to the current plugin.
 
         Returns:
             str: url used for version checking
         """
-        url = "https://crandb.r-pkg.org/{name}/all".format(name=project.name)
+        url = f"https://crandb.r-pkg.org/{project.name}/all"
 
         return url
 
     @classmethod
     def get_versions(cls, project):
         """
         Retrieve all the versions (that can be found) of the provided project from this backend.
@@ -132,33 +131,32 @@
         """
         url = cls.get_version_url(project)
         last_change = project.get_time_last_created_version()
 
         try:
             response = cls.call_url(url, last_change=last_change)
         except requests.RequestException as e:  # pragma: no cover
-            raise AnityaPluginException("Could not contact {}: {}".format(url, str(e)))
+            raise AnityaPluginException(f"Could not contact {url}: {str(e)}") from e
 
         if response.status_code != 200:
             # Not modified
             if response.status_code == 304:
                 return []
             raise AnityaPluginException(
-                "Failed to download from {}: {} {}".format(
-                    url, response.status_code, response.reason
-                )
+                f"Failed to download from {url}: {response.status_code} "
+                f"{response.reason}"
             )
 
         try:
             data = response.json()
-        except json.JSONDecodeError:  # pragma: no cover
-            raise AnityaPluginException("No JSON returned by {}".format(url))
+        except json.JSONDecodeError as e:  # pragma: no cover
+            raise AnityaPluginException(f"No JSON returned by {url}") from e
 
         if "error" in data or "versions" not in data:  # pragma: no cover
-            raise AnityaPluginException("No versions found at {}".format(url))
+            raise AnityaPluginException(f"No versions found at {url}")
 
         filtered_versions = cls.filter_versions(
             list(data["versions"].keys()), project.version_filter
         )
         return filtered_versions
 
     @classmethod
@@ -180,27 +178,26 @@
         """
 
         url = "https://crandb.r-pkg.org/-/pkgreleases?descending=true&limit=50"
 
         try:
             response = cls.call_url(url)
         except requests.RequestException as e:  # pragma: no cover
-            raise AnityaPluginException("Could not contact {}: {}".format(url, str(e)))
+            raise AnityaPluginException(f"Could not contact {url}: {str(e)}") from e
 
         if response.status_code != 200:  # pragma: no cover
             raise AnityaPluginException(
-                "Failed to download from {}: {} {}".format(
-                    url, response.status_code, response.reason
-                )
+                f"Failed to download from {url}: {response.status_code} "
+                f"{response.reason}"
             )
 
         try:
             data = response.json()
-        except json.JSONDecodeError:  # pragma: no cover
-            raise AnityaPluginException("No JSON returned by {}".format(url))
+        except json.JSONDecodeError as err:  # pragma: no cover
+            raise AnityaPluginException(f"No JSON returned by {url}") from err
 
         for item in data:
             name = item["name"]
             package = item["package"]
             homepage = package.get(
                 "URL", "https://cran.r-project.org/web/packages/" + name
             )
```

### Comparing `anitya-1.8.1/anitya/lib/backends/crates.py` & `anitya-1.9.0/anitya/lib/backends/crates.py`

 * *Files 7% similar despite different names*

```diff
@@ -151,19 +151,17 @@
             req = cls.call_url(url, last_change=last_change)
             req.raise_for_status()
             # Not modified
             if req.status_code == 304:
                 return []
             data = req.json()
         except requests.RequestException as e:
-            raise AnityaPluginException(
-                "Could not contact {url}: " "{reason!r}".format(url=url, reason=e)
-            )
+            raise AnityaPluginException(f"Could not contact {url}: {e!r}") from e
         except ValueError as e:
-            raise AnityaPluginException("Failed to decode JSON: {!r}".format(e))
+            raise AnityaPluginException(f"Failed to decode JSON: {e!r}") from e
 
         return data["versions"]
 
     @classmethod
     def get_version(cls, project):
         """
         Get the latest version of the project provided.
@@ -189,15 +187,15 @@
         Attributes:
             project (:obj:`anitya.db.models.Project`): Project object whose backend
                 corresponds to the current plugin.
 
         Returns:
             str: url used for version checking
         """
-        url = "https://crates.io/api/v1/crates/{}/versions".format(project.name)
+        url = f"https://crates.io/api/v1/crates/{project.name}/versions"
 
         return url
 
     @classmethod
     def get_versions(cls, project):
         """
         Get all versions of the project provided.
@@ -233,7 +231,25 @@
 
         Raises:
             AnityaPluginException: If the URL was unreachable or the response
                 was in an unexpected format.
         """
         # crates API returns already ordered versions
         return cls.get_versions(project)
+
+    @classmethod
+    def check_feed(cls):  # pragma: no cover
+        """Method called to retrieve the latest uploads to a given backend,
+        via, for example, RSS or an API.
+
+        Not Supported
+
+        Returns:
+            :obj:`list`: A list of 4-tuples, containing the project name, homepage, the
+            backend, and the version.
+
+        Raises:
+             NotImplementedError: If backend does not
+                support batch updates.
+
+        """
+        raise NotImplementedError()
```

### Comparing `anitya-1.8.1/anitya/lib/backends/custom.py` & `anitya-1.9.0/anitya/lib/backends/sourceforge.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,49 +6,45 @@
  Authors:
    Pierre-Yves Chibon <pingou@pingoured.fr>
 
 """
 
 from anitya.lib.backends import REGEX, BaseBackend, get_versions_by_regex
 
-REGEX_ALIASES = {"DEFAULT": REGEX}
 
-
-class CustomBackend(BaseBackend):
-    """The custom class for project having a special hosting.
+class SourceforgeBackend(BaseBackend):
+    """The custom class for projects hosted on sourceforge.net.
 
     This backend allows to specify a version_url and a regex that will
     be used to retrieve the version information.
     """
 
-    name = "custom"
+    name = "Sourceforge"
     examples = [
-        "https://subsurface-divelog.org/downloads/",
-        "https://www.geany.org/Download/Releases",
+        "https://sourceforge.net/projects/filezilla/",
+        "https://sourceforge.net/projects/file-folder-ren/",
     ]
-    more_info = (
-        "More information in the <a href='"
-        "/static/docs/user-guide.html#regular-expressions'> "
-        "user-guide.html#regular-expressions</a>"
-    )
-    default_regex = REGEX % {"name": "{project name}"}
 
     @classmethod
     def get_version_url(cls, project):
         """Method called to retrieve the url used to check for new version
         of the project provided, project that relies on the backend of this plugin.
 
         Attributes:
             project (:obj:`anitya.db.models.Project`): Project object whose backend
                 corresponds to the current plugin.
 
         Returns:
             str: url used for version checking
         """
-        url = project.version_url
+        url_template = "https://sourceforge.net/projects/%(name)s/rss?limit=200"
+
+        url = url_template % {
+            "name": (project.version_url or project.name).replace("+", r"\+")
+        }
 
         return url
 
     @classmethod
     def get_versions(cls, project):
         """Method called to retrieve all the versions (that can be found)
         of the projects provided, project that relies on the backend of
@@ -60,16 +56,32 @@
         :return type: list
         :raise AnityaPluginException: a
             :class:`anitya.lib.exceptions.AnityaPluginException` exception
             when the versions cannot be retrieved correctly
 
         """
         url = cls.get_version_url(project)
+        regex = REGEX % {"name": project.name.replace("+", r"\+")}
+
+        return get_versions_by_regex(url, regex, project)
+
+    @classmethod
+    def check_feed(cls):  # pragma: no cover
+        """Method called to retrieve the latest uploads to a given backend,
+        via, for example, RSS or an API.
+
+        Not all backends may support this.  It can be used to look for updates
+        much more quickly than scanning all known projects.
 
-        regex = REGEX_ALIASES["DEFAULT"]
-        if project.regex:
-            regex = REGEX_ALIASES.get(project.regex, project.regex)
+        Returns:
+            :obj:`list`: A list of 4-tuples, containing the project name, homepage, the
+            backend, and the version.
 
-        if "%(name)" in regex:
-            regex = regex % {"name": project.name.replace("+", r"\+")}
+        Raises:
+            AnityaPluginException: A
+                :obj:`anitya.lib.exceptions.AnityaPluginException` exception
+                when the versions cannot be retrieved correctly
+            NotImplementedError: If backend does not
+                support batch updates.
 
-        return get_versions_by_regex(url, regex, project, insecure=project.insecure)
+        """
+        raise NotImplementedError()
```

### Comparing `anitya-1.8.1/anitya/lib/backends/debian.py` & `anitya-1.9.0/anitya/lib/backends/debian.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,24 +40,21 @@
         Attributes:
             project (:obj:`anitya.db.models.Project`): Project object whose backend
                 corresponds to the current plugin.
 
         Returns:
             str: url used for version checking
         """
-        url_template = "http://ftp.debian.org/debian/pool/main/" "%(short)s/%(name)s/"
 
         if project.name.startswith("lib"):
             short = project.name[:4]
         else:
             short = project.name[0]
 
-        url = url_template % {"short": short, "name": project.name}
-
-        return url
+        return f"http://ftp.debian.org/debian/pool/main/{short}/{project.name}/"
 
     @classmethod
     def get_versions(cls, project):
         """Method called to retrieve all the versions (that can be found)
         of the projects provided, project that relies on the backend of
         this plugin.
 
@@ -70,7 +67,25 @@
             when the versions cannot be retrieved correctly
 
         """
         url = cls.get_version_url(project)
         regex = DEBIAN_REGEX % {"name": project.name}
 
         return get_versions_by_regex(url, regex, project)
+
+    @classmethod
+    def check_feed(cls):  # pragma: no cover
+        """Method called to retrieve the latest uploads to a given backend,
+        via, for example, RSS or an API.
+
+        Not Supported
+
+        Returns:
+            :obj:`list`: A list of 4-tuples, containing the project name, homepage, the
+            backend, and the version.
+
+        Raises:
+             NotImplementedError: If backend does not
+                support batch updates.
+
+        """
+        raise NotImplementedError()
```

### Comparing `anitya-1.8.1/anitya/lib/backends/drupal6.py` & `anitya-1.9.0/anitya/lib/backends/drupal6.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,17 +46,15 @@
         """
         name = project.name
         if name.lower().strip().startswith("drupal6:"):
             name = name[len("drupal6:") :].strip()
         if "-" in project.name:
             name = project.name.replace("-", "_")
 
-        url_template = "https://updates.drupal.org/release-history/" "%(name)s/6.x"
-
-        url = url_template % {"name": name}
+        url = f"https://updates.drupal.org/release-history/{name}/6.x"
 
         return url
 
     @classmethod
     def get_versions(cls, project):
         """Method called to retrieve all the versions (that can be found)
         of the projects provided, project that relies on the backend of
@@ -80,7 +78,29 @@
 
         try:
             versions = get_versions_by_regex(url, regex, project)
         except AnityaPluginException as err:
             raise err
 
         return versions
+
+    @classmethod
+    def check_feed(cls):  # pragma: no cover
+        """Method called to retrieve the latest uploads to a given backend,
+        via, for example, RSS or an API.
+
+        Not all backends may support this.  It can be used to look for updates
+        much more quickly than scanning all known projects.
+
+        Returns:
+            :obj:`list`: A list of 4-tuples, containing the project name, homepage, the
+            backend, and the version.
+
+        Raises:
+            AnityaPluginException: A
+                :obj:`anitya.lib.exceptions.AnityaPluginException` exception
+                when the versions cannot be retrieved correctly
+            NotImplementedError: If backend does not
+                support batch updates.
+
+        """
+        raise NotImplementedError()
```

### Comparing `anitya-1.8.1/anitya/lib/backends/drupal7.py` & `anitya-1.9.0/anitya/lib/backends/drupal7.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,19 +46,15 @@
         """
         name = project.name
         if name.lower().strip().startswith("drupal7:"):
             name = name[len("drupal7:") :].strip()
         if "-" in project.name:
             name = project.name.replace("-", "_")
 
-        url_template = "https://updates.drupal.org/release-history/" "%(name)s/7.x"
-
-        url = url_template % {"name": name}
-
-        return url
+        return f"https://updates.drupal.org/release-history/{name}/7.x"
 
     @classmethod
     def get_versions(cls, project):
         """Method called to retrieve all the versions (that can be found)
         of the projects provided, project that relies on the backend of
         this plugin.
 
@@ -80,7 +76,25 @@
 
         try:
             versions = get_versions_by_regex(url, regex, project)
         except AnityaPluginException as err:
             raise err
 
         return versions
+
+    @classmethod
+    def check_feed(cls):  # pragma: no cover
+        """Method called to retrieve the latest uploads to a given backend,
+        via, for example, RSS or an API.
+
+        Not Supported
+
+        Returns:
+            :obj:`list`: A list of 4-tuples, containing the project name, homepage, the
+            backend, and the version.
+
+        Raises:
+             NotImplementedError: If backend does not
+                support batch updates.
+
+        """
+        raise NotImplementedError()
```

### Comparing `anitya-1.8.1/anitya/lib/backends/folder.py` & `anitya-1.9.0/anitya/lib/backends/folder.py`

 * *Files 18% similar despite different names*

```diff
@@ -61,17 +61,16 @@
         url = cls.get_version_url(project)
         last_change = project.get_time_last_created_version()
 
         try:
             req = cls.call_url(url, last_change=last_change, insecure=project.insecure)
         except Exception as err:
             raise AnityaPluginException(
-                'Could not call : "%s" of "%s", with error: %s'
-                % (url, project.name, str(err))
-            )
+                f'Could not call : "{url}" of "{project.name}", with error: {str(err)}'
+            ) from err
 
         versions = []
 
         if not isinstance(req, six.string_types):
             # Not modified
             if req.status_code == 304:
                 return versions
@@ -81,7 +80,25 @@
         try:
             regex = REGEX % {"name": project.name.replace("+", r"\+")}
             versions = get_versions_by_regex_for_text(req, url, regex, project)
         except AnityaPluginException:
             versions = get_versions_by_regex_for_text(req, url, DEFAULT_REGEX, project)
 
         return versions
+
+    @classmethod
+    def check_feed(cls):  # pragma: no cover
+        """Method called to retrieve the latest uploads to a given backend,
+        via, for example, RSS or an API.
+
+        Not Supported
+
+        Returns:
+            :obj:`list`: A list of 4-tuples, containing the project name, homepage, the
+            backend, and the version.
+
+        Raises:
+             NotImplementedError: If backend does not
+                support batch updates.
+
+        """
+        raise NotImplementedError()
```

### Comparing `anitya-1.8.1/anitya/lib/backends/freshmeat.py` & `anitya-1.9.0/anitya/lib/backends/freshmeat.py`

 * *Files 21% similar despite different names*

```diff
@@ -58,7 +58,25 @@
             :class:`anitya.lib.exceptions.AnityaPluginException` exception
             when the versions cannot be retrieved correctly
 
         """
         url = cls.get_version_url(project)
 
         return get_versions_by_regex(url, REGEX, project)
+
+    @classmethod
+    def check_feed(cls):
+        """Method called to retrieve the latest uploads to a given backend,
+        via, for example, RSS or an API.
+
+        Not Supported
+
+        Returns:
+            :obj:`list`: A list of 4-tuples, containing the project name, homepage, the
+            backend, and the version.
+
+        Raises:
+             NotImplementedError: If backend does not
+                support batch updates.
+
+        """
+        raise NotImplementedError()
```

### Comparing `anitya-1.8.1/anitya/lib/backends/github.py` & `anitya-1.9.0/anitya/lib/backends/github.py`

 * *Files 12% similar despite different names*

```diff
@@ -81,42 +81,42 @@
         query = prepare_query(owner, repo, project.releases_only)
 
         try:
             headers = REQUEST_HEADERS.copy()
             token = config["GITHUB_ACCESS_TOKEN"]
             if not token:
                 raise AnityaPluginException("github_access_token not configured")
-            headers["Authorization"] = "bearer %s" % token
+            headers["Authorization"] = f"bearer {token}"
             resp = http_session.post(
                 API_URL,
                 json={"query": query},
                 headers=headers,
                 timeout=60,
                 verify=True,
             )
         except Exception as err:
-            _log.debug("%s ERROR: %s" % (project.name, str(err)))
+            _log.debug("%s ERROR: %s", project.name, str(err))
             raise AnityaPluginException(
-                'Could not call : "%s" of "%s", with error: %s'
-                % (API_URL, project.name, str(err))
+                f'Could not call : "{API_URL}" of "{project.name}", '
+                f"with error: {str(err)}"
             ) from err
 
         if resp.ok:
             json = resp.json()
         elif resp.status_code == 403:
             _log.info("Github API ratelimit reached.")
             raise RateLimitException(reset_time)
         else:
             raise AnityaPluginException(
-                '%s: Server responded with status "%s": "%s"'
-                % (project.name, resp.status_code, resp.reason)
+                f"{project.name}: Server responded with status "
+                f'"{resp.status_code}": "{resp.reason}"'
             )
 
         versions = parse_json(json, project)
-        _log.debug(f"Retrieved versions: {versions}")
+        _log.debug("Retrieved versions: %s", versions)
         return versions
 
     @classmethod
     def get_versions(cls, project):
         """Method called to retrieve all the versions (that can be found)
         of the projects provided, project that relies on the backend of
         this plugin.
@@ -139,42 +139,56 @@
         url = cls.get_version_url(project)
         if url:
             url = url.replace("https://github.com/", "")
             url = utilities.remove_suffix(url, "/releases")
             url = utilities.remove_suffix(url, "/tags")
         else:
             raise AnityaPluginException(
-                "Project %s was incorrectly set up." % project.name
+                f"Project {project.name} was incorrectly set up."
             )
 
         try:
             (owner, repo) = url.split("/")
-        except ValueError:
+        except ValueError as err:
             raise AnityaPluginException(
-                """Project {} was incorrectly set up.
-                Can\'t parse owner and repo.""".format(
-                    project.name
-                )
-            )
+                f"""Project {project.name} was incorrectly set up.
+                Can't parse owner and repo."""
+            ) from err
 
         versions = cls._retrieve_versions(owner, repo, project)
 
         if len(versions) == 0:
-            raise AnityaPluginException(
-                "%s: No upstream version found." % (project.name)
-            )
+            raise AnityaPluginException(f"{project.name}: No upstream version found.")
 
         # Filter retrieved versions
         filtered_versions = cls.filter_versions(
             [version["version"] for version in versions], project.version_filter
         )
         return [
             version for version in versions if version["version"] in filtered_versions
         ]
 
+    @classmethod
+    def check_feed(cls):  # pragma: no cover
+        """Method called to retrieve the latest uploads to a given backend,
+        via, for example, RSS or an API.
+
+        Not Supported
+
+        Returns:
+            :obj:`list`: A list of 4-tuples, containing the project name, homepage, the
+            backend, and the version.
+
+        Raises:
+             NotImplementedError: If backend does not
+                support batch updates.
+
+        """
+        raise NotImplementedError()
+
 
 def parse_json(json, project):
     """Function for parsing json response
 
     Args:
         json (dict): Json dictionary to parse.
         project (:obj:`anitya.db.models.Project`): Project object whose backend
@@ -188,49 +202,50 @@
             :obj:`anitya.lib.exceptions.AnityaPluginException` exception
             when the versions cannot be retrieved correctly.
         RateLimitException: A
             :obj:`anitya.lib.exceptions.RateLimitException` exception
             when rate limit threshold is reached.
 
     """
-    global reset_time
+    global reset_time  # pylint: disable=W0603
     # We need to check limit first,
     # because exceeding the limit will also return error
     try:
         limit = json["data"]["rateLimit"]["limit"]
         remaining = json["data"]["rateLimit"]["remaining"]
         reset_time = json["data"]["rateLimit"]["resetAt"]
         _log.debug(
-            "Github API ratelimit remains %s, will reset at %s UTC"
-            % (remaining, reset_time)
+            "Github API ratelimit remains %s, will reset at %s UTC",
+            remaining,
+            reset_time,
         )
 
         if (remaining / limit) <= RATE_LIMIT_THRESHOLD:
             raise RateLimitException(reset_time)
     except KeyError:
         _log.info("Github API ratelimit key is missing. Checking for errors.")
 
     if "errors" in json:
         error_str = ""
         for error in json["errors"]:
-            error_str += '"%s": "%s"\n' % (error["type"], error["message"])
+            error_str += f"\"{error['type']}\": \"{error['message']}\"\n"
         raise AnityaPluginException(
-            "%s: Server responded with following errors\n%s" % (project.name, error_str)
+            f"{project.name}: Server responded with following errors\n{error_str}"
         )
     if project.releases_only:
         json_data = json["data"]["repository"]["releases"]
     else:
         json_data = json["data"]["repository"]["refs"]
 
     total_count = json_data["totalCount"]
 
     if project.releases_only:
-        _log.debug("Received %s releases for %s" % (total_count, project.name))
+        _log.debug("Received %s releases for %s", total_count, project.name)
     else:
-        _log.debug("Received %s tags for %s" % (total_count, project.name))
+        _log.debug("Received %s tags for %s", total_count, project.name)
 
     versions = []
 
     for edge in json_data["edges"]:
         version = {}
         if project.releases_only:
             hook = edge["node"]["tag"]
@@ -239,16 +254,17 @@
 
         if hook:
             version["version"] = hook["name"]
             version["commit_url"] = hook["target"]["commitUrl"]
             versions.append(version)
         else:
             _log.info(
-                "Skipping release %s on %s, because it doesn't have associated tag"
-                % (edge["node"]["name"], project.name)
+                "Skipping release %s on %s, because it doesn't have associated tag",
+                edge["node"]["name"],
+                project.name,
             )
 
     return versions
 
 
 def prepare_query(owner, repo, releases_only):
     """Function for preparing GraphQL query for specified repository
```

### Comparing `anitya-1.8.1/anitya/lib/backends/gitlab.py` & `anitya-1.9.0/anitya/lib/backends/gitlab.py`

 * *Files 18% similar despite different names*

```diff
@@ -89,38 +89,54 @@
             :class:`anitya.lib.exceptions.AnityaPluginException` exception
             when the versions cannot be retrieved correctly
 
         """
         url = cls.get_version_url(project)
         if not url:
             raise AnityaPluginException(
-                "Project %s was incorrectly set up." % project.name
+                f"Project {project.name} was incorrectly set up."
             )
 
         last_change = project.get_time_last_created_version()
         resp = cls.call_url(url, last_change=last_change)
 
         if resp.status_code == 200:
             json = resp.json()
         else:
             # Not modified
             if resp.status_code == 304:
                 return []
             raise AnityaPluginException(
-                '%s: Server responded with status "%s": "%s"'
-                % (project.name, resp.status_code, resp.reason)
+                f"{project.name}: Server responded with status "
+                f'"{resp.status_code}": "{resp.reason}"'
             )
 
-        _log.debug("Received %d tags for %s" % (len(json), project.name))
+        _log.debug("Received %s tags for %s", len(json), project.name)
 
         tags = []
         for tag in json:
             tags.append(tag["name"])
 
         if len(tags) == 0:
-            raise AnityaPluginException(
-                "%s: No upstream version found." % (project.name)
-            )
+            raise AnityaPluginException(f"{project.name}: No upstream version found.")
 
         # Filter retrieved versions
         filtered_versions = cls.filter_versions(tags, project.version_filter)
         return filtered_versions
+
+    @classmethod
+    def check_feed(cls):  # pragma: no cover
+        """Method called to retrieve the latest uploads to a given backend,
+        via, for example, RSS or an API.
+
+        Not Supported
+
+        Returns:
+            :obj:`list`: A list of 4-tuples, containing the project name, homepage, the
+            backend, and the version.
+
+        Raises:
+             NotImplementedError: If backend does not
+                support batch updates.
+
+        """
+        raise NotImplementedError()
```

### Comparing `anitya-1.8.1/anitya/lib/backends/gnome.py` & `anitya-1.9.0/anitya/lib/backends/gnome.py`

 * *Files 21% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         Attributes:
             project (:obj:`anitya.db.models.Project`): Project object whose backend
                 corresponds to the current plugin.
 
         Returns:
             str: url used for version checking
         """
-        url = "https://download.gnome.org/sources/%(name)s/" % {"name": project.name}
+        url = f"https://download.gnome.org/sources/{project.name}/"
 
         return url
 
     @classmethod
     def get_versions(cls, project):
         """Method called to retrieve all the versions (that can be found)
         of the projects provided, project that relies on the backend of
@@ -98,7 +98,25 @@
             # First try to get the version by using the cache.json file
             output = use_gnome_cache_json(project)
         except Exception as err:
             _log.exception(err)
             output = use_gnome_regex(project)
 
         return output
+
+    @classmethod
+    def check_feed(cls):  # pragma: no cover
+        """Method called to retrieve the latest uploads to a given backend,
+        via, for example, RSS or an API.
+
+        Not Supported
+
+        Returns:
+            :obj:`list`: A list of 4-tuples, containing the project name, homepage, the
+            backend, and the version.
+
+        Raises:
+             NotImplementedError: If backend does not
+                support batch updates.
+
+        """
+        raise NotImplementedError()
```

### Comparing `anitya-1.8.1/anitya/lib/backends/gnu.py` & `anitya-1.9.0/anitya/lib/backends/gnu.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         Attributes:
             project (:obj:`anitya.db.models.Project`): Project object whose backend
                 corresponds to the current plugin.
 
         Returns:
             str: url used for version checking
         """
-        url = "https://ftp.gnu.org/gnu/%(name)s/" % {"name": project.name}
+        url = f"https://ftp.gnu.org/gnu/{project.name}/"
 
         return url
 
     @classmethod
     def get_versions(cls, project):
         """Method called to retrieve all the versions (that can be found)
         of the projects provided, project that relies on the backend of
@@ -58,18 +58,18 @@
 
         """
         url = cls.get_version_url(project)
         last_change = project.get_time_last_created_version()
 
         try:
             req = cls.call_url(url, last_change=last_change)
-        except Exception:  # pragma: no cover
+        except Exception as err:  # pragma: no cover
             raise AnityaPluginException(
-                'Could not call : "%s" of "%s"' % (url, project.name)
-            )
+                f'Could not call : "{url}" of "{project.name}"'
+            ) from err
 
         versions = []
         if not isinstance(req, six.string_types):
             # Not modified
             if req.status_code == 304:
                 return versions
 
@@ -78,7 +78,25 @@
             versions = get_versions_by_regex_for_text(req.text, url, regex, project)
         except AnityaPluginException:
             versions = get_versions_by_regex_for_text(
                 req.text, url, DEFAULT_REGEX, project
             )
 
         return versions
+
+    @classmethod
+    def check_feed(cls):  # pragma: no cover
+        """Method called to retrieve the latest uploads to a given backend,
+        via, for example, RSS or an API.
+
+        Not Supported
+
+        Returns:
+            :obj:`list`: A list of 4-tuples, containing the project name, homepage, the
+            backend, and the version.
+
+        Raises:
+             NotImplementedError: If backend does not
+                support batch updates.
+
+        """
+        raise NotImplementedError()
```

### Comparing `anitya-1.8.1/anitya/lib/backends/gogs.py` & `anitya-1.9.0/anitya/lib/backends/gogs.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # useful, but WITHOUT ANY WARRANTY expressed or implied, including the
 # implied warranties of MERCHANTABILITY or FITNESS FOR A PARTICULAR
 # PURPOSE.  See the GNU General Public License for more details.  You
 # should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301, USA.
 #
-
+"""gogs"""
 from anitya.lib.backends import BaseBackend, get_versions_by_regex
 from anitya.lib.exceptions import AnityaPluginException
 
 REGEX = '<i class="tag icon"></i> (.*)</a>'
 
 
 class GogsBackend(BaseBackend):
@@ -75,11 +75,29 @@
 
         Returns:
             str: a list of all the possible releases found
         """
         url = cls.get_version_url(project)
         if not url:
             raise AnityaPluginException(
-                "Project %s was incorrectly set up" % project.name
+                f"Project {project.name} was incorrectly set up"
             )
 
         return get_versions_by_regex(url, REGEX, project, url.startswith("http://"))
+
+    @classmethod
+    def check_feed(cls):  # pragma: no cover
+        """Method called to retrieve the latest uploads to a given backend,
+        via, for example, RSS or an API.
+
+        Not Supported
+
+        Returns:
+            :obj:`list`: A list of 4-tuples, containing the project name, homepage, the
+            backend, and the version.
+
+        Raises:
+             NotImplementedError: If backend does not
+                support batch updates.
+
+        """
+        raise NotImplementedError()
```

### Comparing `anitya-1.8.1/anitya/lib/backends/hackage.py` & `anitya-1.9.0/anitya/lib/backends/hackage.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         Attributes:
             project (:obj:`anitya.db.models.Project`): Project object whose backend
                 corresponds to the current plugin.
 
         Returns:
             str: url used for version checking
         """
-        url = "https://hackage.haskell.org/package/%(name)s" % {"name": project.name}
+        url = f"https://hackage.haskell.org/package/{project.name}"
 
         return url
 
     @classmethod
     def get_versions(cls, project):
         """Method called to retrieve all the versions (that can be found)
         of the projects provided, project that relies on the backend of
```

### Comparing `anitya-1.8.1/anitya/lib/backends/launchpad.py` & `anitya-1.9.0/anitya/lib/backends/launchpad.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         Attributes:
             project (:obj:`anitya.db.models.Project`): Project object whose backend
                 corresponds to the current plugin.
 
         Returns:
             str: url used for version checking
         """
-        url = "https://launchpad.net/%(name)s/+download" % {"name": project.name}
+        url = f"https://launchpad.net/{project.name}/+download"
 
         return url
 
     @classmethod
     def get_versions(cls, project):
         """Method called to retrieve all the versions (that can be found)
         of the projects provided, project that relies on the backend of
@@ -54,7 +54,25 @@
 
         """
         url = cls.get_version_url(project)
 
         regex = REGEX % {"name": project.name}
 
         return get_versions_by_regex(url, regex, project)
+
+    @classmethod
+    def check_feed(cls):  # pragma: no cover
+        """Method called to retrieve the latest uploads to a given backend,
+        via, for example, RSS or an API.
+
+        Not Supported
+
+        Returns:
+            :obj:`list`: A list of 4-tuples, containing the project name, homepage, the
+            backend, and the version.
+
+        Raises:
+             NotImplementedError: If backend does not
+                support batch updates.
+
+        """
+        raise NotImplementedError()
```

### Comparing `anitya-1.8.1/anitya/lib/backends/maven.py` & `anitya-1.9.0/anitya/lib/backends/maven.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,16 +45,17 @@
         else:
             coordinates = project.version_url or project.name
             match = COORDINATES_RE.match(coordinates)
             if not match:
                 return ""
             group_id = match.group(1)
             artifact_id = match.group(2)
-            url = "https://repo1.maven.org/maven2/{group_id}/{artifact_id}/".format(
-                group_id=group_id.replace(".", "/"), artifact_id=artifact_id
+            url = (
+                "https://repo1.maven.org/maven2/"
+                f"{group_id.replace('.', '/')}/{artifact_id}/"
             )
 
         return url
 
     @classmethod
     def get_versions(cls, project):
         """Method called to retrieve all the versions (that can be found)
@@ -73,7 +74,25 @@
         url = cls.get_version_url(project)
         if not url:
             raise AnityaPluginException(
                 "Aritfact needs to be in format groupId:artifactId"
             )
 
         return get_versions_by_regex(url, VERSION_REGEX, project)
+
+    @classmethod
+    def check_feed(cls):  # pragma: no cover
+        """Method called to retrieve the latest uploads to a given backend,
+        via, for example, RSS or an API.
+
+        Not Supported
+
+        Returns:
+            :obj:`list`: A list of 4-tuples, containing the project name, homepage, the
+            backend, and the version.
+
+        Raises:
+             NotImplementedError: If backend does not
+                support batch updates.
+
+        """
+        raise NotImplementedError()
```

### Comparing `anitya-1.8.1/anitya/lib/backends/npmjs.py` & `anitya-1.9.0/anitya/lib/backends/npmjs.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,25 +41,25 @@
 
         """
         url = cls.get_version_url(project)
         last_change = project.get_time_last_created_version()
 
         try:
             req = cls.call_url(url, last_change=last_change)
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("Could not contact %s" % url)
+        except Exception as err:  # pragma: no cover
+            raise AnityaPluginException(f"Could not contact {url}") from err
 
         # Not modified
         if req.status_code == 304:
             return None
 
         try:
             data = req.json()
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("No JSON returned by %s" % url)
+        except Exception as err:  # pragma: no cover
+            raise AnityaPluginException(f"No JSON returned by {url}") from err
 
         if "dist-tags" in data and "latest" in data["dist-tags"]:
             return data["dist-tags"]["latest"]
         else:
             return cls.get_ordered_versions(project)[-1]
 
     @classmethod
@@ -96,28 +96,28 @@
 
         """
         url = cls.get_version_url(project)
         last_change = project.get_time_last_created_version()
 
         try:
             req = cls.call_url(url, last_change=last_change)
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("Could not contact %s" % url)
+        except Exception as err:  # pragma: no cover
+            raise AnityaPluginException(f"Could not contact {url}") from err
 
         # Not modified
         if req.status_code == 304:
             return []
 
         try:
             data = req.json()
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("No JSON returned by %s" % url)
+        except Exception as err:  # pragma: no cover
+            raise AnityaPluginException(f"No JSON returned by {url}") from err
 
         if "error" in data or "versions" not in data:
-            raise AnityaPluginException("No versions found at %s" % url)
+            raise AnityaPluginException(f"No versions found at {url}")
 
         # Filter retrieved versions
         filtered_versions = BaseBackend.filter_versions(
             list(data["versions"].keys()), project.version_filter
         )
         return filtered_versions
 
@@ -135,23 +135,23 @@
             "&limit=40"
             "&include_docs=true"
             "&attachments=false"
         )
 
         try:
             response = cls.call_url(url)
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("Could not contact %s" % url)
+        except Exception as err:  # pragma: no cover
+            raise AnityaPluginException(f"Could not contact {url}") from err
 
         try:
             data = response.json()
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("No JSON returned by %s" % url)
+        except Exception as err:  # pragma: no cover
+            raise AnityaPluginException(f"No JSON returned by {url}") from err
 
         for item in data["results"]:
             if item.get("deleted"):
                 continue
             doc = item["doc"]
             name = doc["name"]
-            homepage = doc.get("homepage", "https://npmjs.org/package/%s" % name)
+            homepage = doc.get("homepage", f"https://npmjs.org/package/{name}")
             for version in doc.get("versions", []):
                 yield name, homepage, cls.name, version
```

### Comparing `anitya-1.8.1/anitya/lib/backends/packagist.py` & `anitya-1.9.0/anitya/lib/backends/rubygems.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,45 @@
 # -*- coding: utf-8 -*-
 
 """
  (c) 2014-2020 - Copyright Red Hat Inc
 
  Authors:
    Pierre-Yves Chibon <pingou@pingoured.fr>
+   Ralph Bean <rbean@redhat.com>
    Michal Konecny <mkonecny@redhat.com>
 
 """
 
-
 from anitya.lib.backends import BaseBackend
 from anitya.lib.exceptions import AnityaPluginException
 
 
-class PackagistBackend(BaseBackend):
-    """The custom class for projects hosted on packagist.org.
+class RubygemsBackend(BaseBackend):
+    """The custom class for projects hosted on rubygems.org.
+
+    This backend allows to specify a version_url and a regex that will
+    be used to retrieve the version information."""
 
-    This backend allows to specify a version_url that will be used to
-    retrieve the version information.
-    """
-
-    name = "Packagist"
-    examples = [
-        "https://packagist.org/packages/phpunit/php-code-coverage",
-        "https://packagist.org/packages/phpunit/php-timer",
-        "https://packagist.org/packages/<owner or group>/<project-name>",
-    ]
+    name = "Rubygems"
+    examples = ["https://rubygems.org/gems/aa", "https://rubygems.org/gems/bio"]
 
     @classmethod
     def get_version_url(cls, project):
         """Method called to retrieve the url used to check for new version
         of the project provided, project that relies on the backend of this plugin.
 
         Attributes:
             project (:obj:`anitya.db.models.Project`): Project object whose backend
                 corresponds to the current plugin.
 
         Returns:
             str: url used for version checking
         """
-        url = ""
-        url_template = "https://packagist.org/packages/%(user)s/%(name)s.json"
-
-        if project.version_url:
-            url = url_template % {"name": project.name, "user": project.version_url}
+        url = f"https://rubygems.org/api/v1/versions/{project.name}/latest.json"
 
         return url
 
     @classmethod
     def get_versions(cls, project):
         """Method called to retrieve all the versions (that can be found)
         of the projects provided, project that relies on the backend of
@@ -60,38 +51,57 @@
         :return type: list
         :raise AnityaPluginException: a
             :class:`anitya.lib.exceptions.AnityaPluginException` exception
             when the versions cannot be retrieved correctly
 
         """
         url = cls.get_version_url(project)
-        if not url:
-            raise AnityaPluginException(
-                "Project {} is not correctly set up.".format(project.name)
-            )
 
         last_change = project.get_time_last_created_version()
         try:
             req = cls.call_url(url, last_change=last_change)
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("Could not contact %s" % url)
+        except Exception as exc:  # pragma: no cover
+            raise AnityaPluginException(f"Could not contact {url}") from exc
 
         # Not modified
         if req.status_code == 304:
             return []
 
         try:
             data = req.json()
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("No JSON returned by %s" % url)
+        except Exception as exc:  # pragma: no cover
+            raise AnityaPluginException(f"No JSON returned by {url}") from exc
 
-        if "package" in data and "versions" in data["package"]:
-            # Filter retrieved versions
-            filtered_versions = cls.filter_versions(
-                sorted(data["package"]["versions"].keys()), project.version_filter
-            )
-
-            return filtered_versions
-        elif "status" in data and data["status"] == "error" and "message" in data:
-            raise AnityaPluginException(data["message"])
-        else:
-            raise AnityaPluginException("Invalid JSON returned by %s" % url)
+        if data["version"] == "unknown":
+            raise AnityaPluginException(
+                f"Project or version unknown at {url}"
+            )  # pragma: no cover
+
+        # Filter retrieved versions
+        filtered_versions = cls.filter_versions(
+            [data["version"]], project.version_filter
+        )
+        return filtered_versions
+
+    @classmethod
+    def check_feed(cls):
+        """Return a generator over the latest 50 uploads to rubygems.org
+
+        by querying the JSON API.
+        """
+
+        url = "https://rubygems.org/api/v1/activity/just_updated.json"
+
+        try:
+            response = cls.call_url(url)
+        except Exception as exc:  # pragma: no cover
+            raise AnityaPluginException(f"Could not contact {url}") from exc
+
+        try:
+            data = response.json()
+        except Exception as exc:  # pragma: no cover
+            raise AnityaPluginException(f"No XML returned by {url}") from exc
+
+        for item in data:
+            name, version = item["name"], item["version"]
+            homepage = f"https://rubygems.org/gems/{name}"
+            yield name, homepage, cls.name, version
```

### Comparing `anitya-1.8.1/anitya/lib/backends/pear.py` & `anitya-1.9.0/anitya/lib/backends/pear.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,25 +6,25 @@
  Authors:
    Pierre-Yves Chibon <pingou@pingoured.fr>
    Ralph Bean <rbean@redhat.com>
    Michal Konecny <mkonecny@redhat.com>
 
 """
 
-import anitya.lib.xml2dict as xml2dict
+from anitya.lib import xml2dict
 from anitya.lib.backends import BaseBackend
 from anitya.lib.exceptions import AnityaPluginException
 
 
 def _get_versions(url):
     """Retrieve the versions for the provided url."""
     try:
         req = PearBackend.call_url(url)
-    except Exception:  # pragma: no cover
-        raise AnityaPluginException("Could not contact %s" % url)
+    except Exception as err:  # pragma: no cover
+        raise AnityaPluginException(f"Could not contact {url}") from err
 
     data = req.text
     versions = []
     for line in data.split("\n"):
         if "<v>" in line and "</v>" in line:
             version = line.split("v>", 2)[1].split("</")[0]
             versions.append(version)
@@ -98,17 +98,15 @@
 
         """
         url = cls.get_version_url(project)
         versions = []
         versions = _get_versions(url)
 
         if not versions:
-            raise AnityaPluginException(
-                "No versions found for %s" % project.name.lower()
-            )
+            raise AnityaPluginException(f"No versions found for {project.name.lower()}")
 
         # Filter retrieved versions
         filtered_versions = cls.filter_versions(versions, project.version_filter)
 
         return filtered_versions
 
     @classmethod
@@ -118,22 +116,22 @@
         by querying an RSS feed.
         """
 
         url = "https://pear.php.net/feeds/latest.rss"
 
         try:
             response = cls.call_url(url)
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("Could not contact %s" % url)
+        except Exception as err:  # pragma: no cover
+            raise AnityaPluginException(f"Could not contact {url}") from err
 
         try:
             parser = xml2dict.XML2Dict()
             data = parser.fromstring(response.text)
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("No XML returned by %s" % url)
+        except Exception as err:  # pragma: no cover
+            raise AnityaPluginException(f"No XML returned by {url}") from err
 
         items = data["RDF"]["item"]
         for entry in items:
             title = entry["title"]["value"]
             name, version = title.rsplit(None, 1)
-            homepage = "https://pear.php.net/package/%s" % name
+            homepage = f"https://pear.php.net/package/{name}"
             yield name, homepage, cls.name, version
```

### Comparing `anitya-1.8.1/anitya/lib/backends/pecl.py` & `anitya-1.9.0/anitya/lib/backends/pecl.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
  Authors:
    Pierre-Yves Chibon <pingou@pingoured.fr>
    Ralph Bean <rbean@redhat.com>
 
 """
 
-import anitya.lib.xml2dict as xml2dict
+from anitya.lib import xml2dict
 from anitya.lib.backends import BaseBackend
 from anitya.lib.exceptions import AnityaPluginException
 
 
 def _get_versions(url):
     """Retrieve the versions for the provided url."""
     try:
         req = PeclBackend.call_url(url)
-    except Exception:  # pragma: no cover
-        raise AnityaPluginException("Could not contact %s" % url)
+    except Exception as exc:  # pragma: no cover
+        raise AnityaPluginException(f"Could not contact {url}") from exc
 
     data = req.text
     versions = []
     for line in data.split("\n"):
         if "<v>" in line and "</v>" in line:
             version = line.split("v>", 2)[1].split("</")[0]
             versions.append(version)
@@ -97,17 +97,15 @@
 
         """
         url = cls.get_version_url(project)
         versions = []
         versions = _get_versions(url)
 
         if not versions:
-            raise AnityaPluginException(
-                "No versions found for %s" % project.name.lower()
-            )
+            raise AnityaPluginException(f"No versions found for {project.name.lower()}")
 
         # Filter retrieved versions
         filtered_versions = BaseBackend.filter_versions(
             versions, project.version_filter
         )
         return filtered_versions
 
@@ -118,22 +116,22 @@
         by querying an RSS feed.
         """
 
         url = "https://pecl.php.net/feeds/latest.rss"
 
         try:
             response = cls.call_url(url)
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("Could not contact %s" % url)
+        except Exception as exc:  # pragma: no cover
+            raise AnityaPluginException(f"Could not contact {url}") from exc
 
         try:
             parser = xml2dict.XML2Dict()
             data = parser.fromstring(response.text)
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("No XML returned by %s" % url)
+        except Exception as exc:  # pragma: no cover
+            raise AnityaPluginException(f"No XML returned by {url}") from exc
 
         items = data["RDF"]["item"]
         for entry in items:
             title = entry["title"]["value"]
             name, version = title.rsplit(None, 1)
-            homepage = "https://pecl.php.net/package/%s" % name
+            homepage = f"https://pecl.php.net/package/{name}"
             yield name, homepage, cls.name, version
```

### Comparing `anitya-1.8.1/anitya/lib/backends/pypi.py` & `anitya-1.9.0/anitya/lib/backends/pypi.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
  Authors:
    Pierre-Yves Chibon <pingou@pingoured.fr>
    Ralph Bean <rbean@redhat.com>
    Michal Konecny <mkonecny@redhat.com>
 
 """
 
-import anitya.lib.xml2dict as xml2dict
+from anitya.lib import xml2dict
 from anitya.lib.backends import BaseBackend
 from anitya.lib.exceptions import AnityaPluginException
 
 
 class PypiBackend(BaseBackend):
     """The PyPI class for project hosted on PyPI."""
 
@@ -38,25 +38,25 @@
             when the version cannot be retrieved correctly
 
         """
         url = cls.get_version_url(project)
         last_change = project.get_time_last_created_version()
         try:
             req = cls.call_url(url, last_change=last_change)
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("Could not contact %s" % url)
+        except Exception as err:  # pragma: no cover
+            raise AnityaPluginException(f"Could not contact {url}") from err
 
         # Not modified
         if req.status_code == 304:
             return None
 
         try:
             data = req.json()
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("No JSON returned by %s" % url)
+        except Exception as err:  # pragma: no cover
+            raise AnityaPluginException(f"No JSON returned by {url}") from err
 
         return data["info"]["version"]
 
     @classmethod
     def get_version_url(cls, project):
         """Method called to retrieve the url used to check for new version
         of the project provided, project that relies on the backend of this plugin.
@@ -64,15 +64,15 @@
         Attributes:
             project (:obj:`anitya.db.models.Project`): Project object whose backend
                 corresponds to the current plugin.
 
         Returns:
             str: url used for version checking
         """
-        url = "https://pypi.org/pypi/%s/json" % project.name
+        url = f"https://pypi.org/pypi/{project.name}/json"
 
         return url
 
     @classmethod
     def get_versions(cls, project):
         """Method called to retrieve all the versions (that can be found)
         of the projects provided, project that relies on the backend of
@@ -87,25 +87,25 @@
             when the versions cannot be retrieved correctly
 
         """
         url = cls.get_version_url(project)
         last_change = project.get_time_last_created_version()
         try:
             req = cls.call_url(url, last_change=last_change)
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("Could not contact %s" % url)
+        except Exception as err:  # pragma: no cover
+            raise AnityaPluginException(f"Could not contact {url}") from err
 
         # Not modified
         if req.status_code == 304:
             return []
 
         try:
             data = req.json()
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("No JSON returned by %s" % url)
+        except Exception as err:  # pragma: no cover
+            raise AnityaPluginException(f"No JSON returned by {url}") from err
 
         # Filter yanked versions
         unyanked_versions = []
 
         # Just return empty list if "releases" key is missing in json
         if "releases" not in data:
             return []
@@ -132,22 +132,22 @@
         by querying an RSS feed.
         """
 
         url = "https://pypi.org/rss/updates.xml"
 
         try:
             response = cls.call_url(url)
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("Could not contact %s" % url)
+        except Exception as err:  # pragma: no cover
+            raise AnityaPluginException(f"Could not contact {url}") from err
 
         try:
             parser = xml2dict.XML2Dict()
             data = parser.fromstring(response.text)
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("No XML returned by %s" % url)
+        except Exception as err:  # pragma: no cover
+            raise AnityaPluginException(f"No XML returned by {url}") from err
 
         items = data["rss"]["channel"]["item"]
         for entry in items:
             title = entry["title"]["value"]
             name, version = title.rsplit(None, 1)
-            homepage = "https://pypi.org/project/%s/" % name
+            homepage = f"https://pypi.org/project/{name}/"
             yield name, homepage, cls.name, version
```

### Comparing `anitya-1.8.1/anitya/lib/backends/rubygems.py` & `anitya-1.9.0/anitya/lib/backends/pagure.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,62 @@
 # -*- coding: utf-8 -*-
 
 """
- (c) 2014-2020 - Copyright Red Hat Inc
+ (c) 2015-2020 - Copyright Red Hat Inc
 
  Authors:
    Pierre-Yves Chibon <pingou@pingoured.fr>
-   Ralph Bean <rbean@redhat.com>
    Michal Konecny <mkonecny@redhat.com>
 
 """
 
+
+from __future__ import print_function
+
 from anitya.lib.backends import BaseBackend
 from anitya.lib.exceptions import AnityaPluginException
 
 
-class RubygemsBackend(BaseBackend):
-    """The custom class for projects hosted on rubygems.org.
+class PagureBackend(BaseBackend):
+    """The pagure class for project hosted on pagure.io."""
+
+    name = "pagure"
+    examples = ["https://pagure.io/pagure", "https://pagure.io/flask-multistatic"]
+
+    @classmethod
+    def get_version(cls, project):
+        """Method called to retrieve the latest version of the projects
+        provided, project that relies on the backend of this plugin.
 
-    This backend allows to specify a version_url and a regex that will
-    be used to retrieve the version information."""
+        :arg Project project: a :class:`anitya.db.models.Project` object whose backend
+            corresponds to the current plugin.
+        :return: the latest version found upstream
+        :return type: str
+        :raise AnityaPluginException: a
+            :class:`anitya.lib.exceptions.AnityaPluginException` exception
+            when the version cannot be retrieved correctly
 
-    name = "Rubygems"
-    examples = ["https://rubygems.org/gems/aa", "https://rubygems.org/gems/bio"]
+        """
+        versions = cls.get_ordered_versions(project)
+        if versions:
+            return versions[-1]
 
     @classmethod
     def get_version_url(cls, project):
         """Method called to retrieve the url used to check for new version
         of the project provided, project that relies on the backend of this plugin.
 
         Attributes:
             project (:obj:`anitya.db.models.Project`): Project object whose backend
                 corresponds to the current plugin.
 
         Returns:
             str: url used for version checking
         """
-        url = "https://rubygems.org/api/v1/versions/%(name)s/latest.json" % {
-            "name": project.name
-        }
+        url = f"https://pagure.io/api/0/{project.name}/git/tags"
 
         return url
 
     @classmethod
     def get_versions(cls, project):
         """Method called to retrieve all the versions (that can be found)
         of the projects provided, project that relies on the backend of
@@ -53,55 +68,46 @@
         :return type: list
         :raise AnityaPluginException: a
             :class:`anitya.lib.exceptions.AnityaPluginException` exception
             when the versions cannot be retrieved correctly
 
         """
         url = cls.get_version_url(project)
-
         last_change = project.get_time_last_created_version()
         try:
             req = cls.call_url(url, last_change=last_change)
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("Could not contact %s" % url)
+        except Exception as err:  # pragma: no cover
+            raise AnityaPluginException(f"Could not contact {url}: {str(err)}") from err
 
         # Not modified
         if req.status_code == 304:
             return []
 
         try:
             data = req.json()
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("No JSON returned by %s" % url)
-
-        if data["version"] == "unknown":
-            raise AnityaPluginException("Project or version unknown at %s" % url)
+        except Exception as err:  # pragma: no cover
+            raise AnityaPluginException(f"No JSON returned by {url}") from err
 
         # Filter retrieved versions
         filtered_versions = cls.filter_versions(
-            [data["version"]], project.version_filter
+            data.get("tags", []), project.version_filter
         )
+
         return filtered_versions
 
     @classmethod
-    def check_feed(cls):
-        """Return a generator over the latest 50 uploads to rubygems.org
+    def check_feed(cls):  # pragma: no cover
+        """Method called to retrieve the latest uploads to a given backend,
+        via, for example, RSS or an API.
 
-        by querying the JSON API.
-        """
+        Not Supported
 
-        url = "https://rubygems.org/api/v1/activity/just_updated.json"
+        Returns:
+            :obj:`list`: A list of 4-tuples, containing the project name, homepage, the
+            backend, and the version.
 
-        try:
-            response = cls.call_url(url)
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("Could not contact %s" % url)
+        Raises:
+             NotImplementedError: If backend does not
+                support batch updates.
 
-        try:
-            data = response.json()
-        except Exception:  # pragma: no cover
-            raise AnityaPluginException("No XML returned by %s" % url)
-
-        for item in data:
-            name, version = item["name"], item["version"]
-            homepage = "https://rubygems.org/gems/%s" % name
-            yield name, homepage, cls.name, version
+        """
+        raise NotImplementedError()
```

### Comparing `anitya-1.8.1/anitya/lib/backends/sourceforge_git.py` & `anitya-1.9.0/anitya/lib/backends/sourceforge_git.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-
+"""sourceforge_git"""
 import requests
 from bs4 import BeautifulSoup
 
 from anitya.lib.backends import BaseBackend
 from anitya.lib.exceptions import AnityaPluginException
 
 
@@ -95,20 +95,20 @@
         :raise AnityaPluginException: a
             :class:`anitya.lib.exceptions.AnityaPluginException` exception
             when the versions cannot be retrieved correctly
 
         """
         namespace, repo = cls.get_namespace_repo(project)
         url = project.get_version_url()
-        git_tag_request = requests.get(url)
+        git_tag_request = requests.get(url)  # pylint: disable=W3101
 
         if git_tag_request.status_code == 404:
             raise AnityaPluginException(
-                'Could not call : "%s" of "%s", with error: %s'
-                % (url, project.name, git_tag_request.status_code)
+                f'Could not call : "{url}" of "{project.name}", with error: '
+                f"{git_tag_request.status_code}"
             )
 
         soup = BeautifulSoup(git_tag_request.content, "html.parser")
 
         def is_release_tag_link(tag):
             link_prefix = f"/p/{namespace}/{repo}/ci/"
             return (
@@ -120,7 +120,25 @@
         release_tags = []
 
         for release_tag in soup.find_all(is_release_tag_link):
             release_tag_text = release_tag.contents[0]
             release_tags.append(release_tag_text)
 
         return release_tags
+
+    @classmethod
+    def check_feed(cls):  # pragma: no cover
+        """Method called to retrieve the latest uploads to a given backend,
+        via, for example, RSS or an API.
+
+        Not Supported
+
+        Returns:
+            :obj:`list`: A list of 4-tuples, containing the project name, homepage, the
+            backend, and the version.
+
+        Raises:
+             NotImplementedError: If backend does not
+                support batch updates.
+
+        """
+        raise NotImplementedError()
```

### Comparing `anitya-1.8.1/anitya/lib/backends/sourcehut.py` & `anitya-1.9.0/anitya/lib/backends/sourcehut.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # useful, but WITHOUT ANY WARRANTY expressed or implied, including the
 # implied warranties of MERCHANTABILITY or FITNESS FOR A PARTICULAR
 # PURPOSE.  See the GNU General Public License for more details.  You
 # should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301, USA.
 #
-
+"""sourcehut"""
 from defusedxml import ElementTree
 
 from anitya.lib.backends import BaseBackend
 from anitya.lib.exceptions import AnityaPluginException
 
 
 class SourceHutBackend(BaseBackend):
@@ -68,31 +68,48 @@
 
         Returns:
             str: a list of all the possible releases found
         """
         url = cls.get_version_url(project)
         if not url:
             raise AnityaPluginException(
-                "Project %s was incorrectly set up" % project.name
+                f"Project {project.name} was incorrectly set up"
             )
 
         last_change = project.get_time_last_created_version()
         res = cls.call_url(url, last_change)
         if res.status_code == 200:
             xml = ElementTree.fromstring(res.text)
         elif res.status_code == 304:
             return []
         else:
             raise AnityaPluginException(
-                '%s: Server responded with status "%s": "%s"'
-                % (project.name, res.status_code, res.reason)
+                f"{project.name}: Server responded with status "
+                f'"{res.status_code}": "{res.reason}"'
             )
 
         versions = [i.find("title").text for i in xml.find("channel").findall("item")]
 
         if len(versions) == 0:
             raise AnityaPluginException(
-                "%(name)s: no upstream version found. - %(url)s -  "
-                % {"name": project.name, "url": url}
+                f"{project.name}: no upstream version found. - {url} -  "
             )
 
         return cls.filter_versions(versions, project.version_filter)
+
+    @classmethod
+    def check_feed(cls):  # pragma: no cover
+        """Method called to retrieve the latest uploads to a given backend,
+        via, for example, RSS or an API.
+
+        Not Supported
+
+        Returns:
+            :obj:`list`: A list of 4-tuples, containing the project name, homepage, the
+            backend, and the version.
+
+        Raises:
+             NotImplementedError: If backend does not
+                support batch updates.
+
+        """
+        raise NotImplementedError()
```

### Comparing `anitya-1.8.1/anitya/lib/backends/stackage.py` & `anitya-1.9.0/anitya/lib/backends/stackage.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         Attributes:
             project (:obj:`anitya.db.models.Project`): Project object whose backend
                 corresponds to the current plugin.
 
         Returns:
             str: url used for version checking
         """
-        url = "https://www.stackage.org/package/%(name)s" % {"name": project.name}
+        url = f"https://www.stackage.org/package/{project.name}"
 
         return url
 
     @classmethod
     def get_versions(cls, project):
         """Method called to retrieve all the versions (that can be found)
         of the projects provided, project that relies on the backend of
@@ -50,12 +50,30 @@
         :raise AnityaPluginException: a
             :class:`anitya.lib.exceptions.AnityaPluginException` exception
             when the versions cannot be retrieved correctly
         """
         url = cls.get_version_url(project)
 
         regex = (
-            r"<a href=\"https://hackage.haskell.org/package/%s\"><span class=\"version\">"
-            r"([\d.]*).*</span></a>" % project.name
+            rf"<a href=\"https://hackage.haskell.org/package/{project.name}\">"
+            r"<span class=\"version\">([\d.]*).*</span></a>"
         )
 
         return get_versions_by_regex(url, regex, project)
+
+    @classmethod
+    def check_feed(cls):  # pragma: no cover
+        """Method called to retrieve the latest uploads to a given backend,
+        via, for example, RSS or an API.
+
+        Not Supported
+
+        Returns:
+            :obj:`list`: A list of 4-tuples, containing the project name, homepage, the
+            backend, and the version.
+
+        Raises:
+             NotImplementedError: If backend does not
+                support batch updates.
+
+        """
+        raise NotImplementedError()
```

### Comparing `anitya-1.8.1/anitya/lib/ecosystems/__init__.py` & `anitya-1.9.0/anitya/lib/ecosystems/__init__.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/lib/ecosystems/crates.py` & `anitya-1.9.0/anitya/lib/ecosystems/crates.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/lib/exceptions.py` & `anitya-1.9.0/anitya/lib/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     outside of an ecosystem have no uniqueness constraints.
     """
 
     def __init__(self, requested_project):
         self.requested_project = requested_project
 
     def to_dict(self):
+        """to_dict"""
         return {"requested_project": self.requested_project.__json__()}
 
     def __str__(self):
         return "Unable to create project since it already exists."
 
 
 class AnityaInvalidMappingException(AnityaException):
@@ -76,26 +77,20 @@
         self.found_distro = found_distro
         self.project_id = project_id
         self.project_name = project_name
         self.link = link
 
     @property
     def message(self):
+        """message"""
         return (
-            "Could not edit the mapping of {pkgname} on "
-            "{distro}, there is already a package {found_pkgname} on "
-            '{found_distro} as part of the project <a href="{link}">'
-            "{project_name}</a>.".format(
-                pkgname=self.pkgname,
-                distro=self.distro,
-                found_pkgname=self.found_pkgname,
-                found_distro=self.found_distro,
-                project_name=self.project_name,
-                link=self.link,
-            )
+            f"Could not edit the mapping of {self.pkgname} on "
+            f"{self.distro}, there is already a package {self.found_pkgname} on "
+            f'{self.found_distro} as part of the project <a href="{self.link}">'
+            f"{self.project_name}</a>."
         )
 
 
 class InvalidVersion(AnityaException):
     """
     Raised when the version string is not valid for the given version scheme.
 
@@ -106,19 +101,17 @@
 
     def __init__(self, version, exception=None):
         self.version = version
         self.exception = exception
 
     def __str__(self):
         if self.exception:
-            return 'Invalid version "{v}": {e}'.format(
-                v=self.version, e=str(self.exception)
-            )
+            return f'Invalid version "{self.version}": {str(self.exception)}'
         else:
-            return 'Invalid version "{v}"'.format(v=self.version)
+            return f'Invalid version "{self.version}"'
 
 
 class RateLimitException(AnityaException):
     """
     Raised when the rate limit for requests is reached.
 
     Attributes:
@@ -131,10 +124,8 @@
 
         Arguments:
             reset_time (str): Time when limit will be reset (UTC time encoded in ISO-8601).
         """
         self.reset_time = arrow.get(reset_time)
 
     def __str__(self):
-        return 'Rate limit was reached. Will be reset in "{0}".'.format(
-            str(self.reset_time)
-        )
+        return f'Rate limit was reached. Will be reset in "{str(self.reset_time)}".'
```

### Comparing `anitya-1.8.1/anitya/lib/plugins.py` & `anitya-1.9.0/anitya/lib/plugins.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/lib/utilities.py` & `anitya-1.9.0/anitya/lib/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 
 import logging
 
 import arrow
 from fedora_messaging import api
 from fedora_messaging import exceptions as fm_exceptions
 from fedora_messaging import message as fm_message
-from sqlalchemy.exc import IntegrityError, SQLAlchemyError
-from sqlalchemy.orm.exc import NoResultFound
+from sqlalchemy import exc, orm
 
 from anitya.db import models
 
 from . import exceptions, plugins
 
 _log = logging.getLogger(__name__)
 
@@ -44,15 +43,15 @@
         distro (str): Name of the distribution
         message (dict): Additional data needed for the topic
     """
 
     msg = dict(project=project, distro=distro, message=message)
     try:
         message_class = fm_message.get_class("anitya." + topic)
-        api.publish(message_class(topic="anitya.{}".format(topic), body=msg))
+        api.publish(message_class(topic=f"anitya.{topic}", body=msg))
     except (
         fm_exceptions.ConnectionException,
         fm_exceptions.PublishException,
     ) as err:
         # For now, continue just logging the error. Once the messaging has
         # been untangled into SQLAlchemy events, it should probably result
         # in an exception and the client should try again later.
@@ -64,15 +63,15 @@
 
     :arg package: a Package object has defined in anitya.db.modelss.Project
 
     """
     backend = plugins.get_plugin(project.backend)
     if not backend:
         raise exceptions.AnityaException(
-            'No backend was found for "%s"' % project.backend
+            f'No backend was found for "{project.backend}"'
         )
 
     if project.archived:
         raise exceptions.AnityaException(
             "Project is archived, can't check new versions"
         )
 
@@ -82,26 +81,26 @@
     # don't change actual data during test run
     if not test:
         project.last_check = arrow.utcnow().datetime
         project.next_check = project.last_check + backend.check_interval
 
     try:
         versions_prefix = backend.get_versions(project)
-        _log.debug("Versions retrieved: '{}'".format(versions_prefix))
+        _log.debug("Versions retrieved: '%s'", versions_prefix)
     except exceptions.RateLimitException as err:
-        _log.error(f"{project.name} ({project.backend}): {str(err)}")
+        _log.error("%s (%s): %s", project.name, project.backend, str(err))
         if not test:
             project.logs = str(err)
             project.next_check = err.reset_time.to("utc").datetime
             project.check_successful = False
             session.add(project)
             session.commit()
         raise
     except exceptions.AnityaPluginException as err:
-        _log.error(f"{project.name} ({project.backend}): {str(err)}")
+        _log.error("%s (%s): %s", project.name, project.backend, str(err))
         if not test:
             project.logs = str(err)
             project.check_successful = False
             project.error_counter += 1
             session.add(project)
             session.commit()
         raise
@@ -131,17 +130,15 @@
                         version=version.version,
                         commit_url=version.commit_url,
                     )
                 )
                 upstream_versions.append(version.parse())
             else:
                 _log.info(
-                    "Version '{}' was skipped. Reason: too long.".format(
-                        version.version
-                    )
+                    "Version '%s' was skipped. Reason: too long.", version.version
                 )
 
     sorted_versions = project.get_sorted_version_objects()
     if sorted_versions:
         max_version_obj = sorted_versions[0]
         max_version = max_version_obj.parse()
     if project.latest_version != max_version:
@@ -222,18 +219,18 @@
         releases_only=releases_only,
     )
 
     session.add(project)
 
     try:
         session.flush()
-    except IntegrityError:
+    except exc.IntegrityError as exception:
         session.rollback()
-        raise exceptions.ProjectExists(project)
-    except SQLAlchemyError as err:
+        raise exceptions.ProjectExists(project) from exception
+    except exc.SQLAlchemyError as err:
         _log.exception(err)
         session.rollback()
         raise exceptions.AnityaException("Could not add this project, already exists?")
 
     if not dry_run:
         publish_message(
             project=project.__json__(),
@@ -346,15 +343,15 @@
                 session.add(project)
                 session.commit()
             if check_release is True:
                 check_project_release(project, session)
         else:
             session.add(project)
             session.flush()
-    except SQLAlchemyError as err:
+    except exc.SQLAlchemyError as err:
         _log.exception(err)
         session.rollback()
         raise exceptions.AnityaException(
             "Could not edit this project. Is there already a project "
             "with these name and homepage?"
         )
 
@@ -389,49 +386,49 @@
     distro_obj = models.Distro.get(session, distribution)
 
     if not distro_obj:
         distro_obj = models.Distro(name=distribution)
         session.add(distro_obj)
         try:
             session.flush()
-        except SQLAlchemyError:
+        except exc.SQLAlchemyError as exception:
             session.rollback()
             raise exceptions.AnityaException(
-                "Could not add the distribution %s to the database, "
-                "please inform an admin." % distribution,
+                f"Could not add the distribution {distribution} to the database, "
+                "please inform an admin.",
                 "errors",
-            )
+            ) from exception
 
         publish_message(
             distro=distro_obj.__json__(),
             topic="distro.add",
             message=dict(agent=user_id, distro=distro_obj.name),
         )
         session.add(distro_obj)
         try:
             session.flush()
-        except SQLAlchemyError:  # pragma: no cover
+        except exc.SQLAlchemyError as exception:  # pragma: no cover
             # We cannot test this situation
             session.rollback()
             raise exceptions.AnityaException(
-                "Could not add the distribution %s to the database, "
-                "please inform an admin." % distribution,
+                f"Could not add the distribution {distribution} to the database, "
+                "please inform an admin.",
                 "errors",
-            )
+            ) from exception
 
     pkgname = old_package_name or package_name
     distro = old_distro_name or distribution
     pkg = models.Packages.get(session, project.id, distro, pkgname)
 
     # See if the new mapping would clash with an existing mapping
     try:
         other_pkg = models.Packages.query.filter_by(
             distro_name=distribution, package_name=package_name
         ).one()
-    except NoResultFound:
+    except orm.exc.NoResultFound:
         other_pkg = None
     # Only raise exception if the package is already associated
     # to project
     if other_pkg and other_pkg.project:
         raise exceptions.AnityaInvalidMappingException(
             pkgname,
             distro,
@@ -462,20 +459,20 @@
         if pkg.package_name != package_name:
             pkg.package_name = package_name
             edited.append("package_name")
 
     session.add(pkg)
     try:
         session.flush()
-    except SQLAlchemyError as err:
+    except exc.SQLAlchemyError as err:
         _log.exception(err)
         session.rollback()
         raise exceptions.AnityaException(
-            "Could not add the mapping of %s to %s, please inform an "
-            "admin." % (package_name, distribution)
+            f"Could not add the mapping of {package_name} to {distribution}, please inform an "
+            "admin."
         )
 
     message = dict(
         agent=user_id, project=project.name, distro=distro_obj.name, new=package_name
     )
     if edited:
         message["prev"] = old_package_name or package_name
@@ -496,15 +493,15 @@
 
     flag = models.ProjectFlag(user=user_email, project=project, reason=reason)
 
     session.add(flag)
 
     try:
         session.flush()
-    except SQLAlchemyError as err:
+    except exc.SQLAlchemyError as err:
         _log.exception(err)
         session.rollback()
         raise exceptions.AnityaException("Could not flag this project.")
 
     publish_message(
         project=project.__json__(),
         topic="project.flag",
@@ -528,15 +525,15 @@
         raise exceptions.AnityaException("Flag state unchanged.")
 
     flag.state = state
     session.add(flag)
 
     try:
         session.flush()
-    except SQLAlchemyError as err:
+    except exc.SQLAlchemyError as err:
         _log.exception(err)
         session.rollback()
         raise exceptions.AnityaException("Could not set the state of this flag.")
 
     publish_message(
         topic="project.flag.set",
         message=dict(agent=user_id, flag=flag.id, state=state),
@@ -546,12 +543,12 @@
 
 
 def get_last_cron(session):
     """Retrieve the last log entry about the cron"""
     return models.Run.last_entry(session)
 
 
-def remove_suffix(str, suffix):
+def remove_suffix(string, suffix):
     """Removes suffix from the given str"""
-    if str.endswith(suffix):
-        return str[: -len(suffix)]
-    return str
+    if string.endswith(suffix):
+        return string[: -len(suffix)]
+    return string
```

### Comparing `anitya-1.8.1/anitya/lib/versions/__init__.py` & `anitya-1.9.0/anitya/lib/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/lib/versions/base.py` & `anitya-1.9.0/anitya/lib/versions/python.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,34 +13,42 @@
 # with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301, USA.
 #
 # Any Red Hat trademarks that are incorporated in the source
 # code or documentation are not subject to the GNU General Public
 # License and may only be used or replicated with the express permission
 # of Red Hat, Inc.
-"""The Anitya versions API."""
-
-from __future__ import unicode_literals
+"""
+This adds support for comparing project versions using the PEP 440 rules,
+as used on the `Python Package Index`_.
+
+See `Version scheme` in PEP 440.
+
+.. _Version scheme:
+   https://www.python.org/dev/peps/pep-0440/#version-scheme
+.. _Python Package Index:
+   https://pypi.org/
+"""
 
 import functools
-import re
 from datetime import datetime
 from typing import Optional
 
-from anitya.lib.exceptions import InvalidVersion
+# Import entire modules so it's clear which "Version" and "InvalidVersion"
+# is used
+import packaging.version
 
-#: A regular expression to determine if the version string contains a 'v' prefix.
-v_prefix = re.compile(r"v\d.*")
+from . import base
 
 
 @functools.total_ordering
-class Version(object):
-    """The base class for versions."""
+class PythonVersion(base.Version):
+    """Python (PEP 440) Version."""
 
-    name = "Generic Version"
+    name = "Python (PEP 440)"
 
     def __init__(
         self,
         version: Optional[str] = None,
         prefix: Optional[str] = None,
         created_on: Optional[datetime] = None,
         pattern: Optional[str] = None,
@@ -57,92 +65,72 @@
             created_on: Date of creation
             pattern: Calendar version pattern.
                 See `Calendar version scheme_` for more information.
             cursor: An opaque, backend-specific cursor pointing to the version.
             commit_url: A URL pointing to the commit tagged as the version.
             pre_release_filter: A filter used to identify pre-release versions
         """
-        self.version = version
-        if prefix:
-            self.prefixes = prefix.split(";")
-            # Sort from shorter to longest, this will prevent stripping
-            # shorter prefix instead of larger.
-            # For example:
-            # version = release_db-1.2.3
-            # prefixes = release_db-;release
-            # would return db-1.2.3 instead of 1.2.3 if the sort is not done
-            self.prefixes.sort(key=len)
-        else:
-            self.prefixes = []
-        self.created_on = created_on
-        self.pattern = None
-        if pattern:
-            self.pattern = pattern.upper()
-        self.cursor = cursor
-        self.commit_url = commit_url
-        if pre_release_filter:
-            self.pre_release_filters = pre_release_filter.split(";")
-        else:
-            self.pre_release_filters = []
+        super().__init__(
+            version, prefix, created_on, pattern, cursor, commit_url, pre_release_filter
+        )
 
-    def __str__(self):
-        """
-        Return a parsed, string version of this instance's version.
-        If parsing fails, the original version string is returned.
-        """
-        try:
-            return str(self.parse())
-        except InvalidVersion:
-            return self.version
+        self.version_object = self.get_version_object()
 
-    def parse(self):
+    def get_version_object(self):
         """
         Parse the version string to an object representing the version.
 
-        This does some minimal string processing, stripping any prefix set on
-        project.
 
         Returns:
-            str: The version string. Sub-classes may return a different type.
-            object: Sub-classes may return a special class that represents the
-            version. This must support comparison operations and return
-            a parsed, prefix-stripped version when ``__str__`` is invoked.
+            packaging.version.Version: This supports comparison operations and
+            returns a parsed, prefix-stripped version from ``__str__``.
 
         Raises:
-            InvalidVersion: If the version cannot be parsed.
+            base.InvalidVersion: If the version cannot be parsed.
         """
-        # If there's a prefix set on the project, strip it if it's present
-        version = self.version
-        for prefix in self.prefixes:
-            if prefix and self.version.startswith(prefix):
-                version = self.version[len(prefix) :].strip()
-
-        # Many projects prefix their tags with 'v', so strip it if it's present
-        if v_prefix.match(version):
-            version = version[1:]
+        # The base implementation does some minimal string processing
+        version = super().parse()
+        # The result should be usable with packaging.version
+        try:
+            return packaging.version.Version(version)
+        except packaging.version.InvalidVersion:
+            return None
 
-        return version
+    def parse(self):
+        """
+        Parse the version string and returns something usable by Anitya.
 
-    def prerelease(self):
+        Returns:
+          str: The version string processed by `packaging` module.
         """
-        Check if a version is a pre-release version.
+        if self.version_object:
+            return str(self.version_object)
+        else:
+            return super().parse()
 
-        This basic version implementation does not have a concept of
-        pre-releases.
+    def prerelease(self) -> bool:
         """
-        return False
+        Check this is a pre-release version.
+        """
+        if not self.version_object:
+            return False
+
+        if self.version_object.is_prerelease:
+            return True
+
+        return super().prerelease()
 
     def postrelease(self):
         """
-        Check if a version is a post-release version.
-
-        This basic version implementation does not have a concept of
-        post-releases.
+        Check this is a post-release version.
         """
-        return False
+        if not self.version_object:
+            return False
+
+        return self.version_object.is_postrelease
 
     def newer(self, other_versions):
         """
         Check a version against a list of other versions to see if it's newer.
 
         Example:
             >>> version = Version(version='1.1.0')
@@ -158,52 +146,37 @@
                 objects to check the `version` string against.
         Returns:
             bool: True if self is the newest version, ``False otherwise``.
         Raises:
             InvalidVersion: if one or more of the version
                 strings provided cannot be parsed.
         """
-        if isinstance(other_versions, (Version, str)):
+        if isinstance(other_versions, (base.Version, str)):
             other_versions = [other_versions]
         cast_versions = []
         for version in other_versions:
             if not isinstance(version, type(self)):
                 version = type(self)(version=version)
             cast_versions.append(version)
-        return all([self.parse() > v.parse() for v in cast_versions])
+        return all(  # pylint: disable=R1729
+            [self.version_object > v.version_object for v in cast_versions]
+        )
 
     def __lt__(self, other):
-        """Support < comparison via objects returned from :meth:`parse`"""
-        try:
-            parsed_self = self.parse()
-        except InvalidVersion:
-            parsed_self = None
-        try:
-            parsed_other = other.parse()
-        except InvalidVersion:
-            parsed_other = None
-
-        # Handle the cases where one or both aren't parsable. Parsable versions
-        # always sort higher than unparsable versions.
-        if not parsed_self and not parsed_other:
+        """Support < comparison via objects returned from :meth:`version_object`"""
+        # Handle the cases where one or both can't be validated. Validated versions
+        # always sort higher than unvalidated versions.
+        if not self.version_object and not other.version_object:
             return self.version.__lt__(other.version)
-        if not parsed_other:
+        if not other.version_object:
             return False
-        if not parsed_self:
+        if not self.version_object:
             return True
 
-        return parsed_self.__lt__(parsed_other)
+        return self.version_object.__lt__(other.version_object)
 
     def __eq__(self, other):
-        """Support == comparison via objects returned from :meth:`parse`"""
-        try:
-            parsed_self = self.parse()
-        except InvalidVersion:
-            parsed_self = None
-        try:
-            parsed_other = other.parse()
-        except InvalidVersion:
-            parsed_other = None
-
-        if not parsed_self or not parsed_other:
+        """Support == comparison via objects returned from :meth:`version_object`"""
+        # Handle the cases where one or both can't be validated.
+        if not self.version_object or not other.version_object:
             return self.version.__eq__(other.version)
-        return parsed_self.__eq__(parsed_other)
+        return self.version_object.__eq__(other.version_object)
```

### Comparing `anitya-1.8.1/anitya/lib/versions/calver.py` & `anitya-1.9.0/anitya/lib/versions/calver.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,16 @@
         rest_string = string[match.end() :]
         return match_string, rest_string
 
     return "", string
 
 
 class SplitResult(TypedDict, total=True):
+    """SplitResult"""
+
     year: Optional[str]
     month: Optional[str]
     day: Optional[str]
     minor: Optional[str]
     micro: Optional[str]
     modifier: Optional[str]
     rc_number: Optional[str]
@@ -142,64 +144,64 @@
             elif pattern_str.startswith("MM"):
                 try:
                     match = re.match(r"(1\d)|\d", version_str)
                     if match and 1 <= int(match.group(0)) <= 12:
                         month = match.group(0)
                     else:
                         raise ValueError("Can't parse version by pattern")
-                except ValueError:
-                    raise ValueError("Can't parse version by pattern")
+                except ValueError as err:
+                    raise ValueError("Can't parse version by pattern") from err
                 result_dict["month"] = month
                 index_version = len(month)
                 index_pattern = 2
             elif pattern_str.startswith("0M"):
                 try:
                     version = version_str[:2]
                     if 1 <= int(version) < 10 and re.fullmatch(r"(0\d)", version):
                         result_dict["month"] = version
                     elif 10 <= int(version) <= 12 and not re.fullmatch(
                         r"(0\d+)", version
                     ):
                         result_dict["month"] = version
                     else:
                         raise ValueError("Can't parse version by pattern")
-                except ValueError:
-                    raise ValueError("Can't parse version by pattern")
+                except ValueError as err:
+                    raise ValueError("Can't parse version by pattern") from err
                 index_version = 2
                 index_pattern = 2
             elif pattern_str.startswith("DD"):
                 try:
                     match = re.match(r"([1-3]\d)|\d", version_str)
                     if match and 1 <= int(match.group(0)) <= 31:
                         day = match.group(0)
                     else:
                         raise ValueError("Can't parse version by pattern")
-                except ValueError:
-                    raise ValueError("Can't parse version by pattern")
+                except ValueError as err:
+                    raise ValueError("Can't parse version by pattern") from err
                 result_dict["day"] = day
                 index_version = len(day)
                 index_pattern = 2
             elif pattern_str.startswith("0D"):
                 try:
                     version = version_str[:2]
                     if 1 <= int(version) < 10 and re.fullmatch(r"(0\d)", version):
                         result_dict["day"] = version
                     elif 10 <= int(version) <= 31 and not re.fullmatch(
                         r"(0\d+)", version
                     ):
                         result_dict["day"] = version
                     else:
                         raise ValueError("Can't parse version by pattern")
-                except ValueError:
-                    raise ValueError("Can't parse version by pattern")
+                except ValueError as err:
+                    raise ValueError("Can't parse version by pattern") from err
                 index_version = 2
                 index_pattern = 2
             elif pattern_str.startswith("MINOR"):
                 for index in range(1, len(version_str) + 1):
-                    if version_str[:index].isdigit():
+                    if version_str[:index].isdigit():  # pylint: disable=R1724
                         continue
                     else:
                         # First character is not number
                         if index == 1:
                             raise ValueError("Can't parse version by pattern")
                         index_version = index - 1
                         result_dict["minor"] = version_str[:index_version]
@@ -207,15 +209,15 @@
                 if index_version == 0:
                     # We are on the end of string
                     index_version = len(version_str)
                     result_dict["minor"] = version_str[:index_version]
                 index_pattern = 5
             elif pattern_str.startswith("MICRO"):
                 for index in range(1, len(version_str) + 1):
-                    if version_str[:index].isdigit():
+                    if version_str[:index].isdigit():  # pylint: disable=R1724
                         continue
                     else:
                         # First character is not number
                         if index == 1:
                             raise ValueError("Can't parse version by pattern")
                         index_version = index - 1
                         result_dict["micro"] = version_str[:index_version]
@@ -268,23 +270,15 @@
         except ValueError:
             # The version can't be parsed, so it's not pre-release
             return False
 
         if version_dict["modifier"]:
             return True
 
-        for pre_release_filter in self.pre_release_filters:
-            if (
-                pre_release_filter
-                and self.version
-                and pre_release_filter in self.version
-            ):
-                return True
-
-        return False
+        return super().prerelease()
 
     def __eq__(self, other) -> bool:
         """
         Compare two versions for equality using the calendar rules with pre-release
         support.
 
         Params:
@@ -296,25 +290,23 @@
         if not isinstance(other, Version):
             return NotImplemented
         try:
             version_dict_self = self.split()  # type: ignore
             version_dict_other = other.split()  # type: ignore
         except ValueError:
             # The version can't be split, so compare them as strings
-            if self.parse() == other.parse():
-                return True
-            else:
-                return False
+            return bool(self.parse() == other.parse())
 
         if version_dict_self == version_dict_other:
             return True
 
         return False
 
     def maybe_split(self) -> Optional[SplitResult]:
+        """maybe_split"""
         try:
             return self.split()
         except ValueError:
             return None
 
     def __lt__(self, other: Version) -> bool:
         """
```

### Comparing `anitya-1.8.1/anitya/lib/versions/rpm.py` & `anitya-1.9.0/anitya/lib/versions/rpm.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,29 +132,25 @@
         """
         match = cls._rc_upstream_regex.match(version)
         if not match or not match.group(1):
             return (version, "", "")
 
         return (match.group(1), match.group(3), match.group(4))
 
-    def prerelease(self):
+    def prerelease(self) -> bool:
         """
         Check if a version is a pre-release version.
 
         This recognizes versions containing "rc", "pre", "beta", "alpha", and
         "dev" as being pre-release versions.
         """
         if self.split_rc(self.parse())[1]:
             return True
 
-        for pre_release_filter in self.pre_release_filters:
-            if pre_release_filter and pre_release_filter in self.version:
-                return True
-
-        return False
+        return super().prerelease()
 
     def __eq__(self, other):
         """
         Compare two versions for equality using the RPM rules with pre-release
         support.
         """
         v1, rc1, rcn1 = self.split_rc(self.parse())
@@ -163,18 +159,15 @@
         v2, rc2, rcn2 = self.split_rc(other.parse())
         if not v2:
             return False
         result = _compare_rpm_labels((None, v1, None), (None, v2, None))
         if result != 0:
             return False
 
-        if rc1 == rc2 and rcn1 == rcn2:
-            return True
-        else:
-            return False
+        return bool(rc1 == rc2 and rcn1 == rcn2)
 
     def __lt__(self, other):
         v1, rc1, rcn1 = self.split_rc(self.parse())
         if not v1:
             return True
         v2, rc2, rcn2 = self.split_rc(other.parse())
         if not v2:
```

### Comparing `anitya-1.8.1/anitya/lib/versions/semver.py` & `anitya-1.9.0/anitya/lib/versions/semver.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     This implements an semantic version plugin.
 
     It sorts versions using the semantic Python library.
     """
 
     name = "Semantic"
 
-    def prerelease(self):
+    def prerelease(self) -> bool:
         """
         Check if a version is a pre-release version.
 
         This recognizes versions containing pre-release string according to semantic
         versioning standard. See `Semantic versioning`_.
 
         Returns:
@@ -60,19 +60,15 @@
         except ValueError:
             # version is not correct semantic version, so it's not a pre-release
             return False
 
         if version_info.prerelease:
             return True
 
-        for pre_release_filter in self.pre_release_filters:
-            if pre_release_filter and pre_release_filter in self.version:
-                return True
-
-        return False
+        return super().prerelease()
 
     def __eq__(self, other):
         """
         Compare two versions for equality using the semantic rules with pre-release
         support.
 
         Params:
```

### Comparing `anitya-1.8.1/anitya/lib/xml2dict.py` & `anitya-1.9.0/anitya/lib/xml2dict.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,16 @@
             return d
 
     def __setattr__(self, item, value):
         self.__setitem__(item, value)
 
 
 class XML2Dict(object):
+    """Class XML2Dict"""
+
     def _parse_node(self, node):
         node_tree = object_dict()
         # Save attrs and text, hope there will not be a child with same name
         if node.text:
             node_tree.value = node.text
         for k, v in node.attrib.items():
             k, v = self._namespace_split(k, object_dict({"value": v}))
@@ -77,16 +79,16 @@
         result = re.compile(r"\{(.*)\}(.*)").search(tag)
         if result:
             value.namespace, tag = result.groups()
         return (tag, value)
 
     def parse(self, file):
         """parse a xml file to a dict"""
-        f = open(file, "rb")
-        return self.fromstring(f.read())
+        with open(file, "rb") as f:  # pragma: no cover
+            return self.fromstring(f.read())
 
     def fromstring(self, s):
         """parse a string"""
         if isinstance(s, six.text_type):
             s = s.encode("utf-8")
         t = ET.fromstring(s)
         root_tag, root_tree = self._namespace_split(t.tag, self._parse_node(t))
```

### Comparing `anitya-1.8.1/anitya/mail_logging.py` & `anitya-1.9.0/anitya/mail_logging.py`

 * *Files 7% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         try:
             record.form = dict(flask.request.form)
             if "csrf_token" in record.form:
                 record.form["csrf_token"] = "Was present, is cleaned up"
         except RuntimeError:
             pass
         try:
-            record.username = "%s -- %s" % (flask.g.user.id, flask.g.user.email)
+            record.username = f"{flask.g.user.id} -- {flask.g.user.email}"
         except Exception:
             pass
 
         return True
 
     @staticmethod
     def format_callstack():
@@ -124,34 +124,34 @@
                 continue
             modname = frame.f_globals["__name__"].split(".")[0]
             if modname != "logging":
                 break
 
         def _format_frame(frame):
             """Format the frame."""
-            return '  File "%s", line %i in %s\n    %s' % (frame)
+            return f'  File "{frame}", line %i in {frame}\n    {frame}'
 
         stack = traceback.extract_stack()
         stack = stack[:-ind]
         return "\n".join([_format_frame(frame) for frame in stack])
 
     @staticmethod
     def get_current_process():
         """Return the current process (PID)."""
         mypid = os.getpid()
 
         if not psutil:
-            return "Could not import psutil for %r" % mypid
+            return f"Could not import psutil for {mypid!r}"
 
         for proc in psutil.process_iter():
             if proc.pid == mypid:
                 return proc
 
         # This should be impossible.
-        raise ValueError("Could not find process %r" % mypid)
+        raise ValueError(f"Could not find process {mypid!r}")
 
 
 MSG_FORMAT = """Process Details
 ---------------
 host:     %(host)s
 PID:      %(pid)s
 name:     %(proc_name)s
```

### Comparing `anitya-1.8.1/anitya/sar.py` & `anitya-1.9.0/anitya/sar.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,19 +49,19 @@
     db.initialize(config)
     sar_username = os.getenv("SAR_USERNAME")
     sar_email = os.getenv("SAR_EMAIL")
 
     users = []
 
     if sar_email:
-        _log.debug("Find users by e-mail {}".format(sar_email))
+        _log.debug("Find users by e-mail %s", sar_email)
         users = users + db.User.query.filter_by(email=sar_email).all()
 
     if sar_username:
-        _log.debug("Find users by username {}".format(sar_username))
+        _log.debug("Find users by username %s", sar_username)
         users = users + db.User.query.filter_by(username=sar_username).all()
 
     users_list = []
     for user in users:
         user_dict = user.to_dict()
         user_social_auths = db.Session.execute(
             "SELECT provider,extra_data,uid FROM social_auth_usersocialauth WHERE user_id = :val",
```

### Comparing `anitya-1.8.1/anitya/static/css/cnucnu.css` & `anitya-1.9.0/anitya/static/css/cnucnu.css`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Cantarell-Bold-webfont.eot` & `anitya-1.9.0/anitya/static/css/fonts/Cantarell-Bold-webfont.eot`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Cantarell-Bold-webfont.svg` & `anitya-1.9.0/anitya/static/css/fonts/Cantarell-Bold-webfont.svg`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Cantarell-Bold-webfont.ttf` & `anitya-1.9.0/anitya/static/css/fonts/Cantarell-Bold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Cantarell-Bold-webfont.woff` & `anitya-1.9.0/anitya/static/css/fonts/Cantarell-Bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.eot` & `anitya-1.9.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.eot`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.svg` & `anitya-1.9.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.svg`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.ttf` & `anitya-1.9.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.ttf`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.woff` & `anitya-1.9.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.woff`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Cantarell-Oblique-webfont.eot` & `anitya-1.9.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.eot`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Cantarell-Oblique-webfont.svg` & `anitya-1.9.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.svg`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Cantarell-Oblique-webfont.ttf` & `anitya-1.9.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.ttf`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Cantarell-Oblique-webfont.woff` & `anitya-1.9.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.woff`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Cantarell-Regular-webfont.eot` & `anitya-1.9.0/anitya/static/css/fonts/Cantarell-Regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Cantarell-Regular-webfont.svg` & `anitya-1.9.0/anitya/static/css/fonts/Cantarell-Regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Cantarell-Regular-webfont.ttf` & `anitya-1.9.0/anitya/static/css/fonts/Cantarell-Regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Cantarell-Regular-webfont.woff` & `anitya-1.9.0/anitya/static/css/fonts/Cantarell-Regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Bold-webfont.eot` & `anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.eot`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Bold-webfont.svg` & `anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.svg`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Bold-webfont.ttf` & `anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Bold-webfont.woff` & `anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Regular-webfont.eot` & `anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Regular-webfont.svg` & `anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Regular-webfont.ttf` & `anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Regular-webfont.woff` & `anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Thin-webfont.eot` & `anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.eot`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Thin-webfont.svg` & `anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.svg`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Thin-webfont.ttf` & `anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.ttf`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/fonts/Comfortaa_Thin-webfont.woff` & `anitya-1.9.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.woff`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/images/ui-icons_0073ea_256x240.png` & `anitya-1.9.0/anitya/static/css/images/ui-icons_0073ea_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/images/ui-icons_454545_256x240.png` & `anitya-1.9.0/anitya/static/css/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/images/ui-icons_666666_256x240.png` & `anitya-1.9.0/anitya/static/css/images/ui-icons_666666_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/images/ui-icons_ff0084_256x240.png` & `anitya-1.9.0/anitya/static/css/images/ui-icons_ff0084_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/images/ui-icons_ffffff_256x240.png` & `anitya-1.9.0/anitya/static/css/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/css/text.css` & `anitya-1.9.0/anitya/static/css/text.css`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/google_logo.png` & `anitya-1.9.0/anitya/static/google_logo.png`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/ico/favicon.ico` & `anitya-1.9.0/anitya/static/ico/favicon.ico`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/img/spinner.gif` & `anitya-1.9.0/anitya/static/img/spinner.gif`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/node_modules/.package-lock.json` & `anitya-1.9.0/anitya/static/package-lock.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7361111111111112%*

 * *Differences: {"'dependencies'": "OrderedDict([('@popperjs/core', OrderedDict([('version', '2.11.6'), "*

 * *                   "('resolved', 'https://registry.npmjs.org/@popperjs/core/-/core-2.11.6.tgz'), "*

 * *                   "('integrity', "*

 * *                   "'sha512-50/17A98tWUfQ176raKiOGXuYpLyyVMkxxG6oylzL3BPOlA6ADGdK7EYunSa4I064xerltq9TGXs8HmOk5E+vw==')])), "*

 * *                   "('bootstrap', OrderedDict([('version', '5.2.2'), ('resolved', "*

 * *                   "'https://registry.npmjs.org/bootstrap/-/bootstrap-5.2.2.tg […]*

```diff
@@ -1,11 +1,54 @@
 {
-    "lockfileVersion": 3,
+    "dependencies": {
+        "@popperjs/core": {
+            "integrity": "sha512-50/17A98tWUfQ176raKiOGXuYpLyyVMkxxG6oylzL3BPOlA6ADGdK7EYunSa4I064xerltq9TGXs8HmOk5E+vw==",
+            "resolved": "https://registry.npmjs.org/@popperjs/core/-/core-2.11.6.tgz",
+            "version": "2.11.6"
+        },
+        "bootstrap": {
+            "integrity": "sha512-dEtzMTV71n6Fhmbg4fYJzQsw1N29hJKO1js5ackCgIpDcGid2ETMGC6zwSYw09v05Y+oRdQ9loC54zB1La3hHQ==",
+            "requires": {},
+            "resolved": "https://registry.npmjs.org/bootstrap/-/bootstrap-5.2.2.tgz",
+            "version": "5.2.2"
+        },
+        "jquery": {
+            "integrity": "sha512-opJeO4nCucVnsjiXOE+/PcCgYw9Gwpvs/a6B1LL/lQhwWwpbVEVYDZ1FokFr8PRc7ghYlrFPuyHuiiDNTQxmcw==",
+            "resolved": "https://registry.npmjs.org/jquery/-/jquery-3.6.1.tgz",
+            "version": "3.6.1"
+        },
+        "jquery-ui": {
+            "integrity": "sha512-wBZPnqWs5GaYJmo1Jj0k/mrSkzdQzKDwhXNtHKcBdAcKVxMM3KNYFq+iJ2i1rwiG53Z8M4mTn3Qxrm17uH1D4Q==",
+            "requires": {
+                "jquery": ">=1.8.0 <4.0.0"
+            },
+            "resolved": "https://registry.npmjs.org/jquery-ui/-/jquery-ui-1.13.2.tgz",
+            "version": "1.13.2"
+        },
+        "moment": {
+            "integrity": "sha512-5LC9SOxjSc2HF6vO2CyuTDNivEdoz2IvyJJGj6X8DJ0eFyfszE0QiEd+iXmBvUP3WHxSjFH/vIsA0EN00cgr8w==",
+            "resolved": "https://registry.npmjs.org/moment/-/moment-2.29.4.tgz",
+            "version": "2.29.4"
+        }
+    },
+    "lockfileVersion": 2,
     "name": "anitya",
     "packages": {
+        "": {
+            "dependencies": {
+                "@popperjs/core": "^2.11.6",
+                "bootstrap": "^5.2.2",
+                "jquery": "^3.6.1",
+                "jquery-ui": "^1.13.2",
+                "moment": "^2.29.4"
+            },
+            "license": "ISC",
+            "name": "anitya",
+            "version": "1.0.0"
+        },
         "node_modules/@popperjs/core": {
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/popperjs"
             },
             "integrity": "sha512-50/17A98tWUfQ176raKiOGXuYpLyyVMkxxG6oylzL3BPOlA6ADGdK7EYunSa4I064xerltq9TGXs8HmOk5E+vw==",
             "resolved": "https://registry.npmjs.org/@popperjs/core/-/core-2.11.6.tgz",
```

### Comparing `anitya-1.8.1/anitya/static/package.json` & `anitya-1.9.0/anitya/static/package.json`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/static/yahoo_logo.png` & `anitya-1.9.0/anitya/static/yahoo_logo.png`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/distro_add_edit.html` & `anitya-1.9.0/anitya/templates/distro_add_edit.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/distro_delete.html` & `anitya-1.9.0/anitya/templates/distro_delete.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/distros.html` & `anitya-1.9.0/anitya/templates/distros.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/flags.html` & `anitya-1.9.0/anitya/templates/flags.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/index.html` & `anitya-1.9.0/anitya/templates/index.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/login.html` & `anitya-1.9.0/anitya/templates/login.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/logs.html` & `anitya-1.9.0/anitya/templates/logs.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/mapping.html` & `anitya-1.9.0/anitya/templates/mapping.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/master.html` & `anitya-1.9.0/anitya/templates/master.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/project.html` & `anitya-1.9.0/anitya/templates/project.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/project_archive.html` & `anitya-1.9.0/anitya/templates/project_archive.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/project_delete.html` & `anitya-1.9.0/anitya/templates/project_delete.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/project_flag.html` & `anitya-1.9.0/anitya/templates/project_flag.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/project_new.html` & `anitya-1.9.0/anitya/templates/project_new.html`

 * *Files 1% similar despite different names*

```diff
@@ -248,14 +248,21 @@
     };
     if (str == 'GitLab'){
       $("label[for='version_url']").text('GitLab project url');
       $('#version_url_row').show();
       $("#version_url").prop('title', "This field should be filled when " +
       "homepage doesn't point to GitLab URL.");
     };
+    if (str == 'Gitea'){
+      $("label[for='version_url']").text('Gitea/Forgejo project url');
+      $('#version_url_row').show();
+      $("#version_url").prop('title', "This field should be filled when " +
+      "homepage doesn't point to Gitea or Forgejo URL.");
+      $('#releases_only_row').show();
+    };
     if (str == 'Gogs'){
       $("label[for='version_url']").text('Gogs project url');
       $('#version_url_row').show();
       $("#version_url").prop('title', "This field should be filled when " +
         "homepage doesn't point to Gogs URL.");
     };
     if (str == 'Cgit'){
```

### Comparing `anitya-1.8.1/anitya/templates/project_versions_delete.html` & `anitya-1.9.0/anitya/templates/project_versions_delete.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/projects.html` & `anitya-1.9.0/anitya/templates/projects.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/regex_delete.html` & `anitya-1.9.0/anitya/templates/regex_delete.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/search.html` & `anitya-1.9.0/anitya/templates/search.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/settings.html` & `anitya-1.9.0/anitya/templates/settings.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/updates.html` & `anitya-1.9.0/anitya/templates/updates.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/users.html` & `anitya-1.9.0/anitya/templates/users.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/templates/version_delete.html` & `anitya-1.9.0/anitya/templates/version_delete.html`

 * *Files identical despite different names*

### Comparing `anitya-1.8.1/anitya/ui.py` & `anitya-1.9.0/anitya/ui.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-
+"""UI"""
 from math import ceil
 
 import flask
 from flask_login import current_user, login_required, logout_user
 from sqlalchemy.exc import SQLAlchemyError
 
 import anitya
@@ -28,14 +28,15 @@
     if not pattern.endswith("*"):
         pattern += "*"
     return pattern
 
 
 @ui_blueprint.route("/")
 def index():
+    """index"""
     total = models.Project.all(Session, count=True)
     if current_user.is_authenticated and flask.session.get("next_url", ""):
         next_url = flask.session.get("next_url")
         del flask.session["next_url"]
         return flask.redirect(next_url)
     return flask.render_template("index.html", current="index", total=total)
 
@@ -46,26 +47,28 @@
     new_path = flask.url_for("anitya_ui.static", filename="docs/index.html")
     return flask.redirect(new_path)
 
 
 @ui_blueprint.route("/login/", methods=("GET", "POST"))
 @ui_blueprint.route("/login", methods=("GET", "POST"))
 def login():
+    """login"""
     next_url = flask.request.args.get("next", "/")
     if not next_url.startswith("/"):
         next_url = "/"
 
     flask.session["next_url"] = next_url
     return flask.render_template("login.html")
 
 
 @ui_blueprint.route("/logout/")
 @ui_blueprint.route("/logout")
 @login_required
 def logout():
+    """logout"""
     logout_user()
     return flask.redirect("/")
 
 
 @ui_blueprint.route("/settings/", methods=("GET", "POST"))
 @login_required
 def settings():
@@ -104,14 +107,15 @@
     else:
         flask.abort(400)
 
 
 @ui_blueprint.route("/project/<int:project_id>")
 @ui_blueprint.route("/project/<int:project_id>/")
 def project(project_id):
+    """project"""
     project = models.Project.by_id(Session, project_id)
 
     if not project:
         flask.abort(404)
 
     return flask.render_template(
         "project.html",
@@ -120,14 +124,15 @@
         links=anitya_config.get("DISTRO_MAPPING_LINKS", {}),
     )
 
 
 @ui_blueprint.route("/project/<project_name>")
 @ui_blueprint.route("/project/<project_name>/")
 def project_name(project_name):
+    """Project name"""
     page = flask.request.args.get("page", 1)
 
     try:
         page = int(page)
     except ValueError:
         page = 1
 
@@ -149,14 +154,15 @@
         page=page,
     )
 
 
 @ui_blueprint.route("/projects")
 @ui_blueprint.route("/projects/")
 def projects():
+    """Projects"""
     page = flask.request.args.get("page", 1)
 
     try:
         page = int(page)
     except ValueError:
         page = 1
 
@@ -175,29 +181,30 @@
     )
 
 
 @ui_blueprint.route("/projects/updates")
 @ui_blueprint.route("/projects/updates/")
 @ui_blueprint.route("/projects/updates/<status>")
 def projects_updated(status="updated"):
+    """Projects updated"""
     page = flask.request.args.get("page", 1)
     name = flask.request.args.get("name", None)
     log = flask.request.args.get("log", None)
 
     try:
         page = int(page)
     except ValueError:
         page = 1
 
     statuses = ["updated", "failed", "never_updated", "archived"]
 
     if status not in statuses:
         flask.flash(
-            "%s is invalid, you should use one of: %s; using default: "
-            "`updated`" % (status, ", ".join(statuses)),
+            f"{status} is invalid, you should use one of: "
+            f"{', '.join(statuses)}; using default: `updated`",
             "errors",
         )
         flask.flash(
             "Returning all the projects regardless of how/if their version "
             "was retrieved correctly"
         )
 
@@ -222,24 +229,24 @@
         log=log,
     )
 
 
 @ui_blueprint.route("/logs")
 @login_required
 def browse_logs():
+    """Browse logs"""
     refresh = flask.request.args.get("refresh", False)
     page = flask.request.args.get("page", 1)
 
     try:
         page = int(page)
     except ValueError:
         page = 1
 
-    if page < 1:
-        page = 1
+    page = max(page, 1)
 
     page_obj = models.Project.query.paginate(
         page=page, order_by=models.Project.last_check.desc()
     )
 
     projects = page_obj.items
 
@@ -256,14 +263,15 @@
         page=page,
     )
 
 
 @ui_blueprint.route("/distros")
 @ui_blueprint.route("/distros/")
 def distros():
+    """distros"""
     page = flask.request.args.get("page", 1)
 
     try:
         page = int(page)
     except ValueError:
         page = 1
 
@@ -281,14 +289,15 @@
         page=page,
     )
 
 
 @ui_blueprint.route("/distro/<distroname>")
 @ui_blueprint.route("/distro/<distroname>/")
 def distro(distroname):
+    """distro"""
     page = flask.request.args.get("page", 1)
 
     try:
         page = int(page)
     except ValueError:
         page = 1
 
@@ -307,14 +316,15 @@
         page=page,
     )
 
 
 @ui_blueprint.route("/distro/add", methods=["GET", "POST"])
 @login_required
 def add_distro():
+    """add distro"""
     form = anitya.forms.DistroForm()
 
     if form.validate_on_submit():
         name = form.name.data
 
         distro = models.Distro(name)
 
@@ -338,26 +348,27 @@
     )
 
 
 @ui_blueprint.route("/projects/search")
 @ui_blueprint.route("/projects/search/")
 @ui_blueprint.route("/projects/search/<pattern>")
 def projects_search(pattern=None):
+    """Search projects"""
     pattern = flask.request.args.get("pattern", pattern) or "*"
     page = flask.request.args.get("page", 1)
     exact = flask.request.args.get("exact", 0)
 
     try:
         page = int(page)
     except ValueError:
         page = 1
 
     projects = models.Project.search(Session, pattern=pattern, page=page)
 
-    if not str(exact).lower() in ["1", "true"]:
+    if str(exact).lower() not in ["1", "true"]:
         # Extends the search
         for proj in models.Project.search(
             Session, pattern=get_extended_pattern(pattern), page=page
         ):
             if proj not in projects:
                 projects.append(proj)
         projects_count = models.Project.search(
@@ -385,28 +396,29 @@
     )
 
 
 @ui_blueprint.route("/distro/<distroname>/search")
 @ui_blueprint.route("/distro/<distroname>/search/")
 @ui_blueprint.route("/distro/<distroname>/search/<pattern>")
 def distro_projects_search(distroname, pattern=None):
+    """Search distro projects"""
     pattern = flask.request.args.get("pattern", pattern) or "*"
     page = flask.request.args.get("page", 1)
     exact = flask.request.args.get("exact", 0)
 
     try:
         page = int(page)
     except ValueError:
         page = 1
 
     projects = models.Project.search(
         Session, pattern=pattern, distro=distroname, page=page
     )
 
-    if not str(exact).lower() in ["1", "true"]:
+    if str(exact).lower() not in ["1", "true"]:
         # Extends the search
         for proj in models.Project.search(
             Session, pattern=get_extended_pattern(pattern), distro=distroname, page=page
         ):
             if proj not in projects:
                 projects.append(proj)
         projects_count = models.Project.search(
@@ -483,26 +495,32 @@
         try:
             project = utilities.create_project(
                 Session,
                 name=form.name.data.strip(),
                 homepage=form.homepage.data.strip(),
                 backend=form.backend.data.strip(),
                 version_scheme=form.version_scheme.data.strip(),
-                version_url=form.version_url.data.strip()
-                if form.version_url.data
-                else None,
-                version_prefix=form.version_prefix.data.strip()
-                if form.version_prefix.data
-                else None,
-                pre_release_filter=form.pre_release_filter.data.strip()
-                if form.pre_release_filter.data
-                else None,
-                version_filter=form.version_filter.data.strip()
-                if form.version_filter.data
-                else None,
+                version_url=(
+                    form.version_url.data.strip() if form.version_url.data else None
+                ),
+                version_prefix=(
+                    form.version_prefix.data.strip()
+                    if form.version_prefix.data
+                    else None
+                ),
+                pre_release_filter=(
+                    form.pre_release_filter.data.strip()
+                    if form.pre_release_filter.data
+                    else None
+                ),
+                version_filter=(
+                    form.version_filter.data.strip()
+                    if form.version_filter.data
+                    else None
+                ),
                 regex=form.regex.data.strip() if form.regex.data else None,
                 user_id=flask.g.user.username,
                 releases_only=form.releases_only.data,
             )
             Session.commit()
 
             # Optionally, the user can also map a distro when creating a proj.
@@ -549,14 +567,15 @@
         400,
     )
 
 
 @ui_blueprint.route("/project/<project_id>/edit", methods=["GET", "POST"])
 @login_required
 def edit_project(project_id):
+    """Edit project"""
     project = models.Project.get(Session, project_id)
     if not project:
         flask.abort(404)
 
     # Archived project is not editable
     if project.archived:
         flask.abort(404)
@@ -574,32 +593,42 @@
         try:
             changes = utilities.edit_project(
                 Session,
                 project=project,
                 name=form.name.data.strip(),
                 homepage=form.homepage.data.strip(),
                 backend=form.backend.data.strip(),
-                version_scheme=form.version_scheme.data.strip()
-                if form.version_scheme.data
-                else None,
-                version_pattern=form.version_pattern.data.strip()
-                if form.version_pattern.data
-                else None,
-                version_url=form.version_url.data.strip()
-                if form.version_url.data
-                else None,
-                version_prefix=form.version_prefix.data.strip()
-                if form.version_prefix.data
-                else None,
-                pre_release_filter=form.pre_release_filter.data.strip()
-                if form.pre_release_filter.data
-                else None,
-                version_filter=form.version_filter.data.strip()
-                if form.version_filter.data
-                else None,
+                version_scheme=(
+                    form.version_scheme.data.strip()
+                    if form.version_scheme.data
+                    else None
+                ),
+                version_pattern=(
+                    form.version_pattern.data.strip()
+                    if form.version_pattern.data
+                    else None
+                ),
+                version_url=(
+                    form.version_url.data.strip() if form.version_url.data else None
+                ),
+                version_prefix=(
+                    form.version_prefix.data.strip()
+                    if form.version_prefix.data
+                    else None
+                ),
+                pre_release_filter=(
+                    form.pre_release_filter.data.strip()
+                    if form.pre_release_filter.data
+                    else None
+                ),
+                version_filter=(
+                    form.version_filter.data.strip()
+                    if form.version_filter.data
+                    else None
+                ),
                 regex=form.regex.data.strip() if form.regex.data else None,
                 insecure=form.insecure.data,
                 user_id=flask.g.user.username,
                 check_release=form.check_release.data,
                 releases_only=form.releases_only.data,
             )
             if changes:
@@ -621,14 +650,15 @@
         plugins=backend_plugins,
     )
 
 
 @ui_blueprint.route("/project/<project_id>/flag", methods=["GET", "POST"])
 @login_required
 def flag_project(project_id):
+    """Flag project"""
     project = models.Project.get(Session, project_id)
     if not project:
         flask.abort(404)
 
     form = anitya.forms.FlagProjectForm(obj=project)
 
     if form.validate_on_submit():
@@ -654,14 +684,15 @@
         project=project,
     )
 
 
 @ui_blueprint.route("/project/<project_id>/map", methods=["GET", "POST"])
 @login_required
 def map_project(project_id):
+    """Map project"""
     project = models.Project.get(Session, project_id)
     if not project:
         flask.abort(404)
 
     # Get all available distros name
     distros = models.Distro.all(Session)
     distro_names = []
@@ -697,14 +728,15 @@
         "mapping.html", current="projects", project=project, form=form
     )
 
 
 @ui_blueprint.route("/project/<project_id>/map/<pkg_id>", methods=["GET", "POST"])
 @login_required
 def edit_project_mapping(project_id, pkg_id):
+    """Edit project mapping"""
     project = models.Project.get(Session, project_id)
     if not project:
         flask.abort(404)
 
     package = models.Packages.by_id(Session, pkg_id)
     if not package:
         flask.abort(404)
@@ -751,15 +783,15 @@
 def format_examples(examples):
     """Return the plugins examples as HTML links."""
     output = ""
     if examples:
         for cnt, example in enumerate(examples):
             if cnt > 0:
                 output += " <br /> "
-            output += "<a href='%(url)s'>%(url)s</a> " % ({"url": example})
+            output += f"<a href='{example}'>{example}</a> "
 
     return output
 
 
 def context_class(category):
     """Return bootstrap context class for a given category."""
     values = {"message": "default", "error": "danger", "info": "info"}
```

### Comparing `anitya-1.8.1/anitya/wsgi.py` & `anitya-1.9.0/anitya/wsgi.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,10 +10,11 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
+"""wsgi"""
 from .app import create
 
 application = create()
```

### Comparing `anitya-1.8.1/createdb.py` & `anitya-1.9.0/createdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-
+"""createdb"""
 import os
 from argparse import ArgumentParser
 from pathlib import Path
 
 from alembic import command
 from alembic.config import Config
 from social_flask_sqlalchemy import models as social_models
@@ -48,13 +48,13 @@
 # Set the alembic_version based on the current migrations available.
 # This presupposes the models haven't changed outside of a migration.
 #
 # Default to the side-by-side alembic.ini.
 if alembic_config is None:
     alembic_config = os.path.join(script_dir, "alembic.ini")
     if args.verbose and os.path.isfile(alembic_config):
-        print("No alembic config specified, defaulting to: {}".format(alembic_config))
+        print(f"No alembic config specified, defaulting to: {alembic_config}")
 
 if alembic_config and os.path.isfile(alembic_config):
     alembic_cfg = Config(alembic_config)
     alembic_cfg.set_main_option("sqlalchemy.url", anitya_config["DB_URL"])
     command.stamp(alembic_cfg, "head")
```

### Comparing `anitya-1.8.1/files/anitya.toml.sample` & `anitya-1.9.0/files/anitya.toml.sample`

 * *Files 12% similar despite different names*

```diff
@@ -42,21 +42,14 @@
     "social_core.backends.yahoo.YahooOAuth2",
     "social_core.backends.open_id.OpenIdAuth"
 ]
 
 # Force the application to require HTTPS on authentication redirects.
 social_auth_redirect_is_https = true
 
-# List of platforms for which Anitya should automatically create new projects
-# when Libraries.io announces a new version. See https://libraries.io/ for the
-# list of valid platforms. By default, Anitya will only update existing projects
-# via Libraries.io.
-librariesio_platform_whitelist = []
-sse_feed = "http://firehose.libraries.io/events"
-
 # Default regular expression used for custom backend
 default_regex = """\
                 (?i)%(name)s(?:[-_]?(?:minsrc|src|source))?[-_](+[^-/_\\s]+?(?:[-_]\
                 (?:rc|devel|dev|alpha|beta)\\d+)?)(?:[-_](?:minsrc|src|source|asc|release))?\
                 \.(?:tar|t[bglx]z|tbz2|zip)\
                 """
```

### Comparing `anitya-1.8.1/pyproject.toml` & `anitya-1.9.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 '''
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "anitya"
-version = "1.8.1"
+version = "1.9.0"
 description = "A cross-distribution upstream release monitoring project"
 authors = ["Pierre-Yves Chibon <pingou@pingoured.fr>"]
 maintainers = ["Michal Konecny <mkonecny@redhat.com>"]
 readme = "README.rst"
 homepage = "https://release-monitoring.org"
 documentation = "https://anitya.readthedocs.io"
 repository = "https://github.com/fedora-infra/anitya"
@@ -87,54 +87,52 @@
   "files/anitya.toml.sample", "files/config.toml.sample",
   "anitya/static/docs/**/*", "anitya/static/node_modules/**/*"
 ]
 
 [tool.poetry.scripts]
 check_service = "anitya.check_service:main"
 sar = "anitya.sar:main"
-librariesio_consumer = "anitya.librariesio_consumer:main"
 
 [tool.poetry.dependencies]
-python = "^3.8.1"
+python = "^3.8.10"
 alembic = "^1.8.1"
 anitya-schema = "^2.0.1"
 arrow = "^1.2.3"
 beautifulsoup4 = "^4.11.1"
 defusedxml = "^0.7.1"
 fedora-messaging = "^3.1.0"
-Flask = "^2.1.2"
-Flask-Login = "^0.6.2"
-Flask-WTF = "^1.0.1"
+Flask = "^3.0.0"
+Flask-Login = "^0.6.3"
+Flask-WTF = "^1.2.1"
 # https://github.com/sphinx-doc/sphinx/issues/10306
-Jinja2 = "<3.1.3"
+Jinja2 = "<3.1.4"
 ordered-set = "^4.1.0"
 packaging = "^23.0"
 python-dateutil = "^2.8.2"
 semver = "^3.0.0"
 social-auth-app-flask = "^1.0.0"
 social-auth-app-flask-sqlalchemy = "^1.0.1"
 SQLAlchemy = "^1.4.41"
-sseclient = "^0.0.27"
 # Limit the package till https://github.com/maxcountryman/flask-login/issues/686 is fixed
-Werkzeug = "2.3.4"
+Werkzeug = "3.0.1"
 "straight.plugin" = "^1.5.0"
 toml = "^0.10.2"
 webargs = "^8.2.0"
 WTForms = "^3.0.1"
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.4"
-black = "^23.0.0"
+black = "^24.0.0"
 coverage = "^7.0.0"
-diff-cover = "^7.0.1"
-flake8 = "^6.0.0"
+diff-cover = "^8.0.0"
+flake8 = "^7.0.0"
 mock = "^5.0.0"
-pytest = "^7.1.3"
+pytest = "^8.0.0"
 pytest-cov = "^4.0.0"
-vcrpy = "^4.2.1"
+vcrpy = "^6.0.0"
 psycopg2-binary = "^2.9.3"
 
 # Authentication integration testing
 requests = "^2.31.0"
 requests-oauthlib = "^1.3.1"
 
 # Required to test building the docs
@@ -149,22 +147,42 @@
 types-requests = "^2.28.11"
 types-setuptools = "^65.3.0"
 types-six = "^1.16.19"
 types-toml = "^0.10.8"
 
 [tool.poetry.group.dev.dependencies]
 tox = "^4.5.1"
-towncrier = "^22.12.0"
+towncrier = "^23.0.0"
+pre-commit = "^3.3.3"
+pylint = "^3.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pylint]
 disable = [
-  "no-member",
+  "attribute-defined-outside-init",
   "broad-exception-caught",
+  "cyclic-import",
+  "duplicate-code",
+  "inconsistent-return-statements",
+  "invalid-name",
   "no-else-return",
-  "use-dict-literal",
+  "no-member",
+  "redefined-outer-name",
+  "too-few-public-methods",
+  "too-many-ancestors",
+  "too-many-arguments",
   "too-many-branches",
-  "too-many-statements"
+  "too-many-instance-attributes",
+  "too-many-lines",
+  "too-many-locals",
+  "too-many-public-methods",
+  "too-many-return-statements",
+  "too-many-statements",
+  "unnecessary-dunder-call",
+  "unnecessary-pass",
+  "unused-argument",
+  "use-dict-literal",
+  "useless-object-inheritance"
 ]
```

### Comparing `anitya-1.8.1/PKG-INFO` & `anitya-1.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 Metadata-Version: 2.1
 Name: anitya
-Version: 1.8.1
+Version: 1.9.0
 Summary: A cross-distribution upstream release monitoring project
 Home-page: https://release-monitoring.org
 License: GPL-2.0-or-later
 Author: Pierre-Yves Chibon
 Author-email: pingou@pingoured.fr
 Maintainer: Michal Konecny
 Maintainer-email: mkonecny@redhat.com
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.8.10,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: Flask (>=2.1.2,<3.0.0)
-Requires-Dist: Flask-Login (>=0.6.2,<0.7.0)
-Requires-Dist: Flask-WTF (>=1.0.1,<2.0.0)
-Requires-Dist: Jinja2 (<3.1.3)
+Requires-Dist: Flask (>=3.0.0,<4.0.0)
+Requires-Dist: Flask-Login (>=0.6.3,<0.7.0)
+Requires-Dist: Flask-WTF (>=1.2.1,<2.0.0)
+Requires-Dist: Jinja2 (<3.1.4)
 Requires-Dist: SQLAlchemy (>=1.4.41,<2.0.0)
 Requires-Dist: WTForms (>=3.0.1,<4.0.0)
-Requires-Dist: Werkzeug (==2.3.4)
+Requires-Dist: Werkzeug (==3.0.1)
 Requires-Dist: alembic (>=1.8.1,<2.0.0)
 Requires-Dist: anitya-schema (>=2.0.1,<3.0.0)
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: fedora-messaging (>=3.1.0,<4.0.0)
 Requires-Dist: ordered-set (>=4.1.0,<5.0.0)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: semver (>=3.0.0,<4.0.0)
 Requires-Dist: social-auth-app-flask (>=1.0.0,<2.0.0)
 Requires-Dist: social-auth-app-flask-sqlalchemy (>=1.0.1,<2.0.0)
-Requires-Dist: sseclient (>=0.0.27,<0.0.28)
 Requires-Dist: straight.plugin (>=1.5.0,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: webargs (>=8.2.0,<9.0.0)
 Project-URL: Documentation, https://anitya.readthedocs.io
 Project-URL: Repository, https://github.com/fedora-infra/anitya
 Description-Content-Type: text/x-rst
 
@@ -55,22 +54,16 @@
 .. image:: https://readthedocs.org/projects/anitya/badge/?version=latest
   :alt: Documentation Status
   :target: https://anitya.readthedocs.io/en/latest/?badge=latest
   
 .. image:: https://img.shields.io/badge/renovate-enabled-brightgreen.svg
   :target: https://renovatebot.com/
 
-.. image:: https://img.shields.io/lgtm/alerts/g/fedora-infra/anitya.svg?logo=lgtm&logoWidth=18
-  :target: https://lgtm.com/projects/g/fedora-infra/anitya/alerts/
-
-.. image:: https://img.shields.io/lgtm/grade/javascript/g/fedora-infra/anitya.svg?logo=lgtm&logoWidth=18
-  :target: https://lgtm.com/projects/g/fedora-infra/anitya/context:javascript
-  
-.. image:: https://img.shields.io/lgtm/grade/python/g/fedora-infra/anitya.svg?logo=lgtm&logoWidth=18
-  :target: https://lgtm.com/projects/g/fedora-infra/anitya/context:python
+.. image::  https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
+  :target:  https://pre-commit.com/
   
 
 ======
 Anitya
 ======
 
 Anitya is a release monitoring project. It provides a user-friendly interface
```

