# Comparing `tmp/fastapi_simple_auth-0.0.5.tar.gz` & `tmp/fastapi_simple_auth-0.0.6.tar.gz`

## Comparing `fastapi_simple_auth-0.0.5.tar` & `fastapi_simple_auth-0.0.6.tar`

### file list

```diff
@@ -1,48 +1,59 @@
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/.env-example
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/alembic.ini
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/app.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/requirements.txt
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/__init__.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/cron.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/crud.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/db.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/envmail.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/exceptions.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/models.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/pub.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/router.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/schemas.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/session.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/settings.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/startup.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/templates.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/verification.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/alembic/README
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/alembic/env.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/alembic/script.py.mako
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/alembic/versions/9a3f872373f4_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/cli/__init__.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/cli/simpleauth.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/templates/afterlogin.html
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/templates/base.html
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/templates/login.html
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/templates/profile.html
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/templates/recover.html
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/templates/recover_code.html
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/templates/register.html
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/templates/verify-email.html
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/templates/email/change-email.html
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/templates/email/confirm-email.html
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/templates/email/recover.html
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/views/__init__.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/views/login.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/views/profile.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/views/recover.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/views/settingsjs.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/views/signup.py
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/fastapi_simple_auth/views/verify.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/LICENSE
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/README.md
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/.env-example
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/alembic.ini
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/app.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/docs/mkdocs.yml
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/docs/docs/apitest.md
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/docs/docs/config.md
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/docs/docs/index.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/docs/docs/quickstart.md
+-rw-r--r--   0        0        0    13491 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/docs/docs/img/favicon.ico
+-rw-r--r--   0        0        0    29196 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/docs/docs/img/login.png
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/__init__.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/cron.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/crud.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/db.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/envmail.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/exceptions.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/jwt.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/models.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/passwordstrength.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/pub.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/router.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/schemas.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/session.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/settings.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/startup.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/str2dict.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/templates.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/verification.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/alembic/README
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/alembic/env.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/alembic/script.py.mako
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/alembic/versions/9a3f872373f4_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/cli/__init__.py
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/cli/simpleauth.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/templates/afterlogin.html
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/templates/base.html
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/templates/login.html
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/templates/profile.html
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/templates/recover.html
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/templates/recover_code.html
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/templates/register.html
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/templates/verify-email.html
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/templates/email/change-email.html
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/templates/email/confirm-email.html
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/templates/email/recover.html
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/views/__init__.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/views/jwt.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/views/login.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/views/profile.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/views/recover.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/views/settingsjs.py
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/views/signup.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/fastapi_simple_auth/views/verify.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/README.md
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 fastapi_simple_auth-0.0.6/PKG-INFO
```

### Comparing `fastapi_simple_auth-0.0.5/.env-example` & `fastapi_simple_auth-0.0.6/.env-example`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.5/alembic.ini` & `fastapi_simple_auth-0.0.6/alembic.ini`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/cron.py` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/cron.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/crud.py` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/crud.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     
     return user
 
 def get_users(db: Session, skip: int = 0, limit: int = 100):
     return db.query(models.User).offset(skip).limit(limit).all()
 
 def change_password(db: Session, user: models.User, new_password: str):
-    user.password = get_password_hash(new_password)
+    user.set_password(new_password)
     db.commit()
     db.refresh(user)
     return user
 
 def create_user(db: Session, user: schemas.UserCreate):
     hashed_password = get_password_hash(user.password)
