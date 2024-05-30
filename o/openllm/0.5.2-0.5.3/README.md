# Comparing `tmp/openllm-0.5.2.tar.gz` & `tmp/openllm-0.5.3.tar.gz`

## Comparing `openllm-0.5.2.tar` & `openllm-0.5.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    44456 2020-02-02 00:00:00.000000 openllm-0.5.2/CHANGELOG.md
--rw-r--r--   0        0        0    29599 2020-02-02 00:00:00.000000 openllm-0.5.2/README.md
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 openllm-0.5.2/pyoxidizer.bzl
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 openllm-0.5.2/src/_service_vars.pyi
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 openllm-0.5.2/src/_openllm_tiny/Dockerfile.j2
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 openllm-0.5.2/src/_openllm_tiny/__init__.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 openllm-0.5.2/src/_openllm_tiny/__init__.pyi
--rw-r--r--   0        0        0    22767 2020-02-02 00:00:00.000000 openllm-0.5.2/src/_openllm_tiny/_entrypoint.py
--rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 openllm-0.5.2/src/_openllm_tiny/_helpers.py
--rw-r--r--   0        0        0     7352 2020-02-02 00:00:00.000000 openllm-0.5.2/src/_openllm_tiny/_llm.py
--rw-r--r--   0        0        0     6556 2020-02-02 00:00:00.000000 openllm-0.5.2/src/_openllm_tiny/_service.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 openllm-0.5.2/src/_openllm_tiny/_service_vars.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 openllm-0.5.2/src/_openllm_tiny/_termui.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 openllm-0.5.2/src/_openllm_tiny/bentofile.yaml
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 openllm-0.5.2/src/_openllm_tiny/service.md
--rwxr-xr-x   0        0        0      459 2020-02-02 00:00:00.000000 openllm-0.5.2/src/_openllm_tiny/setup.sh
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/__init__.py
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/__init__.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/__main__.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/_deprecated.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/_generation.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/_generation.pyi
--rw-r--r--   0        0        0    19732 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/_llm.py
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/_llm.pyi
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/_quantisation.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/_quantisation.pyi
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/_runners.py
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/_runners.pyi
--rw-r--r--   0        0        0    12147 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/_strategies.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/_strategies.pyi
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/_version.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/client.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/client.pyi
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/py.typed
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/utils.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/utils.pyi
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/bundle/__init__.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/bundle/__init__.pyi
--rw-r--r--   0        0        0     6054 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/bundle/_package.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/bundle/_package.pyi
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/models/__init__.py
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/serialisation/__init__.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/serialisation/__init__.pyi
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/serialisation/_helpers.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/serialisation/constants.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/serialisation/ggml/__init__.py
--rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/serialisation/transformers/__init__.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/serialisation/transformers/_helpers.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/serialisation/transformers/weights.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm/serialisation/vllm/__init__.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm_cli/__init__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm_cli/entrypoint.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 openllm-0.5.2/src/openllm_cli/termui.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm-0.5.2/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.5.2/LICENSE.md
--rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 openllm-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    35954 2020-02-02 00:00:00.000000 openllm-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    44541 2020-02-02 00:00:00.000000 openllm-0.5.3/CHANGELOG.md
+-rw-r--r--   0        0        0    29599 2020-02-02 00:00:00.000000 openllm-0.5.3/README.md
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 openllm-0.5.3/pyoxidizer.bzl
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 openllm-0.5.3/src/_service_vars.pyi
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 openllm-0.5.3/src/_openllm_tiny/Dockerfile.j2
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 openllm-0.5.3/src/_openllm_tiny/__init__.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 openllm-0.5.3/src/_openllm_tiny/__init__.pyi
+-rw-r--r--   0        0        0    22767 2020-02-02 00:00:00.000000 openllm-0.5.3/src/_openllm_tiny/_entrypoint.py
+-rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 openllm-0.5.3/src/_openllm_tiny/_helpers.py
+-rw-r--r--   0        0        0     7352 2020-02-02 00:00:00.000000 openllm-0.5.3/src/_openllm_tiny/_llm.py
+-rw-r--r--   0        0        0     6556 2020-02-02 00:00:00.000000 openllm-0.5.3/src/_openllm_tiny/_service.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 openllm-0.5.3/src/_openllm_tiny/_service_vars.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 openllm-0.5.3/src/_openllm_tiny/_termui.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 openllm-0.5.3/src/_openllm_tiny/bentofile.yaml
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 openllm-0.5.3/src/_openllm_tiny/service.md
+-rwxr-xr-x   0        0        0      459 2020-02-02 00:00:00.000000 openllm-0.5.3/src/_openllm_tiny/setup.sh
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/__init__.py
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/__init__.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/__main__.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/_deprecated.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/_generation.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/_generation.pyi
+-rw-r--r--   0        0        0    19732 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/_llm.py
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/_llm.pyi
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/_quantisation.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/_quantisation.pyi
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/_runners.py
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/_runners.pyi
+-rw-r--r--   0        0        0    12147 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/_strategies.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/_strategies.pyi
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/_version.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/client.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/client.pyi
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/py.typed
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/utils.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/utils.pyi
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/bundle/__init__.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/bundle/__init__.pyi
+-rw-r--r--   0        0        0     6054 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/bundle/_package.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/bundle/_package.pyi
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/models/__init__.py
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/serialisation/__init__.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/serialisation/__init__.pyi
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/serialisation/_helpers.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/serialisation/constants.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/serialisation/ggml/__init__.py
+-rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/serialisation/transformers/__init__.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/serialisation/transformers/_helpers.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/serialisation/transformers/weights.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm/serialisation/vllm/__init__.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm_cli/__init__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm_cli/entrypoint.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 openllm-0.5.3/src/openllm_cli/termui.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm-0.5.3/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.5.3/LICENSE.md
+-rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 openllm-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0    35954 2020-02-02 00:00:00.000000 openllm-0.5.3/PKG-INFO
```

### Comparing `openllm-0.5.2/CHANGELOG.md` & `openllm-0.5.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 Do *NOT* add changelog entries here!
 
 This changelog is managed by towncrier and is compiled at release time.
 -->
 
 <!-- towncrier release notes start -->
 
