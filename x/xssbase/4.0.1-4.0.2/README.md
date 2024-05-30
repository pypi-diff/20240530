# Comparing `tmp/xssbase-4.0.1.tar.gz` & `tmp/xssbase-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xssbase-4.0.1.tar", last modified: Sun May 26 19:09:55 2024, max compression
+gzip compressed data, was "xssbase-4.0.2.tar", last modified: Thu May 30 16:29:09 2024, max compression
```

## Comparing `xssbase-4.0.1.tar` & `xssbase-4.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 19:09:55.650131 xssbase-4.0.1/
--rw-rw-rw-   0        0        0     1065 2024-05-26 12:22:40.000000 xssbase-4.0.1/LICENSE
--rw-rw-rw-   0        0        0     3223 2024-05-26 19:09:55.650131 xssbase-4.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2430 2024-05-26 15:37:45.000000 xssbase-4.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 19:09:55.650131 xssbase-4.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1081 2024-05-26 19:07:32.000000 xssbase-4.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 19:09:55.603265 xssbase-4.0.1/xssbase/
--rw-rw-rw-   0        0        0       20 2024-05-26 12:22:40.000000 xssbase-4.0.1/xssbase/__init__.py
--rw-rw-rw-   0        0        0     2016 2024-05-26 19:08:36.000000 xssbase-4.0.1/xssbase/cli.py
--rw-rw-rw-   0        0        0     5318 2024-05-26 15:31:08.000000 xssbase-4.0.1/xssbase/main.py
--rw-rw-rw-   0        0        0      739 2024-05-26 12:22:40.000000 xssbase-4.0.1/xssbase/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 19:09:55.650131 xssbase-4.0.1/xssbase.egg-info/
--rw-rw-rw-   0        0        0     3223 2024-05-26 19:09:55.000000 xssbase-4.0.1/xssbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-05-26 19:09:55.000000 xssbase-4.0.1/xssbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 19:09:55.000000 xssbase-4.0.1/xssbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-26 19:09:55.000000 xssbase-4.0.1/xssbase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2024-05-26 19:09:55.000000 xssbase-4.0.1/xssbase.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 19:09:55.000000 xssbase-4.0.1/xssbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 16:29:09.879288 xssbase-4.0.2/
+-rw-rw-rw-   0        0        0     1065 2024-05-30 16:28:17.000000 xssbase-4.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3722 2024-05-30 16:29:09.879288 xssbase-4.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2914 2024-05-30 16:28:17.000000 xssbase-4.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-30 16:29:09.879288 xssbase-4.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2024-05-30 16:28:18.000000 xssbase-4.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:29:09.809131 xssbase-4.0.2/xssbase/
+-rw-rw-rw-   0        0        0       20 2024-05-30 16:28:17.000000 xssbase-4.0.2/xssbase/__init__.py
+-rw-rw-rw-   0        0        0     2034 2024-05-30 16:28:17.000000 xssbase-4.0.2/xssbase/cli.py
+-rw-rw-rw-   0        0        0     5318 2024-05-30 16:28:17.000000 xssbase-4.0.2/xssbase/main.py
+-rw-rw-rw-   0        0        0      739 2024-05-30 16:28:17.000000 xssbase-4.0.2/xssbase/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:29:09.879288 xssbase-4.0.2/xssbase.egg-info/
+-rw-rw-rw-   0        0        0     3722 2024-05-30 16:29:09.000000 xssbase-4.0.2/xssbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-30 16:29:09.000000 xssbase-4.0.2/xssbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 16:29:09.000000 xssbase-4.0.2/xssbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-30 16:29:09.000000 xssbase-4.0.2/xssbase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2024-05-30 16:29:09.000000 xssbase-4.0.2/xssbase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-30 16:29:09.000000 xssbase-4.0.2/xssbase.egg-info/top_level.txt
```

### Comparing `xssbase-4.0.1/LICENSE` & `xssbase-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xssbase-4.0.1/PKG-INFO` & `xssbase-4.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 4.0.1
+Version: 4.0.2
 Summary: XSSbase: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal,cyber security
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,21 +17,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # XSSbase
 
 xssbase is a professional tool designed to help web developers scan for Cross-Site Scripting (XSS) vulnerabilities. It automates the process of testing web applications for XSS vulnerabilities by using a set of predefined payloads or custom payloads provided by the user.
 
