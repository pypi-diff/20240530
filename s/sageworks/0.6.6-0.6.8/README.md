# Comparing `tmp/sageworks-0.6.6.tar.gz` & `tmp/sageworks-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sageworks-0.6.6.tar", last modified: Fri May 24 14:49:47 2024, max compression
+gzip compressed data, was "sageworks-0.6.8.tar", last modified: Thu May 30 17:23:31 2024, max compression
```

## Comparing `sageworks-0.6.6.tar` & `sageworks-0.6.8.tar`

### file list

```diff
@@ -1,565 +1,569 @@
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.850116 sageworks-0.6.6/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.756734 sageworks-0.6.6/.github/
--rw-r--r--   0 briford    (501) staff       (20)     1338 2024-03-28 17:23:43.000000 sageworks-0.6.6/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 briford    (501) staff       (20)      499 2023-12-24 17:18:24.000000 sageworks-0.6.6/.github/dependabot.yml
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.757215 sageworks-0.6.6/.github/workflows/
--rw-r--r--   0 briford    (501) staff       (20)      598 2024-01-10 18:45:51.000000 sageworks-0.6.6/.github/workflows/deploy-docs.yml
--rw-r--r--   0 briford    (501) staff       (20)      556 2024-01-23 15:36:53.000000 sageworks-0.6.6/.github/workflows/python-lint.yml
--rw-r--r--   0 briford    (501) staff       (20)     2037 2024-05-15 21:28:12.000000 sageworks-0.6.6/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)      791 2024-04-16 15:58:18.000000 sageworks-0.6.6/CONTRIBUTING.md
--rw-r--r--   0 briford    (501) staff       (20)      102 2024-03-28 17:23:43.000000 sageworks-0.6.6/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)     1080 2024-03-28 17:23:43.000000 sageworks-0.6.6/LICENSE
--rw-r--r--   0 briford    (501) staff       (20)     1426 2023-12-24 17:18:24.000000 sageworks-0.6.6/Makefile
--rw-r--r--   0 briford    (501) staff       (20)     4961 2024-05-24 14:49:47.850048 sageworks-0.6.6/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)     3510 2024-05-09 14:32:45.000000 sageworks-0.6.6/README.md
--rw-r--r--   0 briford    (501) staff       (20)      463 2023-12-24 17:18:24.000000 sageworks-0.6.6/SECURITY.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.745838 sageworks-0.6.6/applications/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.759456 sageworks-0.6.6/applications/aws_dashboard/
--rw-r--r--   0 briford    (501) staff       (20)     1071 2024-05-19 21:38:50.000000 sageworks-0.6.6/applications/aws_dashboard/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)      331 2024-03-28 17:23:43.000000 sageworks-0.6.6/applications/aws_dashboard/Dockerfile_plugins
--rw-r--r--   0 briford    (501) staff       (20)      841 2024-01-10 18:45:51.000000 sageworks-0.6.6/applications/aws_dashboard/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1526 2024-04-09 14:37:33.000000 sageworks-0.6.6/applications/aws_dashboard/app.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.761005 sageworks-0.6.6/applications/aws_dashboard/assets/
--rw-r--r--   0 briford    (501) staff       (20)   232839 2024-04-06 16:51:44.000000 sageworks-0.6.6/applications/aws_dashboard/assets/bootstrap_darkly.min.css
--rw-r--r--   0 briford    (501) staff       (20)    14995 2024-04-06 16:51:44.000000 sageworks-0.6.6/applications/aws_dashboard/assets/default.css
--rw-r--r--   0 briford    (501) staff       (20)    10375 2024-04-16 15:58:18.000000 sageworks-0.6.6/applications/aws_dashboard/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)      732 2023-12-24 17:18:24.000000 sageworks-0.6.6/applications/aws_dashboard/assets/trash.png
--rwxr-xr-x   0 briford    (501) staff       (20)      637 2024-04-26 21:03:22.000000 sageworks-0.6.6/applications/aws_dashboard/dashboard
--rw-r--r--   0 briford    (501) staff       (20)      205 2023-12-24 17:18:24.000000 sageworks-0.6.6/applications/aws_dashboard/nginx.conf
--rw-r--r--   0 briford    (501) staff       (20)      684 2024-03-28 17:23:43.000000 sageworks-0.6.6/applications/aws_dashboard/open_source_config.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.745762 sageworks-0.6.6/applications/aws_dashboard/pages/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.761625 sageworks-0.6.6/applications/aws_dashboard/pages/data_sources/
--rw-r--r--   0 briford    (501) staff       (20)    11700 2024-04-16 15:58:18.000000 sageworks-0.6.6/applications/aws_dashboard/pages/data_sources/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2756 2024-03-28 17:23:43.000000 sageworks-0.6.6/applications/aws_dashboard/pages/data_sources/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2555 2024-03-28 17:23:43.000000 sageworks-0.6.6/applications/aws_dashboard/pages/data_sources/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.762328 sageworks-0.6.6/applications/aws_dashboard/pages/endpoints/
--rw-r--r--   0 briford    (501) staff       (20)     4212 2024-04-16 15:58:18.000000 sageworks-0.6.6/applications/aws_dashboard/pages/endpoints/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2677 2024-04-16 15:58:18.000000 sageworks-0.6.6/applications/aws_dashboard/pages/endpoints/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2458 2024-04-23 23:23:47.000000 sageworks-0.6.6/applications/aws_dashboard/pages/endpoints/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.763023 sageworks-0.6.6/applications/aws_dashboard/pages/feature_sets/
--rw-r--r--   0 briford    (501) staff       (20)    11614 2024-04-16 15:58:18.000000 sageworks-0.6.6/applications/aws_dashboard/pages/feature_sets/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2438 2024-03-28 17:23:43.000000 sageworks-0.6.6/applications/aws_dashboard/pages/feature_sets/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.6.6/applications/aws_dashboard/pages/feature_sets/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.763294 sageworks-0.6.6/applications/aws_dashboard/pages/license/
--rw-r--r--   0 briford    (501) staff       (20)     1531 2024-05-19 19:25:10.000000 sageworks-0.6.6/applications/aws_dashboard/pages/license/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.764003 sageworks-0.6.6/applications/aws_dashboard/pages/main/
--rw-r--r--   0 briford    (501) staff       (20)     4899 2024-04-06 16:51:44.000000 sageworks-0.6.6/applications/aws_dashboard/pages/main/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     3307 2024-05-19 19:21:21.000000 sageworks-0.6.6/applications/aws_dashboard/pages/main/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1844 2024-03-28 17:23:43.000000 sageworks-0.6.6/applications/aws_dashboard/pages/main/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.764647 sageworks-0.6.6/applications/aws_dashboard/pages/models/
--rw-r--r--   0 briford    (501) staff       (20)     3954 2024-04-23 23:23:47.000000 sageworks-0.6.6/applications/aws_dashboard/pages/models/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2234 2024-04-27 20:59:25.000000 sageworks-0.6.6/applications/aws_dashboard/pages/models/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2152 2024-04-23 23:23:47.000000 sageworks-0.6.6/applications/aws_dashboard/pages/models/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.765349 sageworks-0.6.6/applications/aws_dashboard/pages/pipelines/
--rw-r--r--   0 briford    (501) staff       (20)     1791 2024-04-26 21:07:33.000000 sageworks-0.6.6/applications/aws_dashboard/pages/pipelines/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2664 2024-04-26 20:07:24.000000 sageworks-0.6.6/applications/aws_dashboard/pages/pipelines/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1927 2024-04-26 21:04:41.000000 sageworks-0.6.6/applications/aws_dashboard/pages/pipelines/page.py
--rw-r--r--   0 briford    (501) staff       (20)      407 2024-05-19 21:33:27.000000 sageworks-0.6.6/applications/aws_dashboard/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)      457 2023-12-24 17:18:24.000000 sageworks-0.6.6/applications/aws_dashboard/supervisord.conf
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.745891 sageworks-0.6.6/applications/experiments/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.766707 sageworks-0.6.6/applications/experiments/compound_explorer/
--rw-r--r--   0 briford    (501) staff       (20)      181 2023-12-24 17:18:24.000000 sageworks-0.6.6/applications/experiments/compound_explorer/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)      360 2023-12-24 17:18:24.000000 sageworks-0.6.6/applications/experiments/compound_explorer/README.md
--rw-r--r--   0 briford    (501) staff       (20)     3082 2024-04-06 16:51:44.000000 sageworks-0.6.6/applications/experiments/compound_explorer/app.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.767195 sageworks-0.6.6/applications/experiments/compound_explorer/assets/
--rw-r--r--   0 briford    (501) staff       (20)    12861 2023-12-24 17:18:24.000000 sageworks-0.6.6/applications/experiments/compound_explorer/assets/custom.css
--rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.6.6/applications/experiments/compound_explorer/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)     7678 2024-04-16 15:58:18.000000 sageworks-0.6.6/applications/experiments/compound_explorer/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     4860 2024-03-28 17:23:43.000000 sageworks-0.6.6/applications/experiments/compound_explorer/layout.py
--rw-r--r--   0 briford    (501) staff       (20)       94 2023-12-24 17:18:24.000000 sageworks-0.6.6/applications/experiments/compound_explorer/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.767681 sageworks-0.6.6/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     3582 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/aws_account_check.py
--rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/aws_identity_check.py
--rw-r--r--   0 briford    (501) staff       (20)     2629 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/build_ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.767826 sageworks-0.6.6/aws_setup/event_bridge/
--rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/event_bridge/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.768483 sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/
--rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     1007 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/cdk.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.768713 sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/lambda/
--rw-r--r--   0 briford    (501) staff       (20)     1812 2024-01-10 18:45:51.000000 sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py
--rw-r--r--   0 briford    (501) staff       (20)     2599 2024-03-27 20:43:31.000000 sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.769881 sageworks-0.6.6/aws_setup/sageworks_core/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_core/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1028 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_core/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/sageworks_core/app.py
--rw-r--r--   0 briford    (501) staff       (20)     1998 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_core/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_core/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       53 2024-01-10 18:45:51.000000 sageworks-0.6.6/aws_setup/sageworks_core/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.770161 sageworks-0.6.6/aws_setup/sageworks_core/sageworks_core/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/aws_setup/sageworks_core/sageworks_core/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    23575 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_core/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.770504 sageworks-0.6.6/aws_setup/sageworks_core/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_core/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.770702 sageworks-0.6.6/aws_setup/sageworks_core/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_core/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      720 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.771961 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1907 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       47 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.772209 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7022 2024-04-24 21:53:47.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.772559 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.772773 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      565 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.773605 sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/
--rw-r--r--   0 briford    (501) staff       (20)      119 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1928 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       47 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.773848 sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     6849 2024-05-19 21:59:13.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.775137 sageworks-0.6.6/data/
--rw-r--r--   0 briford    (501) staff       (20)   191978 2023-12-24 17:18:24.000000 sageworks-0.6.6/data/abalone.csv
--rw-r--r--   0 briford    (501) staff       (20)     1515 2023-12-24 17:18:24.000000 sageworks-0.6.6/data/test_data.csv
--rw-r--r--   0 briford    (501) staff       (20)     2270 2023-12-24 17:18:24.000000 sageworks-0.6.6/data/test_data.json
--rw-r--r--   0 briford    (501) staff       (20)    12977 2024-01-10 18:45:51.000000 sageworks-0.6.6/data/wine_dataset.csv
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.775398 sageworks-0.6.6/docs/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.775639 sageworks-0.6.6/docs/admin/
--rw-r--r--   0 briford    (501) staff       (20)     2176 2024-04-16 15:58:18.000000 sageworks-0.6.6/docs/admin/docker_push.md
--rw-r--r--   0 briford    (501) staff       (20)     1633 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/admin/pypi_release.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.776778 sageworks-0.6.6/docs/api_classes/
--rw-r--r--   0 briford    (501) staff       (20)     3595 2024-01-23 15:36:53.000000 sageworks-0.6.6/docs/api_classes/data_source.md
--rw-r--r--   0 briford    (501) staff       (20)     5199 2024-03-28 17:23:43.000000 sageworks-0.6.6/docs/api_classes/endpoint.md
--rw-r--r--   0 briford    (501) staff       (20)     6299 2024-03-28 17:23:43.000000 sageworks-0.6.6/docs/api_classes/feature_set.md
--rw-r--r--   0 briford    (501) staff       (20)     5350 2024-04-06 16:51:44.000000 sageworks-0.6.6/docs/api_classes/meta.md
--rw-r--r--   0 briford    (501) staff       (20)     4356 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/api_classes/model.md
--rw-r--r--   0 briford    (501) staff       (20)     2218 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/api_classes/monitor.md
--rw-r--r--   0 briford    (501) staff       (20)     3549 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/api_classes/overview.md
--rw-r--r--   0 briford    (501) staff       (20)     4894 2024-04-19 15:50:50.000000 sageworks-0.6.6/docs/api_classes/pipelines.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.777785 sageworks-0.6.6/docs/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     1121 2024-03-28 17:23:43.000000 sageworks-0.6.6/docs/aws_setup/aws_access_management.md
--rw-r--r--   0 briford    (501) staff       (20)     5610 2024-05-06 14:50:56.000000 sageworks-0.6.6/docs/aws_setup/aws_tips_and_tricks.md
--rw-r--r--   0 briford    (501) staff       (20)     4210 2024-05-09 14:32:45.000000 sageworks-0.6.6/docs/aws_setup/core_stack.md
--rw-r--r--   0 briford    (501) staff       (20)     2075 2024-03-28 17:23:43.000000 sageworks-0.6.6/docs/aws_setup/dashboard_stack.md
--rw-r--r--   0 briford    (501) staff       (20)     7313 2024-05-15 23:47:50.000000 sageworks-0.6.6/docs/aws_setup/domain_cert_setup.md
--rw-r--r--   0 briford    (501) staff       (20)     2540 2024-01-23 15:36:53.000000 sageworks-0.6.6/docs/aws_setup/full_pipeline.md
--rw-r--r--   0 briford    (501) staff       (20)     3438 2024-05-09 14:20:27.000000 sageworks-0.6.6/docs/aws_setup/sso_setup.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.778289 sageworks-0.6.6/docs/blogs_research/
--rw-r--r--   0 briford    (501) staff       (20)      912 2024-03-28 17:23:43.000000 sageworks-0.6.6/docs/blogs_research/eda.md
--rw-r--r--   0 briford    (501) staff       (20)     2017 2024-03-28 17:23:43.000000 sageworks-0.6.6/docs/blogs_research/htg.md
--rw-r--r--   0 briford    (501) staff       (20)      802 2024-05-21 22:30:34.000000 sageworks-0.6.6/docs/blogs_research/index.md
--rw-r--r--   0 briford    (501) staff       (20)     1245 2024-05-21 22:34:16.000000 sageworks-0.6.6/docs/blogs_research/residual_analysis.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.778412 sageworks-0.6.6/docs/concepts/
--rw-r--r--   0 briford    (501) staff       (20)      907 2024-01-23 15:36:53.000000 sageworks-0.6.6/docs/concepts/model_monitoring.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.778545 sageworks-0.6.6/docs/core_classes/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.779545 sageworks-0.6.6/docs/core_classes/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      464 2024-01-23 15:36:53.000000 sageworks-0.6.6/docs/core_classes/artifacts/artifact.md
--rw-r--r--   0 briford    (501) staff       (20)      290 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/artifacts/athena_source.md
--rw-r--r--   0 briford    (501) staff       (20)      479 2024-01-23 15:36:53.000000 sageworks-0.6.6/docs/core_classes/artifacts/data_source_abstract.md
--rw-r--r--   0 briford    (501) staff       (20)      292 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/artifacts/endpoint_core.md
--rw-r--r--   0 briford    (501) staff       (20)      294 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/artifacts/feature_set_core.md
--rw-r--r--   0 briford    (501) staff       (20)      281 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/artifacts/model_core.md
--rw-r--r--   0 briford    (501) staff       (20)      289 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/artifacts/monitor_core.md
--rw-r--r--   0 briford    (501) staff       (20)      861 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/artifacts/overview.md
--rw-r--r--   0 briford    (501) staff       (20)     2119 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/overview.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.780612 sageworks-0.6.6/docs/core_classes/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      352 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/transforms/data_loaders_heavy.md
--rw-r--r--   0 briford    (501) staff       (20)      396 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/transforms/data_loaders_light.md
--rw-r--r--   0 briford    (501) staff       (20)      349 2024-03-28 17:23:43.000000 sageworks-0.6.6/docs/core_classes/transforms/data_to_features.md
--rw-r--r--   0 briford    (501) staff       (20)      265 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/transforms/features_to_model.md
--rw-r--r--   0 briford    (501) staff       (20)      264 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/transforms/model_to_endpoint.md
--rw-r--r--   0 briford    (501) staff       (20)     1177 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/transforms/overview.md
--rw-r--r--   0 briford    (501) staff       (20)      970 2024-01-23 15:36:53.000000 sageworks-0.6.6/docs/core_classes/transforms/pandas_transforms.md
--rw-r--r--   0 briford    (501) staff       (20)      521 2024-01-23 15:36:53.000000 sageworks-0.6.6/docs/core_classes/transforms/transform.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.781002 sageworks-0.6.6/docs/enterprise/
--rw-r--r--   0 briford    (501) staff       (20)     4075 2024-05-20 20:55:48.000000 sageworks-0.6.6/docs/enterprise/index.md
--rw-r--r--   0 briford    (501) staff       (20)      786 2024-04-28 17:52:09.000000 sageworks-0.6.6/docs/enterprise/project_branding.md
--rw-r--r--   0 briford    (501) staff       (20)      892 2024-04-28 18:00:11.000000 sageworks-0.6.6/docs/enterprise/themes.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.781138 sageworks-0.6.6/docs/getting_started/
--rw-r--r--   0 briford    (501) staff       (20)     1975 2024-05-09 14:38:45.000000 sageworks-0.6.6/docs/getting_started/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.781267 sageworks-0.6.6/docs/glue/
--rw-r--r--   0 briford    (501) staff       (20)     4837 2024-03-28 17:23:43.000000 sageworks-0.6.6/docs/glue/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.783544 sageworks-0.6.6/docs/images/
--rw-r--r--   0 briford    (501) staff       (20)   605827 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/big_spider.png
--rw-r--r--   0 briford    (501) staff       (20)    32320 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/graph_representation.png
--rw-r--r--   0 briford    (501) staff       (20)    15549 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/powered_aws_dark_blue.png
--rw-r--r--   0 briford    (501) staff       (20)    10003 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/powered_aws_transparent.png
--rw-r--r--   0 briford    (501) staff       (20)     6435 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/powered_aws_white.png
--rw-r--r--   0 briford    (501) staff       (20)    21174 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/powered_aws_with_tm_grey.png
--rw-r--r--   0 briford    (501) staff       (20)    51137 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/sageworks.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)    30017 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/scp.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)   381209 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/small_spider.png
--rw-r--r--   0 briford    (501) staff       (20)     3443 2024-05-09 14:20:27.000000 sageworks-0.6.6/docs/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.784371 sageworks-0.6.6/docs/misc/
--rw-r--r--   0 briford    (501) staff       (20)     2791 2024-03-28 17:23:43.000000 sageworks-0.6.6/docs/misc/faq.md
--rw-r--r--   0 briford    (501) staff       (20)     5069 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/misc/general_info.md
--rw-r--r--   0 briford    (501) staff       (20)      667 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/misc/sageworks_classes_concepts.md
--rw-r--r--   0 briford    (501) staff       (20)     1873 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/misc/scp_consulting.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.784679 sageworks-0.6.6/docs/plugins/
--rw-r--r--   0 briford    (501) staff       (20)     3361 2024-04-16 15:58:18.000000 sageworks-0.6.6/docs/plugins/index.md
--rw-r--r--   0 briford    (501) staff       (20)      750 2024-04-06 16:51:44.000000 sageworks-0.6.6/docs/plugins/plugin_api_changes.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.784820 sageworks-0.6.6/docs/repl/
--rw-r--r--   0 briford    (501) staff       (20)     2080 2024-05-09 14:40:59.000000 sageworks-0.6.6/docs/repl/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.784956 sageworks-0.6.6/examples/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.785118 sageworks-0.6.6/examples/ag-grid/
--rw-r--r--   0 briford    (501) staff       (20)      496 2024-04-06 16:51:44.000000 sageworks-0.6.6/examples/ag-grid/hello_world.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.786603 sageworks-0.6.6/examples/datasource/
--rw-r--r--   0 briford    (501) staff       (20)      326 2024-01-10 18:45:51.000000 sageworks-0.6.6/examples/datasource/datasource_from_df.py
--rw-r--r--   0 briford    (501) staff       (20)      332 2024-01-10 18:45:51.000000 sageworks-0.6.6/examples/datasource/datasource_from_s3.py
--rw-r--r--   0 briford    (501) staff       (20)      536 2024-01-23 15:36:53.000000 sageworks-0.6.6/examples/datasource/datasource_query.py
--rw-r--r--   0 briford    (501) staff       (20)      680 2024-01-23 15:36:53.000000 sageworks-0.6.6/examples/datasource/datasource_stats.py
--rw-r--r--   0 briford    (501) staff       (20)      223 2024-01-10 18:45:51.000000 sageworks-0.6.6/examples/datasource/datasource_to_featureset.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.787256 sageworks-0.6.6/examples/endpoint/
--rw-r--r--   0 briford    (501) staff       (20)      199 2024-01-10 18:45:51.000000 sageworks-0.6.6/examples/endpoint/endpoint_details.py
--rw-r--r--   0 briford    (501) staff       (20)      834 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/endpoint/endpoint_inference.py
--rw-r--r--   0 briford    (501) staff       (20)      481 2024-01-10 18:45:51.000000 sageworks-0.6.6/examples/endpoint/endpoint_metrics.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.787783 sageworks-0.6.6/examples/featureset/
--rw-r--r--   0 briford    (501) staff       (20)      744 2024-01-10 18:45:51.000000 sageworks-0.6.6/examples/featureset/featureset_eda.py
--rw-r--r--   0 briford    (501) staff       (20)      560 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/featureset/featureset_query.py
--rw-r--r--   0 briford    (501) staff       (20)      421 2024-03-27 20:32:26.000000 sageworks-0.6.6/examples/featureset/featureset_to_model.py
--rw-r--r--   0 briford    (501) staff       (20)     1534 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/full_ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.788612 sageworks-0.6.6/examples/glue/
--rw-r--r--   0 briford    (501) staff       (20)      580 2024-01-23 15:36:53.000000 sageworks-0.6.6/examples/glue/glue_hello_world.py
--rw-r--r--   0 briford    (501) staff       (20)      942 2024-01-23 15:36:53.000000 sageworks-0.6.6/examples/glue/glue_hello_world_with_log.py
--rw-r--r--   0 briford    (501) staff       (20)      686 2024-01-23 15:36:53.000000 sageworks-0.6.6/examples/glue/glue_load_s3_bucket.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.789137 sageworks-0.6.6/examples/meta/
--rw-r--r--   0 briford    (501) staff       (20)      363 2024-04-06 16:51:44.000000 sageworks-0.6.6/examples/meta/meta_list_endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      328 2024-04-06 16:51:44.000000 sageworks-0.6.6/examples/meta/meta_list_models.py
--rw-r--r--   0 briford    (501) staff       (20)      659 2024-04-06 16:51:44.000000 sageworks-0.6.6/examples/meta/meta_model_metrics.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.789623 sageworks-0.6.6/examples/model/
--rw-r--r--   0 briford    (501) staff       (20)      548 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/model/model_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)      312 2024-03-27 20:32:26.000000 sageworks-0.6.6/examples/model/model_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)      705 2024-05-08 21:58:54.000000 sageworks-0.6.6/examples/model/onboard_model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.790100 sageworks-0.6.6/examples/monitor/
--rw-r--r--   0 briford    (501) staff       (20)      400 2024-01-10 18:45:51.000000 sageworks-0.6.6/examples/monitor/monitor_setup.py
--rw-r--r--   0 briford    (501) staff       (20)      765 2024-01-10 18:45:51.000000 sageworks-0.6.6/examples/monitor/monitor_usage.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.791627 sageworks-0.6.6/examples/pipelines/
--rw-r--r--   0 briford    (501) staff       (20)     1000 2024-04-19 14:53:32.000000 sageworks-0.6.6/examples/pipelines/abalone_pipeline_v1.json
--rw-r--r--   0 briford    (501) staff       (20)     1073 2024-04-19 19:42:10.000000 sageworks-0.6.6/examples/pipelines/abalone_pipeline_v2.json
--rw-r--r--   0 briford    (501) staff       (20)     4435 2024-04-20 17:35:29.000000 sageworks-0.6.6/examples/pipelines/aqsol_pipeline_v1.json
--rw-r--r--   0 briford    (501) staff       (20)      142 2024-04-19 14:55:38.000000 sageworks-0.6.6/examples/pipelines/pipeline_details.py
--rw-r--r--   0 briford    (501) staff       (20)      324 2024-04-19 14:55:38.000000 sageworks-0.6.6/examples/pipelines/pipeline_execute.py
--rw-r--r--   0 briford    (501) staff       (20)      556 2024-04-19 14:51:51.000000 sageworks-0.6.6/examples/pipelines/pipeline_manager.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.749192 sageworks-0.6.6/examples/plugins/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.792517 sageworks-0.6.6/examples/plugins/pages/
--rw-r--r--   0 briford    (501) staff       (20)     2467 2024-04-09 15:13:19.000000 sageworks-0.6.6/examples/plugins/pages/my_plugin_page.py
--rw-r--r--   0 briford    (501) staff       (20)     1635 2024-04-16 15:58:18.000000 sageworks-0.6.6/examples/plugins/pages/plugin_page_1.py
--rw-r--r--   0 briford    (501) staff       (20)     2464 2024-04-16 15:58:18.000000 sageworks-0.6.6/examples/plugins/pages/plugin_page_2.py
--rw-r--r--   0 briford    (501) staff       (20)     4528 2024-04-16 15:58:18.000000 sageworks-0.6.6/examples/plugins/pages/plugin_page_3.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.792998 sageworks-0.6.6/examples/plugins/views/
--rw-r--r--   0 briford    (501) staff       (20)     1588 2024-04-06 16:51:44.000000 sageworks-0.6.6/examples/plugins/views/model_plugin_view.py
--rw-r--r--   0 briford    (501) staff       (20)     1264 2024-04-06 16:51:44.000000 sageworks-0.6.6/examples/plugins/views/my_view_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.793724 sageworks-0.6.6/examples/plugins/web_components/
--rw-r--r--   0 briford    (501) staff       (20)     1733 2024-04-16 15:58:18.000000 sageworks-0.6.6/examples/plugins/web_components/custom_plugin.py
--rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-16 15:58:18.000000 sageworks-0.6.6/examples/plugins/web_components/endpoint_plugin.py
--rw-r--r--   0 briford    (501) staff       (20)     3660 2024-04-16 15:58:18.000000 sageworks-0.6.6/examples/plugins/web_components/endpoint_turbo.py
--rw-r--r--   0 briford    (501) staff       (20)     2596 2024-04-16 15:58:18.000000 sageworks-0.6.6/examples/plugins/web_components/model_markdown.py
--rw-r--r--   0 briford    (501) staff       (20)     2238 2024-04-16 15:58:18.000000 sageworks-0.6.6/examples/plugins/web_components/model_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.794755 sageworks-0.6.6/examples/storage/
--rw-r--r--   0 briford    (501) staff       (20)     1222 2024-03-27 20:40:53.000000 sageworks-0.6.6/examples/storage/data_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)      856 2024-03-27 20:40:53.000000 sageworks-0.6.6/examples/storage/data_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     1371 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/storage/endpoint_inference.py
--rw-r--r--   0 briford    (501) staff       (20)     1847 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/storage/hello_world_pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)     4380 2024-04-16 15:58:18.000000 sageworks-0.6.6/examples/storage/plugin_page_example.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.795265 sageworks-0.6.6/examples/storage/sagemaker_pipelines/
--rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/storage/sagemaker_pipelines/all_steps.py
--rw-r--r--   0 briford    (501) staff       (20)       40 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/storage/sagemaker_pipelines/hello.py
--rw-r--r--   0 briford    (501) staff       (20)     1487 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/storage/sagemaker_pipelines/ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.749452 sageworks-0.6.6/examples/storage/sagemaker_pipelines/storage/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.796022 sageworks-0.6.6/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/
--rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)      203 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)      160 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/feature_set.py
--rw-r--r--   0 briford    (501) staff       (20)     1599 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)      367 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/model.py
--rw-r--r--   0 briford    (501) staff       (20)     3285 2024-05-24 14:48:45.000000 sageworks-0.6.6/mkdocs.yml
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.797039 sageworks-0.6.6/notebooks/
--rw-r--r--   0 briford    (501) staff       (20)   185443 2024-03-28 17:23:43.000000 sageworks-0.6.6/notebooks/ML_Pipeline_with_SageWorks.ipynb
--rw-r--r--   0 briford    (501) staff       (20)    36405 2024-03-28 17:23:43.000000 sageworks-0.6.6/notebooks/ML_Pipeline_with_SageWorks_2.ipynb
--rw-r--r--   0 briford    (501) staff       (20)   511134 2024-03-28 17:23:43.000000 sageworks-0.6.6/notebooks/Outliers_in_SageWorks.ipynb
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.805949 sageworks-0.6.6/notebooks/images/
--rw-r--r--   0 briford    (501) staff       (20)   142099 2023-12-24 17:18:24.000000 sageworks-0.6.6/notebooks/images/athena_query_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   191022 2023-12-24 17:18:24.000000 sageworks-0.6.6/notebooks/images/aws_dashboard_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   222686 2023-12-24 17:18:24.000000 sageworks-0.6.6/notebooks/images/dashboard_aqsol_features.png
--rw-r--r--   0 briford    (501) staff       (20)   171441 2023-12-24 17:18:24.000000 sageworks-0.6.6/notebooks/images/model_screenshot.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.6/notebooks/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.6/notebooks/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)      444 2024-05-19 21:32:59.000000 sageworks-0.6.6/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.810059 sageworks-0.6.6/scripts/
--rw-r--r--   0 briford    (501) staff       (20)     1710 2024-04-16 15:58:18.000000 sageworks-0.6.6/scripts/ag_table_row_selection.py
--rw-r--r--   0 briford    (501) staff       (20)     2290 2024-03-28 17:23:43.000000 sageworks-0.6.6/scripts/athena_ddl_mixed_case.py
--rw-r--r--   0 briford    (501) staff       (20)     2178 2024-03-27 20:32:26.000000 sageworks-0.6.6/scripts/copy_data_catalog_db.py
--rw-r--r--   0 briford    (501) staff       (20)     1222 2024-04-16 15:58:18.000000 sageworks-0.6.6/scripts/create_glue_workflow_with_trigger.py
--rw-r--r--   0 briford    (501) staff       (20)      706 2024-01-10 18:45:51.000000 sageworks-0.6.6/scripts/delete_redis_keys.py
--rw-r--r--   0 briford    (501) staff       (20)     1761 2024-03-28 17:23:43.000000 sageworks-0.6.6/scripts/glue_mixed_case.py
--rw-r--r--   0 briford    (501) staff       (20)     5544 2024-03-28 17:23:43.000000 sageworks-0.6.6/scripts/model_endpoint_sanity_check.py
--rw-r--r--   0 briford    (501) staff       (20)      715 2024-03-28 17:23:43.000000 sageworks-0.6.6/scripts/onboard_endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      694 2024-03-28 17:23:43.000000 sageworks-0.6.6/scripts/onboard_models.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.810461 sageworks-0.6.6/scripts/storage/
--rw-r--r--   0 briford    (501) staff       (20)     1003 2024-03-27 20:32:27.000000 sageworks-0.6.6/scripts/storage/dns_data_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     1723 2024-04-06 16:51:44.000000 sageworks-0.6.6/scripts/storage/generate_jsonl_data.py
--rw-r--r--   0 briford    (501) staff       (20)      955 2024-03-28 17:23:43.000000 sageworks-0.6.6/scripts/test_feature_resolution.py
--rw-r--r--   0 briford    (501) staff       (20)      533 2024-05-24 14:49:47.850506 sageworks-0.6.6/setup.cfg
--rw-r--r--   0 briford    (501) staff       (20)     1663 2024-03-27 20:32:27.000000 sageworks-0.6.6/setup.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.749906 sageworks-0.6.6/src/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.810696 sageworks-0.6.6/src/sageworks/
--rw-r--r--   0 briford    (501) staff       (20)     1091 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.811578 sageworks-0.6.6/src/sageworks/algorithms/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.6/src/sageworks/algorithms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.813264 sageworks-0.6.6/src/sageworks/algorithms/dataframe/
--rw-r--r--   0 briford    (501) staff       (20)      378 2023-12-24 17:18:24.000000 sageworks-0.6.6/src/sageworks/algorithms/dataframe/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     2852 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/dataframe/aggregation.py
--rw-r--r--   0 briford    (501) staff       (20)     1606 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/dataframe/data_source_eda.py
--rw-r--r--   0 briford    (501) staff       (20)     5388 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/dataframe/dimensionality_reduction.py
--rw-r--r--   0 briford    (501) staff       (20)     9406 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/dataframe/feature_resolution.py
--rw-r--r--   0 briford    (501) staff       (20)    12309 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/dataframe/feature_spider.py
--rw-r--r--   0 briford    (501) staff       (20)     4968 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/dataframe/row_tagger.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.750223 sageworks-0.6.6/src/sageworks/algorithms/graph/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.813540 sageworks-0.6.6/src/sageworks/algorithms/graph/heavy/
--rw-r--r--   0 briford    (501) staff       (20)       96 2023-12-24 17:18:24.000000 sageworks-0.6.6/src/sageworks/algorithms/graph/heavy/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.813745 sageworks-0.6.6/src/sageworks/algorithms/graph/light/
--rw-r--r--   0 briford    (501) staff       (20)      122 2023-12-24 17:18:24.000000 sageworks-0.6.6/src/sageworks/algorithms/graph/light/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.813951 sageworks-0.6.6/src/sageworks/algorithms/spark/
--rw-r--r--   0 briford    (501) staff       (20)      615 2023-12-24 17:18:24.000000 sageworks-0.6.6/src/sageworks/algorithms/spark/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.815560 sageworks-0.6.6/src/sageworks/algorithms/sql/
--rw-r--r--   0 briford    (501) staff       (20)      685 2023-12-24 17:18:24.000000 sageworks-0.6.6/src/sageworks/algorithms/sql/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     6192 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/sql/column_stats.py
--rw-r--r--   0 briford    (501) staff       (20)     3645 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/sql/correlations.py
--rw-r--r--   0 briford    (501) staff       (20)     3622 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/sql/descriptive_stats.py
--rw-r--r--   0 briford    (501) staff       (20)    10174 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/sql/outliers.py
--rw-r--r--   0 briford    (501) staff       (20)     2352 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/sql/sample_rows.py
--rw-r--r--   0 briford    (501) staff       (20)     3437 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/sql/value_counts.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.816844 sageworks-0.6.6/src/sageworks/api/
--rw-r--r--   0 briford    (501) staff       (20)      708 2024-04-18 20:46:23.000000 sageworks-0.6.6/src/sageworks/api/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7811 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/api/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/api/endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     4242 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/api/feature_set.py
--rw-r--r--   0 briford    (501) staff       (20)    16482 2024-04-21 15:28:58.000000 sageworks-0.6.6/src/sageworks/api/meta.py
--rw-r--r--   0 briford    (501) staff       (20)     2595 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/api/model.py
--rw-r--r--   0 briford    (501) staff       (20)     5261 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/api/monitor.py
--rw-r--r--   0 briford    (501) staff       (20)     6953 2024-04-26 21:22:37.000000 sageworks-0.6.6/src/sageworks/api/pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)     6659 2024-04-26 21:22:37.000000 sageworks-0.6.6/src/sageworks/api/pipeline_manager.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.817440 sageworks-0.6.6/src/sageworks/aws_service_broker/
--rw-r--r--   0 briford    (501) staff       (20)     9393 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_account_clamp.py
--rw-r--r--   0 briford    (501) staff       (20)    11198 2024-05-09 14:32:45.000000 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_broker.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.819044 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     1834 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
--rw-r--r--   0 briford    (501) staff       (20)     3258 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)     4055 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)     5238 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)     3712 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py
--rw-r--r--   0 briford    (501) staff       (20)     3889 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     3736 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.819202 sageworks-0.6.6/src/sageworks/core/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.820515 sageworks-0.6.6/src/sageworks/core/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      941 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/artifacts/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    17938 2024-04-15 22:06:08.000000 sageworks-0.6.6/src/sageworks/core/artifacts/artifact.py
--rw-r--r--   0 briford    (501) staff       (20)    22432 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/core/artifacts/athena_source.py
--rw-r--r--   0 briford    (501) staff       (20)    12683 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/artifacts/data_source_abstract.py
--rw-r--r--   0 briford    (501) staff       (20)     2447 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/artifacts/data_source_factory.py
--rw-r--r--   0 briford    (501) staff       (20)    36630 2024-04-21 18:44:59.000000 sageworks-0.6.6/src/sageworks/core/artifacts/endpoint_core.py
--rw-r--r--   0 briford    (501) staff       (20)    29698 2024-04-22 20:46:36.000000 sageworks-0.6.6/src/sageworks/core/artifacts/feature_set_core.py
--rw-r--r--   0 briford    (501) staff       (20)    37022 2024-05-19 19:25:11.000000 sageworks-0.6.6/src/sageworks/core/artifacts/model_core.py
--rw-r--r--   0 briford    (501) staff       (20)    21029 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/artifacts/monitor_core.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.820665 sageworks-0.6.6/src/sageworks/core/pipelines/
--rw-r--r--   0 briford    (501) staff       (20)     6919 2024-04-26 21:22:37.000000 sageworks-0.6.6/src/sageworks/core/pipelines/pipeline_executor.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.821340 sageworks-0.6.6/src/sageworks/core/transforms/
--rw-r--r--   0 briford    (501) staff       (20)     1432 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.821506 sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.821735 sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/heavy/
--rw-r--r--   0 briford    (501) staff       (20)      298 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/heavy/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     9866 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.822300 sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/light/
--rw-r--r--   0 briford    (501) staff       (20)      543 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3011 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2927 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     4225 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.822449 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.822557 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.822654 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.822909 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.823282 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2237 2024-03-27 20:40:53.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/light/clean_data.py
--rw-r--r--   0 briford    (501) staff       (20)     2687 2024-03-27 20:40:53.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.823407 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.823516 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.823722 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/chunk/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/chunk/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     4551 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.823877 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.824028 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.824176 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/storage/
--rw-r--r--   0 briford    (501) staff       (20)     6702 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.824816 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3827 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py
--rw-r--r--   0 briford    (501) staff       (20)     5674 2024-04-23 15:16:38.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.824970 sageworks-0.6.6/src/sageworks/core/transforms/features_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/features_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.752371 sageworks-0.6.6/src/sageworks/core/transforms/features_to_features/heavy/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.825072 sageworks-0.6.6/src/sageworks/core/transforms/features_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/features_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.825222 sageworks-0.6.6/src/sageworks/core/transforms/features_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/features_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.825462 sageworks-0.6.6/src/sageworks/core/transforms/features_to_model/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/features_to_model/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    13050 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/features_to_model/features_to_model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.825833 sageworks-0.6.6/src/sageworks/core/transforms/features_to_model/light_model_harness/
--rw-r--r--   0 briford    (501) staff       (20)       19 2024-02-27 23:40:48.000000 sageworks-0.6.6/src/sageworks/core/transforms/features_to_model/light_model_harness/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)    10806 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.826367 sageworks-0.6.6/src/sageworks/core/transforms/model_to_endpoint/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/model_to_endpoint/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     8185 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.827223 sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/
--rw-r--r--   0 briford    (501) staff       (20)      894 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3615 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     3445 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     8604 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)    18139 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     4440 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py
--rw-r--r--   0 briford    (501) staff       (20)     5391 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/transform.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.827547 sageworks-0.6.6/src/sageworks/experiments/
--rw-r--r--   0 briford    (501) staff       (20)    10658 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/experiments/view_manager.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.828306 sageworks-0.6.6/src/sageworks/repl/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/repl/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    15486 2024-04-21 15:35:25.000000 sageworks-0.6.6/src/sageworks/repl/sageworks_shell.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.828733 sageworks-0.6.6/src/sageworks/resources/
--rw-r--r--   0 briford    (501) staff       (20)      361 2024-01-23 15:36:53.000000 sageworks-0.6.6/src/sageworks/resources/open_source_api.key
--rw-r--r--   0 briford    (501) staff       (20)      272 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/resources/signature_verify_pub.pem
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.833179 sageworks-0.6.6/src/sageworks/utils/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.6/src/sageworks/utils/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    15587 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/utils/aws_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5447 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/utils/cache.py
--rw-r--r--   0 briford    (501) staff       (20)      722 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/chem_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    16543 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/utils/config_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     7392 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/dashboard_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)     4194 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/utils/datetime_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5292 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/df_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     1681 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/docker_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2866 2024-03-27 20:43:31.000000 sageworks-0.6.6/src/sageworks/utils/ecs_info.py
--rw-r--r--   0 briford    (501) staff       (20)     7657 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/endpoint_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)     3097 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/endpoint_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     6979 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/extract_model_artifact.py
--rw-r--r--   0 briford    (501) staff       (20)     1131 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/glue_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     6404 2024-05-20 15:33:17.000000 sageworks-0.6.6/src/sageworks/utils/license_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     1439 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/utils/markdown_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    15517 2024-04-22 20:45:19.000000 sageworks-0.6.6/src/sageworks/utils/pandas_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    12684 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/utils/plugin_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     9533 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/utils/redis_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     4166 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/repl_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2089 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/s3_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2163 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/sageworks_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     3474 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/sageworks_event_bridge.py
--rw-r--r--   0 briford    (501) staff       (20)     5359 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/sageworks_logging.py
--rw-r--r--   0 briford    (501) staff       (20)     2120 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/sageworks_sqs.py
--rw-r--r--   0 briford    (501) staff       (20)     1108 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/utils/symbols.py
--rw-r--r--   0 briford    (501) staff       (20)     6414 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/test_data_generator.py
--rw-r--r--   0 briford    (501) staff       (20)     2092 2024-03-27 20:43:31.000000 sageworks-0.6.6/src/sageworks/utils/trace_calls.py
--rw-r--r--   0 briford    (501) staff       (20)     1470 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/type_abbrev.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.834691 sageworks-0.6.6/src/sageworks/views/
--rw-r--r--   0 briford    (501) staff       (20)     3517 2024-04-16 22:29:17.000000 sageworks-0.6.6/src/sageworks/views/artifacts_text_view.py
--rw-r--r--   0 briford    (501) staff       (20)     7780 2024-04-28 17:17:45.000000 sageworks-0.6.6/src/sageworks/views/artifacts_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     3158 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/views/data_source_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     2150 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/views/endpoint_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     3206 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/views/feature_set_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/views/model_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     1092 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/views/view.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.838397 sageworks-0.6.6/src/sageworks/web_components/
--rw-r--r--   0 briford    (501) staff       (20)     5916 2024-04-25 23:06:38.000000 sageworks-0.6.6/src/sageworks/web_components/component_interface.py
--rw-r--r--   0 briford    (501) staff       (20)     3525 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/confusion_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     5854 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/correlation_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     9328 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/web_components/data_details_markdown.py
--rw-r--r--   0 briford    (501) staff       (20)     4558 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/web_components/endpoint_details.py
--rw-r--r--   0 briford    (501) staff       (20)     3068 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/endpoint_metric_plots.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.840723 sageworks-0.6.6/src/sageworks/web_components/experiments/
--rw-r--r--   0 briford    (501) staff       (20)      837 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/experiments/color_maps.py
--rw-r--r--   0 briford    (501) staff       (20)     1633 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/web_components/experiments/compound_details.py
--rw-r--r--   0 briford    (501) staff       (20)     2974 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/experiments/dashboard_metric_plots.py
--rw-r--r--   0 briford    (501) staff       (20)     2240 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/experiments/data_table.py
--rw-r--r--   0 briford    (501) staff       (20)     1183 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/web_components/experiments/histogram.py
--rw-r--r--   0 briford    (501) staff       (20)      838 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/experiments/line_chart.py
--rw-r--r--   0 briford    (501) staff       (20)     3680 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/web_components/experiments/outlier_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     2373 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/experiments/plugin_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2279 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/web_components/experiments/scatter_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     8690 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/model_details.py
--rw-r--r--   0 briford    (501) staff       (20)     2278 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/model_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     7191 2024-05-19 17:03:46.000000 sageworks-0.6.6/src/sageworks/web_components/plugin_interface.py
--rw-r--r--   0 briford    (501) staff       (20)     3530 2024-04-25 23:09:25.000000 sageworks-0.6.6/src/sageworks/web_components/plugin_unit_test.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.841875 sageworks-0.6.6/src/sageworks/web_components/plugins/
--rw-r--r--   0 briford    (501) staff       (20)     2786 2024-04-26 21:04:42.000000 sageworks-0.6.6/src/sageworks/web_components/plugins/ag_table.py
--rw-r--r--   0 briford    (501) staff       (20)     5498 2024-05-22 14:54:18.000000 sageworks-0.6.6/src/sageworks/web_components/plugins/license_details.py
--rw-r--r--   0 briford    (501) staff       (20)     9653 2024-04-15 13:43:00.000000 sageworks-0.6.6/src/sageworks/web_components/plugins/model_details.py
--rw-r--r--   0 briford    (501) staff       (20)     2429 2024-04-26 21:22:37.000000 sageworks-0.6.6/src/sageworks/web_components/plugins/pipeline_details.py
--rw-r--r--   0 briford    (501) staff       (20)     2945 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/regression_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     6838 2024-05-06 17:24:24.000000 sageworks-0.6.6/src/sageworks/web_components/table.py
--rw-r--r--   0 briford    (501) staff       (20)     5185 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/violin_plots.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.849595 sageworks-0.6.6/src/sageworks.egg-info/
--rw-r--r--   0 briford    (501) staff       (20)     4961 2024-05-24 14:49:47.000000 sageworks-0.6.6/src/sageworks.egg-info/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)    19184 2024-05-24 14:49:47.000000 sageworks-0.6.6/src/sageworks.egg-info/SOURCES.txt
--rw-r--r--   0 briford    (501) staff       (20)        1 2024-05-24 14:49:47.000000 sageworks-0.6.6/src/sageworks.egg-info/dependency_links.txt
--rw-r--r--   0 briford    (501) staff       (20)       74 2024-05-24 14:49:47.000000 sageworks-0.6.6/src/sageworks.egg-info/entry_points.txt
--rw-r--r--   0 briford    (501) staff       (20)      421 2024-05-24 14:49:47.000000 sageworks-0.6.6/src/sageworks.egg-info/requires.txt
--rw-r--r--   0 briford    (501) staff       (20)       10 2024-05-24 14:49:47.000000 sageworks-0.6.6/src/sageworks.egg-info/top_level.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.843256 sageworks-0.6.6/tests/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.844093 sageworks-0.6.6/tests/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)     1548 2024-03-30 19:27:28.000000 sageworks-0.6.6/tests/artifacts/data_source_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     2442 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/artifacts/endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1160 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/artifacts/feature_set_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      805 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/artifacts/model_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.844492 sageworks-0.6.6/tests/aws_account/
--rw-r--r--   0 briford    (501) staff       (20)      962 2023-12-24 17:18:24.000000 sageworks-0.6.6/tests/aws_account/aws_account_clamp_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      642 2023-12-24 17:18:24.000000 sageworks-0.6.6/tests/aws_account/aws_service_broker_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.845681 sageworks-0.6.6/tests/connectors/
--rw-r--r--   0 briford    (501) staff       (20)      725 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)      737 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      702 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)      644 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/connectors/glue_jobs.py
--rw-r--r--   0 briford    (501) staff       (20)      799 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     1008 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/connectors/s3_bucket.py
--rw-r--r--   0 briford    (501) staff       (20)     5618 2024-04-26 21:04:42.000000 sageworks-0.6.6/tests/create_aqsol_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     3217 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/create_basic_test_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)      870 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/create_realtime_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     2378 2024-04-22 20:46:36.000000 sageworks-0.6.6/tests/create_training_adjusted_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     2096 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/create_wine_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     4448 2024-04-16 15:58:18.000000 sageworks-0.6.6/tests/delete_test_artifacts.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.845849 sageworks-0.6.6/tests/plugin_tests/
--rw-r--r--   0 briford    (501) staff       (20)     1885 2024-04-16 15:58:18.000000 sageworks-0.6.6/tests/plugin_tests/crashing_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.846157 sageworks-0.6.6/tests/specific/
--rw-r--r--   0 briford    (501) staff       (20)      639 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/specific/capital_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1513 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/specific/deletion_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.847542 sageworks-0.6.6/tests/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      592 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/transforms/data_to_data_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1025 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/transforms/data_to_features_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      773 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/transforms/features_to_model_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     5142 2024-04-20 00:25:37.000000 sageworks-0.6.6/tests/transforms/model_metrics_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      795 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/transforms/model_to_endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      633 2024-03-27 20:40:53.000000 sageworks-0.6.6/tests/transforms/pandas_to_data_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.848096 sageworks-0.6.6/tests/web_components/
--rw-r--r--   0 briford    (501) staff       (20)      681 2024-04-16 15:58:18.000000 sageworks-0.6.6/tests/web_components/confusion_matrix_test.py
--rw-r--r--   0 briford    (501) staff       (20)      677 2024-04-16 15:58:18.000000 sageworks-0.6.6/tests/web_components/correlation_matrix_test.py
--rw-r--r--   0 briford    (501) staff       (20)     5269 2024-04-16 15:58:18.000000 sageworks-0.6.6/tests/web_components/plugin_interface_test.py
--rw-r--r--   0 briford    (501) staff       (20)     1115 2024-03-27 20:43:31.000000 sageworks-0.6.6/tox.ini
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.848945 sageworks-0.6.6/ui_testing/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.849183 sageworks-0.6.6/ui_testing/assets/
--rw-r--r--   0 briford    (501) staff       (20)      597 2024-05-13 15:14:49.000000 sageworks-0.6.6/ui_testing/assets/custom.css
--rw-r--r--   0 briford    (501) staff       (20)     5770 2024-05-19 19:25:10.000000 sageworks-0.6.6/ui_testing/table_comparison.py
--rw-r--r--   0 briford    (501) staff       (20)     2025 2024-05-19 19:25:10.000000 sageworks-0.6.6/ui_testing/theme_switching.py
--rw-r--r--   0 briford    (501) staff       (20)     1819 2024-05-19 19:25:10.000000 sageworks-0.6.6/ui_testing/theme_switching_2.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.104442 sageworks-0.6.8/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:30.999856 sageworks-0.6.8/.github/
+-rw-r--r--   0 briford    (501) staff       (20)     1338 2024-03-28 17:23:43.000000 sageworks-0.6.8/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 briford    (501) staff       (20)      499 2023-12-24 17:18:24.000000 sageworks-0.6.8/.github/dependabot.yml
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.000306 sageworks-0.6.8/.github/workflows/
+-rw-r--r--   0 briford    (501) staff       (20)      598 2024-01-10 18:45:51.000000 sageworks-0.6.8/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 briford    (501) staff       (20)      556 2024-01-23 15:36:53.000000 sageworks-0.6.8/.github/workflows/python-lint.yml
+-rw-r--r--   0 briford    (501) staff       (20)     2037 2024-05-15 21:28:12.000000 sageworks-0.6.8/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)      791 2024-04-16 15:58:18.000000 sageworks-0.6.8/CONTRIBUTING.md
+-rw-r--r--   0 briford    (501) staff       (20)      102 2024-03-28 17:23:43.000000 sageworks-0.6.8/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)     1080 2024-03-28 17:23:43.000000 sageworks-0.6.8/LICENSE
+-rw-r--r--   0 briford    (501) staff       (20)     1426 2023-12-24 17:18:24.000000 sageworks-0.6.8/Makefile
+-rw-r--r--   0 briford    (501) staff       (20)     4961 2024-05-30 17:23:31.104374 sageworks-0.6.8/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)     3510 2024-05-09 14:32:45.000000 sageworks-0.6.8/README.md
+-rw-r--r--   0 briford    (501) staff       (20)      463 2023-12-24 17:18:24.000000 sageworks-0.6.8/SECURITY.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:30.988849 sageworks-0.6.8/applications/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.002147 sageworks-0.6.8/applications/aws_dashboard/
+-rw-r--r--   0 briford    (501) staff       (20)     1071 2024-05-24 14:50:34.000000 sageworks-0.6.8/applications/aws_dashboard/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)      331 2024-03-28 17:23:43.000000 sageworks-0.6.8/applications/aws_dashboard/Dockerfile_plugins
+-rw-r--r--   0 briford    (501) staff       (20)      841 2024-01-10 18:45:51.000000 sageworks-0.6.8/applications/aws_dashboard/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1526 2024-04-09 14:37:33.000000 sageworks-0.6.8/applications/aws_dashboard/app.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.003543 sageworks-0.6.8/applications/aws_dashboard/assets/
+-rw-r--r--   0 briford    (501) staff       (20)   232839 2024-04-06 16:51:44.000000 sageworks-0.6.8/applications/aws_dashboard/assets/bootstrap_darkly.min.css
+-rw-r--r--   0 briford    (501) staff       (20)    14995 2024-04-06 16:51:44.000000 sageworks-0.6.8/applications/aws_dashboard/assets/default.css
+-rw-r--r--   0 briford    (501) staff       (20)    10375 2024-04-16 15:58:18.000000 sageworks-0.6.8/applications/aws_dashboard/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)      732 2023-12-24 17:18:24.000000 sageworks-0.6.8/applications/aws_dashboard/assets/trash.png
+-rwxr-xr-x   0 briford    (501) staff       (20)      637 2024-04-26 21:03:22.000000 sageworks-0.6.8/applications/aws_dashboard/dashboard
+-rw-r--r--   0 briford    (501) staff       (20)      205 2023-12-24 17:18:24.000000 sageworks-0.6.8/applications/aws_dashboard/nginx.conf
+-rw-r--r--   0 briford    (501) staff       (20)      684 2024-03-28 17:23:43.000000 sageworks-0.6.8/applications/aws_dashboard/open_source_config.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:30.988772 sageworks-0.6.8/applications/aws_dashboard/pages/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.004298 sageworks-0.6.8/applications/aws_dashboard/pages/data_sources/
+-rw-r--r--   0 briford    (501) staff       (20)    11700 2024-04-16 15:58:18.000000 sageworks-0.6.8/applications/aws_dashboard/pages/data_sources/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2756 2024-03-28 17:23:43.000000 sageworks-0.6.8/applications/aws_dashboard/pages/data_sources/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2555 2024-03-28 17:23:43.000000 sageworks-0.6.8/applications/aws_dashboard/pages/data_sources/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.005069 sageworks-0.6.8/applications/aws_dashboard/pages/endpoints/
+-rw-r--r--   0 briford    (501) staff       (20)     4439 2024-05-28 15:10:23.000000 sageworks-0.6.8/applications/aws_dashboard/pages/endpoints/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2677 2024-04-16 15:58:18.000000 sageworks-0.6.8/applications/aws_dashboard/pages/endpoints/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2550 2024-05-28 15:10:23.000000 sageworks-0.6.8/applications/aws_dashboard/pages/endpoints/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.005777 sageworks-0.6.8/applications/aws_dashboard/pages/feature_sets/
+-rw-r--r--   0 briford    (501) staff       (20)    11614 2024-04-16 15:58:18.000000 sageworks-0.6.8/applications/aws_dashboard/pages/feature_sets/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2438 2024-03-28 17:23:43.000000 sageworks-0.6.8/applications/aws_dashboard/pages/feature_sets/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.6.8/applications/aws_dashboard/pages/feature_sets/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.005940 sageworks-0.6.8/applications/aws_dashboard/pages/license/
+-rw-r--r--   0 briford    (501) staff       (20)     1531 2024-05-19 19:25:10.000000 sageworks-0.6.8/applications/aws_dashboard/pages/license/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.006700 sageworks-0.6.8/applications/aws_dashboard/pages/main/
+-rw-r--r--   0 briford    (501) staff       (20)     4899 2024-04-06 16:51:44.000000 sageworks-0.6.8/applications/aws_dashboard/pages/main/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     3307 2024-05-19 19:21:21.000000 sageworks-0.6.8/applications/aws_dashboard/pages/main/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1844 2024-03-28 17:23:43.000000 sageworks-0.6.8/applications/aws_dashboard/pages/main/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.007393 sageworks-0.6.8/applications/aws_dashboard/pages/models/
+-rw-r--r--   0 briford    (501) staff       (20)     4195 2024-05-28 15:10:23.000000 sageworks-0.6.8/applications/aws_dashboard/pages/models/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2234 2024-04-27 20:59:25.000000 sageworks-0.6.8/applications/aws_dashboard/pages/models/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2227 2024-05-28 15:10:23.000000 sageworks-0.6.8/applications/aws_dashboard/pages/models/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.008058 sageworks-0.6.8/applications/aws_dashboard/pages/pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)     1791 2024-04-26 21:07:33.000000 sageworks-0.6.8/applications/aws_dashboard/pages/pipelines/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2664 2024-04-26 20:07:24.000000 sageworks-0.6.8/applications/aws_dashboard/pages/pipelines/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1927 2024-04-26 21:04:41.000000 sageworks-0.6.8/applications/aws_dashboard/pages/pipelines/page.py
+-rw-r--r--   0 briford    (501) staff       (20)      407 2024-05-19 21:33:27.000000 sageworks-0.6.8/applications/aws_dashboard/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)      457 2023-12-24 17:18:24.000000 sageworks-0.6.8/applications/aws_dashboard/supervisord.conf
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:30.988901 sageworks-0.6.8/applications/experiments/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.009674 sageworks-0.6.8/applications/experiments/compound_explorer/
+-rw-r--r--   0 briford    (501) staff       (20)      181 2023-12-24 17:18:24.000000 sageworks-0.6.8/applications/experiments/compound_explorer/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)      360 2023-12-24 17:18:24.000000 sageworks-0.6.8/applications/experiments/compound_explorer/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     3082 2024-04-06 16:51:44.000000 sageworks-0.6.8/applications/experiments/compound_explorer/app.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.010176 sageworks-0.6.8/applications/experiments/compound_explorer/assets/
+-rw-r--r--   0 briford    (501) staff       (20)    12861 2023-12-24 17:18:24.000000 sageworks-0.6.8/applications/experiments/compound_explorer/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.6.8/applications/experiments/compound_explorer/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)     7678 2024-04-16 15:58:18.000000 sageworks-0.6.8/applications/experiments/compound_explorer/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     4860 2024-03-28 17:23:43.000000 sageworks-0.6.8/applications/experiments/compound_explorer/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)       94 2023-12-24 17:18:24.000000 sageworks-0.6.8/applications/experiments/compound_explorer/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.010690 sageworks-0.6.8/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     3582 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/aws_account_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/aws_identity_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     2629 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/build_ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.010841 sageworks-0.6.8/aws_setup/event_bridge/
+-rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/event_bridge/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.011595 sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/
+-rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     1007 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/cdk.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.011838 sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/lambda/
+-rw-r--r--   0 briford    (501) staff       (20)     1812 2024-01-10 18:45:51.000000 sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py
+-rw-r--r--   0 briford    (501) staff       (20)     2599 2024-03-27 20:43:31.000000 sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.013062 sageworks-0.6.8/aws_setup/sageworks_core/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_core/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1028 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_core/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/sageworks_core/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     1998 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_core/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_core/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       53 2024-01-10 18:45:51.000000 sageworks-0.6.8/aws_setup/sageworks_core/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.013432 sageworks-0.6.8/aws_setup/sageworks_core/sageworks_core/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/aws_setup/sageworks_core/sageworks_core/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    23575 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_core/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.013791 sageworks-0.6.8/aws_setup/sageworks_core/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_core/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.014019 sageworks-0.6.8/aws_setup/sageworks_core/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_core/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      720 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.015719 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1907 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       47 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.016042 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7022 2024-04-24 21:53:47.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.016359 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.016562 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      565 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.017272 sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1928 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       47 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.017529 sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     6849 2024-05-24 14:56:58.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.018776 sageworks-0.6.8/data/
+-rw-r--r--   0 briford    (501) staff       (20)   191978 2023-12-24 17:18:24.000000 sageworks-0.6.8/data/abalone.csv
+-rw-r--r--   0 briford    (501) staff       (20)     1515 2023-12-24 17:18:24.000000 sageworks-0.6.8/data/test_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)     2270 2023-12-24 17:18:24.000000 sageworks-0.6.8/data/test_data.json
+-rw-r--r--   0 briford    (501) staff       (20)    12977 2024-01-10 18:45:51.000000 sageworks-0.6.8/data/wine_dataset.csv
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.019022 sageworks-0.6.8/docs/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.019512 sageworks-0.6.8/docs/admin/
+-rw-r--r--   0 briford    (501) staff       (20)     2176 2024-04-16 15:58:18.000000 sageworks-0.6.8/docs/admin/docker_push.md
+-rw-r--r--   0 briford    (501) staff       (20)     1594 2024-05-30 16:53:00.000000 sageworks-0.6.8/docs/admin/pypi_release.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.021416 sageworks-0.6.8/docs/api_classes/
+-rw-r--r--   0 briford    (501) staff       (20)     3595 2024-01-23 15:36:53.000000 sageworks-0.6.8/docs/api_classes/data_source.md
+-rw-r--r--   0 briford    (501) staff       (20)     5199 2024-05-28 20:18:51.000000 sageworks-0.6.8/docs/api_classes/endpoint.md
+-rw-r--r--   0 briford    (501) staff       (20)     6299 2024-03-28 17:23:43.000000 sageworks-0.6.8/docs/api_classes/feature_set.md
+-rw-r--r--   0 briford    (501) staff       (20)     5350 2024-04-06 16:51:44.000000 sageworks-0.6.8/docs/api_classes/meta.md
+-rw-r--r--   0 briford    (501) staff       (20)     4356 2024-05-28 20:18:51.000000 sageworks-0.6.8/docs/api_classes/model.md
+-rw-r--r--   0 briford    (501) staff       (20)     2218 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/api_classes/monitor.md
+-rw-r--r--   0 briford    (501) staff       (20)     3549 2024-05-28 20:18:51.000000 sageworks-0.6.8/docs/api_classes/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)     4894 2024-04-19 15:50:50.000000 sageworks-0.6.8/docs/api_classes/pipelines.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.023124 sageworks-0.6.8/docs/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     1121 2024-03-28 17:23:43.000000 sageworks-0.6.8/docs/aws_setup/aws_access_management.md
+-rw-r--r--   0 briford    (501) staff       (20)     5610 2024-05-06 14:50:56.000000 sageworks-0.6.8/docs/aws_setup/aws_tips_and_tricks.md
+-rw-r--r--   0 briford    (501) staff       (20)     4210 2024-05-09 14:32:45.000000 sageworks-0.6.8/docs/aws_setup/core_stack.md
+-rw-r--r--   0 briford    (501) staff       (20)     2075 2024-03-28 17:23:43.000000 sageworks-0.6.8/docs/aws_setup/dashboard_stack.md
+-rw-r--r--   0 briford    (501) staff       (20)     7313 2024-05-15 23:47:50.000000 sageworks-0.6.8/docs/aws_setup/domain_cert_setup.md
+-rw-r--r--   0 briford    (501) staff       (20)     2540 2024-01-23 15:36:53.000000 sageworks-0.6.8/docs/aws_setup/full_pipeline.md
+-rw-r--r--   0 briford    (501) staff       (20)     3438 2024-05-09 14:20:27.000000 sageworks-0.6.8/docs/aws_setup/sso_setup.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.023886 sageworks-0.6.8/docs/blogs_research/
+-rw-r--r--   0 briford    (501) staff       (20)      912 2024-03-28 17:23:43.000000 sageworks-0.6.8/docs/blogs_research/eda.md
+-rw-r--r--   0 briford    (501) staff       (20)     2017 2024-03-28 17:23:43.000000 sageworks-0.6.8/docs/blogs_research/htg.md
+-rw-r--r--   0 briford    (501) staff       (20)      802 2024-05-21 22:30:34.000000 sageworks-0.6.8/docs/blogs_research/index.md
+-rw-r--r--   0 briford    (501) staff       (20)     1245 2024-05-28 20:18:51.000000 sageworks-0.6.8/docs/blogs_research/residual_analysis.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.024101 sageworks-0.6.8/docs/concepts/
+-rw-r--r--   0 briford    (501) staff       (20)      907 2024-05-28 20:18:51.000000 sageworks-0.6.8/docs/concepts/model_monitoring.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.024321 sageworks-0.6.8/docs/core_classes/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.025900 sageworks-0.6.8/docs/core_classes/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      464 2024-01-23 15:36:53.000000 sageworks-0.6.8/docs/core_classes/artifacts/artifact.md
+-rw-r--r--   0 briford    (501) staff       (20)      290 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/artifacts/athena_source.md
+-rw-r--r--   0 briford    (501) staff       (20)      479 2024-01-23 15:36:53.000000 sageworks-0.6.8/docs/core_classes/artifacts/data_source_abstract.md
+-rw-r--r--   0 briford    (501) staff       (20)      292 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/artifacts/endpoint_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      294 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/artifacts/feature_set_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      281 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/artifacts/model_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      289 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/artifacts/monitor_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      861 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/artifacts/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)     2119 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/overview.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.027545 sageworks-0.6.8/docs/core_classes/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      352 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/transforms/data_loaders_heavy.md
+-rw-r--r--   0 briford    (501) staff       (20)      396 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/transforms/data_loaders_light.md
+-rw-r--r--   0 briford    (501) staff       (20)      349 2024-03-28 17:23:43.000000 sageworks-0.6.8/docs/core_classes/transforms/data_to_features.md
+-rw-r--r--   0 briford    (501) staff       (20)      265 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/transforms/features_to_model.md
+-rw-r--r--   0 briford    (501) staff       (20)      264 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/transforms/model_to_endpoint.md
+-rw-r--r--   0 briford    (501) staff       (20)     1177 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/transforms/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)      970 2024-01-23 15:36:53.000000 sageworks-0.6.8/docs/core_classes/transforms/pandas_transforms.md
+-rw-r--r--   0 briford    (501) staff       (20)      521 2024-01-23 15:36:53.000000 sageworks-0.6.8/docs/core_classes/transforms/transform.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.028312 sageworks-0.6.8/docs/enterprise/
+-rw-r--r--   0 briford    (501) staff       (20)     4075 2024-05-20 20:55:48.000000 sageworks-0.6.8/docs/enterprise/index.md
+-rw-r--r--   0 briford    (501) staff       (20)      786 2024-04-28 17:52:09.000000 sageworks-0.6.8/docs/enterprise/project_branding.md
+-rw-r--r--   0 briford    (501) staff       (20)      892 2024-04-28 18:00:11.000000 sageworks-0.6.8/docs/enterprise/themes.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.028546 sageworks-0.6.8/docs/getting_started/
+-rw-r--r--   0 briford    (501) staff       (20)     1975 2024-05-09 14:38:45.000000 sageworks-0.6.8/docs/getting_started/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.028772 sageworks-0.6.8/docs/glue/
+-rw-r--r--   0 briford    (501) staff       (20)     4837 2024-03-28 17:23:43.000000 sageworks-0.6.8/docs/glue/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.033858 sageworks-0.6.8/docs/images/
+-rw-r--r--   0 briford    (501) staff       (20)   605827 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/big_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)    32320 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/graph_representation.png
+-rw-r--r--   0 briford    (501) staff       (20)    15549 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/powered_aws_dark_blue.png
+-rw-r--r--   0 briford    (501) staff       (20)    10003 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/powered_aws_transparent.png
+-rw-r--r--   0 briford    (501) staff       (20)     6435 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/powered_aws_white.png
+-rw-r--r--   0 briford    (501) staff       (20)    21174 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/powered_aws_with_tm_grey.png
+-rw-r--r--   0 briford    (501) staff       (20)    51137 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/sageworks.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)    30017 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/scp.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)   381209 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/small_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)     3443 2024-05-09 14:20:27.000000 sageworks-0.6.8/docs/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.035444 sageworks-0.6.8/docs/misc/
+-rw-r--r--   0 briford    (501) staff       (20)     2791 2024-03-28 17:23:43.000000 sageworks-0.6.8/docs/misc/faq.md
+-rw-r--r--   0 briford    (501) staff       (20)     5069 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/misc/general_info.md
+-rw-r--r--   0 briford    (501) staff       (20)      667 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/misc/sageworks_classes_concepts.md
+-rw-r--r--   0 briford    (501) staff       (20)     1873 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/misc/scp_consulting.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.035933 sageworks-0.6.8/docs/plugins/
+-rw-r--r--   0 briford    (501) staff       (20)     3361 2024-04-16 15:58:18.000000 sageworks-0.6.8/docs/plugins/index.md
+-rw-r--r--   0 briford    (501) staff       (20)      750 2024-04-06 16:51:44.000000 sageworks-0.6.8/docs/plugins/plugin_api_changes.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.036172 sageworks-0.6.8/docs/repl/
+-rw-r--r--   0 briford    (501) staff       (20)     2080 2024-05-09 14:40:59.000000 sageworks-0.6.8/docs/repl/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.036428 sageworks-0.6.8/examples/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.036648 sageworks-0.6.8/examples/ag-grid/
+-rw-r--r--   0 briford    (501) staff       (20)      496 2024-04-06 16:51:44.000000 sageworks-0.6.8/examples/ag-grid/hello_world.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.037759 sageworks-0.6.8/examples/datasource/
+-rw-r--r--   0 briford    (501) staff       (20)      326 2024-01-10 18:45:51.000000 sageworks-0.6.8/examples/datasource/datasource_from_df.py
+-rw-r--r--   0 briford    (501) staff       (20)      332 2024-01-10 18:45:51.000000 sageworks-0.6.8/examples/datasource/datasource_from_s3.py
+-rw-r--r--   0 briford    (501) staff       (20)      536 2024-01-23 15:36:53.000000 sageworks-0.6.8/examples/datasource/datasource_query.py
+-rw-r--r--   0 briford    (501) staff       (20)      680 2024-01-23 15:36:53.000000 sageworks-0.6.8/examples/datasource/datasource_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)      223 2024-01-10 18:45:51.000000 sageworks-0.6.8/examples/datasource/datasource_to_featureset.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.038282 sageworks-0.6.8/examples/endpoint/
+-rw-r--r--   0 briford    (501) staff       (20)      199 2024-01-10 18:45:51.000000 sageworks-0.6.8/examples/endpoint/endpoint_details.py
+-rw-r--r--   0 briford    (501) staff       (20)      834 2024-05-28 20:18:51.000000 sageworks-0.6.8/examples/endpoint/endpoint_inference.py
+-rw-r--r--   0 briford    (501) staff       (20)      481 2024-01-10 18:45:51.000000 sageworks-0.6.8/examples/endpoint/endpoint_metrics.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.038786 sageworks-0.6.8/examples/featureset/
+-rw-r--r--   0 briford    (501) staff       (20)      744 2024-01-10 18:45:51.000000 sageworks-0.6.8/examples/featureset/featureset_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)      560 2024-03-28 17:23:43.000000 sageworks-0.6.8/examples/featureset/featureset_query.py
+-rw-r--r--   0 briford    (501) staff       (20)      421 2024-03-27 20:32:26.000000 sageworks-0.6.8/examples/featureset/featureset_to_model.py
+-rw-r--r--   0 briford    (501) staff       (20)     1534 2024-05-28 20:18:51.000000 sageworks-0.6.8/examples/full_ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.039477 sageworks-0.6.8/examples/glue/
+-rw-r--r--   0 briford    (501) staff       (20)      580 2024-01-23 15:36:53.000000 sageworks-0.6.8/examples/glue/glue_hello_world.py
+-rw-r--r--   0 briford    (501) staff       (20)      942 2024-01-23 15:36:53.000000 sageworks-0.6.8/examples/glue/glue_hello_world_with_log.py
+-rw-r--r--   0 briford    (501) staff       (20)      686 2024-01-23 15:36:53.000000 sageworks-0.6.8/examples/glue/glue_load_s3_bucket.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.040035 sageworks-0.6.8/examples/meta/
+-rw-r--r--   0 briford    (501) staff       (20)      363 2024-04-06 16:51:44.000000 sageworks-0.6.8/examples/meta/meta_list_endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      328 2024-04-06 16:51:44.000000 sageworks-0.6.8/examples/meta/meta_list_models.py
+-rw-r--r--   0 briford    (501) staff       (20)      659 2024-04-06 16:51:44.000000 sageworks-0.6.8/examples/meta/meta_model_metrics.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.040585 sageworks-0.6.8/examples/model/
+-rw-r--r--   0 briford    (501) staff       (20)      564 2024-05-29 18:44:03.000000 sageworks-0.6.8/examples/model/model_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)      312 2024-03-27 20:32:26.000000 sageworks-0.6.8/examples/model/model_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)      705 2024-05-08 21:58:54.000000 sageworks-0.6.8/examples/model/onboard_model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.040960 sageworks-0.6.8/examples/monitor/
+-rw-r--r--   0 briford    (501) staff       (20)      400 2024-01-10 18:45:51.000000 sageworks-0.6.8/examples/monitor/monitor_setup.py
+-rw-r--r--   0 briford    (501) staff       (20)      765 2024-01-10 18:45:51.000000 sageworks-0.6.8/examples/monitor/monitor_usage.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.042253 sageworks-0.6.8/examples/pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)     1000 2024-04-19 14:53:32.000000 sageworks-0.6.8/examples/pipelines/abalone_pipeline_v1.json
+-rw-r--r--   0 briford    (501) staff       (20)     1073 2024-04-19 19:42:10.000000 sageworks-0.6.8/examples/pipelines/abalone_pipeline_v2.json
+-rw-r--r--   0 briford    (501) staff       (20)     4435 2024-04-20 17:35:29.000000 sageworks-0.6.8/examples/pipelines/aqsol_pipeline_v1.json
+-rw-r--r--   0 briford    (501) staff       (20)      142 2024-04-19 14:55:38.000000 sageworks-0.6.8/examples/pipelines/pipeline_details.py
+-rw-r--r--   0 briford    (501) staff       (20)      324 2024-04-19 14:55:38.000000 sageworks-0.6.8/examples/pipelines/pipeline_execute.py
+-rw-r--r--   0 briford    (501) staff       (20)      556 2024-04-19 14:51:51.000000 sageworks-0.6.8/examples/pipelines/pipeline_manager.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:30.992177 sageworks-0.6.8/examples/plugins/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.043154 sageworks-0.6.8/examples/plugins/pages/
+-rw-r--r--   0 briford    (501) staff       (20)     2467 2024-04-09 15:13:19.000000 sageworks-0.6.8/examples/plugins/pages/my_plugin_page.py
+-rw-r--r--   0 briford    (501) staff       (20)     1635 2024-04-16 15:58:18.000000 sageworks-0.6.8/examples/plugins/pages/plugin_page_1.py
+-rw-r--r--   0 briford    (501) staff       (20)     2464 2024-04-16 15:58:18.000000 sageworks-0.6.8/examples/plugins/pages/plugin_page_2.py
+-rw-r--r--   0 briford    (501) staff       (20)     5810 2024-05-27 22:25:50.000000 sageworks-0.6.8/examples/plugins/pages/plugin_page_3.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.043555 sageworks-0.6.8/examples/plugins/views/
+-rw-r--r--   0 briford    (501) staff       (20)     1588 2024-04-06 16:51:44.000000 sageworks-0.6.8/examples/plugins/views/model_plugin_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     1264 2024-04-06 16:51:44.000000 sageworks-0.6.8/examples/plugins/views/my_view_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.044262 sageworks-0.6.8/examples/plugins/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)     1733 2024-04-16 15:58:18.000000 sageworks-0.6.8/examples/plugins/web_components/custom_plugin.py
+-rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-16 15:58:18.000000 sageworks-0.6.8/examples/plugins/web_components/endpoint_plugin.py
+-rw-r--r--   0 briford    (501) staff       (20)     3660 2024-04-16 15:58:18.000000 sageworks-0.6.8/examples/plugins/web_components/endpoint_turbo.py
+-rw-r--r--   0 briford    (501) staff       (20)     2596 2024-04-16 15:58:18.000000 sageworks-0.6.8/examples/plugins/web_components/model_markdown.py
+-rw-r--r--   0 briford    (501) staff       (20)     2238 2024-04-16 15:58:18.000000 sageworks-0.6.8/examples/plugins/web_components/model_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.045321 sageworks-0.6.8/examples/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     1222 2024-03-27 20:40:53.000000 sageworks-0.6.8/examples/storage/data_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)      856 2024-03-27 20:40:53.000000 sageworks-0.6.8/examples/storage/data_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     1371 2024-05-28 20:18:51.000000 sageworks-0.6.8/examples/storage/endpoint_inference.py
+-rw-r--r--   0 briford    (501) staff       (20)     1847 2024-03-28 17:23:43.000000 sageworks-0.6.8/examples/storage/hello_world_pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)     4380 2024-04-16 15:58:18.000000 sageworks-0.6.8/examples/storage/plugin_page_example.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.046086 sageworks-0.6.8/examples/storage/sagemaker_pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.8/examples/storage/sagemaker_pipelines/all_steps.py
+-rw-r--r--   0 briford    (501) staff       (20)       40 2024-03-28 17:23:43.000000 sageworks-0.6.8/examples/storage/sagemaker_pipelines/hello.py
+-rw-r--r--   0 briford    (501) staff       (20)     1487 2024-03-28 17:23:43.000000 sageworks-0.6.8/examples/storage/sagemaker_pipelines/ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:30.992444 sageworks-0.6.8/examples/storage/sagemaker_pipelines/storage/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.046816 sageworks-0.6.8/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/
+-rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.8/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)      203 2024-03-28 17:23:43.000000 sageworks-0.6.8/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)      160 2024-03-28 17:23:43.000000 sageworks-0.6.8/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/feature_set.py
+-rw-r--r--   0 briford    (501) staff       (20)     1599 2024-03-28 17:23:43.000000 sageworks-0.6.8/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)      367 2024-03-28 17:23:43.000000 sageworks-0.6.8/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/model.py
+-rw-r--r--   0 briford    (501) staff       (20)     3285 2024-05-24 14:48:45.000000 sageworks-0.6.8/mkdocs.yml
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.047634 sageworks-0.6.8/notebooks/
+-rw-r--r--   0 briford    (501) staff       (20)    17688 2024-05-29 15:28:13.000000 sageworks-0.6.8/notebooks/ML_Pipeline_with_SageWorks.ipynb
+-rw-r--r--   0 briford    (501) staff       (20)    16418 2024-05-29 15:28:13.000000 sageworks-0.6.8/notebooks/ML_Pipeline_with_SageWorks_2.ipynb
+-rw-r--r--   0 briford    (501) staff       (20)    12554 2024-05-30 16:49:52.000000 sageworks-0.6.8/notebooks/Outliers_in_SageWorks.ipynb
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.055729 sageworks-0.6.8/notebooks/images/
+-rw-r--r--   0 briford    (501) staff       (20)   142099 2023-12-24 17:18:24.000000 sageworks-0.6.8/notebooks/images/athena_query_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   191022 2023-12-24 17:18:24.000000 sageworks-0.6.8/notebooks/images/aws_dashboard_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   222686 2023-12-24 17:18:24.000000 sageworks-0.6.8/notebooks/images/dashboard_aqsol_features.png
+-rw-r--r--   0 briford    (501) staff       (20)   171441 2023-12-24 17:18:24.000000 sageworks-0.6.8/notebooks/images/model_screenshot.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.8/notebooks/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.8/notebooks/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)      196 2024-05-30 17:04:13.000000 sageworks-0.6.8/pyproject.toml
+-rw-r--r--   0 briford    (501) staff       (20)      444 2024-05-19 21:32:59.000000 sageworks-0.6.8/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.058315 sageworks-0.6.8/scripts/
+-rw-r--r--   0 briford    (501) staff       (20)     1710 2024-04-16 15:58:18.000000 sageworks-0.6.8/scripts/ag_table_row_selection.py
+-rw-r--r--   0 briford    (501) staff       (20)     2290 2024-03-28 17:23:43.000000 sageworks-0.6.8/scripts/athena_ddl_mixed_case.py
+-rw-r--r--   0 briford    (501) staff       (20)     2178 2024-03-27 20:32:26.000000 sageworks-0.6.8/scripts/copy_data_catalog_db.py
+-rw-r--r--   0 briford    (501) staff       (20)     1222 2024-04-16 15:58:18.000000 sageworks-0.6.8/scripts/create_glue_workflow_with_trigger.py
+-rw-r--r--   0 briford    (501) staff       (20)      706 2024-01-10 18:45:51.000000 sageworks-0.6.8/scripts/delete_redis_keys.py
+-rw-r--r--   0 briford    (501) staff       (20)     1761 2024-03-28 17:23:43.000000 sageworks-0.6.8/scripts/glue_mixed_case.py
+-rw-r--r--   0 briford    (501) staff       (20)     5544 2024-03-28 17:23:43.000000 sageworks-0.6.8/scripts/model_endpoint_sanity_check.py
+-rw-r--r--   0 briford    (501) staff       (20)      715 2024-03-28 17:23:43.000000 sageworks-0.6.8/scripts/onboard_endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      694 2024-03-28 17:23:43.000000 sageworks-0.6.8/scripts/onboard_models.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.058716 sageworks-0.6.8/scripts/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     1003 2024-03-27 20:32:27.000000 sageworks-0.6.8/scripts/storage/dns_data_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     1723 2024-04-06 16:51:44.000000 sageworks-0.6.8/scripts/storage/generate_jsonl_data.py
+-rw-r--r--   0 briford    (501) staff       (20)      955 2024-03-28 17:23:43.000000 sageworks-0.6.8/scripts/test_feature_resolution.py
+-rw-r--r--   0 briford    (501) staff       (20)      427 2024-05-30 17:23:31.104761 sageworks-0.6.8/setup.cfg
+-rw-r--r--   0 briford    (501) staff       (20)     1657 2024-05-30 17:21:02.000000 sageworks-0.6.8/setup.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:30.993054 sageworks-0.6.8/src/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.059008 sageworks-0.6.8/src/sageworks/
+-rw-r--r--   0 briford    (501) staff       (20)     1091 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.060012 sageworks-0.6.8/src/sageworks/algorithms/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.8/src/sageworks/algorithms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.061767 sageworks-0.6.8/src/sageworks/algorithms/dataframe/
+-rw-r--r--   0 briford    (501) staff       (20)      378 2023-12-24 17:18:24.000000 sageworks-0.6.8/src/sageworks/algorithms/dataframe/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     2852 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/algorithms/dataframe/aggregation.py
+-rw-r--r--   0 briford    (501) staff       (20)     1606 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/algorithms/dataframe/data_source_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)     5388 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/algorithms/dataframe/dimensionality_reduction.py
+-rw-r--r--   0 briford    (501) staff       (20)     9406 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/algorithms/dataframe/feature_resolution.py
+-rw-r--r--   0 briford    (501) staff       (20)    12309 2024-05-28 20:18:51.000000 sageworks-0.6.8/src/sageworks/algorithms/dataframe/feature_spider.py
+-rw-r--r--   0 briford    (501) staff       (20)     4968 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/algorithms/dataframe/row_tagger.py
+-rw-r--r--   0 briford    (501) staff       (20)     4628 2024-03-27 20:32:27.000000 sageworks-0.6.8/src/sageworks/algorithms/dataframe/target_gradients.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:30.993406 sageworks-0.6.8/src/sageworks/algorithms/graph/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.062042 sageworks-0.6.8/src/sageworks/algorithms/graph/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)       96 2023-12-24 17:18:24.000000 sageworks-0.6.8/src/sageworks/algorithms/graph/heavy/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.062316 sageworks-0.6.8/src/sageworks/algorithms/graph/light/
+-rw-r--r--   0 briford    (501) staff       (20)      122 2023-12-24 17:18:24.000000 sageworks-0.6.8/src/sageworks/algorithms/graph/light/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.062526 sageworks-0.6.8/src/sageworks/algorithms/spark/
+-rw-r--r--   0 briford    (501) staff       (20)      615 2023-12-24 17:18:24.000000 sageworks-0.6.8/src/sageworks/algorithms/spark/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.064055 sageworks-0.6.8/src/sageworks/algorithms/sql/
+-rw-r--r--   0 briford    (501) staff       (20)      685 2023-12-24 17:18:24.000000 sageworks-0.6.8/src/sageworks/algorithms/sql/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     6221 2024-05-30 15:14:43.000000 sageworks-0.6.8/src/sageworks/algorithms/sql/column_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)     3666 2024-05-30 14:49:00.000000 sageworks-0.6.8/src/sageworks/algorithms/sql/correlations.py
+-rw-r--r--   0 briford    (501) staff       (20)     4045 2024-05-30 15:05:13.000000 sageworks-0.6.8/src/sageworks/algorithms/sql/descriptive_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)    10377 2024-05-30 16:34:27.000000 sageworks-0.6.8/src/sageworks/algorithms/sql/outliers.py
+-rw-r--r--   0 briford    (501) staff       (20)     2352 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/algorithms/sql/sample_rows.py
+-rw-r--r--   0 briford    (501) staff       (20)     3466 2024-05-30 14:49:00.000000 sageworks-0.6.8/src/sageworks/algorithms/sql/value_counts.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.066372 sageworks-0.6.8/src/sageworks/api/
+-rw-r--r--   0 briford    (501) staff       (20)      708 2024-04-18 20:46:23.000000 sageworks-0.6.8/src/sageworks/api/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7811 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/api/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2634 2024-05-29 14:06:46.000000 sageworks-0.6.8/src/sageworks/api/endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     4224 2024-05-28 21:46:10.000000 sageworks-0.6.8/src/sageworks/api/feature_set.py
+-rw-r--r--   0 briford    (501) staff       (20)    16482 2024-04-21 15:28:58.000000 sageworks-0.6.8/src/sageworks/api/meta.py
+-rw-r--r--   0 briford    (501) staff       (20)     2595 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/api/model.py
+-rw-r--r--   0 briford    (501) staff       (20)     5261 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/api/monitor.py
+-rw-r--r--   0 briford    (501) staff       (20)     6953 2024-04-26 21:22:37.000000 sageworks-0.6.8/src/sageworks/api/pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)     6659 2024-04-26 21:22:37.000000 sageworks-0.6.8/src/sageworks/api/pipeline_manager.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.066969 sageworks-0.6.8/src/sageworks/aws_service_broker/
+-rw-r--r--   0 briford    (501) staff       (20)     9393 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_account_clamp.py
+-rw-r--r--   0 briford    (501) staff       (20)    11198 2024-05-09 14:32:45.000000 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_broker.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.068603 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     1834 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
+-rw-r--r--   0 briford    (501) staff       (20)     3258 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)     4055 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)     5238 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)     3712 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py
+-rw-r--r--   0 briford    (501) staff       (20)     3889 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     3736 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.068753 sageworks-0.6.8/src/sageworks/core/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.071386 sageworks-0.6.8/src/sageworks/core/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      941 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/artifacts/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    17938 2024-04-15 22:06:08.000000 sageworks-0.6.8/src/sageworks/core/artifacts/artifact.py
+-rw-r--r--   0 briford    (501) staff       (20)    22432 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/core/artifacts/athena_source.py
+-rw-r--r--   0 briford    (501) staff       (20)    12683 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/artifacts/data_source_abstract.py
+-rw-r--r--   0 briford    (501) staff       (20)     2447 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/artifacts/data_source_factory.py
+-rw-r--r--   0 briford    (501) staff       (20)    37061 2024-05-29 13:52:08.000000 sageworks-0.6.8/src/sageworks/core/artifacts/endpoint_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    29698 2024-04-22 20:46:36.000000 sageworks-0.6.8/src/sageworks/core/artifacts/feature_set_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    36644 2024-05-29 18:45:32.000000 sageworks-0.6.8/src/sageworks/core/artifacts/model_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    21029 2024-05-28 20:40:35.000000 sageworks-0.6.8/src/sageworks/core/artifacts/monitor_core.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.071725 sageworks-0.6.8/src/sageworks/core/pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)     6919 2024-04-26 21:22:37.000000 sageworks-0.6.8/src/sageworks/core/pipelines/pipeline_executor.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.072407 sageworks-0.6.8/src/sageworks/core/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)     1432 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.072692 sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.073165 sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)      298 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/heavy/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     9866 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.074309 sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/light/
+-rw-r--r--   0 briford    (501) staff       (20)      543 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3011 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2927 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     4225 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.074638 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.074766 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.074890 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.075180 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.075743 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2237 2024-03-27 20:40:53.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/light/clean_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     2687 2024-03-27 20:40:53.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.075988 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.076101 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.076317 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/chunk/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/chunk/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     4551 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.076666 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.076834 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.077000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     6702 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.077633 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3827 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py
+-rw-r--r--   0 briford    (501) staff       (20)     5674 2024-04-23 15:16:38.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.077965 sageworks-0.6.8/src/sageworks/core/transforms/features_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/features_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:30.995463 sageworks-0.6.8/src/sageworks/core/transforms/features_to_features/heavy/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.078074 sageworks-0.6.8/src/sageworks/core/transforms/features_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/features_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.078223 sageworks-0.6.8/src/sageworks/core/transforms/features_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/features_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.078473 sageworks-0.6.8/src/sageworks/core/transforms/features_to_model/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/features_to_model/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    13050 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/features_to_model/features_to_model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.079273 sageworks-0.6.8/src/sageworks/core/transforms/features_to_model/light_model_harness/
+-rw-r--r--   0 briford    (501) staff       (20)    13982 2024-05-28 20:18:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/features_to_model/light_model_harness/generated_xgb_model.py
+-rw-r--r--   0 briford    (501) staff       (20)       19 2024-02-27 23:40:48.000000 sageworks-0.6.8/src/sageworks/core/transforms/features_to_model/light_model_harness/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)    10806 2024-05-28 20:18:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.079678 sageworks-0.6.8/src/sageworks/core/transforms/model_to_endpoint/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/model_to_endpoint/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     8185 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.081035 sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      894 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3615 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     3445 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     8604 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)    18139 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     4440 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py
+-rw-r--r--   0 briford    (501) staff       (20)     5391 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/transform.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.081243 sageworks-0.6.8/src/sageworks/experiments/
+-rw-r--r--   0 briford    (501) staff       (20)    10658 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/experiments/view_manager.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.081636 sageworks-0.6.8/src/sageworks/repl/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/repl/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    15486 2024-04-21 15:35:25.000000 sageworks-0.6.8/src/sageworks/repl/sageworks_shell.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.082149 sageworks-0.6.8/src/sageworks/resources/
+-rw-r--r--   0 briford    (501) staff       (20)      361 2024-01-23 15:36:53.000000 sageworks-0.6.8/src/sageworks/resources/open_source_api.key
+-rw-r--r--   0 briford    (501) staff       (20)      272 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/resources/signature_verify_pub.pem
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.089062 sageworks-0.6.8/src/sageworks/utils/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.8/src/sageworks/utils/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    15587 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/utils/aws_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5447 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/utils/cache.py
+-rw-r--r--   0 briford    (501) staff       (20)      722 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/chem_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    16543 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/utils/config_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     7392 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/dashboard_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)     4194 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/utils/datetime_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5292 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/df_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     1681 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/docker_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2866 2024-03-27 20:43:31.000000 sageworks-0.6.8/src/sageworks/utils/ecs_info.py
+-rw-r--r--   0 briford    (501) staff       (20)     7657 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/endpoint_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)     3098 2024-05-28 20:18:49.000000 sageworks-0.6.8/src/sageworks/utils/endpoint_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     6979 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/extract_model_artifact.py
+-rw-r--r--   0 briford    (501) staff       (20)     1131 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/glue_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     6404 2024-05-20 15:33:17.000000 sageworks-0.6.8/src/sageworks/utils/license_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     1439 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/utils/markdown_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    15517 2024-04-22 20:45:19.000000 sageworks-0.6.8/src/sageworks/utils/pandas_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    12684 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/utils/plugin_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     9533 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/utils/redis_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     4166 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/repl_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2089 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/s3_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2163 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/sageworks_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     3474 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/sageworks_event_bridge.py
+-rw-r--r--   0 briford    (501) staff       (20)     5359 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/sageworks_logging.py
+-rw-r--r--   0 briford    (501) staff       (20)     2120 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/sageworks_sqs.py
+-rw-r--r--   0 briford    (501) staff       (20)     1108 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/utils/symbols.py
+-rw-r--r--   0 briford    (501) staff       (20)     6414 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/test_data_generator.py
+-rw-r--r--   0 briford    (501) staff       (20)     2092 2024-03-27 20:43:31.000000 sageworks-0.6.8/src/sageworks/utils/trace_calls.py
+-rw-r--r--   0 briford    (501) staff       (20)     1470 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/type_abbrev.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.090585 sageworks-0.6.8/src/sageworks/views/
+-rw-r--r--   0 briford    (501) staff       (20)     3517 2024-04-16 22:29:17.000000 sageworks-0.6.8/src/sageworks/views/artifacts_text_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     7780 2024-04-28 17:17:45.000000 sageworks-0.6.8/src/sageworks/views/artifacts_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     3158 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/views/data_source_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     2150 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/views/endpoint_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     3206 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/views/feature_set_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/views/model_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     1092 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/views/view.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.093567 sageworks-0.6.8/src/sageworks/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)     5916 2024-04-25 23:06:38.000000 sageworks-0.6.8/src/sageworks/web_components/component_interface.py
+-rw-r--r--   0 briford    (501) staff       (20)     3525 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/web_components/confusion_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     5854 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/web_components/correlation_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     9328 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/web_components/data_details_markdown.py
+-rw-r--r--   0 briford    (501) staff       (20)     3068 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/web_components/endpoint_metric_plots.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.095682 sageworks-0.6.8/src/sageworks/web_components/experiments/
+-rw-r--r--   0 briford    (501) staff       (20)      837 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/color_maps.py
+-rw-r--r--   0 briford    (501) staff       (20)     1633 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/compound_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2974 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/dashboard_metric_plots.py
+-rw-r--r--   0 briford    (501) staff       (20)     2240 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/data_table.py
+-rw-r--r--   0 briford    (501) staff       (20)     2453 2024-04-02 16:53:34.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/graph_test.py
+-rw-r--r--   0 briford    (501) staff       (20)     1765 2024-04-02 16:53:34.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/hello.py
+-rw-r--r--   0 briford    (501) staff       (20)     1183 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/histogram.py
+-rw-r--r--   0 briford    (501) staff       (20)      838 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/line_chart.py
+-rw-r--r--   0 briford    (501) staff       (20)     3680 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/outlier_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     2373 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/plugin_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2279 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/scatter_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     2278 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/web_components/model_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     7681 2024-05-27 16:52:27.000000 sageworks-0.6.8/src/sageworks/web_components/plugin_interface.py
+-rw-r--r--   0 briford    (501) staff       (20)     3627 2024-05-27 19:18:14.000000 sageworks-0.6.8/src/sageworks/web_components/plugin_unit_test.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.096865 sageworks-0.6.8/src/sageworks/web_components/plugins/
+-rw-r--r--   0 briford    (501) staff       (20)     2786 2024-04-26 21:04:42.000000 sageworks-0.6.8/src/sageworks/web_components/plugins/ag_table.py
+-rw-r--r--   0 briford    (501) staff       (20)     3749 2024-05-28 15:15:12.000000 sageworks-0.6.8/src/sageworks/web_components/plugins/endpoint_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     5498 2024-05-22 14:54:18.000000 sageworks-0.6.8/src/sageworks/web_components/plugins/license_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     7607 2024-05-29 18:44:03.000000 sageworks-0.6.8/src/sageworks/web_components/plugins/model_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2429 2024-04-26 21:22:37.000000 sageworks-0.6.8/src/sageworks/web_components/plugins/pipeline_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2959 2024-05-29 15:29:46.000000 sageworks-0.6.8/src/sageworks/web_components/regression_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     6838 2024-05-06 17:24:24.000000 sageworks-0.6.8/src/sageworks/web_components/table.py
+-rw-r--r--   0 briford    (501) staff       (20)     5185 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/web_components/violin_plots.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.103860 sageworks-0.6.8/src/sageworks.egg-info/
+-rw-r--r--   0 briford    (501) staff       (20)     4961 2024-05-30 17:23:30.000000 sageworks-0.6.8/src/sageworks.egg-info/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)    19412 2024-05-30 17:23:30.000000 sageworks-0.6.8/src/sageworks.egg-info/SOURCES.txt
+-rw-r--r--   0 briford    (501) staff       (20)        1 2024-05-30 17:23:30.000000 sageworks-0.6.8/src/sageworks.egg-info/dependency_links.txt
+-rw-r--r--   0 briford    (501) staff       (20)       74 2024-05-30 17:23:30.000000 sageworks-0.6.8/src/sageworks.egg-info/entry_points.txt
+-rw-r--r--   0 briford    (501) staff       (20)      421 2024-05-30 17:23:30.000000 sageworks-0.6.8/src/sageworks.egg-info/requires.txt
+-rw-r--r--   0 briford    (501) staff       (20)       10 2024-05-30 17:23:30.000000 sageworks-0.6.8/src/sageworks.egg-info/top_level.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.098055 sageworks-0.6.8/tests/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.098874 sageworks-0.6.8/tests/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)     1548 2024-03-30 19:27:28.000000 sageworks-0.6.8/tests/artifacts/data_source_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     2442 2024-05-28 20:18:51.000000 sageworks-0.6.8/tests/artifacts/endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1160 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/artifacts/feature_set_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      805 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/artifacts/model_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.099285 sageworks-0.6.8/tests/aws_account/
+-rw-r--r--   0 briford    (501) staff       (20)      962 2023-12-24 17:18:24.000000 sageworks-0.6.8/tests/aws_account/aws_account_clamp_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      642 2023-12-24 17:18:24.000000 sageworks-0.6.8/tests/aws_account/aws_service_broker_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.100337 sageworks-0.6.8/tests/connectors/
+-rw-r--r--   0 briford    (501) staff       (20)      725 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)      737 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      702 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)      644 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/connectors/glue_jobs.py
+-rw-r--r--   0 briford    (501) staff       (20)      799 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     1008 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/connectors/s3_bucket.py
+-rw-r--r--   0 briford    (501) staff       (20)     5618 2024-04-26 21:04:42.000000 sageworks-0.6.8/tests/create_aqsol_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     3217 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/create_basic_test_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)      870 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/create_realtime_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     2378 2024-04-22 20:46:36.000000 sageworks-0.6.8/tests/create_training_adjusted_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     2096 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/create_wine_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     4448 2024-04-16 15:58:18.000000 sageworks-0.6.8/tests/delete_test_artifacts.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.100483 sageworks-0.6.8/tests/plugin_tests/
+-rw-r--r--   0 briford    (501) staff       (20)     1885 2024-04-16 15:58:18.000000 sageworks-0.6.8/tests/plugin_tests/crashing_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.100763 sageworks-0.6.8/tests/specific/
+-rw-r--r--   0 briford    (501) staff       (20)      639 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/specific/capital_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1513 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/specific/deletion_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.101846 sageworks-0.6.8/tests/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      592 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/transforms/data_to_data_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1025 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/transforms/data_to_features_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      773 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/transforms/features_to_model_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     5134 2024-05-29 18:44:03.000000 sageworks-0.6.8/tests/transforms/model_metrics_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      795 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/transforms/model_to_endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      633 2024-03-27 20:40:53.000000 sageworks-0.6.8/tests/transforms/pandas_to_data_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.102548 sageworks-0.6.8/tests/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)      681 2024-04-16 15:58:18.000000 sageworks-0.6.8/tests/web_components/confusion_matrix_test.py
+-rw-r--r--   0 briford    (501) staff       (20)      677 2024-04-16 15:58:18.000000 sageworks-0.6.8/tests/web_components/correlation_matrix_test.py
+-rw-r--r--   0 briford    (501) staff       (20)     5269 2024-04-16 15:58:18.000000 sageworks-0.6.8/tests/web_components/plugin_interface_test.py
+-rw-r--r--   0 briford    (501) staff       (20)     1112 2024-05-29 18:21:35.000000 sageworks-0.6.8/tox.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.103324 sageworks-0.6.8/ui_testing/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.103548 sageworks-0.6.8/ui_testing/assets/
+-rw-r--r--   0 briford    (501) staff       (20)      597 2024-05-13 15:14:49.000000 sageworks-0.6.8/ui_testing/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)     5770 2024-05-19 19:25:10.000000 sageworks-0.6.8/ui_testing/table_comparison.py
+-rw-r--r--   0 briford    (501) staff       (20)     2025 2024-05-19 19:25:10.000000 sageworks-0.6.8/ui_testing/theme_switching.py
+-rw-r--r--   0 briford    (501) staff       (20)     1819 2024-05-19 19:25:10.000000 sageworks-0.6.8/ui_testing/theme_switching_2.py
```

### Comparing `sageworks-0.6.6/.github/PULL_REQUEST_TEMPLATE.md` & `sageworks-0.6.8/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/.github/workflows/deploy-docs.yml` & `sageworks-0.6.8/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/.github/workflows/python-lint.yml` & `sageworks-0.6.8/.github/workflows/python-lint.yml`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/.gitignore` & `sageworks-0.6.8/.gitignore`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/CONTRIBUTING.md` & `sageworks-0.6.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/LICENSE` & `sageworks-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/Makefile` & `sageworks-0.6.8/Makefile`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/PKG-INFO` & `sageworks-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.6.6
+Version: 0.6.8
 Summary: SageWorks: A Python WorkBench for creating and deploying AWS SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sageworks-0.6.6/README.md` & `sageworks-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/Dockerfile` & `sageworks-0.6.8/applications/aws_dashboard/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 RUN pip install --no-cache-dir -r requirements.txt
 
 # Copy the Nginx and Supervisor configuration files
 COPY nginx.conf /etc/nginx/sites-available/default
 COPY supervisord.conf /etc/supervisor/conf.d/supervisord.conf
 
 # Install Sageworks (changes often)
-RUN pip install --no-cache-dir sageworks==0.6.5
+RUN pip install --no-cache-dir sageworks==0.6.6
 
 # Copy the current directory contents into the container at /app
 COPY . /app
 
 # Grab the config file from build args, copy, and set ENV var
 ARG SAGEWORKS_CONFIG
 COPY $SAGEWORKS_CONFIG /app/sageworks_config.json
```

