# Comparing `tmp/streamlit_pandera-0.0.1.tar.gz` & `tmp/streamlit_pandera-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_pandera-0.0.1.tar", max compression
+gzip compressed data, was "streamlit_pandera-0.0.2.tar", max compression
```

## Comparing `streamlit_pandera-0.0.1.tar` & `streamlit_pandera-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,6 @@
--rw-r--r--   0        0        0     1063 2024-05-26 22:04:51.393442 streamlit_pandera-0.0.1/LICENSE
--rw-r--r--   0        0        0     2715 2024-05-26 22:04:51.393442 streamlit_pandera-0.0.1/README.md
--rw-r--r--   0        0        0     1198 2024-05-26 22:04:51.393442 streamlit_pandera-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      479 2024-05-26 22:04:51.393442 streamlit_pandera-0.0.1/streamlit_pandera/Home.py
--rw-r--r--   0        0        0        0 2024-05-26 22:04:51.393442 streamlit_pandera-0.0.1/streamlit_pandera/__init__.py
--rw-r--r--   0        0        0      148 2024-05-26 22:04:51.393442 streamlit_pandera-0.0.1/streamlit_pandera/io_file_validator/__init__.py
--rw-r--r--   0        0        0     3168 2024-05-26 22:05:13.129567 streamlit_pandera-0.0.1/streamlit_pandera/io_file_validator/validate_file.py
--rw-r--r--   0        0        0     4119 2024-05-26 22:04:51.397442 streamlit_pandera-0.0.1/streamlit_pandera/io_file_validator/validator.py
--rw-r--r--   0        0        0     1770 2024-05-26 22:04:51.397442 streamlit_pandera-0.0.1/streamlit_pandera/pages/0_Instructions.py
--rw-r--r--   0        0        0        0 2024-05-26 22:04:51.397442 streamlit_pandera-0.0.1/streamlit_pandera/pages/__init__.py
--rw-r--r--   0        0        0     3604 1970-01-01 00:00:00.000000 streamlit_pandera-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2680 2024-05-29 22:09:36.030602 streamlit_pandera-0.0.2/README.md
+-rw-r--r--   0        0        0     1209 2024-05-29 22:09:36.034602 streamlit_pandera-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3414 2024-05-29 22:09:56.390769 streamlit_pandera-0.0.2/streamlit_pandera/Home.py
+-rw-r--r--   0        0        0      629 2024-05-29 22:09:36.034602 streamlit_pandera-0.0.2/streamlit_pandera/__init__.py
+-rw-r--r--   0        0        0     1770 2024-05-29 22:09:36.034602 streamlit_pandera-0.0.2/streamlit_pandera/pages/0_Instructions.py
+-rw-r--r--   0        0        0     3619 1970-01-01 00:00:00.000000 streamlit_pandera-0.0.2/PKG-INFO
```

### Comparing `streamlit_pandera-0.0.1/README.md` & `streamlit_pandera-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ```
 
 ## Usage instructions
 
 ```python
 import streamlit as st
 
