# Comparing `tmp/nodeorc-0.1.6.tar.gz` & `tmp/nodeorc-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodeorc-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "nodeorc-0.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nodeorc-0.1.6.tar` & `nodeorc-0.1.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      187 2024-04-08 12:34:50.650424 nodeorc-0.1.6/.env
--rw-r--r--   0        0        0     1146 2024-04-08 12:34:50.650424 nodeorc-0.1.6/.github/ISSUE_TEMPLATE/issue-report.md
--rw-r--r--   0        0        0     1547 2024-04-08 12:34:50.650424 nodeorc-0.1.6/.github/workflows/publish-release-pypi.yml
--rw-r--r--   0        0        0     2248 2024-04-08 12:34:50.650424 nodeorc-0.1.6/.github/workflows/publish-test-pypi.yml
--rw-r--r--   0        0        0     3129 2024-04-08 12:34:50.650424 nodeorc-0.1.6/.gitignore
--rw-r--r--   0        0        0      559 2024-04-08 12:34:50.650424 nodeorc-0.1.6/Dockerfile
--rw-r--r--   0        0        0    34523 2024-04-08 12:34:50.650424 nodeorc-0.1.6/LICENSE
--rw-r--r--   0        0        0    27141 2024-04-08 12:34:50.650424 nodeorc-0.1.6/README.rst
--rw-r--r--   0        0        0     1594 2024-04-08 12:34:50.650424 nodeorc-0.1.6/docker-compose-test.yml
--rw-r--r--   0        0        0  2525884 2024-04-08 12:34:50.662424 nodeorc-0.1.6/docs/static/front.jpg
--rw-r--r--   0        0        0     2718 2024-04-08 12:34:50.662424 nodeorc-0.1.6/mockserver/initializerJson.json
--rw-r--r--   0        0        0       93 2024-04-08 12:34:50.662424 nodeorc-0.1.6/mockserver/mockserver.properties
--rw-r--r--   0        0        0      445 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/__init__.py
--rw-r--r--   0        0        0     3705 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/callbacks.py
--rw-r--r--   0        0        0     5959 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/config.py
--rw-r--r--   0        0        0      681 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/db/__init__.py
--rw-r--r--   0        0        0      292 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/db/active_config.py
--rw-r--r--   0        0        0      741 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/db/init_basedata.py
--rw-r--r--   0        0        0    10813 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/db/models.py
--rw-r--r--   0        0        0     3761 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/disk_mng.py
--rw-r--r--   0        0        0     2858 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/log.py
--rw-r--r--   0        0        0    10288 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/main.py
--rw-r--r--   0        0        0      959 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/models/__init__.py
--rw-r--r--   0        0        0     1629 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/models/callback.py
--rw-r--r--   0        0        0     6378 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/models/callback_url.py
--rw-r--r--   0        0        0     3966 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/models/config.py
--rw-r--r--   0        0        0     3301 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/models/storage.py
--rw-r--r--   0        0        0     4356 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/models/subtask.py
--rw-r--r--   0        0        0     6261 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/models/task.py
--rw-r--r--   0        0        0      104 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/tasks/__init__.py
--rw-r--r--   0        0        0    24778 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/tasks/local_task.py
--rw-r--r--   0        0        0     8694 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/tasks/task_form.py
--rw-r--r--   0        0        0     2823 2024-04-08 12:34:50.662424 nodeorc-0.1.6/nodeorc/utils.py
--rw-r--r--   0        0        0     1282 2024-04-08 12:34:50.662424 nodeorc-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      106 2024-04-08 12:34:50.662424 nodeorc-0.1.6/requirements.txt
--rw-r--r--   0        0        0      422 2024-04-08 12:34:50.662424 nodeorc-0.1.6/service/10-toggleusbstick.rules
--rw-r--r--   0        0        0     2107 2024-04-08 12:34:50.662424 nodeorc-0.1.6/service/usb-mount.sh
--rw-r--r--   0        0        0      184 2024-04-08 12:34:50.662424 nodeorc-0.1.6/service/usb-mount@.service
--rw-r--r--   0        0        0        0 2024-04-08 12:34:50.662424 nodeorc-0.1.6/settings/.gitkeep
--rw-r--r--   0        0        0      722 2024-04-08 12:34:50.662424 nodeorc-0.1.6/settings/config_template.json
--rwxr-xr-x   0        0        0    21715 2024-04-08 12:34:50.662424 nodeorc-0.1.6/setup.sh
--rw-r--r--   0        0        0     8907 2024-04-08 12:34:50.662424 nodeorc-0.1.6/tests/conftest.py
--rw-r--r--   0        0        0    60249 2024-04-08 12:34:50.666424 nodeorc-0.1.6/tests/examples/ngwerere_transect.nc
--rw-r--r--   0        0        0      496 2024-04-08 12:34:50.666424 nodeorc-0.1.6/tests/test_amqp_task.py
--rw-r--r--   0        0        0      802 2024-04-08 12:34:50.666424 nodeorc-0.1.6/tests/test_callbacks.py
--rw-r--r--   0        0        0     2493 2024-04-08 12:34:50.666424 nodeorc-0.1.6/tests/test_config.py
--rw-r--r--   0        0        0      875 2024-04-08 12:34:50.666424 nodeorc-0.1.6/tests/test_disk_management.py
--rw-r--r--   0        0        0      128 2024-04-08 12:34:50.666424 nodeorc-0.1.6/tests/test_io.py
--rw-r--r--   0        0        0      726 2024-04-08 12:34:50.666424 nodeorc-0.1.6/tests/test_s3.py
--rw-r--r--   0        0        0      184 2024-04-08 12:34:50.666424 nodeorc-0.1.6/tests/test_task.py
--rw-r--r--   0        0        0    28618 1970-01-01 00:00:00.000000 nodeorc-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      187 2024-05-30 15:10:08.431044 nodeorc-0.1.7/.env
+-rw-r--r--   0        0        0     1146 2024-05-30 15:10:08.431044 nodeorc-0.1.7/.github/ISSUE_TEMPLATE/issue-report.md
+-rw-r--r--   0        0        0     1547 2024-05-30 15:10:08.431044 nodeorc-0.1.7/.github/workflows/publish-release-pypi.yml
+-rw-r--r--   0        0        0     2248 2024-05-30 15:10:08.431044 nodeorc-0.1.7/.github/workflows/publish-test-pypi.yml
+-rw-r--r--   0        0        0     3129 2024-05-30 15:10:08.431044 nodeorc-0.1.7/.gitignore
+-rw-r--r--   0        0        0      559 2024-05-30 15:10:08.431044 nodeorc-0.1.7/Dockerfile
+-rw-r--r--   0        0        0    34523 2024-05-30 15:10:08.431044 nodeorc-0.1.7/LICENSE
+-rw-r--r--   0        0        0    27119 2024-05-30 15:10:08.431044 nodeorc-0.1.7/README.rst
+-rw-r--r--   0        0        0     1594 2024-05-30 15:10:08.431044 nodeorc-0.1.7/docker-compose-test.yml
+-rw-r--r--   0        0        0  2525884 2024-05-30 15:10:08.439045 nodeorc-0.1.7/docs/static/front.jpg
+-rw-r--r--   0        0        0     2718 2024-05-30 15:10:08.443045 nodeorc-0.1.7/mockserver/initializerJson.json
+-rw-r--r--   0        0        0       93 2024-05-30 15:10:08.443045 nodeorc-0.1.7/mockserver/mockserver.properties
+-rw-r--r--   0        0        0      444 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/__init__.py
+-rw-r--r--   0        0        0     3705 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/callbacks.py
+-rw-r--r--   0        0        0     5959 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/config.py
+-rw-r--r--   0        0        0      681 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/db/__init__.py
+-rw-r--r--   0        0        0      292 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/db/active_config.py
+-rw-r--r--   0        0        0      741 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/db/init_basedata.py
+-rw-r--r--   0        0        0    10813 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/db/models.py
+-rw-r--r--   0        0        0     3761 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/disk_mng.py
+-rw-r--r--   0        0        0     2858 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/log.py
+-rw-r--r--   0        0        0    10033 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/main.py
+-rw-r--r--   0        0        0      974 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/models/__init__.py
+-rw-r--r--   0        0        0     1629 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/models/callback.py
+-rw-r--r--   0        0        0     6378 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/models/callback_url.py
+-rw-r--r--   0        0        0     3966 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/models/config.py
+-rw-r--r--   0        0        0     3771 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/models/storage.py
+-rw-r--r--   0        0        0     4356 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/models/subtask.py
+-rw-r--r--   0        0        0     6330 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/models/task.py
+-rw-r--r--   0        0        0      104 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/tasks/__init__.py
+-rw-r--r--   0        0        0    24778 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/tasks/local_task.py
+-rw-r--r--   0        0        0     8694 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/tasks/task_form.py
+-rw-r--r--   0        0        0     2788 2024-05-30 15:10:08.443045 nodeorc-0.1.7/nodeorc/utils.py
+-rw-r--r--   0        0        0     1282 2024-05-30 15:10:08.443045 nodeorc-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      106 2024-05-30 15:10:08.443045 nodeorc-0.1.7/requirements.txt
+-rw-r--r--   0        0        0      422 2024-05-30 15:10:08.443045 nodeorc-0.1.7/service/10-toggleusbstick.rules
+-rw-r--r--   0        0        0     2107 2024-05-30 15:10:08.443045 nodeorc-0.1.7/service/usb-mount.sh
+-rw-r--r--   0        0        0      184 2024-05-30 15:10:08.443045 nodeorc-0.1.7/service/usb-mount@.service
+-rw-r--r--   0        0        0        0 2024-05-30 15:10:08.443045 nodeorc-0.1.7/settings/.gitkeep
+-rw-r--r--   0        0        0      722 2024-05-30 15:10:08.443045 nodeorc-0.1.7/settings/config_template.json
+-rwxr-xr-x   0        0        0    21715 2024-05-30 15:10:08.443045 nodeorc-0.1.7/setup.sh
+-rw-r--r--   0        0        0     8907 2024-05-30 15:10:08.443045 nodeorc-0.1.7/tests/conftest.py
+-rw-r--r--   0        0        0    60249 2024-05-30 15:10:08.443045 nodeorc-0.1.7/tests/examples/ngwerere_transect.nc
+-rw-r--r--   0        0        0      496 2024-05-30 15:10:08.443045 nodeorc-0.1.7/tests/test_amqp_task.py
+-rw-r--r--   0        0        0      802 2024-05-30 15:10:08.443045 nodeorc-0.1.7/tests/test_callbacks.py
+-rw-r--r--   0        0        0     2493 2024-05-30 15:10:08.443045 nodeorc-0.1.7/tests/test_config.py
+-rw-r--r--   0        0        0      875 2024-05-30 15:10:08.443045 nodeorc-0.1.7/tests/test_disk_management.py
+-rw-r--r--   0        0        0      128 2024-05-30 15:10:08.443045 nodeorc-0.1.7/tests/test_io.py
+-rw-r--r--   0        0        0      726 2024-05-30 15:10:08.443045 nodeorc-0.1.7/tests/test_s3.py
+-rw-r--r--   0        0        0      184 2024-05-30 15:10:08.443045 nodeorc-0.1.7/tests/test_task.py
+-rw-r--r--   0        0        0    28596 1970-01-01 00:00:00.000000 nodeorc-0.1.7/PKG-INFO
```

### Comparing `nodeorc-0.1.6/.github/ISSUE_TEMPLATE/issue-report.md` & `nodeorc-0.1.7/.github/ISSUE_TEMPLATE/issue-report.md`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/.github/workflows/publish-release-pypi.yml` & `nodeorc-0.1.7/.github/workflows/publish-release-pypi.yml`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/.github/workflows/publish-test-pypi.yml` & `nodeorc-0.1.7/.github/workflows/publish-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/.gitignore` & `nodeorc-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/Dockerfile` & `nodeorc-0.1.7/Dockerfile`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/LICENSE` & `nodeorc-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/README.rst` & `nodeorc-0.1.7/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -525,24 +525,24 @@
         "reboot_after": 86400
 
     },
 
 
 .. _LiveORC: https://github.com/localdevices/LiveORC
 
-.. |pypi| image:: https://badge.fury.io/py/nodeopenrivercam.svg
+.. |pypi| image:: https://badge.fury.io/py/nodeorc.svg
     :alt: PyPI
-    :target: https://pypi.org/project/nodeopenrivercam/
+    :target: https://pypi.org/project/nodeorc/
 
-.. |piwheels| image:: https://img.shields.io/piwheels/v/:wheel
+.. |piwheels| image:: https://img.shields.io/piwheels/v/nodeorc
    :alt: PiWheels Version
    :target: https://localdevice.github.io/nodeorc/latest
 
 .. |docs_latest| image:: https://img.shields.io/badge/docs-latest-brightgreen.svg
     :alt: Latest documentation
-    :target: https://localdevice.github.io/nodeorc/latest
+    :target: https://github.com/localdevices/nodeorc
 
 
 .. |license| image:: https://img.shields.io/github/license/localdevices/nodeorc?style=flat
     :alt: License
     :target: https://github.com/localdevices/nodeorc/blob/main/LICENSE
```

