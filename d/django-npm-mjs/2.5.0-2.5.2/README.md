# Comparing `tmp/django-npm-mjs-2.5.0.tar.gz` & `tmp/django_npm_mjs-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-npm-mjs-2.5.0.tar", last modified: Sun Nov  5 17:03:53 2023, max compression
+gzip compressed data, was "django_npm_mjs-2.5.2.tar", last modified: Thu May 30 18:32:55 2024, max compression
```

## Comparing `django-npm-mjs-2.5.0.tar` & `django_npm_mjs-2.5.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-11-05 17:03:53.051121 django-npm-mjs-2.5.0/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     7651 2019-05-03 23:44:54.000000 django-npm-mjs-2.5.0/LICENSE
--rw-r--r--   0 johannes  (1000) johannes  (1000)      205 2023-01-04 22:37:55.000000 django-npm-mjs-2.5.0/MANIFEST.in
--rw-r--r--   0 johannes  (1000) johannes  (1000)     5750 2023-11-05 17:03:53.051121 django-npm-mjs-2.5.0/PKG-INFO
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4578 2023-11-05 16:12:44.000000 django-npm-mjs-2.5.0/README.md
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-11-05 17:03:53.043121 django-npm-mjs-2.5.0/django_npm_mjs.egg-info/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     5750 2023-11-05 17:03:53.000000 django-npm-mjs-2.5.0/django_npm_mjs.egg-info/PKG-INFO
--rw-r--r--   0 johannes  (1000) johannes  (1000)      768 2023-11-05 17:03:53.000000 django-npm-mjs-2.5.0/django_npm_mjs.egg-info/SOURCES.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)        1 2023-11-05 17:03:53.000000 django-npm-mjs-2.5.0/django_npm_mjs.egg-info/dependency_links.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)       27 2023-11-05 17:03:53.000000 django-npm-mjs-2.5.0/django_npm_mjs.egg-info/requires.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)        8 2023-11-05 17:03:53.000000 django-npm-mjs-2.5.0/django_npm_mjs.egg-info/top_level.txt
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-11-05 17:03:53.047121 django-npm-mjs-2.5.0/npm_mjs/
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-07-21 17:17:29.000000 django-npm-mjs-2.5.0/npm_mjs/__init__.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-11-05 17:03:53.047121 django-npm-mjs-2.5.0/npm_mjs/management/
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-05-03 23:44:54.000000 django-npm-mjs-2.5.0/npm_mjs/management/__init__.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-11-05 17:03:53.047121 django-npm-mjs-2.5.0/npm_mjs/management/commands/
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-05-03 23:44:54.000000 django-npm-mjs-2.5.0/npm_mjs/management/commands/__init__.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)      439 2022-10-17 19:29:25.000000 django-npm-mjs-2.5.0/npm_mjs/management/commands/collectstatic.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2050 2023-11-05 16:20:33.000000 django-npm-mjs-2.5.0/npm_mjs/management/commands/create_package_json.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3945 2023-03-12 06:21:18.000000 django-npm-mjs-2.5.0/npm_mjs/management/commands/makemessages.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3174 2023-11-05 10:56:10.000000 django-npm-mjs-2.5.0/npm_mjs/management/commands/npm_install.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    10561 2022-10-17 19:32:04.000000 django-npm-mjs-2.5.0/npm_mjs/management/commands/transpile.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1399 2023-11-05 15:28:10.000000 django-npm-mjs-2.5.0/npm_mjs/management/commands/webpack.config.template.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      419 2022-10-17 19:33:30.000000 django-npm-mjs-2.5.0/npm_mjs/paths.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)       90 2019-05-03 23:44:54.000000 django-npm-mjs-2.5.0/npm_mjs/signals.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3264 2022-10-17 19:27:57.000000 django-npm-mjs-2.5.0/npm_mjs/storage.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-11-05 17:03:53.047121 django-npm-mjs-2.5.0/npm_mjs/templatetags/
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-05-03 23:44:54.000000 django-npm-mjs-2.5.0/npm_mjs/templatetags/__init__.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1664 2022-10-17 19:28:58.000000 django-npm-mjs-2.5.0/npm_mjs/templatetags/transpile.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      663 2022-10-17 19:27:57.000000 django-npm-mjs-2.5.0/npm_mjs/tools.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1210 2023-11-05 17:02:19.000000 django-npm-mjs-2.5.0/pyproject.toml
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       31 2023-11-05 12:18:57.000000 django-npm-mjs-2.5.0/requirements.txt
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       38 2023-11-05 17:03:53.051121 django-npm-mjs-2.5.0/setup.cfg
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      252 2023-01-04 22:55:55.000000 django-npm-mjs-2.5.0/setup.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2024-05-30 18:32:55.429929 django_npm_mjs-2.5.2/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     7651 2019-05-03 23:44:54.000000 django_npm_mjs-2.5.2/LICENSE
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      206 2024-05-30 17:33:34.000000 django_npm_mjs-2.5.2/MANIFEST.in
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     5879 2024-05-30 18:32:55.429929 django_npm_mjs-2.5.2/PKG-INFO
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4578 2023-11-05 16:12:44.000000 django_npm_mjs-2.5.2/README.md
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2024-05-30 18:32:55.429929 django_npm_mjs-2.5.2/django_npm_mjs.egg-info/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     5879 2024-05-30 18:32:55.000000 django_npm_mjs-2.5.2/django_npm_mjs.egg-info/PKG-INFO
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      790 2024-05-30 18:32:55.000000 django_npm_mjs-2.5.2/django_npm_mjs.egg-info/SOURCES.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        1 2024-05-30 18:32:55.000000 django_npm_mjs-2.5.2/django_npm_mjs.egg-info/dependency_links.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       27 2024-05-30 18:32:55.000000 django_npm_mjs-2.5.2/django_npm_mjs.egg-info/requires.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        8 2024-05-30 18:32:55.000000 django_npm_mjs-2.5.2/django_npm_mjs.egg-info/top_level.txt
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2024-05-30 18:32:55.425928 django_npm_mjs-2.5.2/npm_mjs/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-07-21 17:17:29.000000 django_npm_mjs-2.5.2/npm_mjs/__init__.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2024-05-30 18:32:55.425928 django_npm_mjs-2.5.2/npm_mjs/management/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-05-03 23:44:54.000000 django_npm_mjs-2.5.2/npm_mjs/management/__init__.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2024-05-30 18:32:55.429929 django_npm_mjs-2.5.2/npm_mjs/management/commands/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-05-03 23:44:54.000000 django_npm_mjs-2.5.2/npm_mjs/management/commands/__init__.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      439 2022-10-17 19:29:25.000000 django_npm_mjs-2.5.2/npm_mjs/management/commands/collectstatic.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2050 2024-05-30 17:33:19.000000 django_npm_mjs-2.5.2/npm_mjs/management/commands/create_package_json.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3945 2023-03-12 06:21:18.000000 django_npm_mjs-2.5.2/npm_mjs/management/commands/makemessages.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3174 2023-11-05 10:56:10.000000 django_npm_mjs-2.5.2/npm_mjs/management/commands/npm_install.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    10561 2022-10-17 19:32:04.000000 django_npm_mjs-2.5.2/npm_mjs/management/commands/transpile.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1399 2023-11-05 15:28:10.000000 django_npm_mjs-2.5.2/npm_mjs/management/commands/webpack.config.template.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      652 2024-05-30 17:38:30.000000 django_npm_mjs-2.5.2/npm_mjs/package.json5
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      419 2022-10-17 19:33:30.000000 django_npm_mjs-2.5.2/npm_mjs/paths.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       90 2019-05-03 23:44:54.000000 django_npm_mjs-2.5.2/npm_mjs/signals.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3264 2022-10-17 19:27:57.000000 django_npm_mjs-2.5.2/npm_mjs/storage.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2024-05-30 18:32:55.429929 django_npm_mjs-2.5.2/npm_mjs/templatetags/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-05-03 23:44:54.000000 django_npm_mjs-2.5.2/npm_mjs/templatetags/__init__.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1664 2022-10-17 19:28:58.000000 django_npm_mjs-2.5.2/npm_mjs/templatetags/transpile.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      663 2022-10-17 19:27:57.000000 django_npm_mjs-2.5.2/npm_mjs/tools.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1318 2024-05-30 18:32:32.000000 django_npm_mjs-2.5.2/pyproject.toml
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       31 2024-05-30 17:34:52.000000 django_npm_mjs-2.5.2/requirements.txt
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       38 2024-05-30 18:32:55.429929 django_npm_mjs-2.5.2/setup.cfg
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      252 2023-01-04 22:55:55.000000 django_npm_mjs-2.5.2/setup.py
```

### Comparing `django-npm-mjs-2.5.0/LICENSE` & `django_npm_mjs-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-npm-mjs-2.5.0/PKG-INFO` & `django_npm_mjs-2.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: django-npm-mjs
-Version: 2.5.0
+Version: 2.5.2
 Summary: A Django package to use npm.js dependencies and transpile ES2015+
 Author-email: Johannes Wilm <johannes@fiduswriter.org>
 License: LGPL-3.0-or-later
 Project-URL: repository, https://github.com/fiduswriter/django-npm-mjs
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=3.2
-Requires-Dist: pyjson5==1.6.4
+Requires-Dist: pyjson5==1.6.6
 
 # django-npm-mjs
 A Django package to use npm.js dependencies and transpile ES2015+
 
 This package is used by Fidus Writer to bundle JavaScript. We try to keep it as generic as possible, so if there is something that seems very odd and specific to Fidus Writer, it is likely just an oversight from us. Please contact us and we'll see what we can do about it.
 
 This package similar to django-compressor in that it treats JavaScript files before they are served to the user. But there are some differences:
