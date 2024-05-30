# Comparing `tmp/trsolucoes-8.0.1.tar.gz` & `tmp/trsolucoes-8.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trsolucoes-8.0.1.tar", last modified: Thu May 23 13:39:18 2024, max compression
+gzip compressed data, was "trsolucoes-8.0.2.tar", last modified: Thu May 30 18:46:44 2024, max compression
```

## Comparing `trsolucoes-8.0.1.tar` & `trsolucoes-8.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 13:39:18.002666 trsolucoes-8.0.1/
--rw-rw-rw-   0        0        0     1088 2024-05-19 21:10:17.000000 trsolucoes-8.0.1/LICENCE
--rw-rw-rw-   0        0        0     2508 2024-05-23 13:39:18.001667 trsolucoes-8.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2182 2024-05-19 21:25:05.000000 trsolucoes-8.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 13:39:17.996602 trsolucoes-8.0.1/selenium_helper/
--rw-rw-rw-   0        0        0       43 2024-05-23 13:08:07.000000 trsolucoes-8.0.1/selenium_helper/__init__.py
--rw-rw-rw-   0        0        0    13496 2024-05-23 13:38:35.000000 trsolucoes-8.0.1/selenium_helper/selenium_helper.py
--rw-rw-rw-   0        0        0       42 2024-05-23 13:39:18.002666 trsolucoes-8.0.1/setup.cfg
--rw-rw-rw-   0        0        0      543 2024-05-23 13:37:44.000000 trsolucoes-8.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 13:39:18.000470 trsolucoes-8.0.1/trsolucoes.egg-info/
--rw-rw-rw-   0        0        0     2508 2024-05-23 13:39:17.000000 trsolucoes-8.0.1/trsolucoes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-05-23 13:39:17.000000 trsolucoes-8.0.1/trsolucoes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 13:39:17.000000 trsolucoes-8.0.1/trsolucoes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-23 13:39:17.000000 trsolucoes-8.0.1/trsolucoes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 18:46:44.636723 trsolucoes-8.0.2/
+-rw-rw-rw-   0        0        0     1088 2024-05-19 21:10:17.000000 trsolucoes-8.0.2/LICENCE
+-rw-rw-rw-   0        0        0     2508 2024-05-30 18:46:44.636723 trsolucoes-8.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2182 2024-05-19 21:25:05.000000 trsolucoes-8.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 18:46:44.632573 trsolucoes-8.0.2/selenium_helper/
+-rw-rw-rw-   0        0        0       43 2024-05-23 13:08:07.000000 trsolucoes-8.0.2/selenium_helper/__init__.py
+-rw-rw-rw-   0        0        0    13471 2024-05-30 18:46:22.000000 trsolucoes-8.0.2/selenium_helper/selenium_helper.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 18:46:44.636723 trsolucoes-8.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      543 2024-05-30 18:46:27.000000 trsolucoes-8.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:46:44.635307 trsolucoes-8.0.2/trsolucoes.egg-info/
+-rw-rw-rw-   0        0        0     2508 2024-05-30 18:46:44.000000 trsolucoes-8.0.2/trsolucoes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-05-30 18:46:44.000000 trsolucoes-8.0.2/trsolucoes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 18:46:44.000000 trsolucoes-8.0.2/trsolucoes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-30 18:46:44.000000 trsolucoes-8.0.2/trsolucoes.egg-info/top_level.txt
```

### Comparing `trsolucoes-8.0.1/LICENCE` & `trsolucoes-8.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `trsolucoes-8.0.1/PKG-INFO` & `trsolucoes-8.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trsolucoes
-Version: 8.0.1
+Version: 8.0.2
 Summary: Um repositório não oficial de funções de auxilio para Selenium
 Author: Tainan Ramos
 Author-email: tainan@trsolucoes.com.br
 License: MIT License
 Keywords: trsolucoes
 Requires: selenium
 Description-Content-Type: text/markdown
```

### Comparing `trsolucoes-8.0.1/README.md` & `trsolucoes-8.0.2/README.md`

 * *Files identical despite different names*

### Comparing `trsolucoes-8.0.1/selenium_helper/selenium_helper.py` & `trsolucoes-8.0.2/selenium_helper/selenium_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             * click_before (bool, opcional): Se True, clica no elemento antes de enviar o texto. Default é False.
             * max_result (bool, opcional): Se True, aplica o filtro tag_filter ao resultado para retornar o elemento mais relevante. Default é False.
         """
         sleep(delay_before)
         element: WebElement
         element = _find_element(self.driver, locator, tag_filter, timeout, max_result)
         if(click_before):
-            self.wait_and_click(locator, tag_filter)
+            element.click()
         if(clear_form):
             element.clear()
         element.send_keys(text)
         sleep(delay_after)
 
     def wait_and_click(self, locator: tuple[By, str], tag_filter: list[tuple[str, str]] = None, timeout: int = 30, delay_before: float = 0.3, delay_after: float = 0.3, max_result: bool = False) -> None:
         """
```

### Comparing `trsolucoes-8.0.1/setup.py` & `trsolucoes-8.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="UTF-8") as arq:
     readme = arq.read()
 
 setup(name="trsolucoes",
-      version="8.0.1",
+      version="8.0.2",
       license="MIT License",
       author="Tainan Ramos",
       long_description=readme,
       long_description_content_type="text/markdown",
       author_email="tainan@trsolucoes.com.br",
       keywords="trsolucoes",
       description="Um repositório não oficial de funções de auxilio para Selenium",
```

### Comparing `trsolucoes-8.0.1/trsolucoes.egg-info/PKG-INFO` & `trsolucoes-8.0.2/trsolucoes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trsolucoes
-Version: 8.0.1
+Version: 8.0.2
 Summary: Um repositório não oficial de funções de auxilio para Selenium
 Author: Tainan Ramos
 Author-email: tainan@trsolucoes.com.br
 License: MIT License
 Keywords: trsolucoes
 Requires: selenium
 Description-Content-Type: text/markdown
```

