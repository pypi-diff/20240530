# Comparing `tmp/dante_corpora-1.0.6.tar.gz` & `tmp/dante_corpora-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dante_corpora-1.0.6.tar", last modified: Thu May 30 00:03:12 2024, max compression
+gzip compressed data, was "dante_corpora-1.0.7.tar", last modified: Thu May 30 17:38:59 2024, max compression
```

## Comparing `dante_corpora-1.0.6.tar` & `dante_corpora-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 00:03:12.470911 dante_corpora-1.0.6/
--rw-rw-rw-   0        0        0     1091 2024-05-29 22:19:30.000000 dante_corpora-1.0.6/LICENSE
--rw-rw-rw-   0        0        0       69 2024-05-29 23:13:34.000000 dante_corpora-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     3044 2024-05-30 00:03:12.470911 dante_corpora-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2718 2024-05-29 22:29:52.000000 dante_corpora-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 00:03:12.458698 dante_corpora-1.0.6/dante/
--rw-rw-rw-   0        0        0       75 2024-05-29 23:01:49.000000 dante_corpora-1.0.6/dante/__init__.py
--rw-rw-rw-   0        0        0      219 2024-05-30 00:02:46.000000 dante_corpora-1.0.6/dante/danteshots.py
--rw-rw-rw-   0        0        0      220 2024-05-30 00:02:49.000000 dante_corpora-1.0.6/dante/dantestocks.py
-drwxrwxrwx   0        0        0        0 2024-05-30 00:03:12.461219 dante_corpora-1.0.6/dante/data/
--rw-rw-rw-   0        0        0  1836029 2024-04-08 13:13:38.000000 dante_corpora-1.0.6/dante/data/danteshots.csv
--rw-rw-rw-   0        0        0   770632 2024-03-11 13:06:38.000000 dante_corpora-1.0.6/dante/data/dantestocks.csv
-drwxrwxrwx   0        0        0        0 2024-05-30 00:03:12.470911 dante_corpora-1.0.6/dante_corpora.egg-info/
--rw-rw-rw-   0        0        0     3044 2024-05-30 00:03:12.000000 dante_corpora-1.0.6/dante_corpora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2024-05-30 00:03:12.000000 dante_corpora-1.0.6/dante_corpora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 00:03:12.000000 dante_corpora-1.0.6/dante_corpora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-30 00:03:12.000000 dante_corpora-1.0.6/dante_corpora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-30 00:03:12.000000 dante_corpora-1.0.6/dante_corpora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 00:03:12.470911 dante_corpora-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      620 2024-05-30 00:02:54.000000 dante_corpora-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:38:59.253511 dante_corpora-1.0.7/
+-rw-rw-rw-   0        0        0     1091 2024-05-29 22:19:30.000000 dante_corpora-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0       20 2024-05-30 17:38:03.000000 dante_corpora-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     3053 2024-05-30 17:38:59.252503 dante_corpora-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2747 2024-05-30 16:49:59.000000 dante_corpora-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 17:38:59.243996 dante_corpora-1.0.7/dante/
+-rw-rw-rw-   0        0        0       24 2024-05-30 17:37:44.000000 dante_corpora-1.0.7/dante/__init__.py
+-rw-rw-rw-   0        0        0     2450 2024-05-30 17:35:37.000000 dante_corpora-1.0.7/dante/corpora.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:38:59.251969 dante_corpora-1.0.7/dante_corpora.egg-info/
+-rw-rw-rw-   0        0        0     3053 2024-05-30 17:38:59.000000 dante_corpora-1.0.7/dante_corpora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2024-05-30 17:38:59.000000 dante_corpora-1.0.7/dante_corpora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 17:38:59.000000 dante_corpora-1.0.7/dante_corpora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-30 17:38:59.000000 dante_corpora-1.0.7/dante_corpora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-30 17:38:59.000000 dante_corpora-1.0.7/dante_corpora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 17:38:59.253511 dante_corpora-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      622 2024-05-30 17:38:49.000000 dante_corpora-1.0.7/setup.py
```

### Comparing `dante_corpora-1.0.6/LICENSE` & `dante_corpora-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dante_corpora-1.0.6/PKG-INFO` & `dante_corpora-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,66 +1,63 @@
 Metadata-Version: 2.1
 Name: dante-corpora