+- Full Documentation : <a href="https://bytebreach.github.io/pdf/xssbase-Full-Commands.pdf">Link</a>
+- basic XSS (Cross-Site Scripting) vulnerable HTML code : <a href="https://github.com/ByteBreach/xssbase-test">Link</a>
+
 ## Features
 
 - **Automated XSS Testing**: Scans web applications for XSS vulnerabilities using a list of predefined or user-specified payloads.
 - **Platform Support**: Currently supports Windows.
 - **Custom Payloads**: Allows users to provide their own payloads for testing.
 - **Error Handling**: Handles stale element reference errors gracefully and retries automatically.
 - **Comprehensive Reports**: Provides detailed information about detected XSS vulnerabilities.
+- **Payload List URL**: Displays a URL to a list of useful XSS payloads.
 
 ## Benefits
 
 - **Time-Saving**: Automates the tedious process of testing for XSS vulnerabilities, saving developers valuable time.
 - **Improved Security**: Helps in identifying and fixing XSS vulnerabilities, enhancing the overall security of web applications.
 - **Customizable**: Users can use their own payloads for testing, making it highly customizable for specific needs.
 
@@ -65,16 +69,27 @@
 ```sh
 xssbase --url http://example.com
 ```
 To test http://example.com for XSS vulnerabilities using payloads from `custom-payloads.txt`:
 ```sh
 xssbase --url http://example.com --payload custom-payloads.txt
 ```
+### Displaying Payload List URL
+
+To print the URL of a useful list of XSS payloads:
+```sh
+xssbase --payload-list
+```
+
 ### Arguments
+
 `--url`: The URL to test for XSS vulnerabilities (required).
+
 `--payload`: The file containing custom XSS payloads (optional).
 
+`--payload-list` : Displays a URL to a list of useful XSS payloads.
+
 ### License
 This project is licensed under the MIT <a href="https://pypi.org/project/xssbase/#description">License</a>. See the LICENSE file for details.
 
 ### Disclaimer
 This tool is intended for educational purposes and for use by web developers to secure their own applications. Unauthorized or malicious use is strictly prohibited.
```

#### html2text {}

```diff
@@ -1,40 +1,44 @@
-Metadata-Version: 2.1 Name: xssbase Version: 4.0.1 Summary: XSSbase: A
+Metadata-Version: 2.1 Name: xssbase Version: 4.0.2 Summary: XSSbase: A
 professional tool for scanning XSS vulnerabilities. Home-page: https://
 mrfidal.in/cyber-security/xssbase Author: Fidal Author-email: mrfidal@proton.me
 License: MIT Keywords: xssbase,xss,vulnerability,scanning,mrfidal,cyber
 security Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 System Administrators Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: Security Description-Content-
 Type: text/markdown License-File: LICENSE # XSSbase xssbase is a professional
 tool designed to help web developers scan for Cross-Site Scripting (XSS)
 vulnerabilities. It automates the process of testing web applications for XSS
 vulnerabilities by using a set of predefined payloads or custom payloads
-provided by the user. ## Features - **Automated XSS Testing**: Scans web
-applications for XSS vulnerabilities using a list of predefined or user-
-specified payloads. - **Platform Support**: Currently supports Windows. -
+provided by the user. - Full Documentation : _L_i_n_k - basic XSS (Cross-Site
+Scripting) vulnerable HTML code : _L_i_n_k ## Features - **Automated XSS Testing**:
+Scans web applications for XSS vulnerabilities using a list of predefined or
+user-specified payloads. - **Platform Support**: Currently supports Windows. -
 **Custom Payloads**: Allows users to provide their own payloads for testing. -
 **Error Handling**: Handles stale element reference errors gracefully and
 retries automatically. - **Comprehensive Reports**: Provides detailed
