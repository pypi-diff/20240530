# Comparing `tmp/ussl-1.2.0.tar.gz` & `tmp/ussl-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ussl-1.2.0.tar", last modified: Wed May 29 09:22:05 2024, max compression
+gzip compressed data, was "dist\ussl-1.2.1.tar", last modified: Thu May 30 08:35:04 2024, max compression
```

## Comparing `ussl-1.2.0.tar` & `ussl-1.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 09:22:05.033945 ussl-1.2.0/
--rw-rw-rw-   0        0        0    12117 2024-05-29 09:22:05.031946 ussl-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    11465 2024-05-29 09:21:19.000000 ussl-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-29 09:22:05.034014 ussl-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2233 2024-05-29 09:22:00.000000 ussl-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:22:04.994514 ussl-1.2.0/ussl/
--rw-rw-rw-   0        0        0       49 2024-03-01 08:27:08.000000 ussl-1.2.0/ussl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:22:05.011009 ussl-1.2.0/ussl/exceptions/
--rw-rw-rw-   0        0        0      305 2024-05-29 08:59:11.000000 ussl-1.2.0/ussl/exceptions/__init__.py
--rw-rw-rw-   0        0        0     1369 2024-05-22 08:57:11.000000 ussl-1.2.0/ussl/exceptions/main.py
--rw-rw-rw-   0        0        0     1126 2024-05-29 09:16:44.000000 ussl-1.2.0/ussl/exceptions/protocol_exc.py
--rw-rw-rw-   0        0        0     1084 2024-03-01 08:27:08.000000 ussl-1.2.0/ussl/exceptions/validation_exc.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:22:05.013136 ussl-1.2.0/ussl/model/
--rw-rw-rw-   0        0        0     4405 2024-05-29 08:27:14.000000 ussl-1.2.0/ussl/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:22:05.016173 ussl-1.2.0/ussl/postprocessing/
--rw-rw-rw-   0        0        0        0 2024-03-01 08:27:08.000000 ussl-1.2.0/ussl/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     7341 2024-05-29 09:16:47.000000 ussl-1.2.0/ussl/postprocessing/base.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:22:05.027946 ussl-1.2.0/ussl/protocol/
--rw-rw-rw-   0        0        0      798 2024-05-29 08:13:26.000000 ussl-1.2.0/ussl/protocol/__init__.py
--rw-rw-rw-   0        0        0      711 2024-05-29 08:13:26.000000 ussl-1.2.0/ussl/protocol/base.py
--rw-rw-rw-   0        0        0     1534 2024-05-29 08:13:26.000000 ussl-1.2.0/ussl/protocol/ldap.py
--rw-rw-rw-   0        0        0     4610 2024-05-29 08:13:26.000000 ussl-1.2.0/ussl/protocol/ssh.py
--rw-rw-rw-   0        0        0        0 2024-01-24 09:57:50.000000 ussl-1.2.0/ussl/protocol/winexe.py
--rw-rw-rw-   0        0        0     8202 2024-05-29 08:13:26.000000 ussl-1.2.0/ussl/protocol/winrm.py
--rw-rw-rw-   0        0        0      303 2024-05-29 08:13:26.000000 ussl-1.2.0/ussl/protocol/wmi.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:22:05.028944 ussl-1.2.0/ussl/transport/
--rw-rw-rw-   0        0        0     1508 2024-05-29 08:27:14.000000 ussl-1.2.0/ussl/transport/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:22:05.030948 ussl-1.2.0/ussl/utils/
--rw-rw-rw-   0        0        0     6424 2024-03-01 08:27:08.000000 ussl-1.2.0/ussl/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:22:05.005339 ussl-1.2.0/ussl.egg-info/
--rw-rw-rw-   0        0        0    12117 2024-05-29 09:22:04.000000 ussl-1.2.0/ussl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2024-05-29 09:22:04.000000 ussl-1.2.0/ussl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 09:22:04.000000 ussl-1.2.0/ussl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-05-29 09:22:04.000000 ussl-1.2.0/ussl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-29 09:22:04.000000 ussl-1.2.0/ussl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 08:35:04.934725 ussl-1.2.1/
+-rw-rw-rw-   0        0        0    12117 2024-05-30 08:35:04.930725 ussl-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11465 2024-05-30 08:20:33.000000 ussl-1.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-30 08:35:04.934725 ussl-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2233 2024-05-30 08:31:46.000000 ussl-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:35:04.885216 ussl-1.2.1/ussl/
+-rw-rw-rw-   0        0        0      133 2024-05-30 08:35:02.000000 ussl-1.2.1/ussl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:35:04.903570 ussl-1.2.1/ussl/exceptions/
+-rw-rw-rw-   0        0        0      305 2024-05-29 08:59:11.000000 ussl-1.2.1/ussl/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     1369 2024-05-22 08:57:11.000000 ussl-1.2.1/ussl/exceptions/main.py
+-rw-rw-rw-   0        0        0     1126 2024-05-29 09:16:44.000000 ussl-1.2.1/ussl/exceptions/protocol_exc.py
+-rw-rw-rw-   0        0        0     1084 2024-03-01 08:27:08.000000 ussl-1.2.1/ussl/exceptions/validation_exc.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:35:04.905596 ussl-1.2.1/ussl/model/
+-rw-rw-rw-   0        0        0     4405 2024-05-30 08:20:33.000000 ussl-1.2.1/ussl/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:35:04.909564 ussl-1.2.1/ussl/postprocessing/
+-rw-rw-rw-   0        0        0        0 2024-03-01 08:27:08.000000 ussl-1.2.1/ussl/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     7341 2024-05-30 08:20:33.000000 ussl-1.2.1/ussl/postprocessing/base.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:35:04.923563 ussl-1.2.1/ussl/protocol/
+-rw-rw-rw-   0        0        0      798 2024-05-30 08:20:33.000000 ussl-1.2.1/ussl/protocol/__init__.py
+-rw-rw-rw-   0        0        0      711 2024-05-30 08:20:33.000000 ussl-1.2.1/ussl/protocol/base.py
+-rw-rw-rw-   0        0        0     1534 2024-05-30 08:20:33.000000 ussl-1.2.1/ussl/protocol/ldap.py
+-rw-rw-rw-   0        0        0     4610 2024-05-30 08:20:33.000000 ussl-1.2.1/ussl/protocol/ssh.py
+-rw-rw-rw-   0        0        0        0 2024-01-24 09:57:50.000000 ussl-1.2.1/ussl/protocol/winexe.py
+-rw-rw-rw-   0        0        0     8202 2024-05-30 08:20:33.000000 ussl-1.2.1/ussl/protocol/winrm.py
+-rw-rw-rw-   0        0        0      303 2024-05-30 08:20:33.000000 ussl-1.2.1/ussl/protocol/wmi.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:35:04.925566 ussl-1.2.1/ussl/transport/
+-rw-rw-rw-   0        0        0     1508 2024-05-30 08:20:33.000000 ussl-1.2.1/ussl/transport/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:35:04.927564 ussl-1.2.1/ussl/utils/
+-rw-rw-rw-   0        0        0     6424 2024-03-01 08:27:08.000000 ussl-1.2.1/ussl/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:35:04.894926 ussl-1.2.1/ussl.egg-info/
+-rw-rw-rw-   0        0        0    12117 2024-05-30 08:35:04.000000 ussl-1.2.1/ussl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2024-05-30 08:35:04.000000 ussl-1.2.1/ussl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 08:35:04.000000 ussl-1.2.1/ussl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2024-05-30 08:35:04.000000 ussl-1.2.1/ussl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-30 08:35:04.000000 ussl-1.2.1/ussl.egg-info/top_level.txt
```

### Comparing `ussl-1.2.0/PKG-INFO` & `ussl-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ussl
-Version: 1.2.0
+Version: 1.2.1
 Summary: Пакет разработчиков USSC-SOC для упрощения взаимодействия с АРМ, серверами и сетевыми устройствами
 Author: ussc soc dev team
 Author-email: iushangaraev@ussc.ru, pbikkuzhina@ussc.ru
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-Requires-Dist: pywinrm==0.4.1
-Requires-Dist: paramiko==2.7.2
+Requires-Dist: pywinrm==0.4.3
+Requires-Dist: paramiko==3.3.1
 Requires-Dist: marshmallow==3.20.2
 Requires-Dist: python-ldap==3.4.4; platform_system != "Windows"
 
 # USSL - USSC SOAR SCRIPT LIB
 
 <!-- Оглавление -->
 ## Оглавление
