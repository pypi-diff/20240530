# Comparing `tmp/fuzzquery-24.5.26.tar.gz` & `tmp/fuzzquery-24.5.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzquery-24.5.26.tar", last modified: Sat May 25 02:28:19 2024, max compression
+gzip compressed data, was "fuzzquery-24.5.28.tar", last modified: Thu May 30 07:19:44 2024, max compression
```

## Comparing `fuzzquery-24.5.26.tar` & `fuzzquery-24.5.28.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 02:28:19.899740 fuzzquery-24.5.26/
--rw-rw-rw-   0        0        0     1090 2024-05-16 01:40:27.000000 fuzzquery-24.5.26/LICENSE
--rw-rw-rw-   0        0        0     3667 2024-05-25 02:28:19.899740 fuzzquery-24.5.26/PKG-INFO
--rw-rw-rw-   0        0        0     5017 2024-05-23 10:16:41.000000 fuzzquery-24.5.26/README.md
--rw-rw-rw-   0        0        0     2706 2024-05-25 02:24:38.000000 fuzzquery-24.5.26/README.rst
--rw-rw-rw-   0        0        0     1040 2024-05-25 02:26:57.000000 fuzzquery-24.5.26/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-25 02:28:19.915363 fuzzquery-24.5.26/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-25 02:28:19.665489 fuzzquery-24.5.26/src/
-drwxrwxrwx   0        0        0        0 2024-05-25 02:28:19.805985 fuzzquery-24.5.26/src/fuzzquery/
--rw-rw-rw-   0        0        0     5266 2024-05-23 08:45:12.000000 fuzzquery-24.5.26/src/fuzzquery/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 02:28:19.899740 fuzzquery-24.5.26/src/fuzzquery.egg-info/
--rw-rw-rw-   0        0        0     3667 2024-05-25 02:28:19.000000 fuzzquery-24.5.26/src/fuzzquery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2024-05-25 02:28:19.000000 fuzzquery-24.5.26/src/fuzzquery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 02:28:19.000000 fuzzquery-24.5.26/src/fuzzquery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-25 02:28:19.000000 fuzzquery-24.5.26/src/fuzzquery.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-25 02:28:19.000000 fuzzquery-24.5.26/src/fuzzquery.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 07:19:44.226792 fuzzquery-24.5.28/
+-rw-rw-rw-   0        0        0     1090 2024-05-16 01:40:27.000000 fuzzquery-24.5.28/LICENSE
+-rw-rw-rw-   0        0        0       21 2024-05-29 19:00:24.000000 fuzzquery-24.5.28/MANIFEST.in
+-rw-rw-rw-   0        0        0     3604 2024-05-30 07:19:44.226792 fuzzquery-24.5.28/PKG-INFO
+-rw-rw-rw-   0        0        0     2676 2024-05-30 07:18:18.000000 fuzzquery-24.5.28/README.rst
+-rw-rw-rw-   0        0        0     1002 2024-05-29 22:08:20.000000 fuzzquery-24.5.28/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 07:19:44.226792 fuzzquery-24.5.28/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-30 07:19:44.164285 fuzzquery-24.5.28/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 07:19:44.195539 fuzzquery-24.5.28/src/fuzzquery/
+-rw-rw-rw-   0        0        0     4854 2024-05-29 19:24:26.000000 fuzzquery-24.5.28/src/fuzzquery/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:19:44.226792 fuzzquery-24.5.28/src/fuzzquery.egg-info/
+-rw-rw-rw-   0        0        0     3604 2024-05-30 07:19:44.000000 fuzzquery-24.5.28/src/fuzzquery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2024-05-30 07:19:44.000000 fuzzquery-24.5.28/src/fuzzquery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 07:19:44.000000 fuzzquery-24.5.28/src/fuzzquery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-30 07:19:44.000000 fuzzquery-24.5.28/src/fuzzquery.egg-info/top_level.txt
```

### Comparing `fuzzquery-24.5.26/LICENSE` & `fuzzquery-24.5.28/LICENSE`

 * *Files identical despite different names*

### Comparing `fuzzquery-24.5.26/PKG-INFO` & `fuzzquery-24.5.28/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzquery
-Version: 24.5.26
+Version: 24.5.28
 Summary: A lightweight package for fuzzy word/phrase searches in a body of text.
 Author-email: Oyster Shucker <onemadgypsy@gmail.com>
 Maintainer-email: Oyster Shucker <onemadgypsy@gmail.com>
 Project-URL: Homepage, https://github.com/OneMadGypsy/fuzzquery
 Project-URL: Issues, https://github.com/OneMadGypsy/fuzzquery/issues
 Project-URL: Documentation, https://fuzzquery.readthedocs.io
 Keywords: fuzzy,string,match,filter,regex
