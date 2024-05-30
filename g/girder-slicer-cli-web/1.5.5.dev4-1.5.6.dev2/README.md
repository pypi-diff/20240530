# Comparing `tmp/girder_slicer_cli_web-1.5.5.dev4.tar.gz` & `tmp/girder_slicer_cli_web-1.5.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder_slicer_cli_web-1.5.5.dev4.tar", last modified: Thu May 30 01:15:45 2024, max compression
+gzip compressed data, was "girder_slicer_cli_web-1.5.6.dev2.tar", last modified: Thu May 30 02:40:27 2024, max compression
```

## Comparing `girder_slicer_cli_web-1.5.5.dev4.tar` & `girder_slicer_cli_web-1.5.6.dev2.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.894598 girder_slicer_cli_web-1.5.5.dev4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.870597 girder_slicer_cli_web-1.5.5.dev4/.circleci/
--rw-r--r--   0 root         (0) root         (0)     7477 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/.circleci/config.yml
--rw-r--r--   0 root         (0) root         (0)     4000 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/.dockerignore
--rw-r--r--   0 root         (0) root         (0)      406 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/.editorconfig
--rw-r--r--   0 root         (0) root         (0)     1734 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1645 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    11357 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    17374 2024-05-30 01:15:45.894598 girder_slicer_cli_web-1.5.5.dev4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15959 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/README.rst
--rw-r--r--   0 root         (0) root         (0)      460 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/codecov.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.870597 girder_slicer_cli_web-1.5.5.dev4/docs/
--rw-r--r--   0 root         (0) root         (0)     1692 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/docs/worker_management.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.870597 girder_slicer_cli_web-1.5.5.dev4/example-average-color/
--rw-r--r--   0 root         (0) root         (0)     4000 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/example-average-color/.dockerignore
--rw-r--r--   0 root         (0) root         (0)      260 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/example-average-color/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      877 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/example-average-color/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.870597 girder_slicer_cli_web-1.5.5.dev4/example-average-color/average_color/
--rw-r--r--   0 root         (0) root         (0)     1515 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/example-average-color/average_color/average_color.py
--rw-r--r--   0 root         (0) root         (0)     1494 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/example-average-color/average_color/average_color.xml
--rw-r--r--   0 root         (0) root         (0)       50 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/example-average-color/cli_list.json
--rw-r--r--   0 root         (0) root         (0)     1397 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/example-average-color/cli_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.870597 girder_slicer_cli_web-1.5.5.dev4/example-girder-requests/
--rw-r--r--   0 root         (0) root         (0)      290 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/example-girder-requests/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      507 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/example-girder-requests/README.rst
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/example-girder-requests/cli_list.json
--rw-r--r--   0 root         (0) root         (0)     1397 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/example-girder-requests/cli_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.870597 girder_slicer_cli_web-1.5.5.dev4/example-girder-requests/girder_requests/
--rw-r--r--   0 root         (0) root         (0)      503 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/example-girder-requests/girder_requests/girder_requests.py
--rw-r--r--   0 root         (0) root         (0)     1223 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/example-girder-requests/girder_requests/girder_requests.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.894598 girder_slicer_cli_web-1.5.5.dev4/girder_slicer_cli_web.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17374 2024-05-30 01:15:45.000000 girder_slicer_cli_web-1.5.5.dev4/girder_slicer_cli_web.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6054 2024-05-30 01:15:45.000000 girder_slicer_cli_web-1.5.5.dev4/girder_slicer_cli_web.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 01:15:45.000000 girder_slicer_cli_web-1.5.5.dev4/girder_slicer_cli_web.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      184 2024-05-30 01:15:45.000000 girder_slicer_cli_web-1.5.5.dev4/girder_slicer_cli_web.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 01:15:14.000000 girder_slicer_cli_web-1.5.5.dev4/girder_slicer_cli_web.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      172 2024-05-30 01:15:45.000000 girder_slicer_cli_web-1.5.5.dev4/girder_slicer_cli_web.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-30 01:15:45.000000 girder_slicer_cli_web-1.5.5.dev4/girder_slicer_cli_web.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       67 2024-05-30 01:15:45.894598 girder_slicer_cli_web-1.5.5.dev4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2714 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.874597 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/
--rw-r--r--   0 root         (0) root         (0)     1191 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3558 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/cli_list_entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     2501 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/cli_utils.py
--rw-r--r--   0 root         (0) root         (0)     3109 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/config.py
--rw-r--r--   0 root         (0) root         (0)     6649 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/ctk_cli_adjustment.py
--rw-r--r--   0 root         (0) root         (0)    15908 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/docker_resource.py
--rw-r--r--   0 root         (0) root         (0)     3055 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/girder_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.874597 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/girder_worker_plugin/
--rw-r--r--   0 root         (0) root         (0)     1018 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/girder_worker_plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2553 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/girder_worker_plugin/cli_progress.py
--rw-r--r--   0 root         (0) root         (0)     3834 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/girder_worker_plugin/direct_docker_run.py
--rw-r--r--   0 root         (0) root         (0)    12298 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/image_job.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.874597 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/models/
--rw-r--r--   0 root         (0) root         (0)      208 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10406 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/models/docker_image.py
--rw-r--r--   0 root         (0) root         (0)      809 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/models/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     3045 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/models/json_to_xml.py
--rw-r--r--   0 root         (0) root         (0)     2340 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/models/parser.py
--rw-r--r--   0 root         (0) root         (0)    31703 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/models/schema.json
--rw-r--r--   0 root         (0) root         (0)    14268 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/prepare_task.py
--rw-r--r--   0 root         (0) root         (0)    25905 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/rest_slicer_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.878597 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/JobStatus.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.878597 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/collections/
--rw-r--r--   0 root         (0) root         (0)     1537 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/collections/WidgetCollection.js
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/collections/index.js
--rw-r--r--   0 root         (0) root         (0)       78 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/events.js
--rw-r--r--   0 root         (0) root         (0)      299 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/index.js
--rw-r--r--   0 root         (0) root         (0)      343 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/main.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.878597 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/models/
--rw-r--r--   0 root         (0) root         (0)     9697 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/models/WidgetModel.js
--rw-r--r--   0 root         (0) root         (0)       56 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/models/index.js
--rw-r--r--   0 root         (0) root         (0)     3996 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.878597 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/parser/
--rw-r--r--   0 root         (0) root         (0)      540 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/parser/constraints.js
--rw-r--r--   0 root         (0) root         (0)      610 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/parser/convert.js
--rw-r--r--   0 root         (0) root         (0)      671 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/parser/defaultValue.js
--rw-r--r--   0 root         (0) root         (0)      894 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/parser/group.js
--rw-r--r--   0 root         (0) root         (0)      384 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/parser/index.js
--rw-r--r--   0 root         (0) root         (0)      506 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/parser/panel.js
--rw-r--r--   0 root         (0) root         (0)     2543 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/parser/param.js
--rw-r--r--   0 root         (0) root         (0)     1595 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/parser/parse.js
--rw-r--r--   0 root         (0) root         (0)      921 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/parser/widget.js
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/routes.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.878597 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/stylesheets/
--rw-r--r--   0 root         (0) root         (0)       93 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/stylesheets/configView.styl
--rw-r--r--   0 root         (0) root         (0)      964 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/stylesheets/controlWidget.styl
--rw-r--r--   0 root         (0) root         (0)      112 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/stylesheets/controlsPanel.styl
--rw-r--r--   0 root         (0) root         (0)       85 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/stylesheets/outputParameterDialog.styl
--rw-r--r--   0 root         (0) root         (0)      662 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/stylesheets/panel.styl
--rw-r--r--   0 root         (0) root         (0)      197 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/stylesheets/panelGroup.styl
--rw-r--r--   0 root         (0) root         (0)      370 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/stylesheets/slicerUI.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.882597 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/
--rw-r--r--   0 root         (0) root         (0)      256 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/booleanWidget.pug
--rw-r--r--   0 root         (0) root         (0)      115 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/colorWidget.pug
--rw-r--r--   0 root         (0) root         (0)     2165 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/configView.pug
--rw-r--r--   0 root         (0) root         (0)       42 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/controlsPanel.pug
--rw-r--r--   0 root         (0) root         (0)      136 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/enumerationWidget.pug
--rw-r--r--   0 root         (0) root         (0)     1305 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/fileWidget.pug
--rw-r--r--   0 root         (0) root         (0)      621 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/jobsListWidget.pug
--rw-r--r--   0 root         (0) root         (0)      336 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/outputParameterDialog.pug
--rw-r--r--   0 root         (0) root         (0)      408 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/panel.pug
--rw-r--r--   0 root         (0) root         (0)      529 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/panelGroup.pug
--rw-r--r--   0 root         (0) root         (0)      184 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/rangeWidget.pug
--rw-r--r--   0 root         (0) root         (0)     3623 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/regionWidget.pug
--rw-r--r--   0 root         (0) root         (0)      308 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/slicerUI.pug
--rw-r--r--   0 root         (0) root         (0)      735 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/uploadImageDialog.pug
--rw-r--r--   0 root         (0) root         (0)      569 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/widget.pug
--rw-r--r--   0 root         (0) root         (0)     1642 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/utils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.886597 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/
--rw-r--r--   0 root         (0) root         (0)     4761 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/CollectionView.js
--rw-r--r--   0 root         (0) root         (0)     7145 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/ConfigView.js
--rw-r--r--   0 root         (0) root         (0)    17917 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/ControlWidget.js
--rw-r--r--   0 root         (0) root         (0)     1542 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/ControlsPanel.js
--rw-r--r--   0 root         (0) root         (0)    11455 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/ItemSelectorWidget.js
--rw-r--r--   0 root         (0) root         (0)     4584 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/ItemView.js
--rw-r--r--   0 root         (0) root         (0)     3798 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/JobsListWidget.js
--rw-r--r--   0 root         (0) root         (0)      799 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/JobsPanel.js
--rw-r--r--   0 root         (0) root         (0)      532 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/OutputParameterDialog.js
--rw-r--r--   0 root         (0) root         (0)     1150 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/Panel.js
--rw-r--r--   0 root         (0) root         (0)     8424 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/PanelGroup.js
--rw-r--r--   0 root         (0) root         (0)      394 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/index.js
--rw-r--r--   0 root         (0) root         (0)      872 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/utils.js
--rw-r--r--   0 root         (0) root         (0)     7792 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/worker_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.886597 girder_slicer_cli_web-1.5.5.dev4/small-docker/
--rw-r--r--   0 root         (0) root         (0)     4000 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/small-docker/.dockerignore
--rw-r--r--   0 root         (0) root         (0)      720 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/small-docker/Dockerfile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.886597 girder_slicer_cli_web-1.5.5.dev4/small-docker/Example1/
--rw-r--r--   0 root         (0) root         (0)    11001 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/small-docker/Example1/Example1.json
--rw-r--r--   0 root         (0) root         (0)      681 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/small-docker/Example1/Example1.py
--rw-r--r--   0 root         (0) root         (0)    10702 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/small-docker/Example1/Example1.xml
--rw-r--r--   0 root         (0) root         (0)     7535 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/small-docker/Example1/Example1.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.886597 girder_slicer_cli_web-1.5.5.dev4/small-docker/Example2/
--rw-r--r--   0 root         (0) root         (0)     1042 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/small-docker/Example2/Example2.json
--rw-r--r--   0 root         (0) root         (0)      678 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/small-docker/Example2/Example2.py
--rw-r--r--   0 root         (0) root         (0)     1023 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/small-docker/Example2/Example2.xml
--rw-r--r--   0 root         (0) root         (0)      639 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/small-docker/Example2/Example2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.886597 girder_slicer_cli_web-1.5.5.dev4/small-docker/Example3/
--rw-r--r--   0 root         (0) root         (0)     1035 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/small-docker/Example3/Example3.json
--rw-r--r--   0 root         (0) root         (0)      621 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/small-docker/Example3/Example3.py
--rw-r--r--   0 root         (0) root         (0)     1001 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/small-docker/Example3/Example3.xml
--rw-r--r--   0 root         (0) root         (0)      626 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/small-docker/Example3/Example3.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.886597 girder_slicer_cli_web-1.5.5.dev4/small-docker/ExampleProgress/
--rw-r--r--   0 root         (0) root         (0)      855 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/small-docker/ExampleProgress/ExampleProgress.json
--rw-r--r--   0 root         (0) root         (0)      884 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/small-docker/ExampleProgress/ExampleProgress.py
--rw-r--r--   0 root         (0) root         (0)     1269 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/small-docker/ExampleProgress/progress_helper.py
--rw-r--r--   0 root         (0) root         (0)      523 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/small-docker/cli_list.json
--rw-r--r--   0 root         (0) root         (0)     1397 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/small-docker/cli_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.890597 girder_slicer_cli_web-1.5.5.dev4/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10313 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.890597 girder_slicer_cli_web-1.5.5.dev4/tests/data/
--rw-r--r--   0 root         (0) root         (0)     3850 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/data/ExampleSpec.xml
--rw-r--r--   0 root         (0) root         (0)      301 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/data/girder_worker.cfg
--rw-r--r--   0 root         (0) root         (0)     1235 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/data/parser_params_advanced.json
--rw-r--r--   0 root         (0) root         (0)     1183 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/data/parser_params_advanced.xml
--rw-r--r--   0 root         (0) root         (0)      681 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/data/parser_params_advanced.yaml
--rw-r--r--   0 root         (0) root         (0)      232 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/data/parser_params_simple.json
--rw-r--r--   0 root         (0) root         (0)      218 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/data/parser_params_simple.xml
--rw-r--r--   0 root         (0) root         (0)      109 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/data/parser_params_simple.yaml
--rw-r--r--   0 root         (0) root         (0)      272 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/data/parser_simple.json
--rw-r--r--   0 root         (0) root         (0)      319 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/data/parser_simple.xml
--rw-r--r--   0 root         (0) root         (0)      152 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/data/parser_simple.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.890597 girder_slicer_cli_web-1.5.5.dev4/tests/girder_worker_plugin/
--rw-r--r--   0 root         (0) root         (0)     2769 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/girder_worker_plugin/test_cli_progress.py
--rw-r--r--   0 root         (0) root         (0)     1799 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/girder_worker_plugin/test_direct_docker_run.py
--rw-r--r--   0 root         (0) root         (0)     4961 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/test_batch.py
--rw-r--r--   0 root         (0) root         (0)      762 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)     6041 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/test_docker.py
--rwxr-xr-x   0 root         (0) root         (0)      931 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/test_load.py
--rw-r--r--   0 root         (0) root         (0)     5923 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/test_parser.py
--rw-r--r--   0 root         (0) root         (0)    10568 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/test_rest_slicer_cli.py
--rw-r--r--   0 root         (0) root         (0)      867 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/test_web_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.890597 girder_slicer_cli_web-1.5.5.dev4/tests/web_client_specs/
--rw-r--r--   0 root         (0) root         (0)      237 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/web_client_specs/.eslintrc
--rw-r--r--   0 root         (0) root         (0)     2410 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/web_client_specs/configViewSpec.js
--rw-r--r--   0 root         (0) root         (0)     4543 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/web_client_specs/containerViewSpec.js
--rw-r--r--   0 root         (0) root         (0)     6091 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/web_client_specs/dockerTaskSpec.js
--rw-r--r--   0 root         (0) root         (0)     9891 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/web_client_specs/itemSelectorWidgetSpec.js
--rw-r--r--   0 root         (0) root         (0)     2503 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/web_client_specs/panelGroupSpec.js
--rw-r--r--   0 root         (0) root         (0)    27360 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/web_client_specs/parseSpec.js
--rw-r--r--   0 root         (0) root         (0)    43069 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tests/web_client_specs/widgetSpec.js
--rw-r--r--   0 root         (0) root         (0)     2488 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/tox.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:15:45.890597 girder_slicer_cli_web-1.5.5.dev4/utils/
--rw-r--r--   0 root         (0) root         (0)     3878 2024-05-30 01:15:00.000000 girder_slicer_cli_web-1.5.5.dev4/utils/xmltojson.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.325526 girder_slicer_cli_web-1.5.6.dev2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.301526 girder_slicer_cli_web-1.5.6.dev2/.circleci/
+-rw-r--r--   0 root         (0) root         (0)     7477 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/.circleci/config.yml
+-rw-r--r--   0 root         (0) root         (0)     4000 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/.dockerignore
+-rw-r--r--   0 root         (0) root         (0)      406 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/.editorconfig
+-rw-r--r--   0 root         (0) root         (0)     1734 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1645 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    17374 2024-05-30 02:40:27.325526 girder_slicer_cli_web-1.5.6.dev2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15959 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/README.rst
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/codecov.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.301526 girder_slicer_cli_web-1.5.6.dev2/docs/
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/docs/worker_management.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.301526 girder_slicer_cli_web-1.5.6.dev2/example-average-color/
+-rw-r--r--   0 root         (0) root         (0)     4000 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/example-average-color/.dockerignore
+-rw-r--r--   0 root         (0) root         (0)      260 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/example-average-color/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      877 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/example-average-color/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.301526 girder_slicer_cli_web-1.5.6.dev2/example-average-color/average_color/
+-rw-r--r--   0 root         (0) root         (0)     1515 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/example-average-color/average_color/average_color.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/example-average-color/average_color/average_color.xml
+-rw-r--r--   0 root         (0) root         (0)       50 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/example-average-color/cli_list.json
+-rw-r--r--   0 root         (0) root         (0)     1397 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/example-average-color/cli_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.301526 girder_slicer_cli_web-1.5.6.dev2/example-girder-requests/
+-rw-r--r--   0 root         (0) root         (0)      290 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/example-girder-requests/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      507 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/example-girder-requests/README.rst
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/example-girder-requests/cli_list.json
+-rw-r--r--   0 root         (0) root         (0)     1397 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/example-girder-requests/cli_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.301526 girder_slicer_cli_web-1.5.6.dev2/example-girder-requests/girder_requests/
+-rw-r--r--   0 root         (0) root         (0)      503 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/example-girder-requests/girder_requests/girder_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1223 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/example-girder-requests/girder_requests/girder_requests.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.325526 girder_slicer_cli_web-1.5.6.dev2/girder_slicer_cli_web.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17374 2024-05-30 02:40:27.000000 girder_slicer_cli_web-1.5.6.dev2/girder_slicer_cli_web.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6054 2024-05-30 02:40:27.000000 girder_slicer_cli_web-1.5.6.dev2/girder_slicer_cli_web.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 02:40:27.000000 girder_slicer_cli_web-1.5.6.dev2/girder_slicer_cli_web.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      184 2024-05-30 02:40:27.000000 girder_slicer_cli_web-1.5.6.dev2/girder_slicer_cli_web.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 02:39:55.000000 girder_slicer_cli_web-1.5.6.dev2/girder_slicer_cli_web.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      172 2024-05-30 02:40:27.000000 girder_slicer_cli_web-1.5.6.dev2/girder_slicer_cli_web.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-30 02:40:27.000000 girder_slicer_cli_web-1.5.6.dev2/girder_slicer_cli_web.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-30 02:40:27.325526 girder_slicer_cli_web-1.5.6.dev2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2714 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.305526 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/
+-rw-r--r--   0 root         (0) root         (0)     1191 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/cli_list_entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/cli_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/config.py
+-rw-r--r--   0 root         (0) root         (0)     6649 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/ctk_cli_adjustment.py
+-rw-r--r--   0 root         (0) root         (0)    15908 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/docker_resource.py
+-rw-r--r--   0 root         (0) root         (0)     3055 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/girder_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.305526 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/girder_worker_plugin/
+-rw-r--r--   0 root         (0) root         (0)     1018 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/girder_worker_plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2553 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/girder_worker_plugin/cli_progress.py
+-rw-r--r--   0 root         (0) root         (0)     3834 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/girder_worker_plugin/direct_docker_run.py
+-rw-r--r--   0 root         (0) root         (0)    12298 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/image_job.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.305526 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/models/
+-rw-r--r--   0 root         (0) root         (0)      208 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10406 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/models/docker_image.py
+-rw-r--r--   0 root         (0) root         (0)      809 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/models/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     3045 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/models/json_to_xml.py
+-rw-r--r--   0 root         (0) root         (0)     2340 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/models/parser.py
+-rw-r--r--   0 root         (0) root         (0)    31703 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/models/schema.json
+-rw-r--r--   0 root         (0) root         (0)    14268 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/prepare_task.py
+-rw-r--r--   0 root         (0) root         (0)    25905 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/rest_slicer_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.309526 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/JobStatus.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.309526 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/collections/
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/collections/WidgetCollection.js
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/collections/index.js
+-rw-r--r--   0 root         (0) root         (0)       78 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/events.js
+-rw-r--r--   0 root         (0) root         (0)      299 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/index.js
+-rw-r--r--   0 root         (0) root         (0)      343 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/main.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.309526 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/models/
+-rw-r--r--   0 root         (0) root         (0)     9697 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/models/WidgetModel.js
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/models/index.js
+-rw-r--r--   0 root         (0) root         (0)     3996 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.309526 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/parser/
+-rw-r--r--   0 root         (0) root         (0)      540 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/parser/constraints.js
+-rw-r--r--   0 root         (0) root         (0)      610 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/parser/convert.js
+-rw-r--r--   0 root         (0) root         (0)      671 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/parser/defaultValue.js
+-rw-r--r--   0 root         (0) root         (0)      894 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/parser/group.js
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/parser/index.js
+-rw-r--r--   0 root         (0) root         (0)      506 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/parser/panel.js
+-rw-r--r--   0 root         (0) root         (0)     2543 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/parser/param.js
+-rw-r--r--   0 root         (0) root         (0)     1595 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/parser/parse.js
+-rw-r--r--   0 root         (0) root         (0)      921 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/parser/widget.js
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/routes.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.309526 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/stylesheets/
+-rw-r--r--   0 root         (0) root         (0)       93 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/stylesheets/configView.styl
+-rw-r--r--   0 root         (0) root         (0)      964 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/stylesheets/controlWidget.styl
+-rw-r--r--   0 root         (0) root         (0)      112 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/stylesheets/controlsPanel.styl
+-rw-r--r--   0 root         (0) root         (0)       85 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/stylesheets/outputParameterDialog.styl
+-rw-r--r--   0 root         (0) root         (0)      662 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/stylesheets/panel.styl
+-rw-r--r--   0 root         (0) root         (0)      197 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/stylesheets/panelGroup.styl
+-rw-r--r--   0 root         (0) root         (0)      370 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/stylesheets/slicerUI.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.313526 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/
+-rw-r--r--   0 root         (0) root         (0)      256 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/booleanWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      115 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/colorWidget.pug
+-rw-r--r--   0 root         (0) root         (0)     2165 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/configView.pug
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/controlsPanel.pug
+-rw-r--r--   0 root         (0) root         (0)      136 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/enumerationWidget.pug
+-rw-r--r--   0 root         (0) root         (0)     1305 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/fileWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      621 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/jobsListWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      336 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/outputParameterDialog.pug
+-rw-r--r--   0 root         (0) root         (0)      408 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/panel.pug
+-rw-r--r--   0 root         (0) root         (0)      529 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/panelGroup.pug
+-rw-r--r--   0 root         (0) root         (0)      184 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/rangeWidget.pug
+-rw-r--r--   0 root         (0) root         (0)     3623 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/regionWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      308 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/slicerUI.pug
+-rw-r--r--   0 root         (0) root         (0)      735 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/uploadImageDialog.pug
+-rw-r--r--   0 root         (0) root         (0)      569 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/widget.pug
+-rw-r--r--   0 root         (0) root         (0)     1642 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/utils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.317526 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/
+-rw-r--r--   0 root         (0) root         (0)     4761 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/CollectionView.js
+-rw-r--r--   0 root         (0) root         (0)     7145 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/ConfigView.js
+-rw-r--r--   0 root         (0) root         (0)    18232 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/ControlWidget.js
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/ControlsPanel.js
+-rw-r--r--   0 root         (0) root         (0)    11455 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/ItemSelectorWidget.js
+-rw-r--r--   0 root         (0) root         (0)     4584 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/ItemView.js
+-rw-r--r--   0 root         (0) root         (0)     3798 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/JobsListWidget.js
+-rw-r--r--   0 root         (0) root         (0)      799 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/JobsPanel.js
+-rw-r--r--   0 root         (0) root         (0)      532 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/OutputParameterDialog.js
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/Panel.js
+-rw-r--r--   0 root         (0) root         (0)     8424 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/PanelGroup.js
+-rw-r--r--   0 root         (0) root         (0)      394 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/index.js
+-rw-r--r--   0 root         (0) root         (0)      872 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/utils.js
+-rw-r--r--   0 root         (0) root         (0)     7792 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/worker_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.317526 girder_slicer_cli_web-1.5.6.dev2/small-docker/
+-rw-r--r--   0 root         (0) root         (0)     4000 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/small-docker/.dockerignore
+-rw-r--r--   0 root         (0) root         (0)      720 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/small-docker/Dockerfile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.317526 girder_slicer_cli_web-1.5.6.dev2/small-docker/Example1/
+-rw-r--r--   0 root         (0) root         (0)    11001 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/small-docker/Example1/Example1.json
+-rw-r--r--   0 root         (0) root         (0)      681 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/small-docker/Example1/Example1.py
+-rw-r--r--   0 root         (0) root         (0)    10702 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/small-docker/Example1/Example1.xml
+-rw-r--r--   0 root         (0) root         (0)     7535 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/small-docker/Example1/Example1.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.317526 girder_slicer_cli_web-1.5.6.dev2/small-docker/Example2/
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/small-docker/Example2/Example2.json
+-rw-r--r--   0 root         (0) root         (0)      678 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/small-docker/Example2/Example2.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/small-docker/Example2/Example2.xml
+-rw-r--r--   0 root         (0) root         (0)      639 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/small-docker/Example2/Example2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.317526 girder_slicer_cli_web-1.5.6.dev2/small-docker/Example3/
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/small-docker/Example3/Example3.json
+-rw-r--r--   0 root         (0) root         (0)      621 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/small-docker/Example3/Example3.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/small-docker/Example3/Example3.xml
+-rw-r--r--   0 root         (0) root         (0)      626 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/small-docker/Example3/Example3.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.317526 girder_slicer_cli_web-1.5.6.dev2/small-docker/ExampleProgress/
+-rw-r--r--   0 root         (0) root         (0)      855 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/small-docker/ExampleProgress/ExampleProgress.json
+-rw-r--r--   0 root         (0) root         (0)      884 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/small-docker/ExampleProgress/ExampleProgress.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/small-docker/ExampleProgress/progress_helper.py
+-rw-r--r--   0 root         (0) root         (0)      523 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/small-docker/cli_list.json
+-rw-r--r--   0 root         (0) root         (0)     1397 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/small-docker/cli_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.321526 girder_slicer_cli_web-1.5.6.dev2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10313 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.321526 girder_slicer_cli_web-1.5.6.dev2/tests/data/
+-rw-r--r--   0 root         (0) root         (0)     3850 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/data/ExampleSpec.xml
+-rw-r--r--   0 root         (0) root         (0)      301 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/data/girder_worker.cfg
+-rw-r--r--   0 root         (0) root         (0)     1235 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/data/parser_params_advanced.json
+-rw-r--r--   0 root         (0) root         (0)     1183 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/data/parser_params_advanced.xml
+-rw-r--r--   0 root         (0) root         (0)      681 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/data/parser_params_advanced.yaml
+-rw-r--r--   0 root         (0) root         (0)      232 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/data/parser_params_simple.json
+-rw-r--r--   0 root         (0) root         (0)      218 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/data/parser_params_simple.xml
+-rw-r--r--   0 root         (0) root         (0)      109 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/data/parser_params_simple.yaml
+-rw-r--r--   0 root         (0) root         (0)      272 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/data/parser_simple.json
+-rw-r--r--   0 root         (0) root         (0)      319 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/data/parser_simple.xml
+-rw-r--r--   0 root         (0) root         (0)      152 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/data/parser_simple.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.321526 girder_slicer_cli_web-1.5.6.dev2/tests/girder_worker_plugin/
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/girder_worker_plugin/test_cli_progress.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/girder_worker_plugin/test_direct_docker_run.py
+-rw-r--r--   0 root         (0) root         (0)     4961 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/test_batch.py
+-rw-r--r--   0 root         (0) root         (0)      762 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     6041 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/test_docker.py
+-rwxr-xr-x   0 root         (0) root         (0)      931 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/test_load.py
+-rw-r--r--   0 root         (0) root         (0)     5923 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/test_parser.py
+-rw-r--r--   0 root         (0) root         (0)    10568 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/test_rest_slicer_cli.py
+-rw-r--r--   0 root         (0) root         (0)      867 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/test_web_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.325526 girder_slicer_cli_web-1.5.6.dev2/tests/web_client_specs/
+-rw-r--r--   0 root         (0) root         (0)      237 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/web_client_specs/.eslintrc
+-rw-r--r--   0 root         (0) root         (0)     2410 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/web_client_specs/configViewSpec.js
+-rw-r--r--   0 root         (0) root         (0)     4543 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/web_client_specs/containerViewSpec.js
+-rw-r--r--   0 root         (0) root         (0)     6091 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/web_client_specs/dockerTaskSpec.js
+-rw-r--r--   0 root         (0) root         (0)     9891 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/web_client_specs/itemSelectorWidgetSpec.js
+-rw-r--r--   0 root         (0) root         (0)     2503 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/web_client_specs/panelGroupSpec.js
+-rw-r--r--   0 root         (0) root         (0)    27360 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/web_client_specs/parseSpec.js
+-rw-r--r--   0 root         (0) root         (0)    43069 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tests/web_client_specs/widgetSpec.js
+-rw-r--r--   0 root         (0) root         (0)     2488 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:40:27.325526 girder_slicer_cli_web-1.5.6.dev2/utils/
+-rw-r--r--   0 root         (0) root         (0)     3878 2024-05-30 02:39:41.000000 girder_slicer_cli_web-1.5.6.dev2/utils/xmltojson.py
```

### Comparing `girder_slicer_cli_web-1.5.5.dev4/.circleci/config.yml` & `girder_slicer_cli_web-1.5.6.dev2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/.dockerignore` & `girder_slicer_cli_web-1.5.6.dev2/.dockerignore`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/.gitignore` & `girder_slicer_cli_web-1.5.6.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/.pre-commit-config.yaml` & `girder_slicer_cli_web-1.5.6.dev2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/LICENSE` & `girder_slicer_cli_web-1.5.6.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/PKG-INFO` & `girder_slicer_cli_web-1.5.6.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-slicer-cli-web
-Version: 1.5.5.dev4
+Version: 1.5.6.dev2
 Summary: A girder plugin for exposing slicer CLIs over the web
 Home-page: https://github.com/girder/slicer_cli_web
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: girder-plugin,slicer_cli_web
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `girder_slicer_cli_web-1.5.5.dev4/README.rst` & `girder_slicer_cli_web-1.5.6.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/docs/worker_management.rst` & `girder_slicer_cli_web-1.5.6.dev2/docs/worker_management.rst`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/example-average-color/.dockerignore` & `girder_slicer_cli_web-1.5.6.dev2/example-average-color/.dockerignore`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/example-average-color/README.rst` & `girder_slicer_cli_web-1.5.6.dev2/example-average-color/README.rst`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/example-average-color/average_color/average_color.py` & `girder_slicer_cli_web-1.5.6.dev2/example-average-color/average_color/average_color.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/example-average-color/average_color/average_color.xml` & `girder_slicer_cli_web-1.5.6.dev2/example-average-color/average_color/average_color.xml`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/example-average-color/cli_list.py` & `girder_slicer_cli_web-1.5.6.dev2/example-average-color/cli_list.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/example-girder-requests/cli_list.py` & `girder_slicer_cli_web-1.5.6.dev2/example-girder-requests/cli_list.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/example-girder-requests/girder_requests/girder_requests.xml` & `girder_slicer_cli_web-1.5.6.dev2/example-girder-requests/girder_requests/girder_requests.xml`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/girder_slicer_cli_web.egg-info/PKG-INFO` & `girder_slicer_cli_web-1.5.6.dev2/girder_slicer_cli_web.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-slicer-cli-web
-Version: 1.5.5.dev4
+Version: 1.5.6.dev2
 Summary: A girder plugin for exposing slicer CLIs over the web
 Home-page: https://github.com/girder/slicer_cli_web
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: girder-plugin,slicer_cli_web
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `girder_slicer_cli_web-1.5.5.dev4/girder_slicer_cli_web.egg-info/SOURCES.txt` & `girder_slicer_cli_web-1.5.6.dev2/girder_slicer_cli_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/setup.py` & `girder_slicer_cli_web-1.5.6.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/__init__.py` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/__init__.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/cli_list_entrypoint.py` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/cli_list_entrypoint.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/cli_utils.py` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/cli_utils.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/config.py` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/config.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/ctk_cli_adjustment.py` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/ctk_cli_adjustment.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/docker_resource.py` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/docker_resource.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/girder_plugin.py` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/girder_plugin.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/girder_worker_plugin/__init__.py` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/girder_worker_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/girder_worker_plugin/cli_progress.py` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/girder_worker_plugin/cli_progress.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/girder_worker_plugin/direct_docker_run.py` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/girder_worker_plugin/direct_docker_run.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/image_job.py` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/image_job.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/models/docker_image.py` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/models/docker_image.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/models/exceptions.py` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/models/json_to_xml.py` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/models/json_to_xml.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/models/parser.py` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/models/parser.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/models/schema.json` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/models/schema.json`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/prepare_task.py` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/prepare_task.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/rest_slicer_cli.py` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/rest_slicer_cli.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/collections/WidgetCollection.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/collections/WidgetCollection.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/models/WidgetModel.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/models/WidgetModel.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/package.json` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/parser/constraints.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/parser/constraints.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/parser/convert.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/parser/convert.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/parser/defaultValue.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/parser/defaultValue.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/parser/group.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/parser/group.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/parser/param.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/parser/param.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/parser/parse.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/parser/parse.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/parser/widget.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/parser/widget.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/stylesheets/controlWidget.styl` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/stylesheets/controlWidget.styl`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/stylesheets/panel.styl` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/stylesheets/panel.styl`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/configView.pug` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/fileWidget.pug` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/fileWidget.pug`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/jobsListWidget.pug` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/jobsListWidget.pug`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/panelGroup.pug` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/panelGroup.pug`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/regionWidget.pug` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/regionWidget.pug`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/uploadImageDialog.pug` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/uploadImageDialog.pug`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/templates/widget.pug` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/templates/widget.pug`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/utils.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/utils.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/CollectionView.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/CollectionView.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/ConfigView.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/ControlWidget.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/ControlWidget.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -384,24 +384,32 @@
         } else {
             this.completeInitialization(settings);
         }
     },
     completeInitialization(settings) {
         const modal = new ItemSelectorWidget(settings);
         modal.once('g:saved', () => {
+            this.model.unset('revertType');
             modal.$el.modal('hide');
         }).render();
+        modal.$el.on('hidden.bs.modal', () => {
+            if (this.model.get('revertType')) {
+                this.model.set('type', this.model.get('revertType'));
+                this.model.unset('revertType');
+            }
+        });
     },
     _selectMultiFile() {
         // Store the current type in case it is opened again
         const t = this.model.get('type');
         if (t !== 'multi') {
             this.model.set({
                 type: 'multi',
-                defaultType: t
+                defaultType: t,
+                revertType: t
             });
         }
 
         const itemSelectorSettings = {
             el: $('#g-dialog-container'),
             parentView: this,
             model: this.model,
```

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/ControlsPanel.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/ControlsPanel.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/ItemSelectorWidget.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/ItemSelectorWidget.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/ItemView.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/ItemView.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/JobsListWidget.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/JobsListWidget.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/JobsPanel.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/JobsPanel.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/OutputParameterDialog.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/OutputParameterDialog.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/Panel.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/Panel.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/PanelGroup.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/PanelGroup.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/web_client/views/utils.js` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/web_client/views/utils.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/slicer_cli_web/worker_tools.py` & `girder_slicer_cli_web-1.5.6.dev2/slicer_cli_web/worker_tools.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/small-docker/.dockerignore` & `girder_slicer_cli_web-1.5.6.dev2/small-docker/.dockerignore`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/small-docker/Dockerfile` & `girder_slicer_cli_web-1.5.6.dev2/small-docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/small-docker/Example1/Example1.json` & `girder_slicer_cli_web-1.5.6.dev2/small-docker/Example1/Example1.json`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/small-docker/Example1/Example1.py` & `girder_slicer_cli_web-1.5.6.dev2/small-docker/Example1/Example1.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/small-docker/Example1/Example1.xml` & `girder_slicer_cli_web-1.5.6.dev2/small-docker/Example1/Example1.xml`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/small-docker/Example1/Example1.yaml` & `girder_slicer_cli_web-1.5.6.dev2/small-docker/Example1/Example1.yaml`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/small-docker/Example2/Example2.json` & `girder_slicer_cli_web-1.5.6.dev2/small-docker/Example2/Example2.json`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/small-docker/Example2/Example2.py` & `girder_slicer_cli_web-1.5.6.dev2/small-docker/Example2/Example2.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/small-docker/Example2/Example2.xml` & `girder_slicer_cli_web-1.5.6.dev2/small-docker/Example2/Example2.xml`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/small-docker/Example2/Example2.yaml` & `girder_slicer_cli_web-1.5.6.dev2/small-docker/Example2/Example2.yaml`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/small-docker/Example3/Example3.json` & `girder_slicer_cli_web-1.5.6.dev2/small-docker/Example3/Example3.json`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/small-docker/Example3/Example3.py` & `girder_slicer_cli_web-1.5.6.dev2/small-docker/Example3/Example3.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/small-docker/Example3/Example3.xml` & `girder_slicer_cli_web-1.5.6.dev2/small-docker/Example3/Example3.xml`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/small-docker/Example3/Example3.yaml` & `girder_slicer_cli_web-1.5.6.dev2/small-docker/Example3/Example3.yaml`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/small-docker/ExampleProgress/ExampleProgress.json` & `girder_slicer_cli_web-1.5.6.dev2/small-docker/ExampleProgress/ExampleProgress.json`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/small-docker/ExampleProgress/ExampleProgress.py` & `girder_slicer_cli_web-1.5.6.dev2/small-docker/ExampleProgress/ExampleProgress.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/small-docker/ExampleProgress/progress_helper.py` & `girder_slicer_cli_web-1.5.6.dev2/small-docker/ExampleProgress/progress_helper.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/small-docker/cli_list.json` & `girder_slicer_cli_web-1.5.6.dev2/small-docker/cli_list.json`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/small-docker/cli_list.py` & `girder_slicer_cli_web-1.5.6.dev2/small-docker/cli_list.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/conftest.py` & `girder_slicer_cli_web-1.5.6.dev2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/data/ExampleSpec.xml` & `girder_slicer_cli_web-1.5.6.dev2/tests/data/ExampleSpec.xml`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/data/parser_params_advanced.json` & `girder_slicer_cli_web-1.5.6.dev2/tests/data/parser_params_advanced.json`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/data/parser_params_advanced.xml` & `girder_slicer_cli_web-1.5.6.dev2/tests/data/parser_params_advanced.xml`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/data/parser_params_advanced.yaml` & `girder_slicer_cli_web-1.5.6.dev2/tests/data/parser_params_advanced.yaml`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/girder_worker_plugin/test_cli_progress.py` & `girder_slicer_cli_web-1.5.6.dev2/tests/girder_worker_plugin/test_cli_progress.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/girder_worker_plugin/test_direct_docker_run.py` & `girder_slicer_cli_web-1.5.6.dev2/tests/girder_worker_plugin/test_direct_docker_run.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/test_batch.py` & `girder_slicer_cli_web-1.5.6.dev2/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/test_config.py` & `girder_slicer_cli_web-1.5.6.dev2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/test_docker.py` & `girder_slicer_cli_web-1.5.6.dev2/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/test_load.py` & `girder_slicer_cli_web-1.5.6.dev2/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/test_parser.py` & `girder_slicer_cli_web-1.5.6.dev2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/test_rest_slicer_cli.py` & `girder_slicer_cli_web-1.5.6.dev2/tests/test_rest_slicer_cli.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/test_web_client.py` & `girder_slicer_cli_web-1.5.6.dev2/tests/test_web_client.py`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/web_client_specs/configViewSpec.js` & `girder_slicer_cli_web-1.5.6.dev2/tests/web_client_specs/configViewSpec.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/web_client_specs/containerViewSpec.js` & `girder_slicer_cli_web-1.5.6.dev2/tests/web_client_specs/containerViewSpec.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/web_client_specs/dockerTaskSpec.js` & `girder_slicer_cli_web-1.5.6.dev2/tests/web_client_specs/dockerTaskSpec.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/web_client_specs/itemSelectorWidgetSpec.js` & `girder_slicer_cli_web-1.5.6.dev2/tests/web_client_specs/itemSelectorWidgetSpec.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/web_client_specs/panelGroupSpec.js` & `girder_slicer_cli_web-1.5.6.dev2/tests/web_client_specs/panelGroupSpec.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/web_client_specs/parseSpec.js` & `girder_slicer_cli_web-1.5.6.dev2/tests/web_client_specs/parseSpec.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tests/web_client_specs/widgetSpec.js` & `girder_slicer_cli_web-1.5.6.dev2/tests/web_client_specs/widgetSpec.js`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/tox.ini` & `girder_slicer_cli_web-1.5.6.dev2/tox.ini`

 * *Files identical despite different names*

### Comparing `girder_slicer_cli_web-1.5.5.dev4/utils/xmltojson.py` & `girder_slicer_cli_web-1.5.6.dev2/utils/xmltojson.py`

 * *Files identical despite different names*

