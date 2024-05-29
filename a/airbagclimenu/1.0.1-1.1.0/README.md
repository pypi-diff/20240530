# Comparing `tmp/airbagclimenu-1.0.1.tar.gz` & `tmp/airbagclimenu-1.1.0.tar.gz`

## Comparing `airbagclimenu-1.0.1.tar` & `airbagclimenu-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    64770 2020-02-02 00:00:00.000000 airbagclimenu-1.0.1/qrcode.png
--rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 airbagclimenu-1.0.1/src/airbagclimenu/Menu.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airbagclimenu-1.0.1/src/airbagclimenu/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 airbagclimenu-1.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 airbagclimenu-1.0.1/LICENSE
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 airbagclimenu-1.0.1/README.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 airbagclimenu-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 airbagclimenu-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    64770 2020-02-02 00:00:00.000000 airbagclimenu-1.1.0/qrcode.png
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 airbagclimenu-1.1.0/src/airbagclimenu/Menu.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 airbagclimenu-1.1.0/src/airbagclimenu/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 airbagclimenu-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 airbagclimenu-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 airbagclimenu-1.1.0/README.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 airbagclimenu-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 airbagclimenu-1.1.0/PKG-INFO
```

### Comparing `airbagclimenu-1.0.1/qrcode.png` & `airbagclimenu-1.1.0/qrcode.png`

 * *Files identical despite different names*

### Comparing `airbagclimenu-1.0.1/LICENSE` & `airbagclimenu-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airbagclimenu-1.0.1/README.md` & `airbagclimenu-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -72,16 +72,23 @@
 ```Python
 menu = Menu.CLIMenu()
 def greet():
     print("Hello There!")
 
 menu.add_func(greet, "Say Hello")
 ```
-The function that is used **must** be parameterless, since there is no way of giving parameters as of now.
-
+As of version 1.1.0 the function used does now support parameters. If the function does not take arguments, it will just run it directly. If it however does take arguments, you will
+be prompted to enter these when you try to run the function via the menu. It will look like this: 
+```
+--- Args ---
+argument_1: <value of arugment>
+argument_2: <value of argument>
+------------ 
+```
+> The name of the argument will be displayed instead of ```argument_1``` etc.
 
 ## Example Program
 ```Python
 from airbagclimenu import Menu
 import random
 
 menu = Menu.CLIMenu()
```

### Comparing `airbagclimenu-1.0.1/pyproject.toml` & `airbagclimenu-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "airbagclimenu"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
     { name = "Anton Norman", email="normananton03@gmail.com" },
 ]
 description = "A python package that makes it easy and intuitive to create good looking CLI menus"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `airbagclimenu-1.0.1/PKG-INFO` & `airbagclimenu-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: airbagclimenu
-Version: 1.0.1
+Version: 1.1.0
 Summary: A python package that makes it easy and intuitive to create good looking CLI menus
 Project-URL: Homepage, https://github.com/Airbag65/CLI-Menu
 Project-URL: Issues, https://github.com/Airbag65/CLI-Menu/issues
 Author-email: Anton Norman <normananton03@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -86,16 +86,23 @@
 ```Python
 menu = Menu.CLIMenu()
 def greet():
     print("Hello There!")
 
 menu.add_func(greet, "Say Hello")
 ```
-The function that is used **must** be parameterless, since there is no way of giving parameters as of now.
-
+As of version 1.1.0 the function used does now support parameters. If the function does not take arguments, it will just run it directly. If it however does take arguments, you will
+be prompted to enter these when you try to run the function via the menu. It will look like this: 
+```
+--- Args ---
+argument_1: <value of arugment>
+argument_2: <value of argument>
+------------ 
+```
+> The name of the argument will be displayed instead of ```argument_1``` etc.
 
 ## Example Program
 ```Python
 from airbagclimenu import Menu
 import random
 
 menu = Menu.CLIMenu()
```