### Comparing `nodeorc-0.1.6/docker-compose-test.yml` & `nodeorc-0.1.7/docker-compose-test.yml`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/docs/static/front.jpg` & `nodeorc-0.1.7/docs/static/front.jpg`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/mockserver/initializerJson.json` & `nodeorc-0.1.7/mockserver/initializerJson.json`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/nodeorc/callbacks.py` & `nodeorc-0.1.7/nodeorc/callbacks.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/nodeorc/config.py` & `nodeorc-0.1.7/nodeorc/config.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/nodeorc/db/__init__.py` & `nodeorc-0.1.7/nodeorc/db/__init__.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/nodeorc/db/init_basedata.py` & `nodeorc-0.1.7/nodeorc/db/init_basedata.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/nodeorc/db/models.py` & `nodeorc-0.1.7/nodeorc/db/models.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/nodeorc/disk_mng.py` & `nodeorc-0.1.7/nodeorc/disk_mng.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/nodeorc/log.py` & `nodeorc-0.1.7/nodeorc/log.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/nodeorc/main.py` & `nodeorc-0.1.7/nodeorc/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import click
 import json
 import os
 
-import nodeorc
+# import nodeorc
 from pydantic import ValidationError
 from dotenv import load_dotenv
 # import tasks
-# from nodeorc import settings_path, db, config
 
 # import nodeorc specifics
 from . import db, log, models, config, tasks, settings_path, __version__
 
 
 session = db.session
 # see if there is an active config, if not logger goes to $HOME/.nodeorc
