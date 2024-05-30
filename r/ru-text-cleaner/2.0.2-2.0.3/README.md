# Comparing `tmp/ru_text_cleaner-2.0.2.tar.gz` & `tmp/ru_text_cleaner-2.0.3.tar.gz`

## Comparing `ru_text_cleaner-2.0.2.tar` & `ru_text_cleaner-2.0.3.tar`

### file list

```diff
@@ -1,33 +1,24 @@
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/requirements.txt
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/.idea/TextCleaner.iml
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0    11204 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/__init__.py
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/TextCleaner.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/__init__.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_clean_stopwords.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_emoji_cleaner.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_html_cleaner.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_punctuation_cleaner.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_spaces_cleaner.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_to_lower.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_to_morpheme.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/TextCleaner.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/__init__.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/_clean_stopwords.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/_emoji_cleaner.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/_html_cleaner.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/_punctuation_cleaner.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/_spaces_cleaner.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/_to_lower.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/src/ru_text_cleaner/tensor_cleaner/_to_morpheme.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/LICENSE
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/README.md
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/requirements.txt
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/.idea/TextCleaner.iml
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0    12063 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/.idea/workspace.xml
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/src/ru_text_cleaner/__init__.py
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/src/ru_text_cleaner/simple_cleaner/TextCleaner.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/src/ru_text_cleaner/simple_cleaner/__init__.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/src/ru_text_cleaner/simple_cleaner/_clean_stopwords.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/src/ru_text_cleaner/simple_cleaner/_emoji_cleaner.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/src/ru_text_cleaner/simple_cleaner/_html_cleaner.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/src/ru_text_cleaner/simple_cleaner/_punctuation_cleaner.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/src/ru_text_cleaner/simple_cleaner/_spaces_cleaner.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/src/ru_text_cleaner/simple_cleaner/_to_lower.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/src/ru_text_cleaner/simple_cleaner/_to_morpheme.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/LICENSE
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/README.md
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.3/PKG-INFO
```

### Comparing `ru_text_cleaner-2.0.2/.idea/workspace.xml` & `ru_text_cleaner-2.0.3/.idea/workspace.xml`

 * *Files 25% similar despite different names*

#### Comparing `ru_text_cleaner-2.0.2/.idea/workspace.xml` & `ru_text_cleaner-2.0.3/.idea/workspace.xml`

```diff
@@ -1,14 +1,18 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="1e7c1d4a-6db9-4bec-b8db-c44acb60056e" name="Changes" comment="Adapted for tensforflow strings"/>
+    <list default="true" id="1e7c1d4a-6db9-4bec-b8db-c44acb60056e" name="Changes" comment="Adapted for tensforflow strings">
+      <change beforePath="$PROJECT_DIR$/src/ru_text_cleaner/simple_cleaner/_punctuation_cleaner.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/ru_text_cleaner/simple_cleaner/_punctuation_cleaner.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/ru_text_cleaner/tensor_cleaner/TextCleaner.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/ru_text_cleaner/tensor_cleaner/TextCleaner.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/ru_text_cleaner/tensor_cleaner/_punctuation_cleaner.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/ru_text_cleaner/tensor_cleaner/_punctuation_cleaner.py" afterDir="false"/>
+    </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
@@ -36,28 +40,28 @@
   &quot;associatedIndex&quot;: 1
 }</component>
   <component name="ProjectId" id="2gabPsOhyrp8dGKBt8dT3UO6PX0"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent"><![CDATA[{
-  "keyToString": {
-    "ASKED_ADD_EXTERNAL_FILES": "true",
-    "ASKED_SHARE_PROJECT_CONFIGURATION_FILES": "true",
-    "Python.TextCleaner.executor": "Run",
-    "Python.__init__.executor": "Run",
-    "Python._clean_stopwords.executor": "Run",
-    "Python._spaces_cleaner.executor": "Run",
-    "Python.test.executor": "Run",
-    "RunOnceActivity.ShowReadmeOnStart": "true",
-    "git-widget-placeholder": "master",
-    "last_opened_file_path": "/Users/artemgafarov/PycharmProjects/TextCleaner/src/ru_text_cleaner/tensor_cleaner"
+  <component name="PropertiesComponent">{
+  &quot;keyToString&quot;: {
+    &quot;ASKED_ADD_EXTERNAL_FILES&quot;: &quot;true&quot;,
+    &quot;ASKED_SHARE_PROJECT_CONFIGURATION_FILES&quot;: &quot;true&quot;,
+    &quot;Python.TextCleaner.executor&quot;: &quot;Run&quot;,
+    &quot;Python.__init__.executor&quot;: &quot;Run&quot;,
+    &quot;Python._clean_stopwords.executor&quot;: &quot;Run&quot;,
+    &quot;Python._spaces_cleaner.executor&quot;: &quot;Run&quot;,
+    &quot;Python.test.executor&quot;: &quot;Run&quot;,
+    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
+    &quot;git-widget-placeholder&quot;: &quot;master&quot;,
+    &quot;last_opened_file_path&quot;: &quot;/Users/artemgafarov/PycharmProjects/TextCleaner/src/ru_text_cleaner/tensor_cleaner&quot;
   }
-}]]></component>
+}</component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/src/ru_text_cleaner/tensor_cleaner"/>
     </key>
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/src/ru_text_cleaner/simple_cleaner"/>
       <recent name="$PROJECT_DIR$/src"/>
```

### Comparing `ru_text_cleaner-2.0.2/.idea/inspectionProfiles/Project_Default.xml` & `ru_text_cleaner-2.0.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/TextCleaner.py` & `ru_text_cleaner-2.0.3/src/ru_text_cleaner/simple_cleaner/TextCleaner.py`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_clean_stopwords.py` & `ru_text_cleaner-2.0.3/src/ru_text_cleaner/simple_cleaner/_clean_stopwords.py`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_punctuation_cleaner.py` & `ru_text_cleaner-2.0.3/src/ru_text_cleaner/simple_cleaner/_punctuation_cleaner.py`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_spaces_cleaner.py` & `ru_text_cleaner-2.0.3/src/ru_text_cleaner/simple_cleaner/_spaces_cleaner.py`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-2.0.2/src/ru_text_cleaner/simple_cleaner/_to_morpheme.py` & `ru_text_cleaner-2.0.3/src/ru_text_cleaner/simple_cleaner/_to_morpheme.py`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-2.0.2/LICENSE` & `ru_text_cleaner-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-2.0.2/README.md` & `ru_text_cleaner-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-2.0.2/pyproject.toml` & `ru_text_cleaner-2.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['pymorphy2>=0.9.1', 'nltk>=3.8.1', 'hatchling', 'emoji>=2.11.1', 'tensorflow>=2.16.1']
 build-backend = "hatchling.build"
 
 [project]
 name = "ru-text-cleaner"
-version = "2.0.2"
+version = "2.0.3"
 authors = [
     { name="Vildan Nasyrov", email="" },
     { name="Artem Gafarov", email="a.m.gafarov@ya.ru" },
 ]
 description = "Cleans russian text and preparing for NLP"
 requires-python = ">=3.10.4"
 readme = "README.md"
```

### Comparing `ru_text_cleaner-2.0.2/PKG-INFO` & `ru_text_cleaner-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ru-text-cleaner
-Version: 2.0.2
+Version: 2.0.3
 Summary: Cleans russian text and preparing for NLP
 Project-URL: Homepage, https://github.com/rvneural/TextCleaner
 Project-URL: Issues, https://github.com/rvneural/TextCleaner/issues
 Author: Vildan Nasyrov
 Author-email: Artem Gafarov <a.m.gafarov@ya.ru>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

