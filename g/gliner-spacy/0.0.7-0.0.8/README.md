# Comparing `tmp/gliner-spacy-0.0.7.tar.gz` & `tmp/gliner-spacy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gliner-spacy-0.0.7.tar", last modified: Tue May 28 13:10:14 2024, max compression
+gzip compressed data, was "gliner-spacy-0.0.8.tar", last modified: Thu May 30 10:39:06 2024, max compression
```

## Comparing `gliner-spacy-0.0.7.tar` & `gliner-spacy-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-05-28 13:10:14.588565 gliner-spacy-0.0.7/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     1073 2024-04-08 09:18:42.000000 gliner-spacy-0.0.7/LICENSE
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     3506 2024-05-28 13:10:14.588458 gliner-spacy-0.0.7/PKG-INFO
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     2798 2024-05-28 12:18:02.000000 gliner-spacy-0.0.7/README.md
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-05-28 13:10:14.587778 gliner-spacy-0.0.7/gliner_spacy/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       60 2024-04-25 03:46:10.000000 gliner-spacy-0.0.7/gliner_spacy/__init__.py
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     3177 2024-05-28 12:57:57.000000 gliner-spacy-0.0.7/gliner_spacy/pipeline.py
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       22 2024-05-28 13:07:17.000000 gliner-spacy-0.0.7/gliner_spacy/version.py
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-05-28 13:10:14.588298 gliner-spacy-0.0.7/gliner_spacy.egg-info/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     3506 2024-05-28 13:10:14.000000 gliner-spacy-0.0.7/gliner_spacy.egg-info/PKG-INFO
--rw-r--r--   0 wjbmattingly   (501) staff       (20)      279 2024-05-28 13:10:14.000000 gliner-spacy-0.0.7/gliner_spacy.egg-info/SOURCES.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)        1 2024-05-28 13:10:14.000000 gliner-spacy-0.0.7/gliner_spacy.egg-info/dependency_links.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       27 2024-05-28 13:10:14.000000 gliner-spacy-0.0.7/gliner_spacy.egg-info/requires.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-05-28 13:10:14.000000 gliner-spacy-0.0.7/gliner_spacy.egg-info/top_level.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       38 2024-05-28 13:10:14.588598 gliner-spacy-0.0.7/setup.cfg
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     1309 2024-05-28 12:41:34.000000 gliner-spacy-0.0.7/setup.py
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-05-30 10:39:06.804256 gliner-spacy-0.0.8/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     1073 2024-04-08 09:18:42.000000 gliner-spacy-0.0.8/LICENSE
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     3527 2024-05-30 10:39:06.804138 gliner-spacy-0.0.8/PKG-INFO
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     2819 2024-05-30 10:37:48.000000 gliner-spacy-0.0.8/README.md
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-05-30 10:39:06.803437 gliner-spacy-0.0.8/gliner_spacy/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       60 2024-04-25 03:46:10.000000 gliner-spacy-0.0.8/gliner_spacy/__init__.py
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     3181 2024-05-30 10:37:45.000000 gliner-spacy-0.0.8/gliner_spacy/pipeline.py
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       22 2024-05-30 10:37:48.000000 gliner-spacy-0.0.8/gliner_spacy/version.py
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-05-30 10:39:06.804002 gliner-spacy-0.0.8/gliner_spacy.egg-info/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     3527 2024-05-30 10:39:06.000000 gliner-spacy-0.0.8/gliner_spacy.egg-info/PKG-INFO
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)      318 2024-05-30 10:39:06.000000 gliner-spacy-0.0.8/gliner_spacy.egg-info/SOURCES.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)        1 2024-05-30 10:39:06.000000 gliner-spacy-0.0.8/gliner_spacy.egg-info/dependency_links.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       67 2024-05-30 10:39:06.000000 gliner-spacy-0.0.8/gliner_spacy.egg-info/entry_points.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       27 2024-05-30 10:39:06.000000 gliner-spacy-0.0.8/gliner_spacy.egg-info/requires.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-05-30 10:39:06.000000 gliner-spacy-0.0.8/gliner_spacy.egg-info/top_level.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       38 2024-05-30 10:39:06.804293 gliner-spacy-0.0.8/setup.cfg
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     1414 2024-05-30 10:37:48.000000 gliner-spacy-0.0.8/setup.py
```

### Comparing `gliner-spacy-0.0.7/LICENSE` & `gliner-spacy-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gliner-spacy-0.0.7/PKG-INFO` & `gliner-spacy-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gliner-spacy
-Version: 0.0.7
+Version: 0.0.8
 Summary: A SpaCy wrapper for the GLiNER model for enhanced Named Entity Recognition capabilities
 Home-page: https://github.com/theirstory/gliner-spacy
 Author: William J. B. Mattingly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -35,24 +35,23 @@
 ```bash
 pip install gliner-spacy
 ```
 
 ## Usage
 To use this wrapper in your SpaCy pipeline, follow these steps:
 