+## [0.5.3](https://github.com/bentoml/openllm/tree/v0.5.3)
+No significant changes.
+
+
 ## [0.5.2](https://github.com/bentoml/openllm/tree/v0.5.2)
 No significant changes.
 
 
 ## [0.5.1](https://github.com/bentoml/openllm/tree/v0.5.1)
 No significant changes.
```

### Comparing `openllm-0.5.2/README.md` & `openllm-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/pyoxidizer.bzl` & `openllm-0.5.3/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/_openllm_tiny/__init__.pyi` & `openllm-0.5.3/src/_openllm_tiny/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/_openllm_tiny/_entrypoint.py` & `openllm-0.5.3/src/_openllm_tiny/_entrypoint.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/_openllm_tiny/_helpers.py` & `openllm-0.5.3/src/_openllm_tiny/_helpers.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/_openllm_tiny/_llm.py` & `openllm-0.5.3/src/_openllm_tiny/_llm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/_openllm_tiny/_service.py` & `openllm-0.5.3/src/_openllm_tiny/_service.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/_openllm_tiny/_service_vars.py` & `openllm-0.5.3/src/_openllm_tiny/_service_vars.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/_openllm_tiny/_termui.py` & `openllm-0.5.3/src/_openllm_tiny/_termui.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/_openllm_tiny/service.md` & `openllm-0.5.3/src/_openllm_tiny/service.md`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/__init__.py` & `openllm-0.5.3/src/openllm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/__init__.pyi` & `openllm-0.5.3/src/openllm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/_deprecated.py` & `openllm-0.5.3/src/openllm/_deprecated.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/_generation.py` & `openllm-0.5.3/src/openllm/_generation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/_llm.py` & `openllm-0.5.3/src/openllm/_llm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/_llm.pyi` & `openllm-0.5.3/src/openllm/_llm.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/_quantisation.py` & `openllm-0.5.3/src/openllm/_quantisation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/_quantisation.pyi` & `openllm-0.5.3/src/openllm/_quantisation.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/_runners.py` & `openllm-0.5.3/src/openllm/_runners.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/_runners.pyi` & `openllm-0.5.3/src/openllm/_runners.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/_strategies.py` & `openllm-0.5.3/src/openllm/_strategies.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/_strategies.pyi` & `openllm-0.5.3/src/openllm/_strategies.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/utils.py` & `openllm-0.5.3/src/openllm/utils.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/utils.pyi` & `openllm-0.5.3/src/openllm/utils.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/bundle/__init__.py` & `openllm-0.5.3/src/openllm/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/bundle/__init__.pyi` & `openllm-0.5.3/src/openllm/bundle/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/bundle/_package.py` & `openllm-0.5.3/src/openllm/bundle/_package.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/bundle/_package.pyi` & `openllm-0.5.3/src/openllm/bundle/_package.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/serialisation/__init__.py` & `openllm-0.5.3/src/openllm/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/serialisation/__init__.pyi` & `openllm-0.5.3/src/openllm/serialisation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/serialisation/_helpers.py` & `openllm-0.5.3/src/openllm/serialisation/_helpers.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/serialisation/transformers/__init__.py` & `openllm-0.5.3/src/openllm/serialisation/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/serialisation/transformers/_helpers.py` & `openllm-0.5.3/src/openllm/serialisation/transformers/_helpers.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/serialisation/transformers/weights.py` & `openllm-0.5.3/src/openllm/serialisation/transformers/weights.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/src/openllm/serialisation/vllm/__init__.py` & `openllm-0.5.3/src/openllm/serialisation/vllm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/.gitignore` & `openllm-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/LICENSE.md` & `openllm-0.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm-0.5.2/pyproject.toml` & `openllm-0.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -36,16 +36,16 @@
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     "bentoml[io]>=1.2.16",
     "transformers[torch,tokenizers]>=4.36.0",
-    "openllm-client>=0.5.2",
-    "openllm-core>=0.5.2",
+    "openllm-client>=0.5.3",
+    "openllm-core>=0.5.3",
     "safetensors",
     "vllm>=0.4.2",
     "optimum>=1.12.0",
     "accelerate",
     "ghapi",
     "einops",
     "sentencepiece",
```

