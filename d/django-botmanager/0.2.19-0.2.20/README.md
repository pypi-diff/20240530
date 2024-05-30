# Comparing `tmp/django_botmanager-0.2.19.tar.gz` & `tmp/django_botmanager-0.2.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_botmanager-0.2.19.tar", last modified: Tue May 28 12:41:02 2024, max compression
+gzip compressed data, was "django_botmanager-0.2.20.tar", last modified: Wed May 29 09:14:31 2024, max compression
```

## Comparing `django_botmanager-0.2.19.tar` & `django_botmanager-0.2.20.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-28 12:41:02.751727 django_botmanager-0.2.19/
--rw-rw-r--   0 titov     (1000) titov     (1000)     1479 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/LICENSE
--rw-rw-r--   0 titov     (1000) titov     (1000)       72 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/MANIFEST.in
--rw-r--r--   0 titov     (1000) titov     (1000)      320 2024-05-28 12:41:02.751727 django_botmanager-0.2.19/PKG-INFO
--rw-rw-r--   0 titov     (1000) titov     (1000)      562 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/README.md
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-28 12:41:02.747727 django_botmanager-0.2.19/botmanager/
--rw-rw-r--   0 titov     (1000) titov     (1000)       73 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/__init__.py
--rw-rw-r--   0 titov     (1000) titov     (1000)     2890 2024-05-28 12:39:53.000000 django_botmanager-0.2.19/botmanager/admin.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      135 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/apps.py
--rw-rw-r--   0 titov     (1000) titov     (1000)     7829 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/basetask.py
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-28 12:41:02.747727 django_botmanager-0.2.19/botmanager/management/
--rw-rw-r--   0 titov     (1000) titov     (1000)        0 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/management/__init__.py
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-28 12:41:02.747727 django_botmanager-0.2.19/botmanager/management/commands/
--rw-rw-r--   0 titov     (1000) titov     (1000)      542 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/management/commands/__init__.py
--rw-rw-r--   0 titov     (1000) titov     (1000)    18210 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/management/commands/bot_manager.py
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-28 12:41:02.747727 django_botmanager-0.2.19/botmanager/migrations/
--rw-rw-r--   0 titov     (1000) titov     (1000)     3357 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/migrations/0001_initial.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      742 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/migrations/0002_auto_20161208_1406.py
--rw-rw-r--   0 titov     (1000) titov     (1000)     1935 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/migrations/0003_auto_20161208_1529.py
--rw-rw-r--   0 titov     (1000) titov     (1000)     2880 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/migrations/0004_auto_20161219_1931.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      712 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/migrations/0005_task_parent.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      448 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/migrations/0006_task_priority.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      667 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/migrations/0007_task_is_persistent.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      673 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/migrations/0008_auto_20170331_1752.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      489 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/migrations/0009_task_extra_params.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      653 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/migrations/0010_auto_20170531_1321.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      706 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/migrations/0011_alter_task_create_dt_alter_task_id.py
--rw-rw-r--   0 titov     (1000) titov     (1000)        0 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/migrations/__init__.py
--rw-rw-r--   0 titov     (1000) titov     (1000)     3674 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/models.py
--rw-rw-r--   0 titov     (1000) titov     (1000)     3266 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/settings.py
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-28 12:41:02.743727 django_botmanager-0.2.19/botmanager/templates/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-28 12:41:02.743727 django_botmanager-0.2.19/botmanager/templates/botmanager/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-28 12:41:02.747727 django_botmanager-0.2.19/botmanager/templates/botmanager/task/
--rw-rw-r--   0 titov     (1000) titov     (1000)      277 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/templates/botmanager/task/change_form.html
--rw-rw-r--   0 titov     (1000) titov     (1000)     1105 2024-05-27 08:25:58.000000 django_botmanager-0.2.19/botmanager/utils.py
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-28 12:41:02.751727 django_botmanager-0.2.19/django_botmanager.egg-info/
--rw-r--r--   0 titov     (1000) titov     (1000)      320 2024-05-28 12:41:02.000000 django_botmanager-0.2.19/django_botmanager.egg-info/PKG-INFO
--rw-rw-r--   0 titov     (1000) titov     (1000)     1133 2024-05-28 12:41:02.000000 django_botmanager-0.2.19/django_botmanager.egg-info/SOURCES.txt
--rw-rw-r--   0 titov     (1000) titov     (1000)        1 2024-05-28 12:41:02.000000 django_botmanager-0.2.19/django_botmanager.egg-info/dependency_links.txt
--rw-rw-r--   0 titov     (1000) titov     (1000)       52 2024-05-28 12:41:02.000000 django_botmanager-0.2.19/django_botmanager.egg-info/requires.txt
--rw-rw-r--   0 titov     (1000) titov     (1000)       11 2024-05-28 12:41:02.000000 django_botmanager-0.2.19/django_botmanager.egg-info/top_level.txt
--rw-rw-r--   0 titov     (1000) titov     (1000)       38 2024-05-28 12:41:02.751727 django_botmanager-0.2.19/setup.cfg
--rw-rw-r--   0 titov     (1000) titov     (1000)      561 2024-05-28 12:39:47.000000 django_botmanager-0.2.19/setup.py
+drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-29 09:14:31.230723 django_botmanager-0.2.20/
+-rw-rw-r--   0 titov     (1000) titov     (1000)     1479 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/LICENSE
+-rw-rw-r--   0 titov     (1000) titov     (1000)       72 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/MANIFEST.in
+-rw-r--r--   0 titov     (1000) titov     (1000)      320 2024-05-29 09:14:31.230723 django_botmanager-0.2.20/PKG-INFO
+-rw-rw-r--   0 titov     (1000) titov     (1000)      562 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/README.md
+drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-29 09:14:31.226723 django_botmanager-0.2.20/botmanager/
+-rw-rw-r--   0 titov     (1000) titov     (1000)       73 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/__init__.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)     2972 2024-05-29 09:13:25.000000 django_botmanager-0.2.20/botmanager/admin.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)      135 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/apps.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)     7829 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/basetask.py
+drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-29 09:14:31.226723 django_botmanager-0.2.20/botmanager/management/
+-rw-rw-r--   0 titov     (1000) titov     (1000)        0 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/management/__init__.py
+drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-29 09:14:31.226723 django_botmanager-0.2.20/botmanager/management/commands/
+-rw-rw-r--   0 titov     (1000) titov     (1000)      542 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/management/commands/__init__.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)    18210 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/management/commands/bot_manager.py
+drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-29 09:14:31.230723 django_botmanager-0.2.20/botmanager/migrations/
+-rw-rw-r--   0 titov     (1000) titov     (1000)     3357 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/migrations/0001_initial.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)      742 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/migrations/0002_auto_20161208_1406.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)     1935 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/migrations/0003_auto_20161208_1529.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)     2880 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/migrations/0004_auto_20161219_1931.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)      712 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/migrations/0005_task_parent.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)      448 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/migrations/0006_task_priority.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)      667 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/migrations/0007_task_is_persistent.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)      673 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/migrations/0008_auto_20170331_1752.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)      489 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/migrations/0009_task_extra_params.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)      653 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/migrations/0010_auto_20170531_1321.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)      706 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/migrations/0011_alter_task_create_dt_alter_task_id.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)        0 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/migrations/__init__.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)     3674 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/models.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)     3266 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/settings.py
+drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-29 09:14:31.222723 django_botmanager-0.2.20/botmanager/templates/
+drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-29 09:14:31.222723 django_botmanager-0.2.20/botmanager/templates/botmanager/
+drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-29 09:14:31.230723 django_botmanager-0.2.20/botmanager/templates/botmanager/task/
+-rw-rw-r--   0 titov     (1000) titov     (1000)      277 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/templates/botmanager/task/change_form.html
+-rw-rw-r--   0 titov     (1000) titov     (1000)     1105 2024-05-27 08:25:58.000000 django_botmanager-0.2.20/botmanager/utils.py
+drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-29 09:14:31.230723 django_botmanager-0.2.20/django_botmanager.egg-info/
+-rw-r--r--   0 titov     (1000) titov     (1000)      320 2024-05-29 09:14:31.000000 django_botmanager-0.2.20/django_botmanager.egg-info/PKG-INFO
+-rw-rw-r--   0 titov     (1000) titov     (1000)     1133 2024-05-29 09:14:31.000000 django_botmanager-0.2.20/django_botmanager.egg-info/SOURCES.txt
+-rw-rw-r--   0 titov     (1000) titov     (1000)        1 2024-05-29 09:14:31.000000 django_botmanager-0.2.20/django_botmanager.egg-info/dependency_links.txt
+-rw-rw-r--   0 titov     (1000) titov     (1000)       52 2024-05-29 09:14:31.000000 django_botmanager-0.2.20/django_botmanager.egg-info/requires.txt
+-rw-rw-r--   0 titov     (1000) titov     (1000)       11 2024-05-29 09:14:31.000000 django_botmanager-0.2.20/django_botmanager.egg-info/top_level.txt
+-rw-rw-r--   0 titov     (1000) titov     (1000)       38 2024-05-29 09:14:31.230723 django_botmanager-0.2.20/setup.cfg
+-rw-rw-r--   0 titov     (1000) titov     (1000)      561 2024-05-29 09:13:20.000000 django_botmanager-0.2.20/setup.py
```

### Comparing `django_botmanager-0.2.19/LICENSE` & `django_botmanager-0.2.20/LICENSE`

 * *Files identical despite different names*

### Comparing `django_botmanager-0.2.19/README.md` & `django_botmanager-0.2.20/README.md`

 * *Files identical despite different names*

### Comparing `django_botmanager-0.2.19/botmanager/admin.py` & `django_botmanager-0.2.20/botmanager/admin.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,16 +61,17 @@
             if Command.import_from_string(i).name == task.name
         ]
 
         if not imported_class:
             return HttpResponseNotFound()
 
         filename = imported_class[0](task).get_log_file_name()
