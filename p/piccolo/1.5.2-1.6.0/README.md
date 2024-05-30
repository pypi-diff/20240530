# Comparing `tmp/piccolo-1.5.2.tar.gz` & `tmp/piccolo-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piccolo-1.5.2.tar", last modified: Tue May 28 23:08:12 2024, max compression
+gzip compressed data, was "piccolo-1.6.0.tar", last modified: Thu May 30 00:16:59 2024, max compression
```

## Comparing `piccolo-1.5.2.tar` & `piccolo-1.6.0.tar`

### file list

```diff
@@ -1,456 +1,462 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.070064 piccolo-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-28 23:07:46.000000 piccolo-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-28 23:08:12.070064 piccolo-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-28 23:07:46.000000 piccolo-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.010064 piccolo-1.5.2/piccolo/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.010064 piccolo-1.5.2/piccolo/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.010064 piccolo-1.5.2/piccolo/apps/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.014064 piccolo-1.5.2/piccolo/apps/app/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/app/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/app/commands/new.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/app/commands/show_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.014064 piccolo-1.5.2/piccolo/apps/app/commands/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/app/commands/templates/piccolo_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/app/commands/templates/tables.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/app/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.014064 piccolo-1.5.2/piccolo/apps/asgi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.014064 piccolo-1.5.2/piccolo/apps/asgi/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/new.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:11.998064 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.014064 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/README.md.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/_esmerald_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/_lilya_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/_litestar_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/conftest.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.018064 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/home/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/home/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/home/_blacksheep_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/home/_esmerald_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/home/_lilya_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/home/_litestar_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/home/_starlette_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/home/endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/home/piccolo_app.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.018064 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/home/tables.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.018064 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/home/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/home/templates/base.html.jinja_raw
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/main.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/piccolo_conf.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/piccolo_conf_test.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/requirements.txt.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.018064 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/static/main.css
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/asgi/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.018064 piccolo-1.5.2/piccolo/apps/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.018064 piccolo-1.5.2/piccolo/apps/fixtures/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/fixtures/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/fixtures/commands/dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/fixtures/commands/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/fixtures/commands/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/fixtures/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.018064 piccolo-1.5.2/piccolo/apps/meta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.018064 piccolo-1.5.2/piccolo/apps/meta/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/meta/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/meta/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/meta/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.018064 piccolo-1.5.2/piccolo/apps/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.022064 piccolo-1.5.2/piccolo/apps/migrations/auto/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/migrations/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/migrations/auto/diffable_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    35096 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/migrations/auto/migration_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/migrations/auto/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    26266 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/migrations/auto/schema_differ.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/migrations/auto/schema_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    23927 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/migrations/auto/serialisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/migrations/auto/serialisation_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.022064 piccolo-1.5.2/piccolo/apps/migrations/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/migrations/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/migrations/commands/backwards.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/migrations/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/migrations/commands/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/migrations/commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/migrations/commands/forwards.py
--rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/migrations/commands/new.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.022064 piccolo-1.5.2/piccolo/apps/migrations/commands/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/migrations/commands/templates/migration.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/migrations/piccolo_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/migrations/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.022064 piccolo-1.5.2/piccolo/apps/playground/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/playground/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.022064 piccolo-1.5.2/piccolo/apps/playground/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/playground/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/playground/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/playground/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.022064 piccolo-1.5.2/piccolo/apps/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.022064 piccolo-1.5.2/piccolo/apps/project/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/project/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/project/commands/new.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.022064 piccolo-1.5.2/piccolo/apps/project/commands/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/project/commands/templates/piccolo_conf.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/project/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.026064 piccolo-1.5.2/piccolo/apps/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.026064 piccolo-1.5.2/piccolo/apps/schema/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/schema/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/schema/commands/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30638 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/schema/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/schema/commands/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.026064 piccolo-1.5.2/piccolo/apps/schema/commands/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/schema/commands/templates/graphviz.dot.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/schema/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.026064 piccolo-1.5.2/piccolo/apps/shell/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.026064 piccolo-1.5.2/piccolo/apps/shell/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/shell/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/shell/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/shell/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.026064 piccolo-1.5.2/piccolo/apps/sql_shell/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/sql_shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.026064 piccolo-1.5.2/piccolo/apps/sql_shell/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/sql_shell/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/sql_shell/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/sql_shell/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.026064 piccolo-1.5.2/piccolo/apps/tester/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/tester/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.026064 piccolo-1.5.2/piccolo/apps/tester/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/tester/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/tester/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/tester/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.030064 piccolo-1.5.2/piccolo/apps/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.030064 piccolo-1.5.2/piccolo/apps/user/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/user/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/user/commands/change_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/user/commands/change_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/user/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/user/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/user/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.030064 piccolo-1.5.2/piccolo/apps/user/piccolo_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/user/piccolo_migrations/2019-11-14T21-52-21.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/user/piccolo_migrations/2020-06-11T21-38-55.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/user/piccolo_migrations/2021-04-30T16-14-15.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/user/piccolo_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/apps/user/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.030064 piccolo-1.5.2/piccolo/columns/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31620 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/choices.py
--rw-r--r--   0 runner    (1001) docker     (127)    81013 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/combination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.034064 piccolo-1.5.2/piccolo/columns/defaults/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/defaults/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/defaults/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/defaults/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/defaults/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/defaults/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/defaults/timestamptz.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/defaults/uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/m2m.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.034064 piccolo-1.5.2/piccolo/columns/operators/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/operators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/operators/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/operators/math.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/operators/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/readable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/columns/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.034064 piccolo-1.5.2/piccolo/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18904 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/conf/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/custom_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.034064 piccolo-1.5.2/piccolo/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/engine/cockroach.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/engine/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/engine/finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18276 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/engine/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    22099 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/engine/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.038064 piccolo-1.5.2/piccolo/query/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15212 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/query/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.038064 piccolo-1.5.2/piccolo/query/methods/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/query/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16728 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/query/methods/alter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/query/methods/count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/query/methods/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/query/methods/create_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/query/methods/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/query/methods/drop_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/query/methods/exists.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/query/methods/indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/query/methods/insert.py
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/query/methods/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/query/methods/raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/query/methods/refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)    26883 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/query/methods/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/query/methods/table_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/query/methods/update.py
--rw-r--r--   0 runner    (1001) docker     (127)    21639 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/query/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/query/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/querystring.py
--rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    50001 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/table_reflection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.038064 piccolo-1.5.2/piccolo/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/testing/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/testing/random_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.042064 piccolo-1.5.2/piccolo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/utils/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/utils/encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.042064 piccolo-1.5.2/piccolo/utils/graphlib/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/utils/graphlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/utils/graphlib/_graphlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/utils/lazy_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/utils/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/utils/printing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/utils/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/utils/repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/utils/sql_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/utils/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-28 23:07:46.000000 piccolo-1.5.2/piccolo/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.070064 piccolo-1.5.2/piccolo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-28 23:08:11.000000 piccolo-1.5.2/piccolo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13281 2024-05-28 23:08:11.000000 piccolo-1.5.2/piccolo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 23:08:11.000000 piccolo-1.5.2/piccolo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 23:08:11.000000 piccolo-1.5.2/piccolo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-28 23:08:11.000000 piccolo-1.5.2/piccolo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 23:08:11.000000 piccolo-1.5.2/piccolo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.042064 piccolo-1.5.2/profiling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/profiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-28 23:07:46.000000 piccolo-1.5.2/profiling/run_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-28 23:07:46.000000 piccolo-1.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 23:08:12.074064 piccolo-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-28 23:07:46.000000 piccolo-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.042064 piccolo-1.5.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.042064 piccolo-1.5.2/tests/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.042064 piccolo-1.5.2/tests/apps/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.042064 piccolo-1.5.2/tests/apps/app/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/app/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/app/commands/test_new.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/app/commands/test_show_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.042064 piccolo-1.5.2/tests/apps/asgi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/asgi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.046064 piccolo-1.5.2/tests/apps/asgi/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/asgi/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/asgi/commands/test_new.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.046064 piccolo-1.5.2/tests/apps/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.046064 piccolo-1.5.2/tests/apps/fixtures/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/fixtures/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/fixtures/commands/test_dump_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/fixtures/commands/test_shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.046064 piccolo-1.5.2/tests/apps/meta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.046064 piccolo-1.5.2/tests/apps/meta/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/meta/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/meta/commands/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.046064 piccolo-1.5.2/tests/apps/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.046064 piccolo-1.5.2/tests/apps/migrations/auto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/migrations/auto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.046064 piccolo-1.5.2/tests/apps/migrations/auto/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/migrations/auto/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46131 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/migrations/auto/integration/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/migrations/auto/test_diffable_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    34741 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/migrations/auto/test_migration_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    19391 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/migrations/auto/test_schema_differ.py
--rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/migrations/auto/test_schema_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/migrations/auto/test_serialisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.046064 piccolo-1.5.2/tests/apps/migrations/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/migrations/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/migrations/commands/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/migrations/commands/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/migrations/commands/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/migrations/commands/test_forwards_backwards.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.050064 piccolo-1.5.2/tests/apps/migrations/commands/test_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/migrations/commands/test_migrations/2020-03-31T20-38-22.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/migrations/commands/test_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/migrations/commands/test_new.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/migrations/test_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.050064 piccolo-1.5.2/tests/apps/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.050064 piccolo-1.5.2/tests/apps/project/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/project/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/project/commands/test_new.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.050064 piccolo-1.5.2/tests/apps/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.050064 piccolo-1.5.2/tests/apps/shell/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.050064 piccolo-1.5.2/tests/apps/shell/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/shell/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/shell/commands/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.050064 piccolo-1.5.2/tests/apps/sql_shell/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/sql_shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.050064 piccolo-1.5.2/tests/apps/sql_shell/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/sql_shell/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/sql_shell/commands/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.050064 piccolo-1.5.2/tests/apps/tester/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/tester/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.050064 piccolo-1.5.2/tests/apps/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.050064 piccolo-1.5.2/tests/apps/user/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/user/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/user/commands/test_change_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/user/commands/test_change_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/user/commands/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/user/commands/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/apps/user/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.054064 piccolo-1.5.2/tests/columns/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.058064 piccolo-1.5.2/tests/columns/m2m/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/m2m/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/m2m/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/m2m/test_m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/m2m/test_m2m_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_bigint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_bytea.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_choices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_combination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_db_column_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_double_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_jsonb.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_numeric.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_primary_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_readable.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_real.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_reserved_column_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_smallint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_timestamptz.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/columns/test_varchar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.058064 piccolo-1.5.2/tests/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/conf/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/conf/test_apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.058064 piccolo-1.5.2/tests/engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/engine/test_extra_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/engine/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/engine/test_nested_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/engine/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/engine/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/engine/test_version_parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.058064 piccolo-1.5.2/tests/example_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/example_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.058064 piccolo-1.5.2/tests/example_apps/mega/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/example_apps/mega/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/example_apps/mega/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.058064 piccolo-1.5.2/tests/example_apps/mega/piccolo_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/example_apps/mega/piccolo_migrations/2021-09-20T21-23-25-698988.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/example_apps/mega/piccolo_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/example_apps/mega/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.058064 piccolo-1.5.2/tests/example_apps/music/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/example_apps/music/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/example_apps/music/piccolo_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/example_apps/music/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/example_apps/music/tables_detailed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.062064 piccolo-1.5.2/tests/query/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/query/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.062064 piccolo-1.5.2/tests/query/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/query/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/query/mixins/test_columns_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/query/mixins/test_order_by_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/query/test_await.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/query/test_camelcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/query/test_freeze.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/query/test_gather.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/query/test_querystring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/query/test_slots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.066064 piccolo-1.5.2/tests/table/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.066064 piccolo-1.5.2/tests/table/instance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/instance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/instance/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/instance/test_get_related.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/instance/test_get_related_readable.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/instance/test_instantiate.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/instance/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/instance/test_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/instance/test_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_all_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_alter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_create_db_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_create_table_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_drop_db_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_from_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)    13695 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_insert.py
--rw-r--r--   0 runner    (1001) docker     (127)    15910 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_join_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)    40607 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_table_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/table/test_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.066064 piccolo-1.5.2/tests/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/testing/test_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/testing/test_random_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:08:12.070064 piccolo-1.5.2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/utils/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/utils/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/utils/test_lazy_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/utils/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/utils/test_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/utils/test_printing.py
--rw-r--r--   0 runner    (1001) docker     (127)    26623 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/utils/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/utils/test_sql_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/utils/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/utils/test_table_reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-28 23:07:46.000000 piccolo-1.5.2/tests/utils/test_warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.843379 piccolo-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-30 00:16:23.000000 piccolo-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-30 00:16:59.843379 piccolo-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-30 00:16:23.000000 piccolo-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.775379 piccolo-1.6.0/piccolo/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.775379 piccolo-1.6.0/piccolo/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.775379 piccolo-1.6.0/piccolo/apps/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.779379 piccolo-1.6.0/piccolo/apps/app/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/app/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/app/commands/new.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/app/commands/show_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.779379 piccolo-1.6.0/piccolo/apps/app/commands/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/app/commands/templates/piccolo_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/app/commands/templates/tables.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/app/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.779379 piccolo-1.6.0/piccolo/apps/asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.779379 piccolo-1.6.0/piccolo/apps/asgi/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.763378 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.779379 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/README.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_esmerald_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_lilya_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_litestar_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/conftest.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.783378 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/_blacksheep_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/_esmerald_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/_lilya_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/_litestar_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/_starlette_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_app.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.783378 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/tables.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.783378 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/templates/base.html.jinja_raw
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/main.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/piccolo_conf.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/piccolo_conf_test.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/requirements.txt.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.783378 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/static/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/asgi/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.783378 piccolo-1.6.0/piccolo/apps/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.783378 piccolo-1.6.0/piccolo/apps/fixtures/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/fixtures/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/fixtures/commands/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/fixtures/commands/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/fixtures/commands/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/fixtures/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.783378 piccolo-1.6.0/piccolo/apps/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.783378 piccolo-1.6.0/piccolo/apps/meta/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/meta/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/meta/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/meta/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.787379 piccolo-1.6.0/piccolo/apps/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.787379 piccolo-1.6.0/piccolo/apps/migrations/auto/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/auto/diffable_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35096 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/auto/migration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/auto/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26266 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/auto/schema_differ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/auto/schema_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23927 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/auto/serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/auto/serialisation_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.787379 piccolo-1.6.0/piccolo/apps/migrations/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/commands/backwards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/commands/forwards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/commands/new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.787379 piccolo-1.6.0/piccolo/apps/migrations/commands/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/commands/templates/migration.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/piccolo_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/migrations/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.787379 piccolo-1.6.0/piccolo/apps/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/playground/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/playground/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/playground/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/playground/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/playground/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/project/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/project/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/project/commands/new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/project/commands/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/project/commands/templates/piccolo_conf.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/project/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/schema/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/schema/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/schema/commands/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30638 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/schema/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/schema/commands/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/schema/commands/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/schema/commands/templates/graphviz.dot.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/schema/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/shell/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/shell/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/shell/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/shell/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/sql_shell/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/sql_shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.791379 piccolo-1.6.0/piccolo/apps/sql_shell/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/sql_shell/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/sql_shell/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/sql_shell/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.795379 piccolo-1.6.0/piccolo/apps/tester/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/tester/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.795379 piccolo-1.6.0/piccolo/apps/tester/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/tester/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/tester/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/tester/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.795379 piccolo-1.6.0/piccolo/apps/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.795379 piccolo-1.6.0/piccolo/apps/user/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/commands/change_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/commands/change_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.795379 piccolo-1.6.0/piccolo/apps/user/piccolo_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/piccolo_migrations/2019-11-14T21-52-21.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/piccolo_migrations/2020-06-11T21-38-55.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/piccolo_migrations/2021-04-30T16-14-15.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/piccolo_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/apps/user/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.799378 piccolo-1.6.0/piccolo/columns/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31288 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81069 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/combination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.799378 piccolo-1.6.0/piccolo/columns/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/defaults/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/defaults/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/defaults/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/defaults/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/defaults/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/defaults/timestamptz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/defaults/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14595 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/m2m.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.799378 piccolo-1.6.0/piccolo/columns/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/operators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/operators/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/operators/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/operators/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/readable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/columns/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.799378 piccolo-1.6.0/piccolo/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18904 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/conf/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/custom_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.803379 piccolo-1.6.0/piccolo/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/engine/cockroach.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/engine/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/engine/finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18276 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/engine/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22099 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/engine/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.803379 piccolo-1.6.0/piccolo/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15212 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.803379 piccolo-1.6.0/piccolo/query/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/functions/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/functions/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/functions/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.807379 piccolo-1.6.0/piccolo/query/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16728 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/alter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/create_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/drop_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/insert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21053 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/table_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/methods/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21982 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/query/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8671 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/querystring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49457 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/table_reflection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.807379 piccolo-1.6.0/piccolo/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/testing/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/testing/random_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/piccolo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/piccolo/utils/graphlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/graphlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/graphlib/_graphlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/lazy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/sql_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-30 00:16:23.000000 piccolo-1.6.0/piccolo/utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.839379 piccolo-1.6.0/piccolo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-30 00:16:59.000000 piccolo-1.6.0/piccolo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13450 2024-05-30 00:16:59.000000 piccolo-1.6.0/piccolo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 00:16:59.000000 piccolo-1.6.0/piccolo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 00:16:59.000000 piccolo-1.6.0/piccolo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-30 00:16:59.000000 piccolo-1.6.0/piccolo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 00:16:59.000000 piccolo-1.6.0/piccolo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/profiling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/profiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-30 00:16:23.000000 piccolo-1.6.0/profiling/run_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-30 00:16:23.000000 piccolo-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 00:16:59.843379 piccolo-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-30 00:16:23.000000 piccolo-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/tests/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/tests/apps/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/tests/apps/app/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/app/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/app/commands/test_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/app/commands/test_show_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/tests/apps/asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/asgi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/tests/apps/asgi/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/asgi/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/asgi/commands/test_new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/tests/apps/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/tests/apps/fixtures/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/fixtures/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/fixtures/commands/test_dump_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/fixtures/commands/test_shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/tests/apps/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.811379 piccolo-1.6.0/tests/apps/meta/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/meta/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/meta/commands/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.815379 piccolo-1.6.0/tests/apps/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.815379 piccolo-1.6.0/tests/apps/migrations/auto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/auto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.815379 piccolo-1.6.0/tests/apps/migrations/auto/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/auto/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46131 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/auto/integration/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/auto/test_diffable_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34741 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/auto/test_migration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19391 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/auto/test_schema_differ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/auto/test_schema_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/auto/test_serialisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.815379 piccolo-1.6.0/tests/apps/migrations/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/commands/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/commands/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/commands/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/commands/test_forwards_backwards.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.815379 piccolo-1.6.0/tests/apps/migrations/commands/test_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/commands/test_migrations/2020-03-31T20-38-22.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/commands/test_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/commands/test_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/migrations/test_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.815379 piccolo-1.6.0/tests/apps/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.815379 piccolo-1.6.0/tests/apps/project/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/project/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/project/commands/test_new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.819379 piccolo-1.6.0/tests/apps/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.819379 piccolo-1.6.0/tests/apps/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.819379 piccolo-1.6.0/tests/apps/shell/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/shell/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/shell/commands/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.819379 piccolo-1.6.0/tests/apps/sql_shell/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/sql_shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.819379 piccolo-1.6.0/tests/apps/sql_shell/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/sql_shell/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/sql_shell/commands/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.819379 piccolo-1.6.0/tests/apps/tester/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/tester/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.819379 piccolo-1.6.0/tests/apps/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.819379 piccolo-1.6.0/tests/apps/user/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/user/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/user/commands/test_change_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/user/commands/test_change_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/user/commands/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/user/commands/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/apps/user/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.823379 piccolo-1.6.0/tests/columns/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.827379 piccolo-1.6.0/tests/columns/m2m/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/m2m/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/m2m/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/m2m/test_m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/m2m/test_m2m_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_bigint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_bytea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_combination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_db_column_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_double_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_jsonb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_primary_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_readable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_reserved_column_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_smallint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_timestamptz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/columns/test_varchar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.827379 piccolo-1.6.0/tests/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/conf/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/conf/test_apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.827379 piccolo-1.6.0/tests/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/engine/test_extra_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/engine/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/engine/test_nested_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/engine/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/engine/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/engine/test_version_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.827379 piccolo-1.6.0/tests/example_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/example_apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.827379 piccolo-1.6.0/tests/example_apps/mega/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/example_apps/mega/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/example_apps/mega/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.827379 piccolo-1.6.0/tests/example_apps/mega/piccolo_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/example_apps/mega/piccolo_migrations/2021-09-20T21-23-25-698988.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/example_apps/mega/piccolo_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/example_apps/mega/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.827379 piccolo-1.6.0/tests/example_apps/music/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/example_apps/music/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/example_apps/music/piccolo_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/example_apps/music/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/example_apps/music/tables_detailed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.831379 piccolo-1.6.0/tests/query/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.831379 piccolo-1.6.0/tests/query/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/mixins/test_columns_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/mixins/test_order_by_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/test_await.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/test_camelcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/test_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/test_gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/test_querystring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/query/test_slots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.835379 piccolo-1.6.0/tests/table/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.839379 piccolo-1.6.0/tests/table/instance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/instance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/instance/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/instance/test_get_related.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/instance/test_get_related_readable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/instance/test_instantiate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/instance/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/instance/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/instance/test_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_all_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_alter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_create_db_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_create_table_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_drop_db_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_from_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13695 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_insert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15910 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_join_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40390 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_table_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/table/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.839379 piccolo-1.6.0/tests/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/testing/test_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/testing/test_random_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:59.839379 piccolo-1.6.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_lazy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26623 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_sql_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_table_reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-30 00:16:23.000000 piccolo-1.6.0/tests/utils/test_warnings.py
```

### Comparing `piccolo-1.5.2/LICENSE` & `piccolo-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/PKG-INFO` & `piccolo-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piccolo
-Version: 1.5.2
+Version: 1.6.0
 Summary: A fast, user friendly ORM and query builder which supports asyncio.
 Home-page: https://github.com/piccolo-orm/piccolo
 Author: Daniel Townsend
 Author-email: dan@dantownsend.co.uk
 License: MIT
 Project-URL: Documentation, https://piccolo-orm.readthedocs.io/en/latest/index.html
 Project-URL: Source, https://github.com/piccolo-orm/piccolo