### Comparing `openllm-0.5.2/PKG-INFO` & `openllm-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm
-Version: 0.5.2
+Version: 0.5.3
 Summary: OpenLLM: Run any open-source LLMs, such as Llama 2, Mistral, as OpenAI compatible API endpoint in the cloud.
 Project-URL: Blog, https://modelserving.com
 Project-URL: Chat, https://discord.gg/openllm
 Project-URL: Documentation, https://github.com/bentoml/openllm#readme
 Project-URL: GitHub, https://github.com/bentoml/OpenLLM
 Project-URL: History, https://github.com/bentoml/OpenLLM/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://bentoml.com
@@ -42,16 +42,16 @@
 Requires-Dist: bentoml[io]>=1.2.16
 Requires-Dist: bitsandbytes<0.42
 Requires-Dist: build[virtualenv]<1
 Requires-Dist: click>=8.1.3
 Requires-Dist: cuda-python; platform_system != 'Darwin'
 Requires-Dist: einops
 Requires-Dist: ghapi
-Requires-Dist: openllm-client>=0.5.2
-Requires-Dist: openllm-core>=0.5.2
+Requires-Dist: openllm-client>=0.5.3
+Requires-Dist: openllm-core>=0.5.3
 Requires-Dist: optimum>=1.12.0
 Requires-Dist: safetensors
 Requires-Dist: scipy
 Requires-Dist: sentencepiece
 Requires-Dist: transformers[tokenizers,torch]>=4.36.0
 Requires-Dist: vllm>=0.4.2
 Provides-Extra: agents
```

