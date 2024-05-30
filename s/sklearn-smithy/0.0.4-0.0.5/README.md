# Comparing `tmp/sklearn_smithy-0.0.4.tar.gz` & `tmp/sklearn_smithy-0.0.5.tar.gz`

## Comparing `sklearn_smithy-0.0.4.tar` & `sklearn_smithy-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/sksmithy/__init__.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/sksmithy/__main__.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/sksmithy/_arguments.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/sksmithy/_callbacks.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/sksmithy/_logger.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/sksmithy/_models.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/sksmithy/_prompts.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/sksmithy/_utils.py
--rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/sksmithy/app.py
--rw-r--r--   0        0        0     7938 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/sksmithy/template.py.jinja
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/LICENSE
--rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/README.md
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     9256 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.5/sksmithy/__init__.py
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.5/sksmithy/__main__.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.5/sksmithy/_arguments.py
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.5/sksmithy/_callbacks.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.5/sksmithy/_logger.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.5/sksmithy/_models.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.5/sksmithy/_parsers.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.5/sksmithy/_prompts.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.5/sksmithy/_utils.py
+-rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.5/sksmithy/app.py
+-rw-r--r--   0        0        0     7938 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.5/sksmithy/template.py.jinja
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.5/LICENSE
+-rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.5/README.md
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     9256 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.5/PKG-INFO
```

### Comparing `sklearn_smithy-0.0.4/sksmithy/_arguments.py` & `sklearn_smithy-0.0.5/sksmithy/_arguments.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,111 @@
 from typing import Annotated
 
 from typer import Option
 
-from sksmithy._callbacks import args_callback, name_callback
+from sksmithy._callbacks import estimator_callback, name_callback, params_callback, tags_callback
 from sksmithy._models import EstimatorType
-from sksmithy._prompts import PROMPT_ESTIMATOR, PROMPT_NAME, PROMPT_OPTIONAL, PROMPT_REQUIRED, PROMPT_SAMPLE_WEIGHT
+from sksmithy._prompts import (
+    PROMPT_DECISION_FUNCTION,
+    PROMPT_ESTIMATOR,
+    PROMPT_LINEAR,
+    PROMPT_NAME,
+    PROMPT_OPTIONAL,
+    PROMPT_OUTPUT,
+    PROMPT_PREDICT_PROBA,
+    PROMPT_REQUIRED,
+    PROMPT_SAMPLE_WEIGHT,
+    PROMPT_TAGS,
+)
 
 name_arg = Annotated[
     str,
     Option(
         prompt=PROMPT_NAME,
+        prompt_required=False,
         help="[bold green]Name[/bold green] the estimator.",
         callback=name_callback,
     ),
 ]
 
 estimator_type_arg = Annotated[
     EstimatorType,
     Option(
         prompt=PROMPT_ESTIMATOR,
+        prompt_required=False,
         help="Estimator type.",
+        callback=estimator_callback,
     ),
 ]
 
 required_params_arg = Annotated[
     str,
     Option(
         prompt=PROMPT_REQUIRED,
         help="List of [bold green]required[/bold green] parameters (comma-separated).",
-        callback=args_callback,
+        callback=params_callback,
     ),
 ]
+
 optional_params_arg = Annotated[
     str,
     Option(
         prompt=PROMPT_OPTIONAL,
         help="List of [bold green]optional[/bold green] parameters (comma-separated).",
-        callback=args_callback,
+        callback=params_callback,
     ),
 ]
 
 sample_weight_arg = Annotated[
     bool,
     Option(
+        is_flag=True,
         prompt=PROMPT_SAMPLE_WEIGHT,
+        prompt_required=False,
         help="Whether or not `.fit()` does support [bold green]`sample_weight`[/bold green].",
     ),
 ]
