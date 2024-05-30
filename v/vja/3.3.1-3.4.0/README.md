# Comparing `tmp/vja-3.3.1.tar.gz` & `tmp/vja-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vja-3.3.1.tar", last modified: Tue Mar 26 18:26:41 2024, max compression
+gzip compressed data, was "vja-3.4.0.tar", last modified: Thu May 30 10:36:04 2024, max compression
```

## Comparing `vja-3.3.1.tar` & `vja-3.4.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:26:41.751854 vja-3.3.1/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2024-03-26 18:25:48.000000 vja-3.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7775 2024-03-26 18:26:41.751854 vja-3.3.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     7129 2024-03-26 18:25:48.000000 vja-3.3.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)       66 2024-03-26 18:26:41.751854 vja-3.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      965 2024-03-26 18:25:48.000000 vja-3.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:26:41.745854 vja-3.3.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 18:25:48.000000 vja-3.3.1/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2021 2024-03-26 18:25:48.000000 vja-3.3.1/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2943 2024-03-26 18:25:48.000000 vja-3.3.1/tests/test_basic.py
--rw-rw-rw-   0 root         (0) root         (0)    11681 2024-03-26 18:25:48.000000 vja-3.3.1/tests/test_command.py
--rw-rw-rw-   0 root         (0) root         (0)    10467 2024-03-26 18:25:48.000000 vja-3.3.1/tests/test_query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:26:41.749854 vja-3.3.1/vja/
--rwxrwxrwx   0 root         (0) root         (0)      220 2024-03-26 18:25:48.000000 vja-3.3.1/vja/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6824 2024-03-26 18:25:48.000000 vja-3.3.1/vja/apiclient.py
--rw-rw-rw-   0 root         (0) root         (0)     2777 2024-03-26 18:25:48.000000 vja-3.3.1/vja/authenticate.py
--rwxrwxrwx   0 root         (0) root         (0)    22952 2024-03-26 18:25:48.000000 vja-3.3.1/vja/cli.py
--rwxrwxrwx   0 root         (0) root         (0)     1967 2024-03-26 18:25:48.000000 vja-3.3.1/vja/config.py
--rw-rw-rw-   0 root         (0) root         (0)     4033 2024-03-26 18:25:48.000000 vja-3.3.1/vja/filter.py
--rwxrwxrwx   0 root         (0) root         (0)     5780 2024-03-26 18:25:48.000000 vja-3.3.1/vja/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2997 2024-03-26 18:25:48.000000 vja-3.3.1/vja/output.py
--rw-rw-rw-   0 root         (0) root         (0)     2709 2024-03-26 18:25:48.000000 vja-3.3.1/vja/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     2838 2024-03-26 18:25:48.000000 vja-3.3.1/vja/project_service.py
--rw-rw-rw-   0 root         (0) root         (0)    11983 2024-03-26 18:25:48.000000 vja-3.3.1/vja/service_command.py
--rw-rw-rw-   0 root         (0) root         (0)     2804 2024-03-26 18:25:48.000000 vja-3.3.1/vja/service_query.py
--rw-rw-rw-   0 root         (0) root         (0)      690 2024-03-26 18:25:48.000000 vja-3.3.1/vja/task_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2886 2024-03-26 18:25:48.000000 vja-3.3.1/vja/urgency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:26:41.751854 vja-3.3.1/vja.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7775 2024-03-26 18:26:41.000000 vja-3.3.1/vja.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      532 2024-03-26 18:26:41.000000 vja-3.3.1/vja.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 18:26:41.000000 vja-3.3.1/vja.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       36 2024-03-26 18:26:41.000000 vja-3.3.1/vja.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       83 2024-03-26 18:26:41.000000 vja-3.3.1/vja.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-03-26 18:26:41.000000 vja-3.3.1/vja.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:36:04.320160 vja-3.4.0/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2024-05-30 10:34:50.000000 vja-3.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7775 2024-05-30 10:36:04.320160 vja-3.4.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     7129 2024-05-30 10:34:50.000000 vja-3.4.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       66 2024-05-30 10:36:04.320160 vja-3.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      965 2024-05-30 10:34:50.000000 vja-3.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:36:04.313160 vja-3.4.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-30 10:34:50.000000 vja-3.4.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2021 2024-05-30 10:34:50.000000 vja-3.4.0/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2943 2024-05-30 10:34:50.000000 vja-3.4.0/tests/test_basic.py
+-rw-rw-rw-   0 root         (0) root         (0)    11949 2024-05-30 10:34:50.000000 vja-3.4.0/tests/test_command.py
+-rw-rw-rw-   0 root         (0) root         (0)    10467 2024-05-30 10:34:50.000000 vja-3.4.0/tests/test_query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:36:04.317160 vja-3.4.0/vja/
+-rwxrwxrwx   0 root         (0) root         (0)      220 2024-05-30 10:34:50.000000 vja-3.4.0/vja/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6824 2024-05-30 10:34:50.000000 vja-3.4.0/vja/apiclient.py
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2024-05-30 10:34:50.000000 vja-3.4.0/vja/authenticate.py
+-rwxrwxrwx   0 root         (0) root         (0)    23064 2024-05-30 10:34:50.000000 vja-3.4.0/vja/cli.py
+-rwxrwxrwx   0 root         (0) root         (0)     1967 2024-05-30 10:34:50.000000 vja-3.4.0/vja/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     4033 2024-05-30 10:34:50.000000 vja-3.4.0/vja/filter.py
+-rwxrwxrwx   0 root         (0) root         (0)     5780 2024-05-30 10:34:50.000000 vja-3.4.0/vja/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2997 2024-05-30 10:34:50.000000 vja-3.4.0/vja/output.py
+-rw-rw-rw-   0 root         (0) root         (0)     2872 2024-05-30 10:34:50.000000 vja-3.4.0/vja/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2838 2024-05-30 10:34:50.000000 vja-3.4.0/vja/project_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    11983 2024-05-30 10:34:50.000000 vja-3.4.0/vja/service_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     2804 2024-05-30 10:34:50.000000 vja-3.4.0/vja/service_query.py
+-rw-rw-rw-   0 root         (0) root         (0)      690 2024-05-30 10:34:50.000000 vja-3.4.0/vja/task_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2886 2024-05-30 10:34:50.000000 vja-3.4.0/vja/urgency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:36:04.319160 vja-3.4.0/vja.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7775 2024-05-30 10:36:04.000000 vja-3.4.0/vja.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      532 2024-05-30 10:36:04.000000 vja-3.4.0/vja.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 10:36:04.000000 vja-3.4.0/vja.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2024-05-30 10:36:04.000000 vja-3.4.0/vja.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2024-05-30 10:36:04.000000 vja-3.4.0/vja.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-30 10:36:04.000000 vja-3.4.0/vja.egg-info/top_level.txt
```

### Comparing `vja-3.3.1/LICENSE` & `vja-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vja-3.3.1/PKG-INFO` & `vja-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vja
-Version: 3.3.1
+Version: 3.4.0
 Summary: A simple CLI for Vikunja task manager
 Home-page: https://gitlab.com/ce72/vja
 Author: ce72
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `vja-3.3.1/README.md` & `vja-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `vja-3.3.1/setup.py` & `vja-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `vja-3.3.1/tests/conftest.py` & `vja-3.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vja-3.3.1/tests/test_basic.py` & `vja-3.4.0/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `vja-3.3.1/tests/test_command.py` & `vja-3.4.0/tests/test_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ADD_SUCCESS_PATTERN = re.compile(r'.*Created task (\d+) in project .*')
 TODAY = datetime.datetime.now().replace(microsecond=0)
 TODAY_ISO = TODAY.isoformat()
 YESTERDAY = TODAY + datetime.timedelta(days=-1)
 YESTERDAY_ISO = YESTERDAY.isoformat()
 TOMORROW = TODAY + datetime.timedelta(days=1)
 TOMORROW_ISO = TOMORROW.isoformat()