@@ -165,79 +164,81 @@
 @click.pass_context
 def cli(ctx, info, license, debug):  # , quiet, verbose):
     """Command line interface for pyOpenRiverCam."""
     if ctx.obj is None:
         ctx.obj = {}
 
 @cli.command(short_help="Start main daemon")
-@storage_opt
-@listen_opt
-def start(storage, listen):
+# @storage_opt
+# @listen_opt
+def start():
     # get the device id
     logger.info(f"Device {str(device)} is online to run video analyses")
     # remote storage parameters with local processing is not possible
-    if listen == "local" and storage == "remote":
-        raise click.UsageError('Locally defined tasks ("--listen local")  cannot have remotely defined storage ('
-                              '"--storage remote").')
-    if listen == "local":
-        # get the stored configuration
-        active_config = config.get_active_config(parse=True)
-        if not(active_config):
-            raise click.UsageError('You do not yet have an active configuration. Upload an activate configuration '
-                                  'through the CLI. Type "nodeorc upload-config --help" for more information')
-
-        # initialize the database for storing data
-        session_data = db.init_basedata.get_data_session()
-        # read the task form from the configuration
-        task_form_template = config.get_active_task_form(session, parse=True)
-        callback_url = active_config.callback_url
-        if task_form_template is None:
-            # go into the task form get daemon and try to acquire a task form from server every 5 minutes
-            logger.info("Awaiting task by requesting a new task every 5 seconds")
-            tasks.wait_for_task_form(
-                session=session,
-                callback_url=callback_url,
-                device=device,
-                logger=logger,
-                reboot_after=active_config.settings.reboot_after
-            )
-        else:
-            # check for a new form with one single request
-            logger.info("Checking if a new task form is available for me...")
-            new_task_form_row = tasks.request_task_form(
-                session=session,
-                callback_url=callback_url,
-                device=device,
-                logger=logger
-            )
-            if new_task_form_row:
-                task_form_template = new_task_form_row.task_body
-        # verify that task_template can be converted to a valid Task
-        try:
-            task_test = models.Task(**task_form_template)
-        except Exception as e:
-            logger.error(
-                f"Task body set as active configuration cannot be formed into a valid Task instance. Reason: {str(e)}"
-            )
-            # This only happens with version upgrades. Update the status to BROKEN and report back to platform
-            task_form_template = config.get_active_task_form(session, parse=False)
-            task_form_template.status = db.models.TaskFormStatus.BROKEN
-            device.form_status = db.models.DeviceFormStatus.BROKEN_FORM
-            session.commit()
-        try:
-            processor = tasks.LocalTaskProcessor(
-                task_form_template=task_form_template,
-                logger=logger,
-                **active_config.model_dump()
-            )
-            processor.await_task()
-        except Exception as e:
-            logger.error("Reboot service: %s" % str(e))
+    # if listen == "local" and storage == "remote":
+    #     raise click.UsageError('Locally defined tasks ("--listen local")  cannot have remotely defined storage ('
+    #                           '"--storage remote").')
+    # if listen == "local":
+    # get the stored configuration
+    active_config = config.get_active_config(parse=True)
+    if not(active_config):
+        raise click.UsageError(
+            'You do not yet have an active configuration. Upload an activate configuration '
+            'through the CLI. Type "nodeorc upload-config --help" for more information'
+        )
+
+    # initialize the database for storing data
+    session_data = db.init_basedata.get_data_session()
+    # read the task form from the configuration
+    task_form_template = config.get_active_task_form(session, parse=True)
+    callback_url = active_config.callback_url
+    if task_form_template is None:
+        # go into the task form get daemon and try to acquire a task form from server every 5 minutes
+        logger.info("Awaiting task by requesting a new task every 5 seconds")
+        tasks.wait_for_task_form(
+            session=session,
+            callback_url=callback_url,
+            device=device,
+            logger=logger,
+            reboot_after=active_config.settings.reboot_after
+        )
     else:
