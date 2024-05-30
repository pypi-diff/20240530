# Comparing `tmp/textintegrityinspector-0.1.3.tar.gz` & `tmp/textintegrityinspector-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textintegrityinspector-0.1.3.tar", last modified: Wed May 29 14:20:14 2024, max compression
+gzip compressed data, was "textintegrityinspector-0.1.4.tar", last modified: Thu May 30 08:39:55 2024, max compression
```

## Comparing `textintegrityinspector-0.1.3.tar` & `textintegrityinspector-0.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 14:20:14.284883 textintegrityinspector-0.1.3/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 14:20:14.276883 textintegrityinspector-0.1.3/.github/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 14:20:14.280883 textintegrityinspector-0.1.3/.github/workflows/
--rw-r--r--   0     1001 root         (0)     3226 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/.github/workflows/build.yml
--rw-r--r--   0     1001 root         (0)     3493 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/.gitlab-ci.yml
--rw-r--r--   0     1001 root         (0)      266 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/.textIntegrityInspector.toml
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 14:20:14.280883 textintegrityinspector-0.1.3/.vscode/
--rw-r--r--   0     1001 root         (0)      982 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/.vscode/launch.json
--rw-r--r--   0     1001 root         (0)      498 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/.vscode/settings.json
--rw-r--r--   0     1001 root         (0)       45 2024-05-29 14:20:14.000000 textintegrityinspector-0.1.3/AUTHORS
--rw-r--r--   0     1001 root         (0)      186 2024-05-29 14:20:14.000000 textintegrityinspector-0.1.3/ChangeLog
--rw-r--r--   0     1001 root         (0)      465 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/Dockerfile
--rw-r--r--   0     1001 root         (0)     1069 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/LICENSE
--rw-r--r--   0     1001 root         (0)      473 2024-05-29 14:20:14.284883 textintegrityinspector-0.1.3/PKG-INFO
--rw-r--r--   0     1001 root         (0)      281 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/Pipfile
--rw-r--r--   0     1001 root         (0)    34132 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/Pipfile.lock
--rw-r--r--   0     1001 root         (0)     2591 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/README.md
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 14:20:14.276883 textintegrityinspector-0.1.3/doc/
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 14:20:14.280883 textintegrityinspector-0.1.3/doc/images/
--rw-r--r--   0     1001 root         (0)   187520 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/doc/images/TextIntegrityLogo180.png
--rw-r--r--   0     1001 root         (0)       90 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/pyprojet.toml
--rw-r--r--   0     1001 root         (0)      446 2024-05-29 14:20:14.284883 textintegrityinspector-0.1.3/setup.cfg
--rw-r--r--   0     1001 root         (0)       75 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/setup.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 14:20:14.280883 textintegrityinspector-0.1.3/tests/
--rw-r--r--   0     1001 root         (0)        0 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/tests/__init__.py
--rw-r--r--   0     1001 root         (0)     3214 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/tests/test_main.py
--rw-r--r--   0     1001 root         (0)    13626 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/tests/test_validator.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 14:20:14.280883 textintegrityinspector-0.1.3/textIntegrityInspector/
--rw-r--r--   0     1001 root         (0)      205 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/textIntegrityInspector/__init__.py
--rw-r--r--   0     1001 root         (0)     4692 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/textIntegrityInspector/__main__.py
--rw-r--r--   0     1001 root         (0)     2715 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/textIntegrityInspector/languageData.py
--rw-r--r--   0     1001 root         (0)     6475 2024-05-29 14:19:47.000000 textintegrityinspector-0.1.3/textIntegrityInspector/validator.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-05-29 14:20:14.284883 textintegrityinspector-0.1.3/textIntegrityInspector.egg-info/
--rw-r--r--   0     1001 root         (0)      473 2024-05-29 14:20:14.000000 textintegrityinspector-0.1.3/textIntegrityInspector.egg-info/PKG-INFO
--rw-r--r--   0     1001 root         (0)      820 2024-05-29 14:20:14.000000 textintegrityinspector-0.1.3/textIntegrityInspector.egg-info/SOURCES.txt
--rw-r--r--   0     1001 root         (0)        1 2024-05-29 14:20:14.000000 textintegrityinspector-0.1.3/textIntegrityInspector.egg-info/dependency_links.txt
--rw-r--r--   0     1001 root         (0)       80 2024-05-29 14:20:14.000000 textintegrityinspector-0.1.3/textIntegrityInspector.egg-info/entry_points.txt
--rw-r--r--   0     1001 root         (0)        1 2024-05-29 14:20:14.000000 textintegrityinspector-0.1.3/textIntegrityInspector.egg-info/not-zip-safe
--rw-r--r--   0     1001 root         (0)       47 2024-05-29 14:20:14.000000 textintegrityinspector-0.1.3/textIntegrityInspector.egg-info/pbr.json
--rw-r--r--   0     1001 root         (0)       54 2024-05-29 14:20:14.000000 textintegrityinspector-0.1.3/textIntegrityInspector.egg-info/requires.txt
--rw-r--r--   0     1001 root         (0)       23 2024-05-29 14:20:14.000000 textintegrityinspector-0.1.3/textIntegrityInspector.egg-info/top_level.txt
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-30 08:39:55.602939 textintegrityinspector-0.1.4/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-30 08:39:55.590938 textintegrityinspector-0.1.4/.github/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-30 08:39:55.594938 textintegrityinspector-0.1.4/.github/workflows/
+-rw-r--r--   0     1001 root         (0)     4068 2024-05-30 08:39:26.000000 textintegrityinspector-0.1.4/.github/workflows/build.yml
+-rw-r--r--   0     1001 root         (0)     3493 2024-05-30 08:39:26.000000 textintegrityinspector-0.1.4/.gitlab-ci.yml
+-rw-r--r--   0     1001 root         (0)      266 2024-05-30 08:39:26.000000 textintegrityinspector-0.1.4/.textIntegrityInspector.toml
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-30 08:39:55.594938 textintegrityinspector-0.1.4/.vscode/
+-rw-r--r--   0     1001 root         (0)      982 2024-05-30 08:39:26.000000 textintegrityinspector-0.1.4/.vscode/launch.json
+-rw-r--r--   0     1001 root         (0)      498 2024-05-30 08:39:26.000000 textintegrityinspector-0.1.4/.vscode/settings.json
+-rw-r--r--   0     1001 root         (0)      110 2024-05-30 08:39:55.000000 textintegrityinspector-0.1.4/AUTHORS
+-rw-r--r--   0     1001 root         (0)      333 2024-05-30 08:39:55.000000 textintegrityinspector-0.1.4/ChangeLog
+-rw-r--r--   0     1001 root         (0)      465 2024-05-30 08:39:26.000000 textintegrityinspector-0.1.4/Dockerfile
+-rw-r--r--   0     1001 root         (0)     1069 2024-05-30 08:39:26.000000 textintegrityinspector-0.1.4/LICENSE
+-rw-r--r--   0     1001 root         (0)      473 2024-05-30 08:39:55.602939 textintegrityinspector-0.1.4/PKG-INFO
+-rw-r--r--   0     1001 root         (0)      281 2024-05-30 08:39:26.000000 textintegrityinspector-0.1.4/Pipfile
+-rw-r--r--   0     1001 root         (0)    34132 2024-05-30 08:39:26.000000 textintegrityinspector-0.1.4/Pipfile.lock
+-rw-r--r--   0     1001 root         (0)     2591 2024-05-30 08:39:26.000000 textintegrityinspector-0.1.4/README.md
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-30 08:39:55.590938 textintegrityinspector-0.1.4/doc/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-30 08:39:55.594938 textintegrityinspector-0.1.4/doc/images/
+-rw-r--r--   0     1001 root         (0)   187520 2024-05-30 08:39:26.000000 textintegrityinspector-0.1.4/doc/images/TextIntegrityLogo180.png
+-rw-r--r--   0     1001 root         (0)       90 2024-05-30 08:39:26.000000 textintegrityinspector-0.1.4/pyprojet.toml
+-rw-r--r--   0     1001 root         (0)      446 2024-05-30 08:39:55.602939 textintegrityinspector-0.1.4/setup.cfg
+-rw-r--r--   0     1001 root         (0)       75 2024-05-30 08:39:26.000000 textintegrityinspector-0.1.4/setup.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-30 08:39:55.598938 textintegrityinspector-0.1.4/tests/
+-rw-r--r--   0     1001 root         (0)        0 2024-05-30 08:39:26.000000 textintegrityinspector-0.1.4/tests/__init__.py
+-rw-r--r--   0     1001 root         (0)     3214 2024-05-30 08:39:26.000000 textintegrityinspector-0.1.4/tests/test_main.py
+-rw-r--r--   0     1001 root         (0)    13626 2024-05-30 08:39:26.000000 textintegrityinspector-0.1.4/tests/test_validator.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-30 08:39:55.598938 textintegrityinspector-0.1.4/textIntegrityInspector/
+-rw-r--r--   0     1001 root         (0)      205 2024-05-30 08:39:26.000000 textintegrityinspector-0.1.4/textIntegrityInspector/__init__.py
+-rw-r--r--   0     1001 root         (0)     4692 2024-05-30 08:39:26.000000 textintegrityinspector-0.1.4/textIntegrityInspector/__main__.py
+-rw-r--r--   0     1001 root         (0)     2715 2024-05-30 08:39:26.000000 textintegrityinspector-0.1.4/textIntegrityInspector/languageData.py
+-rw-r--r--   0     1001 root         (0)     6475 2024-05-30 08:39:26.000000 textintegrityinspector-0.1.4/textIntegrityInspector/validator.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-30 08:39:55.598938 textintegrityinspector-0.1.4/textIntegrityInspector.egg-info/
+-rw-r--r--   0     1001 root         (0)      473 2024-05-30 08:39:55.000000 textintegrityinspector-0.1.4/textIntegrityInspector.egg-info/PKG-INFO
+-rw-r--r--   0     1001 root         (0)      820 2024-05-30 08:39:55.000000 textintegrityinspector-0.1.4/textIntegrityInspector.egg-info/SOURCES.txt
+-rw-r--r--   0     1001 root         (0)        1 2024-05-30 08:39:55.000000 textintegrityinspector-0.1.4/textIntegrityInspector.egg-info/dependency_links.txt
+-rw-r--r--   0     1001 root         (0)       80 2024-05-30 08:39:55.000000 textintegrityinspector-0.1.4/textIntegrityInspector.egg-info/entry_points.txt
+-rw-r--r--   0     1001 root         (0)        1 2024-05-30 08:39:55.000000 textintegrityinspector-0.1.4/textIntegrityInspector.egg-info/not-zip-safe
+-rw-r--r--   0     1001 root         (0)       47 2024-05-30 08:39:55.000000 textintegrityinspector-0.1.4/textIntegrityInspector.egg-info/pbr.json
+-rw-r--r--   0     1001 root         (0)       54 2024-05-30 08:39:55.000000 textintegrityinspector-0.1.4/textIntegrityInspector.egg-info/requires.txt
+-rw-r--r--   0     1001 root         (0)       23 2024-05-30 08:39:55.000000 textintegrityinspector-0.1.4/textIntegrityInspector.egg-info/top_level.txt
```

### Comparing `textintegrityinspector-0.1.3/.github/workflows/build.yml` & `textintegrityinspector-0.1.4/.github/workflows/build.yml`

 * *Files 16% similar despite different names*

```diff
@@ -41,16 +41,14 @@
       - name: Run build
         run: |
           PATH=$PATH:/github/home/.local/bin
           git log
           python -V                                   # Print out python version for debugging
           echo 'pip install pipenv'
           pip install pipenv
