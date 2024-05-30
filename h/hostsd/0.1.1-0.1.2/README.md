# Comparing `tmp/hostsd-0.1.1.tar.gz` & `tmp/hostsd-0.1.2.tar.gz`

## Comparing `hostsd-0.1.1.tar` & `hostsd-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 hostsd-0.1.1/.forgejo/workflows/pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hostsd-0.1.1/src/hostsd/__init__.py
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 hostsd-0.1.1/src/hostsd/__main__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 hostsd-0.1.1/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 hostsd-0.1.1/LICENSE
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 hostsd-0.1.1/README.md
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 hostsd-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 hostsd-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 hostsd-0.1.2/.forgejo/workflows/pypi.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hostsd-0.1.2/src/hostsd/__init__.py
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 hostsd-0.1.2/src/hostsd/__main__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 hostsd-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 hostsd-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 hostsd-0.1.2/README.md
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 hostsd-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 hostsd-0.1.2/PKG-INFO
```

### Comparing `hostsd-0.1.1/.forgejo/workflows/pypi.yml` & `hostsd-0.1.2/.forgejo/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `hostsd-0.1.1/src/hostsd/__main__.py` & `hostsd-0.1.2/src/hostsd/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,16 @@
             except UnicodeDecodeError:
                 print(f"File {infile.name} is not a text file - skipping")
                 return
 
             yield f"# {full_path}\n\n{filecontent}"
 
         elif infile.is_dir():
-            yield from read_directory(infile, full_path)
+            if not (infile.name.startswith(".") or infile.name.endswith(".disabled")):
+                yield from read_directory(infile, full_path)
 
 
 def get_new_content(dirpath: Union[str, PathLike] = HOSTS_DIR) -> str:
     """Read all files from a directory and join their contents in a string
 
     This will not read files with names that begin with a period ("."), or binary files.
```

### Comparing `hostsd-0.1.1/LICENSE` & `hostsd-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hostsd-0.1.1/README.md` & `hostsd-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,21 @@
 
 ## Installation
 
 ```bash
 pip install hostsd
 ```
 
+Now, to ensure that your existing `/etc/hosts` contents are retained, you can copy the file to `/etc/hosts.d/00-original`:
+
+```bash
+sudo mkdir /etc/hosts.d
+sudo cp /etc/hosts /etc/hosts.d/00-original
+```
+
 ## Usage
 
 To write the contents of `/etc/hosts.d/*` to `/etc/hosts`:
 
 ```bash
 sudo hostsd
 ```
```

### Comparing `hostsd-0.1.1/pyproject.toml` & `hostsd-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hostsd"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Kumi Mitterer", email="hostsd@kumi.email" },
 ]
 description = "A simple hosts file manager"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `hostsd-0.1.1/PKG-INFO` & `hostsd-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hostsd
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple hosts file manager
 Project-URL: Homepage, https://git.private.coffee/kumi/hostsd
 Project-URL: Bug Tracker, https://git.private.coffee/kumi/hostsd/issues
 Project-URL: Source Code, https://git.private.coffee/kumi/hostsd
 Author-email: Kumi Mitterer <hostsd@kumi.email>
 License: Copyright (c) 2023 Kumi Mitterer <hostsd@kumi.email>
         
@@ -49,14 +49,21 @@
 
 ## Installation
 
 ```bash
 pip install hostsd
 ```
 
+Now, to ensure that your existing `/etc/hosts` contents are retained, you can copy the file to `/etc/hosts.d/00-original`:
+
+```bash
+sudo mkdir /etc/hosts.d
+sudo cp /etc/hosts /etc/hosts.d/00-original
+```
+
 ## Usage
 
 To write the contents of `/etc/hosts.d/*` to `/etc/hosts`:
 
 ```bash
 sudo hostsd
 ```
```