+TOMMORROW_AT_8_ISO = (TOMORROW.replace(hour=8, minute=0, second=0)).isoformat()
 DATE_1 = TODAY + datetime.timedelta(days=10)
 DATE_2 = DATE_1 + datetime.timedelta(days=1)
 DATE_1_ISO = DATE_1.isoformat()
 DATE_2_ISO = DATE_2.isoformat()
 
 
 class TestAddTask:
@@ -24,14 +25,19 @@
         assert after['project']['id'] == 1
 
     def test_project_title(self, runner):
         res = invoke(runner, 'add title of new task --force --project=test-project')
         after = json_for_created_task(runner, res.output)
         assert after['project']['title'] == 'test-project'
 
+    def test_due_date(self, runner):
+        res = invoke(runner, 'add title of new task --force --due=tomorrow')
+        after = json_for_created_task(runner, res.output)
+        assert after['due_date'] == TOMMORROW_AT_8_ISO
+
     def test_duplicate_task_title_rejected(self, runner):
         invoke(runner, 'add title of new task', 1, catch_exceptions=True)
 
     def test_default_reminder_uses_due(self, runner):
         res = invoke(runner, 'add title of new task --force --project=test-project --due=today --reminder')
         after = json_for_created_task(runner, res.output)
         assert after['reminders'][0]['relative_period'] == 0
