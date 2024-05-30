# Comparing `tmp/ateam_pysparklibrary-0.0.8.tar.gz` & `tmp/ateam_pysparklibrary-0.0.9.tar.gz`

## Comparing `ateam_pysparklibrary-0.0.8.tar` & `ateam_pysparklibrary-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 ateam_pysparklibrary-0.0.8/requirements.txt
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 ateam_pysparklibrary-0.0.8/.vscode/settings.json
--rw-r--r--   0        0        0     8931 2020-02-02 00:00:00.000000 ateam_pysparklibrary-0.0.8/src/aTeam_PySparkLibrary/NB_S_delta_and_key_generation.ipynb
--rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 ateam_pysparklibrary-0.0.8/src/aTeam_PySparkLibrary/NB_S_delta_and_key_generation.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ateam_pysparklibrary-0.0.8/src/aTeam_PySparkLibrary/__init__.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 ateam_pysparklibrary-0.0.8/LICENSE
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 ateam_pysparklibrary-0.0.8/README.md
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 ateam_pysparklibrary-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 ateam_pysparklibrary-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 ateam_pysparklibrary-0.0.9/requirements.txt
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 ateam_pysparklibrary-0.0.9/.vscode/settings.json
+-rw-r--r--   0        0        0     8931 2020-02-02 00:00:00.000000 ateam_pysparklibrary-0.0.9/src/aTeam_PySparkLibrary/NB_S_delta_and_key_generation.ipynb
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 ateam_pysparklibrary-0.0.9/src/aTeam_PySparkLibrary/NB_S_delta_and_key_generation.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ateam_pysparklibrary-0.0.9/src/aTeam_PySparkLibrary/__init__.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 ateam_pysparklibrary-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 ateam_pysparklibrary-0.0.9/README.md
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 ateam_pysparklibrary-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 ateam_pysparklibrary-0.0.9/PKG-INFO
```

### Comparing `ateam_pysparklibrary-0.0.8/src/aTeam_PySparkLibrary/NB_S_delta_and_key_generation.ipynb` & `ateam_pysparklibrary-0.0.9/src/aTeam_PySparkLibrary/NB_S_delta_and_key_generation.ipynb`

 * *Files identical despite different names*

### Comparing `ateam_pysparklibrary-0.0.8/src/aTeam_PySparkLibrary/NB_S_delta_and_key_generation.py` & `ateam_pysparklibrary-0.0.9/src/aTeam_PySparkLibrary/NB_S_delta_and_key_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,16 @@
 
     #sjekke om delta tabellen har data
     def exists(path):
         print("inside exists function")
         try:
             mssparkutils.fs.ls(path)
             return True
-        except:
+        except Exception as e:
+            print(f"Error accessing path: {e}")
             return False
 
     def create_select_expression(dataset_key_name):
         column_names = []
         for col in bronze_df.dtypes:
             column_names.append(col[0])
```

### Comparing `ateam_pysparklibrary-0.0.8/LICENSE` & `ateam_pysparklibrary-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ateam_pysparklibrary-0.0.8/README.md` & `ateam_pysparklibrary-0.0.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ## Last opp ny versjon til PyPI:
 
 1. Oppdater 'version' i _pyproject.toml_.
 2. Kjør ``python -m build``
 3. Kjør ``python -m twine upload dist/*``
 4. Ved feilmelding 'InvalidDistribution: Metadata is missing required fields: Name, Version', sørg for at pkginfo har versjon >= 1.10
-5. Skriv inn API token, som du finner ved å logge inn på PyPI.org. Ta kontakt med Ludvig dersom du ikke har tilgang til prosjektet i PyPI.
+5. Skriv inn API token, som du finner ved å logge inn på PyPI.org. Ta kontakt med Ludvig dersom du ikke har tilgang til prosjektet i PyPI. Hvis du får opp at du må skrive inn username, skriv inn '__token__' som username, og API token som passord.
 6. Evenentuelt endre environmenten til å bruke den nye versjonen av Librarien
 7. Det kan ta litt tid før den nye versjonen er tilgjengelig til bruk i f. eks. Fabric. Erfaringsmessig tar det rundt 5 min. 
 
 ## Legg til Library i Fabric:
 
 1. I Synapse Data Engineering, trykk New -> Environment. Lag et navn på det nye environmentet
 2. Under _Public Libraries_, trykk '_Add from PyPI_'.
```

### Comparing `ateam_pysparklibrary-0.0.8/pyproject.toml` & `ateam_pysparklibrary-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aTeam-PySparkLibrary"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Egde A-team", email="ludvig.loite@egde.no" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ateam_pysparklibrary-0.0.8/PKG-INFO` & `ateam_pysparklibrary-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aTeam-PySparkLibrary
-Version: 0.0.8
+Version: 0.0.9
 Project-URL: Homepage, https://github.com/EgdeConsulting/aTeam-PySparkLibrary
 Project-URL: Issues, https://github.com/EgdeConsulting/aTeam-PySparkLibrary/issues
 Author-email: Egde A-team <ludvig.loite@egde.no>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 
 ## Last opp ny versjon til PyPI:
 
 1. Oppdater 'version' i _pyproject.toml_.
 2. Kjør ``python -m build``
 3. Kjør ``python -m twine upload dist/*``
 4. Ved feilmelding 'InvalidDistribution: Metadata is missing required fields: Name, Version', sørg for at pkginfo har versjon >= 1.10
-5. Skriv inn API token, som du finner ved å logge inn på PyPI.org. Ta kontakt med Ludvig dersom du ikke har tilgang til prosjektet i PyPI.
+5. Skriv inn API token, som du finner ved å logge inn på PyPI.org. Ta kontakt med Ludvig dersom du ikke har tilgang til prosjektet i PyPI. Hvis du får opp at du må skrive inn username, skriv inn '__token__' som username, og API token som passord.
 6. Evenentuelt endre environmenten til å bruke den nye versjonen av Librarien
 7. Det kan ta litt tid før den nye versjonen er tilgjengelig til bruk i f. eks. Fabric. Erfaringsmessig tar det rundt 5 min. 
 
 ## Legg til Library i Fabric:
 
 1. I Synapse Data Engineering, trykk New -> Environment. Lag et navn på det nye environmentet
 2. Under _Public Libraries_, trykk '_Add from PyPI_'.
```

