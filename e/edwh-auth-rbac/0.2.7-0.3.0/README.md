# Comparing `tmp/edwh_auth_rbac-0.2.7.tar.gz` & `tmp/edwh_auth_rbac-0.3.0.tar.gz`

## Comparing `edwh_auth_rbac-0.2.7.tar` & `edwh_auth_rbac-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/CHANGELOG.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/.gitignore
--rw-r--r--   0        0        0     9928 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/class_index.html
--rw-r--r--   0        0        0    24699 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/coverage_html_cb_da166b87.js
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/favicon_32_cb_58284776.png
--rw-r--r--   0        0        0    36693 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/function_index.html
--rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/keybd_closed_cb_ce680311.png
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/status.json
--rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/style_cb_8e611ae1.css
--rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/z_438b44bce6437be6___init___py.html
--rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/z_438b44bce6437be6_helpers_py.html
--rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/z_438b44bce6437be6_migrations_py.html
--rw-r--r--   0        0        0   109622 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/z_438b44bce6437be6_model_py.html
--rw-r--r--   0        0        0    61317 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/z_438b44bce6437be6_rbac_py.html
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/z_a44f0ac069e85531___init___py.html
--rw-r--r--   0        0        0    59418 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/htmlcov/z_a44f0ac069e85531_test_rbac_py.html
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/src/edwh_auth_rbac/__init__.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/src/edwh_auth_rbac/helpers.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/src/edwh_auth_rbac/migrations.py
--rw-r--r--   0        0        0    14285 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/src/edwh_auth_rbac/model.py
--rw-r--r--   0        0        0     8098 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/src/edwh_auth_rbac/rbac.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/tests/__init__.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/tests/test_migrate.py
--rw-r--r--   0        0        0     7070 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/tests/test_rbac.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/.gitignore
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/README.md
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0     9928 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/class_index.html
+-rw-r--r--   0        0        0    24699 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/coverage_html_cb_da166b87.js
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/favicon_32_cb_58284776.png
+-rw-r--r--   0        0        0    36693 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/function_index.html
+-rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/keybd_closed_cb_ce680311.png
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/status.json
+-rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/style_cb_8e611ae1.css
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/z_438b44bce6437be6___init___py.html
+-rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/z_438b44bce6437be6_helpers_py.html
+-rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/z_438b44bce6437be6_migrations_py.html
+-rw-r--r--   0        0        0   109622 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/z_438b44bce6437be6_model_py.html
+-rw-r--r--   0        0        0    61317 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/z_438b44bce6437be6_rbac_py.html
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/z_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0    59418 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/htmlcov/z_a44f0ac069e85531_test_rbac_py.html
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/src/edwh_auth_rbac/__init__.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/src/edwh_auth_rbac/helpers.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/src/edwh_auth_rbac/migrations.py
+-rw-r--r--   0        0        0    14401 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/src/edwh_auth_rbac/model.py
+-rw-r--r--   0        0        0     8098 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/src/edwh_auth_rbac/rbac.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/tests/test_migrate.py
+-rw-r--r--   0        0        0     7778 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/tests/test_rbac.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/.gitignore
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/README.md
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.3.0/PKG-INFO
```

### Comparing `edwh_auth_rbac-0.2.7/CHANGELOG.md` & `edwh_auth_rbac-0.3.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.3.0 (2024-05-29)
+
+### Feature
+
+* Allow '*' privileges ([`2980fe1`](https://github.com/educationwarehouse/edwh-auth-rbac/commit/2980fe17038b456d7a101a4486499e3bd3e7a61b))
+
 ## v0.2.7 (2024-05-29)
 
 ### Fix
 
 * Don't autocommit within this library; raise errors from validate_ result ([`b203e46`](https://github.com/educationwarehouse/edwh-auth-rbac/commit/b203e46380e3b0338375c5cbd978fcf6eec5c561))
 
 ## v0.2.6 (2024-05-29)
```

### Comparing `edwh_auth_rbac-0.2.7/htmlcov/class_index.html` & `edwh_auth_rbac-0.3.0/htmlcov/class_index.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.7/htmlcov/coverage_html_cb_da166b87.js` & `edwh_auth_rbac-0.3.0/htmlcov/coverage_html_cb_da166b87.js`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.7/htmlcov/favicon_32_cb_58284776.png` & `edwh_auth_rbac-0.3.0/htmlcov/favicon_32_cb_58284776.png`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.7/htmlcov/function_index.html` & `edwh_auth_rbac-0.3.0/htmlcov/function_index.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.7/htmlcov/index.html` & `edwh_auth_rbac-0.3.0/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.7/htmlcov/keybd_closed_cb_ce680311.png` & `edwh_auth_rbac-0.3.0/htmlcov/keybd_closed_cb_ce680311.png`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.7/htmlcov/status.json` & `edwh_auth_rbac-0.3.0/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.7/htmlcov/style_cb_8e611ae1.css` & `edwh_auth_rbac-0.3.0/htmlcov/style_cb_8e611ae1.css`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.7/htmlcov/z_438b44bce6437be6___init___py.html` & `edwh_auth_rbac-0.3.0/htmlcov/z_438b44bce6437be6___init___py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.7/htmlcov/z_438b44bce6437be6_helpers_py.html` & `edwh_auth_rbac-0.3.0/htmlcov/z_438b44bce6437be6_helpers_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.7/htmlcov/z_438b44bce6437be6_migrations_py.html` & `edwh_auth_rbac-0.3.0/htmlcov/z_438b44bce6437be6_migrations_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.7/htmlcov/z_438b44bce6437be6_model_py.html` & `edwh_auth_rbac-0.3.0/htmlcov/z_438b44bce6437be6_model_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.7/htmlcov/z_438b44bce6437be6_rbac_py.html` & `edwh_auth_rbac-0.3.0/htmlcov/z_438b44bce6437be6_rbac_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.7/htmlcov/z_a44f0ac069e85531___init___py.html` & `edwh_auth_rbac-0.3.0/htmlcov/z_a44f0ac069e85531___init___py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.7/htmlcov/z_a44f0ac069e85531_test_rbac_py.html` & `edwh_auth_rbac-0.3.0/htmlcov/z_a44f0ac069e85531_test_rbac_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.7/src/edwh_auth_rbac/migrations.py` & `edwh_auth_rbac-0.3.0/src/edwh_auth_rbac/migrations.py`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.7/src/edwh_auth_rbac/model.py` & `edwh_auth_rbac-0.3.0/src/edwh_auth_rbac/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from .helpers import IS_IN_LIST
 
 
 class DEFAULT:
     pass
 
 
+SPECIAL_PERMISSIONS = {"*"}
+
 IdentityKey: typing.TypeAlias = str | int | UUID | dict[str, "IdentityKey"]
 ObjectTypes = typing.Literal["user", "group", "item"]
 When: typing.TypeAlias = str | dt.datetime | typing.Type[DEFAULT]
 
 DEFAULT_STARTS = dt.datetime(2000, 1, 1)
 DEFAULT_ENDS = dt.datetime(3000, 1, 1)
 
@@ -89,14 +91,17 @@
     if object_type:
         query &= db.identity.object_type == object_type
 
     return query
 
 
 def key_lookup(db: DAL, identity_key: IdentityKey, object_type: Optional[ObjectTypes] = None) -> str:
+    if isinstance(identity_key, str) and identity_key in SPECIAL_PERMISSIONS:
+        return identity_key
+
     query = key_lookup_query(db, identity_key, object_type)
 
     rowset = db(query).select(db.identity.object_id)
 
     if len(rowset) != 1:
         raise ValueError("Key lookup for {} returned {} results.".format(identity_key, len(rowset)))
 
@@ -197,23 +202,23 @@
         migrate=False,  # view
         redefine=redefine,
         primarykey=["root", "object_id"],  # composed, no primary key
     )
 
 
 def add_identity(
-    db: DAL,
-    email: str,
-    member_of: list[IdentityKey],
-    name: Optional[str] = None,
-    firstname: Optional[str] = None,
-    fullname: Optional[str] = None,
-    password: Optional[str] = None,
-    gid: Optional[IdentityKey] = None,
-    object_type: Optional[ObjectTypes] = None,
+        db: DAL,
+        email: str,
+        member_of: list[IdentityKey],
+        name: Optional[str] = None,
+        firstname: Optional[str] = None,
+        fullname: Optional[str] = None,
+        password: Optional[str] = None,
+        gid: Optional[IdentityKey] = None,
+        object_type: Optional[ObjectTypes] = None,
 ) -> str:
     """paramaters name and firstname are equal."""
     email = email.lower().strip()
     if object_type is None:
         raise ValueError("object_type parameter expected")
     object_id = gid or uuid.uuid4()
     result = db.identity.validate_and_insert(
@@ -281,15 +286,15 @@
     :param key: can be the name of the group, the id, object_id or email_address
     :return: user record or None when not found
     """
     return get_identity(db, key, object_type="group")
 
 
 def authenticate_user(
-    db: DAL, password: Optional[str] = None, user: Optional[Identity] = None, key: Optional[IdentityKey] = None
+        db: DAL, password: Optional[str] = None, user: Optional[Identity] = None, key: Optional[IdentityKey] = None
 ) -> bool:
     if not password:
         return False
 
     if not user and key:
         user = get_user(db, key)
 
@@ -337,20 +342,20 @@
 def get_members(db: DAL, object_id: IdentityKey, bare: bool = True):
     query = db.recursive_members.root == object_id
     fields = [db.recursive_members.object_id, db.recursive_members.object_type] if bare else []
     return db(query).select(*fields)
 
 
 def add_permission(
-    db: DAL,
-    identity_key: IdentityKey,
-    target_oid: IdentityKey,
-    privilege: str,
-    starts: dt.datetime | str = DEFAULT_STARTS,
-    ends: dt.datetime | str = DEFAULT_ENDS,
+        db: DAL,
+        identity_key: IdentityKey | typing.Literal["*"],
+        target_oid: IdentityKey | typing.Literal["*"],
+        privilege: str,
+        starts: dt.datetime | str = DEFAULT_STARTS,
+        ends: dt.datetime | str = DEFAULT_ENDS,
 ) -> None:
     identity_oid = key_lookup(db, identity_key)
     starts = unstr_datetime(starts)
     ends = unstr_datetime(ends)
     if has_permission(db, identity_oid, target_oid, privilege, when=starts):
         # permission already granted. just skip it
         print(
@@ -369,15 +374,15 @@
     )
     if e := result.get("errors"):
         raise ValueError(e)
     # db.commit()
 
 
 def remove_permission(
-    db: DAL, identity_key: IdentityKey, target_oid: IdentityKey, privilege: str, when: When | None = DEFAULT
+        db: DAL, identity_key: IdentityKey, target_oid: IdentityKey, privilege: str, when: When | None = DEFAULT
 ) -> bool:
     identity_oid = key_lookup(db, identity_key)
     if when is DEFAULT:
         when = dt.datetime.now()
     else:
         when = unstr_datetime(when)
     # base object is is the root to check for, user or group
@@ -407,44 +412,33 @@
     if source_id := getattr(source, "_id", None):
         other._id = other[source_id.name]
     db[alias] = other
     return other
 
 
 def has_permission(
-    db: DAL, user_or_group_key: IdentityKey, target_oid: IdentityKey, privilege: str, when: When | None = DEFAULT
+        db: DAL, user_or_group_key: IdentityKey, target_oid: IdentityKey, privilege: str, when: When | None = DEFAULT
 ) -> bool:
-    user_or_group_oid = key_lookup(db, user_or_group_key)
+    root_oid = key_lookup(db, user_or_group_key)
     # the permission system
     if when is DEFAULT:
         when = dt.datetime.now()
     else:
         when = unstr_datetime(when)
     # base object is is the root to check for, user or group
-    root_oid = user_or_group_oid
     permission = db.permission
     # ugly hack to satisfy pydal aliasing keyed tables /views
     left = with_alias(db, db.recursive_memberships, "left")
     right = with_alias(db, db.recursive_memberships, "right")
     # left = db.recursive_memberships.with_alias('left')
     # right = db.recursive_memberships.with_alias('right')
 
     # end of ugly hack
-    query = left.root == root_oid
-    query &= right.root == target_oid
-    query &= permission.identity_object_id == left.object_id
-    query &= permission.target_object_id == right.object_id
-    query &= permission.privilege == privilege
+    query = (left.root == root_oid) | (left.root == "*")
+    query &= (right.root == target_oid) | (right.root == "*")
+    query &= (permission.identity_object_id == left.object_id) | (permission.identity_object_id == "*")
+    query &= (permission.target_object_id == right.object_id) | (permission.target_object_id == "*")
+    query &= (permission.privilege == privilege) | (permission.privilege == "*")
     query &= permission.starts <= when
     query &= permission.ends >= when
 
-    if row := db(permission).select().first():
-        identity = db.identity(object_id=row.identity_object_id)
-        target = db.identity(object_id=row.target_object_id)
-
-        print(
-            row,
-            identity,
-            target,
-        )
-
     return db(query).count() > 0
```

### Comparing `edwh_auth_rbac-0.2.7/src/edwh_auth_rbac/rbac.py` & `edwh_auth_rbac-0.3.0/src/edwh_auth_rbac/rbac.py`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.7/tests/test_migrate.py` & `edwh_auth_rbac-0.3.0/tests/test_migrate.py`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.7/tests/test_rbac.py` & `edwh_auth_rbac-0.3.0/tests/test_rbac.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,36 @@
+import os
 import tempfile
 import uuid
+from pathlib import Path
 
 import dotmap
 import pytest
 from pydal import DAL
 
 from src.edwh_auth_rbac.migrations import rbac_views
 from src.edwh_auth_rbac.model import define_auth_rbac_model
 from src.edwh_auth_rbac.rbac import AuthRbac
 
 namespace = uuid.UUID("84f5c757-4be0-49c8-a3ba-4f4d79167839")
 
+FAKE_TEMPDIR = False
+# FAKE_TEMPDIR = True
+
 
 @pytest.fixture(scope="module")
 def tmpdir():
     with tempfile.TemporaryDirectory() as tmpdirname:
-        print("new tempdir")
-        yield tmpdirname
+        if FAKE_TEMPDIR:
+            fake = Path("/tmp/fake_tmpdir")
+            fake.mkdir(exist_ok=True, parents=True)
+            yield str(fake)
+        else:
+            print("new tempdir")
+            yield tmpdirname
 
 
 @pytest.fixture(scope="module")
 def database(tmpdir):
     class Database:
         def __enter__(self):
             self.db = DAL("sqlite://auth_rbac.sqlite", folder=tmpdir)
@@ -155,7 +165,18 @@
         item = rbac.add_item(f"@{item_gid}", item_gid, [items], gid=item_gid)
 
         assert item["object_id"] == item_gid
 
         rbac.add_permission(users, item_gid, "read")
 
         assert rbac.has_permission(user, item_gid, "read")
+
+        admins = rbac.add_group("admins@internal", "Admins", [users])
+        rbac.add_permission(admins, "*", "*")
+
+        admin1 = rbac.add_user("admin1@example", "Admin1", "Admin One", "secure", [admins])
+
+        assert rbac.has_permission(admin1, item_gid, "read")
+        assert rbac.has_permission(admin1, item_gid, "write")
+
+        assert rbac.has_permission(user, item_gid, "read")
+        assert not rbac.has_permission(user, item_gid, "write")
```

### Comparing `edwh_auth_rbac-0.2.7/pyproject.toml` & `edwh_auth_rbac-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.7/PKG-INFO` & `edwh_auth_rbac-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: edwh-auth-rbac
-Version: 0.2.7
+Version: 0.3.0
 Summary: Recursive Memberships and Permissions for the Education Warehouse Authentication System
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-auth-rbac#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-auth-rbac/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-auth-rbac
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 Keywords: edwh,omgeving,whitelabel
```

