# Comparing `tmp/dias_uteis-0.1.8.tar.gz` & `tmp/dias_uteis-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dias_uteis-0.1.8.tar", max compression
+gzip compressed data, was "dias_uteis-0.1.9.tar", max compression
```

## Comparing `dias_uteis-0.1.8.tar` & `dias_uteis-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6534 2024-01-17 19:13:02.246246 dias_uteis-0.1.8/dias_uteis/__init__.py
--rw-r--r--   0        0        0    11418 2024-01-17 18:39:43.131058 dias_uteis-0.1.8/dias_uteis/business_days.py
--rw-r--r--   0        0        0        0 2024-01-25 22:40:10.049884 dias_uteis-0.1.8/dias_uteis/py.typed
--rw-r--r--   0        0        0     1099 2023-10-20 18:55:39.179995 dias_uteis-0.1.8/LICENSE
--rw-r--r--   0        0        0      571 2024-01-25 22:41:44.517763 dias_uteis-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1770 2023-11-15 20:07:32.581803 dias_uteis-0.1.8/README.md
--rw-r--r--   0        0        0     2450 1970-01-01 00:00:00.000000 dias_uteis-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     6540 2024-03-15 15:03:50.862468 dias_uteis-0.1.9/dias_uteis/__init__.py
+-rw-r--r--   0        0        0    11292 2024-03-15 15:32:06.927986 dias_uteis-0.1.9/dias_uteis/business_days.py
+-rw-r--r--   0        0        0        0 2024-01-25 22:40:10.049884 dias_uteis-0.1.9/dias_uteis/py.typed
+-rw-r--r--   0        0        0     1099 2023-10-20 18:55:39.179995 dias_uteis-0.1.9/LICENSE
+-rw-r--r--   0        0        0      571 2024-03-15 15:42:10.532137 dias_uteis-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1770 2023-11-15 20:07:32.581803 dias_uteis-0.1.9/README.md
+-rw-r--r--   0        0        0     2501 1970-01-01 00:00:00.000000 dias_uteis-0.1.9/PKG-INFO
```

### Comparing `dias_uteis-0.1.8/dias_uteis/__init__.py` & `dias_uteis-0.1.9/dias_uteis/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
         nenhum feriado estiver definido.
     """
     return _business_days_default.year_holidays(year)
 
 
 def diff_du(a: datetime.date, b: datetime.date) -> int:
     """
-    Calcula a diferença entre dois dias úteis.
+    Calcula a diferença entre dois dias úteis (b-a).
 
     Parâmetros
     ----------
     a : datetime.date
     b : datetime.date
 
     Retorna
```

### Comparing `dias_uteis-0.1.8/dias_uteis/business_days.py` & `dias_uteis-0.1.9/dias_uteis/business_days.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,21 +90,21 @@
 class BusinessDays:
     def __init__(self, holidays: Optional[List[Holiday]] = None):
         self.holidays = holidays
 
     def _get_year_business_days(self, year: int) -> List[datetime.date]:
         return _get_year_business_days(year, self.holidays)
 
-    def _find_bd(
-        self, start_date: datetime.date, direction: int
-    ) -> datetime.date:
-        date = start_date
-        while not self.is_bd(date):
-            date += datetime.timedelta(days=direction)
-        return date
+    # def _find_bd(
+    #     self, start_date: datetime.date, direction: int
+    # ) -> datetime.date:
+    #     date = start_date
+    #     while not self.is_bd(date):
+    #         date += datetime.timedelta(days=direction)
+    #     return date
 
     def _get_all_bdays_for_years(self, years: List[int]) -> List[datetime.date]:
         all_bdays = []
         for year in years:
             all_bdays += self._get_year_business_days(year)
         return all_bdays
 
@@ -144,42 +144,14 @@
         # Fix self.holidays to be empty list if None
         self_holidays = [] if not self.holidays else self.holidays
         holidays = _get_year_holidays(date.year, self_holidays)
         if date in holidays:
             return True
         return False
 