-          echo 'rm -f .env'
-          rm -f .env
           echo 'pipenv install --dev'
           pipenv install --dev
           echo 'pipenv run pytest  --cov-report=xml:coverage.xml  --cov=textIntegrityInspector/  --junit-xml=junit.xml --cov-report term'
           pipenv run pytest  --cov-report=xml:coverage.xml  --cov=textIntegrityInspector/  --junit-xml=junit.xml --cov-report term
           echo ' pipenv requirements > requirements.txt'
           pipenv requirements > requirements.txt
           echo 'sed -i "s/==/>=/" requirements.txt'
@@ -59,15 +57,15 @@
           pipenv run python -m build 
       - name: Upload dist directory
         uses: actions/upload-artifact@v3
         with:
           name: dist-files
           path: dist/*
   # Publish the wheel to PyPI
-  deploy:
+  deploy-PyPi:
     if: github.event_name == 'release'
     needs: build
     runs-on: ubuntu-latest
     environment:
       name: pypi
       url: https://pypi.org/p/textIntegrityInspector
     permissions:
@@ -79,23 +77,50 @@
           set-safe-directory: true
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: '3.8'
       - name: Download dist directory
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v3  
         with:
           name: dist-files
           path: dist
 
       - name: Install dependencies
         run: |
           echo 'pip install pipenv'
           pip install pipenv
-          echo 'rm -f .env'
-          rm -f .env
           echo 'pipenv install --dev'
           pipenv install --dev
 
       - name: Publish package distributions to PyPI
-        uses: pypa/gh-action-pypi-publish@release/v1
+        uses: pypa/gh-action-pypi-publish@release/v1
+  deploy-docker:
+    runs-on: ubuntu-latest
+    needs:  build
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v4
+      - name: Download dist directory
+        uses: actions/download-artifact@v3  
+        with:
+          name: dist-files
+          path: dist
+      - name: Docker meta
+        id: meta
+        uses: docker/metadata-action@v5
+        with:
+          images: gaetanschneller12/text_integrity_inspector
+      - name: Login to DockerHub
+        if: github.event_name != 'pull_request'
+        uses: docker/login-action@v3
+        with:
+          username: ${{ secrets.DOCKERHUB_USERNAME }}
+          password: ${{ secrets.DOCKERHUB_TOKEN }}
+      - name: Build and push
+        uses: docker/build-push-action@v5
+        with:
+          context: .
+          push: ${{ github.event_name != 'pull_request' }}
+          tags: ${{ steps.meta.outputs.tags }}
+          labels: ${{ steps.meta.outputs.labels }}
```

### Comparing `textintegrityinspector-0.1.3/.gitlab-ci.yml` & `textintegrityinspector-0.1.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.3/.vscode/launch.json` & `textintegrityinspector-0.1.4/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.3/LICENSE` & `textintegrityinspector-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.3/Pipfile.lock` & `textintegrityinspector-0.1.4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.3/README.md` & `textintegrityinspector-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.3/doc/images/TextIntegrityLogo180.png` & `textintegrityinspector-0.1.4/doc/images/TextIntegrityLogo180.png`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.3/tests/test_main.py` & `textintegrityinspector-0.1.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.3/tests/test_validator.py` & `textintegrityinspector-0.1.4/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.3/textIntegrityInspector/__main__.py` & `textintegrityinspector-0.1.4/textIntegrityInspector/__main__.py`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.3/textIntegrityInspector/languageData.py` & `textintegrityinspector-0.1.4/textIntegrityInspector/languageData.py`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.3/textIntegrityInspector/validator.py` & `textintegrityinspector-0.1.4/textIntegrityInspector/validator.py`

 * *Files identical despite different names*

### Comparing `textintegrityinspector-0.1.3/textIntegrityInspector.egg-info/SOURCES.txt` & `textintegrityinspector-0.1.4/textIntegrityInspector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