@@ -14,25 +14,24 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: regex>=2024.5.15
 
-fuzzquery 24.5.26
+fuzzquery 24.5.28
 =================
 
 **fuzzquery** is a lightweight package for fuzzy word/phrase searches in a body of text. Tokens are used to determine the number and type of approximations that can be made at a token’s position, within your query.
 
 Installation
 ------------
 
-To install ``fuzzquery`` and it's ``regex`` dependency, use the following command-line: 
+To install ``fuzzquery`` use the following command-line: 
 
 .. code-block:: console
 
   pip install fuzzquery
 
 Documentation
 -------------
@@ -52,22 +51,22 @@
 
   data = """ 
   I would classify music as one of my favorite hobbies. 
   I love classical music played by classy musicians for a classic musical. 
   Beethoven can not be out-classed, music-wise - a man of class, musically gifted.
   """
   query = 'class{4} music{5}'
-
-  print(f'\n{query.upper()}')
-  for span, match in fq.finditer(data, query, ci=True):
-      print(f'  {match}')
-
-  print(f'\n{query.upper()} with skip')
+  
+  print(f'\n{query.upper()} using skip')
   for span, match in fq.finditer(data, query, skip=('classify', ','), ci=True):
       print(f'  {match}')
+      
+  print(f'\n{query.upper()} no skip')
+  for span, match in fq.finditer(data, query, ci=True):
+      print(f'  {match}')
 
 **output:**
 
 .. code-block:: console
 
   CLASS{4} MUSIC{5}
     classify music
@@ -91,18 +90,19 @@
   
   data = """ 
   I headed homeward to meet with the Wardens. 
   When I arrived, I was greeted by a homely man that told me the homestead was awarded 5 million dollars.
   We intend to use some of the homage to create a homeless ward. 
   The first piece of furniture will be my late-friend Homer's wardrobe.
   """
+  
   queries = ('home{5}', 
              'home{4} ward{4}', 
-             '{1}ward{!2}{2}', 
-             'hom{5} {?} wa{!1}{5}')
+             '{1}ward{=2}{2}', 
+             'hom{6} {4w} wa{=1}{5}')
   
   for query, span, match in fq.iterall(data, queries, ci=True):
       if query: print(f'\n{query.upper()}')
       print(f'  {match}')
 
 **output:**
 
@@ -110,22 +110,22 @@
 
   HOME{5}
     homeward
     homely
     homestead
     homeless
     Homer's
-
+  
   HOME{4} WARD{4}
     homeless ward
     Homer's wardrobe
-
-  {1}WARD{!2}{2}
+  
+  {1}WARD{=2}{2}
     Wardens
     awarded
     wardrobe
-
-  HOM{5} {?} WA{!1}{5}
+  
+  HOM{6} {4W} WA{=1}{5}
     homeward to meet with the Wardens
-    homely man that told me the homestead was
+    homestead was
     homage to create a homeless ward
     Homer's wardrobe
```

### Comparing `fuzzquery-24.5.26/README.rst` & `fuzzquery-24.5.28/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-fuzzquery 24.5.26
+fuzzquery 24.5.28
 =================
 
 **fuzzquery** is a lightweight package for fuzzy word/phrase searches in a body of text. Tokens are used to determine the number and type of approximations that can be made at a token’s position, within your query.
 
 Installation
 ------------
 
-To install ``fuzzquery`` and it's ``regex`` dependency, use the following command-line: 
+To install ``fuzzquery`` use the following command-line: 
 
 .. code-block:: console
 
   pip install fuzzquery
 
 Documentation
 -------------
@@ -30,22 +30,22 @@
 
   data = """ 
   I would classify music as one of my favorite hobbies. 
   I love classical music played by classy musicians for a classic musical. 
   Beethoven can not be out-classed, music-wise - a man of class, musically gifted.
   """
   query = 'class{4} music{5}'