-    def last_bd(self, date: Optional[datetime.date] = None) -> datetime.date:
-        """
-        Finds the last business day relative to today.
-
-        Returns
-        -------
-        datetime.date
-            The date of the last business day.
-        """
-        if not date:
-            date = datetime.date.today() - datetime.timedelta(days=1)
-        date -= datetime.timedelta(days=1)
-        return self._find_bd(date, -1)
-
-    def next_bd(self, date: Optional[datetime.date] = None) -> datetime.date:
-        """
-        Finds the next business day relative to today.
-
-        Returns
-        -------
-        datetime.date
-            The date of the next business day.
-        """
-        if not date:
-            date = datetime.date.today() + datetime.timedelta(days=1)
-        date += datetime.timedelta(days=1)
-        return self._find_bd(date, 1)
-
     def delta_bd(self, date: datetime.date, delta_days: int) -> datetime.date:
         """
         Calculates the date a certain number of business days from a specified date.
 
         Parameters
         ----------
         from_date : datetime.date
@@ -198,14 +170,40 @@
         # delta_days*2 so the bday of the end year is always inside the list all_bdays
         end_calendar_date = date + datetime.timedelta(days=delta_days * 2)
         years = _get_years_between_two_dates(date, end_calendar_date)
         all_bdays = self._get_all_bdays_for_years(years)
         date_position = all_bdays.index(date)
         return all_bdays[date_position + delta_days]
 
+    def next_bd(self, date: Optional[datetime.date] = None) -> datetime.date:
+        """
+        Finds the next business day relative to today.
+
+        Returns
+        -------
+        datetime.date
+            The date of the next business day.
+        """
+        if not date:
+            date = datetime.date.today()
+        return self.delta_bd(date, 1)
+
+    def last_bd(self, date: Optional[datetime.date] = None) -> datetime.date:
+        """
+        Finds the last business day relative to today.
+
+        Returns
+        -------
+        datetime.date
+            The date of the last business day.
+        """
+        if not date:
+            date = datetime.date.today()
+        return self.delta_bd(date, -1)
+
     def range_bd(
         self,
         start_date: datetime.date,
         end_date: datetime.date,
         include_end: bool = False,
     ) -> List[datetime.date]:
         """
@@ -281,15 +279,15 @@
         if self.holidays:
             return _get_year_holidays(year, self.holidays)
         else:
             return []
 
     def diff_bd(self, a: datetime.date, b: datetime.date) -> int:
         """
-        Calculates the difference between two business days.
+        Calculates the difference between two business days (b-a).
 
         Parameters
         ----------
         a : datetime.date
         b : datetime.date
 
         Returns
```

### Comparing `dias_uteis-0.1.8/LICENSE` & `dias_uteis-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dias_uteis-0.1.8/pyproject.toml` & `dias_uteis-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dias-uteis"
-version = "0.1.8"
+version = "0.1.9"
 description = "Ferramentas para cálculos de dias úteis no calendário brasileiro."
 authors = ["renanmoretto <himynameisrenan@outlook.com>"]
 readme = "README.md"
 packages = [{include = "dias_uteis"}]
 repository = "https://github.com/renanmoretto/dias_uteis"
 include = ["dias_uteis/py.typed"]
```

### Comparing `dias_uteis-0.1.8/README.md` & `dias_uteis-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dias_uteis-0.1.8/PKG-INFO` & `dias_uteis-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: dias-uteis
-Version: 0.1.8
+Version: 0.1.9
 Summary: Ferramentas para cálculos de dias úteis no calendário brasileiro.
 Home-page: https://github.com/renanmoretto/dias_uteis
 Author: renanmoretto
 Author-email: himynameisrenan@outlook.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/renanmoretto/dias_uteis
 Description-Content-Type: text/markdown
 
 # dias_uteis
 Biblioteca feita para facilitar o uso e cálculos de dias úteis no calendário brasileiro.
 
 - Sem dependências externas.
```

