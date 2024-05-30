# Comparing `tmp/bundestag_api-1.0.3.tar.gz` & `tmp/bundestag_api-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bundestag_api-1.0.3.tar", last modified: Wed Nov 23 20:22:59 2022, max compression
+gzip compressed data, was "bundestag_api-1.0.4.tar", last modified: Thu May 30 08:08:38 2024, max compression
```

## Comparing `bundestag_api-1.0.3.tar` & `bundestag_api-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-11-23 20:22:59.493539 bundestag_api-1.0.3/
--rw-rw-rw-   0        0        0     1096 2022-11-02 20:19:40.000000 bundestag_api-1.0.3/LICENSE
--rw-rw-rw-   0        0        0        0 2022-11-02 20:14:54.000000 bundestag_api-1.0.3/LICENSE.bak
--rw-rw-rw-   0        0        0       58 2022-11-02 21:15:18.000000 bundestag_api-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5063 2022-11-23 20:22:59.492530 bundestag_api-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4687 2022-11-05 10:39:10.000000 bundestag_api-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2022-11-23 20:22:59.467318 bundestag_api-1.0.3/bundestag_api/
--rw-rw-rw-   0        0        0      213 2022-11-06 12:15:22.000000 bundestag_api-1.0.3/bundestag_api/__init__.py
--rw-rw-rw-   0        0        0    48541 2022-11-22 14:11:01.000000 bundestag_api-1.0.3/bundestag_api/bta_wrapper.py
-drwxrwxrwx   0        0        0        0 2022-11-23 20:22:59.489447 bundestag_api-1.0.3/bundestag_api.egg-info/
--rw-rw-rw-   0        0        0     5063 2022-11-23 20:22:59.000000 bundestag_api-1.0.3/bundestag_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2022-11-23 20:22:59.000000 bundestag_api-1.0.3/bundestag_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-23 20:22:59.000000 bundestag_api-1.0.3/bundestag_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2022-11-23 20:22:59.000000 bundestag_api-1.0.3/bundestag_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-11-23 20:22:59.000000 bundestag_api-1.0.3/bundestag_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-23 20:22:59.493539 bundestag_api-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      728 2022-11-23 20:22:01.000000 bundestag_api-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:08:38.408520 bundestag_api-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-30 08:08:30.000000 bundestag_api-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 08:08:30.000000 bundestag_api-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-30 08:08:38.408520 bundestag_api-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-05-30 08:08:30.000000 bundestag_api-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:08:38.408520 bundestag_api-1.0.4/bundestag_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-30 08:08:30.000000 bundestag_api-1.0.4/bundestag_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41897 2024-05-30 08:08:30.000000 bundestag_api-1.0.4/bundestag_api/bta_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20096 2024-05-30 08:08:30.000000 bundestag_api-1.0.4/bundestag_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-30 08:08:30.000000 bundestag_api-1.0.4/bundestag_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:08:38.408520 bundestag_api-1.0.4/bundestag_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-30 08:08:38.000000 bundestag_api-1.0.4/bundestag_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-30 08:08:38.000000 bundestag_api-1.0.4/bundestag_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 08:08:38.000000 bundestag_api-1.0.4/bundestag_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 08:08:38.000000 bundestag_api-1.0.4/bundestag_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 08:08:38.000000 bundestag_api-1.0.4/bundestag_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 08:08:38.408520 bundestag_api-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-30 08:08:30.000000 bundestag_api-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:08:38.408520 bundestag_api-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-30 08:08:30.000000 bundestag_api-1.0.4/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-05-30 08:08:30.000000 bundestag_api-1.0.4/tests/test_btawrapper.py
```

### Comparing `bundestag_api-1.0.3/LICENSE` & `bundestag_api-1.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Julian Schibberges
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Julian Schibberges
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `bundestag_api-1.0.3/PKG-INFO` & `bundestag_api-1.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,117 +1,123 @@
-Metadata-Version: 2.1
-Name: bundestag_api
-Version: 1.0.3
-Summary: Python wrapper for the official Bundestag-API
-Home-page: https://github.com/jschibberges/Bundestag-API
-Author: Julian Schibberges
-Author-email: julian@schibberges.de
-License: MIT
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: LICENSE.bak
-
-# Bundestag-API
-A wrapper for the official Bundestag (German Federal Parliament) API in Python.
-
-The official information on the API can be found here: [Bundestag.de](https://dip.bundestag.de/%C3%BCber-dip/hilfe/api)
-
-## Installation
-
-### Pip install (recommended)
-
-```
-$ pip3 install bundestag_api
-```
-
-### Install from source
-
-```
-$ git clone https://github.com/jschibberges/Bundestag-API.git
-$ cd Bundestag-API
-$ pip install -r requirements.txt
-```
-
-## Setup
-The API requires a key to authenticate requests. Personal key can be requested from the [Bundestag administration](mailto:parlamentsdokumentation@bundestag.de). However a general API key has been published that is valid until May 31st 2023. This key is automatically used until that date when no other key is supplied by the user.
-
-## Usage
-To save your API key create a connection-object, that you can then pass to the search functions. It will save you time, should you have to change API keys at a later date. If you don't supply an API key, the official API key will be used until 31st of May 2023. 
-```
-import bundestag_api
-bta = bundestag_api.btaConnection() #if you want to use your own API key, supply it via "apikey="XXX")
-data = bta.query(resource="vorgang")
-for d in data:
-    print(d["drucksachetyp"]+": "+d["titel"])
-```
-The query-function serves as a general search function that can be used to query all resources of the API. However, you will also have to specify all relevant parameters for your search. Data is returned as a dictionary (which can easily be saved as json). Minimally the resource type needs to specified.
-
-For each resource type the api offers a search function and a get function are implemented. Get functions retrieve data for specific entity ids while search function offer all parameters that are relevant to the resource type. Example for documents (Drucksachen):
-```
-bta.search_document(datestart="2022-11-01",dateend="2022-11-01",institution="BT")
-bta.get_document(btid=264030)
-```
-The Bundestag API serves 8 different resources though 2 are doubled with the only difference being whether the document text is returned via the API. 
-
-### Activities ("AktivitÃ¤t")
-Get one or more activities by their ID
-```
-bta.get_activity(btid)
-```
-Search for documents by specifying parameters for start and end date or institution. Important: The standard number of documents returned are 100. If more are desired, the "num" parameter must be set.
-```
-bta.search_activity()
-```
-### Documents / Full-Text ("Drucksache")
-Get one or more documents by their ID
-```
-bta.get_document(btid)
-```
-Search for documents by specifying parameters for start and end date or institution. Important: The standard number of documents returned are 100. If more are desired, the "num" parameter must be set.
-```
-bta.search_document()
-```
-The API differentiates between documents and documents incuding full-text of the document. The functions always query the full-text resource.
-
-### Persons ("Person")
-Get one or more persons by their ID
-```
-bta.get_person(btid)
-```
-Search for persons by specifying parameters for start and end date or institution. Important: The standard number of documents returned are 100. If more are desired, the "num" parameter must be set.
-```
-bta.search_person()
-```
-### Plenary Protocols / Full-Text ("Plenarprotokoll")
-Get one or more plenary protocols by their ID
-```
-bta.get_plenaryprotocol(btid)
-```
-Search for plenary protocols by specifying parameters for start and end date or institution. Important: The standard number of documents returned are 100. If more are desired, the "num" parameter must be set.
-```
-bta.search_plenaryprotocol()
-```
-The API differentiates between plenary protocols and plenary protocols incuding full-text of the protocol. The functions always query the full-text resource.
-
-### Procedures ("Vorgang")
-Get one or more procedures by their ID
-```
-bta.get_procedure(btid)
-```
-Search for procedures by specifying parameters for start and end date or institution. Important: The standard number of documents returned are 100. If more are desired, the "num" parameter must be set.
-```
-bta.search_procedure()
-```
-### Procedure Positions ("Vorgangsposition")
-Get one or more procedure positions by their ID
-```
-bta.get_procedure(btid)
-```
-Search for procedure positions by specifying parameters for start and end date or institution. Important: The standard number of documents returned are 100. If more are desired, the "num" parameter must be set.
-```
-bta.search_procedure()
-```
-
-## ToDo's
-- Parallelize requests for larger queries
-- Extend Class methods
+Metadata-Version: 2.1
+Name: bundestag_api
+Version: 1.0.4
+Summary: Python wrapper for the official Bundestag-API
+Home-page: https://github.com/jschibberges/Bundestag-API
+Author: Julian Schibberges
+Author-email: julian@schibberges.de
+License: MIT
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.0.0
+
+# Bundestag-API
+A wrapper for the official Bundestag (German Federal Parliament) API in Python. It aim is to make querying the API a little easier in Python and relieve you from writing a lot of boilerplate code. 
+
+It currently doesn't encompass a 100% of the lastest API parameters (see To-Do section) but aims to do so shortly.
+
+The official information on the API can be found here: [Bundestag.de](https://dip.bundestag.de/%C3%BCber-dip/hilfe/api)
+
+## Installation
+
+### Pip install (recommended)
+
+```
+$ pip3 install bundestag_api
+```
+
+### Install from source
+
+```
+$ git clone https://github.com/jschibberges/Bundestag-API.git
+$ cd Bundestag-API
+$ pip install -r requirements.txt
+```
+
+## Setup
+The API requires a key to authenticate requests. Personal key can be requested from the [Bundestag administration](mailto:parlamentsdokumentation@bundestag.de). However a general API key has been published that is valid until May 31st 2024. This key is automatically used until that date when no other key is supplied by the user.
+
+## Usage
+To save your API key create a connection-object, that you can then pass to the search functions. It will save you time, should you have to change API keys at a later date. If you don't supply an API key, the official API key will be used until 31st of May 2024. 
+```
+import bundestag_api
+bta = bundestag_api.btaConnection() #if you want to use your own API key, supply it via "apikey="XXX")
+data = bta.search_document()
+for d in data:
+    print(d["drucksachetyp"]+": "+d["titel"])
+```
+The query-function serves as a general search function that can be used to query all resources of the API. However, you will also have to specify all relevant parameters for your search. Data is returned as a dictionary (which can easily be saved as json). Minimally the resource type needs to specified.
+
+For each resource type the api offers a search function and a get function are implemented. Get functions retrieve data for specific entity ids while search function offer all parameters that are relevant to the resource type. Example for documents (Drucksachen):
+```
+bta.search_document(datestart="2022-11-01",dateend="2022-11-01",institution="BT")
+bta.get_document(btid=264030)
+```
+The Bundestag API serves 8 different resources though 2 are doubled with the only difference being whether the document text is returned via the API. 
+
+### Activities ("Aktivität")
+Get one or more activities by their ID
+```
+bta.get_activity(btid)
+```
+Search for documents by specifying parameters for start and end date or institution. Important: The standard number of entities returned are 100. If more are desired, the "num" parameter must be set.
+```
+bta.search_activity()
+```
+### Documents / Full-Text ("Drucksache")
+Get one or more documents by their ID
+```
+bta.get_document(btid)
+```
+Search for documents by specifying parameters for start and end date or institution. Important: The standard number of entities returned are 100. If more are desired, the "num" parameter must be set.
+```
+bta.search_document()
+```
+"fulltext=True" can be passed as parameter to retrieve the full text of the document (if available). It defaults to False.
+
+### Persons ("Person")
+Get one or more persons by their ID
+```
+bta.get_person(btid)
+```
+Search for persons by specifying parameters for start and end date or institution. Important: The standard number of entities returned are 100. If more are desired, the "num" parameter must be set.
+```
+bta.search_person()
+```
+### Plenary Protocols / Full-Text ("Plenarprotokoll")
+Get one or more plenary protocols by their ID
+```
+bta.get_plenaryprotocol(btid)
+```
+Search for plenary protocols by specifying parameters for start and end date or institution. Important: The standard number of entities returned are 100. If more are desired, the "num" parameter must be set.
+```
+bta.search_plenaryprotocol()
+```
+"fulltext=True" can be passed as parameter to retrieve the full text of the plenary protocols (if available). It defaults to False.
+
+### Procedures ("Vorgang")
+Get one or more procedures by their ID
+```
+bta.get_procedure(btid)
+```
+Search for procedures by specifying parameters for start and end date or institution. Important: The standard number of entities returned are 100. If more are desired, the "num" parameter must be set.
+```
+bta.search_procedure()
+```
+### Procedure Positions ("Vorgangsposition")
+Get one or more procedure positions by their ID
+```
+bta.get_procedure(btid)
+```
+Search for procedure positions by specifying parameters for start and end date or institution. Important: The standard number of entities returned are 100. If more are desired, the "num" parameter must be set.
+```
+bta.search_procedure()
+```
+
+## ToDo's
+- Implement filters for GESTA-Number, Beratungsstand, Fundstelle, Initiative, Ressort (federführend), Verkündungsblatt_Kürzel, Vorgangstyp, Vorgangstyp-Notation
+- Implement retries before failure
+- Implement sufficient unit tests
+- Implement more extensive logging
+- Parallelize requests for larger queries
+- Extend Class methods
```

