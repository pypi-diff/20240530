# Comparing `tmp/b2sim-2.1.5.tar.gz` & `tmp/b2sim-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2sim-2.1.5.tar", last modified: Wed May 15 20:00:49 2024, max compression
+gzip compressed data, was "b2sim-2.2.1.tar", last modified: Thu May 30 05:49:57 2024, max compression
```

## Comparing `b2sim-2.1.5.tar` & `b2sim-2.2.1.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 20:00:49.199327 b2sim-2.1.5/
--rw-rw-rw-   0        0        0    35823 2023-05-09 05:51:58.000000 b2sim-2.1.5/LICENSE
--rw-rw-rw-   0        0        0      123 2024-02-07 03:13:22.000000 b2sim-2.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      343 2024-05-15 20:00:49.198328 b2sim-2.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    18853 2024-02-22 04:54:10.000000 b2sim-2.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 20:00:49.096504 b2sim-2.1.5/b2sim/
--rw-rw-rw-   0        0        0        0 2024-02-05 03:29:23.000000 b2sim-2.1.5/b2sim/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 20:00:49.142159 b2sim-2.1.5/b2sim/analysis/
--rw-rw-rw-   0        0        0      108 2024-02-12 21:33:54.000000 b2sim-2.1.5/b2sim/analysis/__init__.py
--rw-rw-rw-   0        0        0    25122 2024-05-15 06:39:44.000000 b2sim-2.1.5/b2sim/analysis/ai.py
--rw-rw-rw-   0        0        0     4346 2024-02-21 01:49:15.000000 b2sim-2.1.5/b2sim/analysis/fitness.py
--rw-rw-rw-   0        0        0     5061 2024-02-12 21:30:11.000000 b2sim-2.1.5/b2sim/analysis/graphing.py
--rw-rw-rw-   0        0        0     5674 2024-02-07 01:42:59.000000 b2sim-2.1.5/b2sim/analysis/visualize.py
-drwxrwxrwx   0        0        0        0 2024-05-15 20:00:49.178679 b2sim-2.1.5/b2sim/engine/
--rw-rw-rw-   0        0        0      102 2024-02-04 07:54:08.000000 b2sim-2.1.5/b2sim/engine/__init__.py
--rw-rw-rw-   0        0        0    14197 2024-02-23 22:29:57.000000 b2sim-2.1.5/b2sim/engine/actions.py
--rw-rw-rw-   0        0        0    13545 2024-05-15 06:56:28.000000 b2sim-2.1.5/b2sim/engine/farms.py
--rw-rw-rw-   0        0        0     9918 2024-02-08 21:25:01.000000 b2sim-2.1.5/b2sim/engine/info.py
--rw-rw-rw-   0        0        0   102973 2024-05-09 00:56:22.000000 b2sim-2.1.5/b2sim/engine/main.py
--rw-rw-rw-   0        0        0     5069 2024-02-09 00:43:24.000000 b2sim-2.1.5/b2sim/engine/rounds.py
-drwxrwxrwx   0        0        0        0 2024-05-15 20:00:49.195814 b2sim-2.1.5/b2sim/templates/
--rw-rw-rw-   0        0        0     1944 2024-02-19 06:29:12.000000 b2sim-2.1.5/b2sim/templates/config.txt
--rw-rw-rw-   0        0        0     2027 2024-04-12 03:06:06.000000 b2sim-2.1.5/b2sim/templates/eco_send_info.csv
--rw-rw-rw-   0        0        0      613 2023-07-19 19:03:45.000000 b2sim-2.1.5/b2sim/templates/nat_send_lengths.csv
-drwxrwxrwx   0        0        0        0 2024-05-15 20:00:49.197318 b2sim-2.1.5/b2sim.egg-info/
--rw-rw-rw-   0        0        0      343 2024-05-15 20:00:49.000000 b2sim-2.1.5/b2sim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      563 2024-05-15 20:00:49.000000 b2sim-2.1.5/b2sim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 20:00:49.000000 b2sim-2.1.5/b2sim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-15 20:00:49.000000 b2sim-2.1.5/b2sim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-15 20:00:49.000000 b2sim-2.1.5/b2sim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 20:00:49.199327 b2sim-2.1.5/setup.cfg
--rw-rw-rw-   0        0        0      469 2024-05-15 06:35:31.000000 b2sim-2.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 05:49:57.840545 b2sim-2.2.1/
+-rw-rw-rw-   0        0        0    35823 2023-05-09 05:51:58.000000 b2sim-2.2.1/LICENSE
+-rw-rw-rw-   0        0        0      123 2024-05-30 05:46:52.000000 b2sim-2.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      384 2024-05-30 05:49:57.839544 b2sim-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    18853 2024-02-22 04:54:10.000000 b2sim-2.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 05:49:57.808951 b2sim-2.2.1/b2sim/
+-rw-rw-rw-   0        0        0        0 2024-02-05 03:29:23.000000 b2sim-2.2.1/b2sim/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 05:49:57.823028 b2sim-2.2.1/b2sim/analysis/
+-rw-rw-rw-   0        0        0      108 2024-02-12 21:33:54.000000 b2sim-2.2.1/b2sim/analysis/__init__.py
+-rw-rw-rw-   0        0        0    25122 2024-05-15 06:39:44.000000 b2sim-2.2.1/b2sim/analysis/ai.py
+-rw-rw-rw-   0        0        0     4346 2024-02-21 01:49:15.000000 b2sim-2.2.1/b2sim/analysis/fitness.py
+-rw-rw-rw-   0        0        0     6651 2024-05-23 20:35:40.000000 b2sim-2.2.1/b2sim/analysis/graphing.py
+-rw-rw-rw-   0        0        0     5674 2024-02-07 01:42:59.000000 b2sim-2.2.1/b2sim/analysis/visualize.py
+drwxrwxrwx   0        0        0        0 2024-05-30 05:49:57.833544 b2sim-2.2.1/b2sim/engine/
+-rw-rw-rw-   0        0        0      102 2024-02-04 07:54:08.000000 b2sim-2.2.1/b2sim/engine/__init__.py
+-rw-rw-rw-   0        0        0    14197 2024-02-23 22:29:57.000000 b2sim-2.2.1/b2sim/engine/actions.py
+-rw-rw-rw-   0        0        0     2996 2024-05-23 20:10:43.000000 b2sim-2.2.1/b2sim/engine/alt_eco.py
+-rw-rw-rw-   0        0        0    13545 2024-05-15 06:56:28.000000 b2sim-2.2.1/b2sim/engine/farms.py
+-rw-rw-rw-   0        0        0     9918 2024-02-08 21:25:01.000000 b2sim-2.2.1/b2sim/engine/info.py
+-rw-rw-rw-   0        0        0      714 2024-05-15 21:55:07.000000 b2sim-2.2.1/b2sim/engine/logger.py
+-rw-rw-rw-   0        0        0   104381 2024-05-23 20:45:28.000000 b2sim-2.2.1/b2sim/engine/main.py
+-rw-rw-rw-   0        0        0     5069 2024-02-09 00:43:24.000000 b2sim-2.2.1/b2sim/engine/rounds.py
+drwxrwxrwx   0        0        0        0 2024-05-30 05:49:57.837543 b2sim-2.2.1/b2sim/templates/
+-rw-rw-rw-   0        0        0     1944 2024-02-19 06:29:12.000000 b2sim-2.2.1/b2sim/templates/config.txt
+-rw-rw-rw-   0        0        0     2027 2024-05-29 16:25:38.000000 b2sim-2.2.1/b2sim/templates/eco_send_info.csv
+-rw-rw-rw-   0        0        0      613 2023-07-19 19:03:45.000000 b2sim-2.2.1/b2sim/templates/nat_send_lengths.csv
+drwxrwxrwx   0        0        0        0 2024-05-30 05:49:57.838544 b2sim-2.2.1/b2sim.egg-info/
+-rw-rw-rw-   0        0        0      384 2024-05-30 05:49:57.000000 b2sim-2.2.1/b2sim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      610 2024-05-30 05:49:57.000000 b2sim-2.2.1/b2sim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 05:49:57.000000 b2sim-2.2.1/b2sim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-30 05:49:57.000000 b2sim-2.2.1/b2sim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-30 05:49:57.000000 b2sim-2.2.1/b2sim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 05:49:57.840545 b2sim-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      520 2024-05-30 05:23:00.000000 b2sim-2.2.1/setup.py
```

### Comparing `b2sim-2.1.5/LICENSE` & `b2sim-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.5/README.md` & `b2sim-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.5/b2sim/analysis/ai.py` & `b2sim-2.2.1/b2sim/analysis/ai.py`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.5/b2sim/analysis/fitness.py` & `b2sim-2.2.1/b2sim/analysis/fitness.py`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.5/b2sim/analysis/graphing.py` & `b2sim-2.2.1/b2sim/analysis/graphing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import matplotlib.pyplot as plt
 