```

#### html2text {}

```diff
@@ -1,56 +1,58 @@
-Metadata-Version: 2.1 Name: django-npm-mjs Version: 2.5.0 Summary: A Django
+Metadata-Version: 2.1 Name: django-npm-mjs Version: 2.5.2 Summary: A Django
 package to use npm.js dependencies and transpile ES2015+ Author-email: Johannes
 Wilm
 fiduswriter.org> License: LGPL-3.0-or-later Project-URL: repository, https://
 github.com/fiduswriter/django-npm-mjs Classifier: Environment :: Web
 Environment Classifier: Framework :: Django Classifier: Framework :: Django ::
 3.2 Classifier: Framework :: Django :: 4.0 Classifier: Framework :: Django ::
-4.1 Classifier: Intended Audience :: Developers Classifier: License :: OSI
+4.1 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Django ::
+5.0 Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: GNU Lesser General Public License v3 (LGPLv3) Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic ::
-Internet :: WWW/HTTP :: Dynamic Content Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: Django>=3.2 Requires-Dist: pyjson5==1.6.4
-# django-npm-mjs A Django package to use npm.js dependencies and transpile
-ES2015+ This package is used by Fidus Writer to bundle JavaScript. We try to
-keep it as generic as possible, so if there is something that seems very odd
-and specific to Fidus Writer, it is likely just an oversight from us. Please
-contact us and we'll see what we can do about it. This package similar to
-django-compressor in that it treats JavaScript files before they are served to
-the user. But there are some differences: * It does not mix different
-JavaScript module entry files. It only bundles everything imported from one
-entry file. With ES2015+ there is not as much need to have lots of JavaScript
-files operating in the global namespace. * It allows importing from one django
-app in another app within the same project as if they were in the same folder
-similar to how static files and templates are handled by Django. * It includes
-handling of npm.js imports. * The JavaScript entry files' base names do not
-change and an automatic version query is added to be able to wipe the browser
-cache (`/js/my_file.mjs` turns into `/js/my_file.js?v=239329884`). This way it
-is also possible to refer to the URL from JavaScript (for example for use with
-web workers). * It allows for JavaScript plugin hooks between django apps used
-in cases when a django project can be used both with or without a specific app,
-and the JavaScript from one app needs to import things from another app. Quick
-start ----------- 1. Install "npm_mjs" pip install django-npm-mjs 2. Add
-"npm_mjs" to your INSTALLED_APPS setting like this:: INSTALLED_APPS = [ ...
-'npm_mjs', ] 3. Define a `PROJECT_PATH` in the settings as the root folder of
-the project (`PROJECT_DIR` will also be accepted):: PROJECT_PATH =
-os.path.realpath(os.path.join(os.path.dirname(__file__), '..')) 4. Define a
-`SETTINGS_PATHS` in the settings to contain the paths of all setting files
-(settings.py + any local_settings.py or similar file you may have defined) -
-this is to transpile again whenever settings have changed:: SETTINGS_PATHS =
-[os.path.dirname(__file__), ] 5. Add the `static-transpile` folder inside the
-`PROJECT_PATH` to the `STATICFILES_DIRS` like this:: STATICFILES_DIRS =
-( os.path.join(PROJECT_PATH, 'static-transpile'), ... ) 6. Load transpile, and
-use `static` template tags to your templates to refer to JavaScript files. All
-entry files to ES2015+ modules need to have \*.mjs endings. Entries can look
-like this:: {% load transpile %} ...
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP ::
+Dynamic Content Description-Content-Type: text/markdown License-File: LICENSE
+Requires-Dist: Django>=3.2 Requires-Dist: pyjson5==1.6.6 # django-npm-mjs A
+Django package to use npm.js dependencies and transpile ES2015+ This package is
+used by Fidus Writer to bundle JavaScript. We try to keep it as generic as
+possible, so if there is something that seems very odd and specific to Fidus
+Writer, it is likely just an oversight from us. Please contact us and we'll see
+what we can do about it. This package similar to django-compressor in that it
+treats JavaScript files before they are served to the user. But there are some
+differences: * It does not mix different JavaScript module entry files. It only
+bundles everything imported from one entry file. With ES2015+ there is not as
+much need to have lots of JavaScript files operating in the global namespace. *
+It allows importing from one django app in another app within the same project
+as if they were in the same folder similar to how static files and templates
+are handled by Django. * It includes handling of npm.js imports. * The
+JavaScript entry files' base names do not change and an automatic version query
+is added to be able to wipe the browser cache (`/js/my_file.mjs` turns into `/
+js/my_file.js?v=239329884`). This way it is also possible to refer to the URL
+from JavaScript (for example for use with web workers). * It allows for
+JavaScript plugin hooks between django apps used in cases when a django project
+can be used both with or without a specific app, and the JavaScript from one
+app needs to import things from another app. Quick start ----------- 1. Install
+"npm_mjs" pip install django-npm-mjs 2. Add "npm_mjs" to your INSTALLED_APPS
+setting like this:: INSTALLED_APPS = [ ... 'npm_mjs', ] 3. Define a
+`PROJECT_PATH` in the settings as the root folder of the project (`PROJECT_DIR`
+will also be accepted):: PROJECT_PATH = os.path.realpath(os.path.join
+(os.path.dirname(__file__), '..')) 4. Define a `SETTINGS_PATHS` in the settings
+to contain the paths of all setting files (settings.py + any local_settings.py
+or similar file you may have defined) - this is to transpile again whenever
+settings have changed:: SETTINGS_PATHS = [os.path.dirname(__file__), ] 5. Add
+the `static-transpile` folder inside the `PROJECT_PATH` to the
+`STATICFILES_DIRS` like this:: STATICFILES_DIRS = ( os.path.join(PROJECT_PATH,
+'static-transpile'), ... ) 6. Load transpile, and use `static` template tags to
+your templates to refer to JavaScript files. All entry files to ES2015+ modules
+need to have \*.mjs endings. Entries can look like this:: {% load transpile %}
+...
 }">
 You can continue to load other resources such as CSS files as before using the
 `static` template tag::
 }" /> 7. Run `./manage.py transpile`. 8. Run `./manage.py runserver`. Your
 ES2015+ modules will be served as browser compatible JS files and all static
 files will have a versioned ending so that you can set your static server to
 let browsers cache static files indefinitely as long as DEBUG is set to False.