```

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/envmail.py` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/envmail.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/models.py` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,18 +2,25 @@
 import datetime
 
 from sqlalchemy import Boolean, Integer, Column, String, DateTime, Text, ForeignKey
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.sql import func
 from sqlalchemy.orm import relationship
 
+from passlib.context import CryptContext
+
 from .settings import settings
 
 Base = declarative_base()
 
+pwd_context = CryptContext(schemes=["bcrypt"], deprecated="auto")
+
+def get_password_hash(password):
+    return pwd_context.hash(password)
+
 def get_uuid():
     return str(uuid.uuid4())
 
 
 class User(Base):
     __tablename__ = "users"
 
@@ -29,14 +36,22 @@
     disabled = Column(Boolean, default=False)
     other = Column(Text)
     codes = relationship("Code", back_populates="user")
 
     def __repr__(self):
         return f"user {self.uuid} {self.username}"
 
+    def dump(self):
+        return f"username: {self.username}\n" \
+            f"uuid: {self.uuid}\n" \
+            f"verified: {self.email_verified}\n" \
+            f"codes: {' '.join([ c.code for c in self.codes]) }"
+
+    def set_password(self, new_password: str):
+        self.password = get_password_hash(new_password)
 
 class Code(Base):
     __tablename__ = "codes"
 
     id = Column(Integer, nullable=False, unique=True, primary_key=True, autoincrement=True)
 
     user_id = Column(String(36), ForeignKey("users.uuid"), nullable=True)
```

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/pub.py` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/pub.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 from typing import Annotated
 from fastapi import Depends, HTTPException, Request 
 from .settings import settings
 from . import views
 from sqlalchemy.orm import Session
 from .db import get_db
 from .session import get_current_user_session
+from .jwt import get_current_user_bearer
 from .models import User
 # public interface
 
 
 async def get_current_user(request: Request, db: Session = Depends(get_db)): 
-    if settings.auth_transport == "session":
-        return get_current_user_session(request, db)
-    
+    if settings.transport_session:
+        user = get_current_user_session(request, db)
+
+    if user:
+        return user
+
+    if settings.transport_bearer:
+        user = get_current_user_bearer(request, db)
+
+    return user
+
 async def get_current_active_user(
         rq: Request,
         user: Annotated[User, Depends(get_current_user)],
 ):
 
     if user is None:
         if settings.notauth_login:
```

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/session.py` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 def get_current_user_session(request: Request, db: Session):
     try:
         uuid = request.session['user']
     except KeyError:
         return None
     
     user = get_user_by_uuid(db, uuid)
-    return user
+    return user
+
```

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/verification.py` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/verification.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/alembic/env.py` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/alembic/env.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/alembic/script.py.mako` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/alembic/versions/9a3f872373f4_initial.py` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/alembic/versions/9a3f872373f4_initial.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/templates/base.html` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/templates/base.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/templates/login.html` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/templates/login.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/templates/profile.html` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/templates/profile.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/templates/recover.html` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/templates/recover.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/templates/recover_code.html` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/templates/recover_code.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/templates/register.html` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/templates/register.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/templates/verify-email.html` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/templates/verify-email.html`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/views/__init__.py` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/views/login.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,67 @@
-
-import json
 from typing import Annotated
-from pydantic import BaseModel, EmailStr
 
-from fastapi import Request, Response, Depends, HTTPException, status
+from fastapi import Request
 from fastapi.responses import HTMLResponse, RedirectResponse
-from fastapi.security import OAuth2PasswordBearer, OAuth2PasswordRequestForm
+from fastapi.security import OAuth2PasswordRequestForm
+from fastapi import Depends, HTTPException, status
 
 from sqlalchemy.orm import Session
 
+from ..db import get_db
 from ..router import auth_router
 from ..templates import template_env
 from ..settings import settings
+from .. import crud
 
-from .. import crud, schemas
-from ..db import get_db
-from ..exceptions import SimpleAuthVerificationAlreadySent
-from ..cron import cron
-
-from . import login, profile, settingsjs, signup, verify, recover
-
-class Token(BaseModel):
-    access_token: str
-    token_type: str
-
-
-class TokenData(BaseModel):
-    username: str | None = None
-
-
-class User(BaseModel):
-    username: str
-    email: str | None = None
-    full_name: str | None = None
-    disabled: bool | None = None
-
+@auth_router.get('/login')
+def get_login(request: Request, response_class=HTMLResponse):
+    tpl = template_env.get_template('login.html')
+
+    ctx = {
+        'rq': request,
+        'settings': settings,
+        'motd2': 'motd motd motd motd motd motd',
+        'error2': 'some problem'
+    }
+
+    html = tpl.render(ctx)
+    return HTMLResponse(html)
+
+@auth_router.post('/login')
+def post_login(
+            rq: Request, 
+            form: Annotated[OAuth2PasswordRequestForm, Depends()],
+            db: Session = Depends(get_db)):
 
-#class UNUSED_UserInDB(User):
-#    hashed_password: str
-
-
-
-
-
-@auth_router.post("/token")
-async def UNUSED_login_for_access_token(
-    form: Annotated[OAuth2PasswordRequestForm, Depends()],
-    db: Session = Depends(get_db)
-) -> Token:
-    
+    # here is POST
     user = crud.get_auth_user(db, form.username, form.password)
     if not user:
         raise HTTPException(
             status_code=status.HTTP_401_UNAUTHORIZED,
             detail="Incorrect username or password",
             headers={"WWW-Authenticate": "Bearer"},
         )
-    access_token_expires = timedelta(minutes=ACCESS_TOKEN_EXPIRE_MINUTES)
-    access_token = create_access_token(
-        data={"sub": user.uuid}, expires_delta=access_token_expires
-    )
-    return Token(access_token=access_token, token_type="bearer")
 
+    # what if unverified?
+    if settings.username_is_email and not user.email_verified:
+        raise HTTPException(
+            status_code=status.HTTP_401_UNAUTHORIZED,
+            detail="Email not verified",
+            headers={"WWW-Authenticate": "Bearer"},
+        )
+
+    # authenticate
+    if settings.auth_transport == "session":
+        rq.session['user'] = user.uuid        
+
+    return {
+        'status': 'OK',
+        'url': settings.afterlogin_url
+    }
+
+@auth_router.post('/logout')
+def logout(rq: Request):
+    if settings.auth_transport == "session":
+        del rq.session['user']
+    return RedirectResponse(settings.afterlogout_url)
```

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/views/login.py` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/views/signup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,71 @@
-from typing import Annotated
-
-from fastapi import Request
-from fastapi.responses import HTMLResponse, RedirectResponse
-from fastapi.security import OAuth2PasswordRequestForm
-from fastapi import Depends, HTTPException, status
-
+from fastapi import APIRouter, Depends, HTTPException, Request, Response
+from fastapi.responses import HTMLResponse
 from sqlalchemy.orm import Session
 
-from ..db import get_db
+from .. import schemas, crud
+from ..settings import settings
 from ..router import auth_router
 from ..templates import template_env
-from ..settings import settings
-from .. import crud
-
-@auth_router.get('/login')
-def get_login(request: Request, response_class=HTMLResponse):
-    tpl = template_env.get_template('login.html')
+from ..db import get_db
+from ..verification import send_verification_signup
+from ..exceptions import SimpleAuthVerificationAlreadySent
+from ..passtr import PasswordStrengthError, check_password
+
+@auth_router.get('/signup')
+def get_signup(request: Request, response_class=HTMLResponse):
+    tpl = template_env.get_template('register.html')
 
     ctx = {
         'rq': request,
         'settings': settings,
         'motd2': 'motd motd motd motd motd motd',
         'error2': 'some problem'
     }
 
     html = tpl.render(ctx)
     return HTMLResponse(html)
 
-@auth_router.post('/login')
-def post_login(
-            rq: Request, 
-            form: Annotated[OAuth2PasswordRequestForm, Depends()],
-            db: Session = Depends(get_db)):
-
-    # here is POST
-    user = crud.get_auth_user(db, form.username, form.password)
-    if not user:
-        raise HTTPException(
-            status_code=status.HTTP_401_UNAUTHORIZED,
-            detail="Incorrect username or password",
-            headers={"WWW-Authenticate": "Bearer"},
-        )
-
-
-    # authenticate
-    if settings.auth_transport == "session":
-        rq.session['user'] = user.uuid        
-
-    return {
-        'status': 'OK',
-        'url': settings.afterlogin_url
-    }
-
-@auth_router.post('/logout')
-def logout(rq: Request):
-    if settings.auth_transport == "session":
-        del rq.session['user']
-    return RedirectResponse(settings.afterlogout_url)
 
+@auth_router.post("/users/") # , response_model=schemas.User)
+def create_user(rq: Request, user: schemas.UserCreate, db: Session = Depends(get_db)):
+    
+    db_user = crud.get_user_by_username(db, username=user.username)
+
+    if db_user:
+        raise HTTPException(status_code=400, detail="User already registered")
+
+
+    try:
+        check_password(user.password)
+    except PasswordStrengthError as e:
+        raise HTTPException(status_code=400, detail=str(e))
+
+
+    user = crud.create_user(db=db, user=user)
+    if settings.username_is_email:
+        try:
+            send_verification_signup(rq=rq, db=db, user=user)
+            return {"status": "OK", 
+                    "message": "Please check your email for verification code",
+                    "redirect": str(rq.url_for("get_email_verify", email=user.username))
+                    }
+        
+        except SimpleAuthVerificationAlreadySent as e:
+            print("ERR", e)
+    else:
+        print("created user", user)    
+        if settings.signin_after_signup:
+            # authenticate user
+            if settings.auth_transport == "session":
+                rq.session['user'] = user.uuid        
+                return {"status": "OK", 
+                        "redirect": settings.afterlogin_url }
+        else:
+            return {"status": "OK", 
+                    "message": "Please check your email for verification code",
+                    "redirect": settings.afterlogin_url }
+
+    
+    print("return")
+    # return user
+    return Response()
```

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/views/profile.py` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/views/profile.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from ..router import auth_router
 from ..templates import template_env
 from ..settings import settings
 from ..pub import logged_in_user
 from ..crud import verify_password, get_password_hash, change_password
 from ..db import get_db
 from ..verification import send_verification_change_email
+from ..passwordstrenght import PasswordStrengthError, check_password
+
 
 @auth_router.get('/profile')
 def profile_get(request: Request, user: logged_in_user, response_class=HTMLResponse):
     tpl = template_env.get_template('profile.html')
 
     ctx = {
         'rq': request,
@@ -33,14 +35,21 @@
 def change_pass_post(request: Request, user: logged_in_user, 
                      chpass: ChangePasswordModel,
                      db: Session = Depends(get_db)):
 
     if not verify_password(chpass.old_password, user.password):
         return Response(status_code=401, content="Wrong password")
 
+    try:
+        check_password(chpass.password)
+    except PasswordStrengthError as e:
+        return Response(status_code=401, content=str(e))
+
+
+
     change_password(db=db, user=user, new_password=chpass.password)
 
     return Response('password changed')
 
 class ChangeEmailModel(BaseModel):
     email: EmailStr
```

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/views/recover.py` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/views/recover.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/views/settingsjs.py` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/views/settingsjs.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.5/fastapi_simple_auth/views/verify.py` & `fastapi_simple_auth-0.0.6/fastapi_simple_auth/views/verify.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.5/.gitignore` & `fastapi_simple_auth-0.0.6/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -155,9 +155,10 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
+docs/site
 NOTES
 test.db
