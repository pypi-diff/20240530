# Comparing `tmp/scoobydoo-0.0.tar.gz` & `tmp/scoobydoo-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoobydoo-0.0.tar", last modified: Wed Mar 15 19:25:25 2023, max compression
+gzip compressed data, was "scoobydoo-0.1.tar", last modified: Thu May 30 13:46:14 2024, max compression
```

## Comparing `scoobydoo-0.0.tar` & `scoobydoo-0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 19:25:25.270645 scoobydoo-0.0/
--rw-rw-rw-   0        0        0      389 2023-03-15 19:25:25.269645 scoobydoo-0.0/PKG-INFO
--rw-rw-rw-   0        0        0       76 2023-02-02 21:49:13.000000 scoobydoo-0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-15 19:25:25.245710 scoobydoo-0.0/scoobydoo/
--rw-rw-rw-   0        0        0        0 2023-03-15 19:16:22.000000 scoobydoo-0.0/scoobydoo/__init__.py
--rw-rw-rw-   0        0        0      623 2023-02-10 14:22:25.000000 scoobydoo-0.0/scoobydoo/catchphrases.py
--rw-rw-rw-   0        0        0     1412 2023-03-15 19:20:14.000000 scoobydoo-0.0/scoobydoo/characters.py
--rw-rw-rw-   0        0        0     2062 2023-03-15 19:18:40.000000 scoobydoo-0.0/scoobydoo/main.py
-drwxrwxrwx   0        0        0        0 2023-03-15 19:25:25.267651 scoobydoo-0.0/scoobydoo.egg-info/
--rw-rw-rw-   0        0        0      389 2023-03-15 19:25:24.000000 scoobydoo-0.0/scoobydoo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-03-15 19:25:25.000000 scoobydoo-0.0/scoobydoo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 19:25:24.000000 scoobydoo-0.0/scoobydoo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-03-15 19:25:24.000000 scoobydoo-0.0/scoobydoo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-15 19:14:10.000000 scoobydoo-0.0/scoobydoo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-03-15 19:25:24.000000 scoobydoo-0.0/scoobydoo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-15 19:25:25.271640 scoobydoo-0.0/setup.cfg
--rw-rw-rw-   0        0        0      804 2023-03-15 18:31:21.000000 scoobydoo-0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:46:14.676882 scoobydoo-0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-30 13:46:14.676882 scoobydoo-0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 13:46:10.000000 scoobydoo-0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:46:14.672882 scoobydoo-0.1/scoobydoo/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 13:46:10.000000 scoobydoo-0.1/scoobydoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-30 13:46:10.000000 scoobydoo-0.1/scoobydoo/catchphrases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-30 13:46:10.000000 scoobydoo-0.1/scoobydoo/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-30 13:46:10.000000 scoobydoo-0.1/scoobydoo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:46:14.672882 scoobydoo-0.1/scoobydoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-30 13:46:14.000000 scoobydoo-0.1/scoobydoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-30 13:46:14.000000 scoobydoo-0.1/scoobydoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:46:14.000000 scoobydoo-0.1/scoobydoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 13:46:14.000000 scoobydoo-0.1/scoobydoo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:46:14.000000 scoobydoo-0.1/scoobydoo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 13:46:14.000000 scoobydoo-0.1/scoobydoo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:46:14.676882 scoobydoo-0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-30 13:46:10.000000 scoobydoo-0.1/setup.py
```

### Comparing `scoobydoo-0.0/scoobydoo/characters.py` & `scoobydoo-0.1/scoobydoo/characters.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import random
-from .catchphrases import phrases
-# parent class
-class Character:
-    def __init__(self,name):
-        self.name=name
-    
-    def gimme_a_catchphrase(self,name):
-        kind = self.kind
-        options = phrases[kind][name]
-        #print(kind_opts)
-        return random.choice(options)
-        
-
-# define child classes of Character
-class People(Character):
-    kind = 'person' # class variable shared by all instances
-    def __init__(self, name, shirtcolor,gender):
-        super().__init__(name)  # inherits Character class attributes
-        self.shirtcolor = shirtcolor # unique attributes to the People sub-class
-        self.gender = gender
-   
-class Animals(Character):
-    kind='animal'
-    def __init__(self, name): # can pass more args to init that can be defined as an attribute via self.attribute = attribute
-        super().__init__(name)
-        #self.species = species
-
-class Villains(Character):
-    kind='villain'
-    def __init__(self,name,unmasked=False):
-        super().__init__(name)
-        self.unmasked=unmasked
-    # how to deal with unmasked bool?
-    # gimme_a_catchphrase() is parent method so the attribute unmasked wouldn't be in scope at Characters
-    # def unmasked_phrase(unmasked):
-    #     if unmasked:
-    #         return "I would have gotten away with it too, if it weren't for those meddling kids!"
+import random
+from .catchphrases import phrases
+# parent class
+class Character:
+    def __init__(self,name):
+        self.name=name
+    
+    def gimme_a_catchphrase(self,name):
+        kind = self.kind
+        options = phrases[kind][name]
+        #print(kind_opts)
+        return random.choice(options)
+        
+
+# define child classes of Character
+class People(Character):
+    kind = 'person' # class variable shared by all instances
+    def __init__(self, name, shirtcolor,gender):
+        super().__init__(name)  # inherits Character class attributes
+        self.shirtcolor = shirtcolor # unique attributes to the People sub-class
+        self.gender = gender
+   
+class Animals(Character):
+    kind='animal'
+    def __init__(self, name): # can pass more args to init that can be defined as an attribute via self.attribute = attribute
+        super().__init__(name)
+        #self.species = species
+
+class Villains(Character):
+    kind='villain'
+    def __init__(self,name,unmasked=False):
+        super().__init__(name)
+        self.unmasked=unmasked
+    # how to deal with unmasked bool?
+    # gimme_a_catchphrase() is parent method so the attribute unmasked wouldn't be in scope at Characters
+    # def unmasked_phrase(unmasked):
+    #     if unmasked:
+    #         return "I would have gotten away with it too, if it weren't for those meddling kids!"
     #     else:
