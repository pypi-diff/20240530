# Comparing `tmp/django_evolution-2.3.tar.gz` & `tmp/django_evolution-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_evolution-2.3.tar", last modified: Sun Oct 15 23:25:20 2023, max compression
+gzip compressed data, was "django_evolution-2.4.tar", last modified: Thu May 30 08:42:08 2024, max compression
```

## Comparing `django_evolution-2.3.tar` & `django_evolution-2.4.tar`

### file list

```diff
@@ -1,258 +1,259 @@
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.433072 django_evolution-2.3/
--rw-r--r--   0 chipx86    (501) staff       (20)     1230 2023-10-15 23:25:18.000000 django_evolution-2.3/AUTHORS
--rw-r--r--   0 chipx86    (501) staff       (20)     1573 2023-10-15 23:25:18.000000 django_evolution-2.3/LICENSE
--rw-r--r--   0 chipx86    (501) staff       (20)      313 2023-10-15 23:25:18.000000 django_evolution-2.3/MANIFEST.in
--rw-r--r--   0 chipx86    (501) staff       (20)      103 2023-10-15 23:25:18.000000 django_evolution-2.3/NEWS
--rw-r--r--   0 chipx86    (501) staff       (20)     5826 2023-10-15 23:25:20.433147 django_evolution-2.3/PKG-INFO
--rw-r--r--   0 chipx86    (501) staff       (20)     3563 2023-10-15 23:25:18.000000 django_evolution-2.3/README.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     5786 2023-10-15 23:25:18.000000 django_evolution-2.3/conftest.py
--rw-r--r--   0 chipx86    (501) staff       (20)      155 2023-10-15 23:25:18.000000 django_evolution-2.3/dev-requirements.txt
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.408443 django_evolution-2.3/django_evolution/
--rw-r--r--   0 chipx86    (501) staff       (20)     1256 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)      192 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/admin.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.410449 django_evolution-2.3/django_evolution/builtin_evolutions/
--rw-r--r--   0 chipx86    (501) staff       (20)     1724 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/builtin_evolutions/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)      218 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/builtin_evolutions/admin_move_to_migrations.py
--rw-r--r--   0 chipx86    (501) staff       (20)      137 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/builtin_evolutions/auth_delete_message.py
--rw-r--r--   0 chipx86    (501) staff       (20)      151 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/builtin_evolutions/auth_move_to_migrations.py
--rw-r--r--   0 chipx86    (501) staff       (20)      205 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/builtin_evolutions/auth_unique_together_baseline.py
--rw-r--r--   0 chipx86    (501) staff       (20)      225 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/builtin_evolutions/contenttypes_move_to_migrations.py
--rw-r--r--   0 chipx86    (501) staff       (20)      185 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/builtin_evolutions/contenttypes_unique_together_baseline.py
--rw-r--r--   0 chipx86    (501) staff       (20)      222 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/builtin_evolutions/flatpages_move_to_migrations.py
--rw-r--r--   0 chipx86    (501) staff       (20)      222 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/builtin_evolutions/redirects_move_to_migrations.py
--rw-r--r--   0 chipx86    (501) staff       (20)      181 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/builtin_evolutions/session_expire_date_db_index.py
--rw-r--r--   0 chipx86    (501) staff       (20)      151 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/builtin_evolutions/sessions_move_to_migrations.py
--rw-r--r--   0 chipx86    (501) staff       (20)      221 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/builtin_evolutions/sites_move_to_migrations.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.411835 django_evolution-2.3/django_evolution/compat/
--rw-r--r--   0 chipx86    (501) staff       (20)      209 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/compat/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     6122 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/compat/apps.py
--rw-r--r--   0 chipx86    (501) staff       (20)     5909 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/compat/commands.py
--rw-r--r--   0 chipx86    (501) staff       (20)      431 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/compat/datastructures.py
--rw-r--r--   0 chipx86    (501) staff       (20)    31895 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/compat/db.py
--rw-r--r--   0 chipx86    (501) staff       (20)     9727 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/compat/models.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.412543 django_evolution-2.3/django_evolution/compat/patches/
--rw-r--r--   0 chipx86    (501) staff       (20)     1482 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/compat/patches/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1963 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/compat/patches/django1_8__1_10_mysql_preserve_db_index.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1937 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/compat/patches/django2_0_quote_unique_index_name.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1761 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/compat/patches/mysqlclient_django_pre_2_encoder_bytes.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1443 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/compat/patches/python3_10_collection_imports.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1411 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/compat/patches/sqlite_legacy_alter_table.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2234 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/compat/picklers.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1420 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/compat/py23.py
--rw-r--r--   0 chipx86    (501) staff       (20)    34549 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/compat/six.py
--rw-r--r--   0 chipx86    (501) staff       (20)      516 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/compat/translation.py
--rw-r--r--   0 chipx86    (501) staff       (20)     5100 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/conf.py
--rw-r--r--   0 chipx86    (501) staff       (20)      655 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/consts.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.413636 django_evolution-2.3/django_evolution/db/
--rw-r--r--   0 chipx86    (501) staff       (20)     1452 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/db/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)    79897 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/db/common.py
--rw-r--r--   0 chipx86    (501) staff       (20)    11133 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/db/mysql.py
--rw-r--r--   0 chipx86    (501) staff       (20)      143 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/db/mysql_old.py
--rw-r--r--   0 chipx86    (501) staff       (20)    13363 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/db/postgresql.py
--rw-r--r--   0 chipx86    (501) staff       (20)      145 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/db/postgresql_psycopg2.py
--rw-r--r--   0 chipx86    (501) staff       (20)    10473 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/db/sql_result.py
--rw-r--r--   0 chipx86    (501) staff       (20)    35114 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/db/sqlite3.py
--rw-r--r--   0 chipx86    (501) staff       (20)    13058 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/db/state.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2288 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/deprecation.py
--rw-r--r--   0 chipx86    (501) staff       (20)    16065 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/diff.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4407 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/errors.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.413843 django_evolution-2.3/django_evolution/evolutions/
--rw-r--r--   0 chipx86    (501) staff       (20)       56 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/evolutions/__init__.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.414601 django_evolution-2.3/django_evolution/evolve/
--rw-r--r--   0 chipx86    (501) staff       (20)      919 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/evolve/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     7123 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/evolve/base.py
--rw-r--r--   0 chipx86    (501) staff       (20)    61328 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/evolve/evolve_app_task.py
--rw-r--r--   0 chipx86    (501) staff       (20)    19887 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/evolve/evolver.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3297 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/evolve/purge_app_task.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.414718 django_evolution-2.3/django_evolution/management/
--rw-r--r--   0 chipx86    (501) staff       (20)     4574 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/management/__init__.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.415703 django_evolution-2.3/django_evolution/management/commands/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/management/commands/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     8921 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/management/commands/evolution-project-sig.py
--rw-r--r--   0 chipx86    (501) staff       (20)    24461 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/management/commands/evolve.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1249 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/management/commands/list-evolutions.py
--rw-r--r--   0 chipx86    (501) staff       (20)     5449 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/management/commands/mark-evolution-applied.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3265 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/management/commands/migrate.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2231 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/management/commands/syncdb.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3330 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/management/commands/wipe-evolution.py
--rw-r--r--   0 chipx86    (501) staff       (20)    19044 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/mock_models.py
--rw-r--r--   0 chipx86    (501) staff       (20)     8738 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/models.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.417166 django_evolution-2.3/django_evolution/mutations/
--rw-r--r--   0 chipx86    (501) staff       (20)     2725 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/mutations/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     7279 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/mutations/add_field.py
--rw-r--r--   0 chipx86    (501) staff       (20)    19564 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/mutations/base.py
--rw-r--r--   0 chipx86    (501) staff       (20)     9774 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/mutations/change_field.py
--rw-r--r--   0 chipx86    (501) staff       (20)     5868 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/mutations/change_meta.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3438 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/mutations/delete_application.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3722 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/mutations/delete_field.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2532 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/mutations/delete_model.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3704 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/mutations/move_to_django_migrations.py
--rw-r--r--   0 chipx86    (501) staff       (20)     5138 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/mutations/rename_app_label.py
--rw-r--r--   0 chipx86    (501) staff       (20)     6444 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/mutations/rename_field.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4134 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/mutations/rename_model.py
--rw-r--r--   0 chipx86    (501) staff       (20)     5192 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/mutations/sql_mutation.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.417859 django_evolution-2.3/django_evolution/mutators/
--rw-r--r--   0 chipx86    (501) staff       (20)      790 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/mutators/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)    40252 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/mutators/app_mutator.py
--rw-r--r--   0 chipx86    (501) staff       (20)     5113 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/mutators/base.py
--rw-r--r--   0 chipx86    (501) staff       (20)    11738 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/mutators/model_mutator.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1492 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/mutators/sql_mutator.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1517 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/mutators/upgrade_method_mutator.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2960 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/placeholders.py
--rw-r--r--   0 chipx86    (501) staff       (20)    30164 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/serialization.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2673 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/signals.py
--rw-r--r--   0 chipx86    (501) staff       (20)    87714 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/signature.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2292 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/support.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.422355 django_evolution-2.3/django_evolution/tests/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/__init__.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.422578 django_evolution-2.3/django_evolution/tests/app_deps_app/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/app_deps_app/__init__.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.422798 django_evolution-2.3/django_evolution/tests/app_deps_app/evolutions/
--rw-r--r--   0 chipx86    (501) staff       (20)      393 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/app_deps_app/evolutions/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)       57 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/app_deps_app/evolutions/test_evolution.py
--rw-r--r--   0 chipx86    (501) staff       (20)       38 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/app_deps_app/models.py
--rw-r--r--   0 chipx86    (501) staff       (20)    43129 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/base_test_case.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.423378 django_evolution-2.3/django_evolution/tests/db/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/db/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)    80400 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/db/mysql.py
--rw-r--r--   0 chipx86    (501) staff       (20)    94924 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/db/postgresql.py
--rw-r--r--   0 chipx86    (501) staff       (20)   144109 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/db/sqlite3.py
--rw-r--r--   0 chipx86    (501) staff       (20)     9108 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/decorators.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.423645 django_evolution-2.3/django_evolution/tests/evolution_deps_app/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/evolution_deps_app/__init__.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.423987 django_evolution-2.3/django_evolution/tests/evolution_deps_app/evolutions/
--rw-r--r--   0 chipx86    (501) staff       (20)       79 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/evolution_deps_app/evolutions/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)      371 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/evolution_deps_app/evolutions/test_evolution.py
--rw-r--r--   0 chipx86    (501) staff       (20)       38 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/evolution_deps_app/models.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.424193 django_evolution-2.3/django_evolution/tests/evolutions_app/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/evolutions_app/__init__.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.424530 django_evolution-2.3/django_evolution/tests/evolutions_app/evolutions/
--rw-r--r--   0 chipx86    (501) staff       (20)       62 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/evolutions_app/evolutions/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)      238 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/evolutions_app/evolutions/first_evolution.py
--rw-r--r--   0 chipx86    (501) staff       (20)      309 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/evolutions_app/evolutions/second_evolution.py
--rw-r--r--   0 chipx86    (501) staff       (20)      237 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/evolutions_app/models.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.424736 django_evolution-2.3/django_evolution/tests/evolutions_app2/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/evolutions_app2/__init__.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.424959 django_evolution-2.3/django_evolution/tests/evolutions_app2/evolutions/
--rw-r--r--   0 chipx86    (501) staff       (20)       79 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/evolutions_app2/evolutions/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)      451 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/evolutions_app2/evolutions/test_evolution.py
--rw-r--r--   0 chipx86    (501) staff       (20)      641 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/evolutions_app2/models.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.425158 django_evolution-2.3/django_evolution/tests/migrations_app/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/migrations_app/__init__.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.425499 django_evolution-2.3/django_evolution/tests/migrations_app/migrations/
--rw-r--r--   0 chipx86    (501) staff       (20)      870 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/migrations_app/migrations/0001_initial.py
--rw-r--r--   0 chipx86    (501) staff       (20)      527 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/migrations_app/migrations/0002_add_field.py
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/migrations_app/migrations/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)      215 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/migrations_app/models.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.425689 django_evolution-2.3/django_evolution/tests/migrations_app2/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/migrations_app2/__init__.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.426028 django_evolution-2.3/django_evolution/tests/migrations_app2/migrations/
--rw-r--r--   0 chipx86    (501) staff       (20)      960 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/migrations_app2/migrations/0001_initial.py
--rw-r--r--   0 chipx86    (501) staff       (20)      532 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/migrations_app2/migrations/0002_add_field.py
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/migrations_app2/migrations/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)      220 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/migrations_app2/models.py
--rw-r--r--   0 chipx86    (501) staff       (20)      633 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/models.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.426120 django_evolution-2.3/django_evolution/tests/no_models_app/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/no_models_app/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)    28908 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_add_field.py
--rw-r--r--   0 chipx86    (501) staff       (20)    92718 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_change_field.py
--rw-r--r--   0 chipx86    (501) staff       (20)    59809 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_change_meta.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1985 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_compat_apps.py
--rw-r--r--   0 chipx86    (501) staff       (20)    10933 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_compat_models.py
--rw-r--r--   0 chipx86    (501) staff       (20)     6448 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_conf.py
--rw-r--r--   0 chipx86    (501) staff       (20)    17373 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_database_state.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4361 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_datastructures_utils.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4344 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_delete_app.py
--rw-r--r--   0 chipx86    (501) staff       (20)    12099 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_delete_field.py
--rw-r--r--   0 chipx86    (501) staff       (20)     6463 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_delete_model.py
--rw-r--r--   0 chipx86    (501) staff       (20)     7042 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_dependency_graph.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1852 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_diff.py
--rw-r--r--   0 chipx86    (501) staff       (20)    24833 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_evolution_graph.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3613 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_evolution_models.py
--rw-r--r--   0 chipx86    (501) staff       (20)    26239 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_evolution_utils.py
--rw-r--r--   0 chipx86    (501) staff       (20)    81787 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_evolver.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2782 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_generics.py
--rw-r--r--   0 chipx86    (501) staff       (20)    35829 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_migration_utils.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2675 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_model_mutator.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1218 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_move_to_django_migrations.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1698 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_ordering.py
--rw-r--r--   0 chipx86    (501) staff       (20)    26964 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_preprocessing.py
--rw-r--r--   0 chipx86    (501) staff       (20)    20793 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_rename_field.py
--rw-r--r--   0 chipx86    (501) staff       (20)     9796 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_rename_model.py
--rw-r--r--   0 chipx86    (501) staff       (20)    21712 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_serialization.py
--rw-r--r--   0 chipx86    (501) staff       (20)   110925 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_signature.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4190 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_sql_mutation.py
--rw-r--r--   0 chipx86    (501) staff       (20)     7418 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/test_utils_models.py
--rw-r--r--   0 chipx86    (501) staff       (20)    33974 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/tests/utils.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.427022 django_evolution-2.3/django_evolution/utils/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/utils/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2759 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/utils/apps.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2717 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/utils/datastructures.py
--rw-r--r--   0 chipx86    (501) staff       (20)    24033 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/utils/evolutions.py
--rw-r--r--   0 chipx86    (501) staff       (20)    27336 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/utils/graph.py
--rw-r--r--   0 chipx86    (501) staff       (20)    35220 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/utils/migrations.py
--rw-r--r--   0 chipx86    (501) staff       (20)     9421 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/utils/models.py
--rw-r--r--   0 chipx86    (501) staff       (20)    12509 2023-10-15 23:25:18.000000 django_evolution-2.3/django_evolution/utils/sql.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.408990 django_evolution-2.3/django_evolution.egg-info/
--rw-r--r--   0 chipx86    (501) staff       (20)     5826 2023-10-15 23:25:20.000000 django_evolution-2.3/django_evolution.egg-info/PKG-INFO
--rw-r--r--   0 chipx86    (501) staff       (20)     8850 2023-10-15 23:25:20.000000 django_evolution-2.3/django_evolution.egg-info/SOURCES.txt
--rw-r--r--   0 chipx86    (501) staff       (20)        1 2023-10-15 23:25:20.000000 django_evolution-2.3/django_evolution.egg-info/dependency_links.txt
--rw-r--r--   0 chipx86    (501) staff       (20)       65 2023-10-15 23:25:20.000000 django_evolution-2.3/django_evolution.egg-info/requires.txt
--rw-r--r--   0 chipx86    (501) staff       (20)       17 2023-10-15 23:25:20.000000 django_evolution-2.3/django_evolution.egg-info/top_level.txt
--rw-r--r--   0 chipx86    (501) staff       (20)      215 2023-10-15 23:25:18.000000 django_evolution-2.3/doc-requirements.txt
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.428198 django_evolution-2.3/docs/
--rw-r--r--   0 chipx86    (501) staff       (20)      700 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/Makefile
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.428325 django_evolution-2.3/docs/coderef/
--rw-r--r--   0 chipx86    (501) staff       (20)     2460 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/coderef/index.rst
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.428983 django_evolution-2.3/docs/commands/
--rw-r--r--   0 chipx86    (501) staff       (20)     1487 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/commands/evolution-project-sig.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     3427 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/commands/evolve.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      204 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/commands/index.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      648 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/commands/list-evolutions.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     1162 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/commands/mark-evolution-applied.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     1257 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/commands/wipe-evolution.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     6448 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/conf.py
--rw-r--r--   0 chipx86    (501) staff       (20)     6241 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/faq.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     1281 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/glossary.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     1531 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/how-does-it-work.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     3046 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/index.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      321 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/installation.rst
--rw-r--r--   0 chipx86    (501) staff       (20)    15172 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/mutations.rst
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.432842 django_evolution-2.3/docs/releasenotes/
--rw-r--r--   0 chipx86    (501) staff       (20)     1306 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.5.1.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      121 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.5.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      245 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.6.1.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      569 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.6.2.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     1203 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.6.3.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     1257 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.6.4.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     1007 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.6.5.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     1074 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.6.6.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      479 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.6.7.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      760 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.6.8.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      695 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.6.9.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      532 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.6.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     3334 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.7-beta-1.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      468 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.7.1.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      428 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.7.2.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      770 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.7.3.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      592 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.7.4.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      984 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.7.5.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     1188 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.7.6.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     1767 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.7.7.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      680 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.7.8.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     3321 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/0.7.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     7179 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/2.0.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      536 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/2.1.1.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      348 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/2.1.2.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     1859 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/2.1.3.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      316 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/2.1.4.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     2046 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/2.1.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     2154 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/2.2.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     1692 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/2.3.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      558 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/releasenotes/index.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      578 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/versioning.rst
--rw-r--r--   0 chipx86    (501) staff       (20)     8969 2023-10-15 23:25:18.000000 django_evolution-2.3/docs/writing-evolutions.rst
--rw-r--r--   0 chipx86    (501) staff       (20)      268 2023-10-15 23:25:20.433538 django_evolution-2.3/setup.cfg
--rwxr-xr-x   0 chipx86    (501) staff       (20)     3024 2023-10-15 23:25:18.000000 django_evolution-2.3/setup.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-10-15 23:25:20.432959 django_evolution-2.3/tests/
--rw-r--r--   0 chipx86    (501) staff       (20)      986 2023-10-15 23:25:18.000000 django_evolution-2.3/tests/test_db_settings.py.tmpl
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.844727 django_evolution-2.4/
+-rw-r--r--   0 chipx86    (501) staff       (20)     1230 2024-05-30 08:42:07.000000 django_evolution-2.4/AUTHORS
+-rw-r--r--   0 chipx86    (501) staff       (20)     1573 2024-05-30 08:42:07.000000 django_evolution-2.4/LICENSE
+-rw-r--r--   0 chipx86    (501) staff       (20)      313 2024-05-30 08:42:07.000000 django_evolution-2.4/MANIFEST.in
+-rw-r--r--   0 chipx86    (501) staff       (20)      103 2024-05-30 08:42:07.000000 django_evolution-2.4/NEWS
+-rw-r--r--   0 chipx86    (501) staff       (20)     5826 2024-05-30 08:42:08.844813 django_evolution-2.4/PKG-INFO
+-rw-r--r--   0 chipx86    (501) staff       (20)     3563 2024-05-30 08:42:07.000000 django_evolution-2.4/README.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     5786 2024-05-30 08:42:07.000000 django_evolution-2.4/conftest.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      155 2024-05-30 08:42:07.000000 django_evolution-2.4/dev-requirements.txt
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.817039 django_evolution-2.4/django_evolution/
+-rw-r--r--   0 chipx86    (501) staff       (20)     1256 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      192 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/admin.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.819700 django_evolution-2.4/django_evolution/builtin_evolutions/
+-rw-r--r--   0 chipx86    (501) staff       (20)     1724 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/builtin_evolutions/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      218 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/builtin_evolutions/admin_move_to_migrations.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      137 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/builtin_evolutions/auth_delete_message.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      151 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/builtin_evolutions/auth_move_to_migrations.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      205 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/builtin_evolutions/auth_unique_together_baseline.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      225 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/builtin_evolutions/contenttypes_move_to_migrations.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      185 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/builtin_evolutions/contenttypes_unique_together_baseline.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      222 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/builtin_evolutions/flatpages_move_to_migrations.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      222 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/builtin_evolutions/redirects_move_to_migrations.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      181 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/builtin_evolutions/session_expire_date_db_index.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      151 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/builtin_evolutions/sessions_move_to_migrations.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      221 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/builtin_evolutions/sites_move_to_migrations.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.821291 django_evolution-2.4/django_evolution/compat/
+-rw-r--r--   0 chipx86    (501) staff       (20)      209 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/compat/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     6122 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/compat/apps.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5909 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/compat/commands.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      431 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/compat/datastructures.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    31895 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/compat/db.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     9727 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/compat/models.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.822166 django_evolution-2.4/django_evolution/compat/patches/
+-rw-r--r--   0 chipx86    (501) staff       (20)     1482 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/compat/patches/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1963 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/compat/patches/django1_8__1_10_mysql_preserve_db_index.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1937 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/compat/patches/django2_0_quote_unique_index_name.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1761 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/compat/patches/mysqlclient_django_pre_2_encoder_bytes.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1443 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/compat/patches/python3_10_collection_imports.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1411 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/compat/patches/sqlite_legacy_alter_table.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2234 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/compat/picklers.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1420 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/compat/py23.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    34549 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/compat/six.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      516 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/compat/translation.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5443 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/conf.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      655 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/consts.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.823713 django_evolution-2.4/django_evolution/db/
+-rw-r--r--   0 chipx86    (501) staff       (20)     1452 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/db/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    79897 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/db/common.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    11133 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/db/mysql.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      143 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/db/mysql_old.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    13363 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/db/postgresql.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      145 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/db/postgresql_psycopg2.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    10473 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/db/sql_result.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    35114 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/db/sqlite3.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    13058 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/db/state.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2288 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/deprecation.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    16065 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/diff.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4407 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/errors.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.823861 django_evolution-2.4/django_evolution/evolutions/
+-rw-r--r--   0 chipx86    (501) staff       (20)       56 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/evolutions/__init__.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.824656 django_evolution-2.4/django_evolution/evolve/
+-rw-r--r--   0 chipx86    (501) staff       (20)      919 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/evolve/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     7123 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/evolve/base.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    61328 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/evolve/evolve_app_task.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    19887 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/evolve/evolver.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3297 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/evolve/purge_app_task.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.824770 django_evolution-2.4/django_evolution/management/
+-rw-r--r--   0 chipx86    (501) staff       (20)     4574 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/management/__init__.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.826058 django_evolution-2.4/django_evolution/management/commands/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/management/commands/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     8921 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/management/commands/evolution-project-sig.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    24461 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/management/commands/evolve.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1249 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/management/commands/list-evolutions.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5449 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/management/commands/mark-evolution-applied.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3265 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/management/commands/migrate.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2231 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/management/commands/syncdb.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3330 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/management/commands/wipe-evolution.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    19044 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/mock_models.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     8738 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/models.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.827770 django_evolution-2.4/django_evolution/mutations/
+-rw-r--r--   0 chipx86    (501) staff       (20)     2725 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/mutations/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     7279 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/mutations/add_field.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    19564 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/mutations/base.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     9774 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/mutations/change_field.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5868 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/mutations/change_meta.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3438 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/mutations/delete_application.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3722 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/mutations/delete_field.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2532 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/mutations/delete_model.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3704 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/mutations/move_to_django_migrations.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5138 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/mutations/rename_app_label.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     6444 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/mutations/rename_field.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4134 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/mutations/rename_model.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5192 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/mutations/sql_mutation.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.828505 django_evolution-2.4/django_evolution/mutators/
+-rw-r--r--   0 chipx86    (501) staff       (20)      790 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/mutators/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    40252 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/mutators/app_mutator.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5113 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/mutators/base.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    11738 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/mutators/model_mutator.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1492 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/mutators/sql_mutator.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1517 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/mutators/upgrade_method_mutator.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2960 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/placeholders.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    30164 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/serialization.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2673 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/signals.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    87967 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/signature.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2292 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/support.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.833003 django_evolution-2.4/django_evolution/tests/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/__init__.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.833287 django_evolution-2.4/django_evolution/tests/app_deps_app/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/app_deps_app/__init__.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.833531 django_evolution-2.4/django_evolution/tests/app_deps_app/evolutions/
+-rw-r--r--   0 chipx86    (501) staff       (20)      393 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/app_deps_app/evolutions/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)       57 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/app_deps_app/evolutions/test_evolution.py
+-rw-r--r--   0 chipx86    (501) staff       (20)       38 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/app_deps_app/models.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    43129 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/base_test_case.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.834070 django_evolution-2.4/django_evolution/tests/db/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/db/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    80400 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/db/mysql.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    94924 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/db/postgresql.py
+-rw-r--r--   0 chipx86    (501) staff       (20)   144109 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/db/sqlite3.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     9108 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/decorators.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.834357 django_evolution-2.4/django_evolution/tests/evolution_deps_app/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/evolution_deps_app/__init__.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.834593 django_evolution-2.4/django_evolution/tests/evolution_deps_app/evolutions/
+-rw-r--r--   0 chipx86    (501) staff       (20)       79 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/evolution_deps_app/evolutions/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      371 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/evolution_deps_app/evolutions/test_evolution.py
+-rw-r--r--   0 chipx86    (501) staff       (20)       38 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/evolution_deps_app/models.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.834833 django_evolution-2.4/django_evolution/tests/evolutions_app/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/evolutions_app/__init__.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.835198 django_evolution-2.4/django_evolution/tests/evolutions_app/evolutions/
+-rw-r--r--   0 chipx86    (501) staff       (20)       62 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/evolutions_app/evolutions/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      238 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/evolutions_app/evolutions/first_evolution.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      309 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/evolutions_app/evolutions/second_evolution.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      237 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/evolutions_app/models.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.835443 django_evolution-2.4/django_evolution/tests/evolutions_app2/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/evolutions_app2/__init__.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.835692 django_evolution-2.4/django_evolution/tests/evolutions_app2/evolutions/
+-rw-r--r--   0 chipx86    (501) staff       (20)       79 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/evolutions_app2/evolutions/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      451 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/evolutions_app2/evolutions/test_evolution.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      641 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/evolutions_app2/models.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.835905 django_evolution-2.4/django_evolution/tests/migrations_app/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/migrations_app/__init__.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.836261 django_evolution-2.4/django_evolution/tests/migrations_app/migrations/
+-rw-r--r--   0 chipx86    (501) staff       (20)      870 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/migrations_app/migrations/0001_initial.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      527 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/migrations_app/migrations/0002_add_field.py
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/migrations_app/migrations/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      215 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/migrations_app/models.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.836473 django_evolution-2.4/django_evolution/tests/migrations_app2/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/migrations_app2/__init__.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.836856 django_evolution-2.4/django_evolution/tests/migrations_app2/migrations/
+-rw-r--r--   0 chipx86    (501) staff       (20)      960 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/migrations_app2/migrations/0001_initial.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      532 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/migrations_app2/migrations/0002_add_field.py
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/migrations_app2/migrations/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      220 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/migrations_app2/models.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      633 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/models.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.836960 django_evolution-2.4/django_evolution/tests/no_models_app/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/no_models_app/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    28908 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_add_field.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    92718 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_change_field.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    59809 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_change_meta.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1985 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_compat_apps.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    10933 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_compat_models.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     6448 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_conf.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    17373 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_database_state.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4361 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_datastructures_utils.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4344 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_delete_app.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    12099 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_delete_field.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     6463 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_delete_model.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     7042 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_dependency_graph.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1852 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_diff.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    24833 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_evolution_graph.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3613 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_evolution_models.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    26239 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_evolution_utils.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    81787 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_evolver.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2782 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_generics.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    35829 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_migration_utils.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2675 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_model_mutator.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1218 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_move_to_django_migrations.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1698 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_ordering.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    26964 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_preprocessing.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    20793 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_rename_field.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     9796 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_rename_model.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    21712 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_serialization.py
+-rw-r--r--   0 chipx86    (501) staff       (20)   112123 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_signature.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4190 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_sql_mutation.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     7418 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/test_utils_models.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    33974 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/tests/utils.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.837937 django_evolution-2.4/django_evolution/utils/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/utils/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2759 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/utils/apps.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2717 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/utils/datastructures.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    24033 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/utils/evolutions.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    27336 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/utils/graph.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    35220 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/utils/migrations.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     9421 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/utils/models.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    12509 2024-05-30 08:42:07.000000 django_evolution-2.4/django_evolution/utils/sql.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.817933 django_evolution-2.4/django_evolution.egg-info/
+-rw-r--r--   0 chipx86    (501) staff       (20)     5826 2024-05-30 08:42:08.000000 django_evolution-2.4/django_evolution.egg-info/PKG-INFO
+-rw-r--r--   0 chipx86    (501) staff       (20)     8876 2024-05-30 08:42:08.000000 django_evolution-2.4/django_evolution.egg-info/SOURCES.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)        1 2024-05-30 08:42:08.000000 django_evolution-2.4/django_evolution.egg-info/dependency_links.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)       65 2024-05-30 08:42:08.000000 django_evolution-2.4/django_evolution.egg-info/requires.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)       17 2024-05-30 08:42:08.000000 django_evolution-2.4/django_evolution.egg-info/top_level.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)      215 2024-05-30 08:42:07.000000 django_evolution-2.4/doc-requirements.txt
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.839154 django_evolution-2.4/docs/
+-rw-r--r--   0 chipx86    (501) staff       (20)      700 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/Makefile
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.839261 django_evolution-2.4/docs/coderef/
+-rw-r--r--   0 chipx86    (501) staff       (20)     2460 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/coderef/index.rst
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.839980 django_evolution-2.4/docs/commands/
+-rw-r--r--   0 chipx86    (501) staff       (20)     1487 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/commands/evolution-project-sig.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     3427 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/commands/evolve.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      204 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/commands/index.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      648 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/commands/list-evolutions.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     1162 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/commands/mark-evolution-applied.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     1257 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/commands/wipe-evolution.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     6448 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/conf.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     6241 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/faq.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     1281 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/glossary.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     1531 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/how-does-it-work.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     3046 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/index.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      321 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/installation.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)    15172 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/mutations.rst
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.844426 django_evolution-2.4/docs/releasenotes/
+-rw-r--r--   0 chipx86    (501) staff       (20)     1306 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.5.1.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      121 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.5.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      245 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.6.1.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      569 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.6.2.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     1203 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.6.3.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     1257 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.6.4.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     1007 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.6.5.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     1074 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.6.6.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      479 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.6.7.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      760 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.6.8.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      695 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.6.9.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      532 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.6.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     3334 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.7-beta-1.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      468 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.7.1.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      428 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.7.2.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      770 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.7.3.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      592 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.7.4.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      984 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.7.5.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     1188 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.7.6.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     1767 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.7.7.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      680 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.7.8.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     3321 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/0.7.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     7179 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/2.0.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      536 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/2.1.1.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      348 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/2.1.2.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     1859 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/2.1.3.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      316 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/2.1.4.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     2046 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/2.1.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     2154 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/2.2.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     1692 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/2.3.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     1319 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/2.4.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      565 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/releasenotes/index.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      578 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/versioning.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)     8969 2024-05-30 08:42:07.000000 django_evolution-2.4/docs/writing-evolutions.rst
+-rw-r--r--   0 chipx86    (501) staff       (20)      268 2024-05-30 08:42:08.845064 django_evolution-2.4/setup.cfg
+-rwxr-xr-x   0 chipx86    (501) staff       (20)     3024 2024-05-30 08:42:07.000000 django_evolution-2.4/setup.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2024-05-30 08:42:08.844573 django_evolution-2.4/tests/
+-rw-r--r--   0 chipx86    (501) staff       (20)      986 2024-05-30 08:42:07.000000 django_evolution-2.4/tests/test_db_settings.py.tmpl
```

### Comparing `django_evolution-2.3/AUTHORS` & `django_evolution-2.4/AUTHORS`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/LICENSE` & `django_evolution-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/PKG-INFO` & `django_evolution-2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django_evolution
-Version: 2.3
+Version: 2.4
 Summary: A database schema evolution tool for the Django web framework.
 Home-page: https://github.com/beanbaginc/django-evolution
-Download-URL: https://downloads.reviewboard.org/releases/django-evolution/2.3/
+Download-URL: https://downloads.reviewboard.org/releases/django-evolution/2.4/
 Author: Beanbag, Inc.
 Author-email: reviewboard@googlegroups.com
 Maintainer: Beanbag, Inc.
 Maintainer-email: reviewboard@googlegroups.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `django_evolution-2.3/README.rst` & `django_evolution-2.4/README.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/conftest.py` & `django_evolution-2.4/conftest.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/__init__.py` & `django_evolution-2.4/django_evolution/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # The version of Django Evolution
 #
 # This is in the format of:
 #
 #   (Major, Minor, Micro, alpha/beta/rc/final, Release Number, Released)
 #