-Version: 1.0.6
+Version: 1.0.7
 Summary: Pacote Python contendo os corpora do projeto DANTE do POeTiSA
 Author: felmateos
 Author-email: felmateos@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas==2.2.2
 
 <a name="readme-top"></a>
 
 <div align="center">
-
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
-
 </div>
 
-<!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/DANTE-POeTiSA/dante-corpora">
-    <img src="images\dante.png" alt="Logo"  height="100" style="border-radius:50%">
+    <img src="https://github.com/DANTE-POeTiSA/dante-corpora/blob/main/images/dante.png?raw=true" alt="Logo"  height="100" style="border-radius:50%">
   </a>
 
 <h3 align="center">DANTE Corpora</h3>
 
   <p align="center">
     Pacote Python contendo os corpora do projeto DANTE do POeTiSA
     <br />
     <br />
     <a href="https://github.com/DANTE-POeTiSA/dante-corpora/issues">Report Bug</a>
-    Â·
+    -
     <a href="https://github.com/DANTE-POeTiSA/dante-corpora/issues">Request Feature</a>
   </p>
 </div>
 
 <br />
 
 ---
 
 ...
 
 ## Git Clone
 
-Para obter uma cÃ³pia local deste repositÃ³rio, utilize o seguinte comando:
+Para obter uma copia local deste repositorio, utilize o seguinte comando:
 
 ```
 git clone https://github.com/DANTE-POeTiSA/dante-corpora.git
 ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-## InstalaÃ§Ã£o
+## Instalacao
 
 
 
 ```
 pip install dante-corpora
 ```
 
@@ -79,21 +76,21 @@
 
 ...
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## ContribuiÃ§Ã£o
 
-ContribuiÃ§Ãµes sÃ£o bem-vindas! Sinta-se Ã  vontade para propor melhorias, relatar problemas ou abrir pull requests.
+Contribuicoes sao bem-vindas! Sinta-se a vontade para propor melhorias, relatar problemas ou abrir pull requests.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## LicenÃ§a
 
-Este projeto Ã© licenciado sob a [LicenÃ§a MIT](LICENSE).
+Este projeto e licenciado sob a [LicenÃ§a MIT](LICENSE).
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 [contributors-shield]: https://img.shields.io/github/contributors/DANTE-POeTiSA/dante-corpora.svg?style=for-the-badge
 [contributors-url]: https://github.com/DANTE-POeTiSA/dante-corpora/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/DANTE-POeTiSA/dante-corpora.svg?style=for-the-badge
 [forks-url]: https://github.com/DANTE-POeTiSA/dante-corpora/network/members
```

#### html2text {}

