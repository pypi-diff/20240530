# Comparing `tmp/rstms_cloudflare-1.1.3.tar.gz` & `tmp/rstms_cloudflare-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstms_cloudflare-1.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rstms_cloudflare-1.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rstms_cloudflare-1.1.3.tar` & `rstms_cloudflare-1.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      383 2024-05-30 20:10:18.443714 rstms_cloudflare-1.1.3/.bumpversion.cfg
--rw-r--r--   0        0        0     1344 2024-05-21 01:52:37.934629 rstms_cloudflare-1.1.3/.gitignore
--rw-r--r--   0        0        0     1071 2024-04-16 03:08:46.805802 rstms_cloudflare-1.1.3/LICENSE
--rw-r--r--   0        0        0      539 2024-04-16 03:08:46.809802 rstms_cloudflare-1.1.3/Makefile
--rw-r--r--   0        0        0      689 2024-04-16 03:08:46.817802 rstms_cloudflare-1.1.3/README.md
--rw-r--r--   0        0        0        6 2024-05-30 20:10:18.439714 rstms_cloudflare-1.1.3/VERSION
--rw-r--r--   0        0        0      617 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.3/docs/Makefile
--rw-r--r--   0        0        0       97 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.3/docs/cli.rst
--rwxr-xr-x   0        0        0     4960 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.3/docs/conf.py
--rw-r--r--   0        0        0       33 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.3/docs/contributing.rst
--rw-r--r--   0        0        0      300 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.3/docs/index.rst
--rw-r--r--   0        0        0     1174 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.3/docs/installation.rst
--rw-r--r--   0        0        0      778 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.3/docs/make.bat
--rw-r--r--   0        0        0       27 2024-04-16 03:08:46.873802 rstms_cloudflare-1.1.3/docs/readme.rst
--rw-r--r--   0        0        0      431 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.3/make/browser.mk
--rw-r--r--   0        0        0      694 2024-04-16 03:08:46.845802 rstms_cloudflare-1.1.3/make/clean.mk
--rw-r--r--   0        0        0     3808 2024-04-16 03:08:46.837802 rstms_cloudflare-1.1.3/make/common.mk
--rw-r--r--   0        0        0      477 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.3/make/depends.mk
--rw-r--r--   0        0        0      441 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.3/make/dist.mk
--rw-r--r--   0        0        0      719 2024-04-16 03:08:46.825802 rstms_cloudflare-1.1.3/make/docs.mk
--rw-r--r--   0        0        0      668 2024-05-20 19:47:31.723566 rstms_cloudflare-1.1.3/make/lint.mk
--rw-r--r--   0        0        0     1214 2024-04-16 03:08:46.825802 rstms_cloudflare-1.1.3/make/publish.mk
--rw-r--r--   0        0        0      517 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.3/make/release.mk
--rw-r--r--   0        0        0      502 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.3/make/requirements.mk
--rw-r--r--   0        0        0      947 2024-04-16 03:08:46.821802 rstms_cloudflare-1.1.3/make/test.mk
--rw-r--r--   0        0        0     1610 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.3/make/version.mk
--rw-r--r--   0        0        0     1165 2024-05-30 20:10:18.443714 rstms_cloudflare-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      231 2024-04-16 03:08:46.789803 rstms_cloudflare-1.1.3/pytest.ini
--rw-r--r--   0        0        0       97 2024-05-30 20:10:18.295715 rstms_cloudflare-1.1.3/requirements-dev.txt
--rw-r--r--   0        0        0       47 2024-05-30 20:10:18.351714 rstms_cloudflare-1.1.3/requirements-docs.txt
--rw-r--r--   0        0        0       25 2024-05-30 20:10:18.239715 rstms_cloudflare-1.1.3/requirements.txt
--rw-r--r--   0        0        0      217 2024-04-16 03:18:17.194893 rstms_cloudflare-1.1.3/rstms_cloudflare/__init__.py
--rw-r--r--   0        0        0     6474 2024-05-29 03:01:48.275249 rstms_cloudflare-1.1.3/rstms_cloudflare/cli.py
--rw-r--r--   0        0        0     6182 2024-05-21 01:42:56.024690 rstms_cloudflare-1.1.3/rstms_cloudflare/cloudflare.py
--rw-r--r--   0        0        0     1065 2024-04-16 03:11:31.499807 rstms_cloudflare-1.1.3/rstms_cloudflare/exception_handler.py
--rw-r--r--   0        0        0     1092 2024-04-16 03:11:31.507807 rstms_cloudflare-1.1.3/rstms_cloudflare/shell.py
--rw-r--r--   0        0        0      127 2024-05-30 20:10:18.439714 rstms_cloudflare-1.1.3/rstms_cloudflare/version.py
--rw-r--r--   0        0        0       46 2024-04-16 03:08:46.849802 rstms_cloudflare-1.1.3/tests/__init__.py
--rw-r--r--   0        0        0     2266 2024-04-16 03:11:31.547806 rstms_cloudflare-1.1.3/tests/test_cli.py
--rw-r--r--   0        0        0      432 2024-04-16 03:08:46.789803 rstms_cloudflare-1.1.3/tox.ini
--rw-r--r--   0        0        0     1915 1970-01-01 00:00:00.000000 rstms_cloudflare-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      383 2024-05-30 20:13:23.433835 rstms_cloudflare-1.1.4/.bumpversion.cfg
+-rw-r--r--   0        0        0     1344 2024-05-21 01:52:37.934629 rstms_cloudflare-1.1.4/.gitignore
+-rw-r--r--   0        0        0     1071 2024-04-16 03:08:46.805802 rstms_cloudflare-1.1.4/LICENSE
+-rw-r--r--   0        0        0      539 2024-04-16 03:08:46.809802 rstms_cloudflare-1.1.4/Makefile
+-rw-r--r--   0        0        0      689 2024-04-16 03:08:46.817802 rstms_cloudflare-1.1.4/README.md
+-rw-r--r--   0        0        0        6 2024-05-30 20:13:23.429835 rstms_cloudflare-1.1.4/VERSION
+-rw-r--r--   0        0        0      617 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.4/docs/Makefile
+-rw-r--r--   0        0        0       97 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.4/docs/cli.rst
+-rwxr-xr-x   0        0        0     4960 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.4/docs/conf.py
+-rw-r--r--   0        0        0       33 2024-04-16 03:08:46.889801 rstms_cloudflare-1.1.4/docs/contributing.rst
+-rw-r--r--   0        0        0      300 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.4/docs/index.rst
+-rw-r--r--   0        0        0     1174 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.4/docs/installation.rst
+-rw-r--r--   0        0        0      778 2024-04-16 03:08:46.877802 rstms_cloudflare-1.1.4/docs/make.bat
+-rw-r--r--   0        0        0       27 2024-04-16 03:08:46.873802 rstms_cloudflare-1.1.4/docs/readme.rst
+-rw-r--r--   0        0        0      431 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.4/make/browser.mk
+-rw-r--r--   0        0        0      694 2024-04-16 03:08:46.845802 rstms_cloudflare-1.1.4/make/clean.mk
+-rw-r--r--   0        0        0     3808 2024-04-16 03:08:46.837802 rstms_cloudflare-1.1.4/make/common.mk
+-rw-r--r--   0        0        0      477 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.4/make/depends.mk
+-rw-r--r--   0        0        0      441 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.4/make/dist.mk
+-rw-r--r--   0        0        0      719 2024-04-16 03:08:46.825802 rstms_cloudflare-1.1.4/make/docs.mk
+-rw-r--r--   0        0        0      668 2024-05-20 19:47:31.723566 rstms_cloudflare-1.1.4/make/lint.mk
+-rw-r--r--   0        0        0     1268 2024-05-30 20:12:44.846227 rstms_cloudflare-1.1.4/make/publish.mk
+-rw-r--r--   0        0        0      517 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.4/make/release.mk
+-rw-r--r--   0        0        0      502 2024-04-16 03:08:46.829802 rstms_cloudflare-1.1.4/make/requirements.mk
+-rw-r--r--   0        0        0      947 2024-04-16 03:08:46.821802 rstms_cloudflare-1.1.4/make/test.mk
+-rw-r--r--   0        0        0     1610 2024-04-16 03:08:46.833802 rstms_cloudflare-1.1.4/make/version.mk
+-rw-r--r--   0        0        0     1165 2024-05-30 20:13:23.429835 rstms_cloudflare-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-04-16 03:08:46.789803 rstms_cloudflare-1.1.4/pytest.ini
+-rw-r--r--   0        0        0       97 2024-05-30 20:13:23.285837 rstms_cloudflare-1.1.4/requirements-dev.txt
+-rw-r--r--   0        0        0       47 2024-05-30 20:13:23.341836 rstms_cloudflare-1.1.4/requirements-docs.txt
+-rw-r--r--   0        0        0       25 2024-05-30 20:13:23.229837 rstms_cloudflare-1.1.4/requirements.txt
+-rw-r--r--   0        0        0      217 2024-04-16 03:18:17.194893 rstms_cloudflare-1.1.4/rstms_cloudflare/__init__.py
+-rw-r--r--   0        0        0     6474 2024-05-29 03:01:48.275249 rstms_cloudflare-1.1.4/rstms_cloudflare/cli.py
+-rw-r--r--   0        0        0     6182 2024-05-21 01:42:56.024690 rstms_cloudflare-1.1.4/rstms_cloudflare/cloudflare.py
+-rw-r--r--   0        0        0     1065 2024-04-16 03:11:31.499807 rstms_cloudflare-1.1.4/rstms_cloudflare/exception_handler.py
+-rw-r--r--   0        0        0     1092 2024-04-16 03:11:31.507807 rstms_cloudflare-1.1.4/rstms_cloudflare/shell.py
+-rw-r--r--   0        0        0      127 2024-05-30 20:13:23.429835 rstms_cloudflare-1.1.4/rstms_cloudflare/version.py
+-rw-r--r--   0        0        0       46 2024-04-16 03:08:46.849802 rstms_cloudflare-1.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     2266 2024-04-16 03:11:31.547806 rstms_cloudflare-1.1.4/tests/test_cli.py
+-rw-r--r--   0        0        0      432 2024-04-16 03:08:46.789803 rstms_cloudflare-1.1.4/tox.ini
+-rw-r--r--   0        0        0     1915 1970-01-01 00:00:00.000000 rstms_cloudflare-1.1.4/PKG-INFO
```

### Comparing `rstms_cloudflare-1.1.3/.gitignore` & `rstms_cloudflare-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.3/LICENSE` & `rstms_cloudflare-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.3/Makefile` & `rstms_cloudflare-1.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.3/README.md` & `rstms_cloudflare-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.3/docs/Makefile` & `rstms_cloudflare-1.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.3/docs/conf.py` & `rstms_cloudflare-1.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.3/docs/installation.rst` & `rstms_cloudflare-1.1.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.3/docs/make.bat` & `rstms_cloudflare-1.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.3/make/clean.mk` & `rstms_cloudflare-1.1.4/make/clean.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.3/make/common.mk` & `rstms_cloudflare-1.1.4/make/common.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.3/make/docs.mk` & `rstms_cloudflare-1.1.4/make/docs.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.3/make/lint.mk` & `rstms_cloudflare-1.1.4/make/lint.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.3/make/publish.mk` & `rstms_cloudflare-1.1.4/make/publish.mk`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 	if [ "$(version)" != "$(pypi_version)" ]; then \
 	  $(call verify_action,publish to PyPi) \
 	  echo publishing $(dist_name) $(version) to PyPI...;\
 	  flit publish;\
 	else \
 	  echo $(dist_name) $(version) is up-to-date on PyPI;\
 	fi
+	which devpi >/dev/null && devpi refresh $(dist_name)
 
 # check current pypi version 
 pypi-check:
 	$(call require_pypi_config)
 	@echo '$(dist_name) local=$(version) pypi=$(call check_pypi_version)'
 
 # clean up publish generated files
```