-information about detected XSS vulnerabilities. ## Benefits - **Time-Saving**:
+information about detected XSS vulnerabilities. - **Payload List URL**:
+Displays a URL to a list of useful XSS payloads. ## Benefits - **Time-Saving**:
 Automates the tedious process of testing for XSS vulnerabilities, saving
 developers valuable time. - **Improved Security**: Helps in identifying and
 fixing XSS vulnerabilities, enhancing the overall security of web applications.
 - **Customizable**: Users can use their own payloads for testing, making it
 highly customizable for specific needs. Payload List : _C_l_i_c_k ## Installation
 Currently, xssbase is only compatible with Windows. To install, use the
 following command: ```sh pip install xssbase ``` ## Usage ### Basic Usage To
 test a URL for XSS vulnerabilities using the predefined payloads: ```sh xssbase
 --url ``` ### Using Custom Payloads To test a URL for XSS vulnerabilities using
 custom payloads from a file: ```sh xssbase --url --payload ``` ### Example To
 test http://example.com for XSS vulnerabilities using predefined payloads:
 ```sh xssbase --url http://example.com ``` To test http://example.com for XSS
 vulnerabilities using payloads from `custom-payloads.txt`: ```sh xssbase --url
-http://example.com --payload custom-payloads.txt ``` ### Arguments `--url`: The
-URL to test for XSS vulnerabilities (required). `--payload`: The file
-containing custom XSS payloads (optional). ### License This project is licensed
-under the MIT _L_i_c_e_n_s_e. See the LICENSE file for details. ### Disclaimer This
-tool is intended for educational purposes and for use by web developers to
-secure their own applications. Unauthorized or malicious use is strictly
-prohibited.
+http://example.com --payload custom-payloads.txt ``` ### Displaying Payload
+List URL To print the URL of a useful list of XSS payloads: ```sh xssbase --
+payload-list ``` ### Arguments `--url`: The URL to test for XSS vulnerabilities
+(required). `--payload`: The file containing custom XSS payloads (optional). `-
+-payload-list` : Displays a URL to a list of useful XSS payloads. ### License
+This project is licensed under the MIT _L_i_c_e_n_s_e. See the LICENSE file for
+details. ### Disclaimer This tool is intended for educational purposes and for
+use by web developers to secure their own applications. Unauthorized or
+malicious use is strictly prohibited.
```

### Comparing `xssbase-4.0.1/README.md` & `xssbase-4.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # XSSbase
 
 xssbase is a professional tool designed to help web developers scan for Cross-Site Scripting (XSS) vulnerabilities. It automates the process of testing web applications for XSS vulnerabilities by using a set of predefined payloads or custom payloads provided by the user.
 
+- Full Documentation : <a href="https://bytebreach.github.io/pdf/xssbase-Full-Commands.pdf">Link</a>
+- basic XSS (Cross-Site Scripting) vulnerable HTML code : <a href="https://github.com/ByteBreach/xssbase-test">Link</a>
+
 ## Features
 
 - **Automated XSS Testing**: Scans web applications for XSS vulnerabilities using a list of predefined or user-specified payloads.
 - **Platform Support**: Currently supports Windows.
 - **Custom Payloads**: Allows users to provide their own payloads for testing.
 - **Error Handling**: Handles stale element reference errors gracefully and retries automatically.
 - **Comprehensive Reports**: Provides detailed information about detected XSS vulnerabilities.
+- **Payload List URL**: Displays a URL to a list of useful XSS payloads.
 
 ## Benefits
 
 - **Time-Saving**: Automates the tedious process of testing for XSS vulnerabilities, saving developers valuable time.
 - **Improved Security**: Helps in identifying and fixing XSS vulnerabilities, enhancing the overall security of web applications.
 - **Customizable**: Users can use their own payloads for testing, making it highly customizable for specific needs.
 
@@ -46,16 +50,27 @@
 ```sh
 xssbase --url http://example.com
 ```
 To test http://example.com for XSS vulnerabilities using payloads from `custom-payloads.txt`:
 ```sh
 xssbase --url http://example.com --payload custom-payloads.txt
 ```