-
-  print(f'\n{query.upper()}')
-  for span, match in fq.finditer(data, query, ci=True):
-      print(f'  {match}')
-
-  print(f'\n{query.upper()} with skip')
+  
+  print(f'\n{query.upper()} using skip')
   for span, match in fq.finditer(data, query, skip=('classify', ','), ci=True):
       print(f'  {match}')
+      
+  print(f'\n{query.upper()} no skip')
+  for span, match in fq.finditer(data, query, ci=True):
+      print(f'  {match}')
 
 **output:**
 
 .. code-block:: console
 
   CLASS{4} MUSIC{5}
     classify music
@@ -69,18 +69,19 @@
   
   data = """ 
   I headed homeward to meet with the Wardens. 
   When I arrived, I was greeted by a homely man that told me the homestead was awarded 5 million dollars.
   We intend to use some of the homage to create a homeless ward. 
   The first piece of furniture will be my late-friend Homer's wardrobe.
   """
+  
   queries = ('home{5}', 
              'home{4} ward{4}', 
-             '{1}ward{!2}{2}', 
-             'hom{5} {?} wa{!1}{5}')
+             '{1}ward{=2}{2}', 
+             'hom{6} {4w} wa{=1}{5}')
   
   for query, span, match in fq.iterall(data, queries, ci=True):
       if query: print(f'\n{query.upper()}')
       print(f'  {match}')
 
 **output:**
 
@@ -88,22 +89,22 @@
 
   HOME{5}
     homeward
     homely
     homestead
     homeless
     Homer's
-
+  
   HOME{4} WARD{4}
     homeless ward
     Homer's wardrobe
-
-  {1}WARD{!2}{2}
+  
+  {1}WARD{=2}{2}
     Wardens
     awarded
     wardrobe
-
-  HOM{5} {?} WA{!1}{5}
+  
+  HOM{6} {4W} WA{=1}{5}
     homeward to meet with the Wardens
-    homely man that told me the homestead was
+    homestead was
     homage to create a homeless ward
     Homer's wardrobe
```

### Comparing `fuzzquery-24.5.26/pyproject.toml` & `fuzzquery-24.5.28/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fuzzquery"
-version = "24.5.26"
+version = "24.5.28"
 description = "A lightweight package for fuzzy word/phrase searches in a body of text."