-VERSION = (2, 3, 0, 'final', 0, True)
+VERSION = (2, 4, 0, 'final', 0, True)
 
 
 def get_version_string():
     version = '%s.%s' % (VERSION[0], VERSION[1])
 
     if VERSION[2]:
         version += ".%s" % VERSION[2]
```

### Comparing `django_evolution-2.3/django_evolution/builtin_evolutions/__init__.py` & `django_evolution-2.4/django_evolution/builtin_evolutions/__init__.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/compat/apps.py` & `django_evolution-2.4/django_evolution/compat/apps.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/compat/commands.py` & `django_evolution-2.4/django_evolution/compat/commands.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/compat/db.py` & `django_evolution-2.4/django_evolution/compat/db.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/compat/models.py` & `django_evolution-2.4/django_evolution/compat/models.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/compat/patches/__init__.py` & `django_evolution-2.4/django_evolution/compat/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/compat/patches/django1_8__1_10_mysql_preserve_db_index.py` & `django_evolution-2.4/django_evolution/compat/patches/django1_8__1_10_mysql_preserve_db_index.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/compat/patches/django2_0_quote_unique_index_name.py` & `django_evolution-2.4/django_evolution/compat/patches/django2_0_quote_unique_index_name.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/compat/patches/mysqlclient_django_pre_2_encoder_bytes.py` & `django_evolution-2.4/django_evolution/compat/patches/mysqlclient_django_pre_2_encoder_bytes.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/compat/patches/python3_10_collection_imports.py` & `django_evolution-2.4/django_evolution/compat/patches/python3_10_collection_imports.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/compat/patches/sqlite_legacy_alter_table.py` & `django_evolution-2.4/django_evolution/compat/patches/sqlite_legacy_alter_table.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/compat/picklers.py` & `django_evolution-2.4/django_evolution/compat/picklers.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/compat/py23.py` & `django_evolution-2.4/django_evolution/compat/py23.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/compat/six.py` & `django_evolution-2.4/django_evolution/compat/six.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/compat/translation.py` & `django_evolution-2.4/django_evolution/compat/translation.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/conf.py` & `django_evolution-2.4/django_evolution/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,20 +51,32 @@
             also cause Django Evolution to track state.
 
             If disabled, the management commands will operate no differently
             than in a normal Django installation.
 
             Type:
                 bool
