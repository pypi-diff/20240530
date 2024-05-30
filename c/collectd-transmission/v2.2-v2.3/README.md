# Comparing `tmp/collectd_transmission-v2.2.tar.gz` & `tmp/collectd_transmission-v2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collectd_transmission-v2.2.tar", last modified: Thu May 14 10:23:49 2015, max compression
+gzip compressed data, was "dist/collectd_transmission-v2.3.tar", last modified: Fri Sep  4 11:57:44 2015, max compression
```

## Comparing `collectd_transmission-v2.2.tar` & `collectd_transmission-v2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2015-05-14 10:23:49.000000 collectd_transmission-v2.2/
--rw-r--r--   0 alex      (1000) alex      (1000)      772 2015-05-14 10:23:49.000000 collectd_transmission-v2.2/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)      736 2015-05-14 09:10:45.000000 collectd_transmission-v2.2/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)     1849 2015-05-14 09:17:56.000000 collectd_transmission-v2.2/README.rst
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2015-05-14 10:23:49.000000 collectd_transmission-v2.2/scripts/
--rwxr-xr-x   0 alex      (1000) alex      (1000)      912 2014-12-11 12:22:49.000000 collectd_transmission-v2.2/scripts/upgrade_from_1_3_to_2_0.sh
--rw-r--r--   0 alex      (1000) alex      (1000)     3164 2015-05-14 10:23:49.000000 collectd_transmission-v2.2/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)       72 2015-05-14 09:09:51.000000 collectd_transmission-v2.2/.travis.yml
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2015-05-14 10:23:49.000000 collectd_transmission-v2.2/collectd_transmission.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)       22 2015-05-14 10:23:49.000000 collectd_transmission-v2.2/collectd_transmission.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       46 2015-05-14 10:23:49.000000 collectd_transmission-v2.2/collectd_transmission.egg-info/pbr.json
--rw-r--r--   0 alex      (1000) alex      (1000)     3164 2015-05-14 10:23:49.000000 collectd_transmission-v2.2/collectd_transmission.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2015-05-14 10:23:49.000000 collectd_transmission-v2.2/collectd_transmission.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       21 2015-05-14 10:23:49.000000 collectd_transmission-v2.2/collectd_transmission.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)      627 2015-05-14 10:23:49.000000 collectd_transmission-v2.2/collectd_transmission.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2015-05-14 09:38:30.000000 collectd_transmission-v2.2/collectd_transmission.egg-info/not-zip-safe
--rw-r--r--   0 alex      (1000) alex      (1000)       32 2015-05-14 09:09:39.000000 collectd_transmission-v2.2/test-requirements.txt
--rw-r--r--   0 alex      (1000) alex      (1000)      272 2015-05-14 10:13:15.000000 collectd_transmission-v2.2/setup.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2015-05-14 10:23:49.000000 collectd_transmission-v2.2/doc/
--rw-r--r--   0 alex      (1000) alex      (1000)      360 2015-05-14 09:32:21.000000 collectd_transmission-v2.2/doc/compatibility.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     5624 2014-12-13 21:04:20.000000 collectd_transmission-v2.2/doc/Makefile
--rw-r--r--   0 alex      (1000) alex      (1000)      172 2014-12-14 19:10:51.000000 collectd_transmission-v2.2/doc/api.rst
--rw-r--r--   0 alex      (1000) alex      (1000)      966 2014-12-14 17:45:05.000000 collectd_transmission-v2.2/doc/install.rst
--rw-r--r--   0 alex      (1000) alex      (1000)      646 2014-12-14 17:48:03.000000 collectd_transmission-v2.2/doc/intro.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     9211 2015-05-14 09:11:36.000000 collectd_transmission-v2.2/doc/conf.py
--rw-r--r--   0 alex      (1000) alex      (1000)      861 2015-05-14 09:30:03.000000 collectd_transmission-v2.2/doc/configure.rst
--rw-r--r--   0 alex      (1000) alex      (1000)      297 2014-12-14 19:09:43.000000 collectd_transmission-v2.2/doc/index.rst
--rw-r--r--   0 alex      (1000) alex      (1000)      869 2014-12-19 13:51:32.000000 collectd_transmission-v2.2/tox.ini
--rw-r--r--   0 alex      (1000) alex      (1000)       42 2015-05-14 10:23:49.000000 collectd_transmission-v2.2/AUTHORS
--rw-r--r--   0 alex      (1000) alex      (1000)       21 2014-12-16 15:33:17.000000 collectd_transmission-v2.2/requirements.txt
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2015-05-14 10:23:49.000000 collectd_transmission-v2.2/tests/
--rwxr-xr-x   0 alex      (1000) alex      (1000)     1724 2014-12-19 13:38:38.000000 collectd_transmission-v2.2/tests/tests.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1262 2015-05-14 10:23:49.000000 collectd_transmission-v2.2/ChangeLog
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2015-05-14 10:23:49.000000 collectd_transmission-v2.2/collectd_transmission/
--rwxr-xr-x   0 alex      (1000) alex      (1000)     4245 2015-05-14 08:30:27.000000 collectd_transmission-v2.2/collectd_transmission/__init__.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2015-09-04 11:57:44.000000 collectd_transmission-v2.3/
+-rw-r--r--   0 alex      (1000) alex      (1000)      772 2015-09-04 11:57:44.000000 collectd_transmission-v2.3/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1000)      736 2015-05-14 09:10:45.000000 collectd_transmission-v2.3/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)     2264 2015-09-03 18:23:27.000000 collectd_transmission-v2.3/README.rst
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2015-09-04 11:57:44.000000 collectd_transmission-v2.3/scripts/
+-rwxr-xr-x   0 alex      (1000) alex      (1000)      912 2014-12-11 12:22:49.000000 collectd_transmission-v2.3/scripts/upgrade_from_1_3_to_2_0.sh
+-rw-r--r--   0 alex      (1000) alex      (1000)     3643 2015-09-04 11:57:44.000000 collectd_transmission-v2.3/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      104 2015-08-24 08:36:34.000000 collectd_transmission-v2.3/.travis.yml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2015-09-04 11:57:44.000000 collectd_transmission-v2.3/collectd_transmission.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)       22 2015-09-04 11:57:44.000000 collectd_transmission-v2.3/collectd_transmission.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       46 2015-09-04 11:57:44.000000 collectd_transmission-v2.3/collectd_transmission.egg-info/pbr.json
+-rw-r--r--   0 alex      (1000) alex      (1000)     3643 2015-09-04 11:57:44.000000 collectd_transmission-v2.3/collectd_transmission.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2015-09-04 11:57:44.000000 collectd_transmission-v2.3/collectd_transmission.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       21 2015-09-04 11:57:44.000000 collectd_transmission-v2.3/collectd_transmission.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)      627 2015-09-04 11:57:44.000000 collectd_transmission-v2.3/collectd_transmission.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2015-09-04 11:57:44.000000 collectd_transmission-v2.3/collectd_transmission.egg-info/not-zip-safe
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2015-09-03 14:33:53.000000 collectd_transmission-v2.3/test-requirements.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)      272 2015-05-14 10:13:15.000000 collectd_transmission-v2.3/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2015-09-04 11:57:44.000000 collectd_transmission-v2.3/doc/
+-rw-r--r--   0 alex      (1000) alex      (1000)      360 2015-08-24 15:52:21.000000 collectd_transmission-v2.3/doc/compatibility.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     5624 2015-08-24 15:55:27.000000 collectd_transmission-v2.3/doc/Makefile
+-rw-r--r--   0 alex      (1000) alex      (1000)      172 2014-12-14 19:10:51.000000 collectd_transmission-v2.3/doc/api.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)      966 2014-12-14 17:45:05.000000 collectd_transmission-v2.3/doc/install.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)      700 2015-08-24 15:55:17.000000 collectd_transmission-v2.3/doc/intro.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     9211 2015-08-24 15:53:39.000000 collectd_transmission-v2.3/doc/conf.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      861 2015-05-14 09:30:03.000000 collectd_transmission-v2.3/doc/configure.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)      297 2014-12-14 19:09:43.000000 collectd_transmission-v2.3/doc/index.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     1035 2015-09-03 18:07:04.000000 collectd_transmission-v2.3/tox.ini
+-rw-r--r--   0 alex      (1000) alex      (1000)       42 2015-09-04 11:57:44.000000 collectd_transmission-v2.3/AUTHORS
+-rw-r--r--   0 alex      (1000) alex      (1000)       21 2015-08-24 07:59:45.000000 collectd_transmission-v2.3/requirements.txt
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2015-09-04 11:57:44.000000 collectd_transmission-v2.3/tests/
+-rwxr-xr-x   0 alex      (1000) alex      (1000)     1918 2015-09-04 11:46:26.000000 collectd_transmission-v2.3/tests/tests.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2143 2015-09-04 11:57:44.000000 collectd_transmission-v2.3/ChangeLog
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2015-09-04 11:57:44.000000 collectd_transmission-v2.3/collectd_transmission/
+-rwxr-xr-x   0 alex      (1000) alex      (1000)     3906 2015-09-03 21:00:09.000000 collectd_transmission-v2.3/collectd_transmission/__init__.py
```

### Comparing `collectd_transmission-v2.2/setup.cfg` & `collectd_transmission-v2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `collectd_transmission-v2.2/LICENSE` & `collectd_transmission-v2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `collectd_transmission-v2.2/README.rst` & `collectd_transmission-v2.3/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 Introduction
 ============
 
 .. image:: https://travis-ci.org/akosiaris/collectd_transmission.svg?branch=master
     :target: https://travis-ci.org/akosiaris/collectd_transmission
         :alt: Build Status
 
