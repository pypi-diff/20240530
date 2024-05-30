# Comparing `tmp/elifecrossref-0.8.0.tar.gz` & `tmp/elifecrossref-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/elifecrossref-0.8.0.tar", last modified: Tue Oct 26 22:46:30 2021, max compression
+gzip compressed data, was "dist/elifecrossref-0.9.0.tar", last modified: Tue Nov  2 23:36:42 2021, max compression
```

## Comparing `elifecrossref-0.8.0.tar` & `elifecrossref-0.9.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 jenkins   (1002) jenkins    (999)        0 2021-10-26 22:46:30.000000 elifecrossref-0.8.0/
--rw-r--r--   0 jenkins   (1002) jenkins    (999)       38 2021-10-26 22:46:30.000000 elifecrossref-0.8.0/setup.cfg
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     5154 2021-10-26 22:46:30.000000 elifecrossref-0.8.0/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     4606 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/README.rst
-drwxr-xr-x   0 jenkins   (1002) jenkins    (999)        0 2021-10-26 22:46:30.000000 elifecrossref-0.8.0/elifecrossref.egg-info/
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     5154 2021-10-26 22:46:30.000000 elifecrossref-0.8.0/elifecrossref.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (999)       56 2021-10-26 22:46:30.000000 elifecrossref-0.8.0/elifecrossref.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (999)       14 2021-10-26 22:46:30.000000 elifecrossref-0.8.0/elifecrossref.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (999)        1 2021-10-26 22:46:30.000000 elifecrossref-0.8.0/elifecrossref.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     1006 2021-10-26 22:46:30.000000 elifecrossref-0.8.0/elifecrossref.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (999)       24 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      891 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/setup.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     1071 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/LICENSE
--rw-r--r--   0 jenkins   (1002) jenkins    (999)       92 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/requirements.txt
-drwxr-xr-x   0 jenkins   (1002) jenkins    (999)        0 2021-10-26 22:46:30.000000 elifecrossref-0.8.0/elifecrossref/
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     6594 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/generate.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     1598 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/dates.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     1908 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/conf.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     2551 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/clinical_trials.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     2326 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/related.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      885 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/head.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     3261 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/tags.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      769 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/doi.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     2517 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/collection.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     1710 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/journal.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     5846 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/crossmark.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     6840 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/abstract.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     1263 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/access_indicators.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     3324 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/peer_review.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      833 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/utils.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     3514 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/contributor.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      753 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/preprint.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      811 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/body.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     2301 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/dataset.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      685 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/title.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)       22 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/__init__.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      763 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/elife.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     1665 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/funding.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     8881 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/citation.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      777 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/pending_publication.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     3591 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/component.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     1823 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/mime_type.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     1621 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/resource_url.py
--rw-r--r--   0 jenkins   (1002) jenkins    (999)     3484 2021-10-26 22:46:01.000000 elifecrossref-0.8.0/elifecrossref/journal_article.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (999)        0 2021-11-02 23:36:42.000000 elifecrossref-0.9.0/
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)       38 2021-11-02 23:36:42.000000 elifecrossref-0.9.0/setup.cfg
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     5154 2021-11-02 23:36:42.000000 elifecrossref-0.9.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     4606 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/README.rst
+drwxr-xr-x   0 jenkins   (1002) jenkins    (999)        0 2021-11-02 23:36:42.000000 elifecrossref-0.9.0/elifecrossref.egg-info/
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     5154 2021-11-02 23:36:42.000000 elifecrossref-0.9.0/elifecrossref.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)       56 2021-11-02 23:36:42.000000 elifecrossref-0.9.0/elifecrossref.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)       14 2021-11-02 23:36:42.000000 elifecrossref-0.9.0/elifecrossref.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)        1 2021-11-02 23:36:42.000000 elifecrossref-0.9.0/elifecrossref.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     1006 2021-11-02 23:36:42.000000 elifecrossref-0.9.0/elifecrossref.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)       24 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)      891 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/setup.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     1071 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/LICENSE
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)       92 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/requirements.txt
+drwxr-xr-x   0 jenkins   (1002) jenkins    (999)        0 2021-11-02 23:36:42.000000 elifecrossref-0.9.0/elifecrossref/
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     6594 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/generate.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     1598 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/dates.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     1908 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/conf.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     2551 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/clinical_trials.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     2326 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/related.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)      885 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/head.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     3261 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/tags.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)      769 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/doi.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     2517 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/collection.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     1710 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/journal.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     5846 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/crossmark.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     6840 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/abstract.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     1263 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/access_indicators.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     3324 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/peer_review.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)      833 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/utils.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     3914 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/contributor.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)      753 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/preprint.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)      811 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/body.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     2301 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/dataset.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)      685 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/title.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)       22 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/__init__.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)      763 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/elife.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     1665 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/funding.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     8881 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/citation.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)      777 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/pending_publication.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     3591 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/component.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     1823 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/mime_type.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     1621 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/resource_url.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (999)     3484 2021-11-02 23:36:14.000000 elifecrossref-0.9.0/elifecrossref/journal_article.py
```

### Comparing `elifecrossref-0.8.0/PKG-INFO` & `elifecrossref-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elifecrossref
-Version: 0.8.0
+Version: 0.9.0
 Summary: eLife Crossref deposit of journal articles.
 Home-page: https://github.com/elifesciences/elife-crossref-xml-generation
 Maintainer: eLife Sciences Publications Ltd.
 Maintainer-email: py@elifesciences.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `elifecrossref-0.8.0/README.rst` & `elifecrossref-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref.egg-info/PKG-INFO` & `elifecrossref-0.9.0/elifecrossref.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elifecrossref
-Version: 0.8.0
+Version: 0.9.0
 Summary: eLife Crossref deposit of journal articles.
 Home-page: https://github.com/elifesciences/elife-crossref-xml-generation
 Maintainer: eLife Sciences Publications Ltd.
 Maintainer-email: py@elifesciences.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `elifecrossref-0.8.0/elifecrossref.egg-info/SOURCES.txt` & `elifecrossref-0.9.0/elifecrossref.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/setup.py` & `elifecrossref-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/LICENSE` & `elifecrossref-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/generate.py` & `elifecrossref-0.9.0/elifecrossref/generate.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/dates.py` & `elifecrossref-0.9.0/elifecrossref/dates.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/conf.py` & `elifecrossref-0.9.0/elifecrossref/conf.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/clinical_trials.py` & `elifecrossref-0.9.0/elifecrossref/clinical_trials.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/related.py` & `elifecrossref-0.9.0/elifecrossref/related.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/head.py` & `elifecrossref-0.9.0/elifecrossref/head.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/tags.py` & `elifecrossref-0.9.0/elifecrossref/tags.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/doi.py` & `elifecrossref-0.9.0/elifecrossref/doi.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/collection.py` & `elifecrossref-0.9.0/elifecrossref/collection.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/journal.py` & `elifecrossref-0.9.0/elifecrossref/journal.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/crossmark.py` & `elifecrossref-0.9.0/elifecrossref/crossmark.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/abstract.py` & `elifecrossref-0.9.0/elifecrossref/abstract.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/access_indicators.py` & `elifecrossref-0.9.0/elifecrossref/access_indicators.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/peer_review.py` & `elifecrossref-0.9.0/elifecrossref/peer_review.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/utils.py` & `elifecrossref-0.9.0/elifecrossref/utils.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/contributor.py` & `elifecrossref-0.9.0/elifecrossref/contributor.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,19 +18,29 @@
 def set_contributors(parent, contributors):
     # If contrib_type is None, all contributors will be added regardless of their type
     contributors_tag = SubElement(parent, "contributors")
 
     # Ready to add to XML
     # Use the natural list order of contributors when setting the first author
     sequence = "first"