-        raise NotImplementedError
+        # check for a new form with one single request
+        logger.info("Checking if a new task form is available for me...")
+        new_task_form_row = tasks.request_task_form(
+            session=session,
+            callback_url=callback_url,
+            device=device,
+            logger=logger
+        )
+        if new_task_form_row:
+            task_form_template = new_task_form_row.task_body
+    # verify that task_template can be converted to a valid Task
+    try:
+        task_test = models.Task(**task_form_template)
+    except Exception as e:
+        logger.error(
+            f"Task body set as active configuration cannot be formed into a valid Task instance. Reason: {str(e)}"
+        )
+        # This only happens with version upgrades. Update the status to BROKEN and report back to platform
+        task_form_template = config.get_active_task_form(session, parse=False)
+        task_form_template.status = db.models.TaskFormStatus.BROKEN
+        device.form_status = db.models.DeviceFormStatus.BROKEN_FORM
+        session.commit()
+    try:
+        processor = tasks.LocalTaskProcessor(
+            task_form_template=task_form_template,
+            logger=logger,
+            **active_config.model_dump()
+        )
+        processor.await_task()
+    except Exception as e:
+        logger.error("Reboot service: %s" % str(e))
+    # else:
+    #     raise NotImplementedError
 
 @cli.command(
     short_help="Upload a new configuration for this device from a JSON formatted file",
     epilog=get_docs_settings()
 )
 @click.argument(
     "JSON-file",
@@ -251,18 +252,17 @@
     default=True,
     help="Flag to define if uploaded configuration should be set as active (default: True)"
 )
 def upload_config(json_file, set_as_active):
     """Upload a new configuration for this device from a JSON formatted file"""
     logger.info(f"Device {str(device)} receiving new configuration from {json_file}")
     config = load_config(json_file)