+.. image:: https://readthedocs.org/projects/collectd-transmission/badge/?version=latest
+    :target: https://readthedocs.org/projects/collectd-transmission/
+    :alt: Documentation Status
+
+.. image:: https://coveralls.io/repos/akosiaris/collectd_transmission/badge.svg?branch=master&service=github
+   :target: https://coveralls.io/github/akosiaris/collectd_transmission?branch=master
+   :alt: Code Coverage Status
+
 A python plugin for integrating collectd and transmission. With this
 installed, collectd will be querying transmission for the following:
 
 Per session and cumulative:
 
 * downloadedBytes
 * uploadedBytes
```

### Comparing `collectd_transmission-v2.2/scripts/upgrade_from_1_3_to_2_0.sh` & `collectd_transmission-v2.3/scripts/upgrade_from_1_3_to_2_0.sh`

 * *Files identical despite different names*

### Comparing `collectd_transmission-v2.2/PKG-INFO` & `collectd_transmission-v2.3/collectd_transmission.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 Metadata-Version: 1.1
-Name: collectd_transmission
-Version: v2.2
+Name: collectd-transmission
+Version: v2.3
 Summary: A python plugin for collectd to get stats from a runnning transmission server.
 Home-page: https://github.com/akosiaris/collectd_transmission
 Author: Alexandros Kosiaris
 Author-email: akosiaris@gmail.com
 License: 'ISC'
 Description: Introduction
         ============
         
         .. image:: https://travis-ci.org/akosiaris/collectd_transmission.svg?branch=master
             :target: https://travis-ci.org/akosiaris/collectd_transmission
                 :alt: Build Status
         