### Comparing `sageworks-0.6.6/applications/aws_dashboard/README.md` & `sageworks-0.6.8/applications/aws_dashboard/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/app.py` & `sageworks-0.6.8/applications/aws_dashboard/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/assets/bootstrap_darkly.min.css` & `sageworks-0.6.8/applications/aws_dashboard/assets/bootstrap_darkly.min.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/assets/default.css` & `sageworks-0.6.8/applications/aws_dashboard/assets/default.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/assets/favicon.ico` & `sageworks-0.6.8/applications/aws_dashboard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/assets/trash.png` & `sageworks-0.6.8/applications/aws_dashboard/assets/trash.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/dashboard` & `sageworks-0.6.8/applications/aws_dashboard/dashboard`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/open_source_config.json` & `sageworks-0.6.8/applications/aws_dashboard/open_source_config.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/pages/data_sources/callbacks.py` & `sageworks-0.6.8/applications/aws_dashboard/pages/data_sources/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/pages/data_sources/layout.py` & `sageworks-0.6.8/applications/aws_dashboard/pages/data_sources/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/pages/data_sources/page.py` & `sageworks-0.6.8/applications/aws_dashboard/pages/data_sources/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/pages/endpoints/callbacks.py` & `sageworks-0.6.8/applications/aws_dashboard/pages/endpoints/callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,20 @@
 
         # Return the details/markdown for these data details
         return endpoint_metrics_figure
 
 
 # Set up the plugin callbacks that take an endpoint
 def setup_plugin_callbacks(plugins):