-    rec = nodeorc.config.add_config(session, config=config, set_as_active=set_as_active)
+    rec = config.add_config(session, config=config, set_as_active=set_as_active)
     logger.info(f"Settings updated successfully to {rec}")
 
-upload_config.__doc__ = get_docs_settings()
 # def main():
 #     connection = pika.BlockingConnection(
 #         pika.URLParameters(
 #             '{}?heartbeat=1800&blocked_connection_timeout=900'.format(
 #                 os.getenv("AMQP_CONNECTION_STRING")
 #             )
 #         )
@@ -278,9 +278,12 @@
 #         channel.start_consuming()
 #     except Exception as e:
 #         logger.error("Reboot service: %s" % str(e))
 #         channel.stop_consuming()
 #         connection.close()
 #         traceback.print_tb(e.__traceback__)
 
+
+upload_config.__doc__ = get_docs_settings()
+
 if __name__ == "__main__":
     cli()
```

### Comparing `nodeorc-0.1.6/nodeorc/models/__init__.py` & `nodeorc-0.1.7/nodeorc/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,16 @@
         raise ValueError('{:s} does not contain a datetime format between {""} signs'.format(fn_fmt))
     datestr = datetime(2000, 1, 1, 1, 1, 1).strftime(fmt)
     dt = datetime.strptime(datestr, fmt)
     if dt.year != 2000 or dt.month != 1 or dt.day != 1:
         raise ValueError(f'Date format "{fmt}" is not a valid date format pattern')
     return True
 
