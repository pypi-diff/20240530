# Comparing `tmp/dbt_command_center-0.1.2.tar.gz` & `tmp/dbt_command_center-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_command_center-0.1.2.tar", last modified: Thu May 30 09:50:58 2024, max compression
+gzip compressed data, was "dbt_command_center-0.1.3.tar", last modified: Thu May 30 10:08:38 2024, max compression
```

## Comparing `dbt_command_center-0.1.2.tar` & `dbt_command_center-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:50:58.057651 dbt_command_center-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-30 09:50:17.000000 dbt_command_center-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-30 09:50:58.057651 dbt_command_center-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-30 09:50:17.000000 dbt_command_center-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:50:58.057651 dbt_command_center-0.1.2/dbt_command_center.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-30 09:50:58.000000 dbt_command_center-0.1.2/dbt_command_center.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-30 09:50:58.000000 dbt_command_center-0.1.2/dbt_command_center.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:50:58.000000 dbt_command_center-0.1.2/dbt_command_center.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 09:50:58.000000 dbt_command_center-0.1.2/dbt_command_center.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 09:50:58.000000 dbt_command_center-0.1.2/dbt_command_center.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 09:50:58.000000 dbt_command_center-0.1.2/dbt_command_center.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 09:50:58.057651 dbt_command_center-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-30 09:50:17.000000 dbt_command_center-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:50:58.057651 dbt_command_center-0.1.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 09:50:17.000000 dbt_command_center-0.1.2/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  3663778 2024-05-30 09:50:57.000000 dbt_command_center-0.1.2/src/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-30 09:50:17.000000 dbt_command_center-0.1.2/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:08:38.046618 dbt_command_center-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-30 10:07:51.000000 dbt_command_center-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-30 10:08:38.046618 dbt_command_center-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-30 10:07:51.000000 dbt_command_center-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:08:38.046618 dbt_command_center-0.1.3/dbt_command_center.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-30 10:08:38.000000 dbt_command_center-0.1.3/dbt_command_center.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-30 10:08:38.000000 dbt_command_center-0.1.3/dbt_command_center.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:08:38.000000 dbt_command_center-0.1.3/dbt_command_center.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 10:08:38.000000 dbt_command_center-0.1.3/dbt_command_center.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 10:08:38.000000 dbt_command_center-0.1.3/dbt_command_center.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 10:08:38.000000 dbt_command_center-0.1.3/dbt_command_center.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 10:08:38.046618 dbt_command_center-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-30 10:07:51.000000 dbt_command_center-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:08:38.046618 dbt_command_center-0.1.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:07:51.000000 dbt_command_center-0.1.3/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  3663778 2024-05-30 10:08:37.000000 dbt_command_center-0.1.3/src/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-30 10:07:51.000000 dbt_command_center-0.1.3/src/main.py
```

### Comparing `dbt_command_center-0.1.2/LICENSE` & `dbt_command_center-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_command_center-0.1.2/README.md` & `dbt_command_center-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # 🚀 dbt Command Center
 
 ## Local env setup
 
 - If you changed your web application run `npm run build` to update the build folder.
 
-- Run `rm -rf dist && cd web && npm run build && cd .. && python setup.py sdist bdist_wheel` to create source and binary distribution files in the dist/ directory.
+- Run `cd web && npm run build && cd .. && rm -rf dist && python setup.py sdist bdist_wheel` to create source and binary distribution files in the dist/ directory.
 
-- (Optional) Test your package locally by installing it with `pip install --force-reinstall --no-deps <path-to-git>/dbt-command-center/dist/dbt-command-center-0.1.1.tar.gz`
+- (Optional) Test your package locally by installing it with `pip install --force-reinstall --no-deps <path-to-git>/dbt-command-center/dist/dbt-command-center-0.1.2.tar.gz`
 
 ## Release a new version to PyPI
 
 - Don't forget to update the version in `setup.py`
 
 - Run `twine upload dist/*` to upload the distribution files to PyPI.
```

### Comparing `dbt_command_center-0.1.2/setup.py` & `dbt_command_center-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dbt-command-center",
-    version="0.1.2",
+    version="0.1.3",
     author="Montara team",
     author_email="support@montara.io",
     description="Stop drilling through dbt logs and start visualizing them",
     long_description="Stop drilling through dbt logs and start visualizing them",
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=["jsonlines"],
```

### Comparing `dbt_command_center-0.1.2/src/index.html` & `dbt_command_center-0.1.3/src/index.html`

 * *Files identical despite different names*

### Comparing `dbt_command_center-0.1.2/src/main.py` & `dbt_command_center-0.1.3/src/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                 return
         self.send_response(200)
         self.send_header("Content-type", "text/html")
         self.end_headers()
         self.wfile.write(file_content)
 
 
-def runWebServer(
+def run_web_server(
     server_class=HTTPServer, handler_class=SimpleHTTPRequestHandler, port=8000
 ):
     server_address = ("", port)
     httpd = server_class(server_address, handler_class)
     print(f"Server running on port {port}")
     httpd.serve_forever()
 
@@ -48,19 +48,14 @@
 def main():
     print("Starting Montara new", flush=True)
 
     # Create the montara_target directory if it doesn't exist
     print("Creating montara_target directory", flush=True)
     if not os.path.exists(MONTARA_TARGET):
         os.makedirs(MONTARA_TARGET)
-    # Else, clear the contents of the directory
-    else:
-        print("Clearing the contents of montara_target directory", flush=True)
-        for file in os.listdir(MONTARA_TARGET):
-            os.remove(f"{MONTARA_TARGET}/{file}")
 
     print(f'Compiling dbt and saving the output to "{MONTARA_TARGET}"', flush=True)
     subprocess.run(
         ["dbt", "parse", "--target-path", MONTARA_TARGET],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         universal_newlines=True,
@@ -72,15 +67,15 @@
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         universal_newlines=True,
     )
 
     print("Opening web browser", flush=True)
     # Open run in a different thread
-    run_thread = threading.Thread(target=runWebServer)
+    run_thread = threading.Thread(target=run_web_server)
     run_thread.start()
     webbrowser.open_new_tab("http://localhost:8000")
 
     print(f"Writing output to {MONTARA_TARGET}/output.jsonl", flush=True)
     print(f"Clearing the contents of {MONTARA_TARGET}/output.jsonl", flush=True)
     with open(f"{MONTARA_TARGET}/output.jsonl", "w") as file:
         file.write("")
```