+
+        RENAMED_FIELD_TYPES:
+            A mapping for fields that have been moved or renamed. This will map
+            the old path to the new one, for purposes of loading and validating
+            field signatures.
+
+            Type:
+                dict
+
+            Version Added:
+                2.4
     """
 
     #: Default settings for all keys.
     _DEFAULTS = {
         'CUSTOM_EVOLUTIONS': {},
         'ENABLED': True,
+        'RENAMED_FIELD_TYPES': {},
     }
 
     #: All valid settings in settings.DJANGO_EVOLUTION.
     _VALID_SETTINGS = set(_DEFAULTS.keys())
 
     #: A mapping of all deprecated settings to modern settings.
     _DEPRECATED_SETTINGS = {
```

### Comparing `django_evolution-2.3/django_evolution/consts.py` & `django_evolution-2.4/django_evolution/consts.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/db/__init__.py` & `django_evolution-2.4/django_evolution/db/__init__.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/db/common.py` & `django_evolution-2.4/django_evolution/db/common.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/db/mysql.py` & `django_evolution-2.4/django_evolution/db/mysql.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/db/postgresql.py` & `django_evolution-2.4/django_evolution/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/db/sql_result.py` & `django_evolution-2.4/django_evolution/db/sql_result.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/db/sqlite3.py` & `django_evolution-2.4/django_evolution/db/sqlite3.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/db/state.py` & `django_evolution-2.4/django_evolution/db/state.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/deprecation.py` & `django_evolution-2.4/django_evolution/deprecation.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/diff.py` & `django_evolution-2.4/django_evolution/diff.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/errors.py` & `django_evolution-2.4/django_evolution/errors.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/evolve/__init__.py` & `django_evolution-2.4/django_evolution/evolve/__init__.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/evolve/base.py` & `django_evolution-2.4/django_evolution/evolve/base.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/evolve/evolve_app_task.py` & `django_evolution-2.4/django_evolution/evolve/evolve_app_task.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/evolve/evolver.py` & `django_evolution-2.4/django_evolution/evolve/evolver.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/evolve/purge_app_task.py` & `django_evolution-2.4/django_evolution/evolve/purge_app_task.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/management/__init__.py` & `django_evolution-2.4/django_evolution/management/__init__.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/management/commands/evolution-project-sig.py` & `django_evolution-2.4/django_evolution/management/commands/evolution-project-sig.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/management/commands/evolve.py` & `django_evolution-2.4/django_evolution/management/commands/evolve.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/management/commands/list-evolutions.py` & `django_evolution-2.4/django_evolution/management/commands/list-evolutions.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/management/commands/mark-evolution-applied.py` & `django_evolution-2.4/django_evolution/management/commands/mark-evolution-applied.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/management/commands/migrate.py` & `django_evolution-2.4/django_evolution/management/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/management/commands/syncdb.py` & `django_evolution-2.4/django_evolution/management/commands/syncdb.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/management/commands/wipe-evolution.py` & `django_evolution-2.4/django_evolution/management/commands/wipe-evolution.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/mock_models.py` & `django_evolution-2.4/django_evolution/mock_models.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/models.py` & `django_evolution-2.4/django_evolution/models.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/mutations/__init__.py` & `django_evolution-2.4/django_evolution/mutations/__init__.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/mutations/add_field.py` & `django_evolution-2.4/django_evolution/mutations/add_field.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/mutations/base.py` & `django_evolution-2.4/django_evolution/mutations/base.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/mutations/change_field.py` & `django_evolution-2.4/django_evolution/mutations/change_field.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/mutations/change_meta.py` & `django_evolution-2.4/django_evolution/mutations/change_meta.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/mutations/delete_application.py` & `django_evolution-2.4/django_evolution/mutations/delete_application.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/mutations/delete_field.py` & `django_evolution-2.4/django_evolution/mutations/delete_field.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/mutations/delete_model.py` & `django_evolution-2.4/django_evolution/mutations/delete_model.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/mutations/move_to_django_migrations.py` & `django_evolution-2.4/django_evolution/mutations/move_to_django_migrations.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/mutations/rename_app_label.py` & `django_evolution-2.4/django_evolution/mutations/rename_app_label.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/mutations/rename_field.py` & `django_evolution-2.4/django_evolution/mutations/rename_field.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/mutations/rename_model.py` & `django_evolution-2.4/django_evolution/mutations/rename_model.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/mutations/sql_mutation.py` & `django_evolution-2.4/django_evolution/mutations/sql_mutation.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/mutators/__init__.py` & `django_evolution-2.4/django_evolution/mutators/__init__.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/mutators/app_mutator.py` & `django_evolution-2.4/django_evolution/mutators/app_mutator.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/mutators/base.py` & `django_evolution-2.4/django_evolution/mutators/base.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/mutators/model_mutator.py` & `django_evolution-2.4/django_evolution/mutators/model_mutator.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/mutators/sql_mutator.py` & `django_evolution-2.4/django_evolution/mutators/sql_mutator.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/mutators/upgrade_method_mutator.py` & `django_evolution-2.4/django_evolution/mutators/upgrade_method_mutator.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/placeholders.py` & `django_evolution-2.4/django_evolution/placeholders.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/serialization.py` & `django_evolution-2.4/django_evolution/serialization.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/signals.py` & `django_evolution-2.4/django_evolution/signals.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/signature.py` & `django_evolution-2.4/django_evolution/signature.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,15 @@
 from django_evolution.compat.datastructures import OrderedDict
 from django_evolution.compat.db import db_router_allows_schema_upgrade
 from django_evolution.compat.models import (GenericRelation,
                                             get_models,
                                             get_remote_field,
                                             get_remote_field_model)
 from django_evolution.compat.translation import gettext as _
+from django_evolution.conf import django_evolution_settings
 from django_evolution.consts import UpgradeMethod
 from django_evolution.errors import (InvalidSignatureVersion,
                                      MissingSignatureError)
 from django_evolution.serialization import (deserialize_from_signature,
                                             serialize_to_signature)
 from django_evolution.utils.apps import get_app_label, get_legacy_app_label
 from django_evolution.utils.evolutions import get_app_upgrade_info
@@ -2263,17 +2264,22 @@
                 The signature version provided isn't supported.
         """
         validate_sig_version(sig_version)
 
         if sig_version == 2:
             field_sig_attrs = field_sig_dict.get('attrs', {})
 
