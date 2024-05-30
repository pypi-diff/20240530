# Comparing `tmp/pkrcomponents-1.7.4.tar.gz` & `tmp/pkrcomponents-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkrcomponents-1.7.4.tar", last modified: Wed May 29 11:11:12 2024, max compression
+gzip compressed data, was "pkrcomponents-1.8.0.tar", last modified: Wed May 29 13:56:54 2024, max compression
```

## Comparing `pkrcomponents-1.7.4.tar` & `pkrcomponents-1.8.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-29 11:11:12.488982 pkrcomponents-1.7.4/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-29 11:11:11.715634 pkrcomponents-1.7.4/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.7.4/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.7.4/LICENSE.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-24 19:24:47.000000 pkrcomponents-1.7.4/MANIFEST.in
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      951 2024-05-29 11:11:12.473321 pkrcomponents-1.7.4/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      224 2024-05-24 00:25:51.000000 pkrcomponents-1.7.4/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1512 2024-05-29 11:07:46.000000 pkrcomponents-1.7.4/coverage.txt
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-29 11:11:12.395083 pkrcomponents-1.7.4/pkrcomponents/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.7.4/pkrcomponents/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.7.4/pkrcomponents/_common.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      933 2024-05-27 23:40:01.000000 pkrcomponents-1.7.4/pkrcomponents/action.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7569 2024-05-24 00:57:29.000000 pkrcomponents-1.7.4/pkrcomponents/bitcard.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3948 2024-05-15 15:52:00.000000 pkrcomponents-1.7.4/pkrcomponents/board.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1386 2024-05-29 10:10:09.000000 pkrcomponents-1.7.4/pkrcomponents/buy_in.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4409 2024-05-29 11:00:59.000000 pkrcomponents-1.7.4/pkrcomponents/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3439 2024-05-27 17:30:11.000000 pkrcomponents-1.7.4/pkrcomponents/constants.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1401 2024-05-29 11:06:38.000000 pkrcomponents-1.7.4/pkrcomponents/deck.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.7.4/pkrcomponents/evaluator.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13075 2024-05-27 18:44:25.000000 pkrcomponents-1.7.4/pkrcomponents/hand.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1586 2024-05-29 09:57:04.000000 pkrcomponents-1.7.4/pkrcomponents/level.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1382 2024-05-27 17:30:11.000000 pkrcomponents-1.7.4/pkrcomponents/listings.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.7.4/pkrcomponents/lookup_table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3998 2024-05-29 10:44:39.000000 pkrcomponents-1.7.4/pkrcomponents/payout.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4434 2024-05-15 18:17:46.000000 pkrcomponents-1.7.4/pkrcomponents/players.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1429 2024-05-29 10:34:29.000000 pkrcomponents-1.7.4/pkrcomponents/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    16774 2024-05-29 11:06:38.000000 pkrcomponents-1.7.4/pkrcomponents/table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    14901 2024-05-29 10:39:42.000000 pkrcomponents-1.7.4/pkrcomponents/table_player.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3439 2024-05-29 09:25:32.000000 pkrcomponents-1.7.4/pkrcomponents/tournament.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-29 11:11:12.458308 pkrcomponents-1.7.4/pkrcomponents/utils/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:06:12.000000 pkrcomponents-1.7.4/pkrcomponents/utils/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      301 2024-05-27 18:51:06.000000 pkrcomponents-1.7.4/pkrcomponents/utils/converters.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      371 2024-05-27 20:12:18.000000 pkrcomponents-1.7.4/pkrcomponents/utils/validators.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-29 11:11:12.473321 pkrcomponents-1.7.4/pkrcomponents.egg-info/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      693 2024-05-29 11:11:09.000000 pkrcomponents-1.7.4/pkrcomponents.egg-info/SOURCES.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.7.4/requirements.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-29 11:11:12.488982 pkrcomponents-1.7.4/setup.cfg
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1399 2024-05-27 22:58:49.000000 pkrcomponents-1.7.4/setup.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-29 13:56:54.219368 pkrcomponents-1.8.0/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-29 13:56:53.168300 pkrcomponents-1.8.0/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.8.0/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.8.0/LICENSE.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-24 19:24:47.000000 pkrcomponents-1.8.0/MANIFEST.in
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      951 2024-05-29 13:56:54.214492 pkrcomponents-1.8.0/PKG-INFO
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      224 2024-05-24 00:25:51.000000 pkrcomponents-1.8.0/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1512 2024-05-29 13:54:07.000000 pkrcomponents-1.8.0/coverage.txt
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-29 13:56:54.092709 pkrcomponents-1.8.0/pkrcomponents/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.8.0/pkrcomponents/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.8.0/pkrcomponents/_common.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      933 2024-05-27 23:40:01.000000 pkrcomponents-1.8.0/pkrcomponents/action.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7569 2024-05-24 00:57:29.000000 pkrcomponents-1.8.0/pkrcomponents/bitcard.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3948 2024-05-15 15:52:00.000000 pkrcomponents-1.8.0/pkrcomponents/board.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1386 2024-05-29 10:10:09.000000 pkrcomponents-1.8.0/pkrcomponents/buy_in.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4409 2024-05-29 11:00:59.000000 pkrcomponents-1.8.0/pkrcomponents/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3439 2024-05-27 17:30:11.000000 pkrcomponents-1.8.0/pkrcomponents/constants.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1401 2024-05-29 11:06:38.000000 pkrcomponents-1.8.0/pkrcomponents/deck.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.8.0/pkrcomponents/evaluator.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13075 2024-05-27 18:44:25.000000 pkrcomponents-1.8.0/pkrcomponents/hand.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1586 2024-05-29 09:57:04.000000 pkrcomponents-1.8.0/pkrcomponents/level.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1382 2024-05-27 17:30:11.000000 pkrcomponents-1.8.0/pkrcomponents/listings.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.8.0/pkrcomponents/lookup_table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3998 2024-05-29 10:44:39.000000 pkrcomponents-1.8.0/pkrcomponents/payout.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5171 2024-05-29 13:53:41.000000 pkrcomponents-1.8.0/pkrcomponents/players.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1429 2024-05-29 10:34:29.000000 pkrcomponents-1.8.0/pkrcomponents/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    16774 2024-05-29 11:06:38.000000 pkrcomponents-1.8.0/pkrcomponents/table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    14901 2024-05-29 10:39:42.000000 pkrcomponents-1.8.0/pkrcomponents/table_player.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3439 2024-05-29 09:25:32.000000 pkrcomponents-1.8.0/pkrcomponents/tournament.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-29 13:56:54.170554 pkrcomponents-1.8.0/pkrcomponents/utils/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:06:12.000000 pkrcomponents-1.8.0/pkrcomponents/utils/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      301 2024-05-27 18:51:06.000000 pkrcomponents-1.8.0/pkrcomponents/utils/converters.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      371 2024-05-27 20:12:18.000000 pkrcomponents-1.8.0/pkrcomponents/utils/validators.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-29 13:56:54.201764 pkrcomponents-1.8.0/pkrcomponents.egg-info/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      693 2024-05-29 13:56:51.000000 pkrcomponents-1.8.0/pkrcomponents.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.8.0/requirements.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-29 13:56:54.219368 pkrcomponents-1.8.0/setup.cfg
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1399 2024-05-27 22:58:49.000000 pkrcomponents-1.8.0/setup.py
```

### Comparing `pkrcomponents-1.7.4/LICENSE.txt` & `pkrcomponents-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/MANIFEST.in` & `pkrcomponents-1.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/PKG-INFO` & `pkrcomponents-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkrcomponents
-Version: 1.7.4
+Version: 1.8.0
 Summary: A Poker Package
 Home-page: https://github.com/manggy94/PokerComponents
 Author: Alexandre MANGWA
 Author-email: alex.mangwa@gmail.com
 License: MIT
 Keywords: poker pkrcomponents pkr
 Platform: UNKNOWN
