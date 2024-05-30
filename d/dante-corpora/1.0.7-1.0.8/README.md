# Comparing `tmp/dante_corpora-1.0.7.tar.gz` & `tmp/dante_corpora-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dante_corpora-1.0.7.tar", last modified: Thu May 30 17:38:59 2024, max compression
+gzip compressed data, was "dante_corpora-1.0.8.tar", last modified: Thu May 30 17:40:25 2024, max compression
```

## Comparing `dante_corpora-1.0.7.tar` & `dante_corpora-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 17:38:59.253511 dante_corpora-1.0.7/
--rw-rw-rw-   0        0        0     1091 2024-05-29 22:19:30.000000 dante_corpora-1.0.7/LICENSE
--rw-rw-rw-   0        0        0       20 2024-05-30 17:38:03.000000 dante_corpora-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     3053 2024-05-30 17:38:59.252503 dante_corpora-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2747 2024-05-30 16:49:59.000000 dante_corpora-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 17:38:59.243996 dante_corpora-1.0.7/dante/
--rw-rw-rw-   0        0        0       24 2024-05-30 17:37:44.000000 dante_corpora-1.0.7/dante/__init__.py
--rw-rw-rw-   0        0        0     2450 2024-05-30 17:35:37.000000 dante_corpora-1.0.7/dante/corpora.py
-drwxrwxrwx   0        0        0        0 2024-05-30 17:38:59.251969 dante_corpora-1.0.7/dante_corpora.egg-info/
--rw-rw-rw-   0        0        0     3053 2024-05-30 17:38:59.000000 dante_corpora-1.0.7/dante_corpora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-05-30 17:38:59.000000 dante_corpora-1.0.7/dante_corpora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 17:38:59.000000 dante_corpora-1.0.7/dante_corpora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-30 17:38:59.000000 dante_corpora-1.0.7/dante_corpora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-30 17:38:59.000000 dante_corpora-1.0.7/dante_corpora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 17:38:59.253511 dante_corpora-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      622 2024-05-30 17:38:49.000000 dante_corpora-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:40:25.110735 dante_corpora-1.0.8/
+-rw-rw-rw-   0        0        0     1091 2024-05-29 22:19:30.000000 dante_corpora-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0       20 2024-05-30 17:38:03.000000 dante_corpora-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     3045 2024-05-30 17:40:25.110735 dante_corpora-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2747 2024-05-30 17:40:13.000000 dante_corpora-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 17:40:25.105980 dante_corpora-1.0.8/dante/
+-rw-rw-rw-   0        0        0       24 2024-05-30 17:37:44.000000 dante_corpora-1.0.8/dante/__init__.py
+-rw-rw-rw-   0        0        0     2450 2024-05-30 17:35:37.000000 dante_corpora-1.0.8/dante/corpora.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:40:25.110033 dante_corpora-1.0.8/dante_corpora.egg-info/
+-rw-rw-rw-   0        0        0     3045 2024-05-30 17:40:25.000000 dante_corpora-1.0.8/dante_corpora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2024-05-30 17:40:25.000000 dante_corpora-1.0.8/dante_corpora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 17:40:25.000000 dante_corpora-1.0.8/dante_corpora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-30 17:40:25.000000 dante_corpora-1.0.8/dante_corpora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-30 17:40:25.000000 dante_corpora-1.0.8/dante_corpora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 17:40:25.112335 dante_corpora-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      622 2024-05-30 17:40:22.000000 dante_corpora-1.0.8/setup.py
```

### Comparing `dante_corpora-1.0.7/LICENSE` & `dante_corpora-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dante_corpora-1.0.7/PKG-INFO` & `dante_corpora-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: dante-corpora
-Version: 1.0.7
+Version: 1.0.8
 Summary: Pacote Python contendo os corpora do projeto DANTE do POeTiSA
 Author: felmateos
 Author-email: felmateos@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas==2.2.2
 
 <a name="readme-top"></a>
 
 <div align="center">
+
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
+
 </div>
 
 <br />
 <div align="center">
   <a href="https://github.com/DANTE-POeTiSA/dante-corpora">
     <img src="https://github.com/DANTE-POeTiSA/dante-corpora/blob/main/images/dante.png?raw=true" alt="Logo"  height="100" style="border-radius:50%">
   </a>
