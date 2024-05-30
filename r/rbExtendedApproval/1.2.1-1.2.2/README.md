# Comparing `tmp/rbextendedapproval-1.2.1.tar.gz` & `tmp/rbextendedapproval-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbextendedapproval-1.2.1.tar", last modified: Thu May 30 11:30:17 2024, max compression
+gzip compressed data, was "rbextendedapproval-1.2.2.tar", last modified: Thu May 30 14:43:23 2024, max compression
```

## Comparing `rbextendedapproval-1.2.1.tar` & `rbextendedapproval-1.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:30:17.660168 rbextendedapproval-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-30 11:29:49.000000 rbextendedapproval-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-30 11:30:17.660168 rbextendedapproval-1.2.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:30:17.656168 rbextendedapproval-1.2.1/extended_approval/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 11:29:49.000000 rbextendedapproval-1.2.1/extended_approval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-30 11:29:49.000000 rbextendedapproval-1.2.1/extended_approval/admin_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    16318 2024-05-30 11:29:49.000000 rbextendedapproval-1.2.1/extended_approval/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-30 11:29:49.000000 rbextendedapproval-1.2.1/extended_approval/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:30:17.660168 rbextendedapproval-1.2.1/rbExtendedApproval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-30 11:30:17.000000 rbextendedapproval-1.2.1/rbExtendedApproval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-30 11:30:17.000000 rbextendedapproval-1.2.1/rbExtendedApproval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:30:17.000000 rbextendedapproval-1.2.1/rbExtendedApproval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-30 11:30:17.000000 rbextendedapproval-1.2.1/rbExtendedApproval.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:30:17.000000 rbextendedapproval-1.2.1/rbExtendedApproval.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 11:30:17.000000 rbextendedapproval-1.2.1/rbExtendedApproval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 11:30:17.000000 rbextendedapproval-1.2.1/rbExtendedApproval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 11:30:17.660168 rbextendedapproval-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-30 11:29:49.000000 rbextendedapproval-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:43:23.331314 rbextendedapproval-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-30 14:42:53.000000 rbextendedapproval-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-30 14:43:23.331314 rbextendedapproval-1.2.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:43:23.331314 rbextendedapproval-1.2.2/extended_approval/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:42:53.000000 rbextendedapproval-1.2.2/extended_approval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-30 14:42:53.000000 rbextendedapproval-1.2.2/extended_approval/admin_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17468 2024-05-30 14:42:53.000000 rbextendedapproval-1.2.2/extended_approval/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-30 14:42:53.000000 rbextendedapproval-1.2.2/extended_approval/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:43:23.331314 rbextendedapproval-1.2.2/rbExtendedApproval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-30 14:43:23.000000 rbextendedapproval-1.2.2/rbExtendedApproval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-30 14:43:23.000000 rbextendedapproval-1.2.2/rbExtendedApproval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:43:23.000000 rbextendedapproval-1.2.2/rbExtendedApproval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-30 14:43:23.000000 rbextendedapproval-1.2.2/rbExtendedApproval.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:43:23.000000 rbextendedapproval-1.2.2/rbExtendedApproval.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 14:43:23.000000 rbextendedapproval-1.2.2/rbExtendedApproval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 14:43:23.000000 rbextendedapproval-1.2.2/rbExtendedApproval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 14:43:23.331314 rbextendedapproval-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-30 14:42:53.000000 rbextendedapproval-1.2.2/setup.py
```

### Comparing `rbextendedapproval-1.2.1/LICENSE` & `rbextendedapproval-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rbextendedapproval-1.2.1/PKG-INFO` & `rbextendedapproval-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbExtendedApproval
-Version: 1.2.1
+Version: 1.2.2
 Summary: Review Board extension: ExtendedApproval
 Home-page: https://github.com/misery/ExtendedApproval
 Author: Andre Klitzing
 Author-email: aklitzing@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Review Board
 Classifier: Intended Audience :: Developers
```

### Comparing `rbextendedapproval-1.2.1/extended_approval/extension.py` & `rbextendedapproval-1.2.2/extended_approval/extension.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,14 @@
-import pytz
 from datetime import datetime, timedelta
