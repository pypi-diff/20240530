# Comparing `tmp/secretaries-0.0.1.8.tar.gz` & `tmp/secretaries-0.0.1.9.tar.gz`

## Comparing `secretaries-0.0.1.8.tar` & `secretaries-0.0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/src/secretaries/__init__.py
--rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/src/secretaries/patterns.py
--rwxr-xr-x   0        0        0    27321 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/src/secretaries/secretary.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/src/secretaries/starter_kit_safe_words_en.csv
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/src/secretaries/startkit_ickenamn_se.csv
--rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/src/secretaries/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/tests/test.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/LICENSE
--rw-r--r--   0        0        0    15860 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/README.md
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/pyproject.toml
--rw-r--r--   0        0        0    16817 2020-02-02 00:00:00.000000 secretaries-0.0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 secretaries-0.0.1.9/src/secretaries/__init__.py
+-rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 secretaries-0.0.1.9/src/secretaries/patterns.py
+-rwxr-xr-x   0        0        0    22978 2020-02-02 00:00:00.000000 secretaries-0.0.1.9/src/secretaries/secretary.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 secretaries-0.0.1.9/src/secretaries/starter_kit_safe_words_en.csv
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 secretaries-0.0.1.9/src/secretaries/startkit_ickenamn_se.csv
+-rw-r--r--   0        0        0    12775 2020-02-02 00:00:00.000000 secretaries-0.0.1.9/src/secretaries/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 secretaries-0.0.1.9/tests/test.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 secretaries-0.0.1.9/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 secretaries-0.0.1.9/LICENSE
+-rw-r--r--   0        0        0    15860 2020-02-02 00:00:00.000000 secretaries-0.0.1.9/README.md
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 secretaries-0.0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    16817 2020-02-02 00:00:00.000000 secretaries-0.0.1.9/PKG-INFO
```

### Comparing `secretaries-0.0.1.8/src/secretaries/patterns.py` & `secretaries-0.0.1.9/src/secretaries/patterns.py`

 * *Files identical despite different names*

### Comparing `secretaries-0.0.1.8/src/secretaries/secretary.py` & `secretaries-0.0.1.9/src/secretaries/secretary.py`

 * *Files 14% similar despite different names*

```diff
@@ -483,83 +483,17 @@
     n_names_regex = df_regex.select(pl.sum('count'))[0,0]
     print_status('summary_regex', n_names_regex)
 
     ts_end = datetime.now()
     print_status('ended', ts_end.strftime("%H:%M:%S"))
     print_status("elapsed", round((ts_end - ts_init).seconds / 60, 1))
 
+    # Concatenate split texts to preserve the original length and order
+    df = unsplit(df, id_column = id_column,
+                       text_column = text_column)
+
     if single_text_mode:
-        return unsplit(df, id_column = id_column,
-                       text_column = text_column) \
-        [text_column].to_list()[0]
+        return df[text_column].to_list()[0]
     else:
