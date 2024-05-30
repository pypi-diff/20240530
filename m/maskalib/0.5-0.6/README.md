# Comparing `tmp/maskalib-0.5.tar.gz` & `tmp/maskalib-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maskalib-0.5.tar", last modified: Wed May 29 01:05:30 2024, max compression
+gzip compressed data, was "maskalib-0.6.tar", last modified: Wed May 29 11:00:02 2024, max compression
```

## Comparing `maskalib-0.5.tar` & `maskalib-0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 01:05:30.060000 maskalib-0.5/
--rw-rw-rw-   0        0        0     1112 2024-05-29 01:05:32.000000 maskalib-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1014 2024-05-26 02:18:54.000000 maskalib-0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 01:05:30.090000 maskalib-0.5/maskalib/
--rw-rw-rw-   0        0        0     8267 2024-05-26 01:56:06.000000 maskalib-0.5/maskalib/MaskaAI.py
--rw-rw-rw-   0        0        0     8107 2024-05-26 02:00:24.000000 maskalib-0.5/maskalib/MaskaAIPremium.py
--rw-rw-rw-   0        0        0      135 2024-05-29 00:21:54.000000 maskalib-0.5/maskalib/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-26 01:47:54.000000 maskalib-0.5/maskalib/main.py
--rw-rw-rw-   0        0        0     6468 2024-05-29 01:04:42.000000 maskalib-0.5/maskalib/ps99invest.py
-drwxrwxrwx   0        0        0        0 2024-05-29 01:05:30.120000 maskalib-0.5/maskalib.egg-info/
--rw-rw-rw-   0        0        0     1112 2024-05-29 01:05:30.000000 maskalib-0.5/maskalib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-05-29 01:05:30.000000 maskalib-0.5/maskalib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 01:05:30.000000 maskalib-0.5/maskalib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-29 01:05:30.000000 maskalib-0.5/maskalib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 01:05:32.000000 maskalib-0.5/setup.cfg
--rw-rw-rw-   0        0        0      373 2024-05-29 01:05:10.000000 maskalib-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:00:02.827686 maskalib-0.6/
+-rw-rw-rw-   0        0        0     1112 2024-05-29 11:00:02.826180 maskalib-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1014 2024-05-26 02:18:54.000000 maskalib-0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 11:00:02.822182 maskalib-0.6/maskalib/
+-rw-rw-rw-   0        0        0     8267 2024-05-26 01:56:06.000000 maskalib-0.6/maskalib/MaskaAI.py
+-rw-rw-rw-   0        0        0     8107 2024-05-26 02:00:24.000000 maskalib-0.6/maskalib/MaskaAIPremium.py
+-rw-rw-rw-   0        0        0      135 2024-05-29 00:21:54.000000 maskalib-0.6/maskalib/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-26 01:47:54.000000 maskalib-0.6/maskalib/main.py
+-rw-rw-rw-   0        0        0     6806 2024-05-29 10:58:45.000000 maskalib-0.6/maskalib/ps99invest.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:00:02.826180 maskalib-0.6/maskalib.egg-info/
+-rw-rw-rw-   0        0        0     1112 2024-05-29 11:00:02.000000 maskalib-0.6/maskalib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-29 11:00:02.000000 maskalib-0.6/maskalib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 11:00:02.000000 maskalib-0.6/maskalib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-29 11:00:02.000000 maskalib-0.6/maskalib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 11:00:02.827686 maskalib-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      373 2024-05-29 10:59:19.000000 maskalib-0.6/setup.py
```

### Comparing `maskalib-0.5/PKG-INFO` & `maskalib-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maskalib
-Version: 0.5
+Version: 0.6
 Description-Content-Type: text/markdown
 
 # Maskalib
 
 Maskalib is a Python library for [describe the purpose of your library].
 
 ## Installation