```diff
@@ -1,35 +1,35 @@
-Metadata-Version: 2.1 Name: dante-corpora Version: 1.0.6 Summary: Pacote Python
+Metadata-Version: 2.1 Name: dante-corpora Version: 1.0.7 Summary: Pacote Python
 contendo os corpora do projeto DANTE do POeTiSA Author: felmateos Author-email:
 felmateos@gmail.com License: MIT Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: pandas==2.2.2
    [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
       shield]][issues-url] [![MIT License][license-shield]][license-url]
 
                                     _[_L_o_g_o_]
                             ******** DDAANNTTEE CCoorrppoorraa ********
         Pacote Python contendo os corpora do projeto DANTE do POeTiSA
 
-                        _R_e_p_o_r_t_ _B_u_g ÃÂ· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
+                         _R_e_p_o_r_t_ _B_u_g - _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 
---- ... ## Git Clone Para obter uma cÃÂ³pia local deste repositÃÂ³rio,
-utilize o seguinte comando: ``` git clone https://github.com/DANTE-POeTiSA/
-dante-corpora.git ```
+--- ... ## Git Clone Para obter uma copia local deste repositorio, utilize o
+seguinte comando: ``` git clone https://github.com/DANTE-POeTiSA/dante-
+corpora.git ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## InstalaÃÂ§ÃÂ£o ``` pip install dante-corpora ```
+## Instalacao ``` pip install dante-corpora ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Conjunto de Dados ...
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Documentos importantes ...
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## ContribuiÃÂ§ÃÂ£o ContribuiÃÂ§ÃÂµes sÃÂ£o bem-vindas! Sinta-se ÃÂ 
-vontade para propor melhorias, relatar problemas ou abrir pull requests.
+## ContribuiÃÂ§ÃÂ£o Contribuicoes sao bem-vindas! Sinta-se a vontade para
+propor melhorias, relatar problemas ou abrir pull requests.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## LicenÃÂ§a Este projeto ÃÂ© licenciado sob a [LicenÃÂ§a MIT](LICENSE).
+## LicenÃÂ§a Este projeto e licenciado sob a [LicenÃÂ§a MIT](LICENSE).
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/DANTE-
 POeTiSA/dante-corpora.svg?style=for-the-badge [contributors-url]: https://
 github.com/DANTE-POeTiSA/dante-corpora/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/DANTE-POeTiSA/dante-corpora.svg?style=for-
 the-badge [forks-url]: https://github.com/DANTE-POeTiSA/dante-corpora/network/
 members [stars-shield]: https://img.shields.io/github/stars/DANTE-POeTiSA/
```

### Comparing `dante_corpora-1.0.6/README.md` & `dante_corpora-1.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 <a name="readme-top"></a>
 
 <div align="center">
-
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
-
 </div>
 
-<!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/DANTE-POeTiSA/dante-corpora">
-    <img src="images\dante.png" alt="Logo"  height="100" style="border-radius:50%">
+    <img src="https://github.com/DANTE-POeTiSA/dante-corpora/blob/main/images/dante.png?raw=true" alt="Logo"  height="100" style="border-radius:50%">
   </a>
 
 <h3 align="center">DANTE Corpora</h3>
 
   <p align="center">
     Pacote Python contendo os corpora do projeto DANTE do POeTiSA
     <br />
     <br />
     <a href="https://github.com/DANTE-POeTiSA/dante-corpora/issues">Report Bug</a>
-    ·
+    -
     <a href="https://github.com/DANTE-POeTiSA/dante-corpora/issues">Request Feature</a>
   </p>
 </div>
 
 <br />
 
 ---
 
 ...
 
 ## Git Clone
 
-Para obter uma cópia local deste repositório, utilize o seguinte comando:
+Para obter uma copia local deste repositorio, utilize o seguinte comando:
 
 ```
 git clone https://github.com/DANTE-POeTiSA/dante-corpora.git
 ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-## Instalação
+## Instalacao
 
 
 
 ```
 pip install dante-corpora
 ```
 
@@ -68,21 +65,21 @@
 
 ...
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## Contribuição
 
-Contribuições são bem-vindas! Sinta-se à vontade para propor melhorias, relatar problemas ou abrir pull requests.
+Contribuicoes sao bem-vindas! Sinta-se a vontade para propor melhorias, relatar problemas ou abrir pull requests.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## Licença
 
-Este projeto é licenciado sob a [Licença MIT](LICENSE).
+Este projeto e licenciado sob a [Licença MIT](LICENSE).
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 [contributors-shield]: https://img.shields.io/github/contributors/DANTE-POeTiSA/dante-corpora.svg?style=for-the-badge
 [contributors-url]: https://github.com/DANTE-POeTiSA/dante-corpora/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/DANTE-POeTiSA/dante-corpora.svg?style=for-the-badge
 [forks-url]: https://github.com/DANTE-POeTiSA/dante-corpora/network/members
```

#### html2text {}