-def viewHistory(gs, dim = (12,6), display_farms = True, font_size = 12):
+def viewHistory(gs, dim = (12,6), display_farms = True, display_snipers = True, font_size = 12):
         '''
         Given an instance of an GameState on which a simulation has been run, graph the history of cash and eco over the course of that simulation.
 
         Parameters:
         gs (GameState): An instance of the GameState class whose cash and eco history we want to graph
 
         Returns: 
@@ -126,8 +126,47 @@
             } 
             df = pd.DataFrame(farm_table)
             df = df.set_index('Farm Index')
             df = df.round(0)
             display(df)
 
         
+        #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        #Create a table that displays the revenue/expenses of each sniper farm
+        #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+        gs.sniper_revenues = []
+        gs.sniper_expenses = []
+        gs.sniper_profits = []
+        gs.sniper_starts = []
+        gs.sniper_ends = []
+
+        for sniper in gs.supply_drops:
+            gs.sniper_revenues.append(sniper.revenue)
+            gs.sniper_expenses.append(sniper.expenses)
+            gs.sniper_profits.append(sniper.revenue - sniper.expenses)
+
+            start_time = max(sniper.purchase_time, gs.simulation_start_time)
+            if sniper.sell_time == None:
+                end_time = gs.current_time
+            else:
+                end_time = sniper.sell_time
+
+            gs.sniper_starts.append(start_time)
+            gs.sniper_ends.append(end_time)
+        
+        # dictionary of lists 
+        if display_snipers and len(gs.supply_drops) > 0:
+            sniper_table = {
+                'Sniper Index': [int(i) for i in range(len(gs.supply_drops))], 
+                'Revenue': gs.sniper_revenues, 
+                'Expenses': gs.sniper_expenses, 
+                'Profit': gs.sniper_profits,
+                'Start Time': gs.sniper_starts, 
+                'End Time': gs.sniper_ends
+            } 
+            df = pd.DataFrame(sniper_table)
+            df = df.set_index('Sniper Index')
+            df = df.round(0)
+            display(df)
+
         # gs.logs.append("Successfully generated graph! \n")
```

### Comparing `b2sim-2.1.5/b2sim/analysis/visualize.py` & `b2sim-2.2.1/b2sim/analysis/visualize.py`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.5/b2sim/engine/actions.py` & `b2sim-2.2.1/b2sim/engine/actions.py`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.5/b2sim/engine/farms.py` & `b2sim-2.2.1/b2sim/engine/farms.py`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.5/b2sim/engine/info.py` & `b2sim-2.2.1/b2sim/engine/info.py`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.5/b2sim/engine/main.py` & `b2sim-2.2.1/b2sim/engine/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # %%
 from math import floor, ceil
 from b2sim.engine.info import *
 from b2sim.engine.actions import *
 from b2sim.engine.farms import *
+from b2sim.engine.alt_eco import *
 from copy import deepcopy as dc
 
 # %%
 
 
 # %%
 def impact(cash: float, loan: float, amount: float):
@@ -137,22 +138,30 @@
         if self.druid_farms is not None:
             self.sotf = self.druid_farms['Spirit of the Forest Index']
             self.druid_key = len(self.druid_farms) - 2
         else:
             self.sotf = None
             self.druid_key = 0
 
-        #Next, supply drops!
+        # Next, supply drops!
+        # This should be a list of Sniper objects
         self.supply_drops = initial_state.get('Supply Drops')
-        if self.supply_drops is not None:
-            self.elite_sniper = self.supply_drops['Elite Sniper Index']
-            self.sniper_key = len(self.supply_drops) - 2
-        else:
-            self.elite_sniper = None
-            self.sniper_key = 0
+
+        # Is there an elite sniper among these supply drops?
+        # If so, where is it located?
+        self.elite_sniper = None
+        if self.supply_drops is None:
+            self.supply_drops = []
+        for i in range(len(self.supply_drops)):
+            if self.supply_drops[i].T5 and self.elite_sniper is None:
+                self.elite_sniper = i
+            if self.supply_drops[i].T5 and self.elite_sniper is not None:
+                # Prevents the sim from running with multiple T5 snipers
+                self.supply_drops[i].T5 = False
+                self.supply_drops[i].update()
 
         #Next, heli farms!
         self.heli_farms = initial_state.get('Heli Farms')
         if self.heli_farms is not None:
             self.special_poperations = self.heli_farms['Special Poperations Index']
             self.heli_key = len(self.heli_farms) - 2
         else:
@@ -256,15 +265,15 @@
         if self.boat_farms is None:
             self.boat_farms = {}
         if self.druid_farms is None:
             self.druid_farms = {}
         if self.heli_farms is None:
             self.heli_farms = {}
         if self.supply_drops is None:
-            self.supply_drops = {}
+            self.supply_drops = []
         self.simulation_start_time = 0
             
         self.logs.append("MESSAGE FROM GameState.__init__(): ")
         self.logs.append("Initialized Game State!")
         self.logs.append("The current game round is %s"%(self.current_round))
         self.logs.append("The current game time is %s seconds"%(self.current_time))
         self.logs.append("The game round start times are given by %s \n"%(self.rounds.round_starts))
@@ -716,14 +725,18 @@
                     new_cash, new_loan = impact(self.cash,self.loan, payout['Payout'])
 
                     if payout['Source'] == 'Farm':
                         #Track the money generated by the farm
                         key = payout['Index']
                         farm = self.farms[key]
                         farm.revenue += new_cash - self.cash
+                    elif payout['Source'] == 'Sniper':
+                        key = payout['Index']
+                        sniper = self.supply_drops[key]
+                        sniper.revenue += new_cash - self.cash
 
                     self.cash, self.loan = new_cash, new_loan
                     self.logs.append("Awarded direct payment %s at time %s"%(round(payout['Payout'],2),round(payout['Time'],2)))
                 
                 
             elif payout['Payout Type'] == 'Bank Payment':
                 #Identify the bank that we're paying and deposit money into that bank's account
@@ -785,16 +798,16 @@
             # WARNING: Unusual results will occur if you attempt to implement automated purchases of multiple alt eco's at the same time.
             # WARNING: Because automated purchases are processed after checking the buy queue, unexpected results may occur if items in the buy queue do not have a min_buy_time designated.
 
             if payout['Time'] <= self.supply_drop_max_buy_time and try_to_buy == True:
                 while self.cash >= sniper_globals['Supply Drop Cost'] + self.supply_drop_buffer:
                     made_purchase = True
                     self.cash -= sniper_globals['Supply Drop Cost']
-                    self.supply_drops[self.sniper_key] = payout['Time']
-                    self.sniper_key += 1
+                    self.supply_drops.append(Sniper(payout['Time']))
+                    self.supply_drops[-1].expenses += sniper_globals['Supply Drop Cost']
                     self.logs.append("Purchased a supply drop! (Automated purchase)")
 
             if payout['Time'] <= self.druid_farm_max_buy_time and try_to_buy == True:
                 while self.cash >= druid_globals['Druid Farm Cost'] + self.druid_farm_buffer:
                     made_purchase = True
                     self.cash -= druid_globals['Druid Farm Cost']
                     self.druid_farms[self.druid_key] = payout['Time']
@@ -913,32 +926,31 @@
                             'Source': 'Druid'
                         }
                         payout_times.append(payout_entry)
                         self.inc += 1
 
 
         #SUPPLY DROPS
-        if self.supply_drops is not None:
-            for key in self.supply_drops.keys():
-                supply_drop = self.supply_drops[key]
-                if key == self.elite_sniper:
-                    payout_amount = sniper_globals['Elite Sniper Payout']
-                else:
-                    payout_amount = sniper_globals['Supply Drop Payout']
+        for i in range(len(self.supply_drops)):
+            sniper = self.supply_drops[i]
+            if sniper.sell_time is None:
+                payout_amount = sniper.payout_amount
 
+                supply_drop = sniper.purchase_time
                 #Determine the earliest supply drop activation that could occur within the interval of interest (self.current_time,target_time]
                 drop_index = max(1,floor(1 + (self.current_time - supply_drop - sniper_globals['Supply Drop Initial Cooldown'])/sniper_globals['Supply Drop Usage Cooldown'])+1)
                 supply_drop_time = supply_drop + sniper_globals['Supply Drop Initial Cooldown'] + sniper_globals['Supply Drop Usage Cooldown']*(drop_index-1)
                 while supply_drop_time <= target_time:
                     
                     payout_entry = {
                         'Time': supply_drop_time,
                         'Payout Type': 'Direct',
                         'Payout': payout_amount,
-                        'Source': 'Sniper'
+                        'Source': 'Sniper',
+                        'Index': i
                     }
                     payout_times.append(payout_entry)
                     supply_drop_time += sniper_globals['Supply Drop Usage Cooldown']
 
         #HELI FARMS
         if self.heli_farms is not None:
             for key in self.heli_farms.keys():
@@ -1270,14 +1282,18 @@
             # In general the this step is necessary if there are in the presence of loans.
             # NOTE: Loans do not influence purchases, so we can process expense tracking for farms only when a transaction actually occurs.
 
             #For tracking the revenue of farms
             for farm in self.farms:
                 farm.h_revenue = farm.revenue
 
+            #For tracking the revenue of snipers
+            for sniper in self.supply_drops:
+                sniper.h_revenue = sniper.revenue
+
             #For tracking the revenue of boat farms
             for key in self.boat_farms.keys():
                 boat_farm = self.boat_farms[key]
                 boat_farm['Hypothetical Revenue'] = boat_farm['Revenue']
             
             for dict_obj in purchase_info:
 
@@ -1319,14 +1335,18 @@
                 self.cash = h_cash
                 self.loan = h_loan
 
                 # Track the revenue made by each farm
                 for farm in self.farms:
                     farm.revenue = farm.h_revenue
 
+                # Track the revenue made by each sniper farm
+                for sniper in self.supply_drops:
+                    sniper.revenue = sniper.h_revenue
+
                 # Track the revenue made by each boat farm
                 for key in self.boat_farms.keys():
                     boat_farm = self.boat_farms[key]
                     boat_farm['Revenue'] = boat_farm['Hypothetical Revenue']
 
                 # self.logs.append("The new lists of farm revenues and expenses are given by: ")
                 # self.logs.append(str(self.farm_revenues))
@@ -1715,42 +1735,49 @@
                 self.druid_farm_buffer = dict_obj['Buffer']
                 self.logs.append("Triggered automated druid farm purchases until time %s"%(self.druid_farm_max_buy_time))
         # SUPPLY DROP RELATED MATTERS
         elif dict_obj['Type'] == 'Buy Supply Drop':
             if stage == 'check':
                 h_cash, h_loan = impact(h_cash, h_loan, -1*sniper_globals['Supply Drop Cost'])
             else:
-                self.supply_drops[self.sniper_key] = payout['Time']
-                self.sniper_key += 1
+                self.supply_drops.append(Sniper(payout['Time']))
+                self.supply_drops[-1].expenses = sniper_globals['Supply Drop Cost']
                 self.logs.append("Purchased a supply drop!")
         elif dict_obj['Type'] == 'Sell Supply Drop':
+            ind = dict_obj['Index']
+            sniper = self.supply_drops[ind]
             if stage == 'check':
+                h_new_cash, h_new_loan = h_cash, h_loan
                 if dict_obj['Index'] == self.elite_sniper:
-                    h_cash, h_loan = impact(h_cash, h_loan, game_globals['Sellback Value']*(sniper_globals['Supply Drop Cost'] + sniper_globals['Elite Sniper Upgrade Cost']) )
+                    h_new_cash, h_new_loan = impact(h_cash, h_loan, game_globals['Sellback Value']*(sniper_globals['Supply Drop Cost'] + sniper_globals['Elite Sniper Upgrade Cost']) )
                 else:
-                    h_cash, h_loan = impact(h_cash, h_loan, game_globals['Sellback Value']*sniper_globals['Supply Drop Cost'])
+                    h_new_cash, h_new_loan = impact(h_cash, h_loan, game_globals['Sellback Value']*sniper_globals['Supply Drop Cost'])
+                sniper.h_revenue += h_new_cash - h_cash
+                h_cash, h_loan = h_new_cash, h_new_loan
             else:
                 ind = dict_obj['Index']
                 self.logs.append("Selling the supply drop at index %s"%(ind))
                 #If the supply drop we're selling is actually an E-sniper, then...
-                if self.elite_sniper is not None:
-                    if ind == self.elite_sniper:
-                        self.logs.append("The supply drop being sold is an elite sniper!")
-                        self.elite_sniper = None
+                if self.elite_sniper is not None and ind == self.elite_sniper:
+                    self.logs.append("The supply drop being sold is an elite sniper!")
+                    self.elite_sniper = None
+                    self.supply_drops[ind].T5 = False
+                    self.supply_drops[ind].sell_time = payout['Time']
         elif dict_obj['Type'] == 'Buy Elite Sniper':
             if stage == 'check':
                 #WARNING: There can only be one e-sniper at a time!
                 if self.elite_sniper is not None:
                     self.logs.append("WARNING! Tried to purchase an Elite Sniper when one already exists! Aborting buy queue!")
                     self.warnings.append(len(self.logs)-1)
                     self.valid_action_flag = False
                 h_cash, h_loan = impact(h_cash, h_loan, -1*sniper_globals['Elite Sniper Upgrade Cost'])
             else:
                 ind = dict_obj['Index']
                 self.elite_sniper = ind
+                self.supply_drops[ind].upgrade()
                 self.logs.append("Upgrading the supply drop at index %s into an elite sniper!"%(ind))
         elif dict_obj['Type'] == 'Repeatedly Buy Supply Drops':
             #There is no checking stage for this action
             if stage != 'check':
                 self.supply_drop_max_buy_time = dict_obj['Maximum Buy Time']
                 self.supply_drop_buffer = dict_obj['Buffer']
                 self.logs.append("Triggered automated supply drop purchases until time %s"%(self.supply_drop_max_buy_time))
@@ -1771,17 +1798,17 @@
             else:
                 ind = dict_obj['Index']
                 self.logs.append("Selling the heli farm at index %s"%(ind))
                 #If the supply drop we're selling is actually a special poperations, then...
                 if self.special_poperations is not None:
                     if ind == self.special_poperations:
                         self.logs.append("The heli farm being sold is a special poperations!")
-                        self.elite_sniper = None
+                        self.special_poperations = None
                 
-                self.supply_drops.pop(ind)
+                self.heli_farms.pop(ind)
         elif dict_obj['Type'] == 'Buy Special Poperations':
             if stage == 'check':
                 #WARNING: There can only be one Special Poperations on screen at a time!
                 if self.special_poperations is not None:
                     self.logs.append("WARNING! Tried to purchase Special Poperations when one already exists! Aborting buy queue!")
                     self.warnings.append(len(self.logs)-1)
                     self.valid_action_flag = False
```

### Comparing `b2sim-2.1.5/b2sim/engine/rounds.py` & `b2sim-2.2.1/b2sim/engine/rounds.py`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.5/b2sim/templates/config.txt` & `b2sim-2.2.1/b2sim/templates/config.txt`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.5/b2sim/templates/eco_send_info.csv` & `b2sim-2.2.1/b2sim/templates/eco_send_info.csv`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ﻿send_name,price,eco,start_round,end_round,send_duration,fortified,camo,regrow,moab_class
 Zero,0,0,0,50,0,FALSE,FALSE,FALSE,FALSE
 Grouped Reds,20,1,1,11,0.8,FALSE,TRUE,TRUE,FALSE
 Spaced Blues,15,0.8,1,2,1.5,FALSE,TRUE,TRUE,FALSE
-Grouped Blues,24,1,3,11,0.6,FALSE,TRUE,TRUE,FALSE
+Grouped Blues,24,1,3,12,0.6,FALSE,TRUE,TRUE,FALSE
 Spaced Greens,18,0.9,2,4,1.15,FALSE,TRUE,TRUE,FALSE
 Grouped Greens,35,1.4,5,16,0.4,FALSE,TRUE,TRUE,FALSE
 Spaced Yellows,24,1.2,3,6,1.15,FALSE,TRUE,TRUE,FALSE
 Grouped Yellows,40,1.6,7,19,0.24,FALSE,TRUE,TRUE,FALSE
 Spaced Pinks,28,1.4,4,8,0.9,FALSE,TRUE,TRUE,FALSE
 Grouped Pinks,65,2.4,9,50,0.2,FALSE,TRUE,TRUE,FALSE
 Spaced Whites,30,1.5,5,9,0.84,FALSE,TRUE,TRUE,FALSE
```

### Comparing `b2sim-2.1.5/b2sim/templates/nat_send_lengths.csv` & `b2sim-2.2.1/b2sim/templates/nat_send_lengths.csv`

 * *Files identical despite different names*

### Comparing `b2sim-2.1.5/b2sim.egg-info/SOURCES.txt` & `b2sim-2.2.1/b2sim.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 b2sim/analysis/__init__.py
 b2sim/analysis/ai.py
 b2sim/analysis/fitness.py
 b2sim/analysis/graphing.py
 b2sim/analysis/visualize.py
 b2sim/engine/__init__.py
 b2sim/engine/actions.py
+b2sim/engine/alt_eco.py
 b2sim/engine/farms.py
 b2sim/engine/info.py
+b2sim/engine/logger.py
 b2sim/engine/main.py
 b2sim/engine/rounds.py
 b2sim/templates/config.txt
 b2sim/templates/eco_send_info.csv
 b2sim/templates/nat_send_lengths.csv
```

