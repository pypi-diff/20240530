# Comparing `tmp/m9s_project_invoice_pricelist-7.0.2.tar.gz` & `tmp/m9s_project_invoice_pricelist-7.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_project_invoice_pricelist-7.0.2.tar", last modified: Wed May 29 16:04:01 2024, max compression
+gzip compressed data, was "m9s_project_invoice_pricelist-7.0.3.tar", last modified: Thu May 30 17:41:32 2024, max compression
```

## Comparing `m9s_project_invoice_pricelist-7.0.2.tar` & `m9s_project_invoice_pricelist-7.0.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-29 16:04:01.266717 m9s_project_invoice_pricelist-7.0.2/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       95 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-13 19:23:18.000000 m9s_project_invoice_pricelist-7.0.2/.drone.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/.gitlab-ci-m9s.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2204 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/.isort.cfg
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-29 16:04:01.266717 m9s_project_invoice_pricelist-7.0.2/.woodpecker/
--rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/.woodpecker/mail_curl.sh
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/.woodpecker/report.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/.woodpecker/test.yml
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      690 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/MANIFEST.in
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3330 2024-05-29 16:04:01.266717 m9s_project_invoice_pricelist-7.0.2/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1112 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       66 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/README.rst
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      303 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       86 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/dev_requirements.txt
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-29 16:04:01.266717 m9s_project_invoice_pricelist-7.0.2/doc/
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-29 16:04:01.266717 m9s_project_invoice_pricelist-7.0.2/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       65 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/doc/de/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       66 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/doc/index.rst
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-29 16:04:01.266717 m9s_project_invoice_pricelist-7.0.2/locale/
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      691 2024-05-29 16:03:48.000000 m9s_project_invoice_pricelist-7.0.2/locale/de.po
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-29 16:04:01.266717 m9s_project_invoice_pricelist-7.0.2/m9s_project_invoice_pricelist.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3330 2024-05-29 16:04:00.000000 m9s_project_invoice_pricelist-7.0.2/m9s_project_invoice_pricelist.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      899 2024-05-29 16:04:01.000000 m9s_project_invoice_pricelist-7.0.2/m9s_project_invoice_pricelist.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-05-29 16:04:00.000000 m9s_project_invoice_pricelist-7.0.2/m9s_project_invoice_pricelist.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       88 2024-05-29 16:04:00.000000 m9s_project_invoice_pricelist-7.0.2/m9s_project_invoice_pricelist.egg-info/entry_points.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2021-04-04 19:01:02.000000 m9s_project_invoice_pricelist-7.0.2/m9s_project_invoice_pricelist.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       98 2024-05-29 16:04:00.000000 m9s_project_invoice_pricelist-7.0.2/m9s_project_invoice_pricelist.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-05-29 16:04:00.000000 m9s_project_invoice_pricelist-7.0.2/m9s_project_invoice_pricelist.egg-info/top_level.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/requirements.txt
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-05-29 16:04:01.266717 m9s_project_invoice_pricelist-7.0.2/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4504 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/setup.py
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-29 16:04:01.266717 m9s_project_invoice_pricelist-7.0.2/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/tests/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      331 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/tests/test_module.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/tox.ini
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      131 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/tryton.cfg
-drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-29 16:04:01.266717 m9s_project_invoice_pricelist-7.0.2/view/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      429 2022-11-10 15:09:53.000000 m9s_project_invoice_pricelist-7.0.2/view/work_form.xml
--rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3573 2024-05-29 16:03:48.000000 m9s_project_invoice_pricelist-7.0.2/work.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      424 2020-10-02 08:16:00.000000 m9s_project_invoice_pricelist-7.0.2/work.xml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-30 17:41:32.381683 m9s_project_invoice_pricelist-7.0.3/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       95 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-13 19:23:18.000000 m9s_project_invoice_pricelist-7.0.3/.drone.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/.gitlab-ci-m9s.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2204 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/.isort.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-30 17:41:32.377683 m9s_project_invoice_pricelist-7.0.3/.woodpecker/
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/.woodpecker/test.yml
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      690 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/MANIFEST.in
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3330 2024-05-30 17:41:32.381683 m9s_project_invoice_pricelist-7.0.3/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1112 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       66 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/README.rst
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      303 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       86 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/dev_requirements.txt
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-30 17:41:32.377683 m9s_project_invoice_pricelist-7.0.3/doc/
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-30 17:41:32.377683 m9s_project_invoice_pricelist-7.0.3/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       65 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/doc/de/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       66 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/doc/index.rst
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-30 17:41:32.377683 m9s_project_invoice_pricelist-7.0.3/locale/
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      691 2024-05-29 16:03:48.000000 m9s_project_invoice_pricelist-7.0.3/locale/de.po
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-30 17:41:32.381683 m9s_project_invoice_pricelist-7.0.3/m9s_project_invoice_pricelist.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3330 2024-05-30 17:41:31.000000 m9s_project_invoice_pricelist-7.0.3/m9s_project_invoice_pricelist.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      899 2024-05-30 17:41:32.000000 m9s_project_invoice_pricelist-7.0.3/m9s_project_invoice_pricelist.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-05-30 17:41:31.000000 m9s_project_invoice_pricelist-7.0.3/m9s_project_invoice_pricelist.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       88 2024-05-30 17:41:31.000000 m9s_project_invoice_pricelist-7.0.3/m9s_project_invoice_pricelist.egg-info/entry_points.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2021-04-04 19:01:02.000000 m9s_project_invoice_pricelist-7.0.3/m9s_project_invoice_pricelist.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       98 2024-05-30 17:41:31.000000 m9s_project_invoice_pricelist-7.0.3/m9s_project_invoice_pricelist.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-05-30 17:41:31.000000 m9s_project_invoice_pricelist-7.0.3/m9s_project_invoice_pricelist.egg-info/top_level.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/requirements.txt
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-05-30 17:41:32.381683 m9s_project_invoice_pricelist-7.0.3/setup.cfg
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4504 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/setup.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-30 17:41:32.377683 m9s_project_invoice_pricelist-7.0.3/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/tests/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      331 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/tests/test_module.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.3/tox.ini
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      131 2024-05-29 16:04:07.000000 m9s_project_invoice_pricelist-7.0.3/tryton.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-30 17:41:32.377683 m9s_project_invoice_pricelist-7.0.3/view/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      429 2022-11-10 15:09:53.000000 m9s_project_invoice_pricelist-7.0.3/view/work_form.xml
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3593 2024-05-30 17:27:28.000000 m9s_project_invoice_pricelist-7.0.3/work.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      424 2020-10-02 08:16:00.000000 m9s_project_invoice_pricelist-7.0.3/work.xml
```

### Comparing `m9s_project_invoice_pricelist-7.0.2/.drone.yml` & `m9s_project_invoice_pricelist-7.0.3/.drone.yml`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.2/.gitlab-ci.yml` & `m9s_project_invoice_pricelist-7.0.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.2/.woodpecker/mail_curl.sh` & `m9s_project_invoice_pricelist-7.0.3/.woodpecker/mail_curl.sh`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.2/.woodpecker/report.yml` & `m9s_project_invoice_pricelist-7.0.3/.woodpecker/report.yml`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.2/.woodpecker/test.yml` & `m9s_project_invoice_pricelist-7.0.3/.woodpecker/test.yml`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.2/COPYRIGHT` & `m9s_project_invoice_pricelist-7.0.3/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.2/INSTALL` & `m9s_project_invoice_pricelist-7.0.3/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.2/LICENSE` & `m9s_project_invoice_pricelist-7.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.2/PKG-INFO` & `m9s_project_invoice_pricelist-7.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s_project_invoice_pricelist
-Version: 7.0.2
+Version: 7.0.3
 Summary: Tryton Project Invoice Pricelist Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/project_invoice_pricelist.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
