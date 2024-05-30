# Comparing `tmp/django-zxcvbn-password-validator-1.4.3.tar.gz` & `tmp/django_zxcvbn_password_validator-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-zxcvbn-password-validator-1.4.3.tar", last modified: Tue Jan  2 22:50:21 2024, max compression
+gzip compressed data, was "django_zxcvbn_password_validator-1.4.4.tar", last modified: Thu May 30 09:38:51 2024, max compression
```

## Comparing `django-zxcvbn-password-validator-1.4.3.tar` & `django_zxcvbn_password_validator-1.4.4.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:50:21.160454 django-zxcvbn-password-validator-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-02 22:50:09.000000 django-zxcvbn-password-validator-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-01-02 22:50:21.160454 django-zxcvbn-password-validator-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-01-02 22:50:09.000000 django-zxcvbn-password-validator-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:50:21.156454 django-zxcvbn-password-validator-1.4.3/django_zxcvbn_password_validator/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-01-02 22:50:09.000000 django-zxcvbn-password-validator-1.4.3/django_zxcvbn_password_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-02 22:50:09.000000 django-zxcvbn-password-validator-1.4.3/django_zxcvbn_password_validator/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-01-02 22:50:09.000000 django-zxcvbn-password-validator-1.4.3/django_zxcvbn_password_validator/test_translate_zxcvbn_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-01-02 22:50:09.000000 django-zxcvbn-password-validator-1.4.3/django_zxcvbn_password_validator/test_zxcvbn_password_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-01-02 22:50:09.000000 django-zxcvbn-password-validator-1.4.3/django_zxcvbn_password_validator/translate_zxcvbn_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-01-02 22:50:09.000000 django-zxcvbn-password-validator-1.4.3/django_zxcvbn_password_validator/zxcvbn_password_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:50:21.160454 django-zxcvbn-password-validator-1.4.3/django_zxcvbn_password_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-01-02 22:50:21.000000 django-zxcvbn-password-validator-1.4.3/django_zxcvbn_password_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-01-02 22:50:21.000000 django-zxcvbn-password-validator-1.4.3/django_zxcvbn_password_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 22:50:21.000000 django-zxcvbn-password-validator-1.4.3/django_zxcvbn_password_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-02 22:50:21.000000 django-zxcvbn-password-validator-1.4.3/django_zxcvbn_password_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-02 22:50:21.000000 django-zxcvbn-password-validator-1.4.3/django_zxcvbn_password_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-01-02 22:50:09.000000 django-zxcvbn-password-validator-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-02 22:50:21.160454 django-zxcvbn-password-validator-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-02 22:50:09.000000 django-zxcvbn-password-validator-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:38:51.876589 django_zxcvbn_password_validator-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-30 09:38:42.000000 django_zxcvbn_password_validator-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-30 09:38:51.876589 django_zxcvbn_password_validator-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-30 09:38:42.000000 django_zxcvbn_password_validator-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:38:51.872589 django_zxcvbn_password_validator-1.4.4/django_zxcvbn_password_validator/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-30 09:38:42.000000 django_zxcvbn_password_validator-1.4.4/django_zxcvbn_password_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 09:38:42.000000 django_zxcvbn_password_validator-1.4.4/django_zxcvbn_password_validator/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-30 09:38:42.000000 django_zxcvbn_password_validator-1.4.4/django_zxcvbn_password_validator/test_translate_zxcvbn_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-05-30 09:38:42.000000 django_zxcvbn_password_validator-1.4.4/django_zxcvbn_password_validator/test_zxcvbn_password_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-30 09:38:42.000000 django_zxcvbn_password_validator-1.4.4/django_zxcvbn_password_validator/translate_zxcvbn_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-30 09:38:42.000000 django_zxcvbn_password_validator-1.4.4/django_zxcvbn_password_validator/zxcvbn_password_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:38:51.876589 django_zxcvbn_password_validator-1.4.4/django_zxcvbn_password_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-30 09:38:51.000000 django_zxcvbn_password_validator-1.4.4/django_zxcvbn_password_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-30 09:38:51.000000 django_zxcvbn_password_validator-1.4.4/django_zxcvbn_password_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:38:51.000000 django_zxcvbn_password_validator-1.4.4/django_zxcvbn_password_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-30 09:38:51.000000 django_zxcvbn_password_validator-1.4.4/django_zxcvbn_password_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-30 09:38:51.000000 django_zxcvbn_password_validator-1.4.4/django_zxcvbn_password_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-30 09:38:42.000000 django_zxcvbn_password_validator-1.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 09:38:51.876589 django_zxcvbn_password_validator-1.4.4/setup.cfg
```

### Comparing `django-zxcvbn-password-validator-1.4.3/LICENSE` & `django_zxcvbn_password_validator-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-zxcvbn-password-validator-1.4.3/PKG-INFO` & `django_zxcvbn_password_validator-1.4.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 Metadata-Version: 2.1
 Name: django-zxcvbn-password-validator