+            field_type = field_sig_dict['type']
+            renamed_types = django_evolution_settings.RENAMED_FIELD_TYPES
+
+            if field_type in renamed_types:
+                field_type = renamed_types[field_type]
+
             # Load the class for the referenced field type.
-            field_type_module, field_type_name = \
-                field_sig_dict['type'].rsplit('.', 1)
+            field_type_module, field_type_name = field_type.rsplit('.', 1)
 
             # If we have a field path in the signature that lives in
             # django.db.models.fields, update it to look in django.db.models
             # instead. This is for compatibility across all Django versions.
             if field_type_module.startswith('django.db.models.fields'):
                 field_type_module = 'django.db.models'
```

### Comparing `django_evolution-2.3/django_evolution/support.py` & `django_evolution-2.4/django_evolution/support.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/base_test_case.py` & `django_evolution-2.4/django_evolution/tests/base_test_case.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/db/mysql.py` & `django_evolution-2.4/django_evolution/tests/db/mysql.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/db/postgresql.py` & `django_evolution-2.4/django_evolution/tests/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/db/sqlite3.py` & `django_evolution-2.4/django_evolution/tests/db/sqlite3.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/decorators.py` & `django_evolution-2.4/django_evolution/tests/decorators.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/evolutions_app2/models.py` & `django_evolution-2.4/django_evolution/tests/evolutions_app2/models.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/migrations_app/migrations/0001_initial.py` & `django_evolution-2.4/django_evolution/tests/migrations_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/migrations_app/migrations/0002_add_field.py` & `django_evolution-2.4/django_evolution/tests/migrations_app/migrations/0002_add_field.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/migrations_app2/migrations/0001_initial.py` & `django_evolution-2.4/django_evolution/tests/migrations_app2/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/migrations_app2/migrations/0002_add_field.py` & `django_evolution-2.4/django_evolution/tests/migrations_app2/migrations/0002_add_field.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/models.py` & `django_evolution-2.4/django_evolution/tests/models.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_add_field.py` & `django_evolution-2.4/django_evolution/tests/test_add_field.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_change_field.py` & `django_evolution-2.4/django_evolution/tests/test_change_field.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_change_meta.py` & `django_evolution-2.4/django_evolution/tests/test_change_meta.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_compat_apps.py` & `django_evolution-2.4/django_evolution/tests/test_compat_apps.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_compat_models.py` & `django_evolution-2.4/django_evolution/tests/test_compat_models.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_conf.py` & `django_evolution-2.4/django_evolution/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_database_state.py` & `django_evolution-2.4/django_evolution/tests/test_database_state.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_datastructures_utils.py` & `django_evolution-2.4/django_evolution/tests/test_datastructures_utils.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_delete_app.py` & `django_evolution-2.4/django_evolution/tests/test_delete_app.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_delete_field.py` & `django_evolution-2.4/django_evolution/tests/test_delete_field.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_delete_model.py` & `django_evolution-2.4/django_evolution/tests/test_delete_model.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_dependency_graph.py` & `django_evolution-2.4/django_evolution/tests/test_dependency_graph.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_diff.py` & `django_evolution-2.4/django_evolution/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_evolution_graph.py` & `django_evolution-2.4/django_evolution/tests/test_evolution_graph.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_evolution_models.py` & `django_evolution-2.4/django_evolution/tests/test_evolution_models.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_evolution_utils.py` & `django_evolution-2.4/django_evolution/tests/test_evolution_utils.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_evolver.py` & `django_evolution-2.4/django_evolution/tests/test_evolver.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_generics.py` & `django_evolution-2.4/django_evolution/tests/test_generics.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_migration_utils.py` & `django_evolution-2.4/django_evolution/tests/test_migration_utils.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_model_mutator.py` & `django_evolution-2.4/django_evolution/tests/test_model_mutator.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_move_to_django_migrations.py` & `django_evolution-2.4/django_evolution/tests/test_move_to_django_migrations.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_ordering.py` & `django_evolution-2.4/django_evolution/tests/test_ordering.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_preprocessing.py` & `django_evolution-2.4/django_evolution/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_rename_field.py` & `django_evolution-2.4/django_evolution/tests/test_rename_field.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_rename_model.py` & `django_evolution-2.4/django_evolution/tests/test_rename_model.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_serialization.py` & `django_evolution-2.4/django_evolution/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_signature.py` & `django_evolution-2.4/django_evolution/tests/test_signature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1150,14 +1150,47 @@
         self.assertEqual(
             field_sig.field_attrs,
             {
                 'null': False,
                 'db_column': 'test_column',
             })
 