+    prev_equal_contrib = None
     for contributor in contributors:
+        if (sequence == "first" and prev_equal_contrib is False) or (
+            sequence == "first"
+            and prev_equal_contrib is True
+            and not contributor.equal_contrib
+        ):
+            # Reset sequence value unless the first contributor and
+            # next contributor is also equal_contrib
+            sequence = "additional"
+
         set_contributor(contributors_tag, contributor, sequence)
 
-        # Reset sequence value after the first sucessful loop
-        sequence = "additional"
+        # set value for the next loop interation
+        prev_equal_contrib = contributor.equal_contrib
 
 
 def set_contributor(parent, contributor, sequence):
     """add tags for a contributor to the parent tag"""
     if contributor.contrib_type == "on-behalf-of":
         contributor_role = "author"
     else:
```

### Comparing `elifecrossref-0.8.0/elifecrossref/preprint.py` & `elifecrossref-0.9.0/elifecrossref/preprint.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/body.py` & `elifecrossref-0.9.0/elifecrossref/body.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/dataset.py` & `elifecrossref-0.9.0/elifecrossref/dataset.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/title.py` & `elifecrossref-0.9.0/elifecrossref/title.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/elife.py` & `elifecrossref-0.9.0/elifecrossref/elife.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/funding.py` & `elifecrossref-0.9.0/elifecrossref/funding.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/citation.py` & `elifecrossref-0.9.0/elifecrossref/citation.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/pending_publication.py` & `elifecrossref-0.9.0/elifecrossref/pending_publication.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/component.py` & `elifecrossref-0.9.0/elifecrossref/component.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/mime_type.py` & `elifecrossref-0.9.0/elifecrossref/mime_type.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/resource_url.py` & `elifecrossref-0.9.0/elifecrossref/resource_url.py`

 * *Files identical despite different names*

### Comparing `elifecrossref-0.8.0/elifecrossref/journal_article.py` & `elifecrossref-0.9.0/elifecrossref/journal_article.py`

 * *Files identical despite different names*