+        folder = imported_class[0].name if imported_class[0].name else ''
         dir = settings.MAIN_CONFIG["logs"]["dir"]
-        file_path = os.path.join(dir, filename) + ".log"
+        file_path = os.path.join(dir, folder, filename) + ".log"
 
         if os.path.exists(file_path):
             return FileResponse(open(file_path, "rb"))
         else:
             return HttpResponseNotFound()
 
     open_logfile.short_description = _(u"Открыть файл")
```

### Comparing `django_botmanager-0.2.19/botmanager/basetask.py` & `django_botmanager-0.2.20/botmanager/basetask.py`

 * *Files identical despite different names*

### Comparing `django_botmanager-0.2.19/botmanager/management/commands/__init__.py` & `django_botmanager-0.2.20/botmanager/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django_botmanager-0.2.19/botmanager/management/commands/bot_manager.py` & `django_botmanager-0.2.20/botmanager/management/commands/bot_manager.py`

 * *Files identical despite different names*

### Comparing `django_botmanager-0.2.19/botmanager/migrations/0001_initial.py` & `django_botmanager-0.2.20/botmanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_botmanager-0.2.19/botmanager/migrations/0002_auto_20161208_1406.py` & `django_botmanager-0.2.20/botmanager/migrations/0002_auto_20161208_1406.py`

 * *Files identical despite different names*

### Comparing `django_botmanager-0.2.19/botmanager/migrations/0003_auto_20161208_1529.py` & `django_botmanager-0.2.20/botmanager/migrations/0003_auto_20161208_1529.py`

 * *Files identical despite different names*

### Comparing `django_botmanager-0.2.19/botmanager/migrations/0004_auto_20161219_1931.py` & `django_botmanager-0.2.20/botmanager/migrations/0004_auto_20161219_1931.py`

 * *Files identical despite different names*

### Comparing `django_botmanager-0.2.19/botmanager/migrations/0005_task_parent.py` & `django_botmanager-0.2.20/botmanager/migrations/0005_task_parent.py`

 * *Files identical despite different names*

### Comparing `django_botmanager-0.2.19/botmanager/migrations/0007_task_is_persistent.py` & `django_botmanager-0.2.20/botmanager/migrations/0007_task_is_persistent.py`

 * *Files identical despite different names*

### Comparing `django_botmanager-0.2.19/botmanager/migrations/0008_auto_20170331_1752.py` & `django_botmanager-0.2.20/botmanager/migrations/0008_auto_20170331_1752.py`

 * *Files identical despite different names*

### Comparing `django_botmanager-0.2.19/botmanager/migrations/0010_auto_20170531_1321.py` & `django_botmanager-0.2.20/botmanager/migrations/0010_auto_20170531_1321.py`

 * *Files identical despite different names*

### Comparing `django_botmanager-0.2.19/botmanager/migrations/0011_alter_task_create_dt_alter_task_id.py` & `django_botmanager-0.2.20/botmanager/migrations/0011_alter_task_create_dt_alter_task_id.py`

 * *Files identical despite different names*

### Comparing `django_botmanager-0.2.19/botmanager/models.py` & `django_botmanager-0.2.20/botmanager/models.py`

 * *Files identical despite different names*

### Comparing `django_botmanager-0.2.19/botmanager/settings.py` & `django_botmanager-0.2.20/botmanager/settings.py`

 * *Files identical despite different names*

### Comparing `django_botmanager-0.2.19/botmanager/utils.py` & `django_botmanager-0.2.20/botmanager/utils.py`

 * *Files identical despite different names*

### Comparing `django_botmanager-0.2.19/django_botmanager.egg-info/SOURCES.txt` & `django_botmanager-0.2.20/django_botmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_botmanager-0.2.19/setup.py` & `django_botmanager-0.2.20/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 setup(
     name='django-botmanager',
-    version='0.2.19',
+    version='0.2.20',
     description='Async tasks for django',
     author='Dimoha',
     author_email='dimoha@controlstyle.ru',
     url='https://github.com/dimoha/django-botmanager',
     install_requires=[
         "setproctitle==1.1.10",
         "jsonfield==3.1.0",
```