```

### Comparing `scoobydoo-0.0/scoobydoo/main.py` & `scoobydoo-0.1/scoobydoo/main.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-from . import characters
-import argparse
-
-# here you can do more with pulling out class attributes and whatnot 
-# but we are just going to use characters.Animals() for main()
-
-# scooby = characters.Animals('scooby')
-# print(f"Instance: {scooby}")
-# print(f"gimme a catchphrase! :{scooby.gimme_a_catchphrase(scooby.name)}") # call a method that belongs to the parent class (Characters)
-
-# shaggy = characters.People('shaggy','green','male')
-# print(shaggy.kind) # global People attribute
-# print(shaggy.shirtcolor) # local instance attributes defined upon instantiation
-# print(shaggy.gender)
-
-# redbeard = characters.Villains("Redbeard's ghost")
-# print(redbeard)
-# print(redbeard.kind)
-
-def create_animal(char_name):
-    char = characters.Animals(char_name)
-    return char
-def create_person(char_name):
-    char = characters.People(char_name)
-    return char
-def create_villain(char_name):
-    char = characters.Villains(char_name)
-    return char
-
-def main():
-    # argparse to pass cli args
-    parser = argparse.ArgumentParser(
-    description="Gimme a catch phrase!",
-    usage = "scoobydoo -n scooby -t animal"
-    )
-    
-    parser.add_argument(
-        "-n",
-        "--name",
-        type=str,
-        required=True,
-        help="character name"
-    )
-    
-    parser.add_argument(
-        "-t",
-        "--type",
-        type=str,
-        required=True,
-        help = "character type"
-    )
-    
-    
-    #parse the args
-    args = parser.parse_args()
-    
-    char_name = args.name
-    char_type = args.type
-
-    #call create_char()
-    if char_type == "person":
-        character = create_person(char_name)
-    elif char_type == "animal":
-        character = create_animal(char_name)
-    elif char_type == "villain":
-        character = create_villain(char_name)
-    else:
-        raise ValueError("invalid value given to -t --type")
-    
-    name = character.name
-    
-    print(character.gimme_a_catchphrase(name))
-    
-    return
-
-if __name__ == "__main__":
+from . import characters
+import argparse
+
+# here you can do more with pulling out class attributes and whatnot 
+# but we are just going to use characters.Animals() for main()
+
+# scooby = characters.Animals('scooby')
+# print(f"Instance: {scooby}")
+# print(f"gimme a catchphrase! :{scooby.gimme_a_catchphrase(scooby.name)}") # call a method that belongs to the parent class (Characters)
+
+# shaggy = characters.People('shaggy','green','male')
+# print(shaggy.kind) # global People attribute
+# print(shaggy.shirtcolor) # local instance attributes defined upon instantiation
+# print(shaggy.gender)
+
+# redbeard = characters.Villains("Redbeard's ghost")
+# print(redbeard)
+# print(redbeard.kind)
+
+def create_animal(char_name):
+    char = characters.Animals(char_name)
+    return char
+def create_person(char_name):
+    char = characters.People(char_name)
+    return char
+def create_villain(char_name):
+    char = characters.Villains(char_name)
+    return char
+
+def main():
+    # argparse to pass cli args
+    parser = argparse.ArgumentParser(
+    description="Gimme a catch phrase!",
+    usage = "scoobydoo -n scooby -t animal"
+    )
+    
+    parser.add_argument(
+        "-n",
+        "--name",
+        type=str,
+        required=True,
+        help="character name"
+    )
+    
+    parser.add_argument(
+        "-t",
+        "--type",
+        type=str,
+        required=True,
+        help = "character type"
+    )
+    
+    
+    #parse the args
+    args = parser.parse_args()
+    
+    char_name = args.name
+    char_type = args.type
+
+    #call create_char()
+    if char_type == "person":
+        character = create_person(char_name)
+    elif char_type == "animal":
+        character = create_animal(char_name)
+    elif char_type == "villain":
+        character = create_villain(char_name)
+    else:
+        raise ValueError("invalid value given to -t --type")
+    
+    name = character.name
+    
+    print(character.gimme_a_catchphrase(name))
+    
+    return
+
+if __name__ == "__main__":
     main()