+try:
+    from datetime import UTC
+    def nowUtc(): return datetime.now(UTC)
+except ImportError:
+    import pytz
+    def nowUtc(): return datetime.utcnow().replace(tzinfo=pytz.utc)
 
 from djblets.datagrid.grids import Column
 
 from django.utils.html import format_html
 from django.utils.safestring import mark_safe
 from django.utils.translation import ugettext_lazy as _
 
@@ -29,14 +34,16 @@
 CONFIG_ENABLE_REVOKE_SHIPITS = 'enable_revoke_shipits'
 CONFIG_ENABLE_TARGET_SHIPITS = 'enable_target_shipits'
 CONFIG_ENABLE_LEGACY_BUTTONS = 'enable_legacy_buttons'
 CONFIG_ENABLE_WAIT_IT_BUTTON = 'enable_wait_it_button'
 CONFIG_FORBIDDEN_USER_SHIPITS = 'forbidden_user_shipits'
 CONFIG_FORBIDDEN_APPROVE_PREFIXES = 'forbidden_approve_prefixes'
 CONFIG_FORBIDDEN_APPROVE_PREFIXES_DICT = 'forbidden_approve_prefixes_dict'
+CONFIG_FORBIDDEN_APPROVE_SUFFIXES = 'forbidden_approve_suffixes'
+CONFIG_FORBIDDEN_APPROVE_SUFFIXES_DICT = 'forbidden_approve_suffixes_dict'
 
 
 class ReqReviews(object):
     def __init__(self, r):
         self.request = r
         self.diffset = r.get_latest_diffset()
         self.total = []
@@ -100,16 +107,15 @@
     if period is None:
         return obj.timestamp
 
     return obj.timestamp + timedelta(0, period)
 
 
 def check_grace_period(settings, diffset, shipit):
-    now = datetime.utcnow().replace(tzinfo=pytz.utc)
-
+    now = nowUtc()
     epoch = calc_epoch(settings, CONFIG_GRACE_PERIOD_DIFFSET, diffset)
     if epoch > now:
         return ('Grace period for latest diff is not reached: %s'
                 % epoch.strftime("%x %X %Z"))
 
     epoch = calc_epoch(settings, CONFIG_GRACE_PERIOD_SHIPIT, shipit)
     if epoch > now:
@@ -167,14 +173,22 @@
         for key, value in prefixes.items():
             if review_request.summary.startswith(key):
                 return self._render([{
                         'icon_name': 'issue-dropped',
                         'title': _(value),
                 }])
 
+        suffixes = self.settings[CONFIG_FORBIDDEN_APPROVE_SUFFIXES_DICT]
+        for key, value in suffixes.items():
+            if review_request.summary.endswith(key):
+                return self._render([{
+                        'icon_name': 'issue-dropped',
+                        'title': _(value),
+                }])
+
         r = ReqReviews(review_request)
         if len(r.getTotal()) > 0 or len(r.getRevoked()) > 0:
             if len(r.getLatest()) > 0:
                 period = check_grace_period(self.settings, r.getDiffset(),
                                             r.getLatest()[0])
 
                 if period is not None:
@@ -221,14 +235,19 @@
             return False, 'The review request has open issues'
 
         prefixes = self.settings[CONFIG_FORBIDDEN_APPROVE_PREFIXES_DICT]
         for key, value in prefixes.items():
             if review_request.summary.startswith(key):
                 return False, 'The review request is marked as "%s"' % value
 
+        suffixes = self.settings[CONFIG_FORBIDDEN_APPROVE_SUFFIXES_DICT]
+        for key, value in suffixes.items():
+            if review_request.summary.endswith(key):
+                return False, 'The review request is marked as "%s"' % value
+
         if not prev_approved:
             return False, prev_failure
 
         r = ReqReviews(review_request)
         if len(r.getLatest()) == 0:
             return False, 'The latest diff has not been marked' \
                           ' "Ship It!" by someone else'
@@ -385,14 +404,16 @@
         CONFIG_ENABLE_REVOKE_SHIPITS: False,
         CONFIG_ENABLE_TARGET_SHIPITS: False,
         CONFIG_ENABLE_LEGACY_BUTTONS: False,
         # CONFIG_ENABLE_WAIT_IT_BUTTON: False,
         CONFIG_FORBIDDEN_USER_SHIPITS: '',
         CONFIG_FORBIDDEN_APPROVE_PREFIXES: 'WIP|work in progress',
         CONFIG_FORBIDDEN_APPROVE_PREFIXES_DICT: None,