### Comparing `bundestag_api-1.0.3/README.md` & `bundestag_api-1.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,104 +1,110 @@
-# Bundestag-API
-A wrapper for the official Bundestag (German Federal Parliament) API in Python.
-
-The official information on the API can be found here: [Bundestag.de](https://dip.bundestag.de/%C3%BCber-dip/hilfe/api)
-
-## Installation
-
-### Pip install (recommended)
-
-```
-$ pip3 install bundestag_api
-```
-
-### Install from source
-
-```
-$ git clone https://github.com/jschibberges/Bundestag-API.git
-$ cd Bundestag-API
-$ pip install -r requirements.txt
-```
-
-## Setup
-The API requires a key to authenticate requests. Personal key can be requested from the [Bundestag administration](mailto:parlamentsdokumentation@bundestag.de). However a general API key has been published that is valid until May 31st 2023. This key is automatically used until that date when no other key is supplied by the user.
-
-## Usage
-To save your API key create a connection-object, that you can then pass to the search functions. It will save you time, should you have to change API keys at a later date. If you don't supply an API key, the official API key will be used until 31st of May 2023. 
-```
-import bundestag_api
-bta = bundestag_api.btaConnection() #if you want to use your own API key, supply it via "apikey="XXX")
-data = bta.query(resource="vorgang")
-for d in data:
-    print(d["drucksachetyp"]+": "+d["titel"])
-```
-The query-function serves as a general search function that can be used to query all resources of the API. However, you will also have to specify all relevant parameters for your search. Data is returned as a dictionary (which can easily be saved as json). Minimally the resource type needs to specified.
-
-For each resource type the api offers a search function and a get function are implemented. Get functions retrieve data for specific entity ids while search function offer all parameters that are relevant to the resource type. Example for documents (Drucksachen):
-```
-bta.search_document(datestart="2022-11-01",dateend="2022-11-01",institution="BT")
-bta.get_document(btid=264030)
-```
-The Bundestag API serves 8 different resources though 2 are doubled with the only difference being whether the document text is returned via the API. 
-
-### Activities ("Aktivität")
-Get one or more activities by their ID
-```
-bta.get_activity(btid)
-```
-Search for documents by specifying parameters for start and end date or institution. Important: The standard number of documents returned are 100. If more are desired, the "num" parameter must be set.
-```
-bta.search_activity()
-```
-### Documents / Full-Text ("Drucksache")
-Get one or more documents by their ID
-```
-bta.get_document(btid)
-```
-Search for documents by specifying parameters for start and end date or institution. Important: The standard number of documents returned are 100. If more are desired, the "num" parameter must be set.
-```
-bta.search_document()
-```
-The API differentiates between documents and documents incuding full-text of the document. The functions always query the full-text resource.
-
-### Persons ("Person")
-Get one or more persons by their ID
-```
-bta.get_person(btid)
-```
-Search for persons by specifying parameters for start and end date or institution. Important: The standard number of documents returned are 100. If more are desired, the "num" parameter must be set.
-```
-bta.search_person()
-```
-### Plenary Protocols / Full-Text ("Plenarprotokoll")
-Get one or more plenary protocols by their ID
-```
-bta.get_plenaryprotocol(btid)
-```
-Search for plenary protocols by specifying parameters for start and end date or institution. Important: The standard number of documents returned are 100. If more are desired, the "num" parameter must be set.
-```
-bta.search_plenaryprotocol()
-```
-The API differentiates between plenary protocols and plenary protocols incuding full-text of the protocol. The functions always query the full-text resource.
-
-### Procedures ("Vorgang")
-Get one or more procedures by their ID
-```
-bta.get_procedure(btid)
-```
-Search for procedures by specifying parameters for start and end date or institution. Important: The standard number of documents returned are 100. If more are desired, the "num" parameter must be set.
-```
-bta.search_procedure()
-```
-### Procedure Positions ("Vorgangsposition")
-Get one or more procedure positions by their ID
-```
-bta.get_procedure(btid)
-```
-Search for procedure positions by specifying parameters for start and end date or institution. Important: The standard number of documents returned are 100. If more are desired, the "num" parameter must be set.
-```
-bta.search_procedure()
-```
-
-## ToDo's
-- Parallelize requests for larger queries
+# Bundestag-API
+A wrapper for the official Bundestag (German Federal Parliament) API in Python. It aim is to make querying the API a little easier in Python and relieve you from writing a lot of boilerplate code. 
+
+It currently doesn't encompass a 100% of the lastest API parameters (see To-Do section) but aims to do so shortly.
+
+The official information on the API can be found here: [Bundestag.de](https://dip.bundestag.de/%C3%BCber-dip/hilfe/api)
+
+## Installation
+
+### Pip install (recommended)
+
+```
+$ pip3 install bundestag_api
+```
+
+### Install from source
+
+```
+$ git clone https://github.com/jschibberges/Bundestag-API.git
+$ cd Bundestag-API
+$ pip install -r requirements.txt
+```
+
+## Setup
+The API requires a key to authenticate requests. Personal key can be requested from the [Bundestag administration](mailto:parlamentsdokumentation@bundestag.de). However a general API key has been published that is valid until May 31st 2024. This key is automatically used until that date when no other key is supplied by the user.
+
+## Usage
+To save your API key create a connection-object, that you can then pass to the search functions. It will save you time, should you have to change API keys at a later date. If you don't supply an API key, the official API key will be used until 31st of May 2024. 
+```
+import bundestag_api
+bta = bundestag_api.btaConnection() #if you want to use your own API key, supply it via "apikey="XXX")
+data = bta.search_document()
+for d in data:
+    print(d["drucksachetyp"]+": "+d["titel"])
+```
+The query-function serves as a general search function that can be used to query all resources of the API. However, you will also have to specify all relevant parameters for your search. Data is returned as a dictionary (which can easily be saved as json). Minimally the resource type needs to specified.
+
+For each resource type the api offers a search function and a get function are implemented. Get functions retrieve data for specific entity ids while search function offer all parameters that are relevant to the resource type. Example for documents (Drucksachen):
+```
+bta.search_document(datestart="2022-11-01",dateend="2022-11-01",institution="BT")
+bta.get_document(btid=264030)
+```
+The Bundestag API serves 8 different resources though 2 are doubled with the only difference being whether the document text is returned via the API. 
+
+### Activities ("Aktivität")
+Get one or more activities by their ID
+```
+bta.get_activity(btid)
+```
+Search for documents by specifying parameters for start and end date or institution. Important: The standard number of entities returned are 100. If more are desired, the "num" parameter must be set.
+```
+bta.search_activity()
+```
+### Documents / Full-Text ("Drucksache")
+Get one or more documents by their ID
+```
+bta.get_document(btid)
+```
+Search for documents by specifying parameters for start and end date or institution. Important: The standard number of entities returned are 100. If more are desired, the "num" parameter must be set.
+```
+bta.search_document()
+```
+"fulltext=True" can be passed as parameter to retrieve the full text of the document (if available). It defaults to False.
+
+### Persons ("Person")
+Get one or more persons by their ID
+```
+bta.get_person(btid)
+```
+Search for persons by specifying parameters for start and end date or institution. Important: The standard number of entities returned are 100. If more are desired, the "num" parameter must be set.
+```
+bta.search_person()
+```
+### Plenary Protocols / Full-Text ("Plenarprotokoll")
+Get one or more plenary protocols by their ID
+```
+bta.get_plenaryprotocol(btid)
+```
+Search for plenary protocols by specifying parameters for start and end date or institution. Important: The standard number of entities returned are 100. If more are desired, the "num" parameter must be set.
+```
+bta.search_plenaryprotocol()
+```
+"fulltext=True" can be passed as parameter to retrieve the full text of the plenary protocols (if available). It defaults to False.
+
+### Procedures ("Vorgang")
+Get one or more procedures by their ID
+```
+bta.get_procedure(btid)
+```
+Search for procedures by specifying parameters for start and end date or institution. Important: The standard number of entities returned are 100. If more are desired, the "num" parameter must be set.
+```
+bta.search_procedure()
+```
+### Procedure Positions ("Vorgangsposition")
+Get one or more procedure positions by their ID
+```
+bta.get_procedure(btid)
+```
+Search for procedure positions by specifying parameters for start and end date or institution. Important: The standard number of entities returned are 100. If more are desired, the "num" parameter must be set.
+```
+bta.search_procedure()
+```
+
+## ToDo's
+- Implement filters for GESTA-Number, Beratungsstand, Fundstelle, Initiative, Ressort (federführend), Verkündungsblatt_Kürzel, Vorgangstyp, Vorgangstyp-Notation
+- Implement retries before failure
+- Implement sufficient unit tests
+- Implement more extensive logging
+- Parallelize requests for larger queries
 - Extend Class methods
```

### Comparing `bundestag_api-1.0.3/bundestag_api.egg-info/PKG-INFO` & `bundestag_api-1.0.4/bundestag_api.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,117 +1,123 @@
-Metadata-Version: 2.1
-Name: bundestag-api
-Version: 1.0.3
-Summary: Python wrapper for the official Bundestag-API
-Home-page: https://github.com/jschibberges/Bundestag-API
-Author: Julian Schibberges
-Author-email: julian@schibberges.de
-License: MIT
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: LICENSE.bak
-
-# Bundestag-API
-A wrapper for the official Bundestag (German Federal Parliament) API in Python.
-
-The official information on the API can be found here: [Bundestag.de](https://dip.bundestag.de/%C3%BCber-dip/hilfe/api)
-
-## Installation
-
-### Pip install (recommended)
-
-```
-$ pip3 install bundestag_api
-```
-
-### Install from source
-
-```
-$ git clone https://github.com/jschibberges/Bundestag-API.git
-$ cd Bundestag-API
-$ pip install -r requirements.txt
-```
-
-## Setup
-The API requires a key to authenticate requests. Personal key can be requested from the [Bundestag administration](mailto:parlamentsdokumentation@bundestag.de). However a general API key has been published that is valid until May 31st 2023. This key is automatically used until that date when no other key is supplied by the user.
-
-## Usage
-To save your API key create a connection-object, that you can then pass to the search functions. It will save you time, should you have to change API keys at a later date. If you don't supply an API key, the official API key will be used until 31st of May 2023. 
-```
-import bundestag_api
-bta = bundestag_api.btaConnection() #if you want to use your own API key, supply it via "apikey="XXX")
-data = bta.query(resource="vorgang")
-for d in data:
-    print(d["drucksachetyp"]+": "+d["titel"])
-```
-The query-function serves as a general search function that can be used to query all resources of the API. However, you will also have to specify all relevant parameters for your search. Data is returned as a dictionary (which can easily be saved as json). Minimally the resource type needs to specified.
-
-For each resource type the api offers a search function and a get function are implemented. Get functions retrieve data for specific entity ids while search function offer all parameters that are relevant to the resource type. Example for documents (Drucksachen):
-```
-bta.search_document(datestart="2022-11-01",dateend="2022-11-01",institution="BT")
-bta.get_document(btid=264030)
-```
-The Bundestag API serves 8 different resources though 2 are doubled with the only difference being whether the document text is returned via the API. 
-
-### Activities ("AktivitÃ¤t")
-Get one or more activities by their ID
-```
-bta.get_activity(btid)
-```
-Search for documents by specifying parameters for start and end date or institution. Important: The standard number of documents returned are 100. If more are desired, the "num" parameter must be set.
-```
-bta.search_activity()
-```
-### Documents / Full-Text ("Drucksache")
-Get one or more documents by their ID
-```
-bta.get_document(btid)
-```
-Search for documents by specifying parameters for start and end date or institution. Important: The standard number of documents returned are 100. If more are desired, the "num" parameter must be set.
-```
-bta.search_document()
-```
-The API differentiates between documents and documents incuding full-text of the document. The functions always query the full-text resource.
-
-### Persons ("Person")
-Get one or more persons by their ID
-```
-bta.get_person(btid)
-```
-Search for persons by specifying parameters for start and end date or institution. Important: The standard number of documents returned are 100. If more are desired, the "num" parameter must be set.
-```
-bta.search_person()
-```
-### Plenary Protocols / Full-Text ("Plenarprotokoll")
-Get one or more plenary protocols by their ID
-```
-bta.get_plenaryprotocol(btid)
-```
-Search for plenary protocols by specifying parameters for start and end date or institution. Important: The standard number of documents returned are 100. If more are desired, the "num" parameter must be set.
-```
-bta.search_plenaryprotocol()
-```
-The API differentiates between plenary protocols and plenary protocols incuding full-text of the protocol. The functions always query the full-text resource.
-
-### Procedures ("Vorgang")
-Get one or more procedures by their ID
-```
-bta.get_procedure(btid)
-```
-Search for procedures by specifying parameters for start and end date or institution. Important: The standard number of documents returned are 100. If more are desired, the "num" parameter must be set.
-```
-bta.search_procedure()
-```
-### Procedure Positions ("Vorgangsposition")
-Get one or more procedure positions by their ID
-```
-bta.get_procedure(btid)
-```
-Search for procedure positions by specifying parameters for start and end date or institution. Important: The standard number of documents returned are 100. If more are desired, the "num" parameter must be set.
-```
-bta.search_procedure()
-```
-
-## ToDo's
-- Parallelize requests for larger queries
-- Extend Class methods
+Metadata-Version: 2.1
+Name: bundestag_api
+Version: 1.0.4
+Summary: Python wrapper for the official Bundestag-API
+Home-page: https://github.com/jschibberges/Bundestag-API
+Author: Julian Schibberges
+Author-email: julian@schibberges.de
+License: MIT
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.0.0
+
+# Bundestag-API
+A wrapper for the official Bundestag (German Federal Parliament) API in Python. It aim is to make querying the API a little easier in Python and relieve you from writing a lot of boilerplate code. 
+
+It currently doesn't encompass a 100% of the lastest API parameters (see To-Do section) but aims to do so shortly.
+
+The official information on the API can be found here: [Bundestag.de](https://dip.bundestag.de/%C3%BCber-dip/hilfe/api)
+
+## Installation
+
+### Pip install (recommended)
+
+```
+$ pip3 install bundestag_api
+```
+
+### Install from source
+
+```
+$ git clone https://github.com/jschibberges/Bundestag-API.git
+$ cd Bundestag-API
+$ pip install -r requirements.txt
+```
+
+## Setup
+The API requires a key to authenticate requests. Personal key can be requested from the [Bundestag administration](mailto:parlamentsdokumentation@bundestag.de). However a general API key has been published that is valid until May 31st 2024. This key is automatically used until that date when no other key is supplied by the user.
+
+## Usage
+To save your API key create a connection-object, that you can then pass to the search functions. It will save you time, should you have to change API keys at a later date. If you don't supply an API key, the official API key will be used until 31st of May 2024. 
+```
+import bundestag_api
+bta = bundestag_api.btaConnection() #if you want to use your own API key, supply it via "apikey="XXX")
+data = bta.search_document()
+for d in data:
+    print(d["drucksachetyp"]+": "+d["titel"])
+```
+The query-function serves as a general search function that can be used to query all resources of the API. However, you will also have to specify all relevant parameters for your search. Data is returned as a dictionary (which can easily be saved as json). Minimally the resource type needs to specified.
+
+For each resource type the api offers a search function and a get function are implemented. Get functions retrieve data for specific entity ids while search function offer all parameters that are relevant to the resource type. Example for documents (Drucksachen):
+```
+bta.search_document(datestart="2022-11-01",dateend="2022-11-01",institution="BT")
+bta.get_document(btid=264030)
+```
+The Bundestag API serves 8 different resources though 2 are doubled with the only difference being whether the document text is returned via the API. 
+
+### Activities ("Aktivität")
+Get one or more activities by their ID
+```
+bta.get_activity(btid)
+```
+Search for documents by specifying parameters for start and end date or institution. Important: The standard number of entities returned are 100. If more are desired, the "num" parameter must be set.
+```
+bta.search_activity()
+```
+### Documents / Full-Text ("Drucksache")
+Get one or more documents by their ID
+```
+bta.get_document(btid)
+```
+Search for documents by specifying parameters for start and end date or institution. Important: The standard number of entities returned are 100. If more are desired, the "num" parameter must be set.
+```
+bta.search_document()
+```
+"fulltext=True" can be passed as parameter to retrieve the full text of the document (if available). It defaults to False.
+
+### Persons ("Person")
+Get one or more persons by their ID
+```
+bta.get_person(btid)
+```
+Search for persons by specifying parameters for start and end date or institution. Important: The standard number of entities returned are 100. If more are desired, the "num" parameter must be set.
+```
+bta.search_person()
+```
+### Plenary Protocols / Full-Text ("Plenarprotokoll")
+Get one or more plenary protocols by their ID
+```
+bta.get_plenaryprotocol(btid)
+```
+Search for plenary protocols by specifying parameters for start and end date or institution. Important: The standard number of entities returned are 100. If more are desired, the "num" parameter must be set.
+```
+bta.search_plenaryprotocol()
+```
+"fulltext=True" can be passed as parameter to retrieve the full text of the plenary protocols (if available). It defaults to False.
+
+### Procedures ("Vorgang")
+Get one or more procedures by their ID
+```
+bta.get_procedure(btid)
+```
+Search for procedures by specifying parameters for start and end date or institution. Important: The standard number of entities returned are 100. If more are desired, the "num" parameter must be set.
+```
+bta.search_procedure()
+```
+### Procedure Positions ("Vorgangsposition")
+Get one or more procedure positions by their ID
+```
+bta.get_procedure(btid)
+```
+Search for procedure positions by specifying parameters for start and end date or institution. Important: The standard number of entities returned are 100. If more are desired, the "num" parameter must be set.
+```
+bta.search_procedure()
+```
+
+## ToDo's
+- Implement filters for GESTA-Number, Beratungsstand, Fundstelle, Initiative, Ressort (federführend), Verkündungsblatt_Kürzel, Vorgangstyp, Vorgangstyp-Notation
+- Implement retries before failure
+- Implement sufficient unit tests
+- Implement more extensive logging
+- Parallelize requests for larger queries
+- Extend Class methods
```

### Comparing `bundestag_api-1.0.3/setup.py` & `bundestag_api-1.0.4/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# -*- coding: utf-8 -*-
-
-from setuptools import setup, find_packages
-
-from pathlib import Path
-this_directory = Path("__file__").parent
-long_description = (this_directory / "README.md").read_text()
-
-setup(
-    author='Julian Schibberges',
-    author_email="julian@schibberges.de",
-    description='Python wrapper for the official Bundestag-API',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url="https://github.com/jschibberges/Bundestag-API",
-    readme="README.md",
-    license="MIT",
-    name='bundestag_api',
-    version='1.0.3',
-    packages=find_packages(),
-    install_requires=[
-         'requests>=2.0.0',
-    ],
-    python_requires='>=3.7.0'
-)
+# -*- coding: utf-8 -*-
+
+from setuptools import setup, find_packages
+
+from pathlib import Path
+this_directory = Path("__file__").parent
+long_description = (this_directory / "README.md").read_text()
+
+setup(
+    author='Julian Schibberges',
+    author_email="julian@schibberges.de",
+    description='Python wrapper for the official Bundestag-API',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url="https://github.com/jschibberges/Bundestag-API",
+    readme="README.md",
+    license="MIT",
+    name='bundestag_api',
+    version='1.0.4',
+    packages=find_packages(),
+    install_requires=[
+         'requests>=2.0.0',
+    ],
+    python_requires='>=3.7.0'
+)
```