+
+linear_arg = Annotated[
+    bool,
+    Option(
+        is_flag=True,
+        prompt=PROMPT_LINEAR,
+        help="Whether or not the estimator is [bold green]linear[/bold green].",
+    ),
+]
+
+predict_proba_arg = Annotated[
+    bool,
+    Option(
+        is_flag=True,
+        prompt=PROMPT_PREDICT_PROBA,
+        help="Whether or not the estimator implements [bold green]`predict_proba`[/bold green] method.",
+    ),
+]
+
+decision_function_arg = Annotated[
+    bool,
+    Option(
+        is_flag=True,
+        prompt=PROMPT_DECISION_FUNCTION,
+        help="Whether or not the estimator implements [bold green]`decision_function`[/bold green] method.",
+    ),
+]
+
+tags_arg = Annotated[
+    str,
+    Option(
+        prompt=PROMPT_TAGS,
+        prompt_required=False,
+        help="List of optional scikit-learn [bold green]tags[/bold green].",
+        callback=tags_callback,
+    ),
+]
+
+output_file_arg = Annotated[
+    str,
+    Option(
+        prompt=PROMPT_OUTPUT,
+        help="[bold green]Destination file[/bold green] where to save the boilerplate code.",
+    ),
+]
```

### Comparing `sklearn_smithy-0.0.4/sksmithy/_callbacks.py` & `sklearn_smithy-0.0.5/sksmithy/_parsers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,64 @@
 from keyword import iskeyword
 
-from typer import BadParameter
-
-from sksmithy._logger import console
 from sksmithy._models import TagType
 
 
-def name_callback(name: str) -> str:
-    """Validate if `name` is a valid python class name."""
-    valid = name.isidentifier()
-    kw = iskeyword(name)
-
-    if not valid:
-        msg = f"{name} is not a valid class name in python!"
-        raise BadParameter(msg)
-    if kw:
-        msg = f"Careful: {name} is a python keyword!"
-        console.print(msg, style="warning")
+def name_parser(name: str | None) -> tuple[str, str]:
+    """Validate that `name` is a valid python class name."""
+    if name:
+        is_valid = name.isidentifier()
+        is_kw = iskeyword(name)
+
+        msg = (
+            f"`{name}` is not a valid python class name!"
+            if not is_valid
+            else f"`{name}` is a python reserved keyword!"
+            if is_kw
+            else ""
+        )
 
-    return name
+        return name, msg
+    return "", "Name cannot be empty!"
 
 
-def args_callback(params: str) -> str:
-    """Validate if `params` contains valid python names."""
+def params_parser(params: str | None) -> tuple[list[str], str]:
+    """Parse and validate that `params` contains valid python names."""
     if params:
         param_list = params.split(",")
         invalid = tuple(p for p in param_list if not p.isidentifier())
 
         if len(invalid) > 0:
             msg = f"The following parameters are invalid python identifiers: {invalid}"
-            raise BadParameter(msg)
+            return [], msg
 
         if len(set(param_list)) < len(param_list):
-            msg = "Found repeated parameter"
-            raise BadParameter(msg)
+            msg = "Found repeated parameters!"
+            return [], msg
+
+        return param_list, ""
+    return [], ""
+
 
-    return params
+def check_duplicates(required: list[str], optional: list[str]) -> str:
+    """Check that there are not duplicates between required and optional params."""
+    duplicated_params = set(required).intersection(set(optional))
 
+    return f"The following parameters are duplicated: {duplicated_params}" if duplicated_params else ""
 
-def parse_tags(tags: str) -> list[str]:
-    """Parse and validate `tags`."""
+
+def tags_parser(tags: str) -> tuple[list[str], str]:
+    """Parse and validate `tags` by comparing with sklearn list."""
     if tags:
         list_tag = tags.split(",")
         unavailable_tags = tuple(t for t in list_tag if t not in TagType.__members__)