-1. Import SpaCy and the GLiNER SpaCy wrapper.
+1. Import SpaCy.
 2. Create a SpaCy `Language` instance.
 3. Add the `gliner_spacy` component to the SpaCy pipeline.
 4. Process text using the pipeline.
 
 Example code:
 
 ```python
 import spacy
-from gliner_spacy.pipeline import GlinerSpacy
 
 nlp = spacy.blank("en")
 nlp.add_pipe("gliner_spacy")
 text = "This is a text about Bill Gates and Microsoft."
 doc = nlp(text)
 
 for ent in doc.ents:
@@ -66,34 +65,38 @@
 Microsoft organization
 ```
 
 ## Example with Custom Configs
 
 ```python
 import spacy
-from gliner_spacy.pipeline import GlinerSpacy
 
 custom_spacy_config = { "gliner_model": "urchade/gliner_multi",
                             "chunk_size": 250,
                             "labels": ["people","company","punctuation"],
                             "style": "ent"}
 nlp = spacy.blank("en")
 nlp.add_pipe("gliner_spacy", config=custom_spacy_config)
 
 text = "This is a text about Bill Gates and Microsoft."
 doc = nlp(text)
 
 for ent in doc.ents:
-    print(ent.text, ent.label_)
+    print(ent.text, ent.label_, ent._.score)
+
+#Output
+# Bill Gates person 0.9967108964920044
+# Tom person 0.9612326622009277
+# Microsoft organization 0.9966742992401123    
 ```
 
 ## Configuration
 The default configuration of the wrapper can be modified according to your requirements. The configurable parameters are:
 - `gliner_model`: The GLiNER model to be used.
 - `chunk_size`: Size of the text chunk to be processed at once.
 - `labels`: The entity labels to be recognized.
 - `style`: The style of output for the entities (either 'ent' or 'span').
 - `threshold`: The threshold of the GliNER model (controls the degree to which a hit is considered an entity)
-- `map_location`: The device on which to run the model: `cpu` or `gpu`
+- `map_location`: The device on which to run the model: `cpu` or `cuda`
 
 ## Contributing
 Contributions to this project are welcome. Please ensure that your code adheres to the project's coding standards and include tests for new features.
```

### Comparing `gliner-spacy-0.0.7/README.md` & `gliner-spacy-0.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,24 +17,23 @@
 ```bash
 pip install gliner-spacy
 ```
 
 ## Usage
 To use this wrapper in your SpaCy pipeline, follow these steps:
 
-1. Import SpaCy and the GLiNER SpaCy wrapper.
+1. Import SpaCy.
 2. Create a SpaCy `Language` instance.
 3. Add the `gliner_spacy` component to the SpaCy pipeline.
 4. Process text using the pipeline.
 
 Example code:
 
 ```python
 import spacy
-from gliner_spacy.pipeline import GlinerSpacy
 
 nlp = spacy.blank("en")
 nlp.add_pipe("gliner_spacy")
 text = "This is a text about Bill Gates and Microsoft."
 doc = nlp(text)
 
 for ent in doc.ents:
@@ -48,34 +47,38 @@
 Microsoft organization
 ```
 
 ## Example with Custom Configs
 
 ```python
 import spacy
-from gliner_spacy.pipeline import GlinerSpacy
 
 custom_spacy_config = { "gliner_model": "urchade/gliner_multi",
                             "chunk_size": 250,
                             "labels": ["people","company","punctuation"],
                             "style": "ent"}
 nlp = spacy.blank("en")
 nlp.add_pipe("gliner_spacy", config=custom_spacy_config)
 
 text = "This is a text about Bill Gates and Microsoft."
 doc = nlp(text)
 
 for ent in doc.ents:
-    print(ent.text, ent.label_)
+    print(ent.text, ent.label_, ent._.score)
+
+#Output
+# Bill Gates person 0.9967108964920044
+# Tom person 0.9612326622009277
+# Microsoft organization 0.9966742992401123    
 ```
 
 ## Configuration
 The default configuration of the wrapper can be modified according to your requirements. The configurable parameters are:
 - `gliner_model`: The GLiNER model to be used.
 - `chunk_size`: Size of the text chunk to be processed at once.
 - `labels`: The entity labels to be recognized.
 - `style`: The style of output for the entities (either 'ent' or 'span').
 - `threshold`: The threshold of the GliNER model (controls the degree to which a hit is considered an entity)