+### Displaying Payload List URL
+
+To print the URL of a useful list of XSS payloads:
+```sh
+xssbase --payload-list
+```
+
 ### Arguments
+
 `--url`: The URL to test for XSS vulnerabilities (required).
+
 `--payload`: The file containing custom XSS payloads (optional).
 
+`--payload-list` : Displays a URL to a list of useful XSS payloads.
+
 ### License
 This project is licensed under the MIT <a href="https://pypi.org/project/xssbase/#description">License</a>. See the LICENSE file for details.
 
 ### Disclaimer
 This tool is intended for educational purposes and for use by web developers to secure their own applications. Unauthorized or malicious use is strictly prohibited.
```

#### html2text {}

```diff
@@ -1,30 +1,35 @@
 # XSSbase xssbase is a professional tool designed to help web developers scan
 for Cross-Site Scripting (XSS) vulnerabilities. It automates the process of
 testing web applications for XSS vulnerabilities by using a set of predefined
-payloads or custom payloads provided by the user. ## Features - **Automated XSS
-Testing**: Scans web applications for XSS vulnerabilities using a list of
-predefined or user-specified payloads. - **Platform Support**: Currently
-supports Windows. - **Custom Payloads**: Allows users to provide their own
-payloads for testing. - **Error Handling**: Handles stale element reference
-errors gracefully and retries automatically. - **Comprehensive Reports**:
-Provides detailed information about detected XSS vulnerabilities. ## Benefits -
-**Time-Saving**: Automates the tedious process of testing for XSS
+payloads or custom payloads provided by the user. - Full Documentation : _L_i_n_k -
+basic XSS (Cross-Site Scripting) vulnerable HTML code : _L_i_n_k ## Features -
+**Automated XSS Testing**: Scans web applications for XSS vulnerabilities using
+a list of predefined or user-specified payloads. - **Platform Support**:
+Currently supports Windows. - **Custom Payloads**: Allows users to provide
+their own payloads for testing. - **Error Handling**: Handles stale element
+reference errors gracefully and retries automatically. - **Comprehensive
+Reports**: Provides detailed information about detected XSS vulnerabilities. -
+**Payload List URL**: Displays a URL to a list of useful XSS payloads. ##
+Benefits - **Time-Saving**: Automates the tedious process of testing for XSS
 vulnerabilities, saving developers valuable time. - **Improved Security**:
 Helps in identifying and fixing XSS vulnerabilities, enhancing the overall
 security of web applications. - **Customizable**: Users can use their own
 payloads for testing, making it highly customizable for specific needs. Payload
 List : _C_l_i_c_k ## Installation Currently, xssbase is only compatible with
 Windows. To install, use the following command: ```sh pip install xssbase ```
 ## Usage ### Basic Usage To test a URL for XSS vulnerabilities using the
 predefined payloads: ```sh xssbase --url ``` ### Using Custom Payloads To test
 a URL for XSS vulnerabilities using custom payloads from a file: ```sh xssbase
 --url --payload ``` ### Example To test http://example.com for XSS
 vulnerabilities using predefined payloads: ```sh xssbase --url http://
 example.com ``` To test http://example.com for XSS vulnerabilities using
 payloads from `custom-payloads.txt`: ```sh xssbase --url http://example.com --
-payload custom-payloads.txt ``` ### Arguments `--url`: The URL to test for XSS
-vulnerabilities (required). `--payload`: The file containing custom XSS
-payloads (optional). ### License This project is licensed under the MIT
-_L_i_c_e_n_s_e. See the LICENSE file for details. ### Disclaimer This tool is intended
-for educational purposes and for use by web developers to secure their own
-applications. Unauthorized or malicious use is strictly prohibited.
+payload custom-payloads.txt ``` ### Displaying Payload List URL To print the
+URL of a useful list of XSS payloads: ```sh xssbase --payload-list ``` ###
+Arguments `--url`: The URL to test for XSS vulnerabilities (required). `--
+payload`: The file containing custom XSS payloads (optional). `--payload-list`
+: Displays a URL to a list of useful XSS payloads. ### License This project is
+licensed under the MIT _L_i_c_e_n_s_e. See the LICENSE file for details. ###
+Disclaimer This tool is intended for educational purposes and for use by web
+developers to secure their own applications. Unauthorized or malicious use is
+strictly prohibited.
```