```

### Comparing `piccolo-1.5.2/README.md` & `piccolo-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/app/commands/new.py` & `piccolo-1.6.0/piccolo/apps/app/commands/new.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/app/commands/templates/piccolo_app.py.jinja` & `piccolo-1.6.0/piccolo/apps/app/commands/templates/piccolo_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/asgi/commands/new.py` & `piccolo-1.6.0/piccolo/apps/asgi/commands/new.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja` & `piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/_esmerald_app.py.jinja` & `piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_esmerald_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja` & `piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/_lilya_app.py.jinja` & `piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_lilya_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/_litestar_app.py.jinja` & `piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_litestar_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja` & `piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/home/_litestar_endpoints.py.jinja` & `piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/_litestar_endpoints.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw` & `piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/static/favicon.ico` & `piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/asgi/commands/templates/app/static/main.css` & `piccolo-1.6.0/piccolo/apps/asgi/commands/templates/app/static/main.css`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/fixtures/commands/dump.py` & `piccolo-1.6.0/piccolo/apps/fixtures/commands/dump.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/fixtures/commands/load.py` & `piccolo-1.6.0/piccolo/apps/fixtures/commands/load.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/fixtures/commands/shared.py` & `piccolo-1.6.0/piccolo/apps/fixtures/commands/shared.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/migrations/auto/diffable_table.py` & `piccolo-1.6.0/piccolo/apps/migrations/auto/diffable_table.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/migrations/auto/migration_manager.py` & `piccolo-1.6.0/piccolo/apps/migrations/auto/migration_manager.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/migrations/auto/operations.py` & `piccolo-1.6.0/piccolo/apps/migrations/auto/operations.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/migrations/auto/schema_differ.py` & `piccolo-1.6.0/piccolo/apps/migrations/auto/schema_differ.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/migrations/auto/schema_snapshot.py` & `piccolo-1.6.0/piccolo/apps/migrations/auto/schema_snapshot.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/migrations/auto/serialisation.py` & `piccolo-1.6.0/piccolo/apps/migrations/auto/serialisation.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/migrations/auto/serialisation_legacy.py` & `piccolo-1.6.0/piccolo/apps/migrations/auto/serialisation_legacy.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/migrations/commands/backwards.py` & `piccolo-1.6.0/piccolo/apps/migrations/commands/backwards.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/migrations/commands/base.py` & `piccolo-1.6.0/piccolo/apps/migrations/commands/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/migrations/commands/check.py` & `piccolo-1.6.0/piccolo/apps/migrations/commands/check.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/migrations/commands/clean.py` & `piccolo-1.6.0/piccolo/apps/migrations/commands/clean.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/migrations/commands/forwards.py` & `piccolo-1.6.0/piccolo/apps/migrations/commands/forwards.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/migrations/commands/new.py` & `piccolo-1.6.0/piccolo/apps/migrations/commands/new.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/migrations/commands/templates/migration.py.jinja` & `piccolo-1.6.0/piccolo/apps/migrations/commands/templates/migration.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/migrations/piccolo_app.py` & `piccolo-1.6.0/piccolo/apps/migrations/piccolo_app.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/migrations/tables.py` & `piccolo-1.6.0/piccolo/apps/migrations/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/playground/commands/run.py` & `piccolo-1.6.0/piccolo/apps/playground/commands/run.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/project/commands/new.py` & `piccolo-1.6.0/piccolo/apps/project/commands/new.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/schema/commands/generate.py` & `piccolo-1.6.0/piccolo/apps/schema/commands/generate.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/schema/commands/graph.py` & `piccolo-1.6.0/piccolo/apps/schema/commands/graph.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/schema/commands/templates/graphviz.dot.jinja` & `piccolo-1.6.0/piccolo/apps/schema/commands/templates/graphviz.dot.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/shell/commands/run.py` & `piccolo-1.6.0/piccolo/apps/shell/commands/run.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/sql_shell/commands/run.py` & `piccolo-1.6.0/piccolo/apps/sql_shell/commands/run.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/tester/commands/run.py` & `piccolo-1.6.0/piccolo/apps/tester/commands/run.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/user/commands/change_password.py` & `piccolo-1.6.0/piccolo/apps/user/commands/change_password.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/user/commands/change_permissions.py` & `piccolo-1.6.0/piccolo/apps/user/commands/change_permissions.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/user/commands/create.py` & `piccolo-1.6.0/piccolo/apps/user/commands/create.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/user/commands/list.py` & `piccolo-1.6.0/piccolo/apps/user/commands/list.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/user/piccolo_app.py` & `piccolo-1.6.0/piccolo/apps/user/piccolo_app.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/user/piccolo_migrations/2019-11-14T21-52-21.py` & `piccolo-1.6.0/piccolo/apps/user/piccolo_migrations/2019-11-14T21-52-21.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/user/piccolo_migrations/2020-06-11T21-38-55.py` & `piccolo-1.6.0/piccolo/apps/user/piccolo_migrations/2020-06-11T21-38-55.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/user/piccolo_migrations/2021-04-30T16-14-15.py` & `piccolo-1.6.0/piccolo/apps/user/piccolo_migrations/2021-04-30T16-14-15.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/apps/user/tables.py` & `piccolo-1.6.0/piccolo/apps/user/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/columns/__init__.py` & `piccolo-1.6.0/piccolo/columns/__init__.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/columns/base.py` & `piccolo-1.6.0/piccolo/columns/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import copy
 import datetime
 import decimal
 import inspect
 import typing as t
 import uuid
-from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass, field, fields
 from enum import Enum
 
 from piccolo.columns.choices import Choice
 from piccolo.columns.combination import Where
 from piccolo.columns.defaults.base import Default
 from piccolo.columns.defaults.interval import IntervalCustom
@@ -28,14 +27,15 @@
     LessThan,
     Like,
     NotEqual,
     NotIn,
     NotLike,
 )
 from piccolo.columns.reference import LazyTableReference
+from piccolo.querystring import QueryString, Selectable
 from piccolo.utils.warnings import colored_warning
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from piccolo.columns.column_types import ForeignKey
     from piccolo.table import Table
 
 
@@ -201,15 +201,14 @@
             )
         return self._table
 
     ###########################################################################
 
     # Used by Foreign Keys:
     call_chain: t.List["ForeignKey"] = field(default_factory=list)
-    table_alias: t.Optional[str] = None
 
     ###########################################################################
 
     @property
     def engine_type(self) -> str:
         engine = self.table._meta.db
         if engine:
@@ -256,27 +255,29 @@
 
         return column_name
 
     def _get_path(self, include_quotes: bool = False):
         column_name = self.db_column_name
 
         if self.call_chain:
-            table_alias = self.call_chain[-1]._meta.table_alias
+            table_alias = self.call_chain[-1].table_alias
             if include_quotes:
                 return f'"{table_alias}"."{column_name}"'
             else:
                 return f"{table_alias}.{column_name}"
         else:
             if include_quotes:
                 return f'"{self.table._meta.tablename}"."{column_name}"'
             else:
                 return f"{self.table._meta.tablename}.{column_name}"
 
     def get_full_name(
-        self, with_alias: bool = True, include_quotes: bool = True
+        self,
+        with_alias: bool = True,
+        include_quotes: bool = True,
     ) -> str:
         """
         Returns the full column name, taking into account joins.
 
         :param with_alias:
             Examples:
 
@@ -298,19 +299,18 @@
 
                 >>> column._meta.get_full_name(include_quotes=True)
                 '"my_table_name"."my_column_name"'
 
                 >>> column._meta.get_full_name(include_quotes=False)
                 'my_table_name.my_column_name'
 
-
         """
         full_name = self._get_path(include_quotes=include_quotes)
 
-        if with_alias and self.call_chain:
+        if with_alias:
             alias = self.get_default_alias()
             if include_quotes:
                 full_name += f' AS "{alias}"'
             else:
                 full_name += f" AS {alias}"
 
         return full_name
@@ -342,40 +342,14 @@
         """
         We override deepcopy, as it's too slow if it has to recreate
         everything.
         """
         return self.copy()
 
 
-class Selectable(metaclass=ABCMeta):
-    """
-    Anything which inherits from this can be used in a select query.
-    """
-
-    _alias: t.Optional[str]
-
-    @abstractmethod
-    def get_select_string(
-        self, engine_type: str, with_alias: bool = True
-    ) -> str:
-        """
-        In a query, what to output after the select statement - could be a
-        column name, a sub query, a function etc. For a column it will be the
-        column name.
-        """
-        raise NotImplementedError()
-
-    def as_alias(self, alias: str) -> Selectable:
-        """
-        Allows column names to be changed in the result of a select.
-        """
-        self._alias = alias
-        return self
-
-
 class Column(Selectable):
     """
     All other columns inherit from ``Column``. Don't use it directly.
 
     The following arguments apply to all column types:
 
     :param null:
@@ -818,33 +792,40 @@
             default = default.value if isinstance(default, Enum) else default
             is_callable = hasattr(default, "__call__")
             return default() if is_callable else default  # type: ignore
         return None
 
     def get_select_string(
         self, engine_type: str, with_alias: bool = True
-    ) -> str:
+    ) -> QueryString:
         """
         How to refer to this column in a SQL query, taking account of any joins
         and aliases.
         """
+
         if with_alias:
             if self._alias:
                 original_name = self._meta.get_full_name(
                     with_alias=False,
                 )
-                return f'{original_name} AS "{self._alias}"'
+                return QueryString(f'{original_name} AS "{self._alias}"')
             else:
-                return self._meta.get_full_name(
-                    with_alias=True,
+                return QueryString(
+                    self._meta.get_full_name(
+                        with_alias=True,
+                    )
                 )
 
-        return self._meta.get_full_name(with_alias=False)
+        return QueryString(
+            self._meta.get_full_name(
+                with_alias=False,
+            )
+        )
 
-    def get_where_string(self, engine_type: str) -> str:
+    def get_where_string(self, engine_type: str) -> QueryString:
         return self.get_select_string(
             engine_type=engine_type, with_alias=False
         )
 
     def get_sql_value(self, value: t.Any) -> t.Any:
         """
         When using DDL statements, we can't parameterise the values. An example
@@ -899,14 +880,21 @@
             return value
 
     @property
     def column_type(self):
         return self.__class__.__name__.upper()
 
     @property
+    def table_alias(self) -> str:
+        return "$".join(
+            f"{_key._meta.table._meta.tablename}${_key._meta.name}"
+            for _key in [*self._meta.call_chain, self]
+        )
+
+    @property
     def ddl(self) -> str:
         """
         Used when creating tables.
         """
         query = f'"{self._meta.db_column_name}" {self.column_type}'
         if self._meta.primary_key:
             query += " PRIMARY KEY"
@@ -941,16 +929,16 @@
         ) or self.__class__.__name__ not in ("Serial", "BigSerial"):
             default = self.get_default_value()
             sql_value = self.get_sql_value(value=default)
             query += f" DEFAULT {sql_value}"
 
         return query
 
-    def copy(self) -> Column:
-        column: Column = copy.copy(self)
+    def copy(self: Self) -> Self:
+        column = copy.copy(self)
         column._meta = self._meta.copy()
         return column
 
     def __deepcopy__(self, memo) -> Column:
         """
         We override deepcopy, as it's too slow if it has to recreate
         everything.
@@ -967,7 +955,10 @@
             table_class_name = "Unknown"
         else:
             table_class_name = table.__name__
         return (
             f"{table_class_name}.{self._meta.name} - "
             f"{self.__class__.__name__}"
         )
+
+
+Self = t.TypeVar("Self", bound=Column)
```