```diff
@@ -2,30 +2,30 @@
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
       shield]][issues-url] [![MIT License][license-shield]][license-url]
 
                                     _[_L_o_g_o_]
                             ******** DDAANNTTEE CCoorrppoorraa ********
         Pacote Python contendo os corpora do projeto DANTE do POeTiSA
 
-                         _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
+                         _R_e_p_o_r_t_ _B_u_g - _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 
---- ... ## Git Clone Para obter uma cÃ³pia local deste repositÃ³rio, utilize o
+--- ... ## Git Clone Para obter uma copia local deste repositorio, utilize o
 seguinte comando: ``` git clone https://github.com/DANTE-POeTiSA/dante-
 corpora.git ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## InstalaÃ§Ã£o ``` pip install dante-corpora ```
+## Instalacao ``` pip install dante-corpora ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Conjunto de Dados ...
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Documentos importantes ...
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## ContribuiÃ§Ã£o ContribuiÃ§Ãµes sÃ£o bem-vindas! Sinta-se Ã  vontade para
-propor melhorias, relatar problemas ou abrir pull requests.
+## ContribuiÃ§Ã£o Contribuicoes sao bem-vindas! Sinta-se a vontade para propor
+melhorias, relatar problemas ou abrir pull requests.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## LicenÃ§a Este projeto Ã© licenciado sob a [LicenÃ§a MIT](LICENSE).
+## LicenÃ§a Este projeto e licenciado sob a [LicenÃ§a MIT](LICENSE).
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/DANTE-
 POeTiSA/dante-corpora.svg?style=for-the-badge [contributors-url]: https://
 github.com/DANTE-POeTiSA/dante-corpora/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/DANTE-POeTiSA/dante-corpora.svg?style=for-
 the-badge [forks-url]: https://github.com/DANTE-POeTiSA/dante-corpora/network/
 members [stars-shield]: https://img.shields.io/github/stars/DANTE-POeTiSA/
```

### Comparing `dante_corpora-1.0.6/dante_corpora.egg-info/PKG-INFO` & `dante_corpora-1.0.7/dante_corpora.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,66 +1,63 @@
 Metadata-Version: 2.1
 Name: dante-corpora
-Version: 1.0.6
+Version: 1.0.7
 Summary: Pacote Python contendo os corpora do projeto DANTE do POeTiSA
 Author: felmateos
 Author-email: felmateos@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas==2.2.2
 
 <a name="readme-top"></a>
 
 <div align="center">
-
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
-
 </div>
 
-<!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/DANTE-POeTiSA/dante-corpora">
-    <img src="images\dante.png" alt="Logo"  height="100" style="border-radius:50%">
+    <img src="https://github.com/DANTE-POeTiSA/dante-corpora/blob/main/images/dante.png?raw=true" alt="Logo"  height="100" style="border-radius:50%">
   </a>
 
 <h3 align="center">DANTE Corpora</h3>
 
   <p align="center">
     Pacote Python contendo os corpora do projeto DANTE do POeTiSA
     <br />
     <br />
     <a href="https://github.com/DANTE-POeTiSA/dante-corpora/issues">Report Bug</a>
-    Â·
+    -
     <a href="https://github.com/DANTE-POeTiSA/dante-corpora/issues">Request Feature</a>
   </p>
 </div>
 
 <br />
 
 ---
 
 ...
 
 ## Git Clone
 
