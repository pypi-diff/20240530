# Comparing `tmp/ecs_game-1.0.tar.gz` & `tmp/ecs_game-1.5.tar.gz`

## Comparing `ecs_game-1.0.tar` & `ecs_game-1.5.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ecs_game-1.0/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ecs_game-1.0/src/ecs_game/__init__.py
--rw-r--r--   0        0        0     7859 2020-02-02 00:00:00.000000 ecs_game-1.0/src/ecs_game/engine.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 ecs_game-1.0/LICENSE
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ecs_game-1.0/README.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 ecs_game-1.0/pyproject.toml
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 ecs_game-1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ecs_game-1.5/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ecs_game-1.5/src/__init__.py
+-rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 ecs_game-1.5/src/engine.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ecs_game-1.5/src/ecs_game/__init__.py
+-rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 ecs_game-1.5/src/ecs_game/flight_engine.py
+-rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 ecs_game-1.5/src/ecs_game/launch_engine.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 ecs_game-1.5/LICENSE
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ecs_game-1.5/README.md
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 ecs_game-1.5/pyproject.toml
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 ecs_game-1.5/PKG-INFO
```

### Comparing `ecs_game-1.0/src/ecs_game/engine.py` & `ecs_game-1.5/src/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     else:
         text_1 = font.render("You Died!", True, color)
         text_2 = font.render("Press ESC to Restart", True, color)
         text_1_rect = text_1.get_rect(center=(width / 2, height / 2 - 20))
         text_2_rect = text_2.get_rect(center=(width / 2, height / 2 + 20))
         screen.blit(text_1, text_1_rect)
         screen.blit(text_2, text_2_rect)
-def update_cycle(player, danger, target, mystery, mysteries, is_onscreen, update_player, update_target, update_danger, update_mystery, is_collision, score, height, k, m_lag, d_lag, t_lag, p_alive, p_spos, t_spos, d_spos):
+def update_cycle(player, danger, target, mystery, mysteries, is_onscreen, update_player, update_target, update_danger, update_mystery, is_collision, score, width, height, k, m_lag, d_lag, t_lag, p_alive, p_spos, t_spos, d_spos):
     if p_alive:
         m_lag -= 1
         d_lag -= 1
         t_lag -= 1
         commanded_player_pos = update_player(player.x, player.y)
         if is_onscreen(commanded_player_pos[0], commanded_player_pos[1]):
             player.pos = commanded_player_pos
@@ -117,17 +117,23 @@
                 score += 20
             elif is_onscreen(commanded_mystery_pos[0], commanded_mystery_pos[1]):
                 mystery.pos = commanded_mystery_pos
             else:
                 mysteries.remove(mystery)
 
         if t_lag == 0:
-            target.pos = (0, randint(50, height - 50))
+            if update_target(0, 0)[0] > 0:
+                target.pos = (0, randint(50, height - 50))
+            else:
+                target.pos = (width, randint(50, height - 50))
         if d_lag == 0:
-            danger.pos = (0, randint(50, height - 50))
+            if update_danger(0, 0)[0] > 0:
+                danger.pos = (0, randint(50, height - 50))
+            else:
+                danger.pos = (width, randint(50, height - 50))
 
         if score <= 0:
             p_alive = False
 
     else:
         player.pos = p_spos
         danger.pos = d_spos
@@ -142,15 +148,15 @@
 
     return score, m_lag, d_lag, t_lag, p_alive
 
 ##########################################################################
 # Modified Actor class to add scale, flip and loading images from urls
 ##########################################################################
 class GameElement(Actor):
-    def __init__(self, url, image, pos=None, anchor=None, **kwargs):
+    def __init__(self, url, pos=None, anchor=None, **kwargs):
         self._handle_unexpected_kwargs(kwargs)
 
         self.__dict__["_rect"] = rect.ZRect((0, 0), (0, 0))
         # Initialise it at (0, 0) for size (0, 0).
         # We'll move it to the right place and resize it later
 
         self.url = url
```

### Comparing `ecs_game-1.0/LICENSE` & `ecs_game-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ecs_game-1.0/pyproject.toml` & `ecs_game-1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "pgzero", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ecs-game"
-version = "1.0"
+version = "1.5"
 authors = [
   { name="Haider Iqbal", email="haideriqbal11@outlook.com" },
 ]
 description = "A package containing the functions and code needed to run the ECS Big Game Project. Based on Pygame-Zero"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ecs_game-1.0/PKG-INFO` & `ecs_game-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ecs-game
-Version: 1.0
+Version: 1.5
 Summary: A package containing the functions and code needed to run the ECS Big Game Project. Based on Pygame-Zero
 Project-URL: Homepage, https://github.com/Luddo183/ECS-Game
 Project-URL: Issues, https://github.com/Luddo183/ECS-Game/issues
 Author-email: Haider Iqbal <haideriqbal11@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

