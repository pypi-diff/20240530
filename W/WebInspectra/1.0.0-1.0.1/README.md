# Comparing `tmp/WebInspectra-1.0.0.tar.gz` & `tmp/webinspectra-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebInspectra-1.0.0.tar", last modified: Wed May 29 20:23:09 2024, max compression
+gzip compressed data, was "webinspectra-1.0.1.tar", last modified: Thu May 30 17:13:45 2024, max compression
```

## Comparing `WebInspectra-1.0.0.tar` & `webinspectra-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,25 @@
-drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-29 20:23:09.359455 WebInspectra-1.0.0/
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    35157 2024-05-29 19:56:36.000000 WebInspectra-1.0.0/LICENSE
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7447 2024-05-29 20:23:09.359455 WebInspectra-1.0.0/PKG-INFO
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6380 2024-05-29 20:03:21.000000 WebInspectra-1.0.0/README.md
-drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-29 20:23:09.355455 WebInspectra-1.0.0/WebInspectra.egg-info/
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7447 2024-05-29 20:23:09.000000 WebInspectra-1.0.0/WebInspectra.egg-info/PKG-INFO
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      305 2024-05-29 20:23:09.000000 WebInspectra-1.0.0/WebInspectra.egg-info/SOURCES.txt
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        1 2024-05-29 20:23:09.000000 WebInspectra-1.0.0/WebInspectra.egg-info/dependency_links.txt
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)       95 2024-05-29 20:23:09.000000 WebInspectra-1.0.0/WebInspectra.egg-info/requires.txt
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)       13 2024-05-29 20:23:09.000000 WebInspectra-1.0.0/WebInspectra.egg-info/top_level.txt
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)       38 2024-05-29 20:23:09.359455 WebInspectra-1.0.0/setup.cfg
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1503 2024-05-29 19:57:01.000000 WebInspectra-1.0.0/setup.py
-drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-29 20:23:09.355455 WebInspectra-1.0.0/webinspectra/
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)       64 2024-05-29 18:06:56.000000 WebInspectra-1.0.0/webinspectra/__init__.py
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      984 2024-05-29 19:57:07.000000 WebInspectra-1.0.0/webinspectra/__main__.py
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    18871 2024-05-29 19:57:27.000000 WebInspectra-1.0.0/webinspectra/inspectra.py
--rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9060 2024-05-27 19:30:04.000000 WebInspectra-1.0.0/webinspectra/webpage.py
+drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 17:13:45.220967 webinspectra-1.0.1/
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    35157 2024-05-29 19:56:36.000000 webinspectra-1.0.1/LICENSE
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      165 2024-05-30 16:44:15.000000 webinspectra-1.0.1/MANIFEST.in
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7668 2024-05-30 17:13:45.220967 webinspectra-1.0.1/PKG-INFO
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6383 2024-05-29 21:01:19.000000 webinspectra-1.0.1/README.md
+drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 17:13:45.220967 webinspectra-1.0.1/WebInspectra.egg-info/
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     7668 2024-05-30 17:13:45.000000 webinspectra-1.0.1/WebInspectra.egg-info/PKG-INFO
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      468 2024-05-30 17:13:45.000000 webinspectra-1.0.1/WebInspectra.egg-info/SOURCES.txt
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        1 2024-05-30 17:13:45.000000 webinspectra-1.0.1/WebInspectra.egg-info/dependency_links.txt
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      105 2024-05-30 17:13:45.000000 webinspectra-1.0.1/WebInspectra.egg-info/requires.txt
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)       13 2024-05-30 17:13:45.000000 webinspectra-1.0.1/WebInspectra.egg-info/top_level.txt
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)       38 2024-05-30 17:13:45.220967 webinspectra-1.0.1/setup.cfg
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     1518 2024-05-30 16:44:58.000000 webinspectra-1.0.1/setup.py
+drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 17:13:45.216967 webinspectra-1.0.1/tests/
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-27 19:54:40.000000 webinspectra-1.0.1/tests/__init__.py
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      996 2024-05-29 18:21:09.000000 webinspectra-1.0.1/tests/test_webinspectra.py
+drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 17:13:45.220967 webinspectra-1.0.1/webinspectra/
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)       64 2024-05-29 18:06:56.000000 webinspectra-1.0.1/webinspectra/__init__.py
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)      984 2024-05-29 19:57:07.000000 webinspectra-1.0.1/webinspectra/__main__.py
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)    18871 2024-05-29 19:57:27.000000 webinspectra-1.0.1/webinspectra/inspectra.py
+drwxr-xr-x   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 17:13:45.220967 webinspectra-1.0.1/webinspectra/utils/
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)        0 2024-05-30 16:38:14.000000 webinspectra-1.0.1/webinspectra/utils/__init__.py
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     3312 2024-04-17 19:29:48.000000 webinspectra-1.0.1/webinspectra/utils/selenium_utils.py
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     6701 2024-05-27 19:29:48.000000 webinspectra-1.0.1/webinspectra/utils/signature_utils.py
+-rw-r--r--   0 dockerizeddjangouser  (1000) dockerizeddjangouser  (1000)     9060 2024-05-27 19:30:04.000000 webinspectra-1.0.1/webinspectra/webpage.py
```

### Comparing `WebInspectra-1.0.0/LICENSE` & `webinspectra-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `WebInspectra-1.0.0/PKG-INFO` & `webinspectra-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 Metadata-Version: 2.1
 Name: WebInspectra
-Version: 1.0.0
-Summary: WebInspectra is a Python package designed for detecting web technologies used by a given URL. It provides a method to analyze the technologies powering a website, including frameworks, libraries, CDN usage, advertising platforms, and more. By leveraging various detection patterns and algorithms, WebInspectra identifies and categorizes the technologies utilized in the frontend and backend of web applications.
+Version: 1.0.1
+Summary: WebInspectra is a Python package designed for detecting web technologies used by a given URL. It provides a method to analyze the technologies powering a website, including frameworks, libraries, CDN usage, advertising platforms, and more. By using various detection patterns and algorithms, WebInspectra identifies and categorizes the technologies utilized in the frontend and backend of web applications.
 Home-page: https://github.com/insafm/WebInspectra
 Author: Mohammed Insaf M (insafm)
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: beautifulsoup4
+Requires-Dist: lxml
+Requires-Dist: requests
+Requires-Dist: selenium
+Requires-Dist: undetected-chromedriver
+Requires-Dist: dnspython
 Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
 Provides-Extra: logging
-License-File: LICENSE
+Requires-Dist: logging; extra == "logging"
 
 # WebInspectra
 
 WebInspectra is a Python package designed for detecting web technologies used by a given URL. It provides a method to analyze the technologies powering a website, including frameworks, libraries, CDN usage, advertising platforms, and more. By leveraging various detection patterns and algorithms, WebInspectra identifies and categorizes the technologies utilized in the frontend and backend of web applications.
 
 ## Features
-- Detects various web technologies and frameworks
-- Analyzes CDN usage and advertising platforms
-- Categorizes frontend and backend technologies
+- Detects various web technologies and frameworks.
+- Analyzes CDN usage and advertising platforms.
+- Categorizes frontend and backend technologies.
 
 ## Installation
 
 ### Prerequisites
 - Python 3.6 or higher
 - Google Chrome
 - Chromedriver
@@ -61,15 +68,15 @@
 mv chromedriver /usr/local/bin/ && \
 chmod +x /usr/local/bin/chromedriver && \
 rm chromedriver_linux64.zip
 ```
 
 ### Install WebInspectra
 ```bash
-pip install webinspectra
+pip install WebInspectra
 ```
 
 ## Usage
 WebInspectra can be used either as a command-line tool or as a Python module. Below are the detailed instructions for both methods.
 
 ### Command-Line Interface (CLI) Usage
 