### Comparing `piccolo-1.5.2/piccolo/columns/choices.py` & `piccolo-1.6.0/piccolo/columns/choices.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/columns/column_types.py` & `piccolo-1.6.0/piccolo/columns/column_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     TimestamptzCustom,
     TimestamptzNow,
 )
 from piccolo.columns.defaults.uuid import UUID4, UUIDArg
 from piccolo.columns.operators.comparison import ArrayAll, ArrayAny
 from piccolo.columns.operators.string import Concat
 from piccolo.columns.reference import LazyTableReference
-from piccolo.querystring import QueryString, Unquoted
+from piccolo.querystring import QueryString
 from piccolo.utils.encoding import dump_json
 from piccolo.utils.warnings import colored_warning
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from piccolo.columns.base import ColumnMeta
     from piccolo.table import Table
 
@@ -748,16 +748,16 @@
     def __set__(self, obj, value: t.Union[int, None]):
         obj.__dict__[self._meta.name] = value
 
 
 ###############################################################################
 
 
-DEFAULT = Unquoted("DEFAULT")
-NULL = Unquoted("null")
+DEFAULT = QueryString("DEFAULT")
+NULL = QueryString("null")
 
 
 class Serial(Column):
     """
     An alias to an autoincrementing integer column in Postgres.
     """
 