-dependencies = ["regex>=2024.5.15",]
 keywords = ["fuzzy", "string", "match", "filter", "regex"]
 authors = [{ name="Oyster Shucker", email="onemadgypsy@gmail.com" },]
 maintainers = [{ name="Oyster Shucker", email="onemadgypsy@gmail.com" },]
 readme = "README.rst"
 requires-python = ">=3.8"
 classifiers = [
     "Intended Audience :: Developers",
```

### Comparing `fuzzquery-24.5.26/src/fuzzquery/__init__.py` & `fuzzquery-24.5.28/src/fuzzquery/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,80 @@
 """A lightweight package for fuzzy word/phrase searches in a body of text, using a very simple token system.
 
 project: https://pypi.org/project/fuzzquery/
 
-version: 24.5.22
+version: 24.5.28
 
 author: OysterShucker
 
 tokens:
- - "{x}"  : from 0 to x non-whitespace characters
- - "{!x}" : exactly x non-whitespace characters
- - "{?}"  : 0 or more unknown words
+ tokens have up to 3 parts:
+ - "x" = a number of characters or words to find. this number by default is considered a range: 0 to `x`
+ - "=" = exactly `x`, instead of a range
+ - "w" = signifies the token should match words
+ 
+token examples:
+ - "{5}"  : from 0 to 5 non-whitespace characters
+ - "{=3}" : exactly 3 non-whitespace characters
+ - "{5w}" : 0 to 5 words
+ - "{=3w}": exactly 3 words
     
 query examples:
- - "home{5}"       : home, homer, homely, homeward, homestead
- - "bomb{!2}"      : bomber, bombed
- - "bomb{!2}{3}"   : bomber, bombed, bombers, bombastic
- - "thou {?} kill" : thou shalt not kill
- - "{2}ward{!2}"   : warden, awarded, rewarded
- * "{4}{!3}-{!4}"  : 504-525-5555, 867-5309, more-or-less
+ - "home{5}"         : home, homer, homely, homeward, homestead
+ - "bomb{=2}"        : bomber, bombed
+ - "bomb{=2}{3}"     : bomber, bombed, bombers, bombastic
+ - "thou {=2w} kill" : thou shalt not kill
+ - "{2}ward{=2}"     : warden, awarded, rewarded
+ * "{4}{=3}-{=4}"    : 504-525-5555, 867-5309, more-or-less
  
  * searches this broad are bound to return some unwanted results
 """
-import regex
+import re
 from typing import Iterator
 
 __all__ = 'finditer', 'findany', 'iterall'
 
-REPL  = '`'                                  # character to represent substitution and deletion points
-TOKEN = regex.compile(r'\{(!{0,1}\d+|\?)\}') # for splitting on token guts
-FLAGS = regex.V1, regex.V1|regex.I           # case-sensitive, case-insensitive
-
-# https://github.com/mrabarnett/mrab-regex?tab=readme-ov-file#approximate-fuzzy-matching-hg-issue-12-hg-issue-41-hg-issue-109
-FORMAT = {
-    '.':r'{{{over}i+1d+1s<={limit}:\S}}',    # allowed range of mixed substitutions and deletions
-    '!':r'{{{limit}<=s<={limit}:\S}}'   ,    # strict amount of substitutions only
-    '?':r'([\w\W]+?(?=\s))*?'           ,}   # 0 or more unknown words 
-    
+FLAGS = None, re.I
+TOKEN = re.compile(r'(\{={0,1}\d+[cw]{0,1}\})')
+
+FORMATS = {
+    'char' : r'(?:\S){{{start},{stop}}}',
+    'word' : r'(?:\S+?(?:\s+?|$)){{{start},{stop}}}',
+}
+
 # convert query to expression
 def __expr(query:str, group:bool=True) -> str:
 
     # convert term segment to expression
-    def subexpr(segment:str) -> str:
-        
-        # assume this is a token and get alleged integer range
-        limit = int(''.join(filter(str.isdigit, segment)) or 0)
-        
-        # alias some facts
-        d, t  = segment.isdigit(), segment[0]
-        
-        # if range or strict get replacement characters group
-        expr  = ('', fr'({REPL * limit})')[d | (t == '!')] 
-        
-        # append respective value and format compatible results with limits
-        expr += FORMAT.get((t, '.')[d], regex.escape(segment)).format(over=limit+1, limit=limit)
-        
-        return expr
+    def subexpr(segment:str, _start:int=0, _stop:int=0, _type:str='explicit') -> str:
+        if TOKEN.fullmatch(segment) is not None:
+            _type  = ('char', 'word')['w' in segment]
+            _stop  = int(''.join(filter(str.isdigit, segment)) or 0)
+            _start = _stop * ('=' in segment)
+
+        return FORMATS.get(_type, re.escape(segment)).format(start=_start, stop=_stop)
     
     # term segments
     segmap = filter(None, map(TOKEN.split, query.split(' ')))
     
     # generator of terms from processed term segments
     terms = (r''.join(map(subexpr, filter(None, segments))) for segments in segmap)
     
     # join terms with conditional spacing
-    expr  = r'((?<=\s)|\s)+?'.join(terms)
+    expr  = r'(?:(?<=\s)|\s)+?'.join(terms)
     
     # create final expression
     return f'{"("*group}{expr}{")"*group}'
    
 # execute final expression on text
 def __exec(expr:str, text:str, skip:None|list|tuple|set=None, ci:bool=False) -> Iterator:
     skip = skip or []
     
-    for match in regex.finditer(expr, text, flags=FLAGS[ci]):
-        result = match['result']
+    for match in re.finditer(expr, text, flags=FLAGS[ci]):
+        result = match.group('result')
         
         # determine if result should be skipped
         for item in skip:
             if item in result: break
         else:
             yield match.span(), result
 
@@ -94,15 +91,15 @@
        words and/or characters that trigger a skip when found in a result
          
      ** ci     : bool, optional
        case insensitive matching  
          
      return tuple of query results (`span`, `results`)
     """
-    expr = fr'\m(?P<result>{__expr(query, False)})\M'
+    expr = fr'\b(?P<result>{__expr(query, False)})\b'
     
     for span, result in __exec(expr, text, **kwargs):
         yield span, result
           
 def findany(text:str, queries:list|tuple|set, **kwargs) -> Iterator:
     """Format and OR queries into a singular expression and yield matches
     
@@ -117,15 +114,15 @@
        
      ** ci     : bool, optional
        case insensitive matching  
      
      return tuple of query results (`span`, `results`)
     """
     expr = r'|'.join(map(__expr, queries))
-    expr = fr'\m(?P<result>{expr})\M'
+    expr = fr'\b(?P<result>{expr})\b'
     
     for span, result in __exec(expr, text, **kwargs):
         yield span, result
 
 def iterall(text:str, queries:list|tuple|set, **kwargs) -> Iterator: 
     """Yield from multiple consecutive queries
```

### Comparing `fuzzquery-24.5.26/src/fuzzquery.egg-info/PKG-INFO` & `fuzzquery-24.5.28/src/fuzzquery.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzquery
-Version: 24.5.26
+Version: 24.5.28
 Summary: A lightweight package for fuzzy word/phrase searches in a body of text.
 Author-email: Oyster Shucker <onemadgypsy@gmail.com>
 Maintainer-email: Oyster Shucker <onemadgypsy@gmail.com>
 Project-URL: Homepage, https://github.com/OneMadGypsy/fuzzquery
 Project-URL: Issues, https://github.com/OneMadGypsy/fuzzquery/issues
 Project-URL: Documentation, https://fuzzquery.readthedocs.io
 Keywords: fuzzy,string,match,filter,regex
@@ -14,25 +14,24 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: regex>=2024.5.15
 
-fuzzquery 24.5.26
+fuzzquery 24.5.28
 =================
 
 **fuzzquery** is a lightweight package for fuzzy word/phrase searches in a body of text. Tokens are used to determine the number and type of approximations that can be made at a token’s position, within your query.
 
 Installation
 ------------
 
-To install ``fuzzquery`` and it's ``regex`` dependency, use the following command-line: 
+To install ``fuzzquery`` use the following command-line: 
 
 .. code-block:: console
 
   pip install fuzzquery
 
 Documentation
 -------------
@@ -52,22 +51,22 @@
 
   data = """ 
   I would classify music as one of my favorite hobbies. 
   I love classical music played by classy musicians for a classic musical. 
   Beethoven can not be out-classed, music-wise - a man of class, musically gifted.
   """
   query = 'class{4} music{5}'
-
-  print(f'\n{query.upper()}')
-  for span, match in fq.finditer(data, query, ci=True):
-      print(f'  {match}')
-
-  print(f'\n{query.upper()} with skip')
+  
+  print(f'\n{query.upper()} using skip')
   for span, match in fq.finditer(data, query, skip=('classify', ','), ci=True):
       print(f'  {match}')
+      
+  print(f'\n{query.upper()} no skip')
+  for span, match in fq.finditer(data, query, ci=True):
+      print(f'  {match}')
 
 **output:**
 
 .. code-block:: console
 
   CLASS{4} MUSIC{5}
     classify music
@@ -91,18 +90,19 @@
   
   data = """ 
   I headed homeward to meet with the Wardens. 
   When I arrived, I was greeted by a homely man that told me the homestead was awarded 5 million dollars.
   We intend to use some of the homage to create a homeless ward. 
   The first piece of furniture will be my late-friend Homer's wardrobe.
   """
+  
   queries = ('home{5}', 
              'home{4} ward{4}', 
-             '{1}ward{!2}{2}', 
-             'hom{5} {?} wa{!1}{5}')
+             '{1}ward{=2}{2}', 
+             'hom{6} {4w} wa{=1}{5}')
   
   for query, span, match in fq.iterall(data, queries, ci=True):
       if query: print(f'\n{query.upper()}')
       print(f'  {match}')
 
 **output:**
 
@@ -110,22 +110,22 @@
 
   HOME{5}
     homeward
     homely
     homestead
     homeless
     Homer's
-
+  
   HOME{4} WARD{4}
     homeless ward
     Homer's wardrobe
-
-  {1}WARD{!2}{2}
+  
+  {1}WARD{=2}{2}
     Wardens
     awarded
     wardrobe
-
-  HOM{5} {?} WA{!1}{5}
+  
+  HOM{6} {4W} WA{=1}{5}
     homeward to meet with the Wardens
-    homely man that told me the homestead was
+    homestead was
     homage to create a homeless ward
     Homer's wardrobe
```