@@ -89,15 +95,15 @@
         assert after['project']['id'] == before['project']['id']
         assert after['created'] == before['created']
 
     def test_edit_due_date_without_time(self, runner):
         invoke(runner, 'edit 1 --due=tomorrow')
 
         after = json_for_task_id(runner, 1)
-        assert after['due_date'] == (TOMORROW.replace(hour=0, minute=0, second=0)).isoformat()
+        assert after['due_date'] == TOMMORROW_AT_8_ISO
 
     def test_edit_due_date_with_time(self, runner):
         invoke(runner, ['edit', '1', '--due=tomorrow 15:00'])
 
         after = json_for_task_id(runner, 1)
         assert after['due_date'] == (TOMORROW.replace(hour=15, minute=0, second=0)).isoformat()
```

### Comparing `vja-3.3.1/tests/test_query.py` & `vja-3.4.0/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `vja-3.3.1/vja/apiclient.py` & `vja-3.4.0/vja/apiclient.py`

 * *Files identical despite different names*

### Comparing `vja-3.3.1/vja/authenticate.py` & `vja-3.4.0/vja/authenticate.py`

 * *Files identical despite different names*

### Comparing `vja-3.3.1/vja/cli.py` & `vja-3.4.0/vja/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,30 +81,30 @@
     if username:
         application.command_service.login(username, password, totp_passcode)
 
 
 # user
 @cli.group('user', help='Subcommand: user (see help)')
 def user_group():
-    pass
+    pass  # group user operations
 
 
 @user_group.command('show', help='Print current user')
 @click.option('is_json', '--json', default=False, is_flag=True, help='Print as Vikunja json')
 @click.option('is_jsonvja', '--jsonvja', default=False, is_flag=True, help='Print as vja application json')
 @with_application
 def user_show(application, is_json=False, is_jsonvja=False):
     application.output.user(
         application.query_service.find_current_user(), is_json, is_jsonvja)
 
 
 # projects
 @cli.group('project', help='Subcommand: project (see help)', aliases=['projects'])
 def project_group():
-    pass
+    pass  # group project operations
 
 
 @project_group.command('add', help='Add project with title')
 @click.option('parent_project', '-o', '--parent-project', '--parent_project',
               help='Create project as child of parent project. May be given by id or title of parent-project.')
 @click.argument('title', nargs=-1, required=True)
 @with_application
@@ -146,15 +146,15 @@
 def project_open(application, project_id):
     application.open_browser_project(project_id)
 
 
 # buckets
 @cli.group('bucket', help='Subcommand: kanban buckets (see help)', aliases=['buckets'])
 def bucket_group():
-    pass
+    pass  # group bucket operations
 
 
 @bucket_group.command('add', help='Add bucket with title')
 @click.option('project', '-o', '--project', '--project-id',
               help='Create bucket in given project.')
 @click.argument('title', nargs=-1, required=True)
 @with_application
@@ -179,15 +179,15 @@
     application.output.bucket_array(
         application.query_service.find_all_buckets_in_project(project_id), is_json, is_jsonvja, custom_format)
 
 
 # labels
 @cli.group('label', help='Subcommand: label (see help)', aliases=['labels'])
 def label_group():
-    pass
+    pass  # group label operations
 
 
 @label_group.command('ls', help='Print labels ... (id; title)')
 @click.option('is_json', '--json', default=False, is_flag=True,
               help='Print as Vikunja json')
 @click.option('is_jsonvja', '--jsonvja', default=False, is_flag=True,
               help='Print as vja application json')
