# Comparing `tmp/streamlit_sqlalchemy-0.2.3.tar.gz` & `tmp/streamlit_sqlalchemy-0.2.4.tar.gz`

## Comparing `streamlit_sqlalchemy-0.2.3.tar` & `streamlit_sqlalchemy-0.2.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/CONTRIBUTING
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/.streamlit/secrets.toml
--rw-r--r--   0        0        0    20991 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/assets/crud_create.png
--rw-r--r--   0        0        0    28128 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/assets/crud_update.png
--rw-r--r--   0        0        0  4919016 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/assets/streamlit-example-2023-12-31-16-12-91.gif
--rw-r--r--   0        0        0  3628434 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/assets/streamlit-example-2023-12-31-16-12-91.webm
--rw-r--r--   0        0        0  3360669 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/assets/streamlit-example-2024-01-06-13-01-36.gif
--rw-r--r--   0        0        0  2426792 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/assets/streamlit-example-2024-01-06-13-01-36.webm
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/examples/__init__.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/examples/example.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/examples/example2.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/examples/models.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/src/streamlit_sqlalchemy/__init__.py
--rw-r--r--   0        0        0    21858 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/src/streamlit_sqlalchemy/mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/tests/conftest.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/tests/objects.py
--rw-r--r--   0        0        0     8939 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/tests/streamlit_sqlalchemy/test_mixin.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/tests/streamlit_sqlalchemy/mixin/create_form.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/tests/streamlit_sqlalchemy/mixin/create_form_advanced.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/tests/streamlit_sqlalchemy/mixin/delete_button.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/tests/streamlit_sqlalchemy/mixin/delete_form.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/tests/streamlit_sqlalchemy/mixin/edit_button.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/tests/streamlit_sqlalchemy/mixin/update_form.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/tests/streamlit_sqlalchemy/mixin/update_form_except_m2o.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/tests/streamlit_sqlalchemy/mixin/update_select_form.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/LICENSE
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/README.md
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/CONTRIBUTING
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/.streamlit/secrets.toml
+-rw-r--r--   0        0        0    20991 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/assets/crud_create.png
+-rw-r--r--   0        0        0    28128 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/assets/crud_update.png
+-rw-r--r--   0        0        0  4919016 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/assets/streamlit-example-2023-12-31-16-12-91.gif
+-rw-r--r--   0        0        0  3628434 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/assets/streamlit-example-2023-12-31-16-12-91.webm
+-rw-r--r--   0        0        0  3360669 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/assets/streamlit-example-2024-01-06-13-01-36.gif
+-rw-r--r--   0        0        0  2426792 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/assets/streamlit-example-2024-01-06-13-01-36.webm
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/examples/__init__.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/examples/example.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/examples/example2.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/examples/models.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/src/streamlit_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    21876 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/src/streamlit_sqlalchemy/mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/tests/conftest.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/tests/objects.py
+-rw-r--r--   0        0        0     8939 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/tests/streamlit_sqlalchemy/test_mixin.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/tests/streamlit_sqlalchemy/mixin/create_form.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/tests/streamlit_sqlalchemy/mixin/create_form_advanced.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/tests/streamlit_sqlalchemy/mixin/delete_button.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/tests/streamlit_sqlalchemy/mixin/delete_form.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/tests/streamlit_sqlalchemy/mixin/edit_button.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/tests/streamlit_sqlalchemy/mixin/update_form.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/tests/streamlit_sqlalchemy/mixin/update_form_except_m2o.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/tests/streamlit_sqlalchemy/mixin/update_select_form.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/LICENSE
+-rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/README.md
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 streamlit_sqlalchemy-0.2.4/PKG-INFO
```

### Comparing `streamlit_sqlalchemy-0.2.3/CONTRIBUTING` & `streamlit_sqlalchemy-0.2.4/CONTRIBUTING`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.3/.github/workflows/python-publish.yml` & `streamlit_sqlalchemy-0.2.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.3/assets/crud_create.png` & `streamlit_sqlalchemy-0.2.4/assets/crud_create.png`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.3/assets/crud_update.png` & `streamlit_sqlalchemy-0.2.4/assets/crud_update.png`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.3/assets/streamlit-example-2023-12-31-16-12-91.gif` & `streamlit_sqlalchemy-0.2.4/assets/streamlit-example-2023-12-31-16-12-91.gif`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.3/assets/streamlit-example-2023-12-31-16-12-91.webm` & `streamlit_sqlalchemy-0.2.4/assets/streamlit-example-2023-12-31-16-12-91.webm`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.3/assets/streamlit-example-2024-01-06-13-01-36.gif` & `streamlit_sqlalchemy-0.2.4/assets/streamlit-example-2024-01-06-13-01-36.gif`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.3/assets/streamlit-example-2024-01-06-13-01-36.webm` & `streamlit_sqlalchemy-0.2.4/assets/streamlit-example-2024-01-06-13-01-36.webm`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.3/examples/example.py` & `streamlit_sqlalchemy-0.2.4/examples/example.py`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.3/examples/example2.py` & `streamlit_sqlalchemy-0.2.4/examples/example2.py`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.3/examples/models.py` & `streamlit_sqlalchemy-0.2.4/examples/models.py`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.3/src/streamlit_sqlalchemy/mixin.py` & `streamlit_sqlalchemy-0.2.4/src/streamlit_sqlalchemy/mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -574,15 +574,15 @@
                         )
                     }
                 )
 
             submitted = st.form_submit_button(f"Update {self.st_pretty_class()}")
             if submitted:
                 for field in set(kwargs) - set(except_columns):
-                    if field.endswith("_id"):
+                    if field.endswith("_id") and kwargs[field]:
                         kwargs[field] = kwargs[field].id
                 self._st_update(**kwargs)
         return submitted
 
     def _get_first_column_name(self, cls: type[DeclarativeBase]) -> Optional[str]:
         """
         Returns the first column name of the given class.
```

### Comparing `streamlit_sqlalchemy-0.2.3/tests/objects.py` & `streamlit_sqlalchemy-0.2.4/tests/objects.py`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.3/tests/streamlit_sqlalchemy/test_mixin.py` & `streamlit_sqlalchemy-0.2.4/tests/streamlit_sqlalchemy/test_mixin.py`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.3/LICENSE` & `streamlit_sqlalchemy-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.3/README.md` & `streamlit_sqlalchemy-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_sqlalchemy-0.2.3/pyproject.toml` & `streamlit_sqlalchemy-0.2.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "streamlit-sqlalchemy"
-version = "0.2.3"
+version = "0.2.4"
 authors = [{ name = "artygo8", email = "arthurgossuin@gmail.com" }]
 description = "Some templating for streamlit and sqlalchemy"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python :: 3",
```

### Comparing `streamlit_sqlalchemy-0.2.3/PKG-INFO` & `streamlit_sqlalchemy-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: streamlit-sqlalchemy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Some templating for streamlit and sqlalchemy
 Project-URL: Homepage, https://github.com/artygo8/streamlit-sqlalchemy
 Project-URL: Issues, https://github.com/artygo8/streamlit-sqlalchemy/issues
 Author-email: artygo8 <arthurgossuin@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: database,sql,sqlalchemy,streamlit,templating
```