-Para obter uma cÃ³pia local deste repositÃ³rio, utilize o seguinte comando:
+Para obter uma copia local deste repositorio, utilize o seguinte comando:
 
 ```
 git clone https://github.com/DANTE-POeTiSA/dante-corpora.git
 ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
-## InstalaÃ§Ã£o
+## Instalacao
 
 
 
 ```
 pip install dante-corpora
 ```
 
@@ -79,21 +76,21 @@
 
 ...
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## ContribuiÃ§Ã£o
 
-ContribuiÃ§Ãµes sÃ£o bem-vindas! Sinta-se Ã  vontade para propor melhorias, relatar problemas ou abrir pull requests.
+Contribuicoes sao bem-vindas! Sinta-se a vontade para propor melhorias, relatar problemas ou abrir pull requests.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## LicenÃ§a
 
-Este projeto Ã© licenciado sob a [LicenÃ§a MIT](LICENSE).
+Este projeto e licenciado sob a [LicenÃ§a MIT](LICENSE).
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 [contributors-shield]: https://img.shields.io/github/contributors/DANTE-POeTiSA/dante-corpora.svg?style=for-the-badge
 [contributors-url]: https://github.com/DANTE-POeTiSA/dante-corpora/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/DANTE-POeTiSA/dante-corpora.svg?style=for-the-badge
 [forks-url]: https://github.com/DANTE-POeTiSA/dante-corpora/network/members
```

#### html2text {}

```diff
@@ -1,35 +1,35 @@
-Metadata-Version: 2.1 Name: dante-corpora Version: 1.0.6 Summary: Pacote Python
+Metadata-Version: 2.1 Name: dante-corpora Version: 1.0.7 Summary: Pacote Python
 contendo os corpora do projeto DANTE do POeTiSA Author: felmateos Author-email:
 felmateos@gmail.com License: MIT Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: pandas==2.2.2
    [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
       shield]][issues-url] [![MIT License][license-shield]][license-url]
 
                                     _[_L_o_g_o_]
                             ******** DDAANNTTEE CCoorrppoorraa ********
         Pacote Python contendo os corpora do projeto DANTE do POeTiSA
 
-                        _R_e_p_o_r_t_ _B_u_g ÃÂ· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
+                         _R_e_p_o_r_t_ _B_u_g - _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 
---- ... ## Git Clone Para obter uma cÃÂ³pia local deste repositÃÂ³rio,
-utilize o seguinte comando: ``` git clone https://github.com/DANTE-POeTiSA/
-dante-corpora.git ```
+--- ... ## Git Clone Para obter uma copia local deste repositorio, utilize o
+seguinte comando: ``` git clone https://github.com/DANTE-POeTiSA/dante-
+corpora.git ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## InstalaÃÂ§ÃÂ£o ``` pip install dante-corpora ```
+## Instalacao ``` pip install dante-corpora ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Conjunto de Dados ...
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Documentos importantes ...
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## ContribuiÃÂ§ÃÂ£o ContribuiÃÂ§ÃÂµes sÃÂ£o bem-vindas! Sinta-se ÃÂ 
-vontade para propor melhorias, relatar problemas ou abrir pull requests.
+## ContribuiÃÂ§ÃÂ£o Contribuicoes sao bem-vindas! Sinta-se a vontade para
+propor melhorias, relatar problemas ou abrir pull requests.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## LicenÃÂ§a Este projeto ÃÂ© licenciado sob a [LicenÃÂ§a MIT](LICENSE).
+## LicenÃÂ§a Este projeto e licenciado sob a [LicenÃÂ§a MIT](LICENSE).
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/DANTE-
 POeTiSA/dante-corpora.svg?style=for-the-badge [contributors-url]: https://
 github.com/DANTE-POeTiSA/dante-corpora/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/DANTE-POeTiSA/dante-corpora.svg?style=for-
 the-badge [forks-url]: https://github.com/DANTE-POeTiSA/dante-corpora/network/
 members [stars-shield]: https://img.shields.io/github/stars/DANTE-POeTiSA/
```

### Comparing `dante_corpora-1.0.6/setup.py` & `dante_corpora-1.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='dante-corpora',
-    version='1.0.6',
+    version='1.0.7',
     description='Pacote Python contendo os corpora do projeto DANTE do POeTiSA',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='felmateos',
     author_email='felmateos@gmail.com',
     packages=find_packages(),
     package_data={
         'dante': ['data/danteshots.csv', 'data/dantestocks.csv']
     },
     install_requires=[
         'pandas==2.2.2'
     ],
     license='MIT'
 )
+
```