```

### Comparing `m9s_project_invoice_pricelist-7.0.2/README.md` & `m9s_project_invoice_pricelist-7.0.3/README.md`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.2/locale/de.po` & `m9s_project_invoice_pricelist-7.0.3/locale/de.po`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.2/m9s_project_invoice_pricelist.egg-info/PKG-INFO` & `m9s_project_invoice_pricelist-7.0.3/m9s_project_invoice_pricelist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s-project-invoice-pricelist
-Version: 7.0.2
+Version: 7.0.3
 Summary: Tryton Project Invoice Pricelist Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/project_invoice_pricelist.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
```

### Comparing `m9s_project_invoice_pricelist-7.0.2/m9s_project_invoice_pricelist.egg-info/SOURCES.txt` & `m9s_project_invoice_pricelist-7.0.3/m9s_project_invoice_pricelist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.2/setup.py` & `m9s_project_invoice_pricelist-7.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.2/tox.ini` & `m9s_project_invoice_pricelist-7.0.3/tox.ini`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.2/work.py` & `m9s_project_invoice_pricelist-7.0.3/work.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,16 @@
         '- Pricelist of the task\n'
         '- Pricelist of the parent project\n'
         '- Pricelist of the party\n'
         '- Pricelist of sale configuration')
     price_list_used = fields.Function(fields.Many2One('product.price_list',
             'Price List Used'), 'on_change_with_price_list_used')
 
-    @fields.depends('price_list', 'parent', '_parent_parent.parent', 'party')
+    @fields.depends(
+        'company', 'price_list', 'parent', '_parent_parent.parent', 'party')
     def on_change_with_price_list_used(self, name=None):
         pool = Pool()
         Configuration = pool.get('sale.configuration')
         if self.price_list:
             return self.price_list.id
         parent_project = self.__class__.search([
                 ('parent', 'parent_of', [self.id]),
```

