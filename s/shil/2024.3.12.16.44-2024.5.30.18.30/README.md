# Comparing `tmp/shil-2024.3.12.16.44.tar.gz` & `tmp/shil-2024.5.30.18.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shil-2024.3.12.16.44.tar", last modified: Tue Mar 12 16:44:59 2024, max compression
+gzip compressed data, was "shil-2024.5.30.18.30.tar", last modified: Thu May 30 18:30:50 2024, max compression
```

## Comparing `shil-2024.3.12.16.44.tar` & `shil-2024.5.30.18.30.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:44:59.564139 shil-2024.3.12.16.44/
--rw-r--r--   0 runner    (1001) docker     (127)     7820 2024-03-12 16:44:59.564139 shil-2024.3.12.16.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6703 2024-03-12 16:43:37.000000 shil-2024.3.12.16.44/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-12 16:44:59.564139 shil-2024.3.12.16.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-12 16:43:37.000000 shil-2024.3.12.16.44/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:44:59.556139 shil-2024.3.12.16.44/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:44:59.560139 shil-2024.3.12.16.44/src/shil/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-12 16:43:37.000000 shil-2024.3.12.16.44/src/shil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-03-12 16:43:37.000000 shil-2024.3.12.16.44/src/shil/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-12 16:44:56.000000 shil-2024.3.12.16.44/src/shil/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-12 16:43:37.000000 shil-2024.3.12.16.44/src/shil/bin.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-12 16:43:37.000000 shil-2024.3.12.16.44/src/shil/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:44:59.560139 shil-2024.3.12.16.44/src/shil/models/
--rw-r--r--   0 runner    (1001) docker     (127)     8823 2024-03-12 16:44:09.000000 shil-2024.3.12.16.44/src/shil/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-12 16:43:37.000000 shil-2024.3.12.16.44/src/shil/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:44:59.560139 shil-2024.3.12.16.44/src/shil/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-12 16:43:37.000000 shil-2024.3.12.16.44/src/shil/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-03-12 16:43:37.000000 shil-2024.3.12.16.44/src/shil/parser/grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-03-12 16:43:37.000000 shil-2024.3.12.16.44/src/shil/parser/semantics.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-12 16:43:37.000000 shil-2024.3.12.16.44/src/shil/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:44:59.560139 shil-2024.3.12.16.44/src/shil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7820 2024-03-12 16:44:59.000000 shil-2024.3.12.16.44/src/shil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-12 16:44:59.000000 shil-2024.3.12.16.44/src/shil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 16:44:59.000000 shil-2024.3.12.16.44/src/shil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 16:44:59.000000 shil-2024.3.12.16.44/src/shil.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-12 16:44:59.000000 shil-2024.3.12.16.44/src/shil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-12 16:44:59.000000 shil-2024.3.12.16.44/src/shil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:30:50.053870 shil-2024.5.30.18.30/
+-rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-05-30 18:30:50.053870 shil-2024.5.30.18.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6703 2024-05-30 18:29:22.000000 shil-2024.5.30.18.30/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-30 18:30:50.053870 shil-2024.5.30.18.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-30 18:29:22.000000 shil-2024.5.30.18.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:30:50.049870 shil-2024.5.30.18.30/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:30:50.049870 shil-2024.5.30.18.30/src/shil/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-30 18:29:22.000000 shil-2024.5.30.18.30/src/shil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-30 18:29:22.000000 shil-2024.5.30.18.30/src/shil/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-30 18:30:47.000000 shil-2024.5.30.18.30/src/shil/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-30 18:29:22.000000 shil-2024.5.30.18.30/src/shil/bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-30 18:29:22.000000 shil-2024.5.30.18.30/src/shil/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:30:50.049870 shil-2024.5.30.18.30/src/shil/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     8816 2024-05-30 18:29:56.000000 shil-2024.5.30.18.30/src/shil/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-30 18:29:22.000000 shil-2024.5.30.18.30/src/shil/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 18:29:22.000000 shil-2024.5.30.18.30/src/shil/models/docker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:30:50.053870 shil-2024.5.30.18.30/src/shil/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-30 18:29:22.000000 shil-2024.5.30.18.30/src/shil/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-05-30 18:29:22.000000 shil-2024.5.30.18.30/src/shil/parser/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-30 18:29:22.000000 shil-2024.5.30.18.30/src/shil/parser/semantics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-30 18:29:22.000000 shil-2024.5.30.18.30/src/shil/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:30:50.053870 shil-2024.5.30.18.30/src/shil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-05-30 18:30:50.000000 shil-2024.5.30.18.30/src/shil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-30 18:30:50.000000 shil-2024.5.30.18.30/src/shil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 18:30:50.000000 shil-2024.5.30.18.30/src/shil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 18:30:50.000000 shil-2024.5.30.18.30/src/shil.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-30 18:30:50.000000 shil-2024.5.30.18.30/src/shil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 18:30:50.000000 shil-2024.5.30.18.30/src/shil.egg-info/top_level.txt
```

### Comparing `shil-2024.3.12.16.44/PKG-INFO` & `shil-2024.5.30.18.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: shil
-Version: 2024.3.12.16.44
+Version: 2024.5.30.18.30
 Summary: Shell helper utilities for python
 Home-page: https://github.com/elo-enterprises/shil/
 Author: elo
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/shil/
 Project-URL: Source, https://github.com/elo-enterprises/shil/
 Project-URL: Download, https://github.com/elo-enterprises/shil/#files
 Platform: any
 Classifier: Programming Language :: Python
 Requires-Python: >3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Requires-Dist: TatSu==5.8.3
 Requires-Dist: pydantic==1.10.11
 Requires-Dist: fleks>=2024.2.9.23.58