+
+    # First we'll register internal callbacks for the plugins
+    for plugin in plugins:
+        plugin.register_internal_callbacks()
+
+    # Now we'll set up the plugin callbacks for their main inputs (endpoints in this case)
     @callback(
         # Aggregate plugin outputs
         [Output(component_id, prop) for p in plugins for component_id, prop in p.properties],
         Input("endpoints_table", "derived_viewport_selected_row_ids"),
         State("endpoints_table", "data"),
     )
     def update_all_plugin_properties(selected_rows, table_data):
```

### Comparing `sageworks-0.6.6/applications/aws_dashboard/pages/endpoints/layout.py` & `sageworks-0.6.8/applications/aws_dashboard/pages/endpoints/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/pages/endpoints/page.py` & `sageworks-0.6.8/applications/aws_dashboard/pages/endpoints/page.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from dash_bootstrap_templates import load_figure_template
 
 # Local Imports
 from .layout import endpoints_layout
 from . import callbacks
 
 # SageWorks Imports
-from sageworks.web_components import table, endpoint_details, endpoint_metric_plots
+from sageworks.web_components import table, endpoint_metric_plots
+from sageworks.web_components.plugins import endpoint_details
 from sageworks.web_components.plugin_interface import PluginPage
 from sageworks.views.endpoint_web_view import EndpointWebView
 from sageworks.utils.plugin_manager import PluginManager
 
 # Register this page with Dash
 register_page(
     __name__,
@@ -46,26 +47,28 @@
     "endpoint_metrics": endpoint_metrics,
 }
 
 # Load any web components plugins of type 'endpoint'
 pm = PluginManager()
 plugins = pm.get_list_of_web_plugins(plugin_page=PluginPage.ENDPOINT)
 