@@ -74,23 +76,23 @@
 
 ## Documentos importantes
 
 ...
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-## ContribuiÃ§Ã£o
+## Contribuicao
 
 Contribuicoes sao bem-vindas! Sinta-se a vontade para propor melhorias, relatar problemas ou abrir pull requests.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-## LicenÃ§a
+## Licenca
 
-Este projeto e licenciado sob a [LicenÃ§a MIT](LICENSE).
+Este projeto e licenciado sob a [Licenca MIT](LICENSE).
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 [contributors-shield]: https://img.shields.io/github/contributors/DANTE-POeTiSA/dante-corpora.svg?style=for-the-badge
 [contributors-url]: https://github.com/DANTE-POeTiSA/dante-corpora/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/DANTE-POeTiSA/dante-corpora.svg?style=for-the-badge
 [forks-url]: https://github.com/DANTE-POeTiSA/dante-corpora/network/members
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dante-corpora Version: 1.0.7 Summary: Pacote Python
+Metadata-Version: 2.1 Name: dante-corpora Version: 1.0.8 Summary: Pacote Python
 contendo os corpora do projeto DANTE do POeTiSA Author: felmateos Author-email:
 felmateos@gmail.com License: MIT Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: pandas==2.2.2
    [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
       shield]][issues-url] [![MIT License][license-shield]][license-url]
 
@@ -18,18 +18,18 @@
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Instalacao ``` pip install dante-corpora ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Conjunto de Dados ...
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Documentos importantes ...
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## ContribuiÃÂ§ÃÂ£o Contribuicoes sao bem-vindas! Sinta-se a vontade para
-propor melhorias, relatar problemas ou abrir pull requests.
+## Contribuicao Contribuicoes sao bem-vindas! Sinta-se a vontade para propor
+melhorias, relatar problemas ou abrir pull requests.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## LicenÃÂ§a Este projeto e licenciado sob a [LicenÃÂ§a MIT](LICENSE).
+## Licenca Este projeto e licenciado sob a [Licenca MIT](LICENSE).
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/DANTE-
 POeTiSA/dante-corpora.svg?style=for-the-badge [contributors-url]: https://
 github.com/DANTE-POeTiSA/dante-corpora/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/DANTE-POeTiSA/dante-corpora.svg?style=for-
 the-badge [forks-url]: https://github.com/DANTE-POeTiSA/dante-corpora/network/
 members [stars-shield]: https://img.shields.io/github/stars/DANTE-POeTiSA/
```

### Comparing `dante_corpora-1.0.7/README.md` & `dante_corpora-1.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 <a name="readme-top"></a>
 
 <div align="center">
+
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
+
 </div>
 
 <br />
 <div align="center">
   <a href="https://github.com/DANTE-POeTiSA/dante-corpora">
     <img src="https://github.com/DANTE-POeTiSA/dante-corpora/blob/main/images/dante.png?raw=true" alt="Logo"  height="100" style="border-radius:50%">
   </a>
@@ -63,23 +65,23 @@
 
 ## Documentos importantes
 
 ...
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-## Contribuição
+## Contribuicao
 
 Contribuicoes sao bem-vindas! Sinta-se a vontade para propor melhorias, relatar problemas ou abrir pull requests.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-## Licença
+## Licenca
 
-Este projeto e licenciado sob a [Licença MIT](LICENSE).
+Este projeto e licenciado sob a [Licenca MIT](LICENSE).
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 [contributors-shield]: https://img.shields.io/github/contributors/DANTE-POeTiSA/dante-corpora.svg?style=for-the-badge
 [contributors-url]: https://github.com/DANTE-POeTiSA/dante-corpora/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/DANTE-POeTiSA/dante-corpora.svg?style=for-the-badge
 [forks-url]: https://github.com/DANTE-POeTiSA/dante-corpora/network/members
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -14,18 +14,18 @@
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Instalacao ``` pip install dante-corpora ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Conjunto de Dados ...
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Documentos importantes ...
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## ContribuiÃ§Ã£o Contribuicoes sao bem-vindas! Sinta-se a vontade para propor
+## Contribuicao Contribuicoes sao bem-vindas! Sinta-se a vontade para propor
 melhorias, relatar problemas ou abrir pull requests.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## LicenÃ§a Este projeto e licenciado sob a [LicenÃ§a MIT](LICENSE).
+## Licenca Este projeto e licenciado sob a [Licenca MIT](LICENSE).
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/DANTE-
 POeTiSA/dante-corpora.svg?style=for-the-badge [contributors-url]: https://
 github.com/DANTE-POeTiSA/dante-corpora/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/DANTE-POeTiSA/dante-corpora.svg?style=for-
 the-badge [forks-url]: https://github.com/DANTE-POeTiSA/dante-corpora/network/
 members [stars-shield]: https://img.shields.io/github/stars/DANTE-POeTiSA/
```