```

### Comparing `ussl-1.2.0/README.md` & `ussl-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ussl-1.2.0/setup.py` & `ussl-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,28 +25,28 @@
 setup(
     name='ussl',
     author='ussc soc dev team',
     author_email='iushangaraev@ussc.ru, pbikkuzhina@ussc.ru',
     description='Пакет разработчиков USSC-SOC для упрощения взаимодействия с АРМ, серверами и сетевыми устройствами',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.0',
+    version='1.2.1',
     python_requires='>=3.8.0',
     packages=[
         'ussl',
         'ussl.model',
         'ussl.postprocessing',
         'ussl.protocol',
         'ussl.transport',
         'ussl.exceptions',
         'ussl.utils',
     ],
     install_requires=[
-        'pywinrm==0.4.1',
-        'paramiko==2.7.2',
+        'pywinrm==0.4.3',
+        'paramiko==3.3.1',
         'marshmallow==3.20.2',
         'python-ldap==3.4.4; platform_system != "Windows"',
         # 'python-ldap-build @ https://github.com/cgohlke/python-ldap-build/releases/download/v3.4.4/python_ldap-3.4
         # .4-cp38-cp38-win_amd64.whl', # for Windows only
     ],
     classifiers=[
         'Programming Language :: Python',
```

### Comparing `ussl-1.2.0/ussl/exceptions/main.py` & `ussl-1.2.1/ussl/exceptions/main.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.0/ussl/exceptions/protocol_exc.py` & `ussl-1.2.1/ussl/exceptions/protocol_exc.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.0/ussl/exceptions/validation_exc.py` & `ussl-1.2.1/ussl/exceptions/validation_exc.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.0/ussl/model/__init__.py` & `ussl-1.2.1/ussl/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.0/ussl/postprocessing/base.py` & `ussl-1.2.1/ussl/postprocessing/base.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.0/ussl/protocol/__init__.py` & `ussl-1.2.1/ussl/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.0/ussl/protocol/base.py` & `ussl-1.2.1/ussl/protocol/base.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.0/ussl/protocol/ldap.py` & `ussl-1.2.1/ussl/protocol/ldap.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.0/ussl/protocol/ssh.py` & `ussl-1.2.1/ussl/protocol/ssh.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.0/ussl/protocol/winrm.py` & `ussl-1.2.1/ussl/protocol/winrm.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.0/ussl/transport/__init__.py` & `ussl-1.2.1/ussl/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.0/ussl/utils/__init__.py` & `ussl-1.2.1/ussl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.0/ussl.egg-info/PKG-INFO` & `ussl-1.2.1/ussl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ussl
-Version: 1.2.0
+Version: 1.2.1
 Summary: Пакет разработчиков USSC-SOC для упрощения взаимодействия с АРМ, серверами и сетевыми устройствами
 Author: ussc soc dev team
 Author-email: iushangaraev@ussc.ru, pbikkuzhina@ussc.ru
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-Requires-Dist: pywinrm==0.4.1
-Requires-Dist: paramiko==2.7.2
+Requires-Dist: pywinrm==0.4.3
+Requires-Dist: paramiko==3.3.1
 Requires-Dist: marshmallow==3.20.2
 Requires-Dist: python-ldap==3.4.4; platform_system != "Windows"
 
 # USSL - USSC SOAR SCRIPT LIB
 
 <!-- Оглавление -->
 ## Оглавление
```

### Comparing `ussl-1.2.0/ussl.egg-info/SOURCES.txt` & `ussl-1.2.1/ussl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