+# Our endpoint details is a plugin, so we need to add it to the list
+plugins.append(endpoint_details)
+
 # Add the plugins to the components dictionary
 for plugin in plugins:
     component_id = plugin.generate_component_id()
     components[component_id] = plugin.create_component(component_id)
 
 # Set up our layout (Dash looks for a var called layout)
 layout = endpoints_layout(**components)
 
 # Setup our callbacks/connections
 app = dash.get_app()
 callbacks.update_endpoints_table(app)
-endpoint_details.register_callbacks("endpoints_table")
 
 # Callback for the endpoints table
 callbacks.table_row_select(app, "endpoints_table")
 callbacks.update_endpoint_metrics(app, endpoint_broker)
 
 # For all the plugins we have we'll call their update_properties method
 if plugins:
```

### Comparing `sageworks-0.6.6/applications/aws_dashboard/pages/feature_sets/callbacks.py` & `sageworks-0.6.8/applications/aws_dashboard/pages/feature_sets/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/pages/feature_sets/layout.py` & `sageworks-0.6.8/applications/aws_dashboard/pages/feature_sets/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/pages/feature_sets/page.py` & `sageworks-0.6.8/applications/aws_dashboard/pages/feature_sets/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/pages/license/page.py` & `sageworks-0.6.8/applications/aws_dashboard/pages/license/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/pages/main/callbacks.py` & `sageworks-0.6.8/applications/aws_dashboard/pages/main/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/pages/main/layout.py` & `sageworks-0.6.8/applications/aws_dashboard/pages/main/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/pages/main/page.py` & `sageworks-0.6.8/applications/aws_dashboard/pages/main/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/pages/models/callbacks.py` & `sageworks-0.6.8/applications/aws_dashboard/pages/models/callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,20 +49,21 @@
         symbol_style = {"if": {"column_id": "Health"}, "fontSize": 16, "textAlign": "left"}
 
         # Append the symbol style to the row style
         row_style.append(symbol_style)
         return row_style
 
 