```

### Comparing `pkrcomponents-1.7.4/coverage.txt` & `pkrcomponents-1.8.0/coverage.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 pkrcomponents/deck.py                  26      1    96%
 pkrcomponents/evaluator.py             28      0   100%
 pkrcomponents/hand.py                 228      0   100%
 pkrcomponents/level.py                 17      0   100%
 pkrcomponents/listings.py              16      0   100%
 pkrcomponents/lookup_table.py         112      0   100%
 pkrcomponents/payout.py                37      0   100%
-pkrcomponents/players.py               96      0   100%
+pkrcomponents/players.py              109      0   100%
 pkrcomponents/pot.py                   13      0   100%
 pkrcomponents/table.py                327      4    99%
 pkrcomponents/table_player.py         182      2    99%
 pkrcomponents/tournament.py            46      0   100%
 pkrcomponents/utils/__init__.py         0      0   100%
 pkrcomponents/utils/converters.py       6      1    83%
 pkrcomponents/utils/validators.py       7      0   100%
 -------------------------------------------------------
-TOTAL                                1521      8    99%
+TOTAL                                1534      8    99%
```

### Comparing `pkrcomponents-1.7.4/pkrcomponents/_common.py` & `pkrcomponents-1.8.0/pkrcomponents/_common.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/pkrcomponents/action.py` & `pkrcomponents-1.8.0/pkrcomponents/action.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/pkrcomponents/bitcard.py` & `pkrcomponents-1.8.0/pkrcomponents/bitcard.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/pkrcomponents/board.py` & `pkrcomponents-1.8.0/pkrcomponents/board.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/pkrcomponents/buy_in.py` & `pkrcomponents-1.8.0/pkrcomponents/buy_in.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/pkrcomponents/card.py` & `pkrcomponents-1.8.0/pkrcomponents/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/pkrcomponents/constants.py` & `pkrcomponents-1.8.0/pkrcomponents/constants.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/pkrcomponents/deck.py` & `pkrcomponents-1.8.0/pkrcomponents/deck.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/pkrcomponents/evaluator.py` & `pkrcomponents-1.8.0/pkrcomponents/evaluator.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/pkrcomponents/hand.py` & `pkrcomponents-1.8.0/pkrcomponents/hand.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/pkrcomponents/level.py` & `pkrcomponents-1.8.0/pkrcomponents/level.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/pkrcomponents/listings.py` & `pkrcomponents-1.8.0/pkrcomponents/listings.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/pkrcomponents/lookup_table.py` & `pkrcomponents-1.8.0/pkrcomponents/lookup_table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/pkrcomponents/payout.py` & `pkrcomponents-1.8.0/pkrcomponents/payout.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/pkrcomponents/players.py` & `pkrcomponents-1.8.0/pkrcomponents/players.py`

 * *Files 19% similar despite different names*

```diff
@@ -135,11 +135,35 @@
         """Advances the Big Blind seat"""
         try:
             self.bb = self.occupied_seats[self.occupied_seats.index(self.bb) + 1]
         except IndexError:
             self.bb = self.occupied_seats[0]
         self.distribute_positions()
 