-
-        if len(unavailable_tags):
-            msg = (
+        msg = (
+            (
                 f"The following tags are not available: {unavailable_tags}."
                 "\nPlease check the documentation at https://scikit-learn.org/dev/developers/develop.html#estimator-tags"
                 " to know which values are available."
             )
-            raise BadParameter(msg)
-        return list_tag
-    return []
+            if len(unavailable_tags)
+            else ""
+        )
+        return list_tag, msg
+    return [], ""
```

### Comparing `sklearn_smithy-0.0.4/sksmithy/_models.py` & `sklearn_smithy-0.0.5/sksmithy/_models.py`

 * *Files identical despite different names*

### Comparing `sklearn_smithy-0.0.4/sksmithy/_prompts.py` & `sklearn_smithy-0.0.5/sksmithy/_prompts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Final
 
 PROMPT_NAME: Final[str] = "🐍 How would you like to name the estimator?"
 PROMPT_ESTIMATOR: Final[str] = "🎯 Which kind of estimator is it?"
 PROMPT_REQUIRED: Final[str] = "📜 Please list the required parameters (comma-separated)"
-PROMPT_OPTIONAL: Final[str] = "📑 Please list the optional parameters (comma separated)"
+PROMPT_OPTIONAL: Final[str] = "📑 Please list the optional parameters (comma-separated)"
 PROMPT_SAMPLE_WEIGHT: Final[str] = "📶 Does the `.fit()` method support `sample_weight`?"
 
 PROMPT_LINEAR: Final[str] = "📏 Is the estimator linear?"
-PROMPT_PREDICT_PROBA: Final[str] = "🎲 Should the estimator have a `predict_proba` method?"
-PROMPT_DECISION_FUNCTION: Final[str] = "❓ Should the estimator have a `decision_function` method?"
+PROMPT_PREDICT_PROBA: Final[str] = "🎲 Should the estimator implement a `predict_proba` method?"
+PROMPT_DECISION_FUNCTION: Final[str] = "❓ Should the estimator implement a `decision_function` method?"
 PROMPT_TAGS: Final[str] = (
-    "🧪 We are almost there... Are there any tag you want to add? (comma or space separated)\n"
+    "🧪 We are almost there... Is there any tag you want to add? (comma or space separated)\n"
     "To know more about tags, check the documentation at:\n"
     "https://scikit-learn.org/dev/developers/develop.html#estimator-tags"
 )
 
 PROMPT_OUTPUT: Final[str] = "📂 Where would you like to save the class?"
```

### Comparing `sklearn_smithy-0.0.4/sksmithy/_utils.py` & `sklearn_smithy-0.0.5/sksmithy/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from typing import Final
 
 from jinja2 import Template
 
 from sksmithy._models import EstimatorType
 
-TEMPLATE_PATH: Final[Path] = resources.files("sksmithy") / "template.py.jinja"  # type: ignore[assignment]
+TEMPLATE_PATH: Final[Path] = Path(str(resources.files("sksmithy") / "template.py.jinja"))
 
 
 def render_template(
     name: str,
     estimator_type: EstimatorType,
     required: list[str],
     optional: list[str],
```

### Comparing `sklearn_smithy-0.0.4/sksmithy/app.py` & `sklearn_smithy-0.0.5/sksmithy/app.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # streamlit run sksmithy/app.py
 import re
 import time
 from importlib.metadata import version
+from typing import Literal
 
 from sksmithy._models import EstimatorType
+from sksmithy._parsers import check_duplicates, name_parser, params_parser
 from sksmithy._prompts import (
     PROMPT_DECISION_FUNCTION,
     PROMPT_ESTIMATOR,
     PROMPT_LINEAR,
     PROMPT_NAME,
     PROMPT_OPTIONAL,
     PROMPT_PREDICT_PROBA,
@@ -62,122 +64,90 @@
         and not on the nitty-gritty details of the scikit-learn API.
 
         Once the core logic is implemented, the estimator should be ready to test against the _somewhat official_
         [`parametrize_with_checks`](https://scikit-learn.org/dev/modules/generated/sklearn.utils.estimator_checks.parametrize_with_checks.html#sklearn.utils.estimator_checks.parametrize_with_checks)
         pytest compatible decorator.
     """)
 
-estimator_type = None
+
 sample_weights = False
 linear = False
 predict_proba = False
 decision_function = False
+estimator_type: Literal[False] | EstimatorType = False
 
 if "forged_template" not in st.session_state:
     st.session_state["forged_template"] = ""
 
 if "forge_counter" not in st.session_state:
     st.session_state["forge_counter"] = 0
 
 with st.container():  # name and type
     c11, c12 = st.columns(2)
 
     with c11:  # name
-        name = st.text_input(
+        name_ = st.text_input(
             label=PROMPT_NAME,
             placeholder="MightyEstimator",
             help=(
                 "It should be a valid "
                 "[python identifier](https://docs.python.org/3/reference/lexical_analysis.html#identifiers)"
             ),
         )
 
-        if name and not name.isidentifier():
-            msg_invalid_name = f"`{name}` is not a valid python class name"
+        name, msg_invalid_name = name_parser(name_)
+
+        if name and msg_invalid_name:
             st.error(msg_invalid_name)
 
     with c12:  # type
         estimator = st.selectbox(
             label=PROMPT_ESTIMATOR,
             options=tuple(e.value for e in EstimatorType),
             format_func=lambda x: x.capitalize(),
             index=None,
         )
 
         if estimator:
             estimator_type = EstimatorType(estimator)
 
+
 with st.container():  # params
     c21, c22 = st.columns(2)
 
     with c21:  # required
         required_params = st.text_input(
             label=PROMPT_REQUIRED,
             placeholder="alpha,beta",
             help=(
                 "It should be a sequence of comma-separated "
                 "[python identifiers](https://docs.python.org/3/reference/lexical_analysis.html#identifiers)"
             ),
         )
 
-        if required_params:
-            required = required_params.split(",")
-            invalid_required = tuple(p for p in required if not p.isidentifier())
-
-            if len(invalid_required) > 0:
-                msg_invalid_required = (
-                    "The following required parameters are invalid "
-                    "[python identifiers](https://docs.python.org/3/reference/lexical_analysis.html#identifiers): "
-                    f"{invalid_required}"
-                )
-                st.error(msg_invalid_required)
-
-            if repeated_required := len(set(required)) < len(required):
-                msg_repeated_required = "Found repeated required parameters!"
-                st.error(msg_repeated_required)
-
-        else:
-            required = []
-            invalid_required = False
-            repeated_required = False
+        required, msg_invalid_required = params_parser(required_params)
+        if msg_invalid_required:
+            st.error(msg_invalid_required)
 
     with c22:  # optional
         optional_params = st.text_input(
             label=PROMPT_OPTIONAL,
             placeholder="mu,sigma",
             help=(
                 "It should be a sequence of comma-separated "
                 "[python identifiers](https://docs.python.org/3/reference/lexical_analysis.html#identifiers)"
             ),
         )
 
-        if optional_params:
-            optional = optional_params.split(",")
-            invalid_optional = tuple(p for p in optional if not p.isidentifier())
-
-            if len(invalid_optional) > 0:
-                msg_invalid_optional = (
-                    "The following optional parameters are invalid "
-                    "[python identifiers](https://docs.python.org/3/reference/lexical_analysis.html#identifiers): "
-                    f"{invalid_optional}"
-                )
-                st.error(msg_invalid_optional)
-
-            if repeated_optional := len(set(optional)) < len(optional):
-                msg_repeated_optional = "Found repeated optional parameters!"
-                st.error(msg_repeated_optional)
-
-        else:
-            optional = []
-            invalid_optional = False
-            repeated_optional = False
-
-    duplicated_params = set(required).intersection(set(optional))
-    if duplicated_params:
-        msg_duplicated_params = f"The following parameters are duplicated: {duplicated_params}"
+        optional, msg_invalid_optional = params_parser(optional_params)
+        if msg_invalid_optional:
+            st.error(msg_invalid_optional)
+
+    msg_duplicated_params = check_duplicates(required, optional)
+    if msg_duplicated_params:
         st.error(msg_duplicated_params)
 
 with st.container():  # sample_weight and linear
     c31, c32 = st.columns(2)
 
     with c31:  # sample_weight
         sample_weight = st.toggle(
@@ -212,45 +182,44 @@
                 "Available only if estimator is `Classifier`"
                 "Glossary: [decision_function](https://scikit-learn.org/dev/glossary.html#term-decision_function)"
             ),
         )
 
 st.write("#")  # empty space hack
 
-with st.container():  # forge button
+with st.container() as forge_row:  # forge button
     _, c52, _, c54 = st.columns([2, 1, 1, 1])
 
     with c52:
         forge_btn = st.button(
             label="Time to forge 🛠️",
             type="primary",
             disabled=any(
                 [
-                    name is None,
-                    estimator_type is None,
-                    invalid_required,
-                    invalid_optional,
-                    repeated_required,
-                    repeated_optional,
-                    duplicated_params,
+                    not name,
+                    not estimator_type,
+                    msg_invalid_name,
+                    msg_invalid_required,
+                    msg_duplicated_params,
                 ]
             ),
         )
         if forge_btn:
             st.session_state["forge_counter"] += 1
 
-        with c54, st.popover(label="Download", disabled=not st.session_state["forge_counter"]):
-            file_name = st.text_input(label="Select filename", value=f"{name.lower()}.py")
+    with c54, st.popover(label="Download", disabled=not st.session_state["forge_counter"]):
+        file_name = st.text_input(label="Select filename", value=f"{name.lower()}.py")
 
-            download_btn = st.download_button(
-                label="Confirm",
-                type="primary",
-                data=st.session_state["forged_template"],
-                file_name=file_name,
-            )
+        data = st.session_state["forged_template"]
+        download_btn = st.download_button(
+            label="Confirm",
+            type="primary",
+            data=data,
+            file_name=file_name,
+        )
 
 
 with st.container():  # code output
     if forge_btn:
         st.toast("Request submitted!")
         progress_text = "Forging in progress ..."
         progress_bar = st.progress(0, text=progress_text)
@@ -259,15 +228,15 @@
 
         for percent_complete in range(100):
             time.sleep(0.002)
             progress_bar.progress(percent_complete + 1, text=progress_text)
 
         st.session_state["forged_template"] = render_template(
             name=name,
-            estimator_type=estimator_type,
+            estimator_type=estimator_type,  # type: ignore[arg-type]
             required=required,
             optional=optional,
             linear=linear,
             sample_weight=sample_weight,
             predict_proba=predict_proba,
             decision_function=decision_function,
         )
```

### Comparing `sklearn_smithy-0.0.4/sksmithy/template.py.jinja` & `sklearn_smithy-0.0.5/sksmithy/template.py.jinja`

 * *Files identical despite different names*

### Comparing `sklearn_smithy-0.0.4/.gitignore` & `sklearn_smithy-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `sklearn_smithy-0.0.4/LICENSE` & `sklearn_smithy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn_smithy-0.0.4/README.md` & `sklearn_smithy-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sklearn_smithy-0.0.4/pyproject.toml` & `sklearn_smithy-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sklearn-smithy"
-version = "0.0.4"
+version = "0.0.5"
 
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [{name = "Francesco Bruzzesi"}]
 
 dependencies = [
```

### Comparing `sklearn_smithy-0.0.4/PKG-INFO` & `sklearn_smithy-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sklearn-smithy
-Version: 0.0.4
+Version: 0.0.5
 Author: Francesco Bruzzesi
 License: MIT License
         
         Copyright (c) 2024 Francesco Bruzzesi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