-        return(df)
-
-
-
-
-# TODO
-# Möjliggör att inte skriva filer
-# Ange dependencies i requirements.txt
-# Övrig dokumentation?
-# Utforma test i test-mappen
-
-
-# KLART
-# Pusha till er1kb:s Github, därefter forka från Malmö stads
-# Fixa Readme.md-fil
-# Paketera paket
-# Vid behov: spara ner "startkit" i arbetsmapparna
-# Maskera årtal? Fyra siffror i rad som inte föregås eller efterföljs av andra siffror. Exakt sökning från år 1950 till 30 år framåt i tiden. 
-# Platshållare för radbrytningar splittas i långa texter och hittas därmed inte - löst.
-# Ta bort enskilda html-taggar som t ex <br>
-# Om NER flaggar ett ord som namn så tas det bort genomgående. Förväntat beteende? jfr. "Stig mötte Björn på en stig". - Kan oavsiktligt peka ut namn. Löst - re.sub(..., count = 1)
-# Paketera startkit med ickenamn
-# Se över kommentarer och filnamn och använd ett språk
-# Dokumentera huvudfunktionens argument
-# Uppdatera till Python 3.9
-# Kolla filers existens? - Detta görs redan när korpuset laddas, i övrigt inga obligatoriska filer
-# "Peter" maskeras men hamnar ändå under output_se/namn_corpus.csv... Löst: skapar tokens på nytt efter maskering.
-# Fixa hjälpfunktion som i tur och ordning går igenom nödvändiga mappar (uppdelat på språk) och skapar vid behov
-# Skriv bara maskerade om ord har maskerats, dvs tabellen inte är tom. Nej - skriv fil oavsett. 
-# Separera input-mapp (input_se, input_en) + parameterisera mappnamnen + korpus på svenska
-# Möjliggör att specificera egna taggar. Separera taggar och övriga inställningar/meningar, så att användaren inte kan mixtra med de senare. Struntar i denna... 
-# Flytta ut inläsning av corpus till extern hjälpfunktion
-# Dubbelkolla hur dubbelnamn hanteras (Sven-Erik etc.)
-# Separera output-mappar (output_se, output_en)
-# Se över användandet av platshållare (null_token, null_list)
-# Ge återkoppling på svenska eller engelska
-# Svenska eller engelska taggar
-# Ladda bara ner relevanta filer från Svensktext, inte hela korpuset
-# Spara engelskt namnkorpus lokalt
-# Ta bort null_token/null_list från corpus_names
-# linebreak_placeholder hamnar i regex_names.csv - möjligt att undvika?  
-# Möjliggör att mata in namn, icke-namn och maskeringar som argument till funktionen, för att kunna mata in detta manuellt i textrutor i ett webbgränssnitt. Sammanfoga dessa extra inmatningar med underlaget i mapparna (a.union(b))
-# Fixa att maskeringar i början eller slutet av texten räknas mångdubbelt
-# Dubbelkolla om det blir flera hälsningar per text och i så fall om kolumnen är i rätt format (list(str) istället för str) - names_from_regex behöver skapas med str.extract_all istället för str.extract nu när en text kan innehålla flera hälsningsfraser
-# Ge möjlighet att specificera namn under input/names, så att engelskspråkiga användare kan bygga ett eget korpus. Icke-namn trumfar namn om samma ord förekommer i båda mängderna. 
-# Fixa fel där df_corpus blir tomt och programmet får panik, dvs garantera att df_corpus inte är tom om inget namn hittas i korpuset
-# Om en lång text analyseras - fixa så att hälsningsfraser inte tar bort resten av texten, dvs byt ut (.*$) i hälsnings-regex
-# Sätt argument för språk (svenska/engelska)
-# Fixa gatunr (ersättning gjordes men resultatet sparades inte)
-# single_text_mode - spara ingen data utan returnera en enskild text
-# Ge möjlighet att välja bort ner och corpus (t ex för felsökning eller ingen gpu tillgänglig)
-# Fixa genitiv-s - Adolf flaggas men inte Adolfs
-# Ge användaren möjlighet att välja separator för csv-filer, både för data och underlag
-# Ge möjlighet att ta bort eller bevara radbrytningar
-# Splitta texter i delar om max 512 ord
-# Sortera korrekt på ID-kolumn innan data sparas, om ID är heltal
-# Använd paket för att göra line wrap på text
-
-# SKIPPAT
-# Ta bort krav på kolumnhuvudet "token" i csv-filer?
-# Ev. lägga alla parametrar i en toml-fil? 
-# Ev. lägga till smeknamn
-
-# Små bokstäver i mest_flaggade, för att undvika en massa dubbletter.
-# Does not remove initials after brackets: "Finns också på [epost]  eb" 
-# The cased bert model does not identify lowercase names as such
-# --> Use SpaCy to pick up "proper nouns" (PROPN) which have not been flagged as people or locations?! 
-# www addresses?! 
-# Obfuscate gendered pronouns? 
+        return df
```

### Comparing `secretaries-0.0.1.8/src/secretaries/startkit_ickenamn_se.csv` & `secretaries-0.0.1.9/src/secretaries/startkit_ickenamn_se.csv`

 * *Files identical despite different names*

### Comparing `secretaries-0.0.1.8/src/secretaries/utils.py` & `secretaries-0.0.1.9/src/secretaries/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 def print_status_(tags, string_id, replacement):
     """Print to the console in a specific language"""
 
     print('\n'.join(wrap(re.sub('placeholder', str(replacement), tags[string_id]), width = textwidth)))
 
 def unsplit(df, id_column, text_column):
     df = df.select([id_column, id_column + "2", 'sub_id', text_column]) \
-            .groupby(id_column) \
+            .group_by(id_column) \
             .agg(pl.col(text_column).str.concat(delimiter = ""))
     return(df)
 
 def ingest(folder, colname = 'token', sep = ',', drop_duplicates = True, keep_other_columns = False):
     """Read a folder of csv files into a Polars dataframe"""
 
     folder = re.sub(r"/$", "", folder)
@@ -252,15 +252,15 @@
             for file in svensktext_filer:
                 f = pl.read_csv(base_url + file)
                 svensktext.vstack(f, in_place = True)
             # Save locally
             svensktext.write_csv(os.path.join(corpus_path, 'svensktext.csv'))
             # Read Corpus. Sum the number of people over multiple occurrences, since the same token can be used as a forename or a surname. 
         svensktext = svensktext \
-            .groupby('name').agg(pl.col('persons').sum()) \
+            .group_by('name').agg(pl.col('persons').sum()) \
             .filter(pl.col('persons') >= min_n_persons) \
             .with_columns(pl.col('name').str.to_lowercase())
 
         corpus_names = set(svensktext.select(pl.col('name')).to_series().to_list())
         return(corpus_names)
 
     if lang == 'en':
```

### Comparing `secretaries-0.0.1.8/LICENSE` & `secretaries-0.0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `secretaries-0.0.1.8/README.md` & `secretaries-0.0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `secretaries-0.0.1.8/pyproject.toml` & `secretaries-0.0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/secretaries"]
 
 [project]
 name = "secretaries"
-version = "0.0.1.8"
+version = "0.0.1.9"
 license = "MIT"
 authors = [
   { name="Erik Broman", email="mikroberna@gmail.com" },
 ]
 description = "A utility for removing personal data in text."
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `secretaries-0.0.1.8/PKG-INFO` & `secretaries-0.0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: secretaries
-Version: 0.0.1.8
+Version: 0.0.1.9
 Summary: A utility for removing personal data in text.
 Project-URL: Homepage, https://github.com/er1kb/secretaries
 Project-URL: Bug Tracker, https://github.com/er1kb/secretaries/issues
 Author-email: Erik Broman <mikroberna@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: anonymization,gdpr,personal data,personuppgifter,python
```