+        .. image:: https://readthedocs.org/projects/collectd-transmission/badge/?version=latest
+            :target: https://readthedocs.org/projects/collectd-transmission/
+            :alt: Documentation Status
+        
+        .. image:: https://coveralls.io/repos/akosiaris/collectd_transmission/badge.svg?branch=master&service=github
+           :target: https://coveralls.io/github/akosiaris/collectd_transmission?branch=master
+           :alt: Code Coverage Status
+        
         A python plugin for integrating collectd and transmission. With this
         installed, collectd will be querying transmission for the following:
         
         Per session and cumulative:
         
         * downloadedBytes
         * uploadedBytes
```

### Comparing `collectd_transmission-v2.2/collectd_transmission.egg-info/PKG-INFO` & `collectd_transmission-v2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 Metadata-Version: 1.1
-Name: collectd-transmission
-Version: v2.2
+Name: collectd_transmission
+Version: v2.3
 Summary: A python plugin for collectd to get stats from a runnning transmission server.
 Home-page: https://github.com/akosiaris/collectd_transmission
 Author: Alexandros Kosiaris
 Author-email: akosiaris@gmail.com
 License: 'ISC'
 Description: Introduction
         ============
         
         .. image:: https://travis-ci.org/akosiaris/collectd_transmission.svg?branch=master
             :target: https://travis-ci.org/akosiaris/collectd_transmission
                 :alt: Build Status
         