### Comparing `xssbase-4.0.1/setup.py` & `xssbase-4.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xssbase',
-    version='4.0.1',
+    version='4.0.2',
     description='XSSbase: A professional tool for scanning XSS vulnerabilities.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://mrfidal.in/cyber-security/xssbase',
     author='Fidal',
     author_email='mrfidal@proton.me',
     license='MIT',
```

### Comparing `xssbase-4.0.1/xssbase/cli.py` & `xssbase-4.0.2/xssbase/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     # Set up Chrome WebDriver
     service = Service('chromedriver-win64/chromedriver.exe')  # Specify the path to chromedriver executable
     driver = webdriver.Chrome(service=service)
 
     # Load payloads
     if args.payload:
-        with open(args.payload, 'r') as f:
+        with open(args.payload, 'r', encoding='utf-8') as f:
             payloads = [line.strip() for line in f.readlines()]
     else:
         payloads = xss_payloads_default
 
     try:
         # Test XSS payloads
         test_xss_payloads(driver, args.url, payloads)
```

### Comparing `xssbase-4.0.1/xssbase/main.py` & `xssbase-4.0.2/xssbase/main.py`

 * *Files identical despite different names*

### Comparing `xssbase-4.0.1/xssbase/utils.py` & `xssbase-4.0.2/xssbase/utils.py`

 * *Files identical despite different names*

### Comparing `xssbase-4.0.1/xssbase.egg-info/PKG-INFO` & `xssbase-4.0.2/xssbase.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 4.0.1
+Version: 4.0.2
 Summary: XSSbase: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal,cyber security
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,21 +17,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # XSSbase
 
 xssbase is a professional tool designed to help web developers scan for Cross-Site Scripting (XSS) vulnerabilities. It automates the process of testing web applications for XSS vulnerabilities by using a set of predefined payloads or custom payloads provided by the user.
 
+- Full Documentation : <a href="https://bytebreach.github.io/pdf/xssbase-Full-Commands.pdf">Link</a>
+- basic XSS (Cross-Site Scripting) vulnerable HTML code : <a href="https://github.com/ByteBreach/xssbase-test">Link</a>
+
 ## Features
 
 - **Automated XSS Testing**: Scans web applications for XSS vulnerabilities using a list of predefined or user-specified payloads.
 - **Platform Support**: Currently supports Windows.
 - **Custom Payloads**: Allows users to provide their own payloads for testing.
 - **Error Handling**: Handles stale element reference errors gracefully and retries automatically.
 - **Comprehensive Reports**: Provides detailed information about detected XSS vulnerabilities.
+- **Payload List URL**: Displays a URL to a list of useful XSS payloads.
 
 ## Benefits
 
 - **Time-Saving**: Automates the tedious process of testing for XSS vulnerabilities, saving developers valuable time.
 - **Improved Security**: Helps in identifying and fixing XSS vulnerabilities, enhancing the overall security of web applications.
 - **Customizable**: Users can use their own payloads for testing, making it highly customizable for specific needs.
 
@@ -65,16 +69,27 @@
 ```sh
 xssbase --url http://example.com
 ```
 To test http://example.com for XSS vulnerabilities using payloads from `custom-payloads.txt`:
 ```sh
 xssbase --url http://example.com --payload custom-payloads.txt
 ```
+### Displaying Payload List URL
+
+To print the URL of a useful list of XSS payloads:
+```sh
+xssbase --payload-list
+```
+
 ### Arguments
+
 `--url`: The URL to test for XSS vulnerabilities (required).
+
 `--payload`: The file containing custom XSS payloads (optional).
 
+`--payload-list` : Displays a URL to a list of useful XSS payloads.
+
 ### License
 This project is licensed under the MIT <a href="https://pypi.org/project/xssbase/#description">License</a>. See the LICENSE file for details.
 
 ### Disclaimer
 This tool is intended for educational purposes and for use by web developers to secure their own applications. Unauthorized or malicious use is strictly prohibited.
