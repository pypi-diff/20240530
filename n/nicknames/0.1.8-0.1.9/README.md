# Comparing `tmp/nicknames-0.1.8.tar.gz` & `tmp/nicknames-0.1.9.tar.gz`

## Comparing `nicknames-0.1.8.tar` & `nicknames-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 nicknames-0.1.8/test_package.py
--rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 nicknames-0.1.8/src/nicknames/__init__.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 nicknames-0.1.8/src/nicknames/_compat.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nicknames-0.1.8/src/nicknames/_version.py
--rw-r--r--   0        0        0    25032 2020-02-02 00:00:00.000000 nicknames-0.1.8/src/nicknames/names.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nicknames-0.1.8/src/nicknames/py.typed
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nicknames-0.1.8/.gitignore
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 nicknames-0.1.8/hatch_build.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 nicknames-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 nicknames-0.1.8/../README.md
--rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 nicknames-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 nicknames-0.1.9/test_package.py
+-rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 nicknames-0.1.9/src/nicknames/__init__.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 nicknames-0.1.9/src/nicknames/_compat.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nicknames-0.1.9/src/nicknames/_version.py
+-rw-r--r--   0        0        0    25132 2020-02-02 00:00:00.000000 nicknames-0.1.9/src/nicknames/names.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nicknames-0.1.9/src/nicknames/py.typed
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nicknames-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 nicknames-0.1.9/hatch_build.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 nicknames-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 nicknames-0.1.9/../README.md
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 nicknames-0.1.9/PKG-INFO
```

### Comparing `nicknames-0.1.8/test_package.py` & `nicknames-0.1.9/test_package.py`

 * *Files identical despite different names*

### Comparing `nicknames-0.1.8/src/nicknames/__init__.py` & `nicknames-0.1.9/src/nicknames/__init__.py`

 * *Files identical despite different names*

### Comparing `nicknames-0.1.8/src/nicknames/_compat.py` & `nicknames-0.1.9/src/nicknames/_compat.py`

 * *Files identical despite different names*

### Comparing `nicknames-0.1.8/src/nicknames/names.csv` & `nicknames-0.1.9/src/nicknames/names.csv`

 * *Files 3% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 ambrose,brose
 amelia,amy,mel,millie,emily
 amos,moses
 anastasia,ana,stacy
 anderson,andy
 andre,drea
 andrea,drea,rea,andrew,andi,andy
-andrew,andy,drew
+andrew,andy,drew,randy
 andriane,ada,adri,rienne
 angela,angel,angie
 angelica,angie,angel,angelika,angelique
 angelina,angel,angie,lina
 ann,annie,nan
 anna,anne,ann,annie,nan
 anne,annie,ann,nan
@@ -151,14 +151,15 @@
 benjamin,benjy,jamie,bennie,ben,benny
 benjy,benjamin
 bernard,barney,bernie,berney,berny
 berney,bernie
 bert,bertie,bob,bobby
 bertha,bert,birdie,bertie
 bertram,bert
+bertrand,randy
 bess,bessie
 beth,betsy,betty,elizabeth
 bethena,beth,thaney
 beverly,bev
 bezaleel,zeely
 biddie,biddy
 bill,william,billy,robert,willie,fred
@@ -749,29 +750,29 @@
 margaretta,maggie,meg,peg,midge,margie,madge,peggy,marge,daisy,margery,gretta,rita
 margarita,maggie,meg,metta,midge,greta,megan,maisie,madge,marge,daisy,peggie,rita,margo
 marge,margery,margaret,margaretta
 margie,marjorie
 marguerite,peggy
 mariah,mary,maria
 marian,marianna,marion
-marie,mae
+marie,mae,mary
 marietta,mariah,mercy,polly,may,molly,mitzi,minnie,mollie,mae,maureen,marion,marie,mamie,mary,maria
 marilyn,mary
 marion,mary
 marissa,rissa
 marjorie,margy,margie
 marni,marnie
 marsha,marcie,mary,marcia
 martha,marty,mattie,mat,patsy,patty
 martin,marty
 martina,tina
 martine,tine
 marv,marvin
 marvin,marv
-mary,mamie,molly,mae,polly,mitzi
+mary,mamie,molly,mae,polly,mitzi,marie
 masayuki,masa
 mat,mattie
 mathew,mat,maty,matt
 mathilda,tillie,patty
 matilda,tilly,maud,matty,tilla
 matthew,thys,matt,thias,mattie,matty
 matthews,matt,mattie,matty
@@ -809,15 +810,15 @@
 mick,micky
 miguel,miguell,miguael,miguaell,miguail,miguaill,miguayl,miguayll,michael,mike,miggy
 mike,micky,mick,michael
 mildred,milly
 millicent,missy,milly
 minerva,minnie
 minnie,wilhelmina
-miranda,randy,mandy,mira
+miranda,randi,randy,mandy,mira
 miriam,mimi,mitzi,mitzie
 missy,melissa
 mitch,mitchell
 mitchell,mitch
 mitzi,mary,mittie,mitty
 mitzie,mittie,mitty
 monet,nettie
@@ -914,14 +915,16 @@
 priscilla,prissy,cissy,cilla
 providence,provy
 prudence,prue,prudy
 prudy,prudence
 rachel,shelly,rachael
 rafaela,rafa
 ramona,mona
+randall,randy
+randolf,dolph,randy
 randolph,dolph,randy
 raphael,ralph
 ray,raymond
 raymond,ray
 reba,beck,becca
 rebecca,beck,becca,reba,becky
 reggie,reginald,reg
@@ -969,21 +972,21 @@
 rudolph,dolph,rudy,olph,rolf
 rudolphus,dolph,rudy,olph,rolf
 russell,russ,rusty
 ryan,ry
 sabrina,brina
 safieel,safie
 salome,loomie
-salvador,sal
-samantha,sammy,sam,mantha
-sammy,samuel
-sampson,sam
-samson,sam
-samuel,sammy,sam
-samyra,myra
+salvador,sal,sally
+sam,sammy
+samantha,sam,sammy,mantha
+sampson,sam,sammy
+samson,sam,sammy
+samuel,sam,sammy
+samyra,sam,sammy,myra
 sandra,sandy,cassandra
 sandy,sandra
 sanford,sandy
 sarah,sally,sadie,sara
 sarilla,silla
 savannah,vannie,anna,savanna
 scott,scotty,sceeter,squat,scottie
```