-from .storage import Storage, S3Storage, File
+
+from .storage import Storage, S3Storage, File, get_storage
 from .callback_url import CallbackUrl
 from .callback import Callback
 from .subtask import Subtask
 from .task import Task
 from .config import LocalConfig, RemoteConfig, DiskManagement, Settings
 
+
```

### Comparing `nodeorc-0.1.6/nodeorc/models/callback.py` & `nodeorc-0.1.7/nodeorc/models/callback.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/nodeorc/models/callback_url.py` & `nodeorc-0.1.7/nodeorc/models/callback_url.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/nodeorc/models/config.py` & `nodeorc-0.1.7/nodeorc/models/config.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/nodeorc/models/storage.py` & `nodeorc-0.1.7/nodeorc/models/storage.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import shutil
 from typing import Optional, Dict, Any
 from pydantic import BaseModel, AnyHttpUrl
 # nodeodm specific imports
 
 from .. import callbacks, utils
 
+
 class Storage(BaseModel):
     url: str = "./tmp"
     bucket_name: str = "video"
-
+    options: Dict = {}
     @property
     def bucket(self):
         return os.path.join(self.url, self.bucket_name)
 
     @property
     def delete(self):
         shutil.rmtree(self.bucket)
@@ -56,56 +57,64 @@
         keep_src : bool
             if set, the file is copied, if not set, a rename will be performed instead.
 
         Returns
         -------
 
         """
+        dirname = os.path.dirname(trg)
+        if not os.path.isdir(dirname):
+            os.makedirs(dirname)
         if keep_src:
             shutil.copyfile(
                 os.path.join(self.bucket, src),
                 trg
             )
         else:
             os.rename(
                 os.path.join(self.bucket, src),
                 trg
             )
 
-class S3Storage(Storage):
+class S3Storage(BaseModel):
     url: AnyHttpUrl = "http://127.0.0.1:9000"
-    options: Dict[str, Any]
+    bucket_name: str = "video"
+    options: Dict[str, Any] = {}
 
 
     @property
     def bucket(self):
         return utils.get_bucket(
             url=str(self.url),
             bucket_name=self.bucket_name,
             **self.options
         )
 
     def upload_io(self, obj, dest, **kwargs):
         utils.upload_io(obj, self.bucket, dest=dest, **kwargs)
 
-    def download_file(self, src, trg):
+    def download_file(self, src, trg, keep_src=True):
         """
         Download file from bucket to specified target file (entire path inc. filename)
 
         Parameters
         ----------
         src : str
             file within bucket
 
         trg : file as it should be named locally
 
         Returns
         -------
 
         """
+        dirname = os.path.dirname(trg)
+        if not os.path.isdir(dirname):
+            os.makedirs(dirname)
+
         self.bucket.download_file(src, trg)
 
 
 
 class File(BaseModel):
     """
     Definition of the location, naming of raw result on tmp location, and in/output file name for cloud storage