### Comparing `dante_corpora-1.0.7/dante/corpora.py` & `dante_corpora-1.0.8/dante/corpora.py`

 * *Files identical despite different names*

### Comparing `dante_corpora-1.0.7/dante_corpora.egg-info/PKG-INFO` & `dante_corpora-1.0.8/dante_corpora.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: dante-corpora
-Version: 1.0.7
+Version: 1.0.8
 Summary: Pacote Python contendo os corpora do projeto DANTE do POeTiSA
 Author: felmateos
 Author-email: felmateos@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas==2.2.2
 
 <a name="readme-top"></a>
 
 <div align="center">
+
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
+
 </div>
 
 <br />
 <div align="center">
   <a href="https://github.com/DANTE-POeTiSA/dante-corpora">
     <img src="https://github.com/DANTE-POeTiSA/dante-corpora/blob/main/images/dante.png?raw=true" alt="Logo"  height="100" style="border-radius:50%">
   </a>
@@ -74,23 +76,23 @@
 
 ## Documentos importantes
 
 ...
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-## ContribuiÃ§Ã£o
+## Contribuicao
 
 Contribuicoes sao bem-vindas! Sinta-se a vontade para propor melhorias, relatar problemas ou abrir pull requests.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-## LicenÃ§a
+## Licenca
 
-Este projeto e licenciado sob a [LicenÃ§a MIT](LICENSE).
+Este projeto e licenciado sob a [Licenca MIT](LICENSE).
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 [contributors-shield]: https://img.shields.io/github/contributors/DANTE-POeTiSA/dante-corpora.svg?style=for-the-badge
 [contributors-url]: https://github.com/DANTE-POeTiSA/dante-corpora/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/DANTE-POeTiSA/dante-corpora.svg?style=for-the-badge
 [forks-url]: https://github.com/DANTE-POeTiSA/dante-corpora/network/members
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dante-corpora Version: 1.0.7 Summary: Pacote Python
+Metadata-Version: 2.1 Name: dante-corpora Version: 1.0.8 Summary: Pacote Python
 contendo os corpora do projeto DANTE do POeTiSA Author: felmateos Author-email:
 felmateos@gmail.com License: MIT Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: pandas==2.2.2
    [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
       shield]][issues-url] [![MIT License][license-shield]][license-url]
 
@@ -18,18 +18,18 @@
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Instalacao ``` pip install dante-corpora ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Conjunto de Dados ...
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Documentos importantes ...
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## ContribuiÃÂ§ÃÂ£o Contribuicoes sao bem-vindas! Sinta-se a vontade para
-propor melhorias, relatar problemas ou abrir pull requests.
+## Contribuicao Contribuicoes sao bem-vindas! Sinta-se a vontade para propor
+melhorias, relatar problemas ou abrir pull requests.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## LicenÃÂ§a Este projeto e licenciado sob a [LicenÃÂ§a MIT](LICENSE).
+## Licenca Este projeto e licenciado sob a [Licenca MIT](LICENSE).
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/DANTE-
 POeTiSA/dante-corpora.svg?style=for-the-badge [contributors-url]: https://
 github.com/DANTE-POeTiSA/dante-corpora/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/DANTE-POeTiSA/dante-corpora.svg?style=for-
 the-badge [forks-url]: https://github.com/DANTE-POeTiSA/dante-corpora/network/
 members [stars-shield]: https://img.shields.io/github/stars/DANTE-POeTiSA/
```

### Comparing `dante_corpora-1.0.7/setup.py` & `dante_corpora-1.0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='dante-corpora',
-    version='1.0.7',
+    version='1.0.8',
     description='Pacote Python contendo os corpora do projeto DANTE do POeTiSA',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='felmateos',
     author_email='felmateos@gmail.com',
     packages=find_packages(),
     package_data={
```

