# Comparing `tmp/isvirtual-1.2.0.tar.gz` & `tmp/isvirtual-1.3.0.tar.gz`

## Comparing `isvirtual-1.2.0.tar` & `isvirtual-1.3.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 isvirtual-1.2.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 isvirtual-1.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 isvirtual-1.2.0/src/VERSION.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 isvirtual-1.2.0/src/__init__.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 isvirtual-1.2.0/src/main.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 isvirtual-1.2.0/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 isvirtual-1.2.0/LICENSE
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 isvirtual-1.2.0/README.md
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 isvirtual-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 isvirtual-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 isvirtual-1.3.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 isvirtual-1.3.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 isvirtual-1.3.0/isvirtual/VERSION.md
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 isvirtual-1.3.0/isvirtual/__init__.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 isvirtual-1.3.0/isvirtual/cli.py
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 isvirtual-1.3.0/isvirtual/main.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 isvirtual-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 isvirtual-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 isvirtual-1.3.0/README.md
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 isvirtual-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 isvirtual-1.3.0/PKG-INFO
```

### Comparing `isvirtual-1.2.0/.github/workflows/publish.yml` & `isvirtual-1.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `isvirtual-1.2.0/.github/workflows/release.yml` & `isvirtual-1.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `isvirtual-1.2.0/LICENSE` & `isvirtual-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isvirtual-1.2.0/README.md` & `isvirtual-1.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -15,41 +15,41 @@
 # Usage
 
 This lib can be used within a python script or as a command line.
 
 ## Python
 Simple check:
 ```python
-from isvirtual import is_virtual_env
+from isvirtual import is_virtual
 
 if __name__ == "__main__":
     if is_virtual() is True:
         print("You are within a virtual environment which can either be venv, virtualenv or conda.")
     else:
         print("You are not in a virtual env")
 ```
 
 You can also check if you are specifically in a `venv`, `virtualenv` or `conda` environment:
 ```python
-from isvirtual import is_venv, is_virtualenv
+from isvirtual import is_venv, is_virtualenv, is_conda
 
 if __name__ == "__main__":
     if is_venv() is True:
         print("You are in a venv")
     elif is_virtualenv() is True:
         print("You are in a virtualenv")
     elif is_conda() is True:
         print("You are in a conda env")
     else:
         print("You are not in a any type of virtual env")
 ```
 
 You can also get the info from the env coming from `pyvenv.cfg` or load equivalent data from `conda` config. The `sys.prefix` data is added to the original config file under the key `prefix`:
 ```python
-from isvirtual import is_virtual_env, get_config
+from isvirtual import get_config
 
 if __name__ == "__main__":
     data = get_config()
     print(data["home"])
 ```
 Result:
 ```console
@@ -58,14 +58,35 @@
 version = 3.10.14
 prefix = /path/to/venv/dir
 prompt = nameOfYourProject
 ```
 
 Note that virtual environment created with `virtualenv` have more keys and the key `prompt` is not present by default in `venv` created environments.
 
+You can also check if the terminal from which the script has been launched is in a virtual env:
+```python
+if running_from_activated_env() is True:
+    print("The script is running from a terminal with an activated virtual env")
+```
+
+Note that this function check the existence of `VIRTUAL_ENV`. It is set by the activate script, but a virtual env can be used without activation by directly running an executable from the virtual env's bin/ (or Scripts on Windows) directory, in which case `VIRTUAL_ENV` will not be set. Or a non-virtual env Python binary can be executed directly while a virtual env is activated in the shell, in which case `VIRTUAL_ENV` may be set in a Python process that is not actually running in that virtual env.
+
+[Source](https://stackoverflow.com/a/1883251)
+
+You can find if a given directory is attached to a virtual env:
+```python
+from isvirtual import check_dir
+
+if __name__ == "__main__":
+    if check_dir("/some/dir/path") is True:
+        print("Virtual environment found")
+    else:
+        print("404 Not Found")
+```
+
 ## CLI
 ```console
 $ isvirtual
 Yes
 ```
 
 # License
```

### Comparing `isvirtual-1.2.0/pyproject.toml` & `isvirtual-1.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -22,25 +22,29 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
 ]
-keywords = ["virtual", "env", "venv", "virtualenv", "pyenv", "environment"]
-dependencies = []
+keywords = ["virtual", "env", "venv", "virtualenv", "environment", "poetry", "pipenv", "pdm"]
+dependencies = ["platformdirs", "typer"]
 
 [project.urls]
 Homepage = "https://github.com/AlexMili/isVirtual"
 Issues = "https://github.com/AlexMili/isVirtual/issues"
 Repository = "https://github.com/AlexMili/isVirtual"
 Documentation = "https://github.com/AlexMili/isVirtual"
 
 [project.scripts]