-# Updates the model plot when a model row is selected
+# Updates the model plot when the model inference run is changed
 def update_model_plot_component(app: Dash):
     @app.callback(
         Output("model_plot", "figure"),
         Input("model_details-dropdown", "value"),
-        [State("models_table", "data"), State("models_table", "derived_viewport_selected_row_ids")],
+        State("models_table", "data"),
+        State("models_table", "derived_viewport_selected_row_ids"),
         prevent_initial_call=True,
     )
     def generate_model_plot_figure(inference_run, table_data, selected_rows):
         # Check for no selected rows
         if not selected_rows or selected_rows[0] is None:
             return no_update
 
@@ -75,18 +76,24 @@
         model_plot_fig = model_plot.ModelPlot().update_properties(m, inference_run)
 
         # Return the details/markdown for these data details
         return model_plot_fig
 
 
 def setup_plugin_callbacks(plugins):
+
+    # First we'll register internal callbacks for the plugins
+    for plugin in plugins:
+        plugin.register_internal_callbacks()
+
+    # Now we'll set up the plugin callbacks for their main inputs (models in this case)
     @callback(
         # Aggregate plugin outputs
         [Output(component_id, prop) for p in plugins for component_id, prop in p.properties],
-        Input("model_details-dropdown", "value"),
+        State("model_details-dropdown", "value"),
         Input("models_table", "derived_viewport_selected_row_ids"),
         State("models_table", "data"),
     )
     def update_all_plugin_properties(inference_run, selected_rows, table_data):
         # Check for no selected rows
         if not selected_rows or selected_rows[0] is None:
             raise PreventUpdate
```

### Comparing `sageworks-0.6.6/applications/aws_dashboard/pages/models/layout.py` & `sageworks-0.6.8/applications/aws_dashboard/pages/models/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/pages/models/page.py` & `sageworks-0.6.8/applications/aws_dashboard/pages/models/page.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,19 +5,16 @@
 from dash_bootstrap_templates import load_figure_template
 
 # Local Imports
 from .layout import models_layout
 from . import callbacks
 
 # SageWorks Imports
-from sageworks.web_components import (
-    table,
-    model_details,
-    model_plot,
-)
+from sageworks.web_components import table, model_plot
+from sageworks.web_components.plugins import model_details
 from sageworks.web_components.plugin_interface import PluginPage
 from sageworks.utils.plugin_manager import PluginManager
 
 # Register this page with Dash
 register_page(
     __name__,
     path="/models",
@@ -46,26 +43,28 @@
     "model_plot": model_plot_component,
 }
 
 # Load any web components plugins of type 'model'
 pm = PluginManager()
 plugins = pm.get_list_of_web_plugins(plugin_page=PluginPage.MODEL)
 
+# Our model details is a plugin, so we need to add it to the list
+plugins.append(model_details)
+
 # Add the plugins to the components dictionary
 for plugin in plugins:
     component_id = plugin.generate_component_id()
     components[component_id] = plugin.create_component(component_id)
 
 # Set up our layout (Dash looks for a var called layout)
 layout = models_layout(**components)
 
 # Setup our callbacks/connections
 app = dash.get_app()
 callbacks.update_models_table(app)
-model_details.register_callbacks("models_table")
 
 # Callback for the model table
 callbacks.table_row_select(app, "models_table")
 callbacks.update_model_plot_component(app)
 
 # Set up callbacks for all the plugins
 if plugins:
```

### Comparing `sageworks-0.6.6/applications/aws_dashboard/pages/pipelines/callbacks.py` & `sageworks-0.6.8/applications/aws_dashboard/pages/pipelines/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/pages/pipelines/layout.py` & `sageworks-0.6.8/applications/aws_dashboard/pages/pipelines/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/aws_dashboard/pages/pipelines/page.py` & `sageworks-0.6.8/applications/aws_dashboard/pages/pipelines/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/experiments/compound_explorer/app.py` & `sageworks-0.6.8/applications/experiments/compound_explorer/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/experiments/compound_explorer/assets/custom.css` & `sageworks-0.6.8/applications/experiments/compound_explorer/assets/custom.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/experiments/compound_explorer/callbacks.py` & `sageworks-0.6.8/applications/experiments/compound_explorer/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/applications/experiments/compound_explorer/layout.py` & `sageworks-0.6.8/applications/experiments/compound_explorer/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/aws_account_check.py` & `sageworks-0.6.8/aws_setup/aws_account_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/aws_identity_check.py` & `sageworks-0.6.8/aws_setup/aws_identity_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/build_ml_pipeline.py` & `sageworks-0.6.8/aws_setup/build_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/app.py` & `sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/cdk.json` & `sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py` & `sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py` & `sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/sageworks_core/README.md` & `sageworks-0.6.8/aws_setup/sageworks_core/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/sageworks_core/app.py` & `sageworks-0.6.8/aws_setup/sageworks_core/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/sageworks_core/cdk.json` & `sageworks-0.6.8/aws_setup/sageworks_core/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py` & `sageworks-0.6.8/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py` & `sageworks-0.6.8/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/sageworks_dashboard_full/README.md` & `sageworks-0.6.8/aws_setup/sageworks_dashboard_full/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/sageworks_dashboard_full/app.py` & `sageworks-0.6.8/aws_setup/sageworks_dashboard_full/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/sageworks_dashboard_full/cdk.json` & `sageworks-0.6.8/aws_setup/sageworks_dashboard_full/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py` & `sageworks-0.6.8/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py` & `sageworks-0.6.8/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/README.md` & `sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/app.py` & `sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/cdk.json` & `sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py` & `sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     aws_logs as logs,
 )
 from aws_cdk.aws_certificatemanager import Certificate
 from aws_cdk.aws_ecs_patterns import ApplicationLoadBalancedFargateService
 from constructs import Construct
 
 # When you want a different version change this line