```

### Comparing `django-npm-mjs-2.5.0/README.md` & `django_npm_mjs-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `django-npm-mjs-2.5.0/django_npm_mjs.egg-info/PKG-INFO` & `django_npm_mjs-2.5.2/django_npm_mjs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: django-npm-mjs
-Version: 2.5.0
+Version: 2.5.2
 Summary: A Django package to use npm.js dependencies and transpile ES2015+
 Author-email: Johannes Wilm <johannes@fiduswriter.org>
 License: LGPL-3.0-or-later
 Project-URL: repository, https://github.com/fiduswriter/django-npm-mjs
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=3.2
-Requires-Dist: pyjson5==1.6.4
+Requires-Dist: pyjson5==1.6.6
 
 # django-npm-mjs
 A Django package to use npm.js dependencies and transpile ES2015+
 
 This package is used by Fidus Writer to bundle JavaScript. We try to keep it as generic as possible, so if there is something that seems very odd and specific to Fidus Writer, it is likely just an oversight from us. Please contact us and we'll see what we can do about it.
 
 This package similar to django-compressor in that it treats JavaScript files before they are served to the user. But there are some differences:
```

#### html2text {}

```diff
@@ -1,56 +1,58 @@
-Metadata-Version: 2.1 Name: django-npm-mjs Version: 2.5.0 Summary: A Django
+Metadata-Version: 2.1 Name: django-npm-mjs Version: 2.5.2 Summary: A Django
 package to use npm.js dependencies and transpile ES2015+ Author-email: Johannes
 Wilm
 fiduswriter.org> License: LGPL-3.0-or-later Project-URL: repository, https://
 github.com/fiduswriter/django-npm-mjs Classifier: Environment :: Web
 Environment Classifier: Framework :: Django Classifier: Framework :: Django ::
 3.2 Classifier: Framework :: Django :: 4.0 Classifier: Framework :: Django ::
-4.1 Classifier: Intended Audience :: Developers Classifier: License :: OSI
+4.1 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Django ::
+5.0 Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: GNU Lesser General Public License v3 (LGPLv3) Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic ::
-Internet :: WWW/HTTP :: Dynamic Content Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: Django>=3.2 Requires-Dist: pyjson5==1.6.4
-# django-npm-mjs A Django package to use npm.js dependencies and transpile
-ES2015+ This package is used by Fidus Writer to bundle JavaScript. We try to
-keep it as generic as possible, so if there is something that seems very odd
-and specific to Fidus Writer, it is likely just an oversight from us. Please
-contact us and we'll see what we can do about it. This package similar to
-django-compressor in that it treats JavaScript files before they are served to
-the user. But there are some differences: * It does not mix different
-JavaScript module entry files. It only bundles everything imported from one
-entry file. With ES2015+ there is not as much need to have lots of JavaScript
-files operating in the global namespace. * It allows importing from one django
-app in another app within the same project as if they were in the same folder
-similar to how static files and templates are handled by Django. * It includes
-handling of npm.js imports. * The JavaScript entry files' base names do not
-change and an automatic version query is added to be able to wipe the browser
-cache (`/js/my_file.mjs` turns into `/js/my_file.js?v=239329884`). This way it
-is also possible to refer to the URL from JavaScript (for example for use with
-web workers). * It allows for JavaScript plugin hooks between django apps used
-in cases when a django project can be used both with or without a specific app,
-and the JavaScript from one app needs to import things from another app. Quick
-start ----------- 1. Install "npm_mjs" pip install django-npm-mjs 2. Add
-"npm_mjs" to your INSTALLED_APPS setting like this:: INSTALLED_APPS = [ ...
-'npm_mjs', ] 3. Define a `PROJECT_PATH` in the settings as the root folder of
-the project (`PROJECT_DIR` will also be accepted):: PROJECT_PATH =
-os.path.realpath(os.path.join(os.path.dirname(__file__), '..')) 4. Define a
-`SETTINGS_PATHS` in the settings to contain the paths of all setting files
-(settings.py + any local_settings.py or similar file you may have defined) -
-this is to transpile again whenever settings have changed:: SETTINGS_PATHS =
-[os.path.dirname(__file__), ] 5. Add the `static-transpile` folder inside the
-`PROJECT_PATH` to the `STATICFILES_DIRS` like this:: STATICFILES_DIRS =
-( os.path.join(PROJECT_PATH, 'static-transpile'), ... ) 6. Load transpile, and
-use `static` template tags to your templates to refer to JavaScript files. All
-entry files to ES2015+ modules need to have \*.mjs endings. Entries can look
-like this:: {% load transpile %} ...
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP ::
+Dynamic Content Description-Content-Type: text/markdown License-File: LICENSE
+Requires-Dist: Django>=3.2 Requires-Dist: pyjson5==1.6.6 # django-npm-mjs A
+Django package to use npm.js dependencies and transpile ES2015+ This package is
+used by Fidus Writer to bundle JavaScript. We try to keep it as generic as
+possible, so if there is something that seems very odd and specific to Fidus
+Writer, it is likely just an oversight from us. Please contact us and we'll see
+what we can do about it. This package similar to django-compressor in that it
+treats JavaScript files before they are served to the user. But there are some
+differences: * It does not mix different JavaScript module entry files. It only
+bundles everything imported from one entry file. With ES2015+ there is not as
+much need to have lots of JavaScript files operating in the global namespace. *
+It allows importing from one django app in another app within the same project
+as if they were in the same folder similar to how static files and templates
+are handled by Django. * It includes handling of npm.js imports. * The
+JavaScript entry files' base names do not change and an automatic version query
+is added to be able to wipe the browser cache (`/js/my_file.mjs` turns into `/
+js/my_file.js?v=239329884`). This way it is also possible to refer to the URL
+from JavaScript (for example for use with web workers). * It allows for
+JavaScript plugin hooks between django apps used in cases when a django project
+can be used both with or without a specific app, and the JavaScript from one
+app needs to import things from another app. Quick start ----------- 1. Install
+"npm_mjs" pip install django-npm-mjs 2. Add "npm_mjs" to your INSTALLED_APPS
+setting like this:: INSTALLED_APPS = [ ... 'npm_mjs', ] 3. Define a
+`PROJECT_PATH` in the settings as the root folder of the project (`PROJECT_DIR`
+will also be accepted):: PROJECT_PATH = os.path.realpath(os.path.join
+(os.path.dirname(__file__), '..')) 4. Define a `SETTINGS_PATHS` in the settings
+to contain the paths of all setting files (settings.py + any local_settings.py
+or similar file you may have defined) - this is to transpile again whenever
+settings have changed:: SETTINGS_PATHS = [os.path.dirname(__file__), ] 5. Add
+the `static-transpile` folder inside the `PROJECT_PATH` to the
+`STATICFILES_DIRS` like this:: STATICFILES_DIRS = ( os.path.join(PROJECT_PATH,
+'static-transpile'), ... ) 6. Load transpile, and use `static` template tags to
+your templates to refer to JavaScript files. All entry files to ES2015+ modules
+need to have \*.mjs endings. Entries can look like this:: {% load transpile %}
+...
 }">
 You can continue to load other resources such as CSS files as before using the
 `static` template tag::
 }" /> 7. Run `./manage.py transpile`. 8. Run `./manage.py runserver`. Your
 ES2015+ modules will be served as browser compatible JS files and all static
 files will have a versioned ending so that you can set your static server to
 let browsers cache static files indefinitely as long as DEBUG is set to False.
```

