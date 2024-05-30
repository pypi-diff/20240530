# Comparing `tmp/yatotem2scdl-0.0.21.tar.gz` & `tmp/yatotem2scdl-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yatotem2scdl-0.0.21.tar", last modified: Wed Dec 28 18:56:57 2022, max compression
+gzip compressed data, was "yatotem2scdl-0.1.0.tar", last modified: Wed May 29 15:58:45 2024, max compression
```

## Comparing `yatotem2scdl-0.0.21.tar` & `yatotem2scdl-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 18:56:57.907683 yatotem2scdl-0.0.21/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2022-12-28 18:56:47.000000 yatotem2scdl-0.0.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2022-12-28 18:56:57.907683 yatotem2scdl-0.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2022-12-28 18:56:47.000000 yatotem2scdl-0.0.21/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      577 2022-12-28 18:56:47.000000 yatotem2scdl-0.0.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-28 18:56:57.907683 yatotem2scdl-0.0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2022-12-28 18:56:47.000000 yatotem2scdl-0.0.21/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 18:56:57.903683 yatotem2scdl-0.0.21/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 18:56:57.903683 yatotem2scdl-0.0.21/src/yatotem2scdl/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2022-12-28 18:56:47.000000 yatotem2scdl-0.0.21/src/yatotem2scdl/TotemMetadataHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-28 18:56:47.000000 yatotem2scdl-0.0.21/src/yatotem2scdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2022-12-28 18:56:47.000000 yatotem2scdl-0.0.21/src/yatotem2scdl/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2022-12-28 18:56:47.000000 yatotem2scdl-0.0.21/src/yatotem2scdl/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2022-12-28 18:56:47.000000 yatotem2scdl-0.0.21/src/yatotem2scdl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2022-12-28 18:56:47.000000 yatotem2scdl-0.0.21/src/yatotem2scdl/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2022-12-28 18:56:47.000000 yatotem2scdl-0.0.21/src/yatotem2scdl/planDeCompte-vide.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 18:56:57.907683 yatotem2scdl-0.0.21/src/yatotem2scdl/xsl/
--rw-r--r--   0 runner    (1001) docker     (123)     7510 2022-12-28 18:56:47.000000 yatotem2scdl-0.0.21/src/yatotem2scdl/xsl/totem2xmlcsv.xsl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 18:56:57.907683 yatotem2scdl-0.0.21/src/yatotem2scdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2022-12-28 18:56:57.000000 yatotem2scdl-0.0.21/src/yatotem2scdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2022-12-28 18:56:57.000000 yatotem2scdl-0.0.21/src/yatotem2scdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-28 18:56:57.000000 yatotem2scdl-0.0.21/src/yatotem2scdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-28 18:56:57.000000 yatotem2scdl-0.0.21/src/yatotem2scdl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2022-12-28 18:56:57.000000 yatotem2scdl-0.0.21/src/yatotem2scdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-28 18:56:57.000000 yatotem2scdl-0.0.21/src/yatotem2scdl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:58:45.829033 yatotem2scdl-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-29 15:58:45.829033 yatotem2scdl-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:58:45.833033 yatotem2scdl-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:58:45.825033 yatotem2scdl-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:58:45.829033 yatotem2scdl-0.1.0/src/yatotem2scdl/
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/src/yatotem2scdl/TotemMetadataHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/src/yatotem2scdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/src/yatotem2scdl/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/src/yatotem2scdl/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/src/yatotem2scdl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/src/yatotem2scdl/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/src/yatotem2scdl/planDeCompte-vide.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:58:45.829033 yatotem2scdl-0.1.0/src/yatotem2scdl/xsl/
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/src/yatotem2scdl/xsl/totem2xmlcsv.xsl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:58:45.829033 yatotem2scdl-0.1.0/src/yatotem2scdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-29 15:58:45.000000 yatotem2scdl-0.1.0/src/yatotem2scdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-29 15:58:45.000000 yatotem2scdl-0.1.0/src/yatotem2scdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:58:45.000000 yatotem2scdl-0.1.0/src/yatotem2scdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-29 15:58:45.000000 yatotem2scdl-0.1.0/src/yatotem2scdl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 15:58:45.000000 yatotem2scdl-0.1.0/src/yatotem2scdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-29 15:58:45.000000 yatotem2scdl-0.1.0/src/yatotem2scdl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:58:45.829033 yatotem2scdl-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/tests/test_cas_alamarge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/tests/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/tests/test_etape_budgetaire.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/tests/test_extraction_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-29 15:58:41.000000 yatotem2scdl-0.1.0/tests/test_totem_budget_metadata.py
```

### Comparing `yatotem2scdl-0.0.21/LICENSE` & `yatotem2scdl-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yatotem2scdl-0.0.21/PKG-INFO` & `yatotem2scdl-0.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,21 @@
-Metadata-Version: 2.1
-Name: yatotem2scdl
-Version: 0.0.21
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE
-
 # Yet Another totem to scdl
 
 ## Rationale
 
 Largement inspiré de [datafin - totem](https://gitlab.com/datafin/totem).
 
 Le but de ce projet est de proposer une bibliothèque python de conversion de fichiers totem vers le format SCDL.
 En effet, le projet de base cité plus haut n'est pas conçu pour être utilisé comme une bibliothèque.
 
 ## Limitations
 
 - Actuellement, seuls les budgets sont supportés.
 - Les plans de comptes ne sont pas fournis avec le package. 
-  - [norme-budgetaire-downloader](https://gitlab.com/datafin/totem/-/tree/master/norme-budgetaire-downloader)
+  - [norme-budgetaire-downloader](https://gitlab.com/opendatafrance/totem/-/tree/main/norme-budgetaire-downloader?ref_type=heads)
 
 ## Quickstart
 
 ### Préparer l'environnement
 
 ```bash
 python -m venv .venv
@@ -66,7 +57,22 @@
 
 Pour upload sur un repository PyPI:
 
 ```bash
 python -m build
 twine upload --repository-url https://<REPO_URL>/repository/pypi-hosted/ dist/*
 ```
+
+## Générer les plans de comptes
+
+**Testé avec nodejs v16.20.2 et python 3.11.5**
+
+- Cloner le repository [norme-budgetaire-downloader](https://gitlab.com/opendatafrance/totem/-/tree/main/norme-budgetaire-downloader?ref_type=heads)
+
+- executer:
+```
+npm ci
+npm run build
+npm run run # Télécharge les plans de compte dans le dossier output
+```
+
+- Copier coller les plans de compte dans le dossier correspondant.
```

### Comparing `yatotem2scdl-0.0.21/pyproject.toml` & `yatotem2scdl-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yatotem2scdl"
-version = "0.0.21"
+version = "0.1.0"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = ["lxml"]
 
 [project.scripts]
 yatotem2scdl = "yatotem2scdl.main:main"
```

### Comparing `yatotem2scdl-0.0.21/src/yatotem2scdl/conversion.py` & `yatotem2scdl-0.1.0/src/yatotem2scdl/conversion.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,14 +44,28 @@
             xslt_budget (Path, optional): Surcharge le fichier de transformation XSLT en
               charge de la construction du modèle intermédiaire. Defaults to None.
         """
         if xslt_budget is None:
             xslt_budget = _BUDGET_XSLT
         self.__xslt_budget = xslt_budget
 
+    def __document_budgetaire_tree(self, totem_fpath: Path) -> ElementTree:
+        tree = etree.parse(totem_fpath)
+
+        documents_budgetaires = tree.findall('{*}DocumentBudgetaire')
+        document_budgetaire_tree = None
+        if len(documents_budgetaires) > 1:
+            raise TotemInvalideErreur("Plusieurs noeuds DocumentBudgetaire présent dans le XML")
+        if len(documents_budgetaires) == 1:
+            document_budgetaire_tree = documents_budgetaires[0]
+        if len(documents_budgetaires) == 0:
+            document_budgetaire_tree = tree
+
+        return document_budgetaire_tree
+
     def totem_budget_vers_scdl(
         self,
         totem_fpath: Path,
         pdcs_dpath: Path,
         output: TextIOBase,
         options: Options = Options(),
     ):
@@ -69,28 +83,28 @@
 
         def _extraire_pdc_for_conversion(tree, pdcs_dpath):
             try:
                 pdc_path = _extraire_plan_de_compte(tree, pdcs_dpath)
                 return pdc_path
             except TotemInvalideErreur:
                 logger.warning(
-                    f"Impossible de trouver un plan de compte pour le fichier totem."
-                    f" Le SCDL sera probablement incomplet"
+                    "Impossible de trouver un plan de compte pour le fichier totem."
+                    " Le SCDL sera probablement incomplet"
                 )
                 return None
 
         if options is None:
             options = Options()
 
         logger.info(f"Conversion du fichier budget totem: {totem_fpath}")
         try:
-            totem_tree: ElementTree = etree.parse(totem_fpath)
-            pdc_path = _extraire_pdc_for_conversion(totem_tree, pdcs_dpath)
+            docBudgetaireTree: ElementTree = self.__document_budgetaire_tree(totem_fpath)
+            pdc_path = _extraire_pdc_for_conversion(docBudgetaireTree, pdcs_dpath)
             transformed_tree = self._transform(
-                totem_tree=totem_tree, pdc_fpath=pdc_path, options=options
+                totem_tree=docBudgetaireTree, pdc_fpath=pdc_path, options=options
             )
             _xml_to_csv(transformed_tree, output, options)
 
         except ConversionErreur as err:
             raise err
         except Exception as err:
             raise ConversionErreur() from err
@@ -225,26 +239,26 @@
 
 
 def _extraire_plan_de_compte(totem_tree: ElementTree, pdcs_dpath: Path) -> Path:
 
     namespaces = _namespaces()
 
     nomenclature: Optional[str] = totem_tree.findall(
-        "/db:Budget/db:EnTeteBudget/db:Nomenclature", namespaces
+        "./db:Budget/db:EnTeteBudget/db:Nomenclature", namespaces
     )[0].attrib.get("V")
     year: Optional[str] = _xpath_totem_budget_annee_exercice(totem_tree)
 
     return _calculer_pdc_from_totem_values(nomenclature, year, pdcs_dpath)
 
 
 def _xpath_totem_budget_annee_exercice(totem_tree: ElementTree) -> Optional[str]:
 
     namespaces = _namespaces()
 
-    year_elmt = totem_tree.find("/db:Budget/db:BlocBudget/db:Exer", namespaces)
+    year_elmt = totem_tree.find("./db:Budget/db:BlocBudget/db:Exer", namespaces)
     if year_elmt is None:
         return None
     year: Optional[str] = year_elmt.attrib.get("V")
     return year
 
 
 def _namespaces() -> dict[str, str]:
@@ -266,18 +280,18 @@
 
     if not text_io.writable():
         raise ConversionErreur(f"{str(text_io)} est en lecture seule.")
 
     writer = _make_writer(text_io, options)
 
     if options.inclure_header_csv:
-        header_names = [elt.attrib["name"] for elt in tree.iterfind("/header/column")]
+        header_names = [elt.attrib["name"] for elt in tree.iterfind("./header/column")]
         writer.writerow(header_names)
 
-    for row_tag in tree.iterfind("/data/row"):
+    for row_tag in tree.iterfind("./data/row"):
         row_data = [cell.attrib["value"] for cell in row_tag.iter("cell")]
         writer.writerow(row_data)
 
 
 def _make_writer(text_io, options: Options):
     if options.lineterminator is None:
         return csv.writer(text_io)
```

### Comparing `yatotem2scdl-0.0.21/src/yatotem2scdl/data_structures.py` & `yatotem2scdl-0.1.0/src/yatotem2scdl/data_structures.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,20 +31,29 @@
     ]
     __ca_aliases__ = [
         "compte administratif",
         "compte administratif",
         "ca",
         "administratif",
     ]
+    __cfu_aliases__ = [
+        "CFU",
+        "cfu",
+        "Cfu",
+        "Compte Financier Unique",
+        "compte financier unique",
+        "Compte financier unique",
+    ]
 
     # Les valeurs de l'enum correspondent au code NatDec des fichiers totem
     PRIMITIF = 1
     DECISION_MODIF = 2
     BUDGET_SUPP = 3
     COMPTE_ADMIN = 9
+    CFU = 10
 
     @staticmethod
     def from_str(chaine: str):
         """ Parse la chaine donnée pour en faire une étape budgetaire.
 
         Chaque étape budgétaire accepte une liste d'alias comme chaine valide. 
         Par exemple, pour le compte administratif, les valeurs acceptées sont:
@@ -60,14 +69,16 @@
             return EtapeBudgetaire.PRIMITIF
         elif chaine in EtapeBudgetaire.__supplementaire_aliases__:
             return EtapeBudgetaire.BUDGET_SUPP
         elif chaine in EtapeBudgetaire.__modificative_aliases__:
             return EtapeBudgetaire.DECISION_MODIF
         elif chaine in EtapeBudgetaire.__ca_aliases__:
             return EtapeBudgetaire.COMPTE_ADMIN
+        elif chaine in EtapeBudgetaire.__cfu_aliases__:
+            return EtapeBudgetaire.CFU
         else:
             raise EtapeBudgetaireStrInvalideError(chaine)
 
     def to_scdl_compatible_str(self):
         if self is EtapeBudgetaire.PRIMITIF:
             return EtapeBudgetaire.__primitif_aliases__[0]
         elif self is EtapeBudgetaire.DECISION_MODIF:
```

### Comparing `yatotem2scdl-0.0.21/src/yatotem2scdl/exceptions.py` & `yatotem2scdl-0.1.0/src/yatotem2scdl/exceptions.py`

 * *Files identical despite different names*

### Comparing `yatotem2scdl-0.0.21/src/yatotem2scdl/main.py` & `yatotem2scdl-0.1.0/src/yatotem2scdl/main.py`

 * *Files identical despite different names*

### Comparing `yatotem2scdl-0.0.21/src/yatotem2scdl/xsl/totem2xmlcsv.xsl` & `yatotem2scdl-0.1.0/src/yatotem2scdl/xsl/totem2xmlcsv.xsl`

 * *Files 1% similar despite different names*

#### Comparing `yatotem2scdl-0.0.21/src/yatotem2scdl/xsl/totem2xmlcsv.xsl` & `yatotem2scdl-0.1.0/src/yatotem2scdl/xsl/totem2xmlcsv.xsl`

```diff
@@ -18,14 +18,15 @@
       <xsl:variable name="code" select="//totem:BlocBudget/totem:NatDec/@V"/>
       <!-- DecNat labels from CommunBudget.xsd -->
       <xsl:choose>
         <xsl:when test="$code = '01'">Budget primitif</xsl:when>
         <xsl:when test="$code = '02'">Décision modificative</xsl:when>
         <xsl:when test="$code = '03'">Budget supplémentaire</xsl:when>
         <xsl:when test="$code = '09'">Compte administratif</xsl:when>
+        <xsl:when test="$code = '10'">Compte administratif</xsl:when>
         <xsl:otherwise>
           NatDec inconnu:
           <xsl:value-of select="$code"/>
         </xsl:otherwise>
       </xsl:choose>
     </xsl:variable>
     <xsl:variable name="Exer" select="//totem:BlocBudget/totem:Exer/@V"/>
```

