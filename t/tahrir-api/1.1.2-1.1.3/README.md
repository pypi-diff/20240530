# Comparing `tmp/tahrir_api-1.1.2.tar.gz` & `tmp/tahrir_api-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahrir_api-1.1.2.tar", max compression
+gzip compressed data, was "tahrir_api-1.1.3.tar", max compression
```

## Comparing `tahrir_api-1.1.2.tar` & `tahrir_api-1.1.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    35147 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/LICENSE
--rw-r--r--   0        0        0     2510 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/README.rst
--rw-r--r--   0        0        0      273 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/examples/awardbadge.py
--rw-r--r--   0        0        0      519 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/examples/fossboxbadge.py
--rw-r--r--   0        0        0     2266 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/tahrir_api/__init__.py
--rw-r--r--   0        0        0    31058 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/tahrir_api/dbapi.py
--rw-r--r--   0        0        0      154 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/tahrir_api/migrations/README
--rw-r--r--   0        0        0      946 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/tahrir_api/migrations/alembic.ini
--rw-r--r--   0        0        0     2121 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/tahrir_api/migrations/env.py
--rw-r--r--   0        0        0      532 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/tahrir_api/migrations/script.py.mako
--rw-r--r--   0        0        0      432 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/tahrir_api/migrations/versions/139ec7ed17b7_add_a_rank_column_to.py
--rw-r--r--   0        0        0      445 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/tahrir_api/migrations/versions/16943d9088cf_fix_foreign_key_mism.py
--rw-r--r--   0        0        0      609 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/tahrir_api/migrations/versions/24282792d72a_add_created_by_field.py
--rw-r--r--   0        0        0      490 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/tahrir_api/migrations/versions/2879ed5a6297_issued_for.py
--rw-r--r--   0        0        0      707 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/migrations/versions/39583332f4ea_add_profile_fields_t.py
--rw-r--r--   0        0        0     1037 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/migrations/versions/3c7fd5b4e2c2_add_two_new_columns_.py
--rw-r--r--   0        0        0      466 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/migrations/versions/3d3fb9e59e7b_add_person_avatar.py
--rw-r--r--   0        0        0      618 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/migrations/versions/4099fa344171_add_last_login.py
--rw-r--r--   0        0        0      507 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/migrations/versions/420c02357a1b_add_created_on_field.py
--rw-r--r--   0        0        0      510 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/migrations/versions/508367dcbbb5_add_an_stl_column_fo.py
--rw-r--r--   0        0        0      500 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/migrations/versions/5791a2b9fb6a_add_tags_field_to_ba.py
--rw-r--r--   0        0        0      735 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/migrations/versions/ce541796a7_add_authz_table.py
--rw-r--r--   0        0        0     2429 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/migrations/versions/e7040e76728_create_new_tables_for_quest.py
--rw-r--r--   0        0        0      526 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/migrations/versions/fa1d309e8c3_add_created_on_field.py
--rw-r--r--   0        0        0     9769 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/model.py
--rw-r--r--   0        0        0        0 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/scripts/__init__.py
--rw-r--r--   0        0        0     1711 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/scripts/populate_avatars.py
--rw-r--r--   0        0        0     2705 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/scripts/populateseries.py
--rw-r--r--   0        0        0      383 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/scripts/syncdb.py
--rw-r--r--   0        0        0     1443 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/scripts/utils.py
--rw-r--r--   0        0        0      838 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/utils.py
--rw-r--r--   0        0        0        0 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tests/__init__.py
--rw-r--r--   0        0        0      408 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tests/conftest.py
--rw-r--r--   0        0        0     6156 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tests/test_dbapi.py
--rw-r--r--   0        0        0     4909 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tests/test_ranking.py
--rw-r--r--   0        0        0     3937 1970-01-01 00:00:00.000000 tahrir_api-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35147 2024-05-30 08:08:00.651746 tahrir_api-1.1.3/LICENSE
+-rw-r--r--   0        0        0     2510 2024-05-30 08:08:00.651746 tahrir_api-1.1.3/README.rst
+-rw-r--r--   0        0        0      273 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/examples/awardbadge.py
+-rw-r--r--   0        0        0      519 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/examples/fossboxbadge.py
+-rw-r--r--   0        0        0     2266 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/tahrir_api/__init__.py
+-rw-r--r--   0        0        0    30822 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/tahrir_api/dbapi.py
+-rw-r--r--   0        0        0      154 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/tahrir_api/migrations/README
+-rw-r--r--   0        0        0      946 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/tahrir_api/migrations/alembic.ini
+-rw-r--r--   0        0        0     2121 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/tahrir_api/migrations/env.py
+-rw-r--r--   0        0        0      532 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/tahrir_api/migrations/script.py.mako
+-rw-r--r--   0        0        0      432 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/tahrir_api/migrations/versions/139ec7ed17b7_add_a_rank_column_to.py
+-rw-r--r--   0        0        0      445 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/tahrir_api/migrations/versions/16943d9088cf_fix_foreign_key_mism.py
+-rw-r--r--   0        0        0      609 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/tahrir_api/migrations/versions/24282792d72a_add_created_by_field.py
+-rw-r--r--   0        0        0      490 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/tahrir_api/migrations/versions/2879ed5a6297_issued_for.py
+-rw-r--r--   0        0        0      707 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/tahrir_api/migrations/versions/39583332f4ea_add_profile_fields_t.py
+-rw-r--r--   0        0        0     1037 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/tahrir_api/migrations/versions/3c7fd5b4e2c2_add_two_new_columns_.py
+-rw-r--r--   0        0        0      466 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/tahrir_api/migrations/versions/3d3fb9e59e7b_add_person_avatar.py
+-rw-r--r--   0        0        0      618 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/tahrir_api/migrations/versions/4099fa344171_add_last_login.py
+-rw-r--r--   0        0        0      507 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/tahrir_api/migrations/versions/420c02357a1b_add_created_on_field.py
+-rw-r--r--   0        0        0      510 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/tahrir_api/migrations/versions/508367dcbbb5_add_an_stl_column_fo.py
+-rw-r--r--   0        0        0      500 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/tahrir_api/migrations/versions/5791a2b9fb6a_add_tags_field_to_ba.py
+-rw-r--r--   0        0        0      735 2024-05-30 08:08:00.655746 tahrir_api-1.1.3/tahrir_api/migrations/versions/ce541796a7_add_authz_table.py
+-rw-r--r--   0        0        0     2429 2024-05-30 08:08:00.659746 tahrir_api-1.1.3/tahrir_api/migrations/versions/e7040e76728_create_new_tables_for_quest.py
+-rw-r--r--   0        0        0      526 2024-05-30 08:08:00.659746 tahrir_api-1.1.3/tahrir_api/migrations/versions/fa1d309e8c3_add_created_on_field.py
+-rw-r--r--   0        0        0     9769 2024-05-30 08:08:00.659746 tahrir_api-1.1.3/tahrir_api/model.py
+-rw-r--r--   0        0        0        0 2024-05-30 08:08:00.659746 tahrir_api-1.1.3/tahrir_api/scripts/__init__.py
+-rw-r--r--   0        0        0     1711 2024-05-30 08:08:00.659746 tahrir_api-1.1.3/tahrir_api/scripts/populate_avatars.py
+-rw-r--r--   0        0        0     2705 2024-05-30 08:08:00.659746 tahrir_api-1.1.3/tahrir_api/scripts/populateseries.py
+-rw-r--r--   0        0        0      383 2024-05-30 08:08:00.659746 tahrir_api-1.1.3/tahrir_api/scripts/syncdb.py
+-rw-r--r--   0        0        0     1176 2024-05-30 08:08:00.659746 tahrir_api-1.1.3/tahrir_api/scripts/utils.py
+-rw-r--r--   0        0        0     1197 2024-05-30 08:08:00.659746 tahrir_api-1.1.3/tahrir_api/utils.py
+-rw-r--r--   0        0        0        0 2024-05-30 08:08:00.659746 tahrir_api-1.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      508 2024-05-30 08:08:00.659746 tahrir_api-1.1.3/tests/conftest.py
+-rw-r--r--   0        0        0     6156 2024-05-30 08:08:00.659746 tahrir_api-1.1.3/tests/test_dbapi.py
+-rw-r--r--   0        0        0     4909 2024-05-30 08:08:00.659746 tahrir_api-1.1.3/tests/test_ranking.py
+-rw-r--r--   0        0        0     3937 1970-01-01 00:00:00.000000 tahrir_api-1.1.3/PKG-INFO
```

### Comparing `tahrir_api-1.1.2/LICENSE` & `tahrir_api-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.2/README.rst` & `tahrir_api-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.2/examples/fossboxbadge.py` & `tahrir_api-1.1.3/examples/fossboxbadge.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.2/pyproject.toml` & `tahrir_api-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tahrir-api"
-version = "1.1.2"
+version = "1.1.3"
 description = "An API for interacting with the Tahrir database"
 
 license = "GPLv3+"
 
 authors = [
   "Ross Delinger <rdelinge@redhat.com>",
   "Fedora Infrastructure <admin@fedoraproject.org>",
```

### Comparing `tahrir_api-1.1.2/tahrir_api/dbapi.py` & `tahrir_api-1.1.3/tahrir_api/dbapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 # Authors: Ross Delinger
 #          Remy D <remyd@civx.us>
 # Description: API For interacting with the Tahrir database
 
-import importlib.resources
 from collections import OrderedDict
 from datetime import datetime, timedelta, timezone
 
 from sqlalchemy import and_, func, not_, text
-from sqlalchemy_helpers import DatabaseManager
 from tahrir_messages import BadgeAwardV1, PersonLoginFirstV1, PersonRankAdvanceV1
 
 from .model import (
     Assertion,
     Authorization,
     Badge,
     Invitation,
     Issuer,
     Milestone,
     Person,
     Series,
     Team,
 )
-from .utils import autocommit, convert_name_to_id
+from .utils import autocommit, convert_name_to_id, get_db_manager_from_uri
 
 
 class TahrirDatabase:
     """
     Class for talking to the Tahrir database
     It handles adding information necessary to issue open badges
 
@@ -44,19 +42,16 @@
 
         if dburi and session:
             raise ValueError("Provide only one, either 'dburi' or 'session'")
 
         self.autocommit = autocommit
 
         if dburi:
-            with importlib.resources.as_file(
-                importlib.resources.files("tahrir_api").joinpath("migrations")
-            ) as alembic_path:
-                self.db_mgr = DatabaseManager(dburi, alembic_path.as_posix())
-            self.session = self.db_mgr.Session()
+            db_mgr = get_db_manager_from_uri(dburi)
+            self.session = db_mgr.Session()
         else:
             self.session = session
 
         self.notification_callback = notification_callback
 
     def team_exists(self, team_id):
         """
```

### Comparing `tahrir_api-1.1.2/tahrir_api/migrations/alembic.ini` & `tahrir_api-1.1.3/tahrir_api/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.2/tahrir_api/migrations/env.py` & `tahrir_api-1.1.3/tahrir_api/migrations/env.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.2/tahrir_api/migrations/script.py.mako` & `tahrir_api-1.1.3/tahrir_api/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.2/tahrir_api/migrations/versions/24282792d72a_add_created_by_field.py` & `tahrir_api-1.1.3/tahrir_api/migrations/versions/24282792d72a_add_created_by_field.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.2/tahrir_api/migrations/versions/39583332f4ea_add_profile_fields_t.py` & `tahrir_api-1.1.3/tahrir_api/migrations/versions/39583332f4ea_add_profile_fields_t.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.2/tahrir_api/migrations/versions/3c7fd5b4e2c2_add_two_new_columns_.py` & `tahrir_api-1.1.3/tahrir_api/migrations/versions/3c7fd5b4e2c2_add_two_new_columns_.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.2/tahrir_api/migrations/versions/4099fa344171_add_last_login.py` & `tahrir_api-1.1.3/tahrir_api/migrations/versions/4099fa344171_add_last_login.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.2/tahrir_api/migrations/versions/ce541796a7_add_authz_table.py` & `tahrir_api-1.1.3/tahrir_api/migrations/versions/ce541796a7_add_authz_table.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.2/tahrir_api/migrations/versions/e7040e76728_create_new_tables_for_quest.py` & `tahrir_api-1.1.3/tahrir_api/migrations/versions/e7040e76728_create_new_tables_for_quest.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.2/tahrir_api/migrations/versions/fa1d309e8c3_add_created_on_field.py` & `tahrir_api-1.1.3/tahrir_api/migrations/versions/fa1d309e8c3_add_created_on_field.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.2/tahrir_api/model.py` & `tahrir_api-1.1.3/tahrir_api/model.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.2/tahrir_api/scripts/populate_avatars.py` & `tahrir_api-1.1.3/tahrir_api/scripts/populate_avatars.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.2/tahrir_api/scripts/populateseries.py` & `tahrir_api-1.1.3/tahrir_api/scripts/populateseries.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.2/tests/test_dbapi.py` & `tahrir_api-1.1.3/tests/test_dbapi.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.2/tests/test_ranking.py` & `tahrir_api-1.1.3/tests/test_ranking.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.2/PKG-INFO` & `tahrir_api-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahrir-api
-Version: 1.1.2
+Version: 1.1.3
 Summary: An API for interacting with the Tahrir database
 Home-page: https://github.com/fedora-infra/tahrir-api
 License: GPLv3+
 Author: Ross Delinger
 Author-email: rdelinge@redhat.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Framework :: Pyramid
```