```

### Comparing `fastapi_simple_auth-0.0.5/LICENSE` & `fastapi_simple_auth-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_simple_auth-0.0.5/pyproject.toml` & `fastapi_simple_auth-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,16 @@
   'alembic',
   'python-dotenv',
   'jinja2',
   'pydantic-settings',
   'itsdangerous',
   'typer',
   'click',
+  'zxcvbn',
+  'password_strength'
 ]
 
 
 [project.urls]
 Documentation = "https://github.com/yaroslaff/fastapi-simple-auth#readme"
 Issues = "https://github.com/yaroslaff/fastapi-simple-auth/issues"
 Source = "https://github.com/yaroslaff/fastapi-simple-auth"
```

### Comparing `fastapi_simple_auth-0.0.5/PKG-INFO` & `fastapi_simple_auth-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: fastapi-simple-auth
-Version: 0.0.5
+Version: 0.0.6
 Summary: FastAPI simple authentication
 Project-URL: Documentation, https://github.com/yaroslaff/fastapi-simple-auth#readme
 Project-URL: Issues, https://github.com/yaroslaff/fastapi-simple-auth/issues
 Project-URL: Source, https://github.com/yaroslaff/fastapi-simple-auth
 Author-email: Yaroslav Polyakov <yaroslaff@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -21,38 +21,78 @@
 Requires-Dist: alembic
 Requires-Dist: click
 Requires-Dist: fastapi
 Requires-Dist: fastapi-simple-auth-basic
 Requires-Dist: itsdangerous
 Requires-Dist: jinja2
 Requires-Dist: passlib[bcrypt]