-dashboard_image = "public.ecr.aws/m6i5k1r2/sageworks_dashboard:v0_6_5_amd64"
+dashboard_image = "public.ecr.aws/m6i5k1r2/sageworks_dashboard:v0_6_6_amd64"
 
 
 class SageworksDashboardStackProps(StackProps):
     def __init__(
         self,
         sageworks_bucket: str,
         sageworks_api_key: str,
```

### Comparing `sageworks-0.6.6/data/abalone.csv` & `sageworks-0.6.8/data/abalone.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/data/test_data.csv` & `sageworks-0.6.8/data/test_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/data/test_data.json` & `sageworks-0.6.8/data/test_data.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/data/wine_dataset.csv` & `sageworks-0.6.8/data/wine_dataset.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/admin/docker_push.md` & `sageworks-0.6.8/docs/admin/docker_push.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/admin/pypi_release.md` & `sageworks-0.6.8/docs/admin/pypi_release.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 [Packaging](https://packaging.python.org/tutorials/packaging-projects/#packaging-your-project)
 
 The following instructions should work, but things change :)
 
 ### Package Requirements
 
 -   pip install tox
--   pip install \--upgrade setuptools wheel
--   pip install twine
+-   pip install \--upgrade wheel build twine
 
 ### Setup pypirc
 
 The easiest thing to do is setup a \~/.pypirc file with the following
 contents
 
 ``` {.bash}
@@ -54,15 +53,15 @@
 git tag v0.1.8 (or whatever)
 git push --tags
 ```
 
 ### Create the TEST PyPI Release
 
 ``` {.bash}
-python setup.py sdist bdist_wheel
+python -m build
 twine upload dist/* -r testpypi
 ```
 
 ### Install the TEST PyPI Release
 
 ``` {.bash}
 pip install --index-url https://test.pypi.org/simple sageworks
```

### Comparing `sageworks-0.6.6/docs/api_classes/data_source.md` & `sageworks-0.6.8/docs/api_classes/data_source.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/api_classes/endpoint.md` & `sageworks-0.6.8/docs/api_classes/endpoint.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/api_classes/feature_set.md` & `sageworks-0.6.8/docs/api_classes/feature_set.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/api_classes/meta.md` & `sageworks-0.6.8/docs/api_classes/meta.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/api_classes/model.md` & `sageworks-0.6.8/docs/api_classes/model.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/api_classes/monitor.md` & `sageworks-0.6.8/docs/api_classes/monitor.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/api_classes/overview.md` & `sageworks-0.6.8/docs/api_classes/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/api_classes/pipelines.md` & `sageworks-0.6.8/docs/api_classes/pipelines.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/aws_setup/aws_access_management.md` & `sageworks-0.6.8/docs/aws_setup/aws_access_management.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/aws_setup/aws_tips_and_tricks.md` & `sageworks-0.6.8/docs/aws_setup/aws_tips_and_tricks.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/aws_setup/core_stack.md` & `sageworks-0.6.8/docs/aws_setup/core_stack.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/aws_setup/dashboard_stack.md` & `sageworks-0.6.8/docs/aws_setup/dashboard_stack.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/aws_setup/domain_cert_setup.md` & `sageworks-0.6.8/docs/aws_setup/domain_cert_setup.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/aws_setup/full_pipeline.md` & `sageworks-0.6.8/docs/aws_setup/full_pipeline.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/aws_setup/sso_setup.md` & `sageworks-0.6.8/docs/aws_setup/sso_setup.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/blogs_research/eda.md` & `sageworks-0.6.8/docs/blogs_research/eda.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/blogs_research/htg.md` & `sageworks-0.6.8/docs/blogs_research/htg.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/blogs_research/index.md` & `sageworks-0.6.8/docs/blogs_research/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/blogs_research/residual_analysis.md` & `sageworks-0.6.8/docs/blogs_research/residual_analysis.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/concepts/model_monitoring.md` & `sageworks-0.6.8/docs/concepts/model_monitoring.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/core_classes/artifacts/overview.md` & `sageworks-0.6.8/docs/core_classes/artifacts/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/core_classes/overview.md` & `sageworks-0.6.8/docs/core_classes/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/core_classes/transforms/overview.md` & `sageworks-0.6.8/docs/core_classes/transforms/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/core_classes/transforms/pandas_transforms.md` & `sageworks-0.6.8/docs/core_classes/transforms/pandas_transforms.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/core_classes/transforms/transform.md` & `sageworks-0.6.8/docs/core_classes/transforms/transform.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/enterprise/index.md` & `sageworks-0.6.8/docs/enterprise/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/enterprise/project_branding.md` & `sageworks-0.6.8/docs/enterprise/project_branding.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/enterprise/themes.md` & `sageworks-0.6.8/docs/enterprise/themes.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/getting_started/index.md` & `sageworks-0.6.8/docs/getting_started/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/glue/index.md` & `sageworks-0.6.8/docs/glue/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/images/big_spider.png` & `sageworks-0.6.8/docs/images/big_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/images/graph_representation.png` & `sageworks-0.6.8/docs/images/graph_representation.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/images/powered_aws_dark_blue.png` & `sageworks-0.6.8/docs/images/powered_aws_dark_blue.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/images/powered_aws_transparent.png` & `sageworks-0.6.8/docs/images/powered_aws_transparent.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/images/powered_aws_white.png` & `sageworks-0.6.8/docs/images/powered_aws_white.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/images/powered_aws_with_tm_grey.png` & `sageworks-0.6.8/docs/images/powered_aws_with_tm_grey.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/images/sageworks.png` & `sageworks-0.6.8/docs/images/sageworks.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/images/sageworks_concepts.png` & `sageworks-0.6.8/docs/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/images/scp.png` & `sageworks-0.6.8/docs/images/scp.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/images/scp_labs.png` & `sageworks-0.6.8/docs/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/images/small_spider.png` & `sageworks-0.6.8/docs/images/small_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/index.md` & `sageworks-0.6.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/misc/faq.md` & `sageworks-0.6.8/docs/misc/faq.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/misc/general_info.md` & `sageworks-0.6.8/docs/misc/general_info.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/misc/sageworks_classes_concepts.md` & `sageworks-0.6.8/docs/misc/sageworks_classes_concepts.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/misc/scp_consulting.md` & `sageworks-0.6.8/docs/misc/scp_consulting.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/plugins/index.md` & `sageworks-0.6.8/docs/plugins/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/plugins/plugin_api_changes.md` & `sageworks-0.6.8/docs/plugins/plugin_api_changes.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/docs/repl/index.md` & `sageworks-0.6.8/docs/repl/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/datasource/datasource_query.py` & `sageworks-0.6.8/examples/datasource/datasource_query.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/datasource/datasource_stats.py` & `sageworks-0.6.8/examples/datasource/datasource_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/endpoint/endpoint_inference.py` & `sageworks-0.6.8/examples/endpoint/endpoint_inference.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/featureset/featureset_eda.py` & `sageworks-0.6.8/examples/featureset/featureset_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/featureset/featureset_query.py` & `sageworks-0.6.8/examples/featureset/featureset_query.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/full_ml_pipeline.py` & `sageworks-0.6.8/examples/full_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/glue/glue_hello_world.py` & `sageworks-0.6.8/examples/glue/glue_hello_world.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/glue/glue_hello_world_with_log.py` & `sageworks-0.6.8/examples/glue/glue_hello_world_with_log.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/glue/glue_load_s3_bucket.py` & `sageworks-0.6.8/examples/glue/glue_load_s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/meta/meta_model_metrics.py` & `sageworks-0.6.8/examples/meta/meta_model_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/model/model_metrics.py` & `sageworks-0.6.8/examples/model/model_metrics.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 if not health_issues:
     print("Model is Healthy")
 else:
     print("Model has issues")
     print(health_issues)
 
 # Get the model metrics and regression predictions
-print(model.performance_metrics())
-print(model.predictions())
+print(model.get_inference_metrics())
+print(model.get_inference_predictions())
```

### Comparing `sageworks-0.6.6/examples/model/onboard_model.py` & `sageworks-0.6.8/examples/model/onboard_model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/monitor/monitor_usage.py` & `sageworks-0.6.8/examples/monitor/monitor_usage.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/pipelines/abalone_pipeline_v1.json` & `sageworks-0.6.8/examples/pipelines/abalone_pipeline_v1.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/pipelines/abalone_pipeline_v2.json` & `sageworks-0.6.8/examples/pipelines/abalone_pipeline_v2.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/pipelines/aqsol_pipeline_v1.json` & `sageworks-0.6.8/examples/pipelines/aqsol_pipeline_v1.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/pipelines/pipeline_manager.py` & `sageworks-0.6.8/examples/pipelines/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/plugins/pages/my_plugin_page.py` & `sageworks-0.6.8/examples/plugins/pages/my_plugin_page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/plugins/pages/plugin_page_1.py` & `sageworks-0.6.8/examples/plugins/pages/plugin_page_1.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/plugins/pages/plugin_page_2.py` & `sageworks-0.6.8/examples/plugins/pages/plugin_page_2.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/plugins/pages/plugin_page_3.py` & `sageworks-0.6.8/examples/plugins/pages/plugin_page_3.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Plugin Page 1:  A 'Hello World' SageWorks Plugin Page"""
 
 import dash
 from dash import html, page_container, register_page, callback, Output, Input, State, no_update
+from dash.exceptions import PreventUpdate
 import dash_bootstrap_components as dbc
 
 # SageWorks Imports
 from sageworks.web_components import table
 from sageworks.api.meta import Meta
-from sageworks.web_components.model_details import ModelDetails
+from sageworks.web_components.plugins.model_details import ModelDetails
 from sageworks.web_components.model_plot import ModelPlot
 from sageworks.api.model import Model
 
 
 class PluginPage3:
     """Plugin Page:  A SageWorks Plugin Web Interface"""
 
@@ -21,14 +22,15 @@
         self.models_table = table.Table()
         self.table_component = None
         self.model_details = ModelDetails()
         self.details_component = None
         self.model_plot = ModelPlot()
         self.plot_component = None
         self.meta = Meta()
+        self.plugins = [self.model_details]  # Add any additional plugins here
 
     def page_setup(self, app: dash.Dash):
         """Required function to set up the page"""
 
         # Create a table to display the models
         self.table_component = self.models_table.create_component(
             "plugin_3_model_table", header_color="rgb(60, 60, 60)", row_select="single", max_height=400
@@ -51,15 +53,16 @@
         models["uuid"] = models["Model Group"]
         models["id"] = range(len(models))
         self.table_component.columns = self.models_table.column_setup(models)
         self.table_component.data = models.to_dict("records")
 
         # Register the callbacks
         self.register_app_callbacks(app)
-        self.model_details.register_callbacks("plugin_3_model_table")
+        self.setup_plugin_callbacks()
+        self.model_details.register_internal_callbacks()
 
     def page_layout(self) -> dash.html.Div:
         """Set up the layout for the page"""
         layout = dash.html.Div(
             children=[
                 dash.html.H1(self.page_name),
                 dbc.Row(self.table_component),
@@ -72,39 +75,65 @@
             ]
         )
         return layout
 
     def register_app_callbacks(self, app: dash.Dash):
         """Register the callbacks for the page"""
 
-        @app.callback(
+        @callback(
             Output("plugin_3_model_plot", "figure"),
-            [
-                Input("plugin_3_model_details-dropdown", "value"),
-                Input("plugin_3_model_table", "derived_viewport_selected_row_ids"),
-            ],
+            Input("plugin_3_model_details-dropdown", "value"),
             State("plugin_3_model_table", "data"),
+            State("plugin_3_model_table", "derived_viewport_selected_row_ids"),
             prevent_initial_call=True,
         )
-        def generate_model_plot_figure(inference_run, selected_rows, table_data):
+        def generate_model_plot_figure(inference_run, table_data, selected_rows):
             # Check for no selected rows
             if not selected_rows or selected_rows[0] is None:
                 return no_update
 
             # Get the selected row data and grab the uuid
             selected_row_data = table_data[selected_rows[0]]
             model_uuid = selected_row_data["uuid"]
-            model = Model(model_uuid, legacy=True)
+            m = Model(model_uuid, legacy=True)
 
             # Model Details Markdown component
-            model_plot_fig = self.model_plot.update_properties(model, inference_run)
+            model_plot_fig = self.model_plot.update_properties(m, inference_run)
 
             # Return the details/markdown for these data details
             return model_plot_fig
 
+    def setup_plugin_callbacks(self):
+        @callback(
+            # Aggregate plugin outputs
+            [Output(component_id, prop) for p in self.plugins for component_id, prop in p.properties],
+            State("plugin_3_model_details-dropdown", "value"),
+            Input("plugin_3_model_table", "derived_viewport_selected_row_ids"),
+            State("plugin_3_model_table", "data"),
+        )
+        def update_all_plugin_properties(inference_run, selected_rows, table_data):
+            # Check for no selected rows
+            if not selected_rows or selected_rows[0] is None:
+                raise PreventUpdate
+
+            # Get the selected row data and grab the uuid
+            selected_row_data = table_data[selected_rows[0]]
+            object_uuid = selected_row_data["uuid"]
+
+            # Create the Model object
+            model = Model(object_uuid, legacy=True)
+
+            # Update all the properties for each plugin
+            all_props = []
+            for p in self.plugins:
+                all_props.extend(p.update_properties(model, inference_run=inference_run))
+
+            # Return all the updated properties
+            return all_props
+
 
 # Unit Test for your Plugin Page
 if __name__ == "__main__":
     import webbrowser
 
     # Create our Dash Application
     my_app = dash.Dash(
```

### Comparing `sageworks-0.6.6/examples/plugins/views/model_plugin_view.py` & `sageworks-0.6.8/examples/plugins/views/model_plugin_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/plugins/views/my_view_plugin.py` & `sageworks-0.6.8/examples/plugins/views/my_view_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/plugins/web_components/custom_plugin.py` & `sageworks-0.6.8/examples/plugins/web_components/custom_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/plugins/web_components/endpoint_plugin.py` & `sageworks-0.6.8/examples/plugins/web_components/endpoint_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/plugins/web_components/endpoint_turbo.py` & `sageworks-0.6.8/examples/plugins/web_components/endpoint_turbo.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/plugins/web_components/model_markdown.py` & `sageworks-0.6.8/examples/plugins/web_components/model_markdown.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/plugins/web_components/model_plugin.py` & `sageworks-0.6.8/examples/plugins/web_components/model_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/storage/data_to_data.py` & `sageworks-0.6.8/examples/storage/data_to_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/storage/data_to_features.py` & `sageworks-0.6.8/examples/storage/data_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/storage/endpoint_inference.py` & `sageworks-0.6.8/examples/storage/endpoint_inference.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/storage/hello_world_pipeline.py` & `sageworks-0.6.8/examples/storage/hello_world_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/storage/plugin_page_example.py` & `sageworks-0.6.8/examples/storage/plugin_page_example.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/storage/sagemaker_pipelines/all_steps.py` & `sageworks-0.6.8/examples/storage/sagemaker_pipelines/all_steps.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/storage/sagemaker_pipelines/ml_pipeline.py` & `sageworks-0.6.8/examples/storage/sagemaker_pipelines/ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py` & `sageworks-0.6.8/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py` & `sageworks-0.6.8/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/mkdocs.yml` & `sageworks-0.6.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/notebooks/images/athena_query_aqsol.png` & `sageworks-0.6.8/notebooks/images/athena_query_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/notebooks/images/aws_dashboard_aqsol.png` & `sageworks-0.6.8/notebooks/images/aws_dashboard_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/notebooks/images/dashboard_aqsol_features.png` & `sageworks-0.6.8/notebooks/images/dashboard_aqsol_features.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/notebooks/images/model_screenshot.png` & `sageworks-0.6.8/notebooks/images/model_screenshot.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/notebooks/images/sageworks_concepts.png` & `sageworks-0.6.8/notebooks/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/notebooks/images/scp_labs.png` & `sageworks-0.6.8/notebooks/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/scripts/ag_table_row_selection.py` & `sageworks-0.6.8/scripts/ag_table_row_selection.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/scripts/athena_ddl_mixed_case.py` & `sageworks-0.6.8/scripts/athena_ddl_mixed_case.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/scripts/copy_data_catalog_db.py` & `sageworks-0.6.8/scripts/copy_data_catalog_db.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/scripts/create_glue_workflow_with_trigger.py` & `sageworks-0.6.8/scripts/create_glue_workflow_with_trigger.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/scripts/delete_redis_keys.py` & `sageworks-0.6.8/scripts/delete_redis_keys.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/scripts/glue_mixed_case.py` & `sageworks-0.6.8/scripts/glue_mixed_case.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/scripts/model_endpoint_sanity_check.py` & `sageworks-0.6.8/scripts/model_endpoint_sanity_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/scripts/onboard_endpoints.py` & `sageworks-0.6.8/scripts/onboard_endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/scripts/onboard_models.py` & `sageworks-0.6.8/scripts/onboard_models.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/scripts/storage/dns_data_to_features.py` & `sageworks-0.6.8/scripts/storage/dns_data_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/scripts/storage/generate_jsonl_data.py` & `sageworks-0.6.8/scripts/storage/generate_jsonl_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/scripts/test_feature_resolution.py` & `sageworks-0.6.8/scripts/test_feature_resolution.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/setup.py` & `sageworks-0.6.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 """Setup.py for SageWorks: Sagemaker Workbench"""
 
-from setuptools import setup, find_packages
+from setuptools import setup, find_namespace_packages
 
 # Readme
 with open("README.md", "r") as f:
     readme = f.read()
 
 # Requirements
 with open("requirements.txt", "r") as f:
@@ -15,17 +15,16 @@
     name="sageworks",
     description="SageWorks: A Python WorkBench for creating and deploying AWS SageMaker Models",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="SuperCowPowers LLC",
     author_email="support@supercowpowers.com",
     url="https://github.com/SuperCowPowers/sageworks",
-    use_scm_version=True,
     package_dir={"": "src"},
-    packages=find_packages(where="src"),
+    packages=find_namespace_packages(where="src"),
     include_package_data=True,
     package_data={
         "sageworks": [
             "resources/signature_verify_pub.pem",
             "resources/open_source_api.key",
             "core/transforms/features_to_model/light_model_harness/xgb_model.template",
             "core/transforms/features_to_model/light_model_harness/requirements.txt",
```

### Comparing `sageworks-0.6.6/src/sageworks/__init__.py` & `sageworks-0.6.8/src/sageworks/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/algorithms/dataframe/aggregation.py` & `sageworks-0.6.8/src/sageworks/algorithms/dataframe/aggregation.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/algorithms/dataframe/data_source_eda.py` & `sageworks-0.6.8/src/sageworks/algorithms/dataframe/data_source_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/algorithms/dataframe/dimensionality_reduction.py` & `sageworks-0.6.8/src/sageworks/algorithms/dataframe/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/algorithms/dataframe/feature_resolution.py` & `sageworks-0.6.8/src/sageworks/algorithms/dataframe/feature_resolution.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/algorithms/dataframe/feature_spider.py` & `sageworks-0.6.8/src/sageworks/algorithms/dataframe/feature_spider.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/algorithms/dataframe/row_tagger.py` & `sageworks-0.6.8/src/sageworks/algorithms/dataframe/row_tagger.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/algorithms/spark/Readme.md` & `sageworks-0.6.8/src/sageworks/algorithms/spark/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/algorithms/sql/Readme.md` & `sageworks-0.6.8/src/sageworks/algorithms/sql/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/algorithms/sql/column_stats.py` & `sageworks-0.6.8/src/sageworks/algorithms/sql/column_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,16 @@
 
     # Now call the queries to compute the counts of distinct, nulls, and zeros
     data_source.log.info("Computing Unique values...")
     distinct_counts = data_source.query(count_distinct_query(all_columns, table))
     data_source.log.info("Computing Null values...")
     null_counts = data_source.query(count_nulls_query(all_columns, table))
     data_source.log.info("Computing Zero values...")
-    zero_counts = data_source.query(count_zeros_query(numeric, table))
+    if len(numeric) > 0:
+        zero_counts = data_source.query(count_zeros_query(numeric, table))
 
     # Okay now we take the results of the queries and add them to the column_data
     for column in all_columns:
         column_data[column]["unique"] = distinct_counts.iloc[0][f"count_{column}"]
         column_data[column]["nulls"] = null_counts.iloc[0][f"count_{column}"]
         if column in numeric:
             column_data[column]["num_zeros"] = zero_counts.iloc[0][f"count_{column}"]
```

### Comparing `sageworks-0.6.6/src/sageworks/algorithms/sql/correlations.py` & `sageworks-0.6.8/src/sageworks/algorithms/sql/correlations.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     # Grab the  DataSource table name
     table = data_source.get_table_name()
 
     # Build the query
     query = correlation_query(numeric, table)
 
     # Run the query
+    log.debug(query)
     result_df = data_source.query(query)
 
     # Drop any columns that have NaNs
     result_df = result_df.dropna(axis=1)
 
     # Process the results
     # Note: The result_df is a DataFrame with a single row and a column for each pairwise correlation
```

### Comparing `sageworks-0.6.6/src/sageworks/algorithms/sql/descriptive_stats.py` & `sageworks-0.6.8/src/sageworks/algorithms/sql/descriptive_stats.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,18 +51,26 @@
     table = data_source.get_table_name()
 
     # Figure out which columns are numeric
     num_type = ["double", "float", "int", "bigint", "smallint", "tinyint"]
     details = data_source.column_details(view="computation")
     numeric = [column for column, data_type in details.items() if data_type in num_type]
 
+    # Sanity Check for numeric columns
+    if len(numeric) == 0:
+        log.warning("No numeric columns found in the current computation view of the DataSource")
+        log.warning("If the data source was created from a DataFrame, ensure that the DataFrame was properly typed")
+        log.warning("Recommendation: Properly type the DataFrame and recreate the SageWorks artifact")
+        return {}
+
     # Build the query
     query = descriptive_stats_query(numeric, table)
 
     # Run the query
+    log.debug(query)
     result_df = data_source.query(query)
 
     # Process the results
     # Note: The result_df is a DataFrame with a single row and a column for each stat metric
     stats_dict = result_df.to_dict(orient="index")[0]
 
     # Convert the dictionary to a nested dictionary
```

### Comparing `sageworks-0.6.6/src/sageworks/algorithms/sql/outliers.py` & `sageworks-0.6.8/src/sageworks/algorithms/sql/outliers.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,18 +44,14 @@
         # If there are no outliers, return a DataFrame with defined columns but no rows
         if outlier_df is None:
             return pd.DataFrame(columns=data_source.column_names() + ["outlier_group"])
 
         # Get the top N outliers for each outlier group
         outlier_df = self.get_top_n_outliers(outlier_df)
 
-        # Drop duplicates
-        all_except_outlier_group = [col for col in outlier_df.columns if col != "outlier_group"]
-        outlier_df = outlier_df.drop_duplicates(subset=all_except_outlier_group, ignore_index=True)
-
         # Make sure the dataframe isn't too big, if it's too big sample it down
         if len(outlier_df) > 300:
             log.important(f"Outliers DataFrame is too large {len(outlier_df)}, sampling down to 300 rows")
             outlier_df = outlier_df.sample(300)
 
         # Sort by outlier_group and reset the index
         outlier_df = outlier_df.sort_values("outlier_group").reset_index(drop=True)
@@ -74,14 +70,21 @@
             pd.DataFrame: A DataFrame of all the outliers combined
         """
 
         # Grab the column stats and descriptive stats for this DataSource
         column_stats = data_source.column_stats()
         descriptive_stats = data_source.descriptive_stats()
 
+        # If there are no numeric columns, return None
+        if not descriptive_stats:
+            log.warning("No numeric columns found in the current computation view of the DataSource")
+            log.warning("If the data source was created from a DataFrame, ensure that the DataFrame was properly typed")
+            log.warning("Recommendation: Properly type the DataFrame and recreate the SageWorks artifact")
+            return None
+
         # Get the column names and types from the DataSource
         column_details = data_source.column_details(view="computation")
 
         # For every column in the data_source that is numeric get the outliers
         # This loop computes the columns, lower bounds, and upper bounds for the SQL query
         log.info("Computing Outliers for numeric columns...")
         numeric = ["tinyint", "smallint", "int", "bigint", "float", "double", "decimal"]
@@ -192,28 +195,28 @@
             outlier_df (pd.DataFrame): The DataFrame of outliers with 'outlier_group' column
             n (int): Number of top outliers to retrieve for each group, defaults to 10
 
         Returns:
             pd.DataFrame: A DataFrame containing the top N outliers for each outlier group
         """
 
-        def get_extreme_values(group):
+        def get_extreme_values(group: pd.DataFrame) -> pd.DataFrame:
             """Helper function to get the top N extreme values from a group."""
-
-            # Get the column and extreme type (high or low)
             col, extreme_type = group.name.rsplit("_", 1)
-
-            # Sort values depending on whether they are 'high' or 'low' outliers
-            group = group.sort_values(by=col, ascending=(extreme_type == "low"))
-
-            return group.head(n)
+            if extreme_type == "low":
+                return group.nsmallest(n, col)
+            else:
+                return group.nlargest(n, col)
 
         # Group by 'outlier_group' and apply the helper function to get top N extreme values
-        top_outliers = outlier_df.groupby("outlier_group").apply(get_extreme_values).reset_index(drop=True)
-        return top_outliers
+        top_outliers = outlier_df.groupby("outlier_group", group_keys=False).apply(
+            get_extreme_values, include_groups=True
+        )
+
+        return top_outliers.reset_index(drop=True)
 
 
 if __name__ == "__main__":
     """Exercise the SQL Outliers Functionality"""
     from sageworks.api.data_source import DataSource
 
     # Setup Pandas output options
```

### Comparing `sageworks-0.6.6/src/sageworks/algorithms/sql/sample_rows.py` & `sageworks-0.6.8/src/sageworks/algorithms/sql/sample_rows.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/algorithms/sql/value_counts.py` & `sageworks-0.6.8/src/sageworks/algorithms/sql/value_counts.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
                 f"FROM {table} "
                 f'GROUP BY "{column}" ORDER BY sageworks_count DESC LIMIT 20) '
                 f"UNION ALL "
                 f'(SELECT "{column}", count(*) as sageworks_count '
                 f"FROM {table} "
                 f'GROUP BY "{column}" ORDER BY sageworks_count ASC LIMIT 20)'
             )
+            log.debug(query)
             result_df = data_source.query(query)
 
             # Convert Int64 (nullable) to int32 so that we can serialize to JSON
             result_df["sageworks_count"] = result_df["sageworks_count"].astype("int32")
 
             # If the column is boolean, convert the values to True/False strings (for JSON)
             if result_df[column].dtype == "boolean":
```

### Comparing `sageworks-0.6.6/src/sageworks/api/__init__.py` & `sageworks-0.6.8/src/sageworks/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/api/data_source.py` & `sageworks-0.6.8/src/sageworks/api/data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/api/endpoint.py` & `sageworks-0.6.8/src/sageworks/api/endpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,25 +24,26 @@
         """Endpoint Details
 
         Returns:
             dict: A dictionary of details about the Endpoint
         """
         return super().details(**kwargs)
 
-    def inference(self, eval_df: pd.DataFrame, capture_uuid: str = None) -> pd.DataFrame:
+    def inference(self, eval_df: pd.DataFrame, capture_uuid: str = None, id_column: str = None) -> pd.DataFrame:
         """Run inference on the Endpoint using the provided DataFrame
 
         Args:
             eval_df (pd.DataFrame): The DataFrame to run predictions on
             capture_uuid (str, optional): The UUID of the capture to use (default: None)
+            id_column (str, optional): The name of the column to use as the ID (default: None)
 
         Returns:
             pd.DataFrame: The DataFrame with predictions
         """
-        return super().inference(eval_df, capture_uuid)
+        return super().inference(eval_df, capture_uuid, id_column)
 
     def auto_inference(self, capture: bool = False) -> pd.DataFrame:
         """Run inference on the Endpoint using the FeatureSet evaluation data
 
         Args:
             capture (bool): Capture the inference results
```

### Comparing `sageworks-0.6.6/src/sageworks/api/feature_set.py` & `sageworks-0.6.8/src/sageworks/api/feature_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,16 @@
 
         # Ensure the model_name is valid
         if name:
             Artifact.ensure_valid_name(name, delimiter="-")
 
         # If the model_name wasn't given generate it
         else:
-            model_name = self.uuid.replace("_features", "") + "-model"
-            model_name = Artifact.generate_valid_name(model_name, delimiter="-")
+            name = self.uuid.replace("_features", "") + "-model"
+            name = Artifact.generate_valid_name(name, delimiter="-")
 
         # Create the Model Tags
         tags = [name] if tags is None else tags
 
         # Transform the FeatureSet into a Model
         features_to_model = FeaturesToModel(self.uuid, name, model_type=model_type)
         features_to_model.set_output_tags(tags)
```

### Comparing `sageworks-0.6.6/src/sageworks/api/meta.py` & `sageworks-0.6.8/src/sageworks/api/meta.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/api/model.py` & `sageworks-0.6.8/src/sageworks/api/model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/api/monitor.py` & `sageworks-0.6.8/src/sageworks/api/monitor.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/api/pipeline.py` & `sageworks-0.6.8/src/sageworks/api/pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/api/pipeline_manager.py` & `sageworks-0.6.8/src/sageworks/api/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/aws_service_broker/aws_account_clamp.py` & `sageworks-0.6.8/src/sageworks/aws_service_broker/aws_account_clamp.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_broker.py` & `sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_broker.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/connector.py` & `sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/connector.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py` & `sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py` & `sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py` & `sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py` & `sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py` & `sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py` & `sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/artifacts/__init__.py` & `sageworks-0.6.8/src/sageworks/core/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/artifacts/artifact.py` & `sageworks-0.6.8/src/sageworks/core/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/artifacts/athena_source.py` & `sageworks-0.6.8/src/sageworks/core/artifacts/athena_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/artifacts/data_source_abstract.py` & `sageworks-0.6.8/src/sageworks/core/artifacts/data_source_abstract.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/artifacts/data_source_factory.py` & `sageworks-0.6.8/src/sageworks/core/artifacts/data_source_factory.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/artifacts/endpoint_core.py` & `sageworks-0.6.8/src/sageworks/core/artifacts/endpoint_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,71 +146,17 @@
         num_invocations = endpoint_metrics["Invocations"].sum()
         if num_invocations == 0:
             health_issues.append("no_activity")
         else:
             self.remove_health_tag("no_activity")
         return health_issues
 
-    def predict(self, eval_df: pd.DataFrame) -> pd.DataFrame:
-        """Run inference/prediction on the given Feature DataFrame
-        Args:
-            eval_df (pd.DataFrame): DataFrame to run predictions on (must have superset of features)
-        Returns:
-            pd.DataFrame: Return the DataFrame with additional columns, prediction and any _proba
-        """
-
-        # Make sure the eval_df has the features used to train the model
-        features = ModelCore(self.model_name).features()
-        if features and not set(features).issubset(eval_df.columns):
-            raise ValueError(f"DataFrame does not contain required features: {features}")
-
-        # Create our Endpoint Predictor Class
-        predictor = Predictor(
-            self.endpoint_name,
-            sagemaker_session=self.sm_session,
-            serializer=CSVSerializer(),
-            deserializer=CSVDeserializer(),
-        )
-
-        # Now split up the dataframe into 500 row chunks, send those chunks to our
-        # endpoint (with error handling) and stitch all the chunks back together
-        df_list = []
-        for index in range(0, len(eval_df), 500):
-            print("Processing...")
-
-            # Compute partial DataFrames, add them to a list, and concatenate at the end
-            partial_df = self._endpoint_error_handling(predictor, eval_df[index : index + 500])
-            df_list.append(partial_df)
-
-        # Concatenate the dataframes
-        combined_df = pd.concat(df_list, ignore_index=True)
-
-        # Convert data to numeric
-        # Note: Since we're using CSV serializers numeric columns often get changed to generic 'object' types
-
-        # Hard Conversion
-        # Note: We explicitly catch exceptions for columns that cannot be converted to numeric
-        converted_df = combined_df.copy()
-        for column in combined_df.columns:
-            try:
-                converted_df[column] = pd.to_numeric(combined_df[column])
-            except ValueError:
-                # If a ValueError is raised, the column cannot be converted to numeric, so we keep it as is
-                pass
-
-        # Soft Conversion
-        # Convert columns to the best possible dtype that supports the pd.NA missing value.
-        converted_df = converted_df.convert_dtypes()
-
-        # Return the Dataframe
-        return converted_df
-
     def is_serverless(self):
-        """
-        Check if the current endpoint is serverless.
+        """Check if the current endpoint is serverless.
+
         Returns:
             bool: True if the endpoint is serverless, False otherwise.
         """
         return "Serverless" in self.endpoint_meta["InstanceType"]
 
     def add_data_capture(self):
         """Add data capture to the endpoint"""
@@ -218,67 +164,14 @@
 
     def get_monitor(self):
         """Get the MonitorCore class for this endpoint"""
         from sageworks.core.artifacts.monitor_core import MonitorCore
 
         return MonitorCore(self.endpoint_name)
 
-    def _endpoint_error_handling(self, predictor, feature_df):
-        """Internal: Method that handles Errors, Retries, and Binary Search for Error Row(s)"""
-
-        # Convert the DataFrame into a CSV buffer
-        csv_buffer = StringIO()
-        feature_df.to_csv(csv_buffer, index=False)
-
-        # Error Handling if the Endpoint gives back an error
-        try:
-            # Send the CSV Buffer to the predictor
-            results = predictor.predict(csv_buffer.getvalue())
-
-            # Construct a DataFrame from the results
-            results_df = pd.DataFrame.from_records(results[1:], columns=results[0])
-
-            # Capture the return columns
-            self.endpoint_return_columns = results_df.columns.tolist()
-
-            # Return the results dataframe
-            return results_df
-
-        except botocore.exceptions.ClientError as err:
-            if err.response["Error"]["Code"] == "ModelError":  # Model Error
-                # Report the error and raise an exception
-                self.log.critical(f"Endpoint prediction error: {err.response.get('Message')}")
-                raise err
-
-            # Base case: DataFrame with 1 Row
-            if len(feature_df) == 1:
-                # If we don't have ANY known good results we're kinda screwed
-                if not self.endpoint_return_columns:
-                    raise err
-
-                # Construct an Error DataFrame (one row of NaNs in the return columns)
-                results_df = self._error_df(feature_df, self.endpoint_return_columns)
-                return results_df
-
-            # Recurse on binary splits of the dataframe
-            num_rows = len(feature_df)
-            split = int(num_rows / 2)
-            first_half = self._endpoint_error_handling(predictor, feature_df[0:split])
-            second_half = self._endpoint_error_handling(predictor, feature_df[split:num_rows])
-            return pd.concat([first_half, second_half], ignore_index=True)
-
-    def _error_df(self, df, all_columns):
-        """Internal: Method to construct an Error DataFrame (a Pandas DataFrame with one row of NaNs)"""
-        # Create a new dataframe with all NaNs
-        error_df = pd.DataFrame(dict(zip(all_columns, [[np.NaN]] * len(self.endpoint_return_columns))))
-        # Now set the original values for the incoming dataframe
-        for column in df.columns:
-            error_df[column] = df[column].values
-        return error_df
-
     def size(self) -> float:
         """Return the size of this data in MegaBytes"""
         return 0.0
 
     def aws_meta(self) -> dict:
         """Get ALL the AWS metadata for this artifact"""
         return self.endpoint_meta
@@ -418,37 +311,38 @@
     def auto_inference(self, capture: bool = False) -> pd.DataFrame:
         """Run inference on the endpoint using FeatureSet data
 
         Args:
             capture (bool, optional): Capture the inference results and metrics (default=False)
         """
 
-        # This Utility needs to be loaded now to avoid circular imports
+        # This import needs to happen here (instead of top of file) to avoid circular imports
         from sageworks.utils.endpoint_utils import fs_evaluation_data
 
         eval_data_df = fs_evaluation_data(self)
         capture_uuid = "training_holdout" if capture else None
         return self.inference(eval_data_df, capture_uuid)
 
-    def inference(self, eval_df: pd.DataFrame, capture_uuid: str = None) -> pd.DataFrame:
+    def inference(self, eval_df: pd.DataFrame, capture_uuid: str = None, id_column: str = None) -> pd.DataFrame:
         """Run inference and compute performance metrics with optional capture
 
         Args:
             eval_df (pd.DataFrame): DataFrame to run predictions on (must have superset of features)
             capture_uuid (str, optional): UUID of the inference capture (default=None)
+            id_column (str, optional): Name of the ID column (default=None)
 
         Returns:
             pd.DataFrame: DataFrame with the inference results
 
         Note:
             If capture=True inference/performance metrics are written to S3 Endpoint Inference Folder
         """
 
         # Run predictions on the evaluation data
-        prediction_df = self.predict(eval_df)
+        prediction_df = self._predict(eval_df)
 
         # Get the target column
         target_column = ModelCore(self.model_name).target()
 
         # Sanity Check that the target column is present
         if target_column not in prediction_df.columns:
             self.log.warning(f"Target Column {target_column} not found in prediction_df!")
@@ -470,35 +364,144 @@
         # Print out the metrics
         print(f"Performance Metrics for {self.model_name} on {self.uuid}")
         print(metrics.head())
 
         # Capture the inference results and metrics
         if capture_uuid is not None:
             description = capture_uuid.replace("_", " ").title()
-            self._capture_inference_results(capture_uuid, prediction_df, target_column, metrics, description)
+            self._capture_inference_results(capture_uuid, prediction_df, target_column, metrics, description, id_column)
 
         # Return the prediction DataFrame
         return prediction_df
 
+    def _predict(self, eval_df: pd.DataFrame) -> pd.DataFrame:
+        """Internal: Run prediction on the given observations in the given DataFrame
+        Args:
+            eval_df (pd.DataFrame): DataFrame to run predictions on (must have superset of features)
+        Returns:
+            pd.DataFrame: Return the DataFrame with additional columns, prediction and any _proba columns
+        """
+
+        # Make sure the eval_df has the features used to train the model
+        features = ModelCore(self.model_name).features()
+        if features and not set(features).issubset(eval_df.columns):
+            raise ValueError(f"DataFrame does not contain required features: {features}")
+
+        # Create our Endpoint Predictor Class
+        predictor = Predictor(
+            self.endpoint_name,
+            sagemaker_session=self.sm_session,
+            serializer=CSVSerializer(),
+            deserializer=CSVDeserializer(),
+        )
+
+        # Now split up the dataframe into 500 row chunks, send those chunks to our
+        # endpoint (with error handling) and stitch all the chunks back together
+        df_list = []
+        for index in range(0, len(eval_df), 500):
+            print("Processing...")
+
+            # Compute partial DataFrames, add them to a list, and concatenate at the end
+            partial_df = self._endpoint_error_handling(predictor, eval_df[index : index + 500])
+            df_list.append(partial_df)
+
+        # Concatenate the dataframes
+        combined_df = pd.concat(df_list, ignore_index=True)
+
+        # Convert data to numeric
+        # Note: Since we're using CSV serializers numeric columns often get changed to generic 'object' types
+
+        # Hard Conversion
+        # Note: We explicitly catch exceptions for columns that cannot be converted to numeric
+        converted_df = combined_df.copy()
+        for column in combined_df.columns:
+            try:
+                converted_df[column] = pd.to_numeric(combined_df[column])
+            except ValueError:
+                # If a ValueError is raised, the column cannot be converted to numeric, so we keep it as is
+                pass
+
+        # Soft Conversion
+        # Convert columns to the best possible dtype that supports the pd.NA missing value.
+        converted_df = converted_df.convert_dtypes()
+
+        # Return the Dataframe
+        return converted_df
+
+    def _endpoint_error_handling(self, predictor, feature_df):
+        """Internal: Method that handles Errors, Retries, and Binary Search for Error Row(s)"""
+
+        # Convert the DataFrame into a CSV buffer
+        csv_buffer = StringIO()
+        feature_df.to_csv(csv_buffer, index=False)
+
+        # Error Handling if the Endpoint gives back an error
+        try:
+            # Send the CSV Buffer to the predictor
+            results = predictor.predict(csv_buffer.getvalue())
+
+            # Construct a DataFrame from the results
+            results_df = pd.DataFrame.from_records(results[1:], columns=results[0])
+
+            # Capture the return columns
+            self.endpoint_return_columns = results_df.columns.tolist()
+
+            # Return the results dataframe
+            return results_df
+
+        except botocore.exceptions.ClientError as err:
+            if err.response["Error"]["Code"] == "ModelError":  # Model Error
+                # Report the error and raise an exception
+                self.log.critical(f"Endpoint prediction error: {err.response.get('Message')}")
+                raise err
+
+            # Base case: DataFrame with 1 Row
+            if len(feature_df) == 1:
+                # If we don't have ANY known good results we're kinda screwed
+                if not self.endpoint_return_columns:
+                    raise err
+
+                # Construct an Error DataFrame (one row of NaNs in the return columns)
+                results_df = self._error_df(feature_df, self.endpoint_return_columns)
+                return results_df
+
+            # Recurse on binary splits of the dataframe
+            num_rows = len(feature_df)
+            split = int(num_rows / 2)
+            first_half = self._endpoint_error_handling(predictor, feature_df[0:split])
+            second_half = self._endpoint_error_handling(predictor, feature_df[split:num_rows])
+            return pd.concat([first_half, second_half], ignore_index=True)
+
+    def _error_df(self, df, all_columns):
+        """Internal: Method to construct an Error DataFrame (a Pandas DataFrame with one row of NaNs)"""
+        # Create a new dataframe with all NaNs
+        error_df = pd.DataFrame(dict(zip(all_columns, [[np.NaN]] * len(self.endpoint_return_columns))))
+        # Now set the original values for the incoming dataframe
+        for column in df.columns:
+            error_df[column] = df[column].values
+        return error_df
+
     def _capture_inference_results(
         self,
         capture_uuid: str,
         pred_results_df: pd.DataFrame,
         target_column: str,
         metrics: pd.DataFrame,
         description: str,
+        id_column: str = None,
     ):
         """Internal: Capture the inference results and metrics to S3
 
         Args:
             capture_uuid (str): UUID of the inference capture
             pred_results_df (pd.DataFrame): DataFrame with the prediction results
             target_column (str): Name of the target column
             metrics (pd.DataFrame): DataFrame with the performance metrics
             description (str): Description of the inference results
+            id_column (str, optional): Name of the ID column (default=None)
         """
 
         # Compute a dataframe hash (just use the last 8)
         data_hash = joblib.hash(pred_results_df)[:8]
 
         # Metadata for the model inference
         inference_meta = {
@@ -516,19 +519,23 @@
             pd.DataFrame([inference_meta]),
             f"{inference_capture_path}/inference_meta.json",
             index=False,
         )
         self.log.info(f"Writing metrics to {inference_capture_path}/inference_metrics.csv")
         wr.s3.to_csv(metrics, f"{inference_capture_path}/inference_metrics.csv", index=False)
 
-        # Write the predictions to our S3 Model Inference Folder (just the target and prediction columns)
-        self.log.info(f"Writing predictions to {inference_capture_path}/inference_predictions.csv")
+        # Grab the target column, prediction column, any _proba columns, and the ID column (if present)
         prediction_col = "prediction" if "prediction" in pred_results_df.columns else "predictions"
         output_columns = [target_column, prediction_col]
         output_columns += [col for col in pred_results_df.columns if col.endswith("_proba")]
+        if id_column and id_column in pred_results_df.columns:
+            output_columns.append(id_column)
+
+        # Write the predictions to our S3 Model Inference Folder
+        self.log.info(f"Writing predictions to {inference_capture_path}/inference_predictions.csv")
         subset_df = pred_results_df[output_columns]
         wr.s3.to_csv(subset_df, f"{inference_capture_path}/inference_predictions.csv", index=False)
 
         # CLASSIFIER: Write the confusion matrix to our S3 Model Inference Folder
         model_type = self.model_type()
         if model_type == ModelType.CLASSIFIER.value:
             conf_mtx = self.confusion_matrix(target_column, pred_results_df)
```

### Comparing `sageworks-0.6.6/src/sageworks/core/artifacts/feature_set_core.py` & `sageworks-0.6.8/src/sageworks/core/artifacts/feature_set_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/artifacts/model_core.py` & `sageworks-0.6.8/src/sageworks/core/artifacts/model_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         # Model Type
         if self._get_model_type() == ModelType.UNKNOWN:
             health_issues.append("model_type_unknown")
         else:
             self.remove_health_tag("model_type_unknown")
 
         # Model Performance Metrics
-        if self.performance_metrics() is None:
+        if self.get_inference_metrics() is None:
             health_issues.append("metrics_needed")
         else:
             self.remove_health_tag("metrics_needed")
         return health_issues
 
     def latest_model_object(self) -> SagemakerModel:
         """Return the latest AWS Sagemaker Model object for this SageWorks Model
@@ -152,29 +152,29 @@
         directories = wr.s3.list_directories(path=self.endpoint_inference_path + "/")
         inference_runs = [urlparse(directory).path.split("/")[-2] for directory in directories]
 
         # We're going to add the training to the front of the list
         inference_runs.insert(0, "model_training")
         return inference_runs
 
-    def performance_metrics(self, capture_uuid: str = "latest") -> Union[pd.DataFrame, None]:
-        """Retrieve the performance metrics for this model
+    def get_inference_metrics(self, capture_uuid: str = "latest") -> Union[pd.DataFrame, None]:
+        """Retrieve the inference performance metrics for this model
 
         Args:
             capture_uuid (str, optional): Specific capture_uuid or "training" (default: "latest")
         Returns:
             pd.DataFrame: DataFrame of the Model Metrics
 
         Note:
             If a capture_uuid isn't specified this will try to return something reasonable
         """
         # Try to get the auto_capture 'training_holdout' or the training
         if capture_uuid == "latest":
-            metrics_df = self.performance_metrics("training_holdout")
-            return metrics_df if metrics_df is not None else self.performance_metrics("model_training")
+            metrics_df = self.get_inference_metrics("training_holdout")
+            return metrics_df if metrics_df is not None else self.get_inference_metrics("model_training")
 
         # Grab the metrics captured during model training (could return None)
         if capture_uuid == "model_training":
             metrics = self.sageworks_meta().get("sageworks_training_metrics")
             return pd.DataFrame.from_dict(metrics) if metrics else None
 
         else:  # Specific capture_uuid (could return None)
@@ -209,28 +209,14 @@
             cm = pull_s3_data(s3_path, embedded_index=True)
             if cm is not None:
                 return cm
             else:
                 self.log.warning(f"Confusion Matrix {capture_uuid} not found for {self.model_name}!")
                 return None
 
-    def predictions(self, capture_uuid: str = "training_holdout") -> Union[pd.DataFrame, None]:
-        """Retrieve the predictions for this model
-
-        Args:
-            capture_uuid (str, optional): Specific capture_uuid or "training" (default: "training_holdout")
-        Returns:
-            pd.DataFrame: DataFrame of the Predictions (might be None)
-        """
-        # Grab the metrics from the SageWorks Metadata (try inference first, then training)
-        inference_preds = self.inference_predictions(capture_uuid)
-        if inference_preds is not None:
-            return inference_preds
-        return self.validation_predictions()
-
     def set_input(self, input: str, force: bool = False):
         """Override: Set the input data for this artifact
 
         Args:
             input (str): Name of input for this artifact
             force (bool, optional): Force the input to be set (default: False)
         Note:
@@ -410,24 +396,24 @@
         container_info = self.model_container_info()
         details["framework"] = container_info.get("Framework", "unknown")
         details["framework_version"] = container_info.get("FrameworkVersion", "unknown")
         details["inference_types"] = inference_spec["SupportedRealtimeInferenceInstanceTypes"]
         details["transform_types"] = inference_spec["SupportedTransformInstanceTypes"]
         details["content_types"] = inference_spec["SupportedContentTypes"]
         details["response_types"] = inference_spec["SupportedResponseMIMETypes"]
-        details["model_metrics"] = self.performance_metrics()
+        details["model_metrics"] = self.get_inference_metrics()
         if self.model_type == ModelType.CLASSIFIER:
             details["confusion_matrix"] = self.confusion_matrix()
             details["predictions"] = None
         else:
             details["confusion_matrix"] = None
-            details["predictions"] = self.predictions()
+            details["predictions"] = self.get_inference_predictions()
 
         # Grab the inference metadata
-        details["inference_meta"] = self.inference_metadata()
+        details["inference_meta"] = self.get_inference_metadata()
 
         # Cache the details
         self.data_storage.set(storage_key, details)
 
         # Return the details
         return details
 
@@ -691,15 +677,15 @@
         s3_path = f"{self.endpoint_inference_path}/{capture_uuid}/inference_cm.csv"
         inference_cm = pull_s3_data(s3_path, embedded_index=True)
 
         # Store data into the SageWorks Metadata
         cm_storage = None if inference_cm is None else inference_cm.to_dict("records")
         self.upsert_sageworks_meta({"sageworks_inference_cm": cm_storage})
 
-    def inference_metadata(self, capture_uuid: str = "training_holdout") -> Union[pd.DataFrame, None]:
+    def get_inference_metadata(self, capture_uuid: str = "training_holdout") -> Union[pd.DataFrame, None]:
         """Retrieve the inference metadata for this model
 
         Args:
             capture_uuid (str, optional): A specific capture_uuid (default: "training_holdout")
 
         Returns:
             dict: Dictionary of the inference metadata (might be None)
@@ -729,28 +715,34 @@
         try:
             s3_path = f"{self.endpoint_inference_path}/{capture_uuid}/inference_meta.json"
             return wr.s3.read_json(s3_path)
         except NoFilesFound:
             self.log.info(f"Could not find model inference meta at {s3_path}...")
             return None
 
-    def inference_predictions(self, capture_uuid: str = "training_holdout") -> Union[pd.DataFrame, None]:
+    def get_inference_predictions(self, capture_uuid: str = "training_holdout") -> Union[pd.DataFrame, None]:
         """Retrieve the captured prediction results for this model
 
         Args:
             capture_uuid (str, optional): Specific capture_uuid (default: training_holdout)
 
         Returns:
             pd.DataFrame: DataFrame of the Captured Predictions (might be None)
         """
         self.log.important(f"Grabbing {capture_uuid} predictions for {self.model_name}...")
+
+        # Special case for model_training
+        if capture_uuid == "model_training":
+            return self._get_validation_predictions()
+
+        # Construct the S3 path for the Inference Predictions
         s3_path = f"{self.endpoint_inference_path}/{capture_uuid}/inference_predictions.csv"
         return pull_s3_data(s3_path)
 
-    def validation_predictions(self) -> Union[pd.DataFrame, None]:
+    def _get_validation_predictions(self) -> Union[pd.DataFrame, None]:
         """Internal: Retrieve the captured prediction results for this model
 
         Returns:
             pd.DataFrame: DataFrame of the Captured Validation Predictions (might be None)
         """
         self.log.important(f"Grabbing Validation Predictions for {self.model_name}...")
         s3_path = f"{self.model_training_path}/validation_predictions.csv"
@@ -865,22 +857,22 @@
     print(f"Training Job: {my_model.training_job_name}")
 
     # List any inference runs
     print(f"Inference Runs: {my_model.list_inference_runs()}")
 
     # Get any captured metrics from the training job
     print("Model Metrics:")
-    print(my_model.performance_metrics())
+    print(my_model.get_inference_metrics())
 
     print("Confusion Matrix: (might be None)")
     print(my_model.confusion_matrix())
 
     # Grab our regression predictions from S3
     print("Captured Predictions: (might be None)")
-    print(my_model.predictions())
+    print(my_model.get_inference_predictions())
 
     # Grab our Shapley values from S3
     print("Shapley Values: (might be None)")
     print(my_model.shapley_values())
 
     # Get the SageWorks metadata associated with this Model
     print(f"SageWorks Meta: {my_model.sageworks_meta()}")
```

### Comparing `sageworks-0.6.6/src/sageworks/core/artifacts/monitor_core.py` & `sageworks-0.6.8/src/sageworks/core/artifacts/monitor_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/pipelines/pipeline_executor.py` & `sageworks-0.6.8/src/sageworks/core/pipelines/pipeline_executor.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/Readme.md` & `sageworks-0.6.8/src/sageworks/core/transforms/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py` & `sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/light/__init__.py` & `sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/light/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py` & `sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py` & `sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py` & `sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/light/clean_data.py` & `sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/light/clean_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py` & `sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py` & `sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py` & `sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py` & `sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py` & `sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/features_to_model/features_to_model.py` & `sageworks-0.6.8/src/sageworks/core/transforms/features_to_model/features_to_model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template` & `sageworks-0.6.8/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py` & `sageworks-0.6.8/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/__init__.py` & `sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py` & `sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py` & `sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py` & `sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py` & `sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py` & `sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/core/transforms/transform.py` & `sageworks-0.6.8/src/sageworks/core/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/experiments/view_manager.py` & `sageworks-0.6.8/src/sageworks/experiments/view_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/repl/sageworks_shell.py` & `sageworks-0.6.8/src/sageworks/repl/sageworks_shell.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/aws_utils.py` & `sageworks-0.6.8/src/sageworks/utils/aws_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/cache.py` & `sageworks-0.6.8/src/sageworks/utils/cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/chem_utils.py` & `sageworks-0.6.8/src/sageworks/utils/chem_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/config_manager.py` & `sageworks-0.6.8/src/sageworks/utils/config_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/dashboard_metrics.py` & `sageworks-0.6.8/src/sageworks/utils/dashboard_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/datetime_utils.py` & `sageworks-0.6.8/src/sageworks/utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/df_to_endpoint.py` & `sageworks-0.6.8/src/sageworks/utils/df_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/docker_utils.py` & `sageworks-0.6.8/src/sageworks/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/ecs_info.py` & `sageworks-0.6.8/src/sageworks/utils/ecs_info.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/endpoint_metrics.py` & `sageworks-0.6.8/src/sageworks/utils/endpoint_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/endpoint_utils.py` & `sageworks-0.6.8/src/sageworks/utils/endpoint_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         end (Endpoint): Endpoint to backtrace: End -> Model -> FeatureSet (evaluation data)
 
     Returns:
         pd.DataFrame: Dataframe with the predictions using the FeatureSet data
     """
     # Grab the FeatureSet evaluation data
     feature_df = fs_evaluation_data(end)
-    return end.predict(feature_df)
+    return end._predict(feature_df)
 
 
 def fs_training_data(end: Endpoint) -> pd.DataFrame:
     """Code to get the training data from the FeatureSet used to train the Model
 
     Args:
         end (Endpoint): Endpoint to backtrace: End -> Model -> FeatureSet (training data)
```

### Comparing `sageworks-0.6.6/src/sageworks/utils/extract_model_artifact.py` & `sageworks-0.6.8/src/sageworks/utils/extract_model_artifact.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/glue_utils.py` & `sageworks-0.6.8/src/sageworks/utils/glue_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/license_manager.py` & `sageworks-0.6.8/src/sageworks/utils/license_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/markdown_utils.py` & `sageworks-0.6.8/src/sageworks/utils/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/pandas_utils.py` & `sageworks-0.6.8/src/sageworks/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/plugin_manager.py` & `sageworks-0.6.8/src/sageworks/utils/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/redis_cache.py` & `sageworks-0.6.8/src/sageworks/utils/redis_cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/repl_utils.py` & `sageworks-0.6.8/src/sageworks/utils/repl_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/s3_utils.py` & `sageworks-0.6.8/src/sageworks/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/sageworks_cache.py` & `sageworks-0.6.8/src/sageworks/utils/sageworks_cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/sageworks_event_bridge.py` & `sageworks-0.6.8/src/sageworks/utils/sageworks_event_bridge.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/sageworks_logging.py` & `sageworks-0.6.8/src/sageworks/utils/sageworks_logging.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/sageworks_sqs.py` & `sageworks-0.6.8/src/sageworks/utils/sageworks_sqs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/symbols.py` & `sageworks-0.6.8/src/sageworks/utils/symbols.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/test_data_generator.py` & `sageworks-0.6.8/src/sageworks/utils/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/trace_calls.py` & `sageworks-0.6.8/src/sageworks/utils/trace_calls.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/utils/type_abbrev.py` & `sageworks-0.6.8/src/sageworks/utils/type_abbrev.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/views/artifacts_text_view.py` & `sageworks-0.6.8/src/sageworks/views/artifacts_text_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/views/artifacts_web_view.py` & `sageworks-0.6.8/src/sageworks/views/artifacts_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/views/data_source_web_view.py` & `sageworks-0.6.8/src/sageworks/views/data_source_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/views/endpoint_web_view.py` & `sageworks-0.6.8/src/sageworks/views/endpoint_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/views/feature_set_web_view.py` & `sageworks-0.6.8/src/sageworks/views/feature_set_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/views/model_web_view.py` & `sageworks-0.6.8/src/sageworks/views/model_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/views/view.py` & `sageworks-0.6.8/src/sageworks/views/view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/web_components/component_interface.py` & `sageworks-0.6.8/src/sageworks/web_components/component_interface.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/web_components/confusion_matrix.py` & `sageworks-0.6.8/src/sageworks/web_components/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/web_components/correlation_matrix.py` & `sageworks-0.6.8/src/sageworks/web_components/correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/web_components/data_details_markdown.py` & `sageworks-0.6.8/src/sageworks/web_components/data_details_markdown.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/web_components/endpoint_metric_plots.py` & `sageworks-0.6.8/src/sageworks/web_components/endpoint_metric_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/web_components/experiments/color_maps.py` & `sageworks-0.6.8/src/sageworks/web_components/experiments/color_maps.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/web_components/experiments/compound_details.py` & `sageworks-0.6.8/src/sageworks/web_components/experiments/compound_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/web_components/experiments/dashboard_metric_plots.py` & `sageworks-0.6.8/src/sageworks/web_components/experiments/dashboard_metric_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/web_components/experiments/data_table.py` & `sageworks-0.6.8/src/sageworks/web_components/experiments/data_table.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/web_components/experiments/histogram.py` & `sageworks-0.6.8/src/sageworks/web_components/experiments/histogram.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/web_components/experiments/line_chart.py` & `sageworks-0.6.8/src/sageworks/web_components/experiments/line_chart.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/web_components/experiments/outlier_plot.py` & `sageworks-0.6.8/src/sageworks/web_components/experiments/outlier_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/web_components/experiments/plugin_callbacks.py` & `sageworks-0.6.8/src/sageworks/web_components/experiments/plugin_callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/web_components/experiments/scatter_plot.py` & `sageworks-0.6.8/src/sageworks/web_components/experiments/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/web_components/model_details.py` & `sageworks-0.6.8/src/sageworks/web_components/plugins/model_details.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,99 +1,102 @@
 """A Markdown Component for details/information about Models"""
 
+import logging
+
 # Dash Imports
 from dash import html, callback, no_update, dcc
-from dash.dependencies import Input, Output, State
+from dash.dependencies import Input, Output
 
 # SageWorks Imports
 from sageworks.api import Model
-from sageworks.web_components.component_interface import ComponentInterface
 from sageworks.utils.markdown_utils import health_tag_markdown
+from sageworks.web_components.plugin_interface import PluginInterface, PluginPage, PluginInputType
+
+# Get the SageWorks logger
+log = logging.getLogger("sageworks")
+
 
+class ModelDetails(PluginInterface):
+    """Model Details Composite Component"""
 
-class ModelDetails(ComponentInterface):
-    """Model Markdown Component"""
+    """Initialize this Plugin Component Class with required attributes"""
+    auto_load_page = PluginPage.NONE
+    plugin_input_type = PluginInputType.MODEL
 
     def __init__(self):
-        self.prefix_id = ""
-        self.model = None
+        """Initialize the ModelDetails plugin class"""
+        self.component_id = None
+        self.current_model = None
+
+        # Call the parent class constructor
         super().__init__()
 
     def create_component(self, component_id: str) -> html.Div:
         """Create a Markdown Component without any data.
         Args:
             component_id (str): The ID of the web component
         Returns:
             html.Div: A Container of Components for the Model Details
         """
-        self.prefix_id = component_id
+        self.component_id = component_id
         container = html.Div(
-            id=self.prefix_id,
+            id=self.component_id,
             children=[
-                html.H3(id=f"{self.prefix_id}-header", children="Model: Loading..."),
-                dcc.Markdown(id=f"{self.prefix_id}-summary"),
+                html.H3(id=f"{self.component_id}-header", children="Model: Loading..."),
+                dcc.Markdown(id=f"{self.component_id}-summary"),
                 html.H3(children="Inference Metrics"),
-                dcc.Dropdown(id=f"{self.prefix_id}-dropdown", className="dropdown"),
-                dcc.Markdown(id=f"{self.prefix_id}-metrics"),
-                dcc.Store(id=f"{self.prefix_id}-model-uuid"),  # Store the model uuid
+                dcc.Dropdown(id=f"{self.component_id}-dropdown", className="dropdown"),
+                dcc.Markdown(id=f"{self.component_id}-metrics"),
             ],
         )
+
+        # Fill in plugin properties
+        self.properties = [
+            (f"{self.component_id}-header", "children"),
+            (f"{self.component_id}-summary", "children"),
+            (f"{self.component_id}-dropdown", "options"),
+            (f"{self.component_id}-dropdown", "value"),
+        ]
+        self.signals = [(f"{self.component_id}-dropdown", "value")]
+
+        # Return the container
         return container
 
-    def register_callbacks(self, model_table):
-        @callback(
-            [
-                Output(f"{self.prefix_id}-header", "children"),
-                Output(f"{self.prefix_id}-summary", "children"),
-                Output(f"{self.prefix_id}-dropdown", "options"),
-                Output(f"{self.prefix_id}-dropdown", "value"),
-                Output(f"{self.prefix_id}-metrics", "children", allow_duplicate=True),
-                Output(f"{self.prefix_id}-model-uuid", "data"),
-            ],
-            Input(model_table, "derived_viewport_selected_row_ids"),
-            State(model_table, "data"),
-            prevent_initial_call=True,
-        )
-        def update_model(selected_rows, table_data):
-            # Check for no selected rows
-            if not selected_rows or selected_rows[0] is None:
-                return no_update
+    def update_properties(self, model: Model, **kwargs) -> list:
+        """Update the properties for the plugin.
 
-            # Get the selected row data, grab the uuid, and set the Model object
-            selected_row_data = table_data[selected_rows[0]]
-            model_uuid = selected_row_data["uuid"]
-            self.model = Model(model_uuid, legacy=True)
-
-            # Update the header, the summary, and the details
-            header = f"Model: {self.model.uuid}"
-            summary = self.model_summary()
-
-            # Populate the inference runs dropdown
-            inference_runs, default_run = self.get_inference_runs()
-
-            # Update the metrics for the default inference run
-            metrics = self.inference_metrics(default_run)
-
-            # Return the updated components
-            return header, summary, inference_runs, default_run, metrics, model_uuid
-
-        @callback(
-            Output(f"{self.prefix_id}-metrics", "children", allow_duplicate=True),
-            Input(f"{self.prefix_id}-dropdown", "value"),
-            State(f"{self.prefix_id}-model-uuid", "data"),
-            prevent_initial_call=True,
-        )
-        def update_inference_run(inference_run, model_uuid):
+        Args:
+            model (Model): An instantiated Model object
+            **kwargs: Additional keyword arguments (unused)
+
+        Returns:
+            list: A list of the updated property values for the plugin
+        """
+        log.important(f"Updating Plugin with Model: {model.uuid} and kwargs: {kwargs}")
+
+        # Update the header and the details
+        self.current_model = model
+        header = f"{self.current_model.uuid}"
+        details = self.model_summary()
+
+        # Populate the inference runs dropdown
+        inference_runs, default_run = self.get_inference_runs()
+
+        # Return the updated property values for the plugin
+        return [header, details, inference_runs, default_run]
+
+    def register_internal_callbacks(self):
+        @callback(Output(f"{self.component_id}-metrics", "children"), Input(f"{self.component_id}-dropdown", "value"))
+        def update_inference_run(inference_run):
             # Check for no inference run
-            if not inference_run or (self.model.uuid != model_uuid):
+            if not inference_run:
                 return no_update
 
             # Update the model metrics
             metrics = self.inference_metrics(inference_run)
-
             return metrics
 
     def model_summary(self):
         """Construct the markdown string for the model summary
 
         Returns:
             str: A markdown string
@@ -107,15 +110,15 @@
             "sageworks_model_type",
             "sageworks_tags",
             "sageworks_model_target",
             "sageworks_model_features",
         ]
 
         # Construct the markdown string