@@ -774,15 +774,15 @@
 
     def default(self):
         engine_type = self._meta.engine_type
 
         if engine_type == "postgres":
             return DEFAULT
         elif engine_type == "cockroach":
-            return Unquoted("unique_rowid()")
+            return QueryString("unique_rowid()")
         elif engine_type == "sqlite":
             return NULL
         raise Exception("Unrecognized engine type")
 
     ###########################################################################
     # Descriptors
 
@@ -2190,14 +2190,15 @@
             return new_column
         elif issubclass(type(value), Column):
             new_column = value.copy()
 
             column_meta: ColumnMeta = object.__getattribute__(self, "_meta")
 
             new_column._meta.call_chain = column_meta.call_chain.copy()
+
             new_column._meta.call_chain.append(self)
             return new_column
         else:
             return value
 
     ###########################################################################
     # Descriptors
@@ -2307,25 +2308,25 @@
         """
         instance = t.cast(JSONB, self.copy())
         instance.json_operator = f"-> '{key}'"
         return instance
 
     def get_select_string(
         self, engine_type: str, with_alias: bool = True
-    ) -> str:
+    ) -> QueryString:
         select_string = self._meta.get_full_name(with_alias=False)
 
         if self.json_operator is not None:
             select_string += f" {self.json_operator}"
 
         if with_alias:
             alias = self._alias or self._meta.get_default_alias()
             select_string += f' AS "{alias}"'
 
-        return select_string
+        return QueryString(select_string)
 
     def eq(self, value) -> Where:
         """
         See ``Boolean.eq`` for more details.
         """
         return self.__eq__(value)
 
@@ -2612,25 +2613,27 @@
             # We deliberately add 1, as Postgres treats the first array element
             # as index 1.
             instance.index = value + 1
             return instance
         else:
             raise ValueError("Only integers can be used for indexing.")
 
-    def get_select_string(self, engine_type: str, with_alias=True) -> str:
+    def get_select_string(
+        self, engine_type: str, with_alias=True
+    ) -> QueryString:
         select_string = self._meta.get_full_name(with_alias=False)
 
         if isinstance(self.index, int):
             select_string += f"[{self.index}]"
 
         if with_alias:
             alias = self._alias or self._meta.get_default_alias()
             select_string += f' AS "{alias}"'
 
-        return select_string
+        return QueryString(select_string)
 
     def any(self, value: t.Any) -> Where:
         """
         Check if any of the items in the array match the given value.
 
         .. code-block:: python
```

### Comparing `piccolo-1.5.2/piccolo/columns/combination.py` & `piccolo-1.6.0/piccolo/columns/combination.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/columns/defaults/base.py` & `piccolo-1.6.0/piccolo/columns/defaults/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/columns/defaults/date.py` & `piccolo-1.6.0/piccolo/columns/defaults/date.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/columns/defaults/interval.py` & `piccolo-1.6.0/piccolo/columns/defaults/interval.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/columns/defaults/time.py` & `piccolo-1.6.0/piccolo/columns/defaults/time.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/columns/defaults/timestamp.py` & `piccolo-1.6.0/piccolo/columns/defaults/timestamp.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/columns/defaults/timestamptz.py` & `piccolo-1.6.0/piccolo/columns/defaults/timestamptz.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/columns/m2m.py` & `piccolo-1.6.0/piccolo/columns/m2m.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import inspect
 import typing as t
 from dataclasses import dataclass
 
-from piccolo.columns.base import Selectable
 from piccolo.columns.column_types import (
     JSON,
     JSONB,
     Column,
     ForeignKey,
     LazyTableReference,
 )
+from piccolo.querystring import QueryString, Selectable
 from piccolo.utils.list import flatten
 from piccolo.utils.sync import run_sync
 
 if t.TYPE_CHECKING:
     from piccolo.table import Table
 
 
@@ -52,15 +52,17 @@
         # can fetch the data all in one go.
         self.serialisation_safe = all(
             (column.__class__.value_type in safe_types)
             and (type(column) not in (JSON, JSONB))
             for column in columns
         )
 
-    def get_select_string(self, engine_type: str, with_alias=True) -> str:
+    def get_select_string(
+        self, engine_type: str, with_alias=True
+    ) -> QueryString:
         m2m_table_name_with_schema = (
             self.m2m._meta.resolved_joining_table._meta.get_formatted_tablename()  # noqa: E501
         )  # noqa: E501
         m2m_relationship_name = self.m2m._meta.name
 
         fk_1 = self.m2m._meta.primary_foreign_key
         fk_1_name = fk_1._meta.db_column_name