+    def get_bb_seat_from_button(self, button_seat: int) -> int:
+        """
+        Returns the Big Blind seat based on the button seat
+
+        Args:
+            button_seat (int): The seat of the button
+
+        Returns:
+            bb_seat (int): The seat of the Big Blind
+        """
+        if len(self.occupied_seats) < 3:
+            advance = 1
+        else:
+            advance = 2
+        button_index = self.occupied_seats.index(button_seat)
+        bb_index = button_index
+        for _ in range(advance):
+            bb_index += 1
+            try:
+                self.occupied_seats[bb_index]
+            except IndexError:
+                bb_index = 0
+        return self.occupied_seats[bb_index]
+
     def hand_reset(self):
         """Reset all players for a new hand"""
         for player in self:
             player.reset_hand_status()
```

### Comparing `pkrcomponents-1.7.4/pkrcomponents/pot.py` & `pkrcomponents-1.8.0/pkrcomponents/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/pkrcomponents/table.py` & `pkrcomponents-1.8.0/pkrcomponents/table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/pkrcomponents/table_player.py` & `pkrcomponents-1.8.0/pkrcomponents/table_player.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/pkrcomponents/tournament.py` & `pkrcomponents-1.8.0/pkrcomponents/tournament.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/pkrcomponents.egg-info/SOURCES.txt` & `pkrcomponents-1.8.0/pkrcomponents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.4/setup.py` & `pkrcomponents-1.8.0/setup.py`

 * *Files identical despite different names*