-        summary = self.model.summary()
+        summary = self.current_model.summary()
         markdown = ""
         for key in show_fields:
 
             # Special case for the health tags
             if key == "health_tags":
                 markdown += health_tag_markdown(summary.get(key, []))
                 continue
@@ -148,15 +151,15 @@
 
         Args:
             inference_run (str): The inference run to get the metrics for
         Returns:
             str: A markdown string
         """
         # Model Metrics
-        meta_df = self.model.inference_metadata(inference_run)
+        meta_df = self.current_model.get_inference_metadata(inference_run)
         if meta_df is None:
             test_data = "Inference Metadata Not Found"
             test_data_hash = " N/A "
             test_rows = " - "
             description = " - "
         else:
             inference_meta = meta_df.to_dict(orient="records")[0]
@@ -169,15 +172,15 @@
         markdown = "\n"
         markdown += f"**Test Data:** {test_data}  \n"
         markdown += f"**Data Hash:** {test_data_hash}  \n"
         markdown += f"**Test Rows:** {test_rows}  \n"
         markdown += f"**Description:** {description}  \n"
 
         # Grab the Metrics from the model details
-        metrics = self.model.performance_metrics(capture_uuid=inference_run)
+        metrics = self.current_model.get_inference_metrics(capture_uuid=inference_run)
         if metrics is None:
             markdown += "  \nNo Data  \n"
         else:
             markdown += "  \n"
             metrics = metrics.round(3)
             markdown += metrics.to_markdown(index=False)
 
@@ -189,55 +192,26 @@
 
         Returns:
             list[str]: A list of inference runs
             default_run (str): The default inference run
         """
 
         # Inference runs