### Comparing `django-npm-mjs-2.5.0/django_npm_mjs.egg-info/SOURCES.txt` & `django_npm_mjs-2.5.2/django_npm_mjs.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 setup.py
 django_npm_mjs.egg-info/PKG-INFO
 django_npm_mjs.egg-info/SOURCES.txt
 django_npm_mjs.egg-info/dependency_links.txt
 django_npm_mjs.egg-info/requires.txt
 django_npm_mjs.egg-info/top_level.txt
 npm_mjs/__init__.py
+npm_mjs/package.json5
 npm_mjs/paths.py
 npm_mjs/signals.py
 npm_mjs/storage.py
 npm_mjs/tools.py
 npm_mjs/management/__init__.py
 npm_mjs/management/commands/__init__.py
 npm_mjs/management/commands/collectstatic.py
```

### Comparing `django-npm-mjs-2.5.0/npm_mjs/management/commands/create_package_json.py` & `django_npm_mjs-2.5.2/npm_mjs/management/commands/create_package_json.py`

 * *Files identical despite different names*

### Comparing `django-npm-mjs-2.5.0/npm_mjs/management/commands/makemessages.py` & `django_npm_mjs-2.5.2/npm_mjs/management/commands/makemessages.py`

 * *Files identical despite different names*

### Comparing `django-npm-mjs-2.5.0/npm_mjs/management/commands/npm_install.py` & `django_npm_mjs-2.5.2/npm_mjs/management/commands/npm_install.py`

 * *Files identical despite different names*

### Comparing `django-npm-mjs-2.5.0/npm_mjs/management/commands/transpile.py` & `django_npm_mjs-2.5.2/npm_mjs/management/commands/transpile.py`

 * *Files identical despite different names*

### Comparing `django-npm-mjs-2.5.0/npm_mjs/management/commands/webpack.config.template.js` & `django_npm_mjs-2.5.2/npm_mjs/management/commands/webpack.config.template.js`

 * *Files identical despite different names*

### Comparing `django-npm-mjs-2.5.0/npm_mjs/storage.py` & `django_npm_mjs-2.5.2/npm_mjs/storage.py`

 * *Files identical despite different names*

### Comparing `django-npm-mjs-2.5.0/npm_mjs/templatetags/transpile.py` & `django_npm_mjs-2.5.2/npm_mjs/templatetags/transpile.py`

 * *Files identical despite different names*

### Comparing `django-npm-mjs-2.5.0/npm_mjs/tools.py` & `django_npm_mjs-2.5.2/npm_mjs/tools.py`

 * *Files identical despite different names*

### Comparing `django-npm-mjs-2.5.0/pyproject.toml` & `django_npm_mjs-2.5.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -3,36 +3,39 @@
   "setuptools>=68.2.2",
   "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-npm-mjs"
-version = "2.5.0"
+version = "2.5.2"
 description = "A Django package to use npm.js dependencies and transpile ES2015+"
 license = {text = "LGPL-3.0-or-later"}
 readme = "README.md"
 authors = [
   {name="Johannes Wilm", email="johannes@fiduswriter.org"}
 ]
 classifiers = [
   "Environment :: Web Environment",
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
+  "Framework :: Django :: 4.2",
+  "Framework :: Django :: 5.0",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Internet :: WWW/HTTP :: Dynamic Content"
 ]
 urls = {repository = "https://github.com/fiduswriter/django-npm-mjs"}
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
```