### Comparing `rstms_cloudflare-1.1.3/make/release.mk` & `rstms_cloudflare-1.1.4/make/release.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.3/make/test.mk` & `rstms_cloudflare-1.1.4/make/test.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.3/make/version.mk` & `rstms_cloudflare-1.1.4/make/version.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.3/pyproject.toml` & `rstms_cloudflare-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 requires_python = ">=3.10"
 
 
 
 [project]
 name = "rstms-cloudflare"
-version = "1.1.3"
+version = "1.1.4"
 authors = [{name = "Matt Krueger", email = "mkrueger@rstms.net"}]
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ["rstms_cloudflare"]
 classifiers = [
   "Intended Audience :: Developers",
```

### Comparing `rstms_cloudflare-1.1.3/rstms_cloudflare/cli.py` & `rstms_cloudflare-1.1.4/rstms_cloudflare/cli.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.3/rstms_cloudflare/cloudflare.py` & `rstms_cloudflare-1.1.4/rstms_cloudflare/cloudflare.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.3/rstms_cloudflare/exception_handler.py` & `rstms_cloudflare-1.1.4/rstms_cloudflare/exception_handler.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.3/rstms_cloudflare/shell.py` & `rstms_cloudflare-1.1.4/rstms_cloudflare/shell.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.3/tests/test_cli.py` & `rstms_cloudflare-1.1.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-1.1.3/PKG-INFO` & `rstms_cloudflare-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rstms-cloudflare
-Version: 1.1.3
+Version: 1.1.4
 Summary: Top-level package for rstms-cloudflare.
 Keywords: rstms_cloudflare
 Author-email: Matt Krueger <mkrueger@rstms.net>
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