-Requires-Dist: rich==13.3.4
+Requires-Dist: python-on-whales==0.71.0
 Provides-Extra: dev
 Requires-Dist: IPython; extra == "dev"
 Provides-Extra: testing
 Requires-Dist: IPython; extra == "testing"
 Requires-Dist: tox; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: shil Version: 2024.3.12.16.44 Summary: Shell helper
+Metadata-Version: 2.1 Name: shil Version: 2024.5.30.18.30 Summary: Shell helper
 utilities for python Home-page: https://github.com/elo-enterprises/shil/
 Author: elo License: MIT Project-URL: Documentation, https://github.com/elo-
 enterprises/shil/ Project-URL: Source, https://github.com/elo-enterprises/shil/
 Project-URL: Download, https://github.com/elo-enterprises/shil/#files Platform:
 any Classifier: Programming Language :: Python Requires-Python: >3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM Requires-
 Dist: TatSu==5.8.3 Requires-Dist: pydantic==1.10.11 Requires-Dist:
-fleks>=2024.2.9.23.58 Requires-Dist: rich==13.3.4 Provides-Extra: dev Requires-
-Dist: IPython; extra == "dev" Provides-Extra: testing Requires-Dist: IPython;
-extra == "testing" Requires-Dist: tox; extra == "testing" Requires-Dist:
-pytest; extra == "testing" Requires-Dist: pytest-cov; extra == "testing"
-Requires-Dist: mock; extra == "testing" Requires-Dist: flake8==5.0.4; extra ==
-"testing" Provides-Extra: lint Requires-Dist: tox; extra == "lint" Provides-
-Extra: publish Requires-Dist: twine; extra == "publish"
+fleks>=2024.2.9.23.58 Requires-Dist: python-on-whales==0.71.0 Provides-Extra:
+dev Requires-Dist: IPython; extra == "dev" Provides-Extra: testing Requires-
+Dist: IPython; extra == "testing" Requires-Dist: tox; extra == "testing"
+Requires-Dist: pytest; extra == "testing" Requires-Dist: pytest-cov; extra ==
+"testing" Requires-Dist: mock; extra == "testing" Requires-Dist: flake8==5.0.4;
+extra == "testing" Provides-Extra: lint Requires-Dist: tox; extra == "lint"
+Provides-Extra: publish Requires-Dist: twine; extra == "publish"
 sshhiill    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/_s_h_i_l_._s_v_g_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/
 _s_h_i_l_._s_v_g_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_l_o_-_e_n_t_e_r_p_r_i_s_e_s_/_s_h_i_l_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_p_y_t_h_o_n_-
 _p_u_b_l_i_s_h_._y_m_l_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_l_o_-_e_n_t_e_r_p_r_i_s_e_s_/_s_h_i_l_/_a_c_t_i_o_n_s_/
 _w_o_r_k_f_l_o_w_s_/_p_y_t_h_o_n_-_t_e_s_t_._y_m_l_/_b_a_d_g_e_._s_v_g_]
                                         Shell-util library for python.
 [https://raw.githubusercontent.com/elo- Includes helpers for subprocess
 enterprises/shil/master/img/icon.png]   invocation, shell-formatters / pretty-