```

#### html2text {}

```diff
@@ -1,40 +1,44 @@
-Metadata-Version: 2.1 Name: xssbase Version: 4.0.1 Summary: XSSbase: A
+Metadata-Version: 2.1 Name: xssbase Version: 4.0.2 Summary: XSSbase: A
 professional tool for scanning XSS vulnerabilities. Home-page: https://
 mrfidal.in/cyber-security/xssbase Author: Fidal Author-email: mrfidal@proton.me
 License: MIT Keywords: xssbase,xss,vulnerability,scanning,mrfidal,cyber
 security Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 System Administrators Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: Security Description-Content-
 Type: text/markdown License-File: LICENSE # XSSbase xssbase is a professional
 tool designed to help web developers scan for Cross-Site Scripting (XSS)
 vulnerabilities. It automates the process of testing web applications for XSS
 vulnerabilities by using a set of predefined payloads or custom payloads
-provided by the user. ## Features - **Automated XSS Testing**: Scans web
-applications for XSS vulnerabilities using a list of predefined or user-
-specified payloads. - **Platform Support**: Currently supports Windows. -
+provided by the user. - Full Documentation : _L_i_n_k - basic XSS (Cross-Site
+Scripting) vulnerable HTML code : _L_i_n_k ## Features - **Automated XSS Testing**:
+Scans web applications for XSS vulnerabilities using a list of predefined or
+user-specified payloads. - **Platform Support**: Currently supports Windows. -
 **Custom Payloads**: Allows users to provide their own payloads for testing. -
 **Error Handling**: Handles stale element reference errors gracefully and
 retries automatically. - **Comprehensive Reports**: Provides detailed
-information about detected XSS vulnerabilities. ## Benefits - **Time-Saving**:
+information about detected XSS vulnerabilities. - **Payload List URL**:
+Displays a URL to a list of useful XSS payloads. ## Benefits - **Time-Saving**:
 Automates the tedious process of testing for XSS vulnerabilities, saving
 developers valuable time. - **Improved Security**: Helps in identifying and
 fixing XSS vulnerabilities, enhancing the overall security of web applications.
 - **Customizable**: Users can use their own payloads for testing, making it
 highly customizable for specific needs. Payload List : _C_l_i_c_k ## Installation
 Currently, xssbase is only compatible with Windows. To install, use the
 following command: ```sh pip install xssbase ``` ## Usage ### Basic Usage To
 test a URL for XSS vulnerabilities using the predefined payloads: ```sh xssbase
 --url ``` ### Using Custom Payloads To test a URL for XSS vulnerabilities using
 custom payloads from a file: ```sh xssbase --url --payload ``` ### Example To
 test http://example.com for XSS vulnerabilities using predefined payloads:
 ```sh xssbase --url http://example.com ``` To test http://example.com for XSS
 vulnerabilities using payloads from `custom-payloads.txt`: ```sh xssbase --url
-http://example.com --payload custom-payloads.txt ``` ### Arguments `--url`: The
-URL to test for XSS vulnerabilities (required). `--payload`: The file
-containing custom XSS payloads (optional). ### License This project is licensed
-under the MIT _L_i_c_e_n_s_e. See the LICENSE file for details. ### Disclaimer This
-tool is intended for educational purposes and for use by web developers to
-secure their own applications. Unauthorized or malicious use is strictly
-prohibited.
+http://example.com --payload custom-payloads.txt ``` ### Displaying Payload
+List URL To print the URL of a useful list of XSS payloads: ```sh xssbase --
+payload-list ``` ### Arguments `--url`: The URL to test for XSS vulnerabilities
+(required). `--payload`: The file containing custom XSS payloads (optional). `-
+-payload-list` : Displays a URL to a list of useful XSS payloads. ### License
+This project is licensed under the MIT _L_i_c_e_n_s_e. See the LICENSE file for
+details. ### Disclaimer This tool is intended for educational purposes and for
+use by web developers to secure their own applications. Unauthorized or
+malicious use is strictly prohibited.
```