@@ -155,9 +162,7 @@
 ## Contributions
 We welcome contributions! Please check the repository for contribution guidelines and open issues.
 
 ## License
 WebInspectra is released under the GNU General Public License v3.0 (GPL-3.0).
 
 We hope WebInspectra becomes an invaluable tool in your web development and security. Stay tuned for more updates and features in future releases!
-
-
```

### Comparing `WebInspectra-1.0.0/README.md` & `webinspectra-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # WebInspectra
 
 WebInspectra is a Python package designed for detecting web technologies used by a given URL. It provides a method to analyze the technologies powering a website, including frameworks, libraries, CDN usage, advertising platforms, and more. By leveraging various detection patterns and algorithms, WebInspectra identifies and categorizes the technologies utilized in the frontend and backend of web applications.
 
 ## Features
-- Detects various web technologies and frameworks
-- Analyzes CDN usage and advertising platforms
-- Categorizes frontend and backend technologies
+- Detects various web technologies and frameworks.
+- Analyzes CDN usage and advertising platforms.
+- Categorizes frontend and backend technologies.
 
 ## Installation
 
 ### Prerequisites
 - Python 3.6 or higher
 - Google Chrome
 - Chromedriver
@@ -40,15 +40,15 @@
 mv chromedriver /usr/local/bin/ && \
 chmod +x /usr/local/bin/chromedriver && \
 rm chromedriver_linux64.zip
 ```
 
 ### Install WebInspectra
 ```bash
-pip install webinspectra
+pip install WebInspectra
 ```
 
 ## Usage
 WebInspectra can be used either as a command-line tool or as a Python module. Below are the detailed instructions for both methods.
 
 ### Command-Line Interface (CLI) Usage
```