```

### Comparing `shil-2024.3.12.16.44/README.md` & `shil-2024.5.30.18.30/README.md`

 * *Files identical despite different names*

### Comparing `shil-2024.3.12.16.44/setup.cfg` & `shil-2024.5.30.18.30/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -20,18 +20,22 @@
 zip_ok = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 python_requires = >3.7
 install_requires = 
+	
 	TatSu==5.8.3
+	
 	pydantic==1.10.11
+	
 	fleks>=2024.2.9.23.58
-	rich==13.3.4
+	
+	python-on-whales==0.71.0
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `shil-2024.3.12.16.44/setup.py` & `shil-2024.5.30.18.30/setup.py`

 * *Files identical despite different names*

### Comparing `shil-2024.3.12.16.44/src/shil/__main__.py` & `shil-2024.5.30.18.30/src/shil/__main__.py`

 * *Files identical despite different names*

### Comparing `shil-2024.3.12.16.44/src/shil/models/__init__.py` & `shil-2024.5.30.18.30/src/shil/models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,14 +29,18 @@
     strict: bool = Field(
         default=False,
         help="Fail if command fails",
     )
     shell: typing.Optional[bool] = Field(
         help="Fail if command fails",
     )
+    decoding: typing.Optional[bool] = Field(
+        default=True,
+        help="When True, results will be decoded as utf-8",
+    )
     interactive: bool = Field(
         default=False,
         help="Interactive mode",
     )
     large_output: bool = Field(
         default=False, help="Flag for indicating that output is huge"
     )
@@ -54,32 +58,22 @@
     )
     environment: dict = Field(
         default={},
         help="",
     )
     # log_stdin: bool = Field(default=True)
     system: bool = Field(
-        help='Execute command in "system" mode',
+        help="Execute command with os.system, bypassing subprocess module",
         default=False,
     )
     load_json: bool = Field(
         help="Load JSON from output",
         default=False,
     )
 