+    def test_deserialize_v2_with_renamed_field_types(self):
+        """Testing FieldSignature.deserialize (signature v2) with renamed
+        fields configured in django_evolution_settings.RENAMED_FIELD_TYPES
+        """
+        new_settings = {
+            'RENAMED_FIELD_TYPES': {
+                'legacy.CustomForeignKey': 'django.db.models.ForeignKey',
+            },
+        }
+
+        with self.settings(DJANGO_EVOLUTION=new_settings):
+            field_sig = FieldSignature.deserialize(
+                'myfield',
+                {
+                    'type': 'legacy.CustomForeignKey',
+                    'related_model': 'tests.Anchor2',
+                    'attrs': {
+                        'null': False,
+                        'db_column': 'test_column',
+                    },
+                },
+                sig_version=2)
+
+        self.assertEqual(field_sig.field_name, 'myfield')
+        self.assertIs(field_sig.field_type, models.ForeignKey)
+        self.assertEqual(field_sig.related_model, 'tests.Anchor2')
+        self.assertEqual(
+            field_sig.field_attrs,
+            {
+                'null': False,
+                'db_column': 'test_column',
+            })
+
     def test_get_attr_value(self):
         """Testing FieldSignature.get_attr_value"""
         field_sig = FieldSignature.from_field(
             SignatureFullModel._meta.get_field('null_field'))
 
         self.assertEqual(field_sig.get_attr_value('db_column'),
                          'size_column')