### Comparing `WebInspectra-1.0.0/WebInspectra.egg-info/PKG-INFO` & `webinspectra-1.0.1/WebInspectra.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 Metadata-Version: 2.1
 Name: WebInspectra
-Version: 1.0.0
-Summary: WebInspectra is a Python package designed for detecting web technologies used by a given URL. It provides a method to analyze the technologies powering a website, including frameworks, libraries, CDN usage, advertising platforms, and more. By leveraging various detection patterns and algorithms, WebInspectra identifies and categorizes the technologies utilized in the frontend and backend of web applications.
+Version: 1.0.1
+Summary: WebInspectra is a Python package designed for detecting web technologies used by a given URL. It provides a method to analyze the technologies powering a website, including frameworks, libraries, CDN usage, advertising platforms, and more. By using various detection patterns and algorithms, WebInspectra identifies and categorizes the technologies utilized in the frontend and backend of web applications.
 Home-page: https://github.com/insafm/WebInspectra
 Author: Mohammed Insaf M (insafm)
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: beautifulsoup4
+Requires-Dist: lxml
+Requires-Dist: requests
+Requires-Dist: selenium
+Requires-Dist: undetected-chromedriver
+Requires-Dist: dnspython
 Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
 Provides-Extra: logging
-License-File: LICENSE
+Requires-Dist: logging; extra == "logging"
 
 # WebInspectra
 
 WebInspectra is a Python package designed for detecting web technologies used by a given URL. It provides a method to analyze the technologies powering a website, including frameworks, libraries, CDN usage, advertising platforms, and more. By leveraging various detection patterns and algorithms, WebInspectra identifies and categorizes the technologies utilized in the frontend and backend of web applications.
 
 ## Features
-- Detects various web technologies and frameworks
-- Analyzes CDN usage and advertising platforms
-- Categorizes frontend and backend technologies
+- Detects various web technologies and frameworks.
+- Analyzes CDN usage and advertising platforms.
+- Categorizes frontend and backend technologies.
 
 ## Installation
 
 ### Prerequisites
 - Python 3.6 or higher
 - Google Chrome
 - Chromedriver
@@ -61,15 +68,15 @@
 mv chromedriver /usr/local/bin/ && \
 chmod +x /usr/local/bin/chromedriver && \
 rm chromedriver_linux64.zip
 ```
 
 ### Install WebInspectra
 ```bash
-pip install webinspectra
+pip install WebInspectra
 ```
 
 ## Usage
 WebInspectra can be used either as a command-line tool or as a Python module. Below are the detailed instructions for both methods.
 
 ### Command-Line Interface (CLI) Usage
 
@@ -155,9 +162,7 @@
 ## Contributions
 We welcome contributions! Please check the repository for contribution guidelines and open issues.
 
 ## License
 WebInspectra is released under the GNU General Public License v3.0 (GPL-3.0).
 
 We hope WebInspectra becomes an invaluable tool in your web development and security. Stay tuned for more updates and features in future releases!
-
-
```

### Comparing `WebInspectra-1.0.0/setup.py` & `webinspectra-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name="WebInspectra",
-    version="1.0.0",
-    description="WebInspectra is a Python package designed for detecting web technologies used by a given URL. It provides a method to analyze the technologies powering a website, including frameworks, libraries, CDN usage, advertising platforms, and more. By leveraging various detection patterns and algorithms, WebInspectra identifies and categorizes the technologies utilized in the frontend and backend of web applications.",
+    version="1.0.1",
+    description="WebInspectra is a Python package designed for detecting web technologies used by a given URL. It provides a method to analyze the technologies powering a website, including frameworks, libraries, CDN usage, advertising platforms, and more. By using various detection patterns and algorithms, WebInspectra identifies and categorizes the technologies utilized in the frontend and backend of web applications.",
     long_description=(pathlib.Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
     author="Mohammed Insaf M (insafm)",
     url="https://github.com/insafm/WebInspectra",
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
@@ -23,14 +23,15 @@
     license="GPLv3",
     install_requires=[
         'beautifulsoup4',
         'lxml',
         'requests',
         'selenium',
         'undetected-chromedriver',
+        'dnspython'
     ],
     extras_require={
         'dev': ["pytest"],
         'logging': ["logging"],
     },
     python_requires='>=3.6'
 )
```

### Comparing `WebInspectra-1.0.0/webinspectra/__main__.py` & `webinspectra-1.0.1/webinspectra/__main__.py`

 * *Files identical despite different names*

### Comparing `WebInspectra-1.0.0/webinspectra/inspectra.py` & `webinspectra-1.0.1/webinspectra/inspectra.py`

 * *Files identical despite different names*

### Comparing `WebInspectra-1.0.0/webinspectra/webpage.py` & `webinspectra-1.0.1/webinspectra/webpage.py`

 * *Files identical despite different names*