-    # @property
-    # def system(self):
-    #     """ """
-    #     tmp = self.__dict__.get("system", False)
-    #     if tmp:
-    #         if self.stdin or self.interactive:
-    #             err = f"{self} `system` cannot be used with `stdin`/`interactive`"
-    #             LOGGER.critical(err)
-    #             raise ValueError(err)
-
     def __rich_console__(self, _console, options):  # noqa
         """
         https://rich.readthedocs.io/en/stable/protocol.html
         """
         fmt = shfmt(self.command)
         extras = [
             f"[yellow]{attr}=1" if getattr(self, attr, None) else ""
@@ -152,15 +146,15 @@
                 self.command.split(),
                 shell=self.shell,
                 input=self.stdin.encode("utf-8"),
                 capture_output=True,
             )
             result.update(
                 pid=getattr(tmp, "pid", -1),
-                stdout=tmp.stdout.decode("utf-8"),
+                stdout=tmp.stdout.decode("utf-8") if self.decoding else tmp.stdout,
                 stderr=tmp.stderr,
                 return_code=tmp.returncode,
                 failed=tmp.returncode != 0,
             )
             result.update(
                 failure=result.failed,
                 succeeded=not result.failure,
@@ -177,15 +171,19 @@
             exec_cmd.wait()
             result.update(return_code=exec_cmd.returncode),
         if exec_cmd.stdout:
             result.update(
                 stdout=(
                     "<LargeOutput>"
                     if self.large_output
-                    else exec_cmd.stdout.read().decode("utf-8")
+                    else (
+                        exec_cmd.stdout.read().decode("utf-8")
+                        if self.decoding
+                        else exec_cmd.stdout.read()
+                    )
                 )
             )
             exec_cmd.stdout.close()
         else:
             exec_cmd.stdout = "<Interactive>"
             result.update(stdout="<Interactive>")
```

### Comparing `shil-2024.3.12.16.44/src/shil/parser/__init__.py` & `shil-2024.5.30.18.30/src/shil/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `shil-2024.3.12.16.44/src/shil/parser/grammar.py` & `shil-2024.5.30.18.30/src/shil/parser/grammar.py`

 * *Files identical despite different names*

### Comparing `shil-2024.3.12.16.44/src/shil/parser/semantics.py` & `shil-2024.5.30.18.30/src/shil/parser/semantics.py`

 * *Files identical despite different names*

### Comparing `shil-2024.3.12.16.44/src/shil/util.py` & `shil-2024.5.30.18.30/src/shil/util.py`

 * *Files identical despite different names*

### Comparing `shil-2024.3.12.16.44/src/shil.egg-info/PKG-INFO` & `shil-2024.5.30.18.30/src/shil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: shil
-Version: 2024.3.12.16.44
+Version: 2024.5.30.18.30
 Summary: Shell helper utilities for python
 Home-page: https://github.com/elo-enterprises/shil/
 Author: elo
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/shil/
 Project-URL: Source, https://github.com/elo-enterprises/shil/
 Project-URL: Download, https://github.com/elo-enterprises/shil/#files
 Platform: any
 Classifier: Programming Language :: Python
 Requires-Python: >3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Requires-Dist: TatSu==5.8.3
 Requires-Dist: pydantic==1.10.11
 Requires-Dist: fleks>=2024.2.9.23.58
-Requires-Dist: rich==13.3.4
+Requires-Dist: python-on-whales==0.71.0
 Provides-Extra: dev
 Requires-Dist: IPython; extra == "dev"
 Provides-Extra: testing
 Requires-Dist: IPython; extra == "testing"
 Requires-Dist: tox; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: shil Version: 2024.3.12.16.44 Summary: Shell helper
+Metadata-Version: 2.1 Name: shil Version: 2024.5.30.18.30 Summary: Shell helper
 utilities for python Home-page: https://github.com/elo-enterprises/shil/
 Author: elo License: MIT Project-URL: Documentation, https://github.com/elo-
 enterprises/shil/ Project-URL: Source, https://github.com/elo-enterprises/shil/
 Project-URL: Download, https://github.com/elo-enterprises/shil/#files Platform:
 any Classifier: Programming Language :: Python Requires-Python: >3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM Requires-
 Dist: TatSu==5.8.3 Requires-Dist: pydantic==1.10.11 Requires-Dist:
-fleks>=2024.2.9.23.58 Requires-Dist: rich==13.3.4 Provides-Extra: dev Requires-
-Dist: IPython; extra == "dev" Provides-Extra: testing Requires-Dist: IPython;
-extra == "testing" Requires-Dist: tox; extra == "testing" Requires-Dist:
-pytest; extra == "testing" Requires-Dist: pytest-cov; extra == "testing"
-Requires-Dist: mock; extra == "testing" Requires-Dist: flake8==5.0.4; extra ==
-"testing" Provides-Extra: lint Requires-Dist: tox; extra == "lint" Provides-
-Extra: publish Requires-Dist: twine; extra == "publish"
+fleks>=2024.2.9.23.58 Requires-Dist: python-on-whales==0.71.0 Provides-Extra:
+dev Requires-Dist: IPython; extra == "dev" Provides-Extra: testing Requires-
+Dist: IPython; extra == "testing" Requires-Dist: tox; extra == "testing"
+Requires-Dist: pytest; extra == "testing" Requires-Dist: pytest-cov; extra ==
+"testing" Requires-Dist: mock; extra == "testing" Requires-Dist: flake8==5.0.4;
+extra == "testing" Provides-Extra: lint Requires-Dist: tox; extra == "lint"
+Provides-Extra: publish Requires-Dist: twine; extra == "publish"
 sshhiill    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/_s_h_i_l_._s_v_g_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/
 _s_h_i_l_._s_v_g_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_l_o_-_e_n_t_e_r_p_r_i_s_e_s_/_s_h_i_l_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_p_y_t_h_o_n_-
 _p_u_b_l_i_s_h_._y_m_l_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_l_o_-_e_n_t_e_r_p_r_i_s_e_s_/_s_h_i_l_/_a_c_t_i_o_n_s_/
 _w_o_r_k_f_l_o_w_s_/_p_y_t_h_o_n_-_t_e_s_t_._y_m_l_/_b_a_d_g_e_._s_v_g_]
                                         Shell-util library for python.
 [https://raw.githubusercontent.com/elo- Includes helpers for subprocess
 enterprises/shil/master/img/icon.png]   invocation, shell-formatters / pretty-
```