-from streamlit_pandera.io_file_validator import run_validate_file
+from  import run_validate_file
 
 
 def validate():
     standards = {
         "store_schema": ("https://raw.githubusercontent.com/resilientinfrastructure/standards/main/panderas_schema.yml")
     }
     st.set_page_config(
```

### Comparing `streamlit_pandera-0.0.1/pyproject.toml` & `streamlit_pandera-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "streamlit_pandera"
-version = "0.0.1"
+version = "0.0.2"
 description = "Streamlit Data Validator Tool helps you validate your data with dataframe-type objects"
 authors = ["Manrique Vargas <machomaxg@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 streamlit = "^1.34.0"
 validators = "^0.28.1"
 pipx = "^1.5.0"
 cookiecutter = "^2.6.0"
 wheel = "*"
+io_file_validator = "^0.1.5"
 playwright = "1.39.0"
 requests = "2.31.0"
 pytest-playwright-snapshot = "1.0"
 pytest-rerunfailures = "12.0"
 pandera = { version = "^0.7.2", extras = ["io"] }
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 pytest = "*"
 pylint = "^3.2.0"
 twine = "*"
-pydiggs = "0.1.3"
 lxml = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
```

### Comparing `streamlit_pandera-0.0.1/streamlit_pandera/io_file_validator/validate_file.py` & `streamlit_pandera-0.0.2/streamlit_pandera/Home.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import logging
 
 import streamlit as st
 import streamlit.components.v1 as components
 import validators
+from io_file_validator.validator import ValidatorDataframe
 from pandera.errors import SchemaError
 
-from streamlit_pandera.io_file_validator.validator import ValidatorDataframe
-
 logger = logging.getLogger(__name__)
 
 if "panderas_url" not in st.session_state:
     st.session_state["panderas_url"] = "Unassigned"
 
 
 def assign_panderas_url(panderas_url):
@@ -44,29 +43,28 @@
 
 def run_validation(validator, uploaded_file):
     try:
         dataframe = validator.run_validation(uploaded_file=uploaded_file)
     except SchemaError as e:
         st.error(
             f"""
-                Please fix file to match expected format in standard defined in URL and try again!!!
+                Please fix file and try again!!!\n\n\n
                 Validation failed with error message: {e}.
             """
         )
         return None
     return dataframe
 
 
 def run_validate_file(standards: dict, validator: ValidatorDataframe = None):
     """
     standards is a key value pair of name and url
     e.g.: 'inclinometr': 'https://path/to/panderas/url"""
     if not validator:
         validator = ValidatorDataframe(url=None, file_format="csv")
-    st.write("# Data Validation Tool Using Pandera Yaml Schemas! 📊")
     with st.sidebar:
         components.html(
             """
             <iframe src="https://github.com/sponsors/machov/button"
             title="Sponsor machov" height="32" width="114" style="border: 0;
             border-radius: 6px;"></iframe>
             """
@@ -83,7 +81,23 @@
                 dataframe = run_validation(validator=validator, uploaded_file=uploaded_file)
                 if dataframe is not None:
                     st.success("Validated dataframe! Dataframe head shown below: ")
                     st.dataframe(dataframe.head())
                     st.balloons()
                     return uploaded_file
     return None
+
+
+def run():
+    st.set_page_config(
+        page_title="Data Validator Home",
+        page_icon="📊",
+    )
+    st.write("# Data Validation Tool! 📊")
+    standards = {
+        "store_schema": ("https://raw.githubusercontent.com/resilientinfrastructure/standards/main/panderas_schema.yml")
+    }
+    run_validate_file(standards=standards)
+
+
+if __name__ == "__main__":
+    run()
```

### Comparing `streamlit_pandera-0.0.1/streamlit_pandera/pages/0_Instructions.py` & `streamlit_pandera-0.0.2/streamlit_pandera/pages/0_Instructions.py`

 * *Files identical despite different names*

### Comparing `streamlit_pandera-0.0.1/PKG-INFO` & `streamlit_pandera-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: streamlit_pandera
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streamlit Data Validator Tool helps you validate your data with dataframe-type objects
 Author: Manrique Vargas
 Author-email: machomaxg@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cookiecutter (>=2.6.0,<3.0.0)
+Requires-Dist: io_file_validator (>=0.1.5,<0.2.0)
 Requires-Dist: pandera[io] (>=0.7.2,<0.8.0)
 Requires-Dist: pipx (>=1.5.0,<2.0.0)
 Requires-Dist: playwright (==1.39.0)
 Requires-Dist: pytest-playwright-snapshot (==1.0)
 Requires-Dist: pytest-rerunfailures (==12.0)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: streamlit (>=1.34.0,<2.0.0)
@@ -44,15 +45,15 @@
 ```
 
 ## Usage instructions
 
 ```python
 import streamlit as st
 
-from streamlit_pandera.io_file_validator import run_validate_file
+from  import run_validate_file
 
 
 def validate():
     standards = {
         "store_schema": ("https://raw.githubusercontent.com/resilientinfrastructure/standards/main/panderas_schema.yml")
     }
     st.set_page_config(
```