```

### Comparing `scoobydoo-0.0/setup.py` & `scoobydoo-0.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import setuptools
-from setuptools import setup
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-# change all this
-setup(
-    name="scoobydoo",
-    version="0.0",
-    description="Giving Scooby Doo Character Catch Phrases",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/kyle-woodward/scooby-doo",
-    packages=setuptools.find_packages(),
-    author="Kyle Woodward",
-    author_email="kw.geospatial@gmail.com",
-    license="GNU GPL v3.0",
-    zip_safe=False,
-    include_package_data=True,
-    entry_points={
-        "console_scripts": [
-            "scoobydoo = scoobydoo.main:main",
-        ]
-    },
-    #install_requires=["simplecmr", "earthengine-api", "gcsfs", "fire", "pipetools"],
+import setuptools
+from setuptools import setup
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+# change all this
+setup(
+    name="scoobydoo",
+    version="0.1",
+    description="Giving Scooby Doo Character Catch Phrases",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/kyle-woodward/scooby-doo",
+    packages=setuptools.find_packages(),
+    author="Kyle Woodward",
+    author_email="kw.geospatial@gmail.com",
+    license="GNU GPL v3.0",
+    zip_safe=False,
+    include_package_data=True,
+    entry_points={
+        "console_scripts": [
+            "scoobydoo = scoobydoo.main:main",
+        ]
+    },
+    #install_requires=["simplecmr", "earthengine-api", "gcsfs", "fire", "pipetools"],
 )
```