```

### Comparing `django_evolution-2.3/django_evolution/tests/test_sql_mutation.py` & `django_evolution-2.4/django_evolution/tests/test_sql_mutation.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/test_utils_models.py` & `django_evolution-2.4/django_evolution/tests/test_utils_models.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/tests/utils.py` & `django_evolution-2.4/django_evolution/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/utils/apps.py` & `django_evolution-2.4/django_evolution/utils/apps.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/utils/datastructures.py` & `django_evolution-2.4/django_evolution/utils/datastructures.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/utils/evolutions.py` & `django_evolution-2.4/django_evolution/utils/evolutions.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/utils/graph.py` & `django_evolution-2.4/django_evolution/utils/graph.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/utils/migrations.py` & `django_evolution-2.4/django_evolution/utils/migrations.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/utils/models.py` & `django_evolution-2.4/django_evolution/utils/models.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution/utils/sql.py` & `django_evolution-2.4/django_evolution/utils/sql.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/django_evolution.egg-info/PKG-INFO` & `django_evolution-2.4/django_evolution.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-evolution
-Version: 2.3
+Version: 2.4
 Summary: A database schema evolution tool for the Django web framework.
 Home-page: https://github.com/beanbaginc/django-evolution
-Download-URL: https://downloads.reviewboard.org/releases/django-evolution/2.3/
+Download-URL: https://downloads.reviewboard.org/releases/django-evolution/2.4/
 Author: Beanbag, Inc.
 Author-email: reviewboard@googlegroups.com
 Maintainer: Beanbag, Inc.
 Maintainer-email: reviewboard@googlegroups.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `django_evolution-2.3/django_evolution.egg-info/SOURCES.txt` & `django_evolution-2.4/django_evolution.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -215,9 +215,10 @@
 docs/releasenotes/2.1.1.rst
 docs/releasenotes/2.1.2.rst
 docs/releasenotes/2.1.3.rst
 docs/releasenotes/2.1.4.rst
 docs/releasenotes/2.1.rst
 docs/releasenotes/2.2.rst
 docs/releasenotes/2.3.rst
+docs/releasenotes/2.4.rst
 docs/releasenotes/index.rst
 tests/test_db_settings.py.tmpl
```