+        .. image:: https://readthedocs.org/projects/collectd-transmission/badge/?version=latest
+            :target: https://readthedocs.org/projects/collectd-transmission/
+            :alt: Documentation Status
+        
+        .. image:: https://coveralls.io/repos/akosiaris/collectd_transmission/badge.svg?branch=master&service=github
+           :target: https://coveralls.io/github/akosiaris/collectd_transmission?branch=master
+           :alt: Code Coverage Status
+        
         A python plugin for integrating collectd and transmission. With this
         installed, collectd will be querying transmission for the following:
         
         Per session and cumulative:
         
         * downloadedBytes
         * uploadedBytes
```

### Comparing `collectd_transmission-v2.2/collectd_transmission.egg-info/SOURCES.txt` & `collectd_transmission-v2.3/collectd_transmission.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collectd_transmission-v2.2/doc/Makefile` & `collectd_transmission-v2.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `collectd_transmission-v2.2/doc/install.rst` & `collectd_transmission-v2.3/doc/install.rst`

 * *Files identical despite different names*

### Comparing `collectd_transmission-v2.2/doc/conf.py` & `collectd_transmission-v2.3/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 #modindex_common_prefix = []
 
 
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'default'
+html_theme = 'classic'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
```

### Comparing `collectd_transmission-v2.2/doc/configure.rst` & `collectd_transmission-v2.3/doc/configure.rst`

 * *Files identical despite different names*

### Comparing `collectd_transmission-v2.2/tox.ini` & `collectd_transmission-v2.3/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [tox]
 ; flake8 includes both pep8 and pyflakes :]
-envlist = py27,flake8,doc,coverage
+envlist = py27-transmissionrpc{_lt_09,_ge_09},py33,py34,flake8,doc,coverage
 
 ;
 ; test environnements
 ;
 [testenv]
 setenv = VIRTUAL_ENV={envdir}
          LANG=en_US.UTF-8
          LANGUAGE=en_US:en
          LC_ALL=C
+passenv = TRAVIS TRAVIS_JOB_ID TRAVIS_BRANCH
 install_command = pip install {opts} {packages}
-deps = -r{toxinidir}/requirements.txt
-       -r{toxinidir}/test-requirements.txt
-commands = python tests/tests.py
-
-[testenv:venv]
-commands = {posargs}
+deps = -r{toxinidir}/test-requirements.txt
+       transmissionrpc_lt_09: transmissionrpc>=0.8,<0.9
+       transmissionrpc_ge_09: transmissionrpc>=0.9
+commands = python -m coverage run --parallel-mode --source collectd_transmission tests/tests.py
 
 [testenv:flake8]
 commands = flake8 collectd_transmission
 
 [testenv:coverage]
-commands = python -m coverage run tests/tests.py
+commands = python -m coverage combine
            python -m coverage html
-whitelist_externals = cp
+           coveralls
 
 [testenv:doc]
 commands = python setup.py build_sphinx --builder html
            python setup.py build_sphinx --builder text
 
 ;
 ; Commands configuration
```

### Comparing `collectd_transmission-v2.2/tests/tests.py` & `collectd_transmission-v2.3/tests/tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #!/usr/bin/env python
 
 import unittest
 import mock
 import sys
 