-isvirtual = "main:is_virtual_cli"
+isvirtual = "isvirtual.cli:app"
 
 [tool.hatch.build.targets.wheel]
-packages = ["./src"]
+packages = ["./isvirtual"]
 
 [tool.hatch.version]
-path = "src/VERSION.md"
+path = "isvirtual/VERSION.md"
 pattern = "(?P<version>.*)"
+
+[tool.ruff.lint.isort]
+lines-after-imports = 2
+known-first-party = ["isvirtual"]
```

### Comparing `isvirtual-1.2.0/PKG-INFO` & `isvirtual-1.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: isvirtual
-Version: 1.2.0
+Version: 1.3.0
 Summary: Detect if your script is running inside a virtual environment
 Project-URL: Homepage, https://github.com/AlexMili/isVirtual
 Project-URL: Issues, https://github.com/AlexMili/isVirtual/issues
 Project-URL: Repository, https://github.com/AlexMili/isVirtual
 Project-URL: Documentation, https://github.com/AlexMili/isVirtual
 Author: Alex Mili
 License: MIT License
@@ -25,15 +25,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
-Keywords: env,environment,pyenv,venv,virtual,virtualenv
+Keywords: env,environment,pdm,pipenv,poetry,venv,virtual,virtualenv
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -41,14 +41,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Requires-Python: >=3.3
+Requires-Dist: platformdirs
+Requires-Dist: typer
 Description-Content-Type: text/markdown
 
 **isVirtual** is a very simple tool to detect if the current script is within a virtual environment.
 
 # Disclaimer
 
 The goal of this project was to play around with the process to publish to [Pypi](https://pypi.org). The code of this module is coming from this [stackoverflow thread](https://stackoverflow.com/questions/1871549/how-to-determine-if-python-is-running-inside-a-virtualenv).
@@ -64,41 +66,41 @@
 # Usage
 
 This lib can be used within a python script or as a command line.
 
 ## Python
 Simple check:
 ```python
-from isvirtual import is_virtual_env
+from isvirtual import is_virtual
 
 if __name__ == "__main__":
     if is_virtual() is True:
         print("You are within a virtual environment which can either be venv, virtualenv or conda.")
     else:
         print("You are not in a virtual env")
 ```
 
 You can also check if you are specifically in a `venv`, `virtualenv` or `conda` environment:
 ```python
-from isvirtual import is_venv, is_virtualenv
+from isvirtual import is_venv, is_virtualenv, is_conda
 
 if __name__ == "__main__":
     if is_venv() is True:
         print("You are in a venv")
     elif is_virtualenv() is True:
         print("You are in a virtualenv")
     elif is_conda() is True:
         print("You are in a conda env")
     else:
         print("You are not in a any type of virtual env")
 ```
 
 You can also get the info from the env coming from `pyvenv.cfg` or load equivalent data from `conda` config. The `sys.prefix` data is added to the original config file under the key `prefix`:
 ```python
-from isvirtual import is_virtual_env, get_config
+from isvirtual import get_config
 
 if __name__ == "__main__":
     data = get_config()
     print(data["home"])
 ```
 Result:
 ```console
@@ -107,14 +109,35 @@
 version = 3.10.14
 prefix = /path/to/venv/dir
 prompt = nameOfYourProject
 ```
 
 Note that virtual environment created with `virtualenv` have more keys and the key `prompt` is not present by default in `venv` created environments.
 
+You can also check if the terminal from which the script has been launched is in a virtual env:
+```python
+if running_from_activated_env() is True:
+    print("The script is running from a terminal with an activated virtual env")
+```
+
+Note that this function check the existence of `VIRTUAL_ENV`. It is set by the activate script, but a virtual env can be used without activation by directly running an executable from the virtual env's bin/ (or Scripts on Windows) directory, in which case `VIRTUAL_ENV` will not be set. Or a non-virtual env Python binary can be executed directly while a virtual env is activated in the shell, in which case `VIRTUAL_ENV` may be set in a Python process that is not actually running in that virtual env.
+
+[Source](https://stackoverflow.com/a/1883251)
+
+You can find if a given directory is attached to a virtual env:
+```python
+from isvirtual import check_dir
+
+if __name__ == "__main__":
+    if check_dir("/some/dir/path") is True:
+        print("Virtual environment found")
+    else:
+        print("404 Not Found")
+```
+
 ## CLI
 ```console
 $ isvirtual
 Yes
 ```
 
 # License
```