```

### Comparing `maskalib-0.5/README.md` & `maskalib-0.6/README.md`

 * *Files identical despite different names*

### Comparing `maskalib-0.5/maskalib/MaskaAI.py` & `maskalib-0.6/maskalib/MaskaAI.py`

 * *Files identical despite different names*

### Comparing `maskalib-0.5/maskalib/MaskaAIPremium.py` & `maskalib-0.6/maskalib/MaskaAIPremium.py`

 * *Files identical despite different names*

### Comparing `maskalib-0.5/maskalib/ps99invest.py` & `maskalib-0.6/maskalib/ps99invest.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,16 +99,16 @@
 def ps99invest(PetsName):
     now = datetime.now()
     formatted_timern = now.strftime('%Y-%m-%d %H:%M:%S.%f')[:-3]
     PetName = PetsName
     rapinfo = f"All rap from Start of data to Today (this is the date and value in gems of each rap data update): {getpetvalue(PetName)}"
     PetExist = f"All exist from Start of data to Today (this is the date and number of exist of each daata update): {getpetexist(PetName)}"
     PetsSimular = f"Pets similar of {PetName} : {getpetsimilar(PetName)}"
-    prompttt = f"Your name is MaskaV2.Petsim99. Talk like an AI that want to help me and also make your text beatiful, with emojies, alot of different color, make sure your text with hashtag work for a Discord message. My question: Should i invest into the {PetName}, what is the minimal value should i buy it for and the maximal and what is your value prediction for next month (Also make sure to check if you think the value is fake because sometimes, peoples like manipulating pets to make a fake value of it, so if it got manipulated, start by saying THIS PET IS PROB MANIPULATED with proof of what you know but if value look like a normal value with all the data, say this pet is not Manipulated)(aslo finish by saying, You can also look for this pets because they are similar as your pet .. with the pets similar but don't include image links)? What you know: we are the: {formatted_timern}. Rap: {rapinfo}. Exists: {PetExist}. Similarity: {PetsSimular}"
-    promptt = f"Make sure to put color and emoji about each subject and make all the things colorfull. The current Rap is the latest one and the one that the date is the closest to {formatted_timern} and its also the last one of the rap list. Make sure that you put alot of info. Make sure all numbers are good because 90000000 is 90million and 90000000.00 is still 90millions and not 900 millions. Make sure it will get a good looking for discord and try to embed it without a code. one hashtag = giant, two hashtag = mid and 3 hashtag is little for the text on discord. Make sure to not use more then 3 hashtag Last part of prompt: {prompttt}"
+    prompttt = f"Your name is MaskaV2.Petsim99. Talk like an AI that want to help me and also make your text beatiful, with emojies, alot of different color, make sure your text with hashtag work for a Discord message. My question: Should i invest into the {PetName}, what is the minimal value should i buy it for and the maximal(make sure to look at last value and all the other value. Verify again to see if its make sense and explain why this amount) and what is your value prediction for next month (Also make sure to check if you think the value is fake because sometimes, peoples like manipulating pets to make a fake value of it, so if it got manipulated, start by saying THIS PET IS PROB MANIPULATED with proof of what you know but if value look like a normal value with all the data, say this pet is not Manipulated)(aslo finish by saying, You can also look for this pets because they are similar as your pet .. with the pets similar but don't include image links)? What you know: we are the: {formatted_timern}. Rap: {rapinfo}. Exists: {PetExist}. Similarity: {PetsSimular}"
+    promptt = f"If it's a pet then say Pet in the infos, but when it as enchant or potion on the name, it's not a pet. it will be a Enchant or a Pet. Make sure to verify all info and explain correctly so everyone will understand. Make sure to put color and emoji about each subject and make all the things colorfull. The current Rap is the latest one and the one that the date is the closest to {formatted_timern} and its also the last one of the rap list. Make sure that you put alot of info. Make sure all numbers are good because 90000000 is 90million and 90000000.00 is still 90millions and not 900 millions. Make sure it will get a good looking for discord and try to embed it without a code. one hashtag = giant, two hashtag = mid and 3 hashtag is little for the text on discord. Make sure to not use more then 3 hashtag Last part of prompt: {prompttt}"
     url = "https://api.jarvis.cx/api/v1/ai-chat"
     jarvis_guid = str(uuid.uuid4())
     headers = {
     "accept": "application/json, text/plain, */*",
     "accept-language": "en-US,en;q=0.9",
     "content-type": "application/json",
     "sec-ch-ua": "\"Google Chrome\";v=\"125\", \"Chromium\";v=\"125\", \"Not.A/Brand\";v=\"24\"",
```

### Comparing `maskalib-0.5/maskalib.egg-info/PKG-INFO` & `maskalib-0.6/maskalib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maskalib
-Version: 0.5
+Version: 0.6
 Description-Content-Type: text/markdown
 
 # Maskalib
 
 Maskalib is a Python library for [describe the purpose of your library].
 
 ## Installation
```