+        CONFIG_FORBIDDEN_APPROVE_SUFFIXES: '',
+        CONFIG_FORBIDDEN_APPROVE_SUFFIXES_DICT: None,
     }
 
     def initialize(self):
         ConfigurableApprovalHook(self)
 
         columns = [ApprovalColumn(self, id='approved')]
         DataGridColumnsHook(self, ReviewRequestDataGrid, columns)
@@ -405,22 +426,28 @@
             AdvancedPingItAction(self.settings),
             AdvancedLegacyEditReviewAction(self.settings),
             AdvancedLegacyAddGeneralCommentAction(self.settings),
             AdvancedLegacyShipItAction(self.settings),
             # AdvancedLegacyWaitItAction(self.settings),
         ])
 
-        prefixDict = {}
-        prefixSettings = self.settings.get(CONFIG_FORBIDDEN_APPROVE_PREFIXES)
-        for entry in prefixSettings.splitlines():
+        self._init_dict(CONFIG_FORBIDDEN_APPROVE_PREFIXES,
+                        CONFIG_FORBIDDEN_APPROVE_PREFIXES_DICT)
+
+        self._init_dict(CONFIG_FORBIDDEN_APPROVE_SUFFIXES,
+                        CONFIG_FORBIDDEN_APPROVE_SUFFIXES_DICT)
+
+    def _init_dict(self, configName, configNameDict):
+        entries = {}
+        for entry in self.settings.get(configName).splitlines():
             lineSplit = entry.split('|', 1)
-            prefixDict[lineSplit[0]] = (lineSplit[1]
-                                        if len(lineSplit) > 1
-                                        else lineSplit[0])
-        self.settings[CONFIG_FORBIDDEN_APPROVE_PREFIXES_DICT] = prefixDict
+            entries[lineSplit[0]] = (lineSplit[1]
+                                     if len(lineSplit) > 1
+                                     else lineSplit[0])
+        self.settings[configNameDict] = entries
 
     def shutdown(self):
         super(ExtendedApproval, self).shutdown()
 
     def _revoke_shipits(self, reviews, request):
         for r in reviews:
             r.revoke_ship_it(request.owner)
```

### Comparing `rbextendedapproval-1.2.1/extended_approval/forms.py` & `rbextendedapproval-1.2.2/extended_approval/forms.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,12 +35,20 @@
     forbidden_user_shipits = CharField(
         required=False,
         label='User who can never ShipIt',
         help_text='Comma separated list of usernames.')
 
     forbidden_approve_prefixes = CharField(
         required=False,
-        label='Non approval commit message prefixes',
+        label='Non approvable commit message prefixes',
         help_text='A prefix per line separated optionally '
                   'by a | for a comment. '
                   'Example: WIP|work in progress',
         widget=Textarea(attrs={'cols': '80', 'rows': '10'}))
+
+    forbidden_approve_suffixes = CharField(
+        required=False,
+        label='Non approvable commit message suffixes',
+        help_text='A suffix per line separated optionally '
+                  'by a | for a comment. '
+                  'Example: (Topic)|Topics cannot be published',
+        widget=Textarea(attrs={'cols': '80', 'rows': '10'}))
```

### Comparing `rbextendedapproval-1.2.1/rbExtendedApproval.egg-info/PKG-INFO` & `rbextendedapproval-1.2.2/rbExtendedApproval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbExtendedApproval
-Version: 1.2.1
+Version: 1.2.2
 Summary: Review Board extension: ExtendedApproval
 Home-page: https://github.com/misery/ExtendedApproval
 Author: Andre Klitzing
 Author-email: aklitzing@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Review Board
 Classifier: Intended Audience :: Developers
```

### Comparing `rbextendedapproval-1.2.1/setup.py` & `rbextendedapproval-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from reviewboard.extensions.packaging import setup
 
 
 PACKAGE = "rbExtendedApproval"
-VERSION = "1.2.1"
+VERSION = "1.2.2"
 
 setup(
     name=PACKAGE,
     version=VERSION,
     description='Review Board extension: ExtendedApproval',
     author='Andre Klitzing',
     author_email='aklitzing@gmail.com',
```