-sys.path.append('..')
-
+# Monkey patching the collectd module to facilitate testing
+mock_collectd = mock.MagicMock()
+sys.modules['collectd'] = mock_collectd
+
+# This is a hack to force tests to use the in-repo version of the module and not
+# the one installed by tox
+sys.path.insert(0, '.')
 import collectd_transmission
 
 
-# A Monkey object to make our lives easier. We want to avoid including
-# collectd module which is why all the fuss
-class MonkeyObject(object):
-    pass
-
-
 class MethodTestCase(unittest.TestCase):
     def setUp(self):
-        self.config = MonkeyObject()
+        # Mock our configuration to enable testing
+        self.config = mock.Mock()
         self.config.children = []
-        child1 = MonkeyObject()
+        child1 = mock.Mock()
         child1.key = 'username'
         child1.values = ['myusername']
-        child2 = MonkeyObject()
+        child2 = mock.Mock()
         child2.key = 'password'
         child2.values = ['mypassword']
 
         self.config.children.append(child1)
         self.config.children.append(child2)
 
     def tearDown(self):
@@ -49,12 +49,13 @@
         collectd_transmission.shutdown()
 
     @mock.patch('collectd_transmission.transmissionrpc.Client')
     def test_get_stats(self, mock_Client):
         collectd_transmission.collectd = mock.MagicMock()
         collectd_transmission.config(self.config)
         collectd_transmission.initialize()
+        collectd_transmission.data['client'] = mock_Client
         collectd_transmission.get_stats()
-        mock_Client.session_status.assert_called()
+        mock_Client.session_stats.assert_called_with()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `collectd_transmission-v2.2/collectd_transmission/__init__.py` & `collectd_transmission-v2.3/collectd_transmission/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,15 @@
 # -*- coding: utf-8 -*- vim:fileencoding=utf-8:
 # vim: tabstop=4:shiftwidth=4:softtabstop=4:expandtab
 
 '''
 ..  moduleauthor:: Alexandros Kosiaris
 '''
 
-# The collectd module is injected on the fly in the namespace by
-# collectd. Depending on it to exist while testing is impossible
-try:
-    import collectd
-    successimport = True
-except ImportError:
-    successimport = False
-
-# These on the other hand are expected to be there
+import collectd
 import transmissionrpc
 from distutils.version import StrictVersion
 
 PLUGIN_NAME = 'transmission'
 
 data = {}
 metrics = {
@@ -102,27 +94,23 @@
     '''
     # 0.9 and onwards have statistics in a different field
     if StrictVersion(data['client_version']) >= StrictVersion('0.9'):
         if category == 'cumulative':
             return stats.cumulative_stats[key]
         elif category == 'current':
             return stats.current_stats[key]
-        elif category == 'general':
+        else:  # We are in "general"
             return getattr(stats, key)
-        else:
-            return 0
     else:
         if category == 'cumulative':
             return stats.fields['cumulative_stats'][key]
         elif category == 'current':
             return stats.fields['current_stats'][key]
-        elif category == 'general':
+        else:  # We are in "general"
             return stats.fields[key]
-        else:
-            return 0
 
 
 def get_stats():
     '''
     Collectd routine to actually get and dispatch the statistics
     '''
     stats = data['client'].session_stats()
@@ -130,12 +118,12 @@
     for category, catmetrics in metrics.items():
         for metric, attrs in catmetrics.items():
             vl = collectd.Values(type=attrs['type'],
                                  plugin=PLUGIN_NAME,
                                  type_instance='%s-%s' % (category, metric))
             vl.dispatch(values=[field_getter(stats, metric, category)])
 
-if successimport:
-    collectd.register_config(config)
-    collectd.register_init(initialize)
-    collectd.register_read(get_stats)
-    collectd.register_shutdown(shutdown)
+# Register our functions
+collectd.register_config(config)
+collectd.register_init(initialize)
+collectd.register_read(get_stats)
+collectd.register_shutdown(shutdown)
```