@@ -86,58 +88,66 @@
             )
             WHERE {m2m_table_name_with_schema}."{fk_1_name}" = "{table_1_name}"."{table_1_pk_name}"
         """  # noqa: E501
 
         if engine_type in ("postgres", "cockroach"):
             if self.as_list:
                 column_name = self.columns[0]._meta.db_column_name
-                return f"""
+                return QueryString(
+                    f"""
                     ARRAY(
                         SELECT
                             "inner_{table_2_name}"."{column_name}"
                         FROM {inner_select}
                     ) AS "{m2m_relationship_name}"
                 """
+                )
             elif not self.serialisation_safe:
                 column_name = table_2_pk_name
-                return f"""
+                return QueryString(
+                    f"""
                     ARRAY(
                         SELECT
                             "inner_{table_2_name}"."{column_name}"
                         FROM {inner_select}
                     ) AS "{m2m_relationship_name}"
                 """
+                )
             else:
                 column_names = ", ".join(
                     f'"inner_{table_2_name}"."{column._meta.db_column_name}"'
                     for column in self.columns
                 )
-                return f"""
+                return QueryString(
+                    f"""
                     (
                         SELECT JSON_AGG({m2m_relationship_name}_results)
                         FROM (
                             SELECT {column_names} FROM {inner_select}
                         ) AS "{m2m_relationship_name}_results"
                     ) AS "{m2m_relationship_name}"
                 """
+                )
         elif engine_type == "sqlite":
             if len(self.columns) > 1 or not self.serialisation_safe:
                 column_name = table_2_pk_name
             else:
                 column_name = self.columns[0]._meta.db_column_name
 
-            return f"""
+            return QueryString(
+                f"""
                 (
                     SELECT group_concat(
                         "inner_{table_2_name}"."{column_name}"
                     )
                     FROM {inner_select}
                 )
                 AS "{m2m_relationship_name} [M2M]"
             """
+            )
         else:
             raise ValueError(f"{engine_type} is an unrecognised engine type")
 
 
 @dataclass
 class M2MMeta:
     joining_table: t.Union[t.Type[Table], LazyTableReference]
```

### Comparing `piccolo-1.5.2/piccolo/columns/operators/comparison.py` & `piccolo-1.6.0/piccolo/columns/operators/comparison.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/columns/readable.py` & `piccolo-1.6.0/piccolo/columns/readable.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import typing as t
 from dataclasses import dataclass
 
-from piccolo.columns.base import Selectable
+from piccolo.querystring import QueryString, Selectable
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from piccolo.columns.base import Column
 
 
 @dataclass
 class Readable(Selectable):
@@ -23,32 +23,34 @@
 
     @property
     def _columns_string(self) -> str:
         return ", ".join(
             i._meta.get_full_name(with_alias=False) for i in self.columns
         )
 
-    def _get_string(self, operator: str) -> str:
-        return (
+    def _get_string(self, operator: str) -> QueryString:
+        return QueryString(
             f"{operator}('{self.template}', {self._columns_string}) AS "
             f"{self.output_name}"
         )
 
     @property
-    def sqlite_string(self) -> str:
+    def sqlite_string(self) -> QueryString:
         return self._get_string(operator="PRINTF")
 
     @property
-    def postgres_string(self) -> str:
+    def postgres_string(self) -> QueryString:
         return self._get_string(operator="FORMAT")
 
     @property
-    def cockroach_string(self) -> str:
+    def cockroach_string(self) -> QueryString:
         return self._get_string(operator="FORMAT")
 
-    def get_select_string(self, engine_type: str, with_alias=True) -> str:
+    def get_select_string(
+        self, engine_type: str, with_alias=True
+    ) -> QueryString:
         try:
             return getattr(self, f"{engine_type}_string")
         except AttributeError as e:
             raise ValueError(
                 f"Unrecognised engine_type - received {engine_type}"
             ) from e
```

### Comparing `piccolo-1.5.2/piccolo/columns/reference.py` & `piccolo-1.6.0/piccolo/columns/reference.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/conf/apps.py` & `piccolo-1.6.0/piccolo/conf/apps.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/custom_types.py` & `piccolo-1.6.0/piccolo/custom_types.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/engine/base.py` & `piccolo-1.6.0/piccolo/engine/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/engine/cockroach.py` & `piccolo-1.6.0/piccolo/engine/cockroach.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/engine/postgres.py` & `piccolo-1.6.0/piccolo/engine/postgres.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/engine/sqlite.py` & `piccolo-1.6.0/piccolo/engine/sqlite.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/main.py` & `piccolo-1.6.0/piccolo/main.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/query/base.py` & `piccolo-1.6.0/piccolo/query/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/query/methods/alter.py` & `piccolo-1.6.0/piccolo/query/methods/alter.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/query/methods/count.py` & `piccolo-1.6.0/piccolo/query/methods/count.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import typing as t
 
 from piccolo.custom_types import Combinable
 from piccolo.query.base import Query
-from piccolo.query.methods.select import Count as SelectCount
+from piccolo.query.functions.aggregate import Count as CountFunction
 from piccolo.query.mixins import WhereDelegate
 from piccolo.querystring import QueryString
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from piccolo.columns import Column
     from piccolo.table import Table
 
@@ -28,15 +28,15 @@
         self.column = column
         self._distinct = distinct
         self.where_delegate = WhereDelegate()
 
     ###########################################################################
     # Clauses
 
-    def where(self: Self, *where: Combinable) -> Self:
+    def where(self: Self, *where: t.Union[Combinable, QueryString]) -> Self:
         self.where_delegate.where(*where)
         return self
 
     def distinct(self: Self, columns: t.Optional[t.Sequence[Column]]) -> Self:
         self._distinct = columns
         return self
 
@@ -46,15 +46,15 @@
         return response[0]["count"]
 
     @property
     def default_querystrings(self) -> t.Sequence[QueryString]:
         table: t.Type[Table] = self.table
 
         query = table.select(
-            SelectCount(column=self.column, distinct=self._distinct)
+            CountFunction(column=self.column, distinct=self._distinct)
         )
 
         query.where_delegate._where = self.where_delegate._where
 
         return query.querystrings
```

### Comparing `piccolo-1.5.2/piccolo/query/methods/create.py` & `piccolo-1.6.0/piccolo/query/methods/create.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/query/methods/create_index.py` & `piccolo-1.6.0/piccolo/query/methods/create_index.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/query/methods/delete.py` & `piccolo-1.6.0/piccolo/query/methods/delete.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     def __init__(self, table: t.Type[Table], force: bool = False, **kwargs):
         super().__init__(table, **kwargs)
         self.force = force
         self.returning_delegate = ReturningDelegate()
         self.where_delegate = WhereDelegate()
 
-    def where(self: Self, *where: Combinable) -> Self:
+    def where(self: Self, *where: t.Union[Combinable, QueryString]) -> Self:
         self.where_delegate.where(*where)
         return self
 
     def returning(self: Self, *columns: Column) -> Self:
         self.returning_delegate.returning(columns)
         return self
```

### Comparing `piccolo-1.5.2/piccolo/query/methods/drop_index.py` & `piccolo-1.6.0/piccolo/query/methods/drop_index.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/query/methods/exists.py` & `piccolo-1.6.0/piccolo/query/methods/exists.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class Exists(Query[TableInstance, bool]):
     __slots__ = ("where_delegate",)
 
     def __init__(self, table: t.Type[TableInstance], **kwargs):
         super().__init__(table, **kwargs)
         self.where_delegate = WhereDelegate()
 
-    def where(self: Self, *where: Combinable) -> Self:
+    def where(self: Self, *where: t.Union[Combinable, QueryString]) -> Self:
         self.where_delegate.where(*where)
         return self
 
     async def response_handler(self, response) -> bool:
         # Convert to a bool - postgres returns True, and sqlite return 1.
         return bool(response[0]["exists"])
```

### Comparing `piccolo-1.5.2/piccolo/query/methods/indexes.py` & `piccolo-1.6.0/piccolo/query/methods/indexes.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/query/methods/insert.py` & `piccolo-1.6.0/piccolo/query/methods/insert.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/query/methods/objects.py` & `piccolo-1.6.0/piccolo/query/methods/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,15 +258,15 @@
                 _columns.append(self.table._meta.get_column_by_name(column))
             else:
                 _columns.append(column)
 
         self.order_by_delegate.order_by(*_columns, ascending=ascending)
         return self
 
-    def where(self: Self, *where: Combinable) -> Self:
+    def where(self: Self, *where: t.Union[Combinable, QueryString]) -> Self:
         self.where_delegate.where(*where)
         return self
 
     ###########################################################################
 
     def first(self: Self) -> First[TableInstance]:
         self.limit_delegate.limit(1)
```

### Comparing `piccolo-1.5.2/piccolo/query/methods/raw.py` & `piccolo-1.6.0/piccolo/query/methods/raw.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/query/methods/refresh.py` & `piccolo-1.6.0/piccolo/query/methods/refresh.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/query/methods/select.py` & `piccolo-1.6.0/piccolo/query/methods/select.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import decimal
 import itertools
 import typing as t
 from collections import OrderedDict
 
 from piccolo.columns import Column, Selectable
 from piccolo.columns.column_types import JSON, JSONB, PrimaryKey
 from piccolo.columns.m2m import M2MSelect
@@ -32,17 +31,16 @@
 from piccolo.utils.encoding import dump_json, load_json
 from piccolo.utils.warnings import colored_warning
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from piccolo.custom_types import Combinable
     from piccolo.table import Table  # noqa
 
-
-def is_numeric_column(column: Column) -> bool:
-    return column.value_type in (int, decimal.Decimal, float)
+# Here to avoid breaking changes - will be removed in the future.
+from piccolo.query.functions.aggregate import Count  # noqa: F401
 
 
 class SelectRaw(Selectable):
     def __init__(self, sql: str, *args: t.Any) -> None:
         """
         Execute raw SQL in your select query.
 