+Requires-Dist: password-strength
 Requires-Dist: pydantic-settings
 Requires-Dist: pydantic[email]
 Requires-Dist: python-dotenv
 Requires-Dist: python-jose[cryptography]
 Requires-Dist: python-multipart
 Requires-Dist: typer
 Requires-Dist: uvicorn
+Requires-Dist: zxcvbn
 Description-Content-Type: text/markdown
 
-# api-auth
+# FastAPI Simple Auth
+
+## Authentication easy as three lines!
+
+1. Import package
+2. hook to app with `SimpleAuth(app)`
+3. add `user: logged_in_user` to protected view
+
+~~~python
+from fastapi import FastAPI
+from fastapi_simple_auth import SimpleAuth, logged_in_user
+        
+app = FastAPI()
+
+simpleauth = SimpleAuth(app)
+
+@app.get("/")
+async def read_users_me(user: logged_in_user) -> str:    
+    return f"Hello {user.username} {user.uuid}"
+~~~
+
+![login screenshot](docs/docs/img/login.png)
+
+## Features
+- Users are stored in any supported SQLAlchemy database
+- Optional email verification
+- User creation
+- Password recovery
+- Profile page with change password, change email
+- Custom UI themes!
+
 
 ## Install
 
 ~~~shell
-cp .env.example .env
-# now edit it
+pip3 install fastapi-simple-auth
+# create/edit .env file
 vim .env
+simpleauth dbupgrade
+~~~
 
-alembic upgrade head
+Write app in app.py
+
+Start:
+~~~
+uvicorn app:app
 ~~~
 
 
 ## Usage
 
+This examples uses [httpie](http://httpie.io/) because it is very good to craft JSON requests.
+
 ~~~
 # register
 http POST http://localhost:8000/auth/users/ username=me@example.com password=secret
 
 # simple auth (session)
 http -f POST http://localhost:8000/auth/login username=me@example.com password=secret
```