-Version: 1.4.3
+Version: 1.4.4
 Summary: A translatable password validator for django, based on zxcvbn-python.
 Author-email: Pierre SASSOULAS <pierre.sassoulas@gmail.com>
 License: MIT
-Project-URL: Source Code, https://github.com/Pierre-Sassoulas/django-zxcvbn-password-validator
 Project-URL: Bug Tracker, https://github.com/Pierre-Sassoulas/django-zxcvbn-password-validator/issues
+Project-URL: Source Code, https://github.com/Pierre-Sassoulas/django-zxcvbn-password-validator
+Keywords: django,password-validator,zxcvbn
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Natural Language :: English
-Classifier: Natural Language :: French
-Classifier: Natural Language :: Dutch
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Dutch
+Classifier: Natural Language :: English
+Classifier: Natural Language :: French
+Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django<6,>=2.0
+Requires-Dist: django<6,>=2
 Requires-Dist: zxcvbn
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
+Requires-Dist: coveralls; extra == "dev"
 Requires-Dist: django-rosetta; extra == "dev"
 Requires-Dist: mock; extra == "dev"
 Requires-Dist: pre-commit>=2.16; extra == "dev"
-Requires-Dist: pylint>=3.0.3; extra == "dev"
+Requires-Dist: pylint>=3.2; extra == "dev"
 Requires-Dist: pylint-django; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
 Requires-Dist: python-coveralls; extra == "dev"
-Requires-Dist: coveralls; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 
 # django-zxcvbn-password-validator
 
 A translatable password validator for django, based on zxcvbn-python and available with
 pip.
 