@@ -55,232 +53,16 @@
             [{'name': 'Pythonistas', 'log_popularity': 3.0}]
 
         """
         self.querystring = QueryString(sql, *args)
 
     def get_select_string(
         self, engine_type: str, with_alias: bool = True
-    ) -> str:
-        return self.querystring.__str__()
-
-
-class Avg(Selectable):
-    """
-    ``AVG()`` SQL function. Column type must be numeric to run the query.
-
-    .. code-block:: python
-
-        await Band.select(Avg(Band.popularity)).run()
-
-        # We can use an alias. These two are equivalent:
-
-        await Band.select(
-            Avg(Band.popularity, alias="popularity_avg")
-        ).run()
-
-        await Band.select(
-            Avg(Band.popularity).as_alias("popularity_avg")
-        ).run()
-
-    """
-
-    def __init__(self, column: Column, alias: str = "avg"):
-        if is_numeric_column(column):
-            self.column = column
-        else:
-            raise ValueError("Column type must be numeric to run the query.")
-        self._alias = alias
-
-    def get_select_string(
-        self, engine_type: str, with_alias: bool = True
-    ) -> str:
-        column_name = self.column._meta.get_full_name(with_alias=False)
-        return f'AVG({column_name}) AS "{self._alias}"'
-
-
-class Count(Selectable):
-    """
-    Used in ``Select`` queries, usually in conjunction with the ``group_by``
-    clause::
-
-        >>> await Band.select(
-        ...     Band.manager.name.as_alias('manager_name'),
-        ...     Count(alias='band_count')
-        ... ).group_by(Band.manager)
-        [{'manager_name': 'Guido', 'count': 1}, ...]
-
-    It can also be used without the ``group_by`` clause (though you may prefer
-    to the :meth:`Table.count <piccolo.table.Table.count>` method instead, as
-    it's more convenient)::
-
-        >>> await Band.select(Count())
-        [{'count': 3}]
-
-    """
-
-    def __init__(
-        self,
-        column: t.Optional[Column] = None,
-        distinct: t.Optional[t.Sequence[Column]] = None,
-        alias: str = "count",
-    ):
-        """
-        :param column:
-            If specified, the count is for non-null values in that column.
-        :param distinct:
-            If specified, the count is for distinct values in those columns.
-        :param alias:
-            The name of the value in the response::
-
-                # These two are equivalent:
-
-                await Band.select(
-                    Band.name, Count(alias="total")
-                ).group_by(Band.name)
-
-                await Band.select(
-                    Band.name,
-                    Count().as_alias("total")
-                ).group_by(Band.name)
-
-        """
-        if distinct and column:
-            raise ValueError("Only specify `column` or `distinct`")
-
-        self.column = column
-        self.distinct = distinct
-        self._alias = alias
-
-    def get_select_string(
-        self, engine_type: str, with_alias: bool = True
-    ) -> str:
-        expression: str
-
-        if self.distinct:
-            if engine_type == "sqlite":
-                # SQLite doesn't allow us to specify multiple columns, so
-                # instead we concatenate the values.
-                column_names = " || ".join(
-                    i._meta.get_full_name(with_alias=False)
-                    for i in self.distinct
-                )
-            else:
-                column_names = ", ".join(
-                    i._meta.get_full_name(with_alias=False)
-                    for i in self.distinct
-                )
-
-            expression = f"DISTINCT ({column_names})"
-        else:
-            if self.column:
-                expression = self.column._meta.get_full_name(with_alias=False)
-            else:
-                expression = "*"
-
-        return f'COUNT({expression}) AS "{self._alias}"'
-
-
-class Max(Selectable):
-    """
-    ``MAX()`` SQL function.
-
-    .. code-block:: python
-
-        await Band.select(
-            Max(Band.popularity)
-        ).run()
-
-        # We can use an alias. These two are equivalent:
-
-        await Band.select(
-            Max(Band.popularity, alias="popularity_max")
-        ).run()
-
-        await Band.select(
-            Max(Band.popularity).as_alias("popularity_max")
-        ).run()
-
-    """
-
-    def __init__(self, column: Column, alias: str = "max"):
-        self.column = column
-        self._alias = alias
-
-    def get_select_string(
-        self, engine_type: str, with_alias: bool = True
-    ) -> str:
-        column_name = self.column._meta.get_full_name(with_alias=False)
-        return f'MAX({column_name}) AS "{self._alias}"'
-
-
-class Min(Selectable):
-    """
-    ``MIN()`` SQL function.
-
-    .. code-block:: python
-
-        await Band.select(Min(Band.popularity)).run()
-
-        # We can use an alias. These two are equivalent:
-
-        await Band.select(
-            Min(Band.popularity, alias="popularity_min")
-        ).run()
-
-        await Band.select(
-            Min(Band.popularity).as_alias("popularity_min")
-        ).run()
-
-    """
-
-    def __init__(self, column: Column, alias: str = "min"):
-        self.column = column
-        self._alias = alias
-
-    def get_select_string(
-        self, engine_type: str, with_alias: bool = True
-    ) -> str:
-        column_name = self.column._meta.get_full_name(with_alias=False)
-        return f'MIN({column_name}) AS "{self._alias}"'
-
-
-class Sum(Selectable):
-    """
-    ``SUM()`` SQL function. Column type must be numeric to run the query.
-
-    .. code-block:: python
-
-        await Band.select(
-            Sum(Band.popularity)
-        ).run()
-
-        # We can use an alias. These two are equivalent:
-
-        await Band.select(
-            Sum(Band.popularity, alias="popularity_sum")
-        ).run()
-
-        await Band.select(
-            Sum(Band.popularity).as_alias("popularity_sum")
-        ).run()
-
-    """
-
-    def __init__(self, column: Column, alias: str = "sum"):
-        if is_numeric_column(column):
-            self.column = column
-        else:
-            raise ValueError("Column type must be numeric to run the query.")
-        self._alias = alias
-
-    def get_select_string(
-        self, engine_type: str, with_alias: bool = True
-    ) -> str:
-        column_name = self.column._meta.get_full_name(with_alias=False)
-        return f'SUM({column_name}) AS "{self._alias}"'
+    ) -> QueryString:
+        return self.querystring
 
 
 OptionalDict = t.Optional[t.Dict[str, t.Any]]
 
 
 class First(Proxy["Select", OptionalDict]):
     """
@@ -641,15 +423,15 @@
         callbacks: t.Union[t.Callable, t.List[t.Callable]],
         *,
         on: CallbackType = CallbackType.success,
     ) -> Self:
         self.callback_delegate.callback(callbacks, on=on)
         return self
 
-    def where(self: Self, *where: Combinable) -> Self:
+    def where(self: Self, *where: t.Union[Combinable, QueryString]) -> Self:
         self.where_delegate.where(*where)
         return self
 
     async def batch(
         self,
         batch_size: t.Optional[int] = None,
         node: t.Optional[str] = None,
@@ -674,31 +456,33 @@
             i for i in columns if isinstance(i, Readable)
         ]
 
         columns = list(columns)
         for readable in readables:
             columns += readable.columns
 
+        querystrings: t.List[QueryString] = [
+            i for i in columns if isinstance(i, QueryString)
+        ]
+        for querystring in querystrings:
+            if querystring_columns := getattr(querystring, "columns", []):
+                columns += querystring_columns
+
         for column in columns:
             if not isinstance(column, Column):
                 continue
 
             _joins: t.List[str] = []
             for index, key in enumerate(column._meta.call_chain, 0):