@@ -434,15 +434,15 @@
 
     tasks = application.query_service.find_filtered_tasks(include_completed, sort_string, filter_args)
     if task_ids:
         tasks = [t for t in tasks if t.id in task_ids]
 
     application.output.task_array(tasks, is_json, is_jsonvja, custom_format)
     if not is_json and not is_jsonvja and not custom_format:
-        click.echo(f"Count: {len(tasks)}")
+        click.echo(f"Count: {len(list(tasks))}")
 
 
 @cli.command('show', help='Show task details. Multiple task ids may be given')
 @click.argument('tasks', type=click.INT, nargs=-1)
 @click.option('is_json', '--json', default=False, is_flag=True,
               help='Print as Vikunja json')
 @click.option('is_jsonvja', '--jsonvja', default=False, is_flag=True,
```

### Comparing `vja-3.3.1/vja/config.py` & `vja-3.4.0/vja/config.py`

 * *Files identical despite different names*

### Comparing `vja-3.3.1/vja/filter.py` & `vja-3.4.0/vja/filter.py`

 * *Files identical despite different names*

### Comparing `vja-3.3.1/vja/model.py` & `vja-3.4.0/vja/model.py`

 * *Files identical despite different names*

### Comparing `vja-3.3.1/vja/output.py` & `vja-3.4.0/vja/output.py`

 * *Files identical despite different names*

### Comparing `vja-3.3.1/vja/parse.py` & `vja-3.4.0/vja/parse.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 from datetime import datetime, timedelta
 from typing import Optional
 
 import dateutil.parser
 from dateutil import tz
 from parsedatetime import parsedatetime
 
+# if dates are given like 'tomorrow' or 'next mon' then this will be used as time
+DEFAULT_DATE_HOUR = 8
+DEFAULT_DATE_MINUTE = 0
+
 _timedelta_regex = re.compile(r'^((?P<weeks>[.\d]+?)w)? *'
                               r'^((?P<days>[.\d]+?)d)? *'
                               r'((?P<hours>[.\d]+?)h)? *'
                               r'((?P<minutes>[.\d]+?)m)? *'
                               r'((?P<seconds>[.\d]+?)s?)?$')
 
 
@@ -20,15 +24,15 @@
         return None
     try:
         return dateutil.parser.isoparse(text)
     except ValueError:
         timetuple, pdt_context = parsedatetime.Calendar(version=parsedatetime.VERSION_CONTEXT_STYLE).parse(text)
         datetime_date = datetime.fromtimestamp(time.mktime(timetuple))
         if not pdt_context.hasTime:
-            datetime_date = datetime_date.replace(hour=0, minute=0, second=0)
+            datetime_date = datetime_date.replace(hour=DEFAULT_DATE_HOUR, minute=DEFAULT_DATE_MINUTE, second=0)
         return datetime_date
 
 
 def parse_date_arg_to_iso(text: str) -> Optional[str]:
     date_value = parse_date_arg_to_datetime(text)
     return datetime_to_isoformat(date_value) if date_value else None
```

### Comparing `vja-3.3.1/vja/project_service.py` & `vja-3.4.0/vja/project_service.py`

 * *Files identical despite different names*

### Comparing `vja-3.3.1/vja/service_command.py` & `vja-3.4.0/vja/service_command.py`

 * *Files identical despite different names*

### Comparing `vja-3.3.1/vja/service_query.py` & `vja-3.4.0/vja/service_query.py`

 * *Files identical despite different names*

### Comparing `vja-3.3.1/vja/task_service.py` & `vja-3.4.0/vja/task_service.py`

 * *Files identical despite different names*

### Comparing `vja-3.3.1/vja/urgency.py` & `vja-3.4.0/vja/urgency.py`

 * *Files identical despite different names*

### Comparing `vja-3.3.1/vja.egg-info/PKG-INFO` & `vja-3.4.0/vja.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vja
-Version: 3.3.1
+Version: 3.4.0
 Summary: A simple CLI for Vikunja task manager
 Home-page: https://gitlab.com/ce72/vja
 Author: ce72
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `vja-3.3.1/vja.egg-info/SOURCES.txt` & `vja-3.4.0/vja.egg-info/SOURCES.txt`

 * *Files identical despite different names*