@@ -128,7 +137,16 @@
         Returns
         -------
 
         """
         src_fn = os.path.join(src, self.tmp_name)
         trg_fn = os.path.join(trg, self.tmp_name)
         os.rename(src_fn, trg_fn)
+
+
+def get_storage(**data):
+    if data.get("url"):
+        if "://" in data["url"]:
+            return S3Storage(**data)
+        else:
+            return Storage(**data)
+
```

### Comparing `nodeorc-0.1.6/nodeorc/models/subtask.py` & `nodeorc-0.1.7/nodeorc/models/subtask.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/nodeorc/models/task.py` & `nodeorc-0.1.7/nodeorc/models/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import List, Optional, Dict, Union
 from pydantic import BaseModel, ConfigDict, model_validator, Field
 from urllib.parse import urljoin
 
 # nodeodm specific imports
 from . import CallbackUrl, Storage, S3Storage, File, Subtask, Callback, REMOVE_FOR_TEMPLATE
 
+
 class Task(BaseModel):
     """
     Definition of an entire task
     """
     id: uuid.UUID = Field(default_factory=uuid.uuid4)
     timestamp: datetime = datetime.now()
     callback_url: Optional[CallbackUrl] = None
@@ -39,17 +40,15 @@
 
         """
         # replace any inputs / outputs of subtasks (which may be mocks) with inputs / outputs defined in main task
         for subtask in self.subtasks:
             subtask.replace_files(self.input_files, self.output_files)
         return self
 
-
-
-    def execute(self, tmp):
+    def execute(self, tmp, keep_src=False):
         """
         Execute the entire task logic
 
         Parameters
         ----------
         tmp
 
@@ -60,15 +59,15 @@
         # prepare tmp location
         if not(os.path.isdir(tmp)):
             os.makedirs(tmp)
         # first download the input files
         try:
             self.logger.info(f"Performing task defined at {self.timestamp} with id {self.id}")
             self.logger.info(f"Downloading all inputs to {tmp}")
-            self.download_input(tmp)
+            self.download_input(tmp, keep_src=keep_src)
             # then perform all subtasks in order, upload occur within the subtasks
             self.logger.info(f"Executing subtasks")
             self.execute_subtasks(tmp, timestamp=self.timestamp)
             # r = self.callback_complete(msg=f"Task complete, id: {str(self.id)}")
             self.logger.info(f"Task id {str(self.id)} completed")
         except BaseException as e:
             # r = self.callback_error(msg=str(e))
@@ -81,28 +80,28 @@
 
         # report success or error
         # if r.status_code == 200:
         # else:
         #     self.logger.error(f"Task id {str(self.id)} failed with code {r.status_code} and message {r.json()}")
         #     raise Exception("Error detected, restarting node")
 
-    def download_input(self, tmp):
+    def download_input(self, tmp, keep_src=False):
         """
         Downloads all required inputs to a required temp path
 
         Parameters
         ----------
         tmp : str
             path to temporary local file store
 
         """
         for key, file in self.input_files.items():
             trg = os.path.join(tmp, file.tmp_name)
             # put the input file on tmp location
-            self.storage.download_file(file.remote_name, trg)
+            self.storage.download_file(file.remote_name, trg, keep_src=keep_src)
             # self.storage.bucket.download_file(file.remote_name, trg)
 
 
     def execute_subtasks(self, tmp, timestamp=None):
         """
 
         Parameters