### Comparing `django_evolution-2.3/docs/Makefile` & `django_evolution-2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/coderef/index.rst` & `django_evolution-2.4/docs/coderef/index.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/commands/evolution-project-sig.rst` & `django_evolution-2.4/docs/commands/evolution-project-sig.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/commands/evolve.rst` & `django_evolution-2.4/docs/commands/evolve.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/commands/list-evolutions.rst` & `django_evolution-2.4/docs/commands/list-evolutions.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/commands/mark-evolution-applied.rst` & `django_evolution-2.4/docs/commands/mark-evolution-applied.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/commands/wipe-evolution.rst` & `django_evolution-2.4/docs/commands/wipe-evolution.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/conf.py` & `django_evolution-2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/faq.rst` & `django_evolution-2.4/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/glossary.rst` & `django_evolution-2.4/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/how-does-it-work.rst` & `django_evolution-2.4/docs/how-does-it-work.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/index.rst` & `django_evolution-2.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/mutations.rst` & `django_evolution-2.4/docs/mutations.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/0.5.1.rst` & `django_evolution-2.4/docs/releasenotes/0.5.1.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/0.6.2.rst` & `django_evolution-2.4/docs/releasenotes/0.6.2.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/0.6.3.rst` & `django_evolution-2.4/docs/releasenotes/0.6.3.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/0.6.4.rst` & `django_evolution-2.4/docs/releasenotes/0.6.4.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/0.6.5.rst` & `django_evolution-2.4/docs/releasenotes/0.6.5.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/0.6.6.rst` & `django_evolution-2.4/docs/releasenotes/0.6.6.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/0.6.8.rst` & `django_evolution-2.4/docs/releasenotes/0.6.8.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/0.6.9.rst` & `django_evolution-2.4/docs/releasenotes/0.6.9.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/0.6.rst` & `django_evolution-2.4/docs/releasenotes/0.6.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/0.7-beta-1.rst` & `django_evolution-2.4/docs/releasenotes/0.7-beta-1.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/0.7.3.rst` & `django_evolution-2.4/docs/releasenotes/0.7.3.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/0.7.4.rst` & `django_evolution-2.4/docs/releasenotes/0.7.4.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/0.7.5.rst` & `django_evolution-2.4/docs/releasenotes/0.7.5.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/0.7.6.rst` & `django_evolution-2.4/docs/releasenotes/0.7.6.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/0.7.7.rst` & `django_evolution-2.4/docs/releasenotes/0.7.7.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/0.7.8.rst` & `django_evolution-2.4/docs/releasenotes/0.7.8.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/0.7.rst` & `django_evolution-2.4/docs/releasenotes/0.7.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/2.0.rst` & `django_evolution-2.4/docs/releasenotes/2.0.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/2.1.1.rst` & `django_evolution-2.4/docs/releasenotes/2.1.1.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/2.1.3.rst` & `django_evolution-2.4/docs/releasenotes/2.1.3.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/2.1.rst` & `django_evolution-2.4/docs/releasenotes/2.1.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/2.2.rst` & `django_evolution-2.4/docs/releasenotes/2.2.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/2.3.rst` & `django_evolution-2.4/docs/releasenotes/2.3.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/releasenotes/index.rst` & `django_evolution-2.4/docs/releasenotes/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 2.x Releases
 ============
 
 .. toctree::
    :maxdepth: 1
 
+   2.4
    2.3
    2.2
    2.1.4
    2.1.3
    2.1.2
    2.1.1
    2.1
```

### Comparing `django_evolution-2.3/docs/versioning.rst` & `django_evolution-2.4/docs/versioning.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/docs/writing-evolutions.rst` & `django_evolution-2.4/docs/writing-evolutions.rst`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/setup.py` & `django_evolution-2.4/setup.py`

 * *Files identical despite different names*

### Comparing `django_evolution-2.3/tests/test_db_settings.py.tmpl` & `django_evolution-2.4/tests/test_db_settings.py.tmpl`

 * *Files identical despite different names*