### Comparing `nicknames-0.1.8/hatch_build.py` & `nicknames-0.1.9/hatch_build.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 but this method didn't work with editable installs. See
 https://stackoverflow.com/q/73466480/5156887
 
 This post https://stackoverflow.com/q/61624018/5156887
 makes it seem like a custom setuptools script is the only way. So that's what I did,
 but using hatch.
 """
+
 import shutil
 
 from hatchling.builders.hooks.plugin.interface import BuildHookInterface
 
 
 class CustomHook(BuildHookInterface):
     def initialize(self, version, build_data):
```

### Comparing `nicknames-0.1.8/pyproject.toml` & `nicknames-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -35,28 +35,28 @@
 "Bug Tracker" = "https://github.com/carltonnorthern/nicknames/issues"
 
 [tool.hatch.version]
 path = "src/nicknames/_version.py"
 
 [tool.hatch.envs.default]
 dependencies = [
-  "pytest",
-  "ruff>=0.1.6",
+  "pytest==7.4.4",  # The last version that supports pythoh 3.7
+  "ruff==0.4.1",
 ]
 
 [tool.hatch.envs.default.scripts]
 # Run these in the repo root to get ALL python files
-lint = "python -m ruff format --check .. && python -m ruff .."
-fmt = "python -m ruff --fix .. && python -m ruff format .."
+lint = "python -m ruff format --check .. && python -m ruff check .."
+fmt = "python -m ruff check --fix .. && python -m ruff format .."
 test = "pytest"
 test-CI = "pytest -Werror"
 sync = "python ../normalize.py && python ../sql/generate_sql.py"
 
 # Instructs hatch to call hatch_build.py during build step
 [tool.hatch.build.hooks.custom]
 
 [tool.ruff]
-select = [
+lint.select = [
   "E",  # pyflakes
   "F",  # pyflakes
   "I",  # isort
 ]
```

### Comparing `nicknames-0.1.8/../README.md` & `nicknames-0.1.9/../README.md`

 * *Files identical despite different names*

### Comparing `nicknames-0.1.8/PKG-INFO` & `nicknames-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: nicknames
-Version: 0.1.8
+Version: 0.1.9
 Summary: Hand-curated dataset of English given names and nicknames
 Project-URL: Homepage, https://github.com/carltonnorthern/nicknames
 Project-URL: Bug Tracker, https://github.com/carltonnorthern/nicknames/issues
 Author-email: Carlton Northern <carlton.northern@gmail.com>
 License-Expression: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

