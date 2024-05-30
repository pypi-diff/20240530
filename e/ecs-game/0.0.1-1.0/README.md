# Comparing `tmp/ecs_game-0.0.1.tar.gz` & `tmp/ecs_game-1.0.tar.gz`

## Comparing `ecs_game-0.0.1.tar` & `ecs_game-1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ecs_game-0.0.1/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ecs_game-0.0.1/src/ecs_game/__init__.py
--rw-r--r--   0        0        0     7859 2020-02-02 00:00:00.000000 ecs_game-0.0.1/src/ecs_game/game_engine.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 ecs_game-0.0.1/LICENSE
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ecs_game-0.0.1/README.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 ecs_game-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 ecs_game-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ecs_game-1.0/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ecs_game-1.0/src/ecs_game/__init__.py
+-rw-r--r--   0        0        0     7859 2020-02-02 00:00:00.000000 ecs_game-1.0/src/ecs_game/engine.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 ecs_game-1.0/LICENSE
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ecs_game-1.0/README.md
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 ecs_game-1.0/pyproject.toml
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 ecs_game-1.0/PKG-INFO
```

### Comparing `ecs_game-0.0.1/src/ecs_game/game_engine.py` & `ecs_game-1.0/src/ecs_game/engine.py`

 * *Files identical despite different names*

### Comparing `ecs_game-0.0.1/LICENSE` & `ecs_game-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecs_game-0.0.1/pyproject.toml` & `ecs_game-1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling", "pgzero", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ecs-game"
-version = "0.0.1"
+version = "1.0"
 authors = [
   { name="Haider Iqbal", email="haideriqbal11@outlook.com" },
 ]
 description = "A package containing the functions and code needed to run the ECS Big Game Project. Based on Pygame-Zero"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-Homepage = "https://github.com/pypa/sampleproject"
-Issues = "https://github.com/pypa/sampleproject/issues"
+Homepage = "https://github.com/Luddo183/ECS-Game"
+Issues = "https://github.com/Luddo183/ECS-Game/issues"
```