-- `map_location`: The device on which to run the model: `cpu` or `gpu`
+- `map_location`: The device on which to run the model: `cpu` or `cuda`
 
 ## Contributing
 Contributions to this project are welcome. Please ensure that your code adheres to the project's coding standards and include tests for new features.
```

### Comparing `gliner-spacy-0.0.7/gliner_spacy/pipeline.py` & `gliner-spacy-0.0.8/gliner_spacy/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,16 +80,16 @@
 
         return doc
 
     def _create_entity_spans(self, doc, all_entities):
         spans = []
         for ent in all_entities:
             span = doc.char_span(ent['start'], ent['end'], label=ent['label'])
-            span._.score = ent['score']
             if span:  # Only add span if it is valid
+                span._.score = ent['score']
                 spans.append(span)
         if self.style == "span":
             doc.spans["sc"] = spans
         else:
             doc.ents = spans
         return doc
```

### Comparing `gliner-spacy-0.0.7/gliner_spacy.egg-info/PKG-INFO` & `gliner-spacy-0.0.8/gliner_spacy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gliner-spacy
-Version: 0.0.7
+Version: 0.0.8
 Summary: A SpaCy wrapper for the GLiNER model for enhanced Named Entity Recognition capabilities
 Home-page: https://github.com/theirstory/gliner-spacy
 Author: William J. B. Mattingly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -35,24 +35,23 @@
 ```bash
 pip install gliner-spacy
 ```
 
 ## Usage
 To use this wrapper in your SpaCy pipeline, follow these steps:
 
-1. Import SpaCy and the GLiNER SpaCy wrapper.
+1. Import SpaCy.
 2. Create a SpaCy `Language` instance.
 3. Add the `gliner_spacy` component to the SpaCy pipeline.
 4. Process text using the pipeline.
 
 Example code:
 
 ```python
 import spacy
-from gliner_spacy.pipeline import GlinerSpacy
 
 nlp = spacy.blank("en")
 nlp.add_pipe("gliner_spacy")
 text = "This is a text about Bill Gates and Microsoft."
 doc = nlp(text)
 
 for ent in doc.ents:
@@ -66,34 +65,38 @@
 Microsoft organization
 ```
 
 ## Example with Custom Configs
 
 ```python
 import spacy
-from gliner_spacy.pipeline import GlinerSpacy
 
 custom_spacy_config = { "gliner_model": "urchade/gliner_multi",
                             "chunk_size": 250,
                             "labels": ["people","company","punctuation"],
                             "style": "ent"}
 nlp = spacy.blank("en")
 nlp.add_pipe("gliner_spacy", config=custom_spacy_config)
 
 text = "This is a text about Bill Gates and Microsoft."
 doc = nlp(text)
 
 for ent in doc.ents:
-    print(ent.text, ent.label_)
+    print(ent.text, ent.label_, ent._.score)
+
+#Output
+# Bill Gates person 0.9967108964920044
+# Tom person 0.9612326622009277
+# Microsoft organization 0.9966742992401123    
 ```
 
 ## Configuration
 The default configuration of the wrapper can be modified according to your requirements. The configurable parameters are:
 - `gliner_model`: The GLiNER model to be used.
 - `chunk_size`: Size of the text chunk to be processed at once.
 - `labels`: The entity labels to be recognized.
 - `style`: The style of output for the entities (either 'ent' or 'span').
 - `threshold`: The threshold of the GliNER model (controls the degree to which a hit is considered an entity)
-- `map_location`: The device on which to run the model: `cpu` or `gpu`
+- `map_location`: The device on which to run the model: `cpu` or `cuda`
 
 ## Contributing
 Contributions to this project are welcome. Please ensure that your code adheres to the project's coding standards and include tests for new features.
```

### Comparing `gliner-spacy-0.0.7/setup.py` & `gliner-spacy-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     version=about['__version__'],
     author='William J. B. Mattingly',
     description='A SpaCy wrapper for the GLiNER model for enhanced Named Entity Recognition capabilities',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/theirstory/gliner-spacy',
     packages=find_packages(),
+    entry_points={
+      "spacy_factories": ["gliner_spacy = gliner_spacy.pipeline:GlinerSpacy"],
+    },
     install_requires=[
         'spacy>=3.0.0',
         'gliner>=0.2.0',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',  
         'Intended Audience :: Developers',
```