-        inference_runs = self.model.list_inference_runs()
+        inference_runs = self.current_model.list_inference_runs()
 
         # Check if there are any inference runs to select
         if not inference_runs:
             return [], None
 
         # Set "training_holdout" as the default, if that doesn't exist, set the first
         default_inference_run = "training_holdout" if "training_holdout" in inference_runs else inference_runs[0]
 
         # Return the options for the dropdown and the selected value
         return inference_runs, default_inference_run
 
 
 if __name__ == "__main__":
     # This class takes in model details and generates a details Markdown component
-    import dash
-    import dash_bootstrap_components as dbc
-    from sageworks.web_components.table import Table
-    from sageworks.api.meta import Meta
-
-    # Create a model table
-    models_table = Table().create_component(
-        "my_models_table", header_color="rgb(60, 100, 60)", row_select="single", max_height=270
-    )
-
-    # Populate the table with data
-    models = Meta().models()
-    models["uuid"] = models["Model Group"]
-    models["id"] = range(len(models))
-    column_setup_list = Table().column_setup(models)
-    models_table.columns = column_setup_list
-    models_table.data = models.to_dict("records")
-
-    # Instantiate the ModelDetails class
-    md = ModelDetails()
-    details_component = md.create_component("my_model_details")
-
-    # Register the callbacks
-    md.register_callbacks("my_models_table")
-
-    # Initialize Dash app
-    app = dash.Dash(
-        __name__,
-        external_stylesheets=[dbc.themes.DARKLY],
-    )
+    from sageworks.web_components.plugin_unit_test import PluginUnitTest
 
-    app.layout = html.Div([models_table, details_component])
-    app.run(debug=True)
+    # Run the Unit Test on the Plugin
+    PluginUnitTest(ModelDetails).run()
```

### Comparing `sageworks-0.6.6/src/sageworks/web_components/model_plot.py` & `sageworks-0.6.8/src/sageworks/web_components/model_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/web_components/plugin_interface.py` & `sageworks-0.6.8/src/sageworks/web_components/plugin_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,39 +33,53 @@
     MODEL_TABLE = "model_table"
     PIPELINE_TABLE = "pipeline_table"
     CUSTOM = "custom"
 
 
 class PluginInterface(ComponentInterface):
     """A Web Plugin Interface
+
     Notes:
-      - The 'create_component' method must be implemented by the child class
-      - The 'update_properties' method must be implemented by the child class
+        - The 'create_component' method must be implemented by the child class
+        - The 'update_properties' method must be implemented by the child class
+        - The 'register_internal_callbacks' method is optional
     """
 
     @abstractmethod
     def create_component(self, component_id: str) -> Component:
         """Create a Dash Component without any data.
 
         Args:
-            component_id (str): The ID of the web component
+            component_id (str): The ID of the web component.
 
         Returns:
-           Component: A Dash Base Component
+            Component: A Dash Base Component.
         """
         pass
 
     @abstractmethod
     def update_properties(self, data_object: ComponentInterface.SageworksObject, **kwargs) -> list:
-        """Update the property values for the plugin component
+        """Update the property values for the plugin component.
+
         Args:
-            data_object (sageworks_object): The instantiated data object for the plugin type.
-            **kwargs: Additional keyword arguments (plugins can define their own arguments)
+            data_object (ComponentInterface.SageworksObject): The instantiated data object for the plugin type.
+            **kwargs: Additional keyword arguments (plugins can define their own arguments).
+
         Returns:
-            list: A list of the updated properties values for the plugin
+            list: A list of the updated property values for the plugin.
+        """
+        pass
+
+    def register_internal_callbacks(self):
+        """Register any internal callbacks for the plugin.
+
+        Notes:
+            Implementing this method is optional. This method is useful for registering internal callbacks
+            that are specific to the plugin. For example, a plugin that needs to update some properties based
+            on a dropdown selection.
         """
         pass
 
     #
     # Internal Methods: These methods are used to validate the plugin interface at runtime
     #
     def __init_subclass__(cls, **kwargs):
```

### Comparing `sageworks-0.6.6/src/sageworks/web_components/plugin_unit_test.py` & `sageworks-0.6.8/src/sageworks/web_components/plugin_unit_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,37 +44,40 @@
             [Input("update-button", "n_clicks")],
             prevent_initial_call=True,
         )
         def update_plugin_properties(n_clicks):
             # Simulate updating the plugin with a new Model, Endpoint, or Model Table
             if plugin_input_type == PluginInputType.MODEL:
                 model = Model("abalone-regression")
-                updated_proporties = self.plugin.update_properties(model, inference_run="training_holdout")
+                updated_properties = self.plugin.update_properties(model, inference_run="training_holdout")
             elif plugin_input_type == PluginInputType.ENDPOINT:
                 endpoint = Endpoint("abalone-regression-end")
-                updated_proporties = self.plugin.update_properties(endpoint)
+                updated_properties = self.plugin.update_properties(endpoint)
             elif plugin_input_type == PluginInputType.PIPELINE:
                 pipeline = Pipeline("abalone_pipeline_v1")
-                updated_proporties = self.plugin.update_properties(pipeline)
+                updated_properties = self.plugin.update_properties(pipeline)
             elif plugin_input_type == PluginInputType.MODEL_TABLE:
                 model_df = Meta().models()
-                updated_proporties = self.plugin.update_properties(model_df)
+                updated_properties = self.plugin.update_properties(model_df)
             elif plugin_input_type == PluginInputType.PIPELINE_TABLE:
                 pipeline_df = Meta().pipelines()
-                updated_proporties = self.plugin.update_properties(pipeline_df)
+                updated_properties = self.plugin.update_properties(pipeline_df)
             else:
                 raise ValueError(f"Invalid test type: {plugin_input_type}")
 
             # Return the updated properties for the plugin
-            return updated_proporties
+            return updated_properties
 
         # Set up callbacks for displaying output signals
         for component_id, property in self.plugin.signals:
 
             @self.app.callback(
                 Output(f"test-output-{component_id}-{property}", "children"), Input(component_id, property)
             )
             def display_output_signal(signal_value):
                 return f"{signal_value}"
 
+        # Now register any internal callbacks
+        self.plugin.register_internal_callbacks()
+
     def run(self):
         self.app.run_server(debug=True)
```

### Comparing `sageworks-0.6.6/src/sageworks/web_components/plugins/ag_table.py` & `sageworks-0.6.8/src/sageworks/web_components/plugins/ag_table.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/web_components/plugins/license_details.py` & `sageworks-0.6.8/src/sageworks/web_components/plugins/license_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/web_components/plugins/pipeline_details.py` & `sageworks-0.6.8/src/sageworks/web_components/plugins/pipeline_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/web_components/regression_plot.py` & `sageworks-0.6.8/src/sageworks/web_components/regression_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     def create_component(self, component_id: str) -> dcc.Graph:
         # Initialize an empty scatter plot figure
         return dcc.Graph(id=component_id, figure=self.display_text("Waiting for Data..."))
 
     def update_properties(self, model: Model, inference_run: str = None) -> go.Figure:
         # Get predictions for specific inference
-        df = model.predictions(inference_run)
+        df = model.get_inference_predictions(inference_run)
 
         if df is None:
             return self.display_text("No Data")
 
         # Get the name of the actual field value column
         actual_col = [col for col in df.columns if col != "prediction"][0]
```

### Comparing `sageworks-0.6.6/src/sageworks/web_components/table.py` & `sageworks-0.6.8/src/sageworks/web_components/table.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks/web_components/violin_plots.py` & `sageworks-0.6.8/src/sageworks/web_components/violin_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/src/sageworks.egg-info/PKG-INFO` & `sageworks-0.6.8/src/sageworks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.6.6
+Version: 0.6.8
 Summary: SageWorks: A Python WorkBench for creating and deploying AWS SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sageworks-0.6.6/src/sageworks.egg-info/SOURCES.txt` & `sageworks-0.6.8/src/sageworks.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 CONTRIBUTING.md
 Dockerfile
 LICENSE
 Makefile
 README.md
 SECURITY.md
 mkdocs.yml
+pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 .github/PULL_REQUEST_TEMPLATE.md
 .github/dependabot.yml
 .github/workflows/deploy-docs.yml
@@ -247,14 +248,15 @@
 src/sageworks/algorithms/dataframe/Readme.md
 src/sageworks/algorithms/dataframe/aggregation.py
 src/sageworks/algorithms/dataframe/data_source_eda.py
 src/sageworks/algorithms/dataframe/dimensionality_reduction.py
 src/sageworks/algorithms/dataframe/feature_resolution.py
 src/sageworks/algorithms/dataframe/feature_spider.py
 src/sageworks/algorithms/dataframe/row_tagger.py
+src/sageworks/algorithms/dataframe/target_gradients.py
 src/sageworks/algorithms/graph/heavy/Readme.md
 src/sageworks/algorithms/graph/light/Readme.md
 src/sageworks/algorithms/spark/Readme.md
 src/sageworks/algorithms/sql/Readme.md
 src/sageworks/algorithms/sql/column_stats.py
 src/sageworks/algorithms/sql/correlations.py
 src/sageworks/algorithms/sql/descriptive_stats.py
@@ -319,14 +321,15 @@
 src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py
 src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py
 src/sageworks/core/transforms/features_to_features/__init__.py
 src/sageworks/core/transforms/features_to_features/heavy/emr/Readme.md
 src/sageworks/core/transforms/features_to_features/heavy/glue/Readme.md
 src/sageworks/core/transforms/features_to_model/__init__.py
 src/sageworks/core/transforms/features_to_model/features_to_model.py
+src/sageworks/core/transforms/features_to_model/light_model_harness/generated_xgb_model.py
 src/sageworks/core/transforms/features_to_model/light_model_harness/requirements.txt
 src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template
 src/sageworks/core/transforms/model_to_endpoint/__init__.py
 src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py
 src/sageworks/core/transforms/pandas_transforms/__init__.py
 src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py
 src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py
@@ -374,33 +377,34 @@
 src/sageworks/views/feature_set_web_view.py
 src/sageworks/views/model_web_view.py
 src/sageworks/views/view.py
 src/sageworks/web_components/component_interface.py
 src/sageworks/web_components/confusion_matrix.py
 src/sageworks/web_components/correlation_matrix.py
 src/sageworks/web_components/data_details_markdown.py
-src/sageworks/web_components/endpoint_details.py
 src/sageworks/web_components/endpoint_metric_plots.py
-src/sageworks/web_components/model_details.py
 src/sageworks/web_components/model_plot.py
 src/sageworks/web_components/plugin_interface.py
 src/sageworks/web_components/plugin_unit_test.py
 src/sageworks/web_components/regression_plot.py
 src/sageworks/web_components/table.py
 src/sageworks/web_components/violin_plots.py
 src/sageworks/web_components/experiments/color_maps.py
 src/sageworks/web_components/experiments/compound_details.py
 src/sageworks/web_components/experiments/dashboard_metric_plots.py
 src/sageworks/web_components/experiments/data_table.py
+src/sageworks/web_components/experiments/graph_test.py
+src/sageworks/web_components/experiments/hello.py
 src/sageworks/web_components/experiments/histogram.py
 src/sageworks/web_components/experiments/line_chart.py
 src/sageworks/web_components/experiments/outlier_plot.py
 src/sageworks/web_components/experiments/plugin_callbacks.py
 src/sageworks/web_components/experiments/scatter_plot.py
 src/sageworks/web_components/plugins/ag_table.py
+src/sageworks/web_components/plugins/endpoint_details.py
 src/sageworks/web_components/plugins/license_details.py
 src/sageworks/web_components/plugins/model_details.py
 src/sageworks/web_components/plugins/pipeline_details.py
 tests/create_aqsol_artifacts.py
 tests/create_basic_test_artifacts.py
 tests/create_realtime_endpoint.py
 tests/create_training_adjusted_artifacts.py
```

### Comparing `sageworks-0.6.6/tests/artifacts/data_source_tests.py` & `sageworks-0.6.8/tests/artifacts/data_source_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/artifacts/endpoint_tests.py` & `sageworks-0.6.8/tests/artifacts/endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/artifacts/feature_set_tests.py` & `sageworks-0.6.8/tests/artifacts/feature_set_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/artifacts/model_tests.py` & `sageworks-0.6.8/tests/artifacts/model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/aws_account/aws_account_clamp_tests.py` & `sageworks-0.6.8/tests/aws_account/aws_account_clamp_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/aws_account/aws_service_broker_tests.py` & `sageworks-0.6.8/tests/aws_account/aws_service_broker_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/connectors/data_catalog.py` & `sageworks-0.6.8/tests/connectors/data_catalog.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/connectors/endpoints.py` & `sageworks-0.6.8/tests/connectors/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/connectors/feature_store.py` & `sageworks-0.6.8/tests/connectors/feature_store.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/connectors/glue_jobs.py` & `sageworks-0.6.8/tests/connectors/glue_jobs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/connectors/model_registry.py` & `sageworks-0.6.8/tests/connectors/model_registry.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/connectors/s3_bucket.py` & `sageworks-0.6.8/tests/connectors/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/create_aqsol_artifacts.py` & `sageworks-0.6.8/tests/create_aqsol_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/create_basic_test_artifacts.py` & `sageworks-0.6.8/tests/create_basic_test_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/create_realtime_endpoint.py` & `sageworks-0.6.8/tests/create_realtime_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/create_training_adjusted_artifacts.py` & `sageworks-0.6.8/tests/create_training_adjusted_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/create_wine_artifacts.py` & `sageworks-0.6.8/tests/create_wine_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/delete_test_artifacts.py` & `sageworks-0.6.8/tests/delete_test_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/plugin_tests/crashing_plugin.py` & `sageworks-0.6.8/tests/plugin_tests/crashing_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/specific/capital_tests.py` & `sageworks-0.6.8/tests/specific/capital_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/specific/deletion_tests.py` & `sageworks-0.6.8/tests/specific/deletion_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/transforms/data_to_data_tests.py` & `sageworks-0.6.8/tests/transforms/data_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/transforms/data_to_features_tests.py` & `sageworks-0.6.8/tests/transforms/data_to_features_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/transforms/features_to_model_tests.py` & `sageworks-0.6.8/tests/transforms/features_to_model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/transforms/model_metrics_tests.py` & `sageworks-0.6.8/tests/transforms/model_metrics_tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,51 +20,51 @@
     pprint(model_reg.list_inference_runs())
     pprint(model_class.list_inference_runs())
 
 
 def test_performance_metrics():
     """Test the Model Performance Metrics"""
     print("\n\n*** Performance Metrics ***")
-    pprint(model_reg.inference_metadata())
-    pprint(model_reg.performance_metrics())
-    pprint(model_class.performance_metrics())
+    pprint(model_reg.get_inference_metadata())
+    pprint(model_reg.get_inference_metrics())
+    pprint(model_class.get_inference_metrics())
 
 
 def test_retrieval_with_capture_uuid():
     """Test the retrieval of the model metrics using capture UUID"""
     capture_list = model_class.list_inference_runs()
     for capture_uuid in capture_list:
         print(f"\n\n*** Retrieval with Capture UUID ({capture_uuid}) ***")
-        pprint(model_class.inference_metadata(capture_uuid).head())  # Needed
-        pprint(model_class.performance_metrics(capture_uuid).head())  # Might be deprecated
-        pprint(model_class.predictions(capture_uuid).head())  # Needed
-        pprint(model_class.confusion_matrix(capture_uuid))  # Might be deprecated
+        pprint(model_class.get_inference_metadata(capture_uuid).head())
+        pprint(model_class.get_inference_metrics(capture_uuid).head())
+        pprint(model_class.get_inference_predictions(capture_uuid).head())
+        pprint(model_class.confusion_matrix(capture_uuid))
         # Classifiers have a list of dataframes for shap values
         shap_list = model_class.shapley_values(capture_uuid)
         for i, df in enumerate(shap_list):
             print(f"SHAP Values for Class {i}")
             pprint(df.head())
 
 
 def test_validation_predictions():
     print("\n\n*** Validation Predictions ***")
-    pprint(model_reg.validation_predictions().head())
-    pprint(model_class.validation_predictions().head())
+    pprint(model_reg._get_validation_predictions().head())
+    pprint(model_class._get_validation_predictions().head())
 
 
 def test_inference_predictions():
     print("\n\n*** Inference Predictions ***")
-    if model_reg.inference_predictions() is None:
+    if model_reg.get_inference_predictions() is None:
         print(f"Model {model_reg.uuid} has no inference predictions!")
         exit(1)
-    pprint(model_reg.inference_predictions().head())
-    if model_class.inference_predictions() is None:
+    pprint(model_reg.get_inference_predictions().head())
+    if model_class.get_inference_predictions() is None:
         print(f"Model {model_class.uuid} has no inference predictions!")
         exit(1)
-    pprint(model_class.inference_predictions().head())
+    pprint(model_class.get_inference_predictions().head())
 
 
 def test_confusion_matrix():
     print("\n\n*** Confusion Matrix ***")
     pprint(model_reg.confusion_matrix())
     pprint(model_class.confusion_matrix())
 
@@ -78,18 +78,18 @@
     for i, df in enumerate(shap_list):
         print(f"SHAP Values for Class {i}")
         pprint(df.head())
 
 
 def test_metrics_with_capture_uuid():
     """Test the Performance Metrics using a Capture UUID"""
-    metrics = model_reg.performance_metrics("training_holdout")
+    metrics = model_reg.get_inference_metrics("training_holdout")
     print("\n\n*** Performance Metrics with Capture UUID ***")
     pprint(metrics)
-    metrics = model_class.performance_metrics("training_holdout")
+    metrics = model_class.get_inference_metrics("training_holdout")
     pprint(metrics)
 
 
 @pytest.mark.long
 def test_auto_inference():
     # Run auto_inference (back track to FeatureSet)
     my_endpoint = Endpoint("abalone-regression-end")
```

### Comparing `sageworks-0.6.6/tests/transforms/model_to_endpoint_tests.py` & `sageworks-0.6.8/tests/transforms/model_to_endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/transforms/pandas_to_data_tests.py` & `sageworks-0.6.8/tests/transforms/pandas_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/web_components/confusion_matrix_test.py` & `sageworks-0.6.8/tests/web_components/confusion_matrix_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/web_components/correlation_matrix_test.py` & `sageworks-0.6.8/tests/web_components/correlation_matrix_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tests/web_components/plugin_interface_test.py` & `sageworks-0.6.8/tests/web_components/plugin_interface_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/tox.ini` & `sageworks-0.6.8/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     tox>=4
 env_list = black, flake8, py310
 
 [testenv]
 description = Run unit tests
 passenv = SAGEWORKS_CONFIG
 deps =
-    pytest>=7
+    pytest
     pytest-sugar
     coverage
     pytest-cov
 commands =
     pytest -x -m "not long" {posargs:tests}
 
 [testenv:debug]
```

### Comparing `sageworks-0.6.6/ui_testing/assets/custom.css` & `sageworks-0.6.8/ui_testing/assets/custom.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/ui_testing/table_comparison.py` & `sageworks-0.6.8/ui_testing/table_comparison.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/ui_testing/theme_switching.py` & `sageworks-0.6.8/ui_testing/theme_switching.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.6/ui_testing/theme_switching_2.py` & `sageworks-0.6.8/ui_testing/theme_switching_2.py`

 * *Files identical despite different names*