-                table_alias = "$".join(
-                    f"{_key._meta.table._meta.tablename}${_key._meta.name}"
-                    for _key in column._meta.call_chain[: index + 1]
-                )
-
-                key._meta.table_alias = table_alias
+                table_alias = key.table_alias
 
                 if index > 0:
                     left_tablename = column._meta.call_chain[
                         index - 1
-                    ]._meta.table_alias
+                    ].table_alias
                 else:
                     left_tablename = (
                         key._meta.table._meta.get_formatted_tablename()
                     )  # noqa: E501
 
                 right_tablename = (
                     key._foreign_key_meta.resolved_references._meta.get_formatted_tablename()  # noqa: E501
@@ -757,33 +541,34 @@
 
         # If secret fields need to be omitted, remove them from the list.
         if self.exclude_secrets:
             self.columns_delegate.remove_secret_columns()
 
         engine_type = self.table._meta.db.engine_type
 
-        select_strings: t.List[str] = [
+        select_strings: t.List[QueryString] = [
             c.get_select_string(engine_type=engine_type)
             for c in self.columns_delegate.selected_columns
         ]
-        columns_str = ", ".join(select_strings)
 
         #######################################################################
 
         args: t.List[t.Any] = []
 
         query = "SELECT"
 
         distinct = self.distinct_delegate._distinct
         if distinct.on:
             distinct.validate_on(self.order_by_delegate._order_by)
         query += "{}"
         args.append(distinct.querystring)
 
+        columns_str = ", ".join("{}" for i in select_strings)
         query += f" {columns_str} FROM {self.table._meta.get_formatted_tablename()}"  # noqa: E501
+        args.extend(select_strings)
 
         for join in joins:
             query += f" {join}"
 
         if self.as_of_delegate._as_of:
             query += "{}"
             args.append(self.as_of_delegate._as_of.querystring)
```

### Comparing `piccolo-1.5.2/piccolo/query/methods/table_exists.py` & `piccolo-1.6.0/piccolo/query/methods/table_exists.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/query/methods/update.py` & `piccolo-1.6.0/piccolo/query/methods/update.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     ) -> Update:
         if values is None:
             values = {}
         values = dict(values, **kwargs)
         self.values_delegate.values(values)
         return self
 
-    def where(self, *where: Combinable) -> Update:
+    def where(self, *where: t.Union[Combinable, QueryString]) -> Update:
         self.where_delegate.where(*where)
         return self
 
     def returning(self, *columns: Column) -> Update:
         self.returning_delegate.returning(columns)
         return self
```

### Comparing `piccolo-1.5.2/piccolo/query/mixins.py` & `piccolo-1.6.0/piccolo/query/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 import itertools
 import typing as t
 from dataclasses import dataclass, field
 from enum import Enum, auto
 
 from piccolo.columns import And, Column, Or, Where
 from piccolo.columns.column_types import ForeignKey
+from piccolo.columns.combination import WhereRaw
 from piccolo.custom_types import Combinable
 from piccolo.querystring import QueryString
 from piccolo.utils.list import flatten
 from piccolo.utils.sql_values import convert_to_sql_value
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from piccolo.columns.base import Selectable
+    from piccolo.querystring import Selectable
     from piccolo.table import Table  # noqa
 
 
 class DistinctOnError(ValueError):
     """
     Raised when ``DISTINCT ON`` queries are malformed.
     """
@@ -250,25 +251,31 @@
 
     def _extract_columns(self, combinable: Combinable):
         if isinstance(combinable, Where):
             self._where_columns.append(combinable.column)
         elif isinstance(combinable, (And, Or)):
             self._extract_columns(combinable.first)
             self._extract_columns(combinable.second)
+        elif isinstance(combinable, WhereRaw):
+            self._where_columns.extend(combinable.querystring.columns)
 
-    def where(self, *where: Combinable):
+    def where(self, *where: t.Union[Combinable, QueryString]):
         for arg in where:
             if isinstance(arg, bool):
                 raise ValueError(
                     "A boolean value has been passed in to a where clause. "
                     "This is probably a mistake. For example "
                     "`.where(MyTable.some_column is None)` instead of "
                     "`.where(MyTable.some_column.is_null())`."
                 )
 
+            if isinstance(arg, QueryString):
+                # If a raw QueryString is passed in.
+                arg = WhereRaw(arg.template, *arg.args)
+
             self._where = And(self._where, arg) if self._where else arg
 
 
 @dataclass
 class OrderByDelegate:
 
     _order_by: OrderBy = field(default_factory=OrderBy)
```

### Comparing `piccolo-1.5.2/piccolo/query/proxy.py` & `piccolo-1.6.0/piccolo/query/proxy.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/schema.py` & `piccolo-1.6.0/piccolo/schema.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/table.py` & `piccolo-1.6.0/piccolo/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,23 +44,23 @@
     TableExists,
     Update,
 )
 from piccolo.query.methods.create_index import CreateIndex
 from piccolo.query.methods.indexes import Indexes
 from piccolo.query.methods.objects import First
 from piccolo.query.methods.refresh import Refresh
-from piccolo.querystring import QueryString, Unquoted
+from piccolo.querystring import QueryString
 from piccolo.utils import _camel_to_snake
 from piccolo.utils.graphlib import TopologicalSorter
 from piccolo.utils.sql_values import convert_to_sql_value
 from piccolo.utils.sync import run_sync
 from piccolo.utils.warnings import colored_warning
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from piccolo.columns import Selectable
+    from piccolo.querystring import Selectable
 
 PROTECTED_TABLENAMES = ("user",)
 TABLENAME_WARNING = (
     "We recommend giving your table a different name as `{tablename}` is a "
     "reserved keyword. It should still work, but avoid if possible."
 )
 
@@ -792,38 +792,22 @@
     ###########################################################################
 
     @property
     def querystring(self) -> QueryString:
         """
         Used when inserting rows.
         """
-        args_dict = {}
-        for col in self._meta.columns:
-            column_name = col._meta.name
-            value = convert_to_sql_value(value=self[column_name], column=col)
-            args_dict[column_name] = value
-
-        def is_unquoted(arg):
-            return isinstance(arg, Unquoted)
-
-        # Strip out any args which are unquoted.
-        filtered_args = [i for i in args_dict.values() if not is_unquoted(i)]
+        args = [
+            convert_to_sql_value(value=self[column._meta.name], column=column)
+            for column in self._meta.columns
+        ]
 
         # If unquoted, dump it straight into the query.