@@ -57,14 +59,15 @@
 ### Language available
 
 The software is developed in english. Other available languages are :
 
 - [x] Dutch thanks to [Thom Wiggers](https://github.com/thomwiggers/)
 - [x] French thanks to [Pierre Sassoulas](https://github.com/Pierre-Sassoulas/) and
       [Lionel Sausin](https://github.com/ls-initiatives)
+- [x] Brazilian Portuguese thanks to [Andrés Martano](https://github.com/andresmrm/)
 - [x] English
 
 ## Creating a user with django-zxcvbn-password-validator
 
 If the password is not strong enough, we provide errors explaining what you need to do :
 
 ![English example](doc/english_example.png "English example")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-zxcvbn-password-validator-1.4.3/README.md` & `django_zxcvbn_password_validator-1.4.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 ### Language available
 
 The software is developed in english. Other available languages are :
 
 - [x] Dutch thanks to [Thom Wiggers](https://github.com/thomwiggers/)
 - [x] French thanks to [Pierre Sassoulas](https://github.com/Pierre-Sassoulas/) and
       [Lionel Sausin](https://github.com/ls-initiatives)
+- [x] Brazilian Portuguese thanks to [Andrés Martano](https://github.com/andresmrm/)
 - [x] English
 
 ## Creating a user with django-zxcvbn-password-validator
 
 If the password is not strong enough, we provide errors explaining what you need to do :
 
 ![English example](doc/english_example.png "English example")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-zxcvbn-password-validator-1.4.3/django_zxcvbn_password_validator/test_translate_zxcvbn_text.py` & `django_zxcvbn_password_validator-1.4.4/django_zxcvbn_password_validator/test_translate_zxcvbn_text.py`

 * *Files identical despite different names*

### Comparing `django-zxcvbn-password-validator-1.4.3/django_zxcvbn_password_validator/test_zxcvbn_password_validator.py` & `django_zxcvbn_password_validator-1.4.4/django_zxcvbn_password_validator/test_zxcvbn_password_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,24 +86,27 @@
         self.assertIsNone(self.validator.validate("password"))
         self.assertIsNone(self.validator.validate("123"))
         self.assertIsNone(self.validator.validate("godzilla"))
 
     @override_settings(PASSWORD_MINIMAL_STRENGTH=None)
     @override_settings(PASSWORD_MINIMAL_STRENTH=0)
     def test_compatibility_with_old_settings(self):
-        """If we're using the default value of 2 instead of taking the old
-        value into account the password are not strong enough."""
+        """'PASSWORD_MINIMAL_STRENTH' with a typo is still working.
+
+        If we're using the default value of 2 instead of taking the value
+        from 'PASSWORD_MINIMAL_STRENTH' into account  then 'password'
+        would not be strong enough.
+        """
         self.validator = ZxcvbnPasswordValidator()
         self.assertIsNone(self.validator.validate("password"))
 
     @override_settings(PASSWORD_MINIMAL_STRENGTH=0)
     @override_settings(PASSWORD_MINIMAL_STRENTH=2)
     def test_priority_of_new_settings(self):
-        """We need to give priority to the new value when we
-        have both settings."""
+        """We need to give priority to the new value when we have both settings."""
         self.validator = ZxcvbnPasswordValidator()
         self.assertIsNone(self.validator.validate("password"))
 
     @override_settings(PASSWORD_MINIMAL_STRENGTH=2)
     @override_settings(LANGUAGE_CODE="en-us")
     def test_medium_strength(self):
         self.validator = ZxcvbnPasswordValidator()
```

### Comparing `django-zxcvbn-password-validator-1.4.3/django_zxcvbn_password_validator/translate_zxcvbn_text.py` & `django_zxcvbn_password_validator-1.4.4/django_zxcvbn_password_validator/translate_zxcvbn_text.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 except ImportError:
     from django.utils.translation import ugettext_lazy as _
 
 LOGGER = logging.getLogger(__file__)
 
 
 def translate_zxcvbn_text(text):
-    """This PR would make it cleaner, but it will also be very slow
-    to be integrated in python-zxcvbn and we want this to work now :
-    https://github.com/dropbox/zxcvbn/pull/124"""
+    """Translate text using our own i18n dict.
+
+    https://github.com/dropbox/zxcvbn/pull/124#issuecomment-430081232 would have
+    made this cleaner.
+    """
     i18n = {
         "Use a few words, avoid common phrases": _(
             "Use a few words, avoid common phrases"
         ),
         "No need for symbols, digits, or uppercase letters": _(
             "No need for symbols, digits, or uppercase letters"
         ),
```

### Comparing `django-zxcvbn-password-validator-1.4.3/django_zxcvbn_password_validator/zxcvbn_password_validator.py` & `django_zxcvbn_password_validator-1.4.4/django_zxcvbn_password_validator/zxcvbn_password_validator.py`

 * *Files identical despite different names*

### Comparing `django-zxcvbn-password-validator-1.4.3/django_zxcvbn_password_validator.egg-info/PKG-INFO` & `django_zxcvbn_password_validator-1.4.4/django_zxcvbn_password_validator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 Metadata-Version: 2.1
 Name: django-zxcvbn-password-validator
-Version: 1.4.3
+Version: 1.4.4
 Summary: A translatable password validator for django, based on zxcvbn-python.
 Author-email: Pierre SASSOULAS <pierre.sassoulas@gmail.com>
 License: MIT
-Project-URL: Source Code, https://github.com/Pierre-Sassoulas/django-zxcvbn-password-validator
 Project-URL: Bug Tracker, https://github.com/Pierre-Sassoulas/django-zxcvbn-password-validator/issues
+Project-URL: Source Code, https://github.com/Pierre-Sassoulas/django-zxcvbn-password-validator
+Keywords: django,password-validator,zxcvbn
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Natural Language :: English
-Classifier: Natural Language :: French
-Classifier: Natural Language :: Dutch
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Dutch
+Classifier: Natural Language :: English
+Classifier: Natural Language :: French
+Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django<6,>=2.0
+Requires-Dist: django<6,>=2
 Requires-Dist: zxcvbn
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
+Requires-Dist: coveralls; extra == "dev"
 Requires-Dist: django-rosetta; extra == "dev"
 Requires-Dist: mock; extra == "dev"
 Requires-Dist: pre-commit>=2.16; extra == "dev"
-Requires-Dist: pylint>=3.0.3; extra == "dev"
+Requires-Dist: pylint>=3.2; extra == "dev"
 Requires-Dist: pylint-django; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
 Requires-Dist: python-coveralls; extra == "dev"
-Requires-Dist: coveralls; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 
 # django-zxcvbn-password-validator
 
 A translatable password validator for django, based on zxcvbn-python and available with
 pip.
 
@@ -57,14 +59,15 @@
 ### Language available
 
 The software is developed in english. Other available languages are :
 
 - [x] Dutch thanks to [Thom Wiggers](https://github.com/thomwiggers/)
 - [x] French thanks to [Pierre Sassoulas](https://github.com/Pierre-Sassoulas/) and
       [Lionel Sausin](https://github.com/ls-initiatives)
+- [x] Brazilian Portuguese thanks to [Andrés Martano](https://github.com/andresmrm/)
 - [x] English
 
 ## Creating a user with django-zxcvbn-password-validator
 
 If the password is not strong enough, we provide errors explaining what you need to do :
 
 ![English example](doc/english_example.png "English example")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-zxcvbn-password-validator-1.4.3/django_zxcvbn_password_validator.egg-info/SOURCES.txt` & `django_zxcvbn_password_validator-1.4.4/django_zxcvbn_password_validator.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-setup.py
 django_zxcvbn_password_validator/__init__.py
 django_zxcvbn_password_validator/settings.py
 django_zxcvbn_password_validator/test_translate_zxcvbn_text.py
 django_zxcvbn_password_validator/test_zxcvbn_password_validator.py
 django_zxcvbn_password_validator/translate_zxcvbn_text.py
 django_zxcvbn_password_validator/zxcvbn_password_validator.py
 django_zxcvbn_password_validator.egg-info/PKG-INFO
```

### Comparing `django-zxcvbn-password-validator-1.4.3/pyproject.toml` & `django_zxcvbn_password_validator-1.4.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,81 +1,109 @@
 [build-system]
-requires = ["setuptools>=67.5.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
-[tool.setuptools.packages.find]
-include = ["django_zxcvbn_password_validator*"]
+requires = [
+  "setuptools>=67.5.1",
+  "wheel",
+]
 
 [project]
 name = "django-zxcvbn-password-validator"
+version = "1.4.4"
 description = "A translatable password validator for django, based on zxcvbn-python."
-version = "1.4.3"
 readme = "README.md"
+keywords = [
+  "django",
+  "password-validator",
+  "zxcvbn",
+]
+license = { text = "MIT" }
 authors = [
-    {email="pierre.sassoulas@gmail.com", name="Pierre SASSOULAS"}
+  { email = "pierre.sassoulas@gmail.com", name = "Pierre SASSOULAS" },
 ]
-license = {text = "MIT"}
+requires-python = ">=3.8.0"
+
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Natural Language :: English",
-    "Natural Language :: French",
-    "Natural Language :: Dutch",
-    "Framework :: Django",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
+  "Development Status :: 5 - Production/Stable",
+  "Framework :: Django",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Natural Language :: Dutch",
+  "Natural Language :: English",
+  "Natural Language :: French",
+  "Natural Language :: Portuguese (Brazilian)",
+  "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
-    "django>=2.0,<6",
-    "zxcvbn",
+  "django>=2,<6",
+  "zxcvbn",
 ]
-requires-python = ">=3.8.0"
+optional-dependencies.dev = [
+  "coverage",
+  "coveralls",
+  "django-rosetta",
+  "mock",
+  "pre-commit>=2.16",
+  "pylint>=3.2",
+  "pylint-django",
+  "python-coveralls",
+  "tox",
+]
+urls."Bug Tracker" = "https://github.com/Pierre-Sassoulas/django-zxcvbn-password-validator/issues"
+urls."Source Code" = "https://github.com/Pierre-Sassoulas/django-zxcvbn-password-validator"
 
-[project.urls]
-"Source Code"       = "https://github.com/Pierre-Sassoulas/django-zxcvbn-password-validator"
-"Bug Tracker"       = "https://github.com/Pierre-Sassoulas/django-zxcvbn-password-validator/issues"
-
-[project.optional-dependencies]
-dev = [
-    "coverage",
-    "django-rosetta",
-    "mock",
-    "pre-commit>=2.16",
-    "pylint>=3.0.3",
-    "pylint-django",
-    "coverage",
-    "python-coveralls",
-    "coveralls",
-    "tox",
+[tool.setuptools.packages.find]
+include = [
+  "django_zxcvbn_password_validator*",
 ]
 
 [tool.ruff]
 
 line-length = 88
-
-select = [
-    "E",  # pycodestyle
-    "F",  # pyflakes
-    "W",  # pycodestyle
-    "B",  # bugbear
-    "I",  # isort
-    "RUF", # ruff
-    "UP", # pyupgrade
+lint.select = [
+  "B",      # bugbear
+  "D",      # pydocstyle
+  "E",      # pycodestyle
+  "F",      # pyflakes
+  "I",      # isort
+  "PGH004", # pygrep-hooks - Use specific rule codes when using noqa
+  "PIE",    # flake8-pie
+  "PL",     # pylint
+  "PYI",    # flake8-pyi
+  "RUF",    # ruff
+  "T100",   # flake8-debugger
+  "UP",     # pyupgrade
+  "W",      # pycodestyle
+]
+
+lint.ignore = [
+  # pydocstyle ignore
+  "D100", # Missing docstring in public module
+  "D101", # Missing docstring in public class
+  "D102", # Missing docstring in public method
+  "D103", # Missing docstring in public function
+  "D105", # Missing docstring in magic method
+  "D106", # Missing docstring in public nested class
+  "D107", # Missing docstring in `__init__`
+  "D203", # one-blank-line-before-class`
+  # pylint ignore
+  "PLR2004", # Magic value used in comparison
 ]
 
 [tool.pylint.main]
 
 load-plugins = "pylint_django"
-django-settings-module="django_zxcvbn_password_validator.settings"
-disable=[
-    # I0011 Warning locally suppressed using disable-msg
-    "I0011",
-    "missing-docstring", # We don't want docstring everywhere
-    "imported-auth-user", # harmful according to django's dev
+django-settings-module = "django_zxcvbn_password_validator.settings"
+disable = [
+  # I0011 Warning locally suppressed using disable-msg
+  "I0011",
+  "missing-docstring",  # We don't want docstring everywhere
+  "imported-auth-user", # harmful according to django's dev
 ]
 
 max-line-length = 88
```