```

### Comparing `nodeorc-0.1.6/nodeorc/tasks/local_task.py` & `nodeorc-0.1.7/nodeorc/tasks/local_task.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/nodeorc/tasks/task_form.py` & `nodeorc-0.1.7/nodeorc/tasks/task_form.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/nodeorc/utils.py` & `nodeorc-0.1.7/nodeorc/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import boto3
 import os
 import logging
 import time
 
+
 def check_bucket(s3, bucket_name):
     try:
         bucket = s3.Bucket(bucket_name)
         s3.meta.client.head_bucket(Bucket=bucket_name)
         return {
             "code": 200,
             "message": "Bucket is accessible"
@@ -24,22 +25,22 @@
         return {
             "code": error_code,
             "message": msg
         }
 
 def get_s3(
     endpoint_url,
-    aws_access_key_id,
-    aws_secret_access_key,
+    access_key,
+    secret_key,
 ):
     return boto3.resource(
         "s3",
         endpoint_url=endpoint_url,
-        aws_access_key_id=aws_access_key_id,
-        aws_secret_access_key=aws_secret_access_key,
+        aws_access_key_id=access_key,
+        aws_secret_access_key=secret_key,
         config=boto3.session.Config(signature_version="s3v4"),
         verify=False
     )
 
 
 def get_bucket(
     url,
```

### Comparing `nodeorc-0.1.6/pyproject.toml` & `nodeorc-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/service/usb-mount.sh` & `nodeorc-0.1.7/service/usb-mount.sh`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/settings/config_template.json` & `nodeorc-0.1.7/settings/config_template.json`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/setup.sh` & `nodeorc-0.1.7/setup.sh`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/tests/conftest.py` & `nodeorc-0.1.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/tests/examples/ngwerere_transect.nc` & `nodeorc-0.1.7/tests/examples/ngwerere_transect.nc`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/tests/test_callbacks.py` & `nodeorc-0.1.7/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/tests/test_config.py` & `nodeorc-0.1.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/tests/test_disk_management.py` & `nodeorc-0.1.7/tests/test_disk_management.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/tests/test_s3.py` & `nodeorc-0.1.7/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `nodeorc-0.1.6/PKG-INFO` & `nodeorc-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodeorc
-Version: 0.1.6
+Version: 0.1.7
 Summary: NodeORC: Automated edge and cloud image-based discharge estimation with OpenRiverCam
 Author-email: Hessel Winsemius <winsemius@rainbowsensing.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -564,25 +564,25 @@
         "reboot_after": 86400
 
     },
 
 
 .. _LiveORC: https://github.com/localdevices/LiveORC
 
-.. |pypi| image:: https://badge.fury.io/py/nodeopenrivercam.svg
+.. |pypi| image:: https://badge.fury.io/py/nodeorc.svg
     :alt: PyPI
-    :target: https://pypi.org/project/nodeopenrivercam/
+    :target: https://pypi.org/project/nodeorc/
 
-.. |piwheels| image:: https://img.shields.io/piwheels/v/:wheel
+.. |piwheels| image:: https://img.shields.io/piwheels/v/nodeorc
    :alt: PiWheels Version
    :target: https://localdevice.github.io/nodeorc/latest
 
 .. |docs_latest| image:: https://img.shields.io/badge/docs-latest-brightgreen.svg
     :alt: Latest documentation
-    :target: https://localdevice.github.io/nodeorc/latest
+    :target: https://github.com/localdevices/nodeorc
 
 
 .. |license| image:: https://img.shields.io/github/license/localdevices/nodeorc?style=flat
     :alt: License
     :target: https://github.com/localdevices/nodeorc/blob/main/LICENSE
```