-        query = ",".join(
-            [
-                (
-                    args_dict[column._meta.name].value
-                    if is_unquoted(args_dict[column._meta.name])
-                    else "{}"
-                )
-                for column in self._meta.columns
-            ]
-        )
-        return QueryString(f"({query})", *filtered_args)
+        query = ",".join(["{}" for _ in args])
+        return QueryString(f"({query})", *args)
 
     def __str__(self) -> str:
         return self.querystring.__str__()
 
     def __repr__(self) -> str:
         pk = (
             None
```

### Comparing `piccolo-1.5.2/piccolo/table_reflection.py` & `piccolo-1.6.0/piccolo/table_reflection.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/testing/model_builder.py` & `piccolo-1.6.0/piccolo/testing/model_builder.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/testing/random_builder.py` & `piccolo-1.6.0/piccolo/testing/random_builder.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/utils/dictionary.py` & `piccolo-1.6.0/piccolo/utils/dictionary.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/utils/encoding.py` & `piccolo-1.6.0/piccolo/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/utils/graphlib/_graphlib.py` & `piccolo-1.6.0/piccolo/utils/graphlib/_graphlib.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/utils/lazy_loader.py` & `piccolo-1.6.0/piccolo/utils/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/utils/list.py` & `piccolo-1.6.0/piccolo/utils/list.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/utils/objects.py` & `piccolo-1.6.0/piccolo/utils/objects.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/utils/printing.py` & `piccolo-1.6.0/piccolo/utils/printing.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/utils/pydantic.py` & `piccolo-1.6.0/piccolo/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/utils/repr.py` & `piccolo-1.6.0/piccolo/utils/repr.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/utils/sql_values.py` & `piccolo-1.6.0/piccolo/utils/sql_values.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/utils/sync.py` & `piccolo-1.6.0/piccolo/utils/sync.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo/utils/warnings.py` & `piccolo-1.6.0/piccolo/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/piccolo.egg-info/PKG-INFO` & `piccolo-1.6.0/piccolo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piccolo
-Version: 1.5.2
+Version: 1.6.0
 Summary: A fast, user friendly ORM and query builder which supports asyncio.
 Home-page: https://github.com/piccolo-orm/piccolo
 Author: Daniel Townsend
 Author-email: dan@dantownsend.co.uk
 License: MIT
 Project-URL: Documentation, https://piccolo-orm.readthedocs.io/en/latest/index.html
 Project-URL: Source, https://github.com/piccolo-orm/piccolo
```

### Comparing `piccolo-1.5.2/piccolo.egg-info/SOURCES.txt` & `piccolo-1.6.0/piccolo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,18 @@
 piccolo/engine/finder.py
 piccolo/engine/postgres.py
 piccolo/engine/sqlite.py
 piccolo/query/__init__.py
 piccolo/query/base.py
 piccolo/query/mixins.py
 piccolo/query/proxy.py
+piccolo/query/functions/__init__.py
+piccolo/query/functions/aggregate.py
+piccolo/query/functions/base.py
+piccolo/query/functions/string.py
 piccolo/query/methods/__init__.py
 piccolo/query/methods/alter.py
 piccolo/query/methods/count.py
 piccolo/query/methods/create.py
 piccolo/query/methods/create_index.py
 piccolo/query/methods/delete.py
 piccolo/query/methods/drop_index.py
@@ -299,14 +303,15 @@
 tests/example_apps/music/piccolo_app.py
 tests/example_apps/music/tables.py
 tests/example_apps/music/tables_detailed.py
 tests/query/__init__.py
 tests/query/test_await.py
 tests/query/test_camelcase.py
 tests/query/test_freeze.py
+tests/query/test_functions.py
 tests/query/test_gather.py
 tests/query/test_querystring.py
 tests/query/test_slots.py
 tests/query/mixins/__init__.py
 tests/query/mixins/test_columns_delegate.py
 tests/query/mixins/test_order_by_delegate.py
 tests/table/__init__.py
```

### Comparing `piccolo-1.5.2/profiling/run_profile.py` & `piccolo-1.6.0/profiling/run_profile.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/pyproject.toml` & `piccolo-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/setup.py` & `piccolo-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/app/commands/test_new.py` & `piccolo-1.6.0/tests/apps/app/commands/test_new.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/app/commands/test_show_all.py` & `piccolo-1.6.0/tests/apps/app/commands/test_show_all.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/asgi/commands/test_new.py` & `piccolo-1.6.0/tests/apps/asgi/commands/test_new.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/fixtures/commands/test_dump_load.py` & `piccolo-1.6.0/tests/apps/fixtures/commands/test_dump_load.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/fixtures/commands/test_shared.py` & `piccolo-1.6.0/tests/apps/fixtures/commands/test_shared.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/migrations/auto/integration/test_migrations.py` & `piccolo-1.6.0/tests/apps/migrations/auto/integration/test_migrations.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/migrations/auto/test_diffable_table.py` & `piccolo-1.6.0/tests/apps/migrations/auto/test_diffable_table.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/migrations/auto/test_migration_manager.py` & `piccolo-1.6.0/tests/apps/migrations/auto/test_migration_manager.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/migrations/auto/test_schema_differ.py` & `piccolo-1.6.0/tests/apps/migrations/auto/test_schema_differ.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/migrations/auto/test_schema_snapshot.py` & `piccolo-1.6.0/tests/apps/migrations/auto/test_schema_snapshot.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/migrations/auto/test_serialisation.py` & `piccolo-1.6.0/tests/apps/migrations/auto/test_serialisation.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/migrations/commands/test_base.py` & `piccolo-1.6.0/tests/apps/migrations/commands/test_base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/migrations/commands/test_check.py` & `piccolo-1.6.0/tests/apps/migrations/commands/test_check.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/migrations/commands/test_clean.py` & `piccolo-1.6.0/tests/apps/migrations/commands/test_clean.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/migrations/commands/test_forwards_backwards.py` & `piccolo-1.6.0/tests/apps/migrations/commands/test_forwards_backwards.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/migrations/commands/test_migrations/2020-03-31T20-38-22.py` & `piccolo-1.6.0/tests/apps/migrations/commands/test_migrations/2020-03-31T20-38-22.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/migrations/commands/test_new.py` & `piccolo-1.6.0/tests/apps/migrations/commands/test_new.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/shell/commands/test_run.py` & `piccolo-1.6.0/tests/apps/shell/commands/test_run.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/user/commands/test_change_password.py` & `piccolo-1.6.0/tests/apps/user/commands/test_change_password.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/user/commands/test_change_permissions.py` & `piccolo-1.6.0/tests/apps/user/commands/test_change_permissions.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/user/commands/test_create.py` & `piccolo-1.6.0/tests/apps/user/commands/test_create.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/user/commands/test_list.py` & `piccolo-1.6.0/tests/apps/user/commands/test_list.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/apps/user/test_tables.py` & `piccolo-1.6.0/tests/apps/user/test_tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/m2m/base.py` & `piccolo-1.6.0/tests/columns/m2m/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/m2m/test_m2m.py` & `piccolo-1.6.0/tests/columns/m2m/test_m2m.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_array.py` & `piccolo-1.6.0/tests/columns/test_array.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_base.py` & `piccolo-1.6.0/tests/columns/test_base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_bigint.py` & `piccolo-1.6.0/tests/columns/test_bigint.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_boolean.py` & `piccolo-1.6.0/tests/columns/test_boolean.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_bytea.py` & `piccolo-1.6.0/tests/columns/test_bytea.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_choices.py` & `piccolo-1.6.0/tests/columns/test_choices.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_combination.py` & `piccolo-1.6.0/tests/columns/test_combination.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_date.py` & `piccolo-1.6.0/tests/columns/test_date.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_db_column_name.py` & `piccolo-1.6.0/tests/columns/test_db_column_name.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_defaults.py` & `piccolo-1.6.0/tests/columns/test_defaults.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_double_precision.py` & `piccolo-1.6.0/tests/columns/test_double_precision.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_interval.py` & `piccolo-1.6.0/tests/columns/test_interval.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_json.py` & `piccolo-1.6.0/tests/columns/test_json.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_jsonb.py` & `piccolo-1.6.0/tests/columns/test_jsonb.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_numeric.py` & `piccolo-1.6.0/tests/columns/test_numeric.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_primary_key.py` & `piccolo-1.6.0/tests/columns/test_primary_key.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_readable.py` & `piccolo-1.6.0/tests/columns/test_readable.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_real.py` & `piccolo-1.6.0/tests/columns/test_real.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_reference.py` & `piccolo-1.6.0/tests/columns/test_reference.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_reserved_column_names.py` & `piccolo-1.6.0/tests/columns/test_reserved_column_names.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_smallint.py` & `piccolo-1.6.0/tests/columns/test_smallint.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_time.py` & `piccolo-1.6.0/tests/columns/test_time.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_timestamp.py` & `piccolo-1.6.0/tests/columns/test_timestamp.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_timestamptz.py` & `piccolo-1.6.0/tests/columns/test_timestamptz.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/columns/test_varchar.py` & `piccolo-1.6.0/tests/columns/test_varchar.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/conf/test_apps.py` & `piccolo-1.6.0/tests/conf/test_apps.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/engine/test_extra_nodes.py` & `piccolo-1.6.0/tests/engine/test_extra_nodes.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/engine/test_logging.py` & `piccolo-1.6.0/tests/engine/test_logging.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/engine/test_nested_transaction.py` & `piccolo-1.6.0/tests/engine/test_nested_transaction.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/engine/test_pool.py` & `piccolo-1.6.0/tests/engine/test_pool.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/engine/test_transaction.py` & `piccolo-1.6.0/tests/engine/test_transaction.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/engine/test_version_parsing.py` & `piccolo-1.6.0/tests/engine/test_version_parsing.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/example_apps/mega/piccolo_migrations/2021-09-20T21-23-25-698988.py` & `piccolo-1.6.0/tests/example_apps/mega/piccolo_migrations/2021-09-20T21-23-25-698988.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/example_apps/mega/tables.py` & `piccolo-1.6.0/tests/example_apps/mega/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/example_apps/music/tables.py` & `piccolo-1.6.0/tests/example_apps/music/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/example_apps/music/tables_detailed.py` & `piccolo-1.6.0/tests/example_apps/music/tables_detailed.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/query/mixins/test_columns_delegate.py` & `piccolo-1.6.0/tests/query/mixins/test_columns_delegate.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/query/test_camelcase.py` & `piccolo-1.6.0/tests/query/test_camelcase.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/query/test_freeze.py` & `piccolo-1.6.0/tests/query/test_freeze.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/query/test_gather.py` & `piccolo-1.6.0/tests/query/test_gather.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/query/test_querystring.py` & `piccolo-1.6.0/tests/query/test_querystring.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/query/test_slots.py` & `piccolo-1.6.0/tests/query/test_slots.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/instance/test_create.py` & `piccolo-1.6.0/tests/table/instance/test_create.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/instance/test_get_related.py` & `piccolo-1.6.0/tests/table/instance/test_get_related.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/instance/test_get_related_readable.py` & `piccolo-1.6.0/tests/table/instance/test_get_related_readable.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/instance/test_instantiate.py` & `piccolo-1.6.0/tests/table/instance/test_instantiate.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/instance/test_remove.py` & `piccolo-1.6.0/tests/table/instance/test_remove.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/instance/test_save.py` & `piccolo-1.6.0/tests/table/instance/test_save.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/instance/test_to_dict.py` & `piccolo-1.6.0/tests/table/instance/test_to_dict.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_all_columns.py` & `piccolo-1.6.0/tests/table/test_all_columns.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_alter.py` & `piccolo-1.6.0/tests/table/test_alter.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_batch.py` & `piccolo-1.6.0/tests/table/test_batch.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_callback.py` & `piccolo-1.6.0/tests/table/test_callback.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_constructor.py` & `piccolo-1.6.0/tests/table/test_constructor.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_count.py` & `piccolo-1.6.0/tests/table/test_count.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_create.py` & `piccolo-1.6.0/tests/table/test_create.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_create_db_tables.py` & `piccolo-1.6.0/tests/table/test_create_db_tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_create_table_class.py` & `piccolo-1.6.0/tests/table/test_create_table_class.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_delete.py` & `piccolo-1.6.0/tests/table/test_delete.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_drop_db_tables.py` & `piccolo-1.6.0/tests/table/test_drop_db_tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_from_dict.py` & `piccolo-1.6.0/tests/table/test_from_dict.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_indexes.py` & `piccolo-1.6.0/tests/table/test_indexes.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_inheritance.py` & `piccolo-1.6.0/tests/table/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_insert.py` & `piccolo-1.6.0/tests/table/test_insert.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_join.py` & `piccolo-1.6.0/tests/table/test_join.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_join_on.py` & `piccolo-1.6.0/tests/table/test_join_on.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_metaclass.py` & `piccolo-1.6.0/tests/table/test_metaclass.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_objects.py` & `piccolo-1.6.0/tests/table/test_objects.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_output.py` & `piccolo-1.6.0/tests/table/test_output.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_raw.py` & `piccolo-1.6.0/tests/table/test_raw.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_refresh.py` & `piccolo-1.6.0/tests/table/test_refresh.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_select.py` & `piccolo-1.6.0/tests/table/test_select.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 import pytest
 
 from piccolo.apps.user.tables import BaseUser
 from piccolo.columns import Date, Varchar
 from piccolo.columns.combination import WhereRaw
 from piccolo.query import OrderByRaw
-from piccolo.query.methods.select import Avg, Count, Max, Min, SelectRaw, Sum
+from piccolo.query.functions.aggregate import Avg, Count, Max, Min, Sum
+from piccolo.query.methods.select import SelectRaw
 from piccolo.query.mixins import DistinctOnError
 from piccolo.table import Table, create_db_tables_sync, drop_db_tables_sync
 from tests.base import (
     DBTestCase,
     engine_is,
     engine_version_lt,
     engines_only,
@@ -923,22 +924,14 @@
             .run_sync()
         )
         assert response is not None
 
         self.assertEqual(float(response["popularity_avg"]), 1003.3333333333334)
         self.assertEqual(response["popularity_sum"], 3010)
 
-    def test_avg_validation(self):
-        with self.assertRaises(ValueError):
-            Band.select(Avg(Band.name)).run_sync()
-
-    def test_sum_validation(self):
-        with self.assertRaises(ValueError):
-            Band.select(Sum(Band.name)).run_sync()
-
     def test_columns(self):
         """
         Make sure the colums method can be used to specify which columns to
         query.
         """
         self.insert_rows()
```

### Comparing `piccolo-1.5.2/tests/table/test_str.py` & `piccolo-1.6.0/tests/table/test_str.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_table_exists.py` & `piccolo-1.6.0/tests/table/test_table_exists.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/table/test_update.py` & `piccolo-1.6.0/tests/table/test_update.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/test_schema.py` & `piccolo-1.6.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/testing/test_model_builder.py` & `piccolo-1.6.0/tests/testing/test_model_builder.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/testing/test_random_builder.py` & `piccolo-1.6.0/tests/testing/test_random_builder.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/utils/test_dictionary.py` & `piccolo-1.6.0/tests/utils/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/utils/test_lazy_loader.py` & `piccolo-1.6.0/tests/utils/test_lazy_loader.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/utils/test_list.py` & `piccolo-1.6.0/tests/utils/test_list.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/utils/test_naming.py` & `piccolo-1.6.0/tests/utils/test_naming.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/utils/test_printing.py` & `piccolo-1.6.0/tests/utils/test_printing.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/utils/test_pydantic.py` & `piccolo-1.6.0/tests/utils/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/utils/test_sql_values.py` & `piccolo-1.6.0/tests/utils/test_sql_values.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/utils/test_sync.py` & `piccolo-1.6.0/tests/utils/test_sync.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.2/tests/utils/test_table_reflection.py` & `piccolo-1.6.0/tests/utils/test_table_reflection.py`

 * *Files identical despite different names*

