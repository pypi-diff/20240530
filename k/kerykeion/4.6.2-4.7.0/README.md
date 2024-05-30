# Comparing `tmp/kerykeion-4.6.2.tar.gz` & `tmp/kerykeion-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerykeion-4.6.2.tar", max compression
+gzip compressed data, was "kerykeion-4.7.0.tar", max compression
```

## Comparing `kerykeion-4.6.2.tar` & `kerykeion-4.7.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    34273 2024-03-05 19:55:06.854597 kerykeion-4.6.2/LICENSE
--rw-r--r--   0        0        0     8634 2024-03-05 19:55:06.855014 kerykeion-4.6.2/README.md
--rw-r--r--   0        0        0     3917 2024-05-20 21:44:34.775470 kerykeion-4.6.2/kerykeion/__init__.py
--rw-r--r--   0        0        0      293 2024-05-20 21:44:34.775703 kerykeion-4.6.2/kerykeion/aspects/__init__.py
--rw-r--r--   0        0        0     5832 2024-05-20 21:44:34.775937 kerykeion-4.6.2/kerykeion/aspects/aspects_utils.py
--rw-r--r--   0        0        0     4507 2024-05-20 21:44:34.776153 kerykeion-4.6.2/kerykeion/aspects/natal_aspects.py
--rw-r--r--   0        0        0     3993 2024-05-20 21:44:34.776366 kerykeion-4.6.2/kerykeion/aspects/synastry_aspects.py
--rw-r--r--   0        0        0    22965 2024-05-20 21:44:34.776635 kerykeion-4.6.2/kerykeion/astrological_subject.py
--rw-r--r--   0        0        0      127 2024-05-20 21:44:34.776876 kerykeion-4.6.2/kerykeion/charts/__init__.py
--rw-r--r--   0        0        0     5167 2024-05-21 10:16:22.735355 kerykeion-4.6.2/kerykeion/charts/charts_utils.py
--rwxr-xr-x   0        0        0    64764 2024-05-21 11:01:53.142967 kerykeion-4.6.2/kerykeion/charts/kerykeion_chart_svg.py
--rwxr-xr-x   0        0        0    69874 2024-03-05 19:18:31.416341 kerykeion-4.6.2/kerykeion/charts/templates/chart.xml
--rw-r--r--   0        0        0      965 2024-05-13 20:03:16.436187 kerykeion-4.6.2/kerykeion/enums.py
--rw-r--r--   0        0        0     4444 2024-05-20 21:44:34.777442 kerykeion-4.6.2/kerykeion/fetch_geonames.py
--rw-r--r--   0        0        0      295 2024-05-20 21:44:34.777647 kerykeion-4.6.2/kerykeion/kr_types/__init__.py
--rw-r--r--   0        0        0     1945 2024-03-05 19:18:31.416709 kerykeion-4.6.2/kerykeion/kr_types/chart_types.py
--rw-r--r--   0        0        0      314 2024-05-20 21:44:34.777837 kerykeion-4.6.2/kerykeion/kr_types/kerykeion_exception.py
--rw-r--r--   0        0        0     1267 2024-05-20 21:44:34.778024 kerykeion-4.6.2/kerykeion/kr_types/kr_literals.py
--rw-r--r--   0        0        0     4260 2024-05-20 21:44:34.778212 kerykeion-4.6.2/kerykeion/kr_types/kr_models.py
--rw-r--r--   0        0        0    12743 2024-05-20 21:44:34.778431 kerykeion-4.6.2/kerykeion/kr_types/settings_models.py
--rw-r--r--   0        0        0     6794 2024-05-20 21:44:34.778633 kerykeion-4.6.2/kerykeion/relationship_score.py
--rw-r--r--   0        0        0     2565 2024-03-05 19:18:31.417278 kerykeion-4.6.2/kerykeion/report.py
--rw-r--r--   0        0        0       69 2024-03-05 19:18:31.417375 kerykeion-4.6.2/kerykeion/settings/__init__.py
--rw-r--r--   0        0        0     2347 2024-05-20 21:44:34.778844 kerykeion-4.6.2/kerykeion/settings/kerykeion_settings.py
--rw-r--r--   0        0        0    12282 2024-03-05 19:18:31.417645 kerykeion-4.6.2/kerykeion/settings/kr.config.json
--rw-r--r--   0        0        0       73 2024-03-05 19:18:31.417768 kerykeion-4.6.2/kerykeion/sweph/README.md
--rw-r--r--   0        0        0   223002 2024-03-05 19:18:31.418653 kerykeion-4.6.2/kerykeion/sweph/seas_18.se1
--rw-r--r--   0        0        0    10822 2024-05-20 21:44:34.779112 kerykeion-4.6.2/kerykeion/utilities.py
--rw-r--r--   0        0        0     2354 2024-05-21 11:02:19.022293 kerykeion-4.6.2/pyproject.toml
--rw-r--r--   0        0        0    10311 1970-01-01 00:00:00.000000 kerykeion-4.6.2/PKG-INFO
+-rw-r--r--   0        0        0    34273 2024-03-05 19:55:06.854597 kerykeion-4.7.0/LICENSE
+-rw-r--r--   0        0        0     8634 2024-03-05 19:55:06.855014 kerykeion-4.7.0/README.md
+-rw-r--r--   0        0        0     3917 2024-05-20 21:44:34.775470 kerykeion-4.7.0/kerykeion/__init__.py
+-rw-r--r--   0        0        0      293 2024-05-20 21:44:34.775703 kerykeion-4.7.0/kerykeion/aspects/__init__.py
+-rw-r--r--   0        0        0     5832 2024-05-28 15:08:25.859576 kerykeion-4.7.0/kerykeion/aspects/aspects_utils.py
+-rw-r--r--   0        0        0     4507 2024-05-28 22:30:25.470279 kerykeion-4.7.0/kerykeion/aspects/natal_aspects.py
+-rw-r--r--   0        0        0     3993 2024-05-28 15:08:25.860557 kerykeion-4.7.0/kerykeion/aspects/synastry_aspects.py
+-rw-r--r--   0        0        0    22965 2024-05-28 15:08:25.860953 kerykeion-4.7.0/kerykeion/astrological_subject.py
+-rw-r--r--   0        0        0      127 2024-05-28 15:08:25.861449 kerykeion-4.7.0/kerykeion/charts/__init__.py
+-rw-r--r--   0        0        0    13214 2024-05-30 16:08:23.762869 kerykeion-4.7.0/kerykeion/charts/charts_utils.py
+-rwxr-xr-x   0        0        0    60991 2024-05-30 17:17:29.928702 kerykeion-4.7.0/kerykeion/charts/kerykeion_chart_svg.py
+-rwxr-xr-x   0        0        0    70156 2024-05-28 10:50:49.385502 kerykeion-4.7.0/kerykeion/charts/templates/chart.xml
+-rw-r--r--   0        0        0      965 2024-05-13 20:03:16.436187 kerykeion-4.7.0/kerykeion/enums.py
+-rw-r--r--   0        0        0     4444 2024-05-28 15:08:25.862483 kerykeion-4.7.0/kerykeion/fetch_geonames.py
+-rw-r--r--   0        0        0      295 2024-05-20 21:44:34.777647 kerykeion-4.7.0/kerykeion/kr_types/__init__.py
+-rw-r--r--   0        0        0     2169 2024-05-28 21:56:30.572998 kerykeion-4.7.0/kerykeion/kr_types/chart_types.py
+-rw-r--r--   0        0        0      314 2024-05-20 21:44:34.777837 kerykeion-4.7.0/kerykeion/kr_types/kerykeion_exception.py
+-rw-r--r--   0        0        0     1267 2024-05-28 15:08:25.862785 kerykeion-4.7.0/kerykeion/kr_types/kr_literals.py
+-rw-r--r--   0        0        0     4260 2024-05-20 21:44:34.778212 kerykeion-4.7.0/kerykeion/kr_types/kr_models.py
+-rw-r--r--   0        0        0    12683 2024-05-28 21:45:15.274033 kerykeion-4.7.0/kerykeion/kr_types/settings_models.py
+-rw-r--r--   0        0        0     6794 2024-05-28 15:08:25.864025 kerykeion-4.7.0/kerykeion/relationship_score.py
+-rw-r--r--   0        0        0     2565 2024-05-28 15:08:25.864441 kerykeion-4.7.0/kerykeion/report.py
+-rw-r--r--   0        0        0       69 2024-03-05 19:18:31.417375 kerykeion-4.7.0/kerykeion/settings/__init__.py
+-rw-r--r--   0        0        0     2347 2024-05-28 15:08:25.864793 kerykeion-4.7.0/kerykeion/settings/kerykeion_settings.py
+-rw-r--r--   0        0        0    12282 2024-05-30 16:45:50.478222 kerykeion-4.7.0/kerykeion/settings/kr.config.json
+-rw-r--r--   0        0        0       73 2024-03-05 19:18:31.417768 kerykeion-4.7.0/kerykeion/sweph/README.md
+-rw-r--r--   0        0        0   223002 2024-03-05 19:18:31.418653 kerykeion-4.7.0/kerykeion/sweph/seas_18.se1
+-rw-r--r--   0        0        0    10822 2024-05-28 15:08:25.865121 kerykeion-4.7.0/kerykeion/utilities.py
+-rw-r--r--   0        0        0     2354 2024-05-30 17:18:39.151832 kerykeion-4.7.0/pyproject.toml
+-rw-r--r--   0        0        0    10311 1970-01-01 00:00:00.000000 kerykeion-4.7.0/PKG-INFO
```

### Comparing `kerykeion-4.6.2/LICENSE` & `kerykeion-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.2/README.md` & `kerykeion-4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.2/kerykeion/__init__.py` & `kerykeion-4.7.0/kerykeion/__init__.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.2/kerykeion/aspects/aspects_utils.py` & `kerykeion-4.7.0/kerykeion/aspects/aspects_utils.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.2/kerykeion/aspects/natal_aspects.py` & `kerykeion-4.7.0/kerykeion/aspects/natal_aspects.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.2/kerykeion/aspects/synastry_aspects.py` & `kerykeion-4.7.0/kerykeion/aspects/synastry_aspects.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.2/kerykeion/astrological_subject.py` & `kerykeion-4.7.0/kerykeion/astrological_subject.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.2/kerykeion/charts/kerykeion_chart_svg.py` & `kerykeion-4.7.0/kerykeion/charts/kerykeion_chart_svg.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 # -*- coding: utf-8 -*-
 """
     This is part of Kerykeion (C) 2024 Giacomo Battaglia
 """
 
 
-import pytz
 import logging
 
-from datetime import datetime
 from kerykeion.settings.kerykeion_settings import get_settings
 from kerykeion.aspects.synastry_aspects import SynastryAspects
 from kerykeion.aspects.natal_aspects import NatalAspects
 from kerykeion.astrological_subject import AstrologicalSubject
 from kerykeion.kr_types import KerykeionException, ChartType
 from kerykeion.kr_types import ChartTemplateDictionary
-from kerykeion.charts.charts_utils import decHourJoin, degreeDiff, offsetToTz, sliceToX, sliceToY, draw_zodiac_slice
+from kerykeion.kr_types.settings_models import KerykeionSettingsCelestialPointModel
+from kerykeion.charts.charts_utils import (
+    degreeDiff, 
+    sliceToX, 
+    sliceToY, 
+    draw_zodiac_slice, 
+    convert_latitude_coordinate_to_string, 
+    convert_longitude_coordinate_to_string,
+    draw_aspect_line,
+    draw_elements_percentages,
+    convert_decimal_to_degree_string,
+    draw_transit_ring_degree_steps,
+    draw_degree_ring,
+    draw_transit_ring
+)
 from pathlib import Path
 from string import Template
-from typing import Union
+from typing import Union, List
 
 
 class KerykeionChartSVG:
     """
     Creates the instance that can generate the chart with the
     function makeSVG().
 
@@ -30,21 +42,62 @@
         - chart_type: Natal, ExternalNatal, Transit, Synastry (Default: Type="Natal").
         - second_obj: Second kerykeion object (Not required if type is Natal)
         - new_output_directory: Set the output directory (default: output_directory)
         - lang: language settings (default: "EN")
         - new_settings_file: Set the settings file (default: kr.config.json)
     """
 
+    # Set at init
     first_obj: AstrologicalSubject
     second_obj: Union[AstrologicalSubject, None]
     chart_type: ChartType
     new_output_directory: Union[Path, None]
     new_settings_file: Union[Path, None]
     output_directory: Path
 
+    # Internal properties
+    fire: float
+    earth: float
+    air: float
+    water: float
+    c1: float
+    c2: float
+    c3: float
+    homedir: Path
+    xml_svg: Path
+    natal_width: float
+    full_width: float
+    language_settings: dict
+    chart_colors_settings: dict
+    planets_settings: dict
+    aspects_settings: dict
+    planet_in_zodiac_extra_points: int
+    chart_settings: dict
+    user: AstrologicalSubject
+    available_planets_setting: List[KerykeionSettingsCelestialPointModel]
+    transit_ring_exclude_points_names: List[str]
+    points_deg_ut: list
+    points_deg: list
+    points_sign: list
+    points_retrograde: list
+    houses_sign_graph: list
+    t_points_deg_ut: list
+    t_points_deg: list
+    t_points_sign: list
+    t_points_retrograde: list
+    t_houses_sign_graph: list
+    screen_width: float
+    screen_height: float
+    location: str
+    geolat: float
+    geolon: float
+    zoom: int
+    zodiac: tuple
+    template: str
+
     def __init__(
         self,
         first_obj: AstrologicalSubject,
         chart_type: ChartType = "Natal",
         second_obj: Union[AstrologicalSubject, None] = None,
         new_output_directory: Union[str, None] = None,
         new_settings_file: Union[Path, None] = None,
@@ -73,15 +126,31 @@
 
         self.available_planets_setting = []
         for body in self.planets_settings:
             if body['is_active'] == False:
                 continue
 
             self.available_planets_setting.append(body)
-            
+
+        # House cusp points are excluded from the transit ring.
+        self.transit_ring_exclude_points_names = [
+            "First_House",
+            "Second_House",
+            "Third_House",
+            "Fourth_House",
+            "Fifth_House",
+            "Sixth_House",
+            "Seventh_House",
+            "Eighth_House",
+            "Ninth_House",
+            "Tenth_House",
+            "Eleventh_House",
+            "Twelfth_House"
+        ]
+
         # Available bodies
         available_celestial_points = []
         for body in self.available_planets_setting:
             available_celestial_points.append(body["name"].lower())
         
         # Make a list for the absolute degrees of the points of the graphic.
         self.points_deg_ut = []
@@ -148,65 +217,23 @@
         # screen size
         if self.chart_type == "Natal":
             self.screen_width = 772.2
         else:
             self.screen_width = 1200
         self.screen_height = 772.2
 
-        # check for home
-        self.home_location = self.user.city
-        self.home_geolat = self.user.lat
-        self.home_geolon = self.user.lng
-        self.home_countrycode = self.user.nation
-        self.home_timezonestr = self.user.tz_str
-
-        logging.info(f"{self.user.name} birth location: {self.home_location}, {self.home_geolat}, {self.home_geolon}")
-
         # default location
-        self.location = self.home_location
-        self.geolat = float(self.home_geolat)
-        self.geolon = float(self.home_geolon)
-        self.countrycode = self.home_countrycode
-        self.timezonestr = self.home_timezonestr
-
-        # current datetime
-        now = datetime.now()
-
-        # aware datetime object
-        dt_input = datetime(now.year, now.month, now.day, now.hour, now.minute, now.second)
-        dt = pytz.timezone(self.timezonestr).localize(dt_input)
-
-        # naive utc datetime object
-        dt_utc = dt.replace(tzinfo=None) - dt.utcoffset()  # type: ignore
-
-        # Default
-        self.name = self.user.name
-        self.charttype = self.chart_type
-        self.year = self.user.utc.year
-        self.month = self.user.utc.month
-        self.day = self.user.utc.day
-        self.hour = self.user.utc.hour + self.user.utc.minute / 100
-        self.timezone = offsetToTz(dt.utcoffset())
-        self.altitude = 25
-        self.geonameid = None
-
-        # Transit
+        self.location = self.user.city
+        self.geolat = self.user.lat
+        self.geolon =  self.user.lng
+        
+        logging.info(f"{self.user.name} birth location: {self.location}, {self.geolat}, {self.geolon}")
 
         if self.chart_type == "Transit":
-            self.t_geolon = self.geolon
-            self.t_geolat = self.geolat
-            self.t_altitude = self.altitude
             self.t_name = self.language_settings["transit_name"]
-            self.t_year = dt_utc.year
-            self.t_month = dt_utc.month
-            self.t_day = dt_utc.day
-            self.t_hour = decHourJoin(dt_utc.hour, dt_utc.minute, dt_utc.second)
-            self.t_timezone = offsetToTz(dt.utcoffset())
-            self.t_altitude = 25
-            self.t_geonameid = None
 
         # configuration
         # ZOOM 1 = 100%
         self.zoom = 1
 
         self.zodiac = (
             {"name": "aries", "element": "fire"},
@@ -243,138 +270,14 @@
         self.language_settings = settings["language_settings"].get(language, "EN")
         self.chart_colors_settings = settings["chart_colors"]
         self.planets_settings = settings["celestial_points"]
         self.aspects_settings = settings["aspects"]
         self.planet_in_zodiac_extra_points = settings["general_settings"]["planet_in_zodiac_extra_points"]
         self.chart_settings = settings["chart_settings"]
 
-    def _transitRing(self, r) -> str:
-        """
-        Draws the transit ring.
-        """
-        radius_offset = 18
-
-        out = f'<circle cx="{r}" cy="{r}" r="{r - radius_offset}" style="fill: none; stroke: {self.chart_colors_settings["paper_1"]}; stroke-width: 36px; stroke-opacity: .4;"/>'
-        out += f'<circle cx="{r}" cy="{r}" r="{r}" style="fill: none; stroke: {self.chart_colors_settings["zodiac_transit_ring_3"]}; stroke-width: 1px; stroke-opacity: .6;"/>'
-
-        return out
-
-    def _degreeRing(self, r) -> str:
-        """
-        Draws the degree ring.
-        """
-        out = ""
-        for i in range(72):
-            offset = float(i * 5) - self.user.houses_degree_ut[6]
-            if offset < 0:
-                offset = offset + 360.0
-            elif offset > 360:
-                offset = offset - 360.0
-            x1 = sliceToX(0, r - self.c1, offset) + self.c1
-            y1 = sliceToY(0, r - self.c1, offset) + self.c1
-            x2 = sliceToX(0, r + 2 - self.c1, offset) - 2 + self.c1
-            y2 = sliceToY(0, r + 2 - self.c1, offset) - 2 + self.c1
-
-            out += f'<line x1="{x1}" y1="{y1}" x2="{x2}" y2="{y2}" style="stroke: {self.chart_colors_settings["paper_0"]}; stroke-width: 1px; stroke-opacity:.9;"/>'
-
-        return out
-
-    def _degreeTransitRing(self, r):
-        out = ""
-        for i in range(72):
-            offset = float(i * 5) - self.user.houses_degree_ut[6]
-            if offset < 0:
-                offset = offset + 360.0
-            elif offset > 360:
-                offset = offset - 360.0
-            x1 = sliceToX(0, r, offset)
-            y1 = sliceToY(0, r, offset)
-            x2 = sliceToX(0, r + 2, offset) - 2
-            y2 = sliceToY(0, r + 2, offset) - 2
-            out += f'<line x1="{x1}" y1="{y1}" x2="{x2}" y2="{y2}" style="stroke: #F00; stroke-width: 1px; stroke-opacity:.9;"/>'
-
-        return out
-
-    def _lat2str(self, coord):
-        """Converts a floating point latitude to string with
-        degree, minutes and seconds and the appropriate sign
-        (north or south). Eg. 52.1234567 -> 52°7'25" N
-
-        Args:
-            coord (float): latitude in floating point format
-        Returns:
-            str: latitude in string format with degree, minutes,
-             seconds and sign (N/S)
-        """
-
-        sign = self.language_settings["north"]
-        if coord < 0.0:
-            sign = self.language_settings["south"]
-            coord = abs(coord)
-        deg = int(coord)
-        min = int((float(coord) - deg) * 60)
-        sec = int(round(float(((float(coord) - deg) * 60) - min) * 60.0))
-        return f"{deg}°{min}'{sec}\" {sign}"
-
-    def _lon2str(self, coord):
-        """Converts a floating point longitude to string with
-        degree, minutes and seconds and the appropriate sign
-        (east or west). Eg. 52.1234567 -> 52°7'25" E
-
-        Args:
-            coord (float): longitude in floating point format
-        Returns:
-            str: longitude in string format with degree, minutes,
-                seconds and sign (E/W)
-        """
-
-        sign = self.language_settings["east"]
-        if coord < 0.0:
-            sign = self.language_settings["west"]
-            coord = abs(coord)
-        deg = int(coord)
-        min = int((float(coord) - deg) * 60)
-        sec = int(round(float(((float(coord) - deg) * 60) - min) * 60.0))
-        return f"{deg}°{min}'{sec}\" {sign}"
-
-    def _dec2deg(self, dec, type="3"):
-        """Coverts decimal float to degrees in format
-        a°b'c".
-        """
-
-        dec = float(dec)
-        a = int(dec)
-        a_new = (dec - float(a)) * 60.0
-        b_rounded = int(round(a_new))
-        b = int(a_new)
-        c = int(round((a_new - float(b)) * 60.0))
-        if type == "3":
-            out = f"{a:02d}&#176;{b:02d}&#39;{c:02d}&#34;"
-        elif type == "2":
-            out = f"{a:02d}&#176;{b_rounded:02d}&#39;"
-        elif type == "1":
-            out = f"{a:02d}&#176;"
-        else:
-            raise KerykeionException(f"Wrong type: {type}, it must be 1, 2 or 3.")
-        return str(out)
-
-    def _drawAspect(self, r, ar, degA, degB, color):
-        """
-        Draws svg aspects: ring, aspect ring, degreeA degreeB
-        """
-        offset = (int(self.user.houses_degree_ut[6]) / -1) + int(degA)
-        x1 = sliceToX(0, ar, offset) + (r - ar)
-        y1 = sliceToY(0, ar, offset) + (r - ar)
-        offset = (int(self.user.houses_degree_ut[6]) / -1) + int(degB)
-        x2 = sliceToX(0, ar, offset) + (r - ar)
-        y2 = sliceToY(0, ar, offset) + (r - ar)
-        out = f'            <line x1="{x1}" y1="{y1}" x2="{x2}" y2="{y2}" style="stroke: {color}; stroke-width: 1; stroke-opacity: .9;"/>'
-
-        return out
-
     def _draw_zodiac_circle_slices(self, r):
         """
         Generate the SVG string representing the zodiac circle
         with the 12 slices for each zodiac sign.
 
         Args:
             r (float): The radius of the zodiac slices.
@@ -384,15 +287,15 @@
         """
 
         output = ""
         for i, zodiac_element in enumerate(self.zodiac):
             output += draw_zodiac_slice(
                 c1=self.c1,
                 chart_type=self.chart_type,
-                sixth_house_degree_ut=self.user.houses_degree_ut[6],
+                seventh_house_degree_ut=self.user.houses_degree_ut[6],
                 num=i,
                 r=r,
                 style=f'fill:{self.chart_colors_settings[f"zodiac_bg_{i}"]}; fill-opacity: 0.5;',
                 type=zodiac_element["name"],
             )
 
         return output
@@ -480,52 +383,58 @@
             xtext = sliceToX(0, (r - dropin), text_offset) + dropin  # was 132
             ytext = sliceToY(0, (r - dropin), text_offset) + dropin  # was 132
             path = f'{path}<line x1="{x1}" y1="{y1}" x2="{x2}" y2="{y2}" style="stroke: {linecolor}; stroke-width: 2px; stroke-dasharray:3,2; stroke-opacity:.4;"/>'
             path = path + '<text style="fill: #f00; fill-opacity: .6; font-size: 14px"><tspan x="' + str(xtext - 3) + '" y="' + str(ytext + 3) + '">' + str(i + 1) + "</tspan></text>"
 
         return path
 
-    def _value_element_from_planet(self, i):
+    def _calculate_elements_points_from_planets(self):
         """
         Calculate chart element points from a planet.
         """
+        
+        for i in range(len(self.available_planets_setting)):
+            # element: get extra points if planet is in own zodiac sign.
+            related_zodiac_signs = self.available_planets_setting[i]["related_zodiac_signs"]
+            cz = self.points_sign[i]
+            extra_points = 0
+            if related_zodiac_signs != []:
+                for e in range(len(related_zodiac_signs)):
+                    if int(related_zodiac_signs[e]) == int(cz):
+                        extra_points = self.planet_in_zodiac_extra_points
+
+            ele = self.zodiac[self.points_sign[i]]["element"]
+            if ele == "fire":
+                self.fire = self.fire + self.available_planets_setting[i]["element_points"] + extra_points
 
-        # element: get extra points if planet is in own zodiac sign.
-        related_zodiac_signs = self.available_planets_setting[i]["related_zodiac_signs"]
-        cz = self.points_sign[i]
-        extra_points = 0
-        if related_zodiac_signs != []:
-            for e in range(len(related_zodiac_signs)):
-                if int(related_zodiac_signs[e]) == int(cz):
-                    extra_points = self.planet_in_zodiac_extra_points
-
-        ele = self.zodiac[self.points_sign[i]]["element"]
-        if ele == "fire":
-            self.fire = self.fire + self.available_planets_setting[i]["element_points"] + extra_points
-
-        elif ele == "earth":
-            self.earth = self.earth + self.available_planets_setting[i]["element_points"] + extra_points
+            elif ele == "earth":
+                self.earth = self.earth + self.available_planets_setting[i]["element_points"] + extra_points
 
-        elif ele == "air":
-            self.air = self.air + self.available_planets_setting[i]["element_points"] + extra_points
+            elif ele == "air":
+                self.air = self.air + self.available_planets_setting[i]["element_points"] + extra_points
 
-        elif ele == "water":
-            self.water = self.water + self.available_planets_setting[i]["element_points"] + extra_points
+            elif ele == "water":
+                self.water = self.water + self.available_planets_setting[i]["element_points"] + extra_points
 
     def _make_planets(self, r):
         planets_degut = {}
         diff = range(len(self.available_planets_setting))
 
         for i in range(len(self.available_planets_setting)):
-            if self.available_planets_setting[i]["is_active"] == 1:
-                # list of planets sorted by degree
-                logging.debug(f"planet: {i}, degree: {self.points_deg_ut[i]}")
-                planets_degut[self.points_deg_ut[i]] = i
+            # list of planets sorted by degree
+            logging.debug(f"planet: {i}, degree: {self.points_deg_ut[i]}")
+            planets_degut[self.points_deg_ut[i]] = i
 
-            self._value_element_from_planet(i)
+        """
+        FIXME: The planets_degut is a dictionary like:
+        {planet_degree: planet_index}
+        It should be replaced bu points_deg_ut
+        print(self.points_deg_ut)
+        print(planets_degut)
+        """
 
         output = ""
         keys = list(planets_degut.keys())
         keys.sort()
         switch = 0
 
         planets_degrouped = {}
@@ -699,22 +608,23 @@
             # output planet
             output += f'<g transform="translate(-{12 * scale},-{12 * scale})"><g transform="scale({scale})"><use x="{planet_x * (1/scale)}" y="{planet_y * (1/scale)}" xlink:href="#{self.available_planets_setting[i]["name"]}" /></g></g>'
 
         # make transit degut and display planets
         if self.chart_type == "Transit" or self.chart_type == "Synastry":
             group_offset = {}
             t_planets_degut = {}
-            if self.chart_type == "Transit":
-                list_range = len(self.available_planets_setting) - 4
-            else:
-                list_range = len(self.available_planets_setting)
+            list_range = len(self.available_planets_setting)
+
             for i in range(list_range):
+                if self.chart_type == "Transit" and self.available_planets_setting[i]['name'] in self.transit_ring_exclude_points_names:
+                    continue
+                
                 group_offset[i] = 0
-                if self.available_planets_setting[i]["is_active"] == 1:
-                    t_planets_degut[self.t_points_deg_ut[i]] = i
+                t_planets_degut[self.t_points_deg_ut[i]] = i
+        
             t_keys = list(t_planets_degut.keys())
             t_keys.sort()
 
             # grab closely grouped planets
             groups = []
             in_group = False
             for e in range(len(t_keys)):
@@ -748,40 +658,46 @@
                 elif len(groups[i]) == 4:
                     group_offset[groups[i][0]] = -2.0
                     group_offset[groups[i][1]] = -1.0
                     group_offset[groups[i][2]] = 1.0
                     group_offset[groups[i][3]] = 2.0
 
             switch = 0
+            
+            # Transit planets loop
             for e in range(len(t_keys)):
+                if self.chart_type == "Transit" and self.available_planets_setting[e]["name"] in self.transit_ring_exclude_points_names:
+                    continue
+
                 i = t_planets_degut[t_keys[e]]
 
                 if 22 < i < 27:
                     rplanet = 9
                 elif switch == 1:
                     rplanet = 18
                     switch = 0
                 else:
                     rplanet = 26
                     switch = 1
 
+                # Transit planet name
                 zeropoint = 360 - self.user.houses_degree_ut[6]
                 t_offset = zeropoint + self.t_points_deg_ut[i]
                 if t_offset > 360:
                     t_offset = t_offset - 360
                 planet_x = sliceToX(0, (r - rplanet), t_offset) + rplanet
                 planet_y = sliceToY(0, (r - rplanet), t_offset) + rplanet
-                output += f'<g transform="translate(-6,-6)"><g transform="scale(0.5)"><use x="{planet_x*2}" y="{planet_y*2}" xlink:href="#{self.available_planets_setting[i]["name"]}" /></g></g>'
+                output += f'<g class="transit-planet-name" transform="translate(-6,-6)"><g transform="scale(0.5)"><use x="{planet_x*2}" y="{planet_y*2}" xlink:href="#{self.available_planets_setting[i]["name"]}" /></g></g>'
 
-                # transit planet line
+                # Transit planet line
                 x1 = sliceToX(0, r + 3, t_offset) - 3
                 y1 = sliceToY(0, r + 3, t_offset) - 3
                 x2 = sliceToX(0, r - 3, t_offset) + 3
                 y2 = sliceToY(0, r - 3, t_offset) + 3
-                output += f'<line x1="{str(x1)}" y1="{str(y1)}" x2="{str(x2)}" y2="{str(y2)}" style="stroke: {self.available_planets_setting[i]["color"]}; stroke-width: 1px; stroke-opacity:.8;"/>'
+                output += f'<line class="transit-planet-line" x1="{str(x1)}" y1="{str(y1)}" x2="{str(x2)}" y2="{str(y2)}" style="stroke: {self.available_planets_setting[i]["color"]}; stroke-width: 1px; stroke-opacity:.8;"/>'
 
                 # transit planet degree text
                 rotate = self.user.houses_degree_ut[0] - self.t_points_deg_ut[i]
                 textanchor = "end"
                 t_offset += group_offset[i]
                 rtext = -3.0
 
@@ -797,15 +713,15 @@
                 else:
                     xo = -1
                 deg_x = sliceToX(0, (r - rtext), t_offset + xo) + rtext
                 deg_y = sliceToY(0, (r - rtext), t_offset + xo) + rtext
                 degree = int(t_offset)
                 output += f'<g transform="translate({deg_x},{deg_y})">'
                 output += f'<text transform="rotate({rotate})" text-anchor="{textanchor}'
-                output += f'" style="fill: {self.available_planets_setting[i]["color"]}; font-size: 10px;">{self._dec2deg(self.t_points_deg[i], type="1")}'
+                output += f'" style="fill: {self.available_planets_setting[i]["color"]}; font-size: 10px;">{convert_decimal_to_degree_string(self.t_points_deg[i], type="1")}'
                 output += "</text></g>"
 
             # check transit
             if self.chart_type == "Transit" or self.chart_type == "Synastry":
                 dropin = 36
             else:
                 dropin = 0
@@ -979,20 +895,21 @@
         # return out
         return ""
 
     # Aspect and aspect grid functions for natal type charts.
     def _makeAspects(self, r, ar):
         out = ""
         for element in self.aspects_list:
-            out += self._drawAspect(
-                r,
-                ar,
-                element["p1_abs_pos"],
-                element["p2_abs_pos"],
-                self.aspects_settings[element["aid"]]["color"],
+            out += draw_aspect_line(
+                r=r,
+                ar=ar,
+                degA=element["p1_abs_pos"],
+                degB=element["p2_abs_pos"],
+                color=self.aspects_settings[element["aid"]]["color"],
+                seventh_house_degree_ut=self.user.seventh_house.abs_pos
             )
 
         return out
 
     def _makeAspectGrid(self, r):
         out = ""
         style = "stroke:%s; stroke-width: 1px; stroke-opacity:.6; fill:none" % (self.chart_colors_settings["paper_0"])
@@ -1000,48 +917,47 @@
         yindent = 468
         box = 14
         revr = list(range(len(self.available_planets_setting)))
         revr.reverse()
         counter = 0
         for a in revr:
             counter += 1
-            if self.available_planets_setting[a]["is_active"] == 1:
-                out += f'<rect x="{xindent}" y="{yindent}" width="{box}" height="{box}" style="{style}"/>'
-                out += f'<use transform="scale(0.4)" x="{(xindent+2)*2.5}" y="{(yindent+1)*2.5}" xlink:href="#{self.available_planets_setting[a]["name"]}" />'
-
-                xindent = xindent + box
-                yindent = yindent - box
-                revr2 = list(range(a))
-                revr2.reverse()
-                xorb = xindent
-                yorb = yindent + box
-                for b in revr2:
-                    if self.available_planets_setting[b]["is_active"] == 1:
-                        out += f'<rect x="{xorb}" y="{yorb}" width="{box}" height="{box}" style="{style}"/>'
-
-                        xorb = xorb + box
-                        for element in self.aspects_list:
-                            if (element["p1"] == a and element["p2"] == b) or (element["p1"] == b and element["p2"] == a):
-                                out += f'<use  x="{xorb-box+1}" y="{yorb+1}" xlink:href="#orb{element["aspect_degrees"]}" />'
+            out += f'<rect x="{xindent}" y="{yindent}" width="{box}" height="{box}" style="{style}"/>'
+            out += f'<use transform="scale(0.4)" x="{(xindent+2)*2.5}" y="{(yindent+1)*2.5}" xlink:href="#{self.available_planets_setting[a]["name"]}" />'
+
+            xindent = xindent + box
+            yindent = yindent - box
+            revr2 = list(range(a))
+            revr2.reverse()
+            xorb = xindent
+            yorb = yindent + box
+            for b in revr2:
+                out += f'<rect x="{xorb}" y="{yorb}" width="{box}" height="{box}" style="{style}"/>'
+
+                xorb = xorb + box
+                for element in self.aspects_list:
+                    if (element["p1"] == a and element["p2"] == b) or (element["p1"] == b and element["p2"] == a):
+                        out += f'<use  x="{xorb-box+1}" y="{yorb+1}" xlink:href="#orb{element["aspect_degrees"]}" />'
 
         return out
 
     # Aspect and aspect grid functions for transit type charts
     def _makeAspectsTransit(self, r, ar):
         out = ""
 
         self.aspects_list = SynastryAspects(self.user, self.t_user, new_settings_file=self.new_settings_file).relevant_aspects
 
         for element in self.aspects_list:
-            out += self._drawAspect(
-                r,
-                ar,
-                element["p1_abs_pos"],
-                element["p2_abs_pos"],
-                self.aspects_settings[element["aid"]]["color"],
+            out += draw_aspect_line(
+                r=r,
+                ar=ar,
+                degA=element["p1_abs_pos"],
+                degB=element["p2_abs_pos"],
+                color=self.aspects_settings[element["aid"]]["color"],
+                seventh_house_degree_ut=self.user.seventh_house.abs_pos
             )
 
         return out
 
     def _makeAspectTransitGrid(self, r):
         out = '<g transform="translate(500,310)">'
         out += f'<text y="-15" x="0" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 14px;">{self.language_settings["aspects"]}:</text>'
@@ -1084,44 +1000,28 @@
             
             # second planet symbol
             out += '<g transform="translate(30,0)">'
             out += '<use transform="scale(0.4)" x="0" y="3" xlink:href="#%s" />' % (self.planets_settings[self.aspects_list[i]["p2"]]["name"]) 
             
             out += "</g>"
             # difference in degrees
-            out += f'<text y="8" x="45" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;">{self._dec2deg(self.aspects_list[i]["orbit"])}</text>'
+            out += f'<text y="8" x="45" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;">{convert_decimal_to_degree_string(self.aspects_list[i]["orbit"])}</text>'
             # line
             out += "</g>"
             line = line + 14
         out += "</g>"
         return out
 
-    def _makeElements(self, r):
-        total = self.fire + self.earth + self.air + self.water
-        pf = int(round(100 * self.fire / total))
-        pe = int(round(100 * self.earth / total))
-        pa = int(round(100 * self.air / total))
-        pw = int(round(100 * self.water / total))
-
-        out = '<g transform="translate(-30,79)">'
-        out += f'<text y="0" style="fill:#ff6600; font-size: 10px;">{self.language_settings["fire"]}  {str(pf)}%</text>'
-        out += f'<text y="12" style="fill:#6a2d04; font-size: 10px;">{self.language_settings["earth"]} {str(pe)}%</text>'
-        out += f'<text y="24" style="fill:#6f76d1; font-size: 10px;">{self.language_settings["air"]}   {str(pa)}%</text>'
-        out += f'<text y="36" style="fill:#630e73; font-size: 10px;">{self.language_settings["water"]} {str(pw)}%</text>'
-        out += "</g>"
-
-        return out
-
     def _makePlanetGrid(self):
         li = 10
         offset = 0
 
         out = '<g transform="translate(500,-20)">'
         out += '<g transform="translate(140, -15)">'
-        out += f'<text text-anchor="end" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 14px;">{self.language_settings["planets_and_house"]} {self.name}:</text>'
+        out += f'<text text-anchor="end" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 14px;">{self.language_settings["planets_and_house"]} {self.user.name}:</text>'
         out += "</g>"
 
         end_of_line = None
         for i in range(len(self.available_planets_setting)):
             offset_between_lines = 14
             end_of_line = "</g>"
 
@@ -1136,15 +1036,15 @@
             # planet text
             out += f'<text text-anchor="end" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;">{self.language_settings["celestial_points"][self.available_planets_setting[i]["label"]]}</text>'
 
             # planet symbol
             out += f'<g transform="translate(5,-8)"><use transform="scale(0.4)" xlink:href="#{self.available_planets_setting[i]["name"]}" /></g>'
 
             # planet degree
-            out += f'<text text-anchor="start" x="19" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;">{self._dec2deg(self.points_deg[i])}</text>'
+            out += f'<text text-anchor="start" x="19" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;">{convert_decimal_to_degree_string(self.points_deg[i])}</text>'
 
             # zodiac
             out += f'<g transform="translate(60,-8)"><use transform="scale(0.3)" xlink:href="#{self.zodiac[self.points_sign[i]]["name"]}" /></g>'
 
             # planet retrograde
             if self.points_retrograde[i]:
                 out += '<g transform="translate(74,-6)"><use transform="scale(.5)" xlink:href="#retrograde" /></g>'
@@ -1168,55 +1068,60 @@
             t_offset = 250
 
             for i in range(len(self.available_planets_setting)):
                 if i == 27:
                     t_li = 10
                     t_offset = -120
 
-                if self.available_planets_setting[i]["is_active"] == 1:
-                    # start of line
-                    out += f'<g transform="translate({t_offset},{t_li})">'
-
-                    # planet text
-                    out += f'<text text-anchor="end" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;">{self.language_settings["celestial_points"][self.available_planets_setting[i]["label"]]}</text>'
-                    # planet symbol
-                    out += f'<g transform="translate(5,-8)"><use transform="scale(0.4)" xlink:href="#{self.available_planets_setting[i]["name"]}" /></g>'
-                    # planet degree
-                    out += f'<text text-anchor="start" x="19" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;">{self._dec2deg(self.t_points_deg[i])}</text>'
-                    # zodiac
-                    out += f'<g transform="translate(60,-8)"><use transform="scale(0.3)" xlink:href="#{self.zodiac[self.t_points_sign[i]]["name"]}" /></g>'
-
-                    # planet retrograde
-                    if self.t_points_retrograde[i]:
-                        out += '<g transform="translate(74,-6)"><use transform="scale(.5)" xlink:href="#retrograde" /></g>'
+                # start of line
+                out += f'<g transform="translate({t_offset},{t_li})">'
+
+                # planet text
+                out += f'<text text-anchor="end" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;">{self.language_settings["celestial_points"][self.available_planets_setting[i]["label"]]}</text>'
+                # planet symbol
+                out += f'<g transform="translate(5,-8)"><use transform="scale(0.4)" xlink:href="#{self.available_planets_setting[i]["name"]}" /></g>'
+                # planet degree
+                out += f'<text text-anchor="start" x="19" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;">{convert_decimal_to_degree_string(self.t_points_deg[i])}</text>'
+                # zodiac
+                out += f'<g transform="translate(60,-8)"><use transform="scale(0.3)" xlink:href="#{self.zodiac[self.t_points_sign[i]]["name"]}" /></g>'
+
+                # planet retrograde
+                if self.t_points_retrograde[i]:
+                    out += '<g transform="translate(74,-6)"><use transform="scale(.5)" xlink:href="#retrograde" /></g>'
 
-                    # end of line
-                    out += end_of_line
+                # end of line
+                out += end_of_line
 
-                    t_li = t_li + offset_between_lines
+                t_li = t_li + offset_between_lines
 
         if end_of_line is None:
             raise KerykeionException("End of line not found")
 
         out += end_of_line
         return out
 
     def _draw_house_grid(self):
+        """
+        Generate SVG code for a grid of astrological houses.
+
+        Returns:
+            str: The SVG code for the grid of houses.
+        """
         out = '<g transform="translate(600,-20)">'
 
         li = 10
         for i in range(12):
             if i < 9:
                 cusp = "&#160;&#160;" + str(i + 1)
             else:
                 cusp = str(i + 1)
             out += f'<g transform="translate(0,{li})">'
             out += f'<text text-anchor="end" x="40" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;">{self.language_settings["cusp"]} {cusp}:</text>'
             out += f'<g transform="translate(40,-8)"><use transform="scale(0.3)" xlink:href="#{self.zodiac[self.houses_sign_graph[i]]["name"]}" /></g>'
-            out += f'<text x="53" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;"> {self._dec2deg(self.user.houses_list[i]["position"])}</text>'
+            out += f'<text x="53" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;"> {convert_decimal_to_degree_string(self.user.houses_list[i]["position"])}</text>'
             out += "</g>"
             li = li + 14
 
         out += "</g>"
 
         if self.chart_type == "Synastry":
             out += '<g transform="translate(840, -20)">'
@@ -1225,29 +1130,32 @@
                 if i < 9:
                     cusp = "&#160;&#160;" + str(i + 1)
                 else:
                     cusp = str(i + 1)
                 out += '<g transform="translate(0,' + str(li) + ')">'
                 out += f'<text text-anchor="end" x="40" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;">{self.language_settings["cusp"]} {cusp}:</text>'
                 out += f'<g transform="translate(40,-8)"><use transform="scale(0.3)" xlink:href="#{self.zodiac[self.t_houses_sign_graph[i]]["name"]}" /></g>'
-                out += f'<text x="53" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;"> {self._dec2deg(self.t_user.houses_list[i]["position"])}</text>'
+                out += f'<text x="53" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;"> {convert_decimal_to_degree_string(self.t_user.houses_list[i]["position"])}</text>'
                 out += "</g>"
                 li = li + 14
             out += "</g>"
 
         return out
 
     def _createTemplateDictionary(self) -> ChartTemplateDictionary:
         # self.chart_type = "Transit"
         # empty element points
         self.fire = 0.0
         self.earth = 0.0
         self.air = 0.0
         self.water = 0.0
 
+        # Calculate the elements points
+        self._calculate_elements_points_from_planets()
+
         # width and height from screen
         ratio = float(self.screen_width) / float(self.screen_height)
         if ratio < 1.3:  # 1280x1024
             wm_off = 130
         else:  # 1024x768, 800x600, 1280x800, 1680x1050
             wm_off = 100
 
@@ -1274,16 +1182,16 @@
         else:
             self.c1 = 0
             self.c2 = 36
             self.c3 = 120
 
         # transit
         if self.chart_type == "Transit" or self.chart_type == "Synastry":
-            td["transitRing"] = self._transitRing(r)
-            td["degreeRing"] = self._degreeTransitRing(r)
+            td["transitRing"] = draw_transit_ring(r, self.chart_colors_settings["paper_1"], self.chart_colors_settings["zodiac_transit_ring_3"])
+            td["degreeRing"] = draw_transit_ring_degree_steps(r, self.user.seventh_house.abs_pos)
 
             # circles
             td["c1"] = f'cx="{r}" cy="{r}" r="{r - 36}"'
             td["c1style"] = f'fill: none; stroke: {self.chart_colors_settings["zodiac_transit_ring_2"]}; stroke-width: 1px; stroke-opacity:.4;'
             td["c2"] = 'cx="' + str(r) + '" cy="' + str(r) + '" r="' + str(r - 72) + '"'
             td["c2style"] = f"fill: {self.chart_colors_settings['paper_1']}; fill-opacity:.4; stroke: {self.chart_colors_settings['zodiac_transit_ring_1']}; stroke-opacity:.4; stroke-width: 1px"
 
@@ -1292,15 +1200,15 @@
 
             td["makeAspects"] = self._makeAspectsTransit(r, (r - 160))
             td["makeAspectGrid"] = self._makeAspectTransitGrid(r)
             td["makePatterns"] = ""
             td["chart_width"] = self.full_width
         else:
             td["transitRing"] = ""
-            td["degreeRing"] = self._degreeRing(r)
+            td["degreeRing"] = draw_degree_ring(r, self.c1, self.user.seventh_house.abs_pos, self.chart_colors_settings["paper_0"])
 
             # circles
             td["c1"] = f'cx="{r}" cy="{r}" r="{r - self.c1}"'
             td["c1style"] = f'fill: none; stroke: {self.chart_colors_settings["zodiac_radix_ring_2"]}; stroke-width: 1px; '
             td["c2"] = f'cx="{r}" cy="{r}" r="{r - self.c2}"'
             td["c2style"] = f'fill: {self.chart_colors_settings["paper_1"]}; fill-opacity:.2; stroke: {self.chart_colors_settings["zodiac_radix_ring_1"]}; stroke-opacity:.4; stroke-width: 1px'
             td["c3"] = f'cx="{r}" cy="{r}" r="{r - self.c3}"'
@@ -1313,25 +1221,25 @@
         td["circleX"] = str(0)
         td["circleY"] = str(0)
         td["svgWidth"] = str(svgWidth)
         td["svgHeight"] = str(svgHeight)
         td["viewbox"] = viewbox
 
         if self.chart_type == "Synastry":
-            td["stringTitle"] = f"{self.name} {self.language_settings['and_word']} {self.t_user.name}"
+            td["stringTitle"] = f"{self.user.name} {self.language_settings['and_word']} {self.t_user.name}"
 
         elif self.chart_type == "Transit":
             td["stringTitle"] = f"{self.language_settings['transits']} {self.t_user.day}/{self.t_user.month}/{self.t_user.year}"
 
         else:
-            td["stringTitle"] = self.name
+            td["stringTitle"] = self.user.name
 
         # Tipo di carta
-        if self.chart_type == "Synastry" or self.name == "Transit":
-            td["stringName"] = f"{self.name}:"
+        if self.chart_type == "Synastry" or self.chart_type == "Transit":
+            td["stringName"] = f"{self.user.name}:"
         else:
             td["stringName"] = f'{self.language_settings["info"]}:'
 
         # bottom left
         td["bottomLeft1"] = ""
         td["bottomLeft2"] = ""
         td["bottomLeft3"] = f'{self.language_settings.get("lunar_phase", "Lunar Phase")}: {self.language_settings.get("day", "Day")} {self.user.lunar_phase.get("moon_phase", "")}'
@@ -1407,17 +1315,28 @@
 
         if self.chart_type == "Synastry":
             td["stringLat"] = f"{self.t_user.name}: "
             td["stringLon"] = self.t_user.city
             td["stringPosition"] = f"{self.t_user.year}-{self.t_user.month}-{self.t_user.day} {self.t_user.hour:02d}:{self.t_user.minute:02d}"
 
         else:
-            td["stringLat"] = f"{self.language_settings['latitude']}: {self._lat2str(self.geolat)}"
-            td["stringLon"] = f"{self.language_settings['longitude']}: {self._lon2str(self.geolon)}"
-            td["stringPosition"] = f"{self.language_settings['type']}: {self.charttype}"
+            latitude_string = convert_latitude_coordinate_to_string(
+                self.geolat, 
+                self.language_settings['north'], 
+                self.language_settings['south']
+            )
+            longitude_string = convert_longitude_coordinate_to_string(
+                self.geolon, 
+                self.language_settings['east'], 
+                self.language_settings['west']
+            )
+
+            td["stringLat"] = f"{self.language_settings['latitude']}: {latitude_string}"
+            td["stringLon"] = f"{self.language_settings['longitude']}: {longitude_string}"
+            td["stringPosition"] = f"{self.language_settings['type']}: {self.chart_type}"
 
         # paper_color_X
         td["paper_color_0"] = self.chart_colors_settings["paper_0"]
         td["paper_color_1"] = self.chart_colors_settings["paper_1"]
 
         # planets_color_X
         for i in range(len(self.planets_settings)):
@@ -1442,15 +1361,24 @@
         #--- 
 
         td["makeZodiac"] = self._draw_zodiac_circle_slices(r)
         td["makeHousesGrid"] = self._draw_house_grid()
         # TODO: Add the rest of the functions
         td["makeHouses"] = self._makeHouses(r)
         td["makePlanets"] = self._make_planets(r)
-        td["makeElements"] = self._makeElements(r)
+        td["elements_percentages"] = draw_elements_percentages(
+            self.language_settings['fire'],
+            self.fire,
+            self.language_settings['earth'],
+            self.earth,
+            self.language_settings['air'],
+            self.air,
+            self.language_settings['water'],
+            self.water,
+        )
         td["makePlanetGrid"] = self._makePlanetGrid()
 
         return td
 
     def makeTemplate(self):
         """Creates the template for the SVG file"""
         td = self._createTemplateDictionary()
@@ -1468,15 +1396,15 @@
 
     def makeSVG(self) -> None:
         """Prints out the SVG file in the specifide folder"""
 
         if not (self.template):
             self.template = self.makeTemplate()
 
-        self.chartname = self.output_directory / f"{self.name}{self.chart_type}Chart.svg"
+        self.chartname = self.output_directory / f"{self.user.name}{self.chart_type}Chart.svg"
 
         with open(self.chartname, "w", encoding="utf-8", errors="ignore") as output_file:
             output_file.write(self.template)
 
         logging.info(f"SVG Generated Correctly in: {self.chartname}")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kerykeion-4.6.2/kerykeion/charts/templates/chart.xml` & `kerykeion-4.7.0/kerykeion/charts/templates/chart.xml`

 * *Files 0% similar despite different names*

```diff
@@ -1,4368 +1,4385 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2731  <?xml version='1
 00000010: 2e30 2720 656e 636f 6469 6e67 3d27 5554  .0' encoding='UT
-00000020: 462d 3827 3f3e 0a3c 2144 4f43 5459 5045  F-8'?>.<!DOCTYPE
-00000030: 2073 7667 2050 5542 4c49 4320 272d 2f2f   svg PUBLIC '-//
-00000040: 5733 432f 2f44 5444 2053 5647 2031 2e31  W3C//DTD SVG 1.1
-00000050: 2f2f 454e 2720 2768 7474 703a 2f2f 7777  //EN' 'http://ww
-00000060: 772e 7733 2e6f 7267 2f47 7261 7068 6963  w.w3.org/Graphic
-00000070: 732f 5356 472f 312e 312f 4454 442f 7376  s/SVG/1.1/DTD/sv
-00000080: 6731 312e 6474 6427 3e0a 3c21 2d2d 2d0a  g11.dtd'>.<!---.
-00000090: 5468 6973 2066 696c 6520 6973 2070 6172  This file is par
-000000a0: 7420 6f66 204b 6572 796b 6569 6f6e 2061  t of Kerykeion a
-000000b0: 6e64 2069 7320 6261 7365 6420 6f6e 204f  nd is based on O
-000000c0: 7065 6e41 7374 726f 2e6f 7267 202d 2d3e  penAstro.org -->
-000000d0: 0a3c 7376 670a 2020 2020 786d 6c6e 733d  .<svg.    xmlns=
-000000e0: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
-000000f0: 7267 2f32 3030 302f 7376 6722 0a20 2020  rg/2000/svg".   
-00000100: 2078 6d6c 6e73 3a78 6c69 6e6b 3d22 6874   xmlns:xlink="ht
-00000110: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
-00000120: 3139 3939 2f78 6c69 6e6b 220a 2020 2020  1999/xlink".    
-00000130: 7769 6474 683d 2224 7376 6757 6964 7468  width="$svgWidth
-00000140: 220a 2020 2020 6865 6967 6874 3d22 2473  ".    height="$s
-00000150: 7667 4865 6967 6874 220a 2020 2020 7669  vgHeight".    vi
-00000160: 6577 426f 783d 2224 7669 6577 626f 7822  ewBox="$viewbox"
-00000170: 0a20 2020 2070 7265 7365 7276 6541 7370  .    preserveAsp
-00000180: 6563 7452 6174 696f 3d22 784d 6964 594d  ectRatio="xMidYM
-00000190: 6964 220a 3e0a 2020 2020 3c74 6974 6c65  id".>.    <title
-000001a0: 3e4b 6572 796b 6569 6f6e 3c2f 7469 746c  >Kerykeion</titl
-000001b0: 653e 0a20 2020 203c 6720 7472 616e 7366  e>.    <g transf
-000001c0: 6f72 6d3d 2274 7261 6e73 6c61 7465 2824  orm="translate($
-000001d0: 6366 6754 7261 6e73 6c61 7465 2922 3e0a  cfgTranslate)">.
-000001e0: 2020 2020 2020 2020 3c67 2074 7261 6e73          <g trans
-000001f0: 666f 726d 3d22 726f 7461 7465 2824 6366  form="rotate($cf
-00000200: 6752 6f74 6174 6529 223e 0a20 2020 2020  gRotate)">.     
-00000210: 2020 2020 2020 203c 6720 7472 616e 7366         <g transf
-00000220: 6f72 6d3d 2273 6361 6c65 2824 6366 675a  orm="scale($cfgZ
-00000230: 6f6f 6d29 223e 0a20 2020 2020 2020 2020  oom)">.         
-00000240: 2020 2020 2020 203c 7265 6374 2078 3d22         <rect x="
-00000250: 3022 2079 3d22 3022 2077 6964 7468 3d22  0" y="0" width="
-00000260: 2463 6861 7274 5f77 6964 7468 2220 6865  $chart_width" he
-00000270: 6967 6874 3d22 3534 362e 3022 2073 7479  ight="546.0" sty
-00000280: 6c65 3d22 6669 6c6c 3a20 2470 6170 6572  le="fill: $paper
-00000290: 5f63 6f6c 6f72 5f31 2220 2f3e 0a20 2020  _color_1" />.   
-000002a0: 2020 2020 2020 2020 2020 2020 203c 7465               <te
-000002b0: 7874 2078 3d22 3230 2220 793d 2233 3022  xt x="20" y="30"
-000002c0: 2073 7479 6c65 3d22 6669 6c6c 3a20 2470   style="fill: $p
-000002d0: 6170 6572 5f63 6f6c 6f72 5f30 3b20 666f  aper_color_0; fo
-000002e0: 6e74 2d73 697a 653a 2032 3470 7822 3e24  nt-size: 24px">$
-000002f0: 7374 7269 6e67 5469 746c 653c 2f74 6578  stringTitle</tex
-00000300: 743e 0a20 2020 2020 2020 2020 2020 2020  t>.             
-00000310: 2020 203c 7465 7874 2078 3d22 3230 2220     <text x="20" 
-00000320: 793d 2235 3022 2073 7479 6c65 3d22 6669  y="50" style="fi
-00000330: 6c6c 3a20 2470 6170 6572 5f63 6f6c 6f72  ll: $paper_color
-00000340: 5f30 3b20 666f 6e74 2d73 697a 653a 2031  _0; font-size: 1
-00000350: 3170 7822 3e24 7374 7269 6e67 4e61 6d65  1px">$stringName
-00000360: 3c2f 7465 7874 3e0a 2020 2020 2020 2020  </text>.        
-00000370: 2020 2020 2020 2020 3c74 6578 7420 783d          <text x=
-00000380: 2232 3022 2079 3d22 3632 2220 7374 796c  "20" y="62" styl
-00000390: 653d 2266 696c 6c3a 2024 7061 7065 725f  e="fill: $paper_
-000003a0: 636f 6c6f 725f 303b 2066 6f6e 742d 7369  color_0; font-si
-000003b0: 7a65 3a20 3131 7078 223e 2473 7472 696e  ze: 11px">$strin
-000003c0: 674c 6f63 6174 696f 6e3c 2f74 6578 743e  gLocation</text>
-000003d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000003e0: 203c 7465 7874 2078 3d22 3230 2220 793d   <text x="20" y=
-000003f0: 2237 3422 2073 7479 6c65 3d22 6669 6c6c  "74" style="fill
-00000400: 3a20 2470 6170 6572 5f63 6f6c 6f72 5f30  : $paper_color_0
-00000410: 3b20 666f 6e74 2d73 697a 653a 2031 3170  ; font-size: 11p
-00000420: 7822 3e24 7374 7269 6e67 4461 7465 5469  x">$stringDateTi
-00000430: 6d65 3c2f 7465 7874 3e0a 2020 2020 2020  me</text>.      
-00000440: 2020 2020 2020 2020 2020 3c74 6578 7420            <text 
-00000450: 783d 2232 3022 2079 3d22 3836 2220 7374  x="20" y="86" st
-00000460: 796c 653d 2266 696c 6c3a 2024 7061 7065  yle="fill: $pape
-00000470: 725f 636f 6c6f 725f 303b 2066 6f6e 742d  r_color_0; font-
-00000480: 7369 7a65 3a20 3131 7078 223e 2473 7472  size: 11px">$str
-00000490: 696e 674c 6174 3c2f 7465 7874 3e0a 2020  ingLat</text>.  
-000004a0: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
-000004b0: 6578 7420 783d 2232 3022 2079 3d22 3938  ext x="20" y="98
-000004c0: 2220 7374 796c 653d 2266 696c 6c3a 2024  " style="fill: $
-000004d0: 7061 7065 725f 636f 6c6f 725f 303b 2066  paper_color_0; f
-000004e0: 6f6e 742d 7369 7a65 3a20 3131 7078 223e  ont-size: 11px">
-000004f0: 2473 7472 696e 674c 6f6e 3c2f 7465 7874  $stringLon</text
-00000500: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000510: 2020 3c74 6578 7420 783d 2232 3022 2079    <text x="20" y
-00000520: 3d22 3131 3022 2073 7479 6c65 3d22 6669  ="110" style="fi
-00000530: 6c6c 3a20 2470 6170 6572 5f63 6f6c 6f72  ll: $paper_color
-00000540: 5f30 3b20 666f 6e74 2d73 697a 653a 2031  _0; font-size: 1
-00000550: 3170 7822 3e24 7374 7269 6e67 506f 7369  1px">$stringPosi
-00000560: 7469 6f6e 3c2f 7465 7874 3e0a 2020 2020  tion</text>.    
-00000570: 2020 2020 2020 2020 2020 2020 3c74 6578              <tex
-00000580: 7420 783d 2232 3022 2079 3d22 3438 3022  t x="20" y="480"
-00000590: 2073 7479 6c65 3d22 6669 6c6c 3a20 2470   style="fill: $p
-000005a0: 6170 6572 5f63 6f6c 6f72 5f30 3b20 666f  aper_color_0; fo
-000005b0: 6e74 2d73 697a 653a 2031 3070 7822 3e24  nt-size: 10px">$
-000005c0: 626f 7474 6f6d 4c65 6674 313c 2f74 6578  bottomLeft1</tex
-000005d0: 743e 0a20 2020 2020 2020 2020 2020 2020  t>.             
-000005e0: 2020 203c 7465 7874 2078 3d22 3230 2220     <text x="20" 
-000005f0: 793d 2234 3934 2220 7374 796c 653d 2266  y="494" style="f
-00000600: 696c 6c3a 2024 7061 7065 725f 636f 6c6f  ill: $paper_colo
-00000610: 725f 303b 2066 6f6e 742d 7369 7a65 3a20  r_0; font-size: 
-00000620: 3130 7078 223e 2462 6f74 746f 6d4c 6566  10px">$bottomLef
-00000630: 7432 3c2f 7465 7874 3e0a 2020 2020 2020  t2</text>.      
-00000640: 2020 2020 2020 2020 2020 3c74 6578 7420            <text 
-00000650: 783d 2232 3022 2079 3d22 3530 3822 2073  x="20" y="508" s
-00000660: 7479 6c65 3d22 6669 6c6c 3a20 2470 6170  tyle="fill: $pap
-00000670: 6572 5f63 6f6c 6f72 5f30 3b20 666f 6e74  er_color_0; font
-00000680: 2d73 697a 653a 2031 3070 7822 3e24 626f  -size: 10px">$bo
-00000690: 7474 6f6d 4c65 6674 333c 2f74 6578 743e  ttomLeft3</text>
-000006a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000006b0: 203c 7465 7874 2078 3d22 3230 2220 793d   <text x="20" y=
-000006c0: 2235 3232 2220 7374 796c 653d 2266 696c  "522" style="fil
-000006d0: 6c3a 2024 7061 7065 725f 636f 6c6f 725f  l: $paper_color_
-000006e0: 303b 2066 6f6e 742d 7369 7a65 3a20 3130  0; font-size: 10
-000006f0: 7078 223e 2462 6f74 746f 6d4c 6566 7434  px">$bottomLeft4
-00000700: 3c2f 7465 7874 3e0a 2020 2020 2020 2020  </text>.        
-00000710: 2020 2020 2020 2020 3c21 2d2d 204c 756e          <!-- Lun
-00000720: 6172 2050 6861 7365 202d 2d3e 0a20 2020  ar Phase -->.   
-00000730: 2020 2020 2020 2020 2020 2020 203c 6720               <g 
-00000740: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
-00000750: 6c61 7465 2832 302c 3531 3829 223e 0a20  late(20,518)">. 
-00000760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000770: 2020 203c 6720 7472 616e 7366 6f72 6d3d     <g transform=
-00000780: 2272 6f74 6174 6528 246c 756e 6172 5f70  "rotate($lunar_p
-00000790: 6861 7365 5f72 6f74 6174 6520 3230 2031  hase_rotate 20 1
-000007a0: 3029 223e 0a20 2020 2020 2020 2020 2020  0)">.           
-000007b0: 2020 2020 2020 2020 2020 2020 203c 6465               <de
-000007c0: 6673 3e0a 2020 2020 2020 2020 2020 2020  fs>.            
-000007d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007e0: 3c63 6c69 7050 6174 6820 6964 3d22 6375  <clipPath id="cu
-000007f0: 742d 6f66 662d 6369 7263 6c65 223e 0a20  t-off-circle">. 
-00000800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000810: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000820: 6369 7263 6c65 2063 783d 2232 3022 2063  circle cx="20" c
-00000830: 793d 2231 3022 2072 3d22 3130 2220 2f3e  y="10" r="10" />
-00000840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000850: 2020 2020 2020 2020 2020 2020 203c 2f63               </c
-00000860: 6c69 7050 6174 683e 0a20 2020 2020 2020  lipPath>.       
-00000870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000880: 203c 2f64 6566 733e 0a20 2020 2020 2020   </defs>.       
+00000020: 462d 3827 3f3e 0a3c 212d 2d2d 2054 6869  F-8'?>.<!--- Thi
+00000030: 7320 6669 6c65 2069 7320 7061 7274 206f  s file is part o
+00000040: 6620 4b65 7279 6b65 696f 6e20 616e 6420  f Kerykeion and 
+00000050: 6973 2062 6173 6564 206f 6e20 4f70 656e  is based on Open
+00000060: 4173 7472 6f2e 6f72 6720 2d2d 3e0a 3c73  Astro.org -->.<s
+00000070: 7667 0a20 2020 2078 6d6c 6e73 3d22 6874  vg.    xmlns="ht
+00000080: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
+00000090: 3230 3030 2f73 7667 220a 2020 2020 786d  2000/svg".    xm
+000000a0: 6c6e 733a 786c 696e 6b3d 2268 7474 703a  lns:xlink="http:
+000000b0: 2f2f 7777 772e 7733 2e6f 7267 2f31 3939  //www.w3.org/199
+000000c0: 392f 786c 696e 6b22 0a20 2020 2077 6964  9/xlink".    wid
+000000d0: 7468 3d22 2473 7667 5769 6474 6822 0a20  th="$svgWidth". 
+000000e0: 2020 2068 6569 6768 743d 2224 7376 6748     height="$svgH
+000000f0: 6569 6768 7422 0a20 2020 2076 6965 7742  eight".    viewB
+00000100: 6f78 3d22 2476 6965 7762 6f78 220a 2020  ox="$viewbox".  
+00000110: 2020 7072 6573 6572 7665 4173 7065 6374    preserveAspect
+00000120: 5261 7469 6f3d 2278 4d69 6459 4d69 6422  Ratio="xMidYMid"
+00000130: 0a3e 0a20 2020 203c 7469 746c 653e 2473  .>.    <title>$s
+00000140: 7472 696e 6754 6974 6c65 207c 204b 6572  tringTitle | Ker
+00000150: 796b 6569 6f6e 3c2f 7469 746c 653e 0a20  ykeion</title>. 
+00000160: 2020 203c 6720 7472 616e 7366 6f72 6d3d     <g transform=
+00000170: 2274 7261 6e73 6c61 7465 2824 6366 6754  "translate($cfgT
+00000180: 7261 6e73 6c61 7465 2922 3e0a 2020 2020  ranslate)">.    
+00000190: 2020 2020 3c67 2074 7261 6e73 666f 726d      <g transform
+000001a0: 3d22 726f 7461 7465 2824 6366 6752 6f74  ="rotate($cfgRot
+000001b0: 6174 6529 223e 0a20 2020 2020 2020 2020  ate)">.         
+000001c0: 2020 203c 6720 7472 616e 7366 6f72 6d3d     <g transform=
+000001d0: 2273 6361 6c65 2824 6366 675a 6f6f 6d29  "scale($cfgZoom)
+000001e0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+000001f0: 2020 203c 7265 6374 2078 3d22 3022 2079     <rect x="0" y
+00000200: 3d22 3022 2077 6964 7468 3d22 2463 6861  ="0" width="$cha
+00000210: 7274 5f77 6964 7468 2220 6865 6967 6874  rt_width" height
+00000220: 3d22 3534 362e 3022 2073 7479 6c65 3d22  ="546.0" style="
+00000230: 6669 6c6c 3a20 2470 6170 6572 5f63 6f6c  fill: $paper_col
+00000240: 6f72 5f31 2220 2f3e 0a20 2020 2020 2020  or_1" />.       
+00000250: 2020 2020 2020 2020 203c 7465 7874 2078           <text x
+00000260: 3d22 3230 2220 793d 2233 3022 2073 7479  ="20" y="30" sty
+00000270: 6c65 3d22 6669 6c6c 3a20 2470 6170 6572  le="fill: $paper
+00000280: 5f63 6f6c 6f72 5f30 3b20 666f 6e74 2d73  _color_0; font-s
+00000290: 697a 653a 2032 3470 7822 3e24 7374 7269  ize: 24px">$stri
+000002a0: 6e67 5469 746c 653c 2f74 6578 743e 0a20  ngTitle</text>. 
+000002b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000002c0: 7465 7874 2078 3d22 3230 2220 793d 2235  text x="20" y="5
+000002d0: 3022 2073 7479 6c65 3d22 6669 6c6c 3a20  0" style="fill: 
+000002e0: 2470 6170 6572 5f63 6f6c 6f72 5f30 3b20  $paper_color_0; 
+000002f0: 666f 6e74 2d73 697a 653a 2031 3170 7822  font-size: 11px"
+00000300: 3e24 7374 7269 6e67 4e61 6d65 3c2f 7465  >$stringName</te
+00000310: 7874 3e0a 2020 2020 2020 2020 2020 2020  xt>.            
+00000320: 2020 2020 3c74 6578 7420 783d 2232 3022      <text x="20"
+00000330: 2079 3d22 3632 2220 7374 796c 653d 2266   y="62" style="f
+00000340: 696c 6c3a 2024 7061 7065 725f 636f 6c6f  ill: $paper_colo
+00000350: 725f 303b 2066 6f6e 742d 7369 7a65 3a20  r_0; font-size: 
+00000360: 3131 7078 223e 2473 7472 696e 674c 6f63  11px">$stringLoc
+00000370: 6174 696f 6e3c 2f74 6578 743e 0a20 2020  ation</text>.   
+00000380: 2020 2020 2020 2020 2020 2020 203c 7465               <te
+00000390: 7874 2078 3d22 3230 2220 793d 2237 3422  xt x="20" y="74"
+000003a0: 2073 7479 6c65 3d22 6669 6c6c 3a20 2470   style="fill: $p
+000003b0: 6170 6572 5f63 6f6c 6f72 5f30 3b20 666f  aper_color_0; fo
+000003c0: 6e74 2d73 697a 653a 2031 3170 7822 3e24  nt-size: 11px">$
+000003d0: 7374 7269 6e67 4461 7465 5469 6d65 3c2f  stringDateTime</
+000003e0: 7465 7874 3e0a 2020 2020 2020 2020 2020  text>.          
+000003f0: 2020 2020 2020 3c74 6578 7420 783d 2232        <text x="2
+00000400: 3022 2079 3d22 3836 2220 7374 796c 653d  0" y="86" style=
+00000410: 2266 696c 6c3a 2024 7061 7065 725f 636f  "fill: $paper_co
+00000420: 6c6f 725f 303b 2066 6f6e 742d 7369 7a65  lor_0; font-size
+00000430: 3a20 3131 7078 223e 2473 7472 696e 674c  : 11px">$stringL
+00000440: 6174 3c2f 7465 7874 3e0a 2020 2020 2020  at</text>.      
+00000450: 2020 2020 2020 2020 2020 3c74 6578 7420            <text 
+00000460: 783d 2232 3022 2079 3d22 3938 2220 7374  x="20" y="98" st
+00000470: 796c 653d 2266 696c 6c3a 2024 7061 7065  yle="fill: $pape
+00000480: 725f 636f 6c6f 725f 303b 2066 6f6e 742d  r_color_0; font-
+00000490: 7369 7a65 3a20 3131 7078 223e 2473 7472  size: 11px">$str
+000004a0: 696e 674c 6f6e 3c2f 7465 7874 3e0a 2020  ingLon</text>.  
+000004b0: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
+000004c0: 6578 7420 783d 2232 3022 2079 3d22 3131  ext x="20" y="11
+000004d0: 3022 2073 7479 6c65 3d22 6669 6c6c 3a20  0" style="fill: 
+000004e0: 2470 6170 6572 5f63 6f6c 6f72 5f30 3b20  $paper_color_0; 
+000004f0: 666f 6e74 2d73 697a 653a 2031 3170 7822  font-size: 11px"
+00000500: 3e24 7374 7269 6e67 506f 7369 7469 6f6e  >$stringPosition
+00000510: 3c2f 7465 7874 3e0a 2020 2020 2020 2020  </text>.        
+00000520: 2020 2020 2020 2020 3c74 6578 7420 783d          <text x=
+00000530: 2232 3022 2079 3d22 3438 3022 2073 7479  "20" y="480" sty
+00000540: 6c65 3d22 6669 6c6c 3a20 2470 6170 6572  le="fill: $paper
+00000550: 5f63 6f6c 6f72 5f30 3b20 666f 6e74 2d73  _color_0; font-s
+00000560: 697a 653a 2031 3070 7822 3e24 626f 7474  ize: 10px">$bott
+00000570: 6f6d 4c65 6674 313c 2f74 6578 743e 0a20  omLeft1</text>. 
+00000580: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000590: 7465 7874 2078 3d22 3230 2220 793d 2234  text x="20" y="4
+000005a0: 3934 2220 7374 796c 653d 2266 696c 6c3a  94" style="fill:
+000005b0: 2024 7061 7065 725f 636f 6c6f 725f 303b   $paper_color_0;
+000005c0: 2066 6f6e 742d 7369 7a65 3a20 3130 7078   font-size: 10px
+000005d0: 223e 2462 6f74 746f 6d4c 6566 7432 3c2f  ">$bottomLeft2</
+000005e0: 7465 7874 3e0a 2020 2020 2020 2020 2020  text>.          
+000005f0: 2020 2020 2020 3c74 6578 7420 783d 2232        <text x="2
+00000600: 3022 2079 3d22 3530 3822 2073 7479 6c65  0" y="508" style
+00000610: 3d22 6669 6c6c 3a20 2470 6170 6572 5f63  ="fill: $paper_c
+00000620: 6f6c 6f72 5f30 3b20 666f 6e74 2d73 697a  olor_0; font-siz
+00000630: 653a 2031 3070 7822 3e24 626f 7474 6f6d  e: 10px">$bottom
+00000640: 4c65 6674 333c 2f74 6578 743e 0a20 2020  Left3</text>.   
+00000650: 2020 2020 2020 2020 2020 2020 203c 7465               <te
+00000660: 7874 2078 3d22 3230 2220 793d 2235 3232  xt x="20" y="522
+00000670: 2220 7374 796c 653d 2266 696c 6c3a 2024  " style="fill: $
+00000680: 7061 7065 725f 636f 6c6f 725f 303b 2066  paper_color_0; f
+00000690: 6f6e 742d 7369 7a65 3a20 3130 7078 223e  ont-size: 10px">
+000006a0: 2462 6f74 746f 6d4c 6566 7434 3c2f 7465  $bottomLeft4</te
+000006b0: 7874 3e0a 2020 2020 2020 2020 2020 2020  xt>.            
+000006c0: 2020 2020 3c21 2d2d 204c 756e 6172 2050      <!-- Lunar P
+000006d0: 6861 7365 202d 2d3e 0a20 2020 2020 2020  hase -->.       
+000006e0: 2020 2020 2020 2020 203c 6720 7472 616e           <g tran
+000006f0: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
+00000700: 2832 302c 3531 3829 223e 0a20 2020 2020  (20,518)">.     
+00000710: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000720: 6720 7472 616e 7366 6f72 6d3d 2272 6f74  g transform="rot
+00000730: 6174 6528 246c 756e 6172 5f70 6861 7365  ate($lunar_phase
+00000740: 5f72 6f74 6174 6520 3230 2031 3029 223e  _rotate 20 10)">
+00000750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000760: 2020 2020 2020 2020 203c 6465 6673 3e0a           <defs>.
+00000770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000780: 2020 2020 2020 2020 2020 2020 3c63 6c69              <cli
+00000790: 7050 6174 6820 6964 3d22 6375 742d 6f66  pPath id="cut-of
+000007a0: 662d 6369 7263 6c65 223e 0a20 2020 2020  f-circle">.     
+000007b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007c0: 2020 2020 2020 2020 2020 203c 6369 7263             <circ
+000007d0: 6c65 2063 783d 2232 3022 2063 793d 2231  le cx="20" cy="1
+000007e0: 3022 2072 3d22 3130 2220 2f3e 0a20 2020  0" r="10" />.   
+000007f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000800: 2020 2020 2020 2020 203c 2f63 6c69 7050           </clipP
+00000810: 6174 683e 0a20 2020 2020 2020 2020 2020  ath>.           
+00000820: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+00000830: 6566 733e 0a20 2020 2020 2020 2020 2020  efs>.           
+00000840: 2020 2020 2020 2020 2020 2020 203c 6369               <ci
+00000850: 7263 6c65 2063 783d 2232 3022 2063 793d  rcle cx="20" cy=
+00000860: 2231 3022 2072 3d22 3130 2220 7374 796c  "10" r="10" styl
+00000870: 653d 2266 696c 6c3a 2024 6c75 6e61 725f  e="fill: $lunar_
+00000880: 7068 6173 655f 6267 2220 2f3e 0a20 2020  phase_bg" />.   
 00000890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008a0: 203c 6369 7263 6c65 2063 783d 2232 3022   <circle cx="20"
-000008b0: 2063 793d 2231 3022 2072 3d22 3130 2220   cy="10" r="10" 
-000008c0: 7374 796c 653d 2266 696c 6c3a 2024 6c75  style="fill: $lu
-000008d0: 6e61 725f 7068 6173 655f 6267 2220 2f3e  nar_phase_bg" />
-000008e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000008f0: 2020 2020 2020 2020 203c 6369 7263 6c65           <circle
-00000900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000910: 2020 2020 2020 2020 2020 2020 2063 783d               cx=
-00000920: 2224 6c75 6e61 725f 7068 6173 655f 6378  "$lunar_phase_cx
-00000930: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00000940: 2020 2020 2020 2020 2020 2020 2020 6379                cy
-00000950: 3d22 3130 220a 2020 2020 2020 2020 2020  ="10".          
-00000960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000970: 2020 723d 2224 6c75 6e61 725f 7068 6173    r="$lunar_phas
-00000980: 655f 7222 0a20 2020 2020 2020 2020 2020  e_r".           
-00000990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009a0: 2073 7479 6c65 3d22 6669 6c6c 3a20 246c   style="fill: $l
-000009b0: 756e 6172 5f70 6861 7365 5f66 6722 0a20  unar_phase_fg". 
-000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009d0: 2020 2020 2020 2020 2020 2063 6c69 702d             clip-
-000009e0: 7061 7468 3d22 7572 6c28 2363 7574 2d6f  path="url(#cut-o
-000009f0: 6666 2d63 6972 636c 6529 220a 2020 2020  ff-circle)".    
-00000a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a10: 2020 2020 2f3e 0a20 2020 2020 2020 2020      />.         
-00000a20: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000a30: 6369 7263 6c65 0a20 2020 2020 2020 2020  circle.         
-00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a50: 2020 2063 783d 2232 3022 0a20 2020 2020     cx="20".     
-00000a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a70: 2020 2020 2020 2063 793d 2231 3022 0a20         cy="10". 
-00000a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a90: 2020 2020 2020 2020 2020 2072 3d22 3130             r="10
-00000aa0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00000ab0: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00000ac0: 796c 653d 2266 696c 6c3a 206e 6f6e 653b  yle="fill: none;
-00000ad0: 2073 7472 6f6b 653a 2024 6c75 6e61 725f   stroke: $lunar_
-00000ae0: 7068 6173 655f 6f75 746c 696e 653b 2073  phase_outline; s
-00000af0: 7472 6f6b 652d 7769 6474 683a 2030 2e35  troke-width: 0.5
-00000b00: 7078 3b20 7374 726f 6b65 2d6f 7061 6369  px; stroke-opaci
-00000b10: 7479 3a20 302e 3522 0a20 2020 2020 2020  ty: 0.5".       
-00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b30: 202f 3e0a 2020 2020 2020 2020 2020 2020   />.            
-00000b40: 2020 2020 2020 2020 3c2f 673e 0a20 2020          </g>.   
-00000b50: 2020 2020 2020 2020 2020 2020 203c 2f67               </g
-00000b60: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000b70: 2020 3c21 2d2d 2050 6c61 6e65 7473 2028    <!-- Planets (
-00000b80: 3234 7832 3429 202d 2d3e 0a20 2020 2020  24x24) -->.     
-00000b90: 2020 2020 2020 2020 2020 203c 7379 6d62             <symb
-00000ba0: 6f6c 2069 643d 2253 756e 223e 0a20 2020  ol id="Sun">.   
-00000bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bc0: 203c 6720 7472 616e 7366 6f72 6d3d 2274   <g transform="t
-00000bd0: 7261 6e73 6c61 7465 2831 2c34 2922 3e0a  ranslate(1,4)">.
-00000be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bf0: 2020 2020 2020 2020 3c63 6972 636c 6520          <circle 
-00000c00: 6378 3d22 3130 2220 6379 3d22 3130 2220  cx="10" cy="10" 
-00000c10: 723d 2239 220a 2020 2020 2020 2020 2020  r="9".          
-00000c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c30: 2020 7374 796c 653d 2266 696c 6c3a 206e    style="fill: n
-00000c40: 6f6e 653b 2073 7472 6f6b 653a 2024 706c  one; stroke: $pl
-00000c50: 616e 6574 735f 636f 6c6f 725f 303b 2073  anets_color_0; s
-00000c60: 7472 6f6b 652d 7769 6474 683a 2032 7078  troke-width: 2px
-00000c70: 2220 2f3e 0a20 2020 2020 2020 2020 2020  " />.           
-00000c80: 2020 2020 2020 2020 2020 2020 203c 6369               <ci
-00000c90: 7263 6c65 2063 783d 2231 3022 2063 793d  rcle cx="10" cy=
-00000ca0: 2231 3022 2072 3d22 3222 2073 7479 6c65  "10" r="2" style
-00000cb0: 3d22 6669 6c6c 3a20 2470 6c61 6e65 7473  ="fill: $planets
-00000cc0: 5f63 6f6c 6f72 5f30 2220 2f3e 0a20 2020  _color_0" />.   
+000008a0: 2020 2020 203c 6369 7263 6c65 0a20 2020       <circle.   
+000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008c0: 2020 2020 2020 2020 2063 783d 2224 6c75           cx="$lu
+000008d0: 6e61 725f 7068 6173 655f 6378 220a 2020  nar_phase_cx".  
+000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008f0: 2020 2020 2020 2020 2020 6379 3d22 3130            cy="10
+00000900: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00000910: 2020 2020 2020 2020 2020 2020 2020 723d                r=
+00000920: 2224 6c75 6e61 725f 7068 6173 655f 7222  "$lunar_phase_r"
+00000930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000940: 2020 2020 2020 2020 2020 2020 2073 7479               sty
+00000950: 6c65 3d22 6669 6c6c 3a20 246c 756e 6172  le="fill: $lunar
+00000960: 5f70 6861 7365 5f66 6722 0a20 2020 2020  _phase_fg".     
+00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000980: 2020 2020 2020 2063 6c69 702d 7061 7468         clip-path
+00000990: 3d22 7572 6c28 2363 7574 2d6f 6666 2d63  ="url(#cut-off-c
+000009a0: 6972 636c 6529 220a 2020 2020 2020 2020  ircle)".        
+000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009c0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+000009d0: 2020 2020 2020 2020 2020 203c 6369 7263             <circ
+000009e0: 6c65 0a20 2020 2020 2020 2020 2020 2020  le.             
+000009f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00000a00: 783d 2232 3022 0a20 2020 2020 2020 2020  x="20".         
+00000a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a20: 2020 2063 793d 2231 3022 0a20 2020 2020     cy="10".     
+00000a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a40: 2020 2020 2020 2072 3d22 3130 220a 2020         r="10".  
+00000a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a60: 2020 2020 2020 2020 2020 7374 796c 653d            style=
+00000a70: 2266 696c 6c3a 206e 6f6e 653b 2073 7472  "fill: none; str
+00000a80: 6f6b 653a 2024 6c75 6e61 725f 7068 6173  oke: $lunar_phas
+00000a90: 655f 6f75 746c 696e 653b 2073 7472 6f6b  e_outline; strok
+00000aa0: 652d 7769 6474 683a 2030 2e35 7078 3b20  e-width: 0.5px; 
+00000ab0: 7374 726f 6b65 2d6f 7061 6369 7479 3a20  stroke-opacity: 
+00000ac0: 302e 3522 0a20 2020 2020 2020 2020 2020  0.5".           
+00000ad0: 2020 2020 2020 2020 2020 2020 202f 3e0a               />.
+00000ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000af0: 2020 2020 3c2f 673e 0a20 2020 2020 2020      </g>.       
+00000b00: 2020 2020 2020 2020 203c 2f67 3e0a 2020           </g>.  
+00000b10: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
+00000b20: 2d2d 2050 6c61 6e65 7473 2028 3234 7832  -- Planets (24x2
+00000b30: 3429 202d 2d3e 0a20 2020 2020 2020 2020  4) -->.         
+00000b40: 2020 2020 2020 203c 7379 6d62 6f6c 2069         <symbol i
+00000b50: 643d 2253 756e 223e 0a20 2020 2020 2020  d="Sun">.       
+00000b60: 2020 2020 2020 2020 2020 2020 203c 6720               <g 
+00000b70: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+00000b80: 6c61 7465 2831 2c34 2922 3e0a 2020 2020  late(1,4)">.    
+00000b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ba0: 2020 2020 3c63 6972 636c 6520 6378 3d22      <circle cx="
+00000bb0: 3130 2220 6379 3d22 3130 2220 723d 2239  10" cy="10" r="9
+00000bc0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00000bd0: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00000be0: 796c 653d 2266 696c 6c3a 206e 6f6e 653b  yle="fill: none;
+00000bf0: 2073 7472 6f6b 653a 2024 706c 616e 6574   stroke: $planet
+00000c00: 735f 636f 6c6f 725f 303b 2073 7472 6f6b  s_color_0; strok
+00000c10: 652d 7769 6474 683a 2032 7078 2220 2f3e  e-width: 2px" />
+00000c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000c30: 2020 2020 2020 2020 203c 6369 7263 6c65           <circle
+00000c40: 2063 783d 2231 3022 2063 793d 2231 3022   cx="10" cy="10"
+00000c50: 2072 3d22 3222 2073 7479 6c65 3d22 6669   r="2" style="fi
+00000c60: 6c6c 3a20 2470 6c61 6e65 7473 5f63 6f6c  ll: $planets_col
+00000c70: 6f72 5f30 2220 2f3e 0a20 2020 2020 2020  or_0" />.       
+00000c80: 2020 2020 2020 2020 2020 2020 203c 2f67               </g
+00000c90: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000ca0: 2020 3c2f 7379 6d62 6f6c 3e0a 2020 2020    </symbol>.    
+00000cb0: 2020 2020 2020 2020 2020 2020 3c73 796d              <sym
+00000cc0: 626f 6c20 6964 3d22 4d6f 6f6e 223e 0a20  bol id="Moon">. 
 00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ce0: 203c 2f67 3e0a 2020 2020 2020 2020 2020   </g>.          
-00000cf0: 2020 2020 2020 3c2f 7379 6d62 6f6c 3e0a        </symbol>.
-00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d10: 3c73 796d 626f 6c20 6964 3d22 4d6f 6f6e  <symbol id="Moon
-00000d20: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00000d30: 2020 2020 2020 203c 6720 7472 616e 7366         <g transf
-00000d40: 6f72 6d3d 2274 7261 6e73 6c61 7465 2834  orm="translate(4
-00000d50: 2c33 2922 3e0a 2020 2020 2020 2020 2020  ,3)">.          
-00000d60: 2020 2020 2020 2020 2020 2020 2020 3c67                <g
-00000d70: 2074 7261 6e73 666f 726d 3d22 7363 616c   transform="scal
-00000d80: 6528 2e38 2922 3e0a 2020 2020 2020 2020  e(.8)">.        
-00000d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000da0: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
-00000db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000dc0: 2020 2020 2020 2020 2020 643d 224d 2033            d="M 3
-00000dd0: 2e36 3633 3931 3934 2c31 2e30 3330 3835  .6639194,1.03085
-00000de0: 3039 2043 2032 2e37 3439 3834 3934 2c31  09 C 2.7498494,1
-00000df0: 2e30 3635 3633 3039 2031 2e38 3732 3133  .0656309 1.87213
-00000e00: 3934 2c31 2e32 3133 3932 3039 2031 2e30  94,1.2139209 1.0
-00000e10: 3238 3436 3934 2c31 2e34 3539 3338 3039  284694,1.4593809
-00000e20: 2043 2035 2e35 3732 3937 3934 2c32 2e37   C 5.5729794,2.7
-00000e30: 3939 3936 3039 2038 2e38 3931 3937 3934  999609 8.8919794
-00000e40: 2c37 2e30 3234 3232 3039 2038 2e38 3931  ,7.0242209 8.891
-00000e50: 3937 3934 2c31 322e 3030 3131 3931 2043  9794,12.001191 C
-00000e60: 2038 2e38 3931 3937 3934 2c31 362e 3937   8.8919794,16.97
-00000e70: 3831 3631 2035 2e35 3732 3937 3934 2c32  8161 5.5729794,2
-00000e80: 312e 3230 3234 3131 2031 2e30 3238 3436  1.202411 1.02846
-00000e90: 3934 2c32 322e 3534 3330 3031 2043 2032  94,22.543001 C 2
-00000ea0: 2e30 3031 3932 3934 2c32 322e 3832 3632  .0019294,22.8262
-00000eb0: 3231 2033 2e30 3237 3938 3934 2c32 322e  21 3.0279894,22.
-00000ec0: 3937 3135 3331 2034 2e30 3932 3434 3934  971531 4.0924494
-00000ed0: 2c32 322e 3937 3135 3331 2043 2031 302e  ,22.971531 C 10.
-00000ee0: 3134 3830 3739 2c32 322e 3937 3135 3331  148079,22.971531
-00000ef0: 2031 352e 3036 3237 3839 2c31 382e 3035   15.062789,18.05
-00000f00: 3638 3231 2031 352e 3036 3237 3839 2c31  6821 15.062789,1
-00000f10: 322e 3030 3131 3931 2043 2031 352e 3036  2.001191 C 15.06
-00000f20: 3237 3839 2c35 2e39 3435 3536 3039 2031  2789,5.9455609 1
-00000f30: 302e 3134 3830 3739 2c31 2e30 3330 3835  0.148079,1.03085
-00000f40: 3039 2034 2e30 3932 3434 3934 2c31 2e30  09 4.0924494,1.0
-00000f50: 3330 3835 3039 2043 2033 2e39 3530 3531  308509 C 3.95051
-00000f60: 3934 2c31 2e30 3330 3835 3039 2033 2e38  94,1.0308509 3.8
-00000f70: 3034 3534 3934 2c31 2e30 3235 3439 3039  045494,1.0254909
-00000f80: 2033 2e36 3633 3931 3934 2c31 2e30 3330   3.6639194,1.030
-00000f90: 3835 3039 207a 2022 0a20 2020 2020 2020  8509 z ".       
-00000fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fb0: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-00000fc0: 7374 726f 6b65 3a20 2470 6c61 6e65 7473  stroke: $planets
-00000fd0: 5f63 6f6c 6f72 5f31 3b20 7374 726f 6b65  _color_1; stroke
-00000fe0: 2d77 6964 7468 3a20 3270 783b 2066 696c  -width: 2px; fil
-00000ff0: 6c3a 206e 6f6e 6522 0a20 2020 2020 2020  l: none".       
-00001000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001010: 2020 2020 202f 3e0a 2020 2020 2020 2020       />.        
-00001020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001030: 3c2f 673e 0a20 2020 2020 2020 2020 2020  </g>.           
-00001040: 2020 2020 2020 2020 203c 2f67 3e0a 2020           </g>.  
-00001050: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00001060: 7379 6d62 6f6c 3e0a 2020 2020 2020 2020  symbol>.        
-00001070: 2020 2020 2020 2020 3c73 796d 626f 6c20          <symbol 
-00001080: 6964 3d22 4d65 7263 7572 7922 3e0a 2020  id="Mercury">.  
+00000ce0: 2020 203c 6720 7472 616e 7366 6f72 6d3d     <g transform=
+00000cf0: 2274 7261 6e73 6c61 7465 2834 2c33 2922  "translate(4,3)"
+00000d00: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000d10: 2020 2020 2020 2020 2020 3c67 2074 7261            <g tra
+00000d20: 6e73 666f 726d 3d22 7363 616c 6528 2e38  nsform="scale(.8
+00000d30: 2922 3e0a 2020 2020 2020 2020 2020 2020  )">.            
+00000d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d50: 3c70 6174 680a 2020 2020 2020 2020 2020  <path.          
+00000d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d70: 2020 2020 2020 643d 224d 2033 2e36 3633        d="M 3.663
+00000d80: 3931 3934 2c31 2e30 3330 3835 3039 2043  9194,1.0308509 C
+00000d90: 2032 2e37 3439 3834 3934 2c31 2e30 3635   2.7498494,1.065
+00000da0: 3633 3039 2031 2e38 3732 3133 3934 2c31  6309 1.8721394,1
+00000db0: 2e32 3133 3932 3039 2031 2e30 3238 3436  .2139209 1.02846
+00000dc0: 3934 2c31 2e34 3539 3338 3039 2043 2035  94,1.4593809 C 5
+00000dd0: 2e35 3732 3937 3934 2c32 2e37 3939 3936  .5729794,2.79996
+00000de0: 3039 2038 2e38 3931 3937 3934 2c37 2e30  09 8.8919794,7.0
+00000df0: 3234 3232 3039 2038 2e38 3931 3937 3934  242209 8.8919794
+00000e00: 2c31 322e 3030 3131 3931 2043 2038 2e38  ,12.001191 C 8.8
+00000e10: 3931 3937 3934 2c31 362e 3937 3831 3631  919794,16.978161
+00000e20: 2035 2e35 3732 3937 3934 2c32 312e 3230   5.5729794,21.20
+00000e30: 3234 3131 2031 2e30 3238 3436 3934 2c32  2411 1.0284694,2
+00000e40: 322e 3534 3330 3031 2043 2032 2e30 3031  2.543001 C 2.001
+00000e50: 3932 3934 2c32 322e 3832 3632 3231 2033  9294,22.826221 3
+00000e60: 2e30 3237 3938 3934 2c32 322e 3937 3135  .0279894,22.9715
+00000e70: 3331 2034 2e30 3932 3434 3934 2c32 322e  31 4.0924494,22.
+00000e80: 3937 3135 3331 2043 2031 302e 3134 3830  971531 C 10.1480
+00000e90: 3739 2c32 322e 3937 3135 3331 2031 352e  79,22.971531 15.
+00000ea0: 3036 3237 3839 2c31 382e 3035 3638 3231  062789,18.056821
+00000eb0: 2031 352e 3036 3237 3839 2c31 322e 3030   15.062789,12.00
+00000ec0: 3131 3931 2043 2031 352e 3036 3237 3839  1191 C 15.062789
+00000ed0: 2c35 2e39 3435 3536 3039 2031 302e 3134  ,5.9455609 10.14
+00000ee0: 3830 3739 2c31 2e30 3330 3835 3039 2034  8079,1.0308509 4
+00000ef0: 2e30 3932 3434 3934 2c31 2e30 3330 3835  .0924494,1.03085
+00000f00: 3039 2043 2033 2e39 3530 3531 3934 2c31  09 C 3.9505194,1
+00000f10: 2e30 3330 3835 3039 2033 2e38 3034 3534  .0308509 3.80454
+00000f20: 3934 2c31 2e30 3235 3439 3039 2033 2e36  94,1.0254909 3.6
+00000f30: 3633 3931 3934 2c31 2e30 3330 3835 3039  639194,1.0308509
+00000f40: 207a 2022 0a20 2020 2020 2020 2020 2020   z ".           
+00000f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f60: 2020 2020 2073 7479 6c65 3d22 7374 726f       style="stro
+00000f70: 6b65 3a20 2470 6c61 6e65 7473 5f63 6f6c  ke: $planets_col
+00000f80: 6f72 5f31 3b20 7374 726f 6b65 2d77 6964  or_1; stroke-wid
+00000f90: 7468 3a20 3270 783b 2066 696c 6c3a 206e  th: 2px; fill: n
+00000fa0: 6f6e 6522 0a20 2020 2020 2020 2020 2020  one".           
+00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fc0: 202f 3e0a 2020 2020 2020 2020 2020 2020   />.            
+00000fd0: 2020 2020 2020 2020 2020 2020 3c2f 673e              </g>
+00000fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ff0: 2020 2020 203c 2f67 3e0a 2020 2020 2020       </g>.      
+00001000: 2020 2020 2020 2020 2020 3c2f 7379 6d62            </symb
+00001010: 6f6c 3e0a 2020 2020 2020 2020 2020 2020  ol>.            
+00001020: 2020 2020 3c73 796d 626f 6c20 6964 3d22      <symbol id="
+00001030: 4d65 7263 7572 7922 3e0a 2020 2020 2020  Mercury">.      
+00001040: 2020 2020 2020 2020 2020 2020 2020 3c67                <g
+00001050: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
+00001060: 736c 6174 6528 332c 3129 223e 0a20 2020  slate(3,1)">.   
+00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001080: 2020 2020 203c 7061 7468 0a20 2020 2020       <path.     
 00001090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010a0: 2020 3c67 2074 7261 6e73 666f 726d 3d22    <g transform="
-000010b0: 7472 616e 736c 6174 6528 332c 3129 223e  translate(3,1)">
-000010c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000010d0: 2020 2020 2020 2020 203c 7061 7468 0a20           <path. 
-000010e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010f0: 2020 2020 2020 2020 2020 2064 3d22 4d20             d="M 
-00001100: 3132 2e34 3137 3930 382c 3131 2e30 3937  12.417908,11.097
-00001110: 3530 3720 4320 3132 2e34 3630 3831 382c  507 C 12.460818,
-00001120: 3133 2e36 3034 3931 3620 3130 2e36 3638  13.604916 10.668
-00001130: 3231 372c 3135 2e39 3936 3635 3620 382e  217,15.996656 8.
-00001140: 3235 3636 3830 352c 3136 2e36 3736 3633  2566805,16.67663
-00001150: 3920 4320 362e 3131 3830 3337 352c 3137  9 C 6.1180375,17
-00001160: 2e33 3232 3532 3220 332e 3634 3038 3637  .322522 3.640867
-00001170: 352c 3136 2e36 3131 3836 3920 322e 3139  5,16.611869 2.19
-00001180: 3930 3931 352c 3134 2e38 3937 3032 3520  90915,14.897025 
-00001190: 4320 302e 3730 3235 3133 3531 2c31 332e  C 0.70251351,13.
-000011a0: 3138 3538 3934 2030 2e33 3437 3035 3535  185894 0.3470555
-000011b0: 312c 3130 2e35 3734 3134 3920 312e 3337  1,10.574149 1.37
-000011c0: 3837 3833 352c 382e 3534 3036 3337 2043  87835,8.540637 C
-000011d0: 2032 2e33 3330 3930 3635 2c36 2e35 3737   2.3309065,6.577
-000011e0: 3831 3936 2034 2e34 3434 3839 3235 2c35  8196 4.4448925,5
-000011f0: 2e32 3339 3035 3135 2036 2e36 3334 3433  .2390515 6.63443
-00001200: 3835 2c35 2e32 3830 3138 3132 2043 2038  85,5.2801812 C 8
-00001210: 2e37 3433 3634 3835 2c35 2e32 3830 3831  .7436485,5.28081
-00001220: 3834 2031 302e 3739 3732 312c 362e 3531  84 10.79721,6.51
-00001230: 3834 3839 3720 3131 2e37 3535 3634 312c  84897 11.755641,
-00001240: 382e 3430 3134 3232 3920 4320 3132 2e31  8.4014229 C 12.1
-00001250: 3838 3730 392c 392e 3232 3933 3536 3320  88709,9.2293563 
-00001260: 3132 2e34 3231 3932 362c 3130 2e31 3632  12.421926,10.162
-00001270: 3536 3820 3132 2e34 3137 3930 382c 3131  568 12.417908,11
-00001280: 2e30 3937 3530 3720 7a20 4d20 3131 2e35  .097507 z M 11.5
-00001290: 3337 3534 392c 302e 3739 3437 3737 3536  37549,0.79477756
-000012a0: 2043 2031 312e 3336 3830 3131 2c32 2e39   C 11.368011,2.9
-000012b0: 3533 3136 3336 2039 2e35 3932 3831 3035  531636 9.5928105
-000012c0: 2c34 2e38 3439 3339 3420 372e 3435 3238  ,4.849394 7.4528
-000012d0: 3435 352c 352e 3137 3131 3237 2043 2035  455,5.171127 C 5
-000012e0: 2e34 3933 3430 3335 2c35 2e35 3035 3834  .4934035,5.50584
-000012f0: 3637 2033 2e33 3633 3435 3035 2c34 2e35  67 3.3634505,4.5
-00001300: 3439 3436 3836 2032 2e33 3935 3831 3335  494686 2.3958135
-00001310: 2c32 2e37 3934 3635 3836 2043 2032 2e30  ,2.7946586 C 2.0
-00001320: 3434 3831 3535 2c32 2e31 3831 3837 3436  448155,2.1818746
-00001330: 2031 2e38 3237 3537 3535 2c31 2e34 3933   1.8275755,1.493
-00001340: 3039 3636 2031 2e37 3632 3638 3435 2c30  0966 1.7626845,0
-00001350: 2e37 3839 3933 3735 3620 4d20 362e 3630  .78993756 M 6.60
-00001360: 3339 3632 352c 3136 2e38 3930 3531 3820  39625,16.890518 
-00001370: 4320 362e 3630 3339 3632 352c 3138 2e39  C 6.6039625,18.9
-00001380: 3937 3033 3120 362e 3630 3339 3632 352c  97031 6.6039625,
-00001390: 3231 2e31 3033 3534 3520 362e 3630 3339  21.103545 6.6039
-000013a0: 3632 352c 3233 2e32 3130 3035 3820 4d20  625,23.210058 M 
-000013b0: 332e 3937 3038 3231 352c 3230 2e35 3736  3.9708215,20.576
-000013c0: 3931 3620 4320 352e 3732 3632 3437 352c  916 C 5.7262475,
-000013d0: 3230 2e35 3736 3931 3620 372e 3438 3136  20.576916 7.4816
-000013e0: 3738 352c 3230 2e35 3736 3931 3620 392e  785,20.576916 9.
-000013f0: 3233 3731 3034 352c 3230 2e35 3736 3931  2371045,20.57691
-00001400: 3622 0a20 2020 2020 2020 2020 2020 2020  6".             
-00001410: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001420: 7479 6c65 3d22 7374 726f 6b65 3a20 2470  tyle="stroke: $p
-00001430: 6c61 6e65 7473 5f63 6f6c 6f72 5f32 3b20  lanets_color_2; 
-00001440: 7374 726f 6b65 2d77 6964 7468 3a20 3270  stroke-width: 2p
-00001450: 783b 2066 696c 6c3a 206e 6f6e 6522 0a20  x; fill: none". 
-00001460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001470: 2020 2020 2020 202f 3e0a 2020 2020 2020         />.      
-00001480: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00001490: 673e 0a20 2020 2020 2020 2020 2020 2020  g>.             
-000014a0: 2020 203c 2f73 796d 626f 6c3e 0a20 2020     </symbol>.   
-000014b0: 2020 2020 2020 2020 2020 2020 203c 7379               <sy
-000014c0: 6d62 6f6c 2069 643d 2256 656e 7573 223e  mbol id="Venus">
-000014d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000014e0: 2020 2020 203c 6720 7472 616e 7366 6f72       <g transfor
-000014f0: 6d3d 2274 7261 6e73 6c61 7465 2830 2c32  m="translate(0,2
-00001500: 2922 3e0a 2020 2020 2020 2020 2020 2020  )">.            
-00001510: 2020 2020 2020 2020 2020 2020 3c67 2074              <g t
-00001520: 7261 6e73 666f 726d 3d22 7363 616c 6528  ransform="scale(
-00001530: 2e39 2922 3e0a 2020 2020 2020 2020 2020  .9)">.          
-00001540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001550: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
-00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001570: 2020 2020 2020 2020 643d 224d 2031 382e          d="M 18.
-00001580: 3430 3037 3033 2c37 2e33 3636 3734 3833  400703,7.3667483
-00001590: 2043 2031 382e 3432 3339 362c 392e 3636   C 18.42396,9.66
-000015a0: 3535 3332 3920 3137 2e31 3730 3130 322c  55329 17.170102,
-000015b0: 3131 2e39 3134 3537 3920 3135 2e32 3138  11.914579 15.218
-000015c0: 3937 322c 3133 2e31 3133 3732 3820 4320  972,13.113728 C 
-000015d0: 3133 2e31 3632 3435 392c 3134 2e34 3237  13.162459,14.427
-000015e0: 3235 3320 3130 2e33 3839 3835 352c 3134  253 10.389855,14
-000015f0: 2e34 3736 3737 3220 382e 3238 3731 3636  .476772 8.287166
-00001600: 332c 3133 2e32 3339 3730 3920 4320 362e  3,13.239709 C 6.
-00001610: 3237 3335 3835 312c 3132 2e31 3030 3532  2735851,12.10052
-00001620: 3420 342e 3933 3336 3333 2c39 2e38 3634  4 4.933633,9.864
-00001630: 3033 3233 2034 2e38 3937 3939 3135 2c37  0323 4.8979915,7
-00001640: 2e35 3431 3438 3034 2043 2034 2e38 3137  .5414804 C 4.817
-00001650: 3336 3137 2c35 2e32 3637 3835 3932 2035  3617,5.2678592 5
-00001660: 2e39 3835 3531 3936 2c33 2e30 3039 3030  .9855196,3.00900
-00001670: 3031 2037 2e38 3732 3838 3037 2c31 2e37  01 7.8728807,1.7
-00001680: 3533 3034 3731 2043 2039 2e38 3830 3339  530471 C 9.88039
-00001690: 3135 2c30 2e33 3635 3039 3534 3620 3132  15,0.36509546 12
-000016a0: 2e36 3438 3930 362c 302e 3231 3635 3731  .648906,0.216571
-000016b0: 3436 2031 342e 3739 3438 3439 2c31 2e33  46 14.794849,1.3
-000016c0: 3735 3238 3331 2043 2031 362e 3836 3937  752831 C 16.8697
-000016d0: 3732 2c32 2e34 3531 3436 3333 2031 382e  72,2.4514633 18.
-000016e0: 3239 3632 3431 2c34 2e36 3733 3134 3533  296241,4.6731453
-000016f0: 2031 382e 3339 3139 3138 2c37 2e30 3138   18.391918,7.018
-00001700: 3337 3233 2043 2031 382e 3339 3737 3831  3723 C 18.397781
-00001710: 2c37 2e31 3334 3339 3633 2031 382e 3430  ,7.1343963 18.40
-00001720: 3037 3033 2c37 2e32 3530 3537 3233 2031  0703,7.2505723 1
-00001730: 382e 3430 3037 3033 2c37 2e33 3636 3734  8.400703,7.36674
-00001740: 3833 207a 204d 2031 312e 3634 3832 3839  83 z M 11.648289
-00001750: 2c31 342e 3133 3636 3839 2043 2031 312e  ,14.136689 C 11.
-00001760: 3634 3832 3839 2c31 372e 3030 3837 3634  648289,17.008764
-00001770: 2031 312e 3634 3832 3839 2c31 392e 3838   11.648289,19.88
-00001780: 3038 3420 3131 2e36 3438 3238 392c 3232  084 11.648289,22
-00001790: 2e37 3532 3931 3520 4d20 372e 3936 3531  .752915 M 7.9651
-000017a0: 3333 332c 3139 2e30 3630 3234 3320 4320  333,19.060243 C 
-000017b0: 3130 2e34 3230 3537 2c31 392e 3036 3032  10.42057,19.0602
-000017c0: 3433 2031 322e 3837 3630 3038 2c31 392e  43 12.876008,19.
-000017d0: 3036 3032 3433 2031 352e 3333 3134 3434  060243 15.331444
-000017e0: 2c31 392e 3036 3032 3433 220a 2020 2020  ,19.060243".    
-000017f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001800: 2020 2020 2020 2020 2020 2020 7374 796c              styl
-00001810: 653d 2273 7472 6f6b 653a 2024 706c 616e  e="stroke: $plan
-00001820: 6574 735f 636f 6c6f 725f 333b 2073 7472  ets_color_3; str
-00001830: 6f6b 652d 7769 6474 683a 2032 7078 3b20  oke-width: 2px; 
-00001840: 6669 6c6c 3a20 6e6f 6e65 220a 2020 2020  fill: none".    
-00001850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001860: 2020 2020 2020 2020 2f3e 0a20 2020 2020          />.     
-00001870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001880: 2020 203c 2f67 3e0a 2020 2020 2020 2020     </g>.        
-00001890: 2020 2020 2020 2020 2020 2020 3c2f 673e              </g>
-000018a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000018b0: 203c 2f73 796d 626f 6c3e 0a20 2020 2020   </symbol>.     
-000018c0: 2020 2020 2020 2020 2020 203c 7379 6d62             <symb
-000018d0: 6f6c 2069 643d 224d 6172 7322 3e0a 2020  ol id="Mars">.  
-000018e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018f0: 2020 3c67 2074 7261 6e73 666f 726d 3d22    <g transform="
-00001900: 7472 616e 736c 6174 6528 312c 3329 223e  translate(1,3)">
+000010a0: 2020 2020 2020 2064 3d22 4d20 3132 2e34         d="M 12.4
+000010b0: 3137 3930 382c 3131 2e30 3937 3530 3720  17908,11.097507 
+000010c0: 4320 3132 2e34 3630 3831 382c 3133 2e36  C 12.460818,13.6
+000010d0: 3034 3931 3620 3130 2e36 3638 3231 372c  04916 10.668217,
+000010e0: 3135 2e39 3936 3635 3620 382e 3235 3636  15.996656 8.2566
+000010f0: 3830 352c 3136 2e36 3736 3633 3920 4320  805,16.676639 C 
+00001100: 362e 3131 3830 3337 352c 3137 2e33 3232  6.1180375,17.322
+00001110: 3532 3220 332e 3634 3038 3637 352c 3136  522 3.6408675,16
+00001120: 2e36 3131 3836 3920 322e 3139 3930 3931  .611869 2.199091
+00001130: 352c 3134 2e38 3937 3032 3520 4320 302e  5,14.897025 C 0.
+00001140: 3730 3235 3133 3531 2c31 332e 3138 3538  70251351,13.1858
+00001150: 3934 2030 2e33 3437 3035 3535 312c 3130  94 0.34705551,10
+00001160: 2e35 3734 3134 3920 312e 3337 3837 3833  .574149 1.378783
+00001170: 352c 382e 3534 3036 3337 2043 2032 2e33  5,8.540637 C 2.3
+00001180: 3330 3930 3635 2c36 2e35 3737 3831 3936  309065,6.5778196
+00001190: 2034 2e34 3434 3839 3235 2c35 2e32 3339   4.4448925,5.239
+000011a0: 3035 3135 2036 2e36 3334 3433 3835 2c35  0515 6.6344385,5
+000011b0: 2e32 3830 3138 3132 2043 2038 2e37 3433  .2801812 C 8.743
+000011c0: 3634 3835 2c35 2e32 3830 3831 3834 2031  6485,5.2808184 1
+000011d0: 302e 3739 3732 312c 362e 3531 3834 3839  0.79721,6.518489
+000011e0: 3720 3131 2e37 3535 3634 312c 382e 3430  7 11.755641,8.40
+000011f0: 3134 3232 3920 4320 3132 2e31 3838 3730  14229 C 12.18870
+00001200: 392c 392e 3232 3933 3536 3320 3132 2e34  9,9.2293563 12.4
+00001210: 3231 3932 362c 3130 2e31 3632 3536 3820  21926,10.162568 
+00001220: 3132 2e34 3137 3930 382c 3131 2e30 3937  12.417908,11.097
+00001230: 3530 3720 7a20 4d20 3131 2e35 3337 3534  507 z M 11.53754
+00001240: 392c 302e 3739 3437 3737 3536 2043 2031  9,0.79477756 C 1
+00001250: 312e 3336 3830 3131 2c32 2e39 3533 3136  1.368011,2.95316
+00001260: 3336 2039 2e35 3932 3831 3035 2c34 2e38  36 9.5928105,4.8
+00001270: 3439 3339 3420 372e 3435 3238 3435 352c  49394 7.4528455,
+00001280: 352e 3137 3131 3237 2043 2035 2e34 3933  5.171127 C 5.493
+00001290: 3430 3335 2c35 2e35 3035 3834 3637 2033  4035,5.5058467 3
+000012a0: 2e33 3633 3435 3035 2c34 2e35 3439 3436  .3634505,4.54946
+000012b0: 3836 2032 2e33 3935 3831 3335 2c32 2e37  86 2.3958135,2.7
+000012c0: 3934 3635 3836 2043 2032 2e30 3434 3831  946586 C 2.04481
+000012d0: 3535 2c32 2e31 3831 3837 3436 2031 2e38  55,2.1818746 1.8
+000012e0: 3237 3537 3535 2c31 2e34 3933 3039 3636  275755,1.4930966
+000012f0: 2031 2e37 3632 3638 3435 2c30 2e37 3839   1.7626845,0.789
+00001300: 3933 3735 3620 4d20 362e 3630 3339 3632  93756 M 6.603962
+00001310: 352c 3136 2e38 3930 3531 3820 4320 362e  5,16.890518 C 6.
+00001320: 3630 3339 3632 352c 3138 2e39 3937 3033  6039625,18.99703
+00001330: 3120 362e 3630 3339 3632 352c 3231 2e31  1 6.6039625,21.1
+00001340: 3033 3534 3520 362e 3630 3339 3632 352c  03545 6.6039625,
+00001350: 3233 2e32 3130 3035 3820 4d20 332e 3937  23.210058 M 3.97
+00001360: 3038 3231 352c 3230 2e35 3736 3931 3620  08215,20.576916 
+00001370: 4320 352e 3732 3632 3437 352c 3230 2e35  C 5.7262475,20.5
+00001380: 3736 3931 3620 372e 3438 3136 3738 352c  76916 7.4816785,
+00001390: 3230 2e35 3736 3931 3620 392e 3233 3731  20.576916 9.2371
+000013a0: 3034 352c 3230 2e35 3736 3931 3622 0a20  045,20.576916". 
+000013b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013c0: 2020 2020 2020 2020 2020 2073 7479 6c65             style
+000013d0: 3d22 7374 726f 6b65 3a20 2470 6c61 6e65  ="stroke: $plane
+000013e0: 7473 5f63 6f6c 6f72 5f32 3b20 7374 726f  ts_color_2; stro
+000013f0: 6b65 2d77 6964 7468 3a20 3270 783b 2066  ke-width: 2px; f
+00001400: 696c 6c3a 206e 6f6e 6522 0a20 2020 2020  ill: none".     
+00001410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001420: 2020 202f 3e0a 2020 2020 2020 2020 2020     />.          
+00001430: 2020 2020 2020 2020 2020 3c2f 673e 0a20            </g>. 
+00001440: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001450: 2f73 796d 626f 6c3e 0a20 2020 2020 2020  /symbol>.       
+00001460: 2020 2020 2020 2020 203c 7379 6d62 6f6c           <symbol
+00001470: 2069 643d 2256 656e 7573 223e 0a20 2020   id="Venus">.   
+00001480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001490: 203c 6720 7472 616e 7366 6f72 6d3d 2274   <g transform="t
+000014a0: 7261 6e73 6c61 7465 2830 2c32 2922 3e0a  ranslate(0,2)">.
+000014b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014c0: 2020 2020 2020 2020 3c67 2074 7261 6e73          <g trans
+000014d0: 666f 726d 3d22 7363 616c 6528 2e39 2922  form="scale(.9)"
+000014e0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000014f0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+00001500: 6174 680a 2020 2020 2020 2020 2020 2020  ath.            
+00001510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001520: 2020 2020 643d 224d 2031 382e 3430 3037      d="M 18.4007
+00001530: 3033 2c37 2e33 3636 3734 3833 2043 2031  03,7.3667483 C 1
+00001540: 382e 3432 3339 362c 392e 3636 3535 3332  8.42396,9.665532
+00001550: 3920 3137 2e31 3730 3130 322c 3131 2e39  9 17.170102,11.9
+00001560: 3134 3537 3920 3135 2e32 3138 3937 322c  14579 15.218972,
+00001570: 3133 2e31 3133 3732 3820 4320 3133 2e31  13.113728 C 13.1
+00001580: 3632 3435 392c 3134 2e34 3237 3235 3320  62459,14.427253 
+00001590: 3130 2e33 3839 3835 352c 3134 2e34 3736  10.389855,14.476
+000015a0: 3737 3220 382e 3238 3731 3636 332c 3133  772 8.2871663,13
+000015b0: 2e32 3339 3730 3920 4320 362e 3237 3335  .239709 C 6.2735
+000015c0: 3835 312c 3132 2e31 3030 3532 3420 342e  851,12.100524 4.
+000015d0: 3933 3336 3333 2c39 2e38 3634 3033 3233  933633,9.8640323
+000015e0: 2034 2e38 3937 3939 3135 2c37 2e35 3431   4.8979915,7.541
+000015f0: 3438 3034 2043 2034 2e38 3137 3336 3137  4804 C 4.8173617
+00001600: 2c35 2e32 3637 3835 3932 2035 2e39 3835  ,5.2678592 5.985
+00001610: 3531 3936 2c33 2e30 3039 3030 3031 2037  5196,3.0090001 7
+00001620: 2e38 3732 3838 3037 2c31 2e37 3533 3034  .8728807,1.75304
+00001630: 3731 2043 2039 2e38 3830 3339 3135 2c30  71 C 9.8803915,0
+00001640: 2e33 3635 3039 3534 3620 3132 2e36 3438  .36509546 12.648
+00001650: 3930 362c 302e 3231 3635 3731 3436 2031  906,0.21657146 1
+00001660: 342e 3739 3438 3439 2c31 2e33 3735 3238  4.794849,1.37528
+00001670: 3331 2043 2031 362e 3836 3937 3732 2c32  31 C 16.869772,2
+00001680: 2e34 3531 3436 3333 2031 382e 3239 3632  .4514633 18.2962
+00001690: 3431 2c34 2e36 3733 3134 3533 2031 382e  41,4.6731453 18.
+000016a0: 3339 3139 3138 2c37 2e30 3138 3337 3233  391918,7.0183723
+000016b0: 2043 2031 382e 3339 3737 3831 2c37 2e31   C 18.397781,7.1
+000016c0: 3334 3339 3633 2031 382e 3430 3037 3033  343963 18.400703
+000016d0: 2c37 2e32 3530 3537 3233 2031 382e 3430  ,7.2505723 18.40
+000016e0: 3037 3033 2c37 2e33 3636 3734 3833 207a  0703,7.3667483 z
+000016f0: 204d 2031 312e 3634 3832 3839 2c31 342e   M 11.648289,14.
+00001700: 3133 3636 3839 2043 2031 312e 3634 3832  136689 C 11.6482
+00001710: 3839 2c31 372e 3030 3837 3634 2031 312e  89,17.008764 11.
+00001720: 3634 3832 3839 2c31 392e 3838 3038 3420  648289,19.88084 
+00001730: 3131 2e36 3438 3238 392c 3232 2e37 3532  11.648289,22.752
+00001740: 3931 3520 4d20 372e 3936 3531 3333 332c  915 M 7.9651333,
+00001750: 3139 2e30 3630 3234 3320 4320 3130 2e34  19.060243 C 10.4
+00001760: 3230 3537 2c31 392e 3036 3032 3433 2031  2057,19.060243 1
+00001770: 322e 3837 3630 3038 2c31 392e 3036 3032  2.876008,19.0602
+00001780: 3433 2031 352e 3333 3134 3434 2c31 392e  43 15.331444,19.
+00001790: 3036 3032 3433 220a 2020 2020 2020 2020  060243".        
+000017a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017b0: 2020 2020 2020 2020 7374 796c 653d 2273          style="s
+000017c0: 7472 6f6b 653a 2024 706c 616e 6574 735f  troke: $planets_
+000017d0: 636f 6c6f 725f 333b 2073 7472 6f6b 652d  color_3; stroke-
+000017e0: 7769 6474 683a 2032 7078 3b20 6669 6c6c  width: 2px; fill
+000017f0: 3a20 6e6f 6e65 220a 2020 2020 2020 2020  : none".        
+00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001810: 2020 2020 2f3e 0a20 2020 2020 2020 2020      />.         
+00001820: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001830: 2f67 3e0a 2020 2020 2020 2020 2020 2020  /g>.            
+00001840: 2020 2020 2020 2020 3c2f 673e 0a20 2020          </g>.   
+00001850: 2020 2020 2020 2020 2020 2020 203c 2f73               </s
+00001860: 796d 626f 6c3e 0a20 2020 2020 2020 2020  ymbol>.         
+00001870: 2020 2020 2020 203c 7379 6d62 6f6c 2069         <symbol i
+00001880: 643d 224d 6172 7322 3e0a 2020 2020 2020  d="Mars">.      
+00001890: 2020 2020 2020 2020 2020 2020 2020 3c67                <g
+000018a0: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
+000018b0: 736c 6174 6528 312c 3329 223e 0a20 2020  slate(1,3)">.   
+000018c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018d0: 2020 2020 203c 6720 7472 616e 7366 6f72       <g transfor
+000018e0: 6d3d 2273 6361 6c65 282e 3929 223e 0a20  m="scale(.9)">. 
+000018f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001900: 2020 2020 2020 2020 2020 203c 7061 7468             <path
 00001910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001920: 2020 2020 2020 2020 203c 6720 7472 616e           <g tran
-00001930: 7366 6f72 6d3d 2273 6361 6c65 282e 3929  sform="scale(.9)
-00001940: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00001950: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001960: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
-00001970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001980: 2020 2020 2064 3d22 4d20 3139 2e38 3336       d="M 19.836
-00001990: 3832 382c 312e 3232 3638 3538 3520 4320  828,1.2268585 C 
-000019a0: 3137 2e34 3234 3432 322c 332e 3632 3538  17.424422,3.6258
-000019b0: 3737 3620 3135 2e30 3132 3030 382c 362e  776 15.012008,6.
-000019c0: 3032 3439 3034 3720 3132 2e35 3939 3539  0249047 12.59959
-000019d0: 342c 382e 3432 3339 3331 3720 4d20 3133  4,8.4239317 M 13
-000019e0: 2e35 3836 3133 312c 312e 3330 3332 3835  .586131,1.303285
-000019f0: 3320 4320 3135 2e36 3431 3632 322c 312e  3 C 15.641622,1.
-00001a00: 3330 3332 3835 3320 3137 2e36 3937 3130  3032853 17.69710
-00001a10: 352c 312e 3330 3332 3835 3320 3139 2e37  5,1.3032853 19.7
-00001a20: 3532 3539 352c 312e 3330 3332 3835 3320  52595,1.3032853 
-00001a30: 4320 3139 2e37 3532 3539 352c 332e 3334  C 19.752595,3.34
-00001a40: 3733 3638 3620 3139 2e37 3532 3630 332c  73686 19.752603,
-00001a50: 352e 3339 3134 3531 3720 3139 2e37 3532  5.3914517 19.752
-00001a60: 3630 332c 372e 3433 3535 3335 3722 0a20  603,7.4355357". 
-00001a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001a90: 7479 6c65 3d22 7374 726f 6b65 3a20 2470  tyle="stroke: $p
-00001aa0: 6c61 6e65 7473 5f63 6f6c 6f72 5f34 3b20  lanets_color_4; 
-00001ab0: 7374 726f 6b65 2d77 6964 7468 3a20 3270  stroke-width: 2p
-00001ac0: 783b 2066 696c 6c3a 206e 6f6e 6522 0a20  x; fill: none". 
-00001ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ae0: 2020 2020 2020 2020 2020 202f 3e0a 2020             />.  
-00001af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b00: 2020 2020 2020 2020 2020 3c70 6174 680a            <path.
-00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b30: 643d 224d 2031 352e 3230 3838 3335 2c31  d="M 15.208835,1
-00001b40: 332e 3133 3737 3131 2043 2031 352e 3234  3.137711 C 15.24
-00001b50: 3537 3837 2c31 352e 3838 3833 3039 2031  5787,15.888309 1
-00001b60: 332e 3439 3735 3233 2c31 382e 3534 3334  3.497523,18.5434
-00001b70: 3620 3130 2e39 3639 3034 332c 3139 2e36  6 10.969043,19.6
-00001b80: 3137 3733 2043 2038 2e34 3538 3431 3735  1773 C 8.4584175
-00001b90: 2c32 302e 3734 3930 3336 2035 2e33 3135  ,20.749036 5.315
-00001ba0: 3534 3238 2c32 302e 3231 3634 3120 332e  5428,20.21641 3.
-00001bb0: 3332 3336 3330 362c 3138 2e33 3132 3834  3236306,18.31284
-00001bc0: 3320 4320 312e 3332 3934 3738 392c 3136  3 C 1.3294789,16
-00001bd0: 2e35 3032 3638 3620 302e 3535 3436 3631  .502686 0.554661
-00001be0: 3237 2c31 332e 3530 3436 3738 2031 2e34  27,13.504678 1.4
-00001bf0: 3133 3336 3135 2c31 302e 3935 3333 3032  133615,10.953302
-00001c00: 2043 2032 2e32 3438 3537 3231 2c38 2e32   C 2.2485721,8.2
-00001c10: 3833 3334 3532 2034 2e38 3030 3530 3433  833452 4.8005043
-00001c20: 2c36 2e32 3636 3030 3735 2037 2e35 3935  ,6.2660075 7.595
-00001c30: 3231 382c 362e 3038 3834 3236 3620 4320  218,6.0884266 C 
-00001c40: 3130 2e32 3837 3033 322c 352e 3834 3637  10.287032,5.8467
-00001c50: 3938 3420 3133 2e30 3232 3334 382c 372e  984 13.022348,7.
-00001c60: 3332 3331 3034 3820 3134 2e33 3133 3836  3231048 14.31386
-00001c70: 2c39 2e36 3933 3830 3831 2043 2031 342e  ,9.6938081 C 14.
-00001c80: 3930 3131 3633 2c31 302e 3733 3939 3637  901163,10.739967
-00001c90: 2031 352e 3231 3130 3832 2c31 312e 3933   15.211082,11.93
-00001ca0: 3831 3936 2031 352e 3230 3838 3335 2c31  8196 15.208835,1
-00001cb0: 332e 3133 3737 3131 207a 220a 2020 2020  3.137711 z".    
-00001cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cd0: 2020 2020 2020 2020 2020 2020 7374 796c              styl
-00001ce0: 653d 2273 7472 6f6b 653a 2024 706c 616e  e="stroke: $plan
-00001cf0: 6574 735f 636f 6c6f 725f 343b 2073 7472  ets_color_4; str
-00001d00: 6f6b 652d 7769 6474 683a 2032 7078 3b20  oke-width: 2px; 
-00001d10: 6669 6c6c 3a20 6e6f 6e65 220a 2020 2020  fill: none".    
-00001d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d30: 2020 2020 2020 2020 2f3e 0a20 2020 2020          />.     
-00001d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d50: 2020 203c 2f67 3e0a 2020 2020 2020 2020     </g>.        
-00001d60: 2020 2020 2020 2020 2020 2020 3c2f 673e              </g>
-00001d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001d80: 203c 2f73 796d 626f 6c3e 0a20 2020 2020   </symbol>.     
-00001d90: 2020 2020 2020 2020 2020 203c 7379 6d62             <symb
-00001da0: 6f6c 2069 643d 224a 7570 6974 6572 223e  ol id="Jupiter">
-00001db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001dc0: 2020 2020 203c 6720 7472 616e 7366 6f72       <g transfor
-00001dd0: 6d3d 2274 7261 6e73 6c61 7465 2831 2c33  m="translate(1,3
-00001de0: 2922 3e0a 2020 2020 2020 2020 2020 2020  )">.            
-00001df0: 2020 2020 2020 2020 2020 2020 3c67 2074              <g t
-00001e00: 7261 6e73 666f 726d 3d22 7363 616c 6528  ransform="scale(
-00001e10: 2e39 2922 3e0a 2020 2020 2020 2020 2020  .9)">.          
-00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e30: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
-00001e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e50: 2020 2020 2020 2020 643d 224d 2031 362e          d="M 16.
-00001e60: 3930 3330 3038 2c30 2e39 3938 3439 3135  903008,0.9984915
-00001e70: 3720 4c20 3136 2e39 3033 3030 382c 3233  7 L 16.903008,23
-00001e80: 2e30 3031 3531 3220 4d20 3230 2e35 3330  .001512 M 20.530
-00001e90: 3237 382c 3137 2e33 3539 3731 3220 4c20  278,17.359712 L 
-00001ea0: 322e 3939 3834 3838 342c 3137 2e33 3539  2.9984884,17.359
-00001eb0: 3731 3220 4d20 342e 3831 3231 3138 342c  712 M 4.8121184,
-00001ec0: 382e 3839 3730 3132 2043 2034 2e32 3037  8.897012 C 4.207
-00001ed0: 3537 3834 2c38 2e38 3937 3031 3220 322e  5784,8.897012 2.
-00001ee0: 3939 3834 3838 342c 382e 3333 3238 3332  9984884,8.332832
-00001ef0: 2032 2e39 3938 3438 3834 2c36 2e30 3736   2.9984884,6.076
-00001f00: 3131 3220 4320 322e 3939 3834 3838 342c  112 C 2.9984884,
-00001f10: 332e 3831 3933 3832 2035 2e34 3136 3636  3.819382 5.41666
-00001f20: 3834 2c31 2e35 3632 3637 3136 2037 2e38  84,1.5626716 7.8
-00001f30: 3334 3834 3834 2c31 2e35 3632 3637 3136  348484,1.5626716
-00001f40: 2043 2031 302e 3235 3330 3238 2c31 2e35   C 10.253028,1.5
-00001f50: 3632 3637 3136 2031 322e 3637 3131 3938  626716 12.671198
-00001f60: 2c33 2e32 3535 3231 3220 3132 2e36 3731  ,3.255212 12.671
-00001f70: 3139 382c 372e 3230 3434 3732 2043 2031  198,7.204472 C 1
-00001f80: 322e 3637 3131 3938 2c31 312e 3135 3337  2.671198,11.1537
-00001f90: 3332 2039 2e36 3438 3437 3834 2c31 372e  32 9.6484784,17.
-00001fa0: 3335 3937 3132 2033 2e36 3033 3032 3834  359712 3.6030284
-00001fb0: 2c31 372e 3335 3937 3132 220a 2020 2020  ,17.359712".    
-00001fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fd0: 2020 2020 2020 2020 2020 2020 7374 796c              styl
-00001fe0: 653d 2273 7472 6f6b 653a 2024 706c 616e  e="stroke: $plan
-00001ff0: 6574 735f 636f 6c6f 725f 353b 2073 7472  ets_color_5; str
-00002000: 6f6b 652d 7769 6474 683a 2032 7078 3b20  oke-width: 2px; 
-00002010: 6669 6c6c 3a20 6e6f 6e65 220a 2020 2020  fill: none".    
-00002020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002030: 2020 2020 2020 2020 2f3e 0a20 2020 2020          />.     
-00002040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002050: 2020 203c 2f67 3e0a 2020 2020 2020 2020     </g>.        
-00002060: 2020 2020 2020 2020 2020 2020 3c2f 673e              </g>
-00002070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002080: 203c 2f73 796d 626f 6c3e 0a20 2020 2020   </symbol>.     
-00002090: 2020 2020 2020 2020 2020 203c 7379 6d62             <symb
-000020a0: 6f6c 2069 643d 2253 6174 7572 6e22 3e0a  ol id="Saturn">.
+00001920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001930: 2064 3d22 4d20 3139 2e38 3336 3832 382c   d="M 19.836828,
+00001940: 312e 3232 3638 3538 3520 4320 3137 2e34  1.2268585 C 17.4
+00001950: 3234 3432 322c 332e 3632 3538 3737 3620  24422,3.6258776 
+00001960: 3135 2e30 3132 3030 382c 362e 3032 3439  15.012008,6.0249
+00001970: 3034 3720 3132 2e35 3939 3539 342c 382e  047 12.599594,8.
+00001980: 3432 3339 3331 3720 4d20 3133 2e35 3836  4239317 M 13.586
+00001990: 3133 312c 312e 3330 3332 3835 3320 4320  131,1.3032853 C 
+000019a0: 3135 2e36 3431 3632 322c 312e 3330 3332  15.641622,1.3032
+000019b0: 3835 3320 3137 2e36 3937 3130 352c 312e  853 17.697105,1.
+000019c0: 3330 3332 3835 3320 3139 2e37 3532 3539  3032853 19.75259
+000019d0: 352c 312e 3330 3332 3835 3320 4320 3139  5,1.3032853 C 19
+000019e0: 2e37 3532 3539 352c 332e 3334 3733 3638  .752595,3.347368
+000019f0: 3620 3139 2e37 3532 3630 332c 352e 3339  6 19.752603,5.39
+00001a00: 3134 3531 3720 3139 2e37 3532 3630 332c  14517 19.752603,
+00001a10: 372e 3433 3535 3335 3722 0a20 2020 2020  7.4355357".     
+00001a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a30: 2020 2020 2020 2020 2020 2073 7479 6c65             style
+00001a40: 3d22 7374 726f 6b65 3a20 2470 6c61 6e65  ="stroke: $plane
+00001a50: 7473 5f63 6f6c 6f72 5f34 3b20 7374 726f  ts_color_4; stro
+00001a60: 6b65 2d77 6964 7468 3a20 3270 783b 2066  ke-width: 2px; f
+00001a70: 696c 6c3a 206e 6f6e 6522 0a20 2020 2020  ill: none".     
+00001a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a90: 2020 2020 2020 202f 3e0a 2020 2020 2020         />.      
+00001aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ab0: 2020 2020 2020 3c70 6174 680a 2020 2020        <path.    
+00001ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ad0: 2020 2020 2020 2020 2020 2020 643d 224d              d="M
+00001ae0: 2031 352e 3230 3838 3335 2c31 332e 3133   15.208835,13.13
+00001af0: 3737 3131 2043 2031 352e 3234 3537 3837  7711 C 15.245787
+00001b00: 2c31 352e 3838 3833 3039 2031 332e 3439  ,15.888309 13.49
+00001b10: 3735 3233 2c31 382e 3534 3334 3620 3130  7523,18.54346 10
+00001b20: 2e39 3639 3034 332c 3139 2e36 3137 3733  .969043,19.61773
+00001b30: 2043 2038 2e34 3538 3431 3735 2c32 302e   C 8.4584175,20.
+00001b40: 3734 3930 3336 2035 2e33 3135 3534 3238  749036 5.3155428
+00001b50: 2c32 302e 3231 3634 3120 332e 3332 3336  ,20.21641 3.3236
+00001b60: 3330 362c 3138 2e33 3132 3834 3320 4320  306,18.312843 C 
+00001b70: 312e 3332 3934 3738 392c 3136 2e35 3032  1.3294789,16.502
+00001b80: 3638 3620 302e 3535 3436 3631 3237 2c31  686 0.55466127,1
+00001b90: 332e 3530 3436 3738 2031 2e34 3133 3336  3.504678 1.41336
+00001ba0: 3135 2c31 302e 3935 3333 3032 2043 2032  15,10.953302 C 2
+00001bb0: 2e32 3438 3537 3231 2c38 2e32 3833 3334  .2485721,8.28334
+00001bc0: 3532 2034 2e38 3030 3530 3433 2c36 2e32  52 4.8005043,6.2
+00001bd0: 3636 3030 3735 2037 2e35 3935 3231 382c  660075 7.595218,
+00001be0: 362e 3038 3834 3236 3620 4320 3130 2e32  6.0884266 C 10.2
+00001bf0: 3837 3033 322c 352e 3834 3637 3938 3420  87032,5.8467984 
+00001c00: 3133 2e30 3232 3334 382c 372e 3332 3331  13.022348,7.3231
+00001c10: 3034 3820 3134 2e33 3133 3836 2c39 2e36  048 14.31386,9.6
+00001c20: 3933 3830 3831 2043 2031 342e 3930 3131  938081 C 14.9011
+00001c30: 3633 2c31 302e 3733 3939 3637 2031 352e  63,10.739967 15.
+00001c40: 3231 3130 3832 2c31 312e 3933 3831 3936  211082,11.938196
+00001c50: 2031 352e 3230 3838 3335 2c31 332e 3133   15.208835,13.13
+00001c60: 3737 3131 207a 220a 2020 2020 2020 2020  7711 z".        
+00001c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c80: 2020 2020 2020 2020 7374 796c 653d 2273          style="s
+00001c90: 7472 6f6b 653a 2024 706c 616e 6574 735f  troke: $planets_
+00001ca0: 636f 6c6f 725f 343b 2073 7472 6f6b 652d  color_4; stroke-
+00001cb0: 7769 6474 683a 2032 7078 3b20 6669 6c6c  width: 2px; fill
+00001cc0: 3a20 6e6f 6e65 220a 2020 2020 2020 2020  : none".        
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ce0: 2020 2020 2f3e 0a20 2020 2020 2020 2020      />.         
+00001cf0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001d00: 2f67 3e0a 2020 2020 2020 2020 2020 2020  /g>.            
+00001d10: 2020 2020 2020 2020 3c2f 673e 0a20 2020          </g>.   
+00001d20: 2020 2020 2020 2020 2020 2020 203c 2f73               </s
+00001d30: 796d 626f 6c3e 0a20 2020 2020 2020 2020  ymbol>.         
+00001d40: 2020 2020 2020 203c 7379 6d62 6f6c 2069         <symbol i
+00001d50: 643d 224a 7570 6974 6572 223e 0a20 2020  d="Jupiter">.   
+00001d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d70: 203c 6720 7472 616e 7366 6f72 6d3d 2274   <g transform="t
+00001d80: 7261 6e73 6c61 7465 2831 2c33 2922 3e0a  ranslate(1,3)">.
+00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001da0: 2020 2020 2020 2020 3c67 2074 7261 6e73          <g trans
+00001db0: 666f 726d 3d22 7363 616c 6528 2e39 2922  form="scale(.9)"
+00001dc0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001dd0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+00001de0: 6174 680a 2020 2020 2020 2020 2020 2020  ath.            
+00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e00: 2020 2020 643d 224d 2031 362e 3930 3330      d="M 16.9030
+00001e10: 3038 2c30 2e39 3938 3439 3135 3720 4c20  08,0.99849157 L 
+00001e20: 3136 2e39 3033 3030 382c 3233 2e30 3031  16.903008,23.001
+00001e30: 3531 3220 4d20 3230 2e35 3330 3237 382c  512 M 20.530278,
+00001e40: 3137 2e33 3539 3731 3220 4c20 322e 3939  17.359712 L 2.99
+00001e50: 3834 3838 342c 3137 2e33 3539 3731 3220  84884,17.359712 
+00001e60: 4d20 342e 3831 3231 3138 342c 382e 3839  M 4.8121184,8.89
+00001e70: 3730 3132 2043 2034 2e32 3037 3537 3834  7012 C 4.2075784
+00001e80: 2c38 2e38 3937 3031 3220 322e 3939 3834  ,8.897012 2.9984
+00001e90: 3838 342c 382e 3333 3238 3332 2032 2e39  884,8.332832 2.9
+00001ea0: 3938 3438 3834 2c36 2e30 3736 3131 3220  984884,6.076112 
+00001eb0: 4320 322e 3939 3834 3838 342c 332e 3831  C 2.9984884,3.81
+00001ec0: 3933 3832 2035 2e34 3136 3636 3834 2c31  9382 5.4166684,1
+00001ed0: 2e35 3632 3637 3136 2037 2e38 3334 3834  .5626716 7.83484
+00001ee0: 3834 2c31 2e35 3632 3637 3136 2043 2031  84,1.5626716 C 1
+00001ef0: 302e 3235 3330 3238 2c31 2e35 3632 3637  0.253028,1.56267
+00001f00: 3136 2031 322e 3637 3131 3938 2c33 2e32  16 12.671198,3.2
+00001f10: 3535 3231 3220 3132 2e36 3731 3139 382c  55212 12.671198,
+00001f20: 372e 3230 3434 3732 2043 2031 322e 3637  7.204472 C 12.67
+00001f30: 3131 3938 2c31 312e 3135 3337 3332 2039  1198,11.153732 9
+00001f40: 2e36 3438 3437 3834 2c31 372e 3335 3937  .6484784,17.3597
+00001f50: 3132 2033 2e36 3033 3032 3834 2c31 372e  12 3.6030284,17.
+00001f60: 3335 3937 3132 220a 2020 2020 2020 2020  359712".        
+00001f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f80: 2020 2020 2020 2020 7374 796c 653d 2273          style="s
+00001f90: 7472 6f6b 653a 2024 706c 616e 6574 735f  troke: $planets_
+00001fa0: 636f 6c6f 725f 353b 2073 7472 6f6b 652d  color_5; stroke-
+00001fb0: 7769 6474 683a 2032 7078 3b20 6669 6c6c  width: 2px; fill
+00001fc0: 3a20 6e6f 6e65 220a 2020 2020 2020 2020  : none".        
+00001fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fe0: 2020 2020 2f3e 0a20 2020 2020 2020 2020      />.         
+00001ff0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00002000: 2f67 3e0a 2020 2020 2020 2020 2020 2020  /g>.            
+00002010: 2020 2020 2020 2020 3c2f 673e 0a20 2020          </g>.   
+00002020: 2020 2020 2020 2020 2020 2020 203c 2f73               </s
+00002030: 796d 626f 6c3e 0a20 2020 2020 2020 2020  ymbol>.         
+00002040: 2020 2020 2020 203c 7379 6d62 6f6c 2069         <symbol i
+00002050: 643d 2253 6174 7572 6e22 3e0a 2020 2020  d="Saturn">.    
+00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002070: 3c67 2074 7261 6e73 666f 726d 3d22 7472  <g transform="tr
+00002080: 616e 736c 6174 6528 312c 3229 223e 0a20  anslate(1,2)">. 
+00002090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020a0: 2020 2020 2020 203c 7061 7468 0a20 2020         <path.   
 000020b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020c0: 2020 2020 3c67 2074 7261 6e73 666f 726d      <g transform
-000020d0: 3d22 7472 616e 736c 6174 6528 312c 3229  ="translate(1,2)
-000020e0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-000020f0: 2020 2020 2020 2020 2020 203c 7061 7468             <path
-00002100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002110: 2020 2020 2020 2020 2020 2020 2064 3d22               d="
-00002120: 4d20 382e 3338 3434 3334 392c 302e 3930  M 8.3844349,0.90
-00002130: 3230 3332 3331 204c 2038 2e33 3834 3433  203231 L 8.38443
-00002140: 3439 2c31 382e 3239 3838 3532 204d 2035  49,18.298852 M 5
-00002150: 2e34 3334 3934 3439 2c33 2e37 3531 3531  .4349449,3.75151
-00002160: 3233 204c 2031 322e 3636 3837 3435 2c33  23 L 12.668745,3
-00002170: 2e37 3531 3531 3233 204d 2031 362e 3832  .7515123 M 16.82
-00002180: 3338 3735 2c32 312e 3839 3831 3932 2043  3875,21.898192 C
-00002190: 2031 362e 3232 3130 3535 2c32 322e 3439   16.221055,22.49
-000021a0: 3830 3832 2031 352e 3631 3832 3335 2c32  8082 15.618235,2
-000021b0: 332e 3039 3739 3732 2031 352e 3031 3534  3.097972 15.0154
-000021c0: 3135 2c32 332e 3039 3739 3732 2043 2031  15,23.097972 C 1
-000021d0: 342e 3431 3236 3035 2c32 332e 3039 3739  4.412605,23.0979
-000021e0: 3732 2031 332e 3230 3639 3735 2c32 322e  72 13.206975,22.
-000021f0: 3439 3830 3832 2031 332e 3230 3639 3735  498082 13.206975
-00002200: 2c32 312e 3239 3833 3032 2043 2031 332e  ,21.298302 C 13.
-00002210: 3230 3639 3735 2c32 302e 3039 3835 3232  206975,20.098522
-00002220: 2031 332e 3830 3937 3835 2c31 382e 3839   13.809785,18.89
-00002230: 3837 3432 2031 352e 3031 3534 3135 2c31  8742 15.015415,1
-00002240: 372e 3639 3839 3632 2043 2031 362e 3232  7.698962 C 16.22
-00002250: 3130 3535 2c31 362e 3439 3931 3832 2031  1055,16.499182 1
-00002260: 372e 3432 3636 3835 2c31 342e 3039 3936  7.426685,14.0996
-00002270: 3232 2031 372e 3432 3636 3835 2c31 312e  22 17.426685,11.
-00002280: 3730 3030 3532 2043 2031 372e 3432 3636  700052 C 17.4266
-00002290: 3835 2c39 2e33 3030 3439 3233 2031 362e  85,9.3004923 16.
-000022a0: 3232 3130 3535 2c36 2e39 3030 3933 3233  221055,6.9009323
-000022b0: 2031 332e 3830 3937 3835 2c36 2e39 3030   13.809785,6.900
-000022c0: 3933 3233 2043 2031 312e 3532 3932 3135  9323 C 11.529215
-000022d0: 2c36 2e39 3030 3933 3233 2039 2e35 3930  ,6.9009323 9.590
-000022e0: 3036 3439 2c38 2e31 3030 3731 3233 2038  0649,8.1007123 8
-000022f0: 2e33 3834 3433 3439 2c31 302e 3530 3032  .3844349,10.5002
-00002300: 3832 220a 2020 2020 2020 2020 2020 2020  82".            
+000020c0: 2020 2020 2020 2020 2064 3d22 4d20 382e           d="M 8.
+000020d0: 3338 3434 3334 392c 302e 3930 3230 3332  3844349,0.902032
+000020e0: 3331 204c 2038 2e33 3834 3433 3439 2c31  31 L 8.3844349,1
+000020f0: 382e 3239 3838 3532 204d 2035 2e34 3334  8.298852 M 5.434
+00002100: 3934 3439 2c33 2e37 3531 3531 3233 204c  9449,3.7515123 L
+00002110: 2031 322e 3636 3837 3435 2c33 2e37 3531   12.668745,3.751
+00002120: 3531 3233 204d 2031 362e 3832 3338 3735  5123 M 16.823875
+00002130: 2c32 312e 3839 3831 3932 2043 2031 362e  ,21.898192 C 16.
+00002140: 3232 3130 3535 2c32 322e 3439 3830 3832  221055,22.498082
+00002150: 2031 352e 3631 3832 3335 2c32 332e 3039   15.618235,23.09
+00002160: 3739 3732 2031 352e 3031 3534 3135 2c32  7972 15.015415,2
+00002170: 332e 3039 3739 3732 2043 2031 342e 3431  3.097972 C 14.41
+00002180: 3236 3035 2c32 332e 3039 3739 3732 2031  2605,23.097972 1
+00002190: 332e 3230 3639 3735 2c32 322e 3439 3830  3.206975,22.4980
+000021a0: 3832 2031 332e 3230 3639 3735 2c32 312e  82 13.206975,21.
+000021b0: 3239 3833 3032 2043 2031 332e 3230 3639  298302 C 13.2069
+000021c0: 3735 2c32 302e 3039 3835 3232 2031 332e  75,20.098522 13.
+000021d0: 3830 3937 3835 2c31 382e 3839 3837 3432  809785,18.898742
+000021e0: 2031 352e 3031 3534 3135 2c31 372e 3639   15.015415,17.69
+000021f0: 3839 3632 2043 2031 362e 3232 3130 3535  8962 C 16.221055
+00002200: 2c31 362e 3439 3931 3832 2031 372e 3432  ,16.499182 17.42
+00002210: 3636 3835 2c31 342e 3039 3936 3232 2031  6685,14.099622 1
+00002220: 372e 3432 3636 3835 2c31 312e 3730 3030  7.426685,11.7000
+00002230: 3532 2043 2031 372e 3432 3636 3835 2c39  52 C 17.426685,9
+00002240: 2e33 3030 3439 3233 2031 362e 3232 3130  .3004923 16.2210
+00002250: 3535 2c36 2e39 3030 3933 3233 2031 332e  55,6.9009323 13.
+00002260: 3830 3937 3835 2c36 2e39 3030 3933 3233  809785,6.9009323
+00002270: 2043 2031 312e 3532 3932 3135 2c36 2e39   C 11.529215,6.9
+00002280: 3030 3933 3233 2039 2e35 3930 3036 3439  009323 9.5900649
+00002290: 2c38 2e31 3030 3731 3233 2038 2e33 3834  ,8.1007123 8.384
+000022a0: 3433 3439 2c31 302e 3530 3032 3832 220a  4349,10.500282".
+000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022c0: 2020 2020 2020 2020 2020 2020 7374 796c              styl
+000022d0: 653d 2273 7472 6f6b 653a 2024 706c 616e  e="stroke: $plan
+000022e0: 6574 735f 636f 6c6f 725f 363b 2073 7472  ets_color_6; str
+000022f0: 6f6b 652d 7769 6474 683a 2032 7078 3b20  oke-width: 2px; 
+00002300: 6669 6c6c 3a20 6e6f 6e65 220a 2020 2020  fill: none".    
 00002310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002320: 7374 796c 653d 2273 7472 6f6b 653a 2024  style="stroke: $
-00002330: 706c 616e 6574 735f 636f 6c6f 725f 363b  planets_color_6;
-00002340: 2073 7472 6f6b 652d 7769 6474 683a 2032   stroke-width: 2
-00002350: 7078 3b20 6669 6c6c 3a20 6e6f 6e65 220a  px; fill: none".
-00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002370: 2020 2020 2020 2020 2f3e 0a20 2020 2020          />.     
-00002380: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002390: 2f67 3e0a 2020 2020 2020 2020 2020 2020  /g>.            
-000023a0: 2020 2020 3c2f 7379 6d62 6f6c 3e0a 2020      </symbol>.  
-000023b0: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-000023c0: 796d 626f 6c20 6964 3d22 5572 616e 7573  ymbol id="Uranus
-000023d0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-000023e0: 2020 2020 2020 203c 6720 7472 616e 7366         <g transf
-000023f0: 6f72 6d3d 2274 7261 6e73 6c61 7465 2832  orm="translate(2
-00002400: 2c34 2922 3e0a 2020 2020 2020 2020 2020  ,4)">.          
-00002410: 2020 2020 2020 2020 2020 2020 2020 3c67                <g
-00002420: 2074 7261 6e73 666f 726d 3d22 7363 616c   transform="scal
-00002430: 6528 2e38 2922 3e0a 2020 2020 2020 2020  e(.8)">.        
-00002440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002450: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
-00002460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002470: 2020 2020 2020 2020 2020 643d 224d 2034            d="M 4
-00002480: 2e36 3737 3230 3636 2c31 362e 3039 3734  .6772066,16.0974
-00002490: 3233 2043 2033 2e32 3034 3234 3236 2c31  23 C 3.2042426,1
-000024a0: 362e 3039 3734 3233 2031 2e37 3331 3237  6.097423 1.73127
-000024b0: 3736 2c31 362e 3039 3734 3233 2030 2e32  76,16.097423 0.2
-000024c0: 3538 3330 3636 312c 3136 2e30 3937 3432  5830661,16.09742
-000024d0: 3320 4320 302e 3332 3138 3530 3631 2c31  3 C 0.32185061,1
-000024e0: 352e 3839 3438 3739 2030 2e31 3139 3935  5.894879 0.11995
-000024f0: 3636 312c 3135 2e34 3835 3039 3620 302e  661,15.485096 0.
-00002500: 3337 3937 3633 3631 2c31 352e 3433 3537  37976361,15.4357
-00002510: 3837 2043 2031 2e31 3830 3937 3236 2c31  87 C 1.1809726,1
-00002520: 352e 3233 3534 3835 2031 2e39 3832 3138  5.235485 1.98218
-00002530: 3236 2c31 352e 3033 3531 3832 2032 2e37  26,15.035182 2.7
-00002540: 3833 3339 3236 2c31 342e 3833 3438 3820  833926,14.83488 
-00002550: 4320 322e 3738 3333 3932 362c 3130 2e36  C 2.7833926,10.6
-00002560: 3236 3430 3120 322e 3738 3333 3932 362c  26401 2.7833926,
-00002570: 362e 3431 3739 3239 2032 2e37 3833 3339  6.417929 2.78339
-00002580: 3236 2c32 2e32 3039 3435 3032 2043 2031  26,2.2094502 C 1
-00002590: 2e39 3431 3639 3936 2c31 2e39 3939 3032  .9416996,1.99902
-000025a0: 3835 2031 2e31 3030 3030 3536 2c31 2e37  85 1.1000056,1.7
-000025b0: 3838 3630 3034 2030 2e32 3538 3330 3636  886004 0.2583066
-000025c0: 312c 312e 3537 3831 3738 3720 4320 302e  1,1.5781787 C 0.
-000025d0: 3332 3338 3037 3631 2c31 2e33 3931 3532  32380761,1.39152
-000025e0: 3433 2030 2e31 3135 3730 3236 312c 302e  43 0.11570261,0.
-000025f0: 3933 3132 3634 3332 2030 2e33 3833 3530  93126432 0.38350
-00002600: 3036 312c 302e 3934 3639 3037 3232 2043  061,0.94690722 C
-00002610: 2031 2e38 3134 3733 3736 2c30 2e39 3436   1.8147376,0.946
-00002620: 3930 3732 3220 332e 3234 3539 3639 362c  90722 3.2459696,
-00002630: 302e 3934 3639 3037 3232 2034 2e36 3737  0.94690722 4.677
-00002640: 3230 3636 2c30 2e39 3436 3930 3732 3220  2066,0.94690722 
-00002650: 4320 342e 3637 3732 3036 362c 352e 3939  C 4.6772066,5.99
-00002660: 3730 3739 3220 342e 3637 3732 3036 362c  70792 4.6772066,
-00002670: 3131 2e30 3437 3235 3120 342e 3637 3732  11.047251 4.6772
-00002680: 3036 362c 3136 2e30 3937 3432 3320 7a20  066,16.097423 z 
-00002690: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000026a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026b0: 2020 7374 796c 653d 2273 7472 6f6b 653a    style="stroke:
-000026c0: 2024 706c 616e 6574 735f 636f 6c6f 725f   $planets_color_
-000026d0: 373b 2073 7472 6f6b 652d 7769 6474 683a  7; stroke-width:
-000026e0: 2031 7078 3b20 6669 6c6c 3a20 2470 6c61   1px; fill: $pla
-000026f0: 6e65 7473 5f63 6f6c 6f72 5f35 220a 2020  nets_color_5".  
-00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002710: 2020 2020 2020 2020 2020 2f3e 0a20 2020            />.   
-00002720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002730: 2020 2020 2020 2020 203c 7061 7468 0a20           <path. 
-00002740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002750: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00002760: 3d22 4d20 3138 2e35 3635 3138 2c31 362e  ="M 18.56518,16.
-00002770: 3039 3734 3233 2043 2032 302e 3033 3831  097423 C 20.0381
-00002780: 3531 2c31 362e 3039 3734 3233 2032 312e  51,16.097423 21.
-00002790: 3531 3131 3136 2c31 362e 3039 3734 3233  511116,16.097423
-000027a0: 2032 322e 3938 3430 3831 2c31 362e 3039   22.984081,16.09
-000027b0: 3734 3233 2043 2032 322e 3932 3035 3433  7423 C 22.920543
-000027c0: 2c31 352e 3839 3438 3739 2032 332e 3132  ,15.894879 23.12
-000027d0: 3234 332c 3135 2e34 3835 3039 3620 3232  243,15.485096 22
-000027e0: 2e38 3632 3633 312c 3135 2e34 3335 3738  .862631,15.43578
-000027f0: 3720 4320 3232 2e30 3631 3432 312c 3135  7 C 22.061421,15
-00002800: 2e32 3335 3438 3520 3231 2e32 3630 3231  .235485 21.26021
-00002810: 312c 3135 2e30 3335 3138 3220 3230 2e34  1,15.035182 20.4
-00002820: 3538 3939 352c 3134 2e38 3334 3838 2043  58995,14.83488 C
-00002830: 2032 302e 3435 3839 3935 2c31 302e 3632   20.458995,10.62
-00002840: 3634 3031 2032 302e 3435 3839 3935 2c36  6401 20.458995,6
-00002850: 2e34 3137 3932 3920 3230 2e34 3538 3939  .417929 20.45899
-00002860: 352c 322e 3230 3934 3530 3220 4320 3231  5,2.2094502 C 21
-00002870: 2e33 3030 3639 342c 312e 3939 3930 3238  .300694,1.999028
-00002880: 3520 3232 2e31 3432 3338 382c 312e 3738  5 22.142388,1.78
-00002890: 3836 3030 3420 3232 2e39 3834 3038 312c  86004 22.984081,
-000028a0: 312e 3537 3831 3738 3720 4320 3232 2e39  1.5781787 C 22.9
-000028b0: 3138 3538 372c 312e 3339 3135 3234 3320  18587,1.3915243 
-000028c0: 3233 2e31 3236 3639 312c 302e 3933 3132  23.126691,0.9312
-000028d0: 3634 3332 2032 322e 3835 3838 3933 2c30  6432 22.858893,0
-000028e0: 2e39 3436 3930 3732 3220 4320 3231 2e34  .94690722 C 21.4
-000028f0: 3237 3635 362c 302e 3934 3639 3037 3232  27656,0.94690722
-00002900: 2031 392e 3939 3634 3138 2c30 2e39 3436   19.996418,0.946
-00002910: 3930 3732 3220 3138 2e35 3635 3138 2c30  90722 18.56518,0
-00002920: 2e39 3436 3930 3732 3220 4320 3138 2e35  .94690722 C 18.5
-00002930: 3635 3138 2c35 2e39 3937 3037 3932 2031  6518,5.9970792 1
-00002940: 382e 3536 3531 382c 3131 2e30 3437 3235  8.56518,11.04725
-00002950: 3120 3138 2e35 3635 3138 2c31 362e 3039  1 18.56518,16.09
-00002960: 3734 3233 207a 2022 0a20 2020 2020 2020  7423 z ".       
-00002970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002980: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-00002990: 7374 726f 6b65 3a20 2470 6c61 6e65 7473  stroke: $planets
-000029a0: 5f63 6f6c 6f72 5f37 3b20 7374 726f 6b65  _color_7; stroke
-000029b0: 2d77 6964 7468 3a20 3170 783b 2066 696c  -width: 1px; fil
-000029c0: 6c3a 2024 706c 616e 6574 735f 636f 6c6f  l: $planets_colo
-000029d0: 725f 3522 0a20 2020 2020 2020 2020 2020  r_5".           
-000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029f0: 202f 3e0a 2020 2020 2020 2020 2020 2020   />.            
-00002a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a10: 3c70 6174 680a 2020 2020 2020 2020 2020  <path.          
-00002a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a30: 2020 2020 2020 643d 224d 2034 2e30 3435        d="M 4.045
-00002a40: 3933 3536 2c38 2e35 3232 3136 3532 2043  9356,8.5221652 C
-00002a50: 2039 2e30 3936 3130 3736 2c38 2e35 3232   9.0961076,8.522
-00002a60: 3136 3532 2031 342e 3134 3632 382c 382e  1652 14.14628,8.
-00002a70: 3532 3231 3635 3220 3139 2e31 3936 3435  5221652 19.19645
-00002a80: 322c 382e 3532 3231 3635 3220 4d20 3131  2,8.5221652 M 11
-00002a90: 2e36 3231 3139 342c 302e 3934 3639 3037  .621194,0.946907
-00002aa0: 3232 2043 2031 312e 3632 3131 3934 2c36  22 C 11.621194,6
-00002ab0: 2e34 3137 3932 3920 3131 2e36 3231 3139  .417929 11.62119
-00002ac0: 342c 3131 2e38 3838 3934 3420 3131 2e36  4,11.888944 11.6
-00002ad0: 3231 3139 342c 3137 2e33 3539 3936 3620  21194,17.359966 
-00002ae0: 4d20 3134 2e31 3436 3234 322c 3230 2e35  M 14.146242,20.5
-00002af0: 3136 3334 3220 4320 3134 2e32 3237 3935  16342 C 14.22795
-00002b00: 342c 3232 2e32 3031 3130 3520 3132 2e32  4,22.201105 12.2
-00002b10: 3735 3636 352c 3233 2e35 3530 3330 3220  75665,23.550302 
-00002b20: 3130 2e37 3235 3637 382c 3232 2e38 3833  10.725678,22.883
-00002b30: 3032 3320 4320 392e 3133 3935 3736 362c  023 C 9.1395766,
-00002b40: 3232 2e33 3438 3639 3620 382e 3535 3230  22.348696 8.5520
-00002b50: 3436 362c 3230 2e30 3839 3638 3520 392e  466,20.089685 9.
-00002b60: 3730 3334 3937 362c 3138 2e38 3630 3837  7034976,18.86087
-00002b70: 3120 4320 3130 2e37 3234 3037 352c 3137  1 C 10.724075,17
-00002b80: 2e36 3038 3138 3220 3132 2e39 3539 3436  .608182 12.95946
-00002b90: 342c 3137 2e37 3436 3438 3120 3133 2e37  4,17.746481 13.7
-00002ba0: 3630 3733 312c 3139 2e31 3734 3830 3820  60731,19.174808 
-00002bb0: 4320 3134 2e30 3131 3333 392c 3139 2e35  C 14.011339,19.5
-00002bc0: 3734 3120 3134 2e31 3438 3138 2c32 302e  741 14.14818,20.
-00002bd0: 3034 3436 3434 2031 342e 3134 3632 3432  044644 14.146242
-00002be0: 2c32 302e 3531 3633 3432 207a 2022 0a20  ,20.516342 z ". 
-00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00002c10: 7479 6c65 3d22 7374 726f 6b65 3a20 2470  tyle="stroke: $p
-00002c20: 6c61 6e65 7473 5f63 6f6c 6f72 5f37 3b20  lanets_color_7; 
-00002c30: 7374 726f 6b65 2d77 6964 7468 3a20 3270  stroke-width: 2p
-00002c40: 783b 2066 696c 6c3a 206e 6f6e 6522 0a20  x; fill: none". 
+00002320: 2020 2020 2f3e 0a20 2020 2020 2020 2020      />.         
+00002330: 2020 2020 2020 2020 2020 203c 2f67 3e0a             </g>.
+00002340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002350: 3c2f 7379 6d62 6f6c 3e0a 2020 2020 2020  </symbol>.      
+00002360: 2020 2020 2020 2020 2020 3c73 796d 626f            <symbo
+00002370: 6c20 6964 3d22 5572 616e 7573 223e 0a20  l id="Uranus">. 
+00002380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002390: 2020 203c 6720 7472 616e 7366 6f72 6d3d     <g transform=
+000023a0: 2274 7261 6e73 6c61 7465 2832 2c34 2922  "translate(2,4)"
+000023b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000023c0: 2020 2020 2020 2020 2020 3c67 2074 7261            <g tra
+000023d0: 6e73 666f 726d 3d22 7363 616c 6528 2e38  nsform="scale(.8
+000023e0: 2922 3e0a 2020 2020 2020 2020 2020 2020  )">.            
+000023f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002400: 3c70 6174 680a 2020 2020 2020 2020 2020  <path.          
+00002410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002420: 2020 2020 2020 643d 224d 2034 2e36 3737        d="M 4.677
+00002430: 3230 3636 2c31 362e 3039 3734 3233 2043  2066,16.097423 C
+00002440: 2033 2e32 3034 3234 3236 2c31 362e 3039   3.2042426,16.09
+00002450: 3734 3233 2031 2e37 3331 3237 3736 2c31  7423 1.7312776,1
+00002460: 362e 3039 3734 3233 2030 2e32 3538 3330  6.097423 0.25830
+00002470: 3636 312c 3136 2e30 3937 3432 3320 4320  661,16.097423 C 
+00002480: 302e 3332 3138 3530 3631 2c31 352e 3839  0.32185061,15.89
+00002490: 3438 3739 2030 2e31 3139 3935 3636 312c  4879 0.11995661,
+000024a0: 3135 2e34 3835 3039 3620 302e 3337 3937  15.485096 0.3797
+000024b0: 3633 3631 2c31 352e 3433 3537 3837 2043  6361,15.435787 C
+000024c0: 2031 2e31 3830 3937 3236 2c31 352e 3233   1.1809726,15.23
+000024d0: 3534 3835 2031 2e39 3832 3138 3236 2c31  5485 1.9821826,1
+000024e0: 352e 3033 3531 3832 2032 2e37 3833 3339  5.035182 2.78339
+000024f0: 3236 2c31 342e 3833 3438 3820 4320 322e  26,14.83488 C 2.
+00002500: 3738 3333 3932 362c 3130 2e36 3236 3430  7833926,10.62640
+00002510: 3120 322e 3738 3333 3932 362c 362e 3431  1 2.7833926,6.41
+00002520: 3739 3239 2032 2e37 3833 3339 3236 2c32  7929 2.7833926,2
+00002530: 2e32 3039 3435 3032 2043 2031 2e39 3431  .2094502 C 1.941
+00002540: 3639 3936 2c31 2e39 3939 3032 3835 2031  6996,1.9990285 1
+00002550: 2e31 3030 3030 3536 2c31 2e37 3838 3630  .1000056,1.78860
+00002560: 3034 2030 2e32 3538 3330 3636 312c 312e  04 0.25830661,1.
+00002570: 3537 3831 3738 3720 4320 302e 3332 3338  5781787 C 0.3238
+00002580: 3037 3631 2c31 2e33 3931 3532 3433 2030  0761,1.3915243 0
+00002590: 2e31 3135 3730 3236 312c 302e 3933 3132  .11570261,0.9312
+000025a0: 3634 3332 2030 2e33 3833 3530 3036 312c  6432 0.38350061,
+000025b0: 302e 3934 3639 3037 3232 2043 2031 2e38  0.94690722 C 1.8
+000025c0: 3134 3733 3736 2c30 2e39 3436 3930 3732  147376,0.9469072
+000025d0: 3220 332e 3234 3539 3639 362c 302e 3934  2 3.2459696,0.94
+000025e0: 3639 3037 3232 2034 2e36 3737 3230 3636  690722 4.6772066
+000025f0: 2c30 2e39 3436 3930 3732 3220 4320 342e  ,0.94690722 C 4.
+00002600: 3637 3732 3036 362c 352e 3939 3730 3739  6772066,5.997079
+00002610: 3220 342e 3637 3732 3036 362c 3131 2e30  2 4.6772066,11.0
+00002620: 3437 3235 3120 342e 3637 3732 3036 362c  47251 4.6772066,
+00002630: 3136 2e30 3937 3432 3320 7a20 220a 2020  16.097423 z ".  
+00002640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002650: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00002660: 796c 653d 2273 7472 6f6b 653a 2024 706c  yle="stroke: $pl
+00002670: 616e 6574 735f 636f 6c6f 725f 373b 2073  anets_color_7; s
+00002680: 7472 6f6b 652d 7769 6474 683a 2031 7078  troke-width: 1px
+00002690: 3b20 6669 6c6c 3a20 2470 6c61 6e65 7473  ; fill: $planets
+000026a0: 5f63 6f6c 6f72 5f35 220a 2020 2020 2020  _color_5".      
+000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026c0: 2020 2020 2020 2f3e 0a20 2020 2020 2020        />.       
+000026d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026e0: 2020 2020 203c 7061 7468 0a20 2020 2020       <path.     
+000026f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002700: 2020 2020 2020 2020 2020 2064 3d22 4d20             d="M 
+00002710: 3138 2e35 3635 3138 2c31 362e 3039 3734  18.56518,16.0974
+00002720: 3233 2043 2032 302e 3033 3831 3531 2c31  23 C 20.038151,1
+00002730: 362e 3039 3734 3233 2032 312e 3531 3131  6.097423 21.5111
+00002740: 3136 2c31 362e 3039 3734 3233 2032 322e  16,16.097423 22.
+00002750: 3938 3430 3831 2c31 362e 3039 3734 3233  984081,16.097423
+00002760: 2043 2032 322e 3932 3035 3433 2c31 352e   C 22.920543,15.
+00002770: 3839 3438 3739 2032 332e 3132 3234 332c  894879 23.12243,
+00002780: 3135 2e34 3835 3039 3620 3232 2e38 3632  15.485096 22.862
+00002790: 3633 312c 3135 2e34 3335 3738 3720 4320  631,15.435787 C 
+000027a0: 3232 2e30 3631 3432 312c 3135 2e32 3335  22.061421,15.235
+000027b0: 3438 3520 3231 2e32 3630 3231 312c 3135  485 21.260211,15
+000027c0: 2e30 3335 3138 3220 3230 2e34 3538 3939  .035182 20.45899
+000027d0: 352c 3134 2e38 3334 3838 2043 2032 302e  5,14.83488 C 20.
+000027e0: 3435 3839 3935 2c31 302e 3632 3634 3031  458995,10.626401
+000027f0: 2032 302e 3435 3839 3935 2c36 2e34 3137   20.458995,6.417
+00002800: 3932 3920 3230 2e34 3538 3939 352c 322e  929 20.458995,2.
+00002810: 3230 3934 3530 3220 4320 3231 2e33 3030  2094502 C 21.300
+00002820: 3639 342c 312e 3939 3930 3238 3520 3232  694,1.9990285 22
+00002830: 2e31 3432 3338 382c 312e 3738 3836 3030  .142388,1.788600
+00002840: 3420 3232 2e39 3834 3038 312c 312e 3537  4 22.984081,1.57
+00002850: 3831 3738 3720 4320 3232 2e39 3138 3538  81787 C 22.91858
+00002860: 372c 312e 3339 3135 3234 3320 3233 2e31  7,1.3915243 23.1
+00002870: 3236 3639 312c 302e 3933 3132 3634 3332  26691,0.93126432
+00002880: 2032 322e 3835 3838 3933 2c30 2e39 3436   22.858893,0.946
+00002890: 3930 3732 3220 4320 3231 2e34 3237 3635  90722 C 21.42765
+000028a0: 362c 302e 3934 3639 3037 3232 2031 392e  6,0.94690722 19.
+000028b0: 3939 3634 3138 2c30 2e39 3436 3930 3732  996418,0.9469072
+000028c0: 3220 3138 2e35 3635 3138 2c30 2e39 3436  2 18.56518,0.946
+000028d0: 3930 3732 3220 4320 3138 2e35 3635 3138  90722 C 18.56518
+000028e0: 2c35 2e39 3937 3037 3932 2031 382e 3536  ,5.9970792 18.56
+000028f0: 3531 382c 3131 2e30 3437 3235 3120 3138  518,11.047251 18
+00002900: 2e35 3635 3138 2c31 362e 3039 3734 3233  .56518,16.097423
+00002910: 207a 2022 0a20 2020 2020 2020 2020 2020   z ".           
+00002920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002930: 2020 2020 2073 7479 6c65 3d22 7374 726f       style="stro
+00002940: 6b65 3a20 2470 6c61 6e65 7473 5f63 6f6c  ke: $planets_col
+00002950: 6f72 5f37 3b20 7374 726f 6b65 2d77 6964  or_7; stroke-wid
+00002960: 7468 3a20 3170 783b 2066 696c 6c3a 2024  th: 1px; fill: $
+00002970: 706c 616e 6574 735f 636f 6c6f 725f 3522  planets_color_5"
+00002980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002990: 2020 2020 2020 2020 2020 2020 202f 3e0a               />.
+000029a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029b0: 2020 2020 2020 2020 2020 2020 3c70 6174              <pat
+000029c0: 680a 2020 2020 2020 2020 2020 2020 2020  h.              
+000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029e0: 2020 643d 224d 2034 2e30 3435 3933 3536    d="M 4.0459356
+000029f0: 2c38 2e35 3232 3136 3532 2043 2039 2e30  ,8.5221652 C 9.0
+00002a00: 3936 3130 3736 2c38 2e35 3232 3136 3532  961076,8.5221652
+00002a10: 2031 342e 3134 3632 382c 382e 3532 3231   14.14628,8.5221
+00002a20: 3635 3220 3139 2e31 3936 3435 322c 382e  652 19.196452,8.
+00002a30: 3532 3231 3635 3220 4d20 3131 2e36 3231  5221652 M 11.621
+00002a40: 3139 342c 302e 3934 3639 3037 3232 2043  194,0.94690722 C
+00002a50: 2031 312e 3632 3131 3934 2c36 2e34 3137   11.621194,6.417
+00002a60: 3932 3920 3131 2e36 3231 3139 342c 3131  929 11.621194,11
+00002a70: 2e38 3838 3934 3420 3131 2e36 3231 3139  .888944 11.62119
+00002a80: 342c 3137 2e33 3539 3936 3620 4d20 3134  4,17.359966 M 14
+00002a90: 2e31 3436 3234 322c 3230 2e35 3136 3334  .146242,20.51634
+00002aa0: 3220 4320 3134 2e32 3237 3935 342c 3232  2 C 14.227954,22
+00002ab0: 2e32 3031 3130 3520 3132 2e32 3735 3636  .201105 12.27566
+00002ac0: 352c 3233 2e35 3530 3330 3220 3130 2e37  5,23.550302 10.7
+00002ad0: 3235 3637 382c 3232 2e38 3833 3032 3320  25678,22.883023 
+00002ae0: 4320 392e 3133 3935 3736 362c 3232 2e33  C 9.1395766,22.3
+00002af0: 3438 3639 3620 382e 3535 3230 3436 362c  48696 8.5520466,
+00002b00: 3230 2e30 3839 3638 3520 392e 3730 3334  20.089685 9.7034
+00002b10: 3937 362c 3138 2e38 3630 3837 3120 4320  976,18.860871 C 
+00002b20: 3130 2e37 3234 3037 352c 3137 2e36 3038  10.724075,17.608
+00002b30: 3138 3220 3132 2e39 3539 3436 342c 3137  182 12.959464,17
+00002b40: 2e37 3436 3438 3120 3133 2e37 3630 3733  .746481 13.76073
+00002b50: 312c 3139 2e31 3734 3830 3820 4320 3134  1,19.174808 C 14
+00002b60: 2e30 3131 3333 392c 3139 2e35 3734 3120  .011339,19.5741 
+00002b70: 3134 2e31 3438 3138 2c32 302e 3034 3436  14.14818,20.0446
+00002b80: 3434 2031 342e 3134 3632 3432 2c32 302e  44 14.146242,20.
+00002b90: 3531 3633 3432 207a 2022 0a20 2020 2020  516342 z ".     
+00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bb0: 2020 2020 2020 2020 2020 2073 7479 6c65             style
+00002bc0: 3d22 7374 726f 6b65 3a20 2470 6c61 6e65  ="stroke: $plane
+00002bd0: 7473 5f63 6f6c 6f72 5f37 3b20 7374 726f  ts_color_7; stro
+00002be0: 6b65 2d77 6964 7468 3a20 3270 783b 2066  ke-width: 2px; f
+00002bf0: 696c 6c3a 206e 6f6e 6522 0a20 2020 2020  ill: none".     
+00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c10: 2020 2020 2020 202f 3e0a 2020 2020 2020         />.      
+00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c30: 2020 3c2f 673e 0a20 2020 2020 2020 2020    </g>.         
+00002c40: 2020 2020 2020 2020 2020 203c 2f67 3e0a             </g>.
 00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c60: 2020 2020 2020 2020 2020 202f 3e0a 2020             />.  
-00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c80: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
-00002c90: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002ca0: 2f67 3e0a 2020 2020 2020 2020 2020 2020  /g>.            
-00002cb0: 2020 2020 3c2f 7379 6d62 6f6c 3e0a 2020      </symbol>.  
-00002cc0: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-00002cd0: 796d 626f 6c20 6964 3d22 4e65 7074 756e  ymbol id="Neptun
-00002ce0: 6522 3e0a 2020 2020 2020 2020 2020 2020  e">.            
-00002cf0: 2020 2020 2020 2020 3c67 2074 7261 6e73          <g trans
-00002d00: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
-00002d10: 322c 3429 223e 0a20 2020 2020 2020 2020  2,4)">.         
-00002d20: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002d30: 6720 7472 616e 7366 6f72 6d3d 2273 6361  g transform="sca
-00002d40: 6c65 282e 3929 223e 0a20 2020 2020 2020  le(.9)">.       
-00002d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d60: 2020 2020 203c 7061 7468 0a20 2020 2020       <path.     
-00002d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d80: 2020 2020 2020 2020 2020 2064 3d22 4d20             d="M 
-00002d90: 332e 3838 3633 3037 2c32 2e32 3039 3831  3.886307,2.20981
-00002da0: 3334 2043 2032 2e32 3732 3832 3439 2c31  34 C 2.2728249,1
-00002db0: 332e 3137 3233 3336 2034 2e39 3631 3937  3.172336 4.96197
-00002dc0: 3138 2c31 342e 3831 3637 3138 2031 302e  18,14.816718 10.
-00002dd0: 3334 3032 3635 2c31 342e 3831 3637 3138  340265,14.816718
-00002de0: 2043 2031 352e 3731 3835 3637 2c31 342e   C 15.718567,14.
-00002df0: 3831 3637 3138 2031 382e 3430 3737 3231  816718 18.407721
-00002e00: 2c31 332e 3137 3233 3336 2031 362e 3739  ,13.172336 16.79
-00002e10: 3432 3331 2c32 2e32 3039 3831 3334 204d  4231,2.2098134 M
-00002e20: 2031 302e 3334 3032 3635 2c33 2e33 3036   10.340265,3.306
-00002e30: 3036 3538 204c 2031 302e 3334 3032 3635  0658 L 10.340265
-00002e40: 2c32 332e 3538 3637 3336 204d 2036 2e30  ,23.586736 M 6.0
-00002e50: 3337 3632 392c 3139 2e32 3031 3732 3720  37629,19.201727 
-00002e60: 4c20 3134 2e36 3432 3930 392c 3139 2e32  L 14.642909,19.2
-00002e70: 3031 3732 3720 4d20 302e 3931 3138 3030  01727 M 0.911800
-00002e80: 3237 2c33 2e37 3233 3038 3038 204c 2033  27,3.7230808 L 3
-00002e90: 2e39 3633 3537 3935 2c31 2e34 3130 3333  .9635795,1.41033
-00002ea0: 3631 204c 2036 2e32 3332 3836 3839 2c34  61 L 6.2328689,4
-00002eb0: 2e35 3230 3534 3738 204d 2037 2e35 3939  .5205478 M 7.599
-00002ec0: 3834 3836 2c36 2e33 3432 3132 3438 204c  8486,6.3421248 L
-00002ed0: 2031 302e 3235 3930 3535 2c33 2e35 3731   10.259055,3.571
-00002ee0: 3331 3038 204c 2031 322e 3937 3738 3132  3108 L 12.977812
-00002ef0: 2c36 2e32 3831 3434 3238 204d 2031 342e  ,6.2814428 M 14.
-00002f00: 3430 3738 3839 2c34 2e37 3132 3035 3238  407889,4.7120528
-00002f10: 204c 2031 362e 3731 3539 3436 2c31 2e36   L 16.715946,1.6
-00002f20: 3331 3630 3835 204c 2031 392e 3733 3835  316085 L 19.7385
-00002f30: 3036 2c33 2e39 3833 3836 3238 220a 2020  06,3.9838628".  
-00002f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f50: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00002f60: 796c 653d 2273 7472 6f6b 653a 2024 706c  yle="stroke: $pl
-00002f70: 616e 6574 735f 636f 6c6f 725f 383b 2073  anets_color_8; s
-00002f80: 7472 6f6b 652d 7769 6474 683a 2032 7078  troke-width: 2px
-00002f90: 3b20 6669 6c6c 3a20 6e6f 6e65 220a 2020  ; fill: none".  
-00002fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fb0: 2020 2020 2020 2020 2020 2f3e 0a20 2020            />.   
-00002fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fd0: 2020 2020 203c 2f67 3e0a 2020 2020 2020       </g>.      
-00002fe0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00002ff0: 673e 0a20 2020 2020 2020 2020 2020 2020  g>.             
-00003000: 2020 203c 2f73 796d 626f 6c3e 0a20 2020     </symbol>.   
-00003010: 2020 2020 2020 2020 2020 2020 203c 7379               <sy
-00003020: 6d62 6f6c 2069 643d 2250 6c75 746f 223e  mbol id="Pluto">
-00003030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003040: 2020 2020 203c 6720 7472 616e 7366 6f72       <g transfor
-00003050: 6d3d 2274 7261 6e73 6c61 7465 2830 2c33  m="translate(0,3
-00003060: 2922 3e0a 2020 2020 2020 2020 2020 2020  )">.            
-00003070: 2020 2020 2020 2020 2020 2020 3c67 2074              <g t
-00003080: 7261 6e73 666f 726d 3d22 7363 616c 6528  ransform="scale(
-00003090: 2e39 2922 3e0a 2020 2020 2020 2020 2020  .9)">.          
-000030a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030b0: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
-000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030d0: 2020 2020 2020 2020 643d 224d 2037 2e32          d="M 7.2
-000030e0: 3938 3833 3839 2c31 382e 3136 3936 3731  988389,18.169671
-000030f0: 204c 2031 372e 3137 3032 3939 2c31 382e   L 17.170299,18.
-00003100: 3136 3936 3731 204d 2031 322e 3233 3435  169671 M 12.2345
-00003110: 3639 2c32 332e 3130 3534 3031 204c 2031  69,23.105401 L 1
-00003120: 322e 3233 3435 3639 2c31 322e 3631 3639  2.234569,12.6169
-00003130: 3831 204d 2031 362e 3535 3333 3039 2c35  81 M 16.553309,5
-00003140: 2e32 3133 3336 3039 2043 2031 362e 3535  .2133609 C 16.55
-00003150: 3333 3039 2c37 2e35 3937 3332 3039 2031  3309,7.5973209 1
-00003160: 342e 3631 3834 3939 2c39 2e35 3332 3133  4.618499,9.53213
-00003170: 3039 2031 322e 3233 3435 3339 2c39 2e35  09 12.234539,9.5
-00003180: 3332 3133 3039 2043 2039 2e38 3530 3538  321309 C 9.85058
-00003190: 3839 2c39 2e35 3332 3133 3039 2037 2e39  89,9.5321309 7.9
-000031a0: 3135 3737 3839 2c37 2e35 3937 3332 3039  157789,7.5973209
-000031b0: 2037 2e39 3135 3737 3839 2c35 2e32 3133   7.9157789,5.213
-000031c0: 3336 3039 2043 2037 2e39 3135 3737 3839  3609 C 7.9157789
-000031d0: 2c32 2e38 3239 3431 3039 2039 2e38 3530  ,2.8294109 9.850
-000031e0: 3538 3839 2c30 2e38 3934 3630 3038 3720  5889,0.89460087 
-000031f0: 3132 2e32 3334 3533 392c 302e 3839 3436  12.234539,0.8946
-00003200: 3030 3837 2043 2031 342e 3631 3834 3939  0087 C 14.618499
-00003210: 2c30 2e38 3934 3630 3038 3720 3136 2e35  ,0.89460087 16.5
-00003220: 3533 3330 392c 322e 3832 3934 3130 3920  53309,2.8294109 
-00003230: 3136 2e35 3533 3330 392c 352e 3231 3333  16.553309,5.2133
-00003240: 3630 3920 7a20 4d20 3139 2e36 3338 3133  609 z M 19.63813
-00003250: 392c 352e 3231 3333 3630 3920 4320 3139  9,5.2133609 C 19
-00003260: 2e36 3338 3133 392c 392e 3330 3031 3530  .638139,9.300150
-00003270: 3920 3136 2e33 3231 3332 392c 3132 2e36  9 16.321329,12.6
-00003280: 3136 3936 3120 3132 2e32 3334 3533 392c  16961 12.234539,
-00003290: 3132 2e36 3136 3936 3120 4320 382e 3134  12.616961 C 8.14
-000032a0: 3737 3538 392c 3132 2e36 3136 3936 3120  77589,12.616961 
-000032b0: 342e 3833 3039 3438 392c 392e 3330 3031  4.8309489,9.3001
-000032c0: 3530 3920 342e 3833 3039 3438 392c 352e  509 4.8309489,5.
-000032d0: 3231 3333 3630 3920 4320 342e 3833 3039  2133609 C 4.8309
-000032e0: 3438 392c 352e 3231 3333 3630 3920 342e  489,5.2133609 4.
-000032f0: 3833 3039 3438 392c 352e 3231 3333 3630  8309489,5.213360
-00003300: 3920 342e 3833 3039 3438 392c 352e 3231  9 4.8309489,5.21
-00003310: 3333 3630 3922 0a20 2020 2020 2020 2020  33609".         
-00003320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003330: 2020 2020 2020 2073 7479 6c65 3d22 7374         style="st
-00003340: 726f 6b65 3a20 2470 6c61 6e65 7473 5f63  roke: $planets_c
-00003350: 6f6c 6f72 5f39 3b20 7374 726f 6b65 2d77  olor_9; stroke-w
-00003360: 6964 7468 3a20 3270 783b 2066 696c 6c3a  idth: 2px; fill:
-00003370: 206e 6f6e 6522 0a20 2020 2020 2020 2020   none".         
-00003380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003390: 2020 202f 3e0a 2020 2020 2020 2020 2020     />.          
-000033a0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-000033b0: 673e 0a20 2020 2020 2020 2020 2020 2020  g>.             
-000033c0: 2020 2020 2020 203c 2f67 3e0a 2020 2020         </g>.    
-000033d0: 2020 2020 2020 2020 2020 2020 3c2f 7379              </sy
-000033e0: 6d62 6f6c 3e0a 2020 2020 2020 2020 2020  mbol>.          
-000033f0: 2020 2020 2020 3c73 796d 626f 6c20 6964        <symbol id
-00003400: 3d22 4d65 616e 5f4e 6f64 6522 3e0a 2020  ="Mean_Node">.  
+00002c60: 3c2f 7379 6d62 6f6c 3e0a 2020 2020 2020  </symbol>.      
+00002c70: 2020 2020 2020 2020 2020 3c73 796d 626f            <symbo
+00002c80: 6c20 6964 3d22 4e65 7074 756e 6522 3e0a  l id="Neptune">.
+00002c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ca0: 2020 2020 3c67 2074 7261 6e73 666f 726d      <g transform
+00002cb0: 3d22 7472 616e 736c 6174 6528 322c 3429  ="translate(2,4)
+00002cc0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00002cd0: 2020 2020 2020 2020 2020 203c 6720 7472             <g tr
+00002ce0: 616e 7366 6f72 6d3d 2273 6361 6c65 282e  ansform="scale(.
+00002cf0: 3929 223e 0a20 2020 2020 2020 2020 2020  9)">.           
+00002d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d10: 203c 7061 7468 0a20 2020 2020 2020 2020   <path.         
+00002d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d30: 2020 2020 2020 2064 3d22 4d20 332e 3838         d="M 3.88
+00002d40: 3633 3037 2c32 2e32 3039 3831 3334 2043  6307,2.2098134 C
+00002d50: 2032 2e32 3732 3832 3439 2c31 332e 3137   2.2728249,13.17
+00002d60: 3233 3336 2034 2e39 3631 3937 3138 2c31  2336 4.9619718,1
+00002d70: 342e 3831 3637 3138 2031 302e 3334 3032  4.816718 10.3402
+00002d80: 3635 2c31 342e 3831 3637 3138 2043 2031  65,14.816718 C 1
+00002d90: 352e 3731 3835 3637 2c31 342e 3831 3637  5.718567,14.8167
+00002da0: 3138 2031 382e 3430 3737 3231 2c31 332e  18 18.407721,13.
+00002db0: 3137 3233 3336 2031 362e 3739 3432 3331  172336 16.794231
+00002dc0: 2c32 2e32 3039 3831 3334 204d 2031 302e  ,2.2098134 M 10.
+00002dd0: 3334 3032 3635 2c33 2e33 3036 3036 3538  340265,3.3060658
+00002de0: 204c 2031 302e 3334 3032 3635 2c32 332e   L 10.340265,23.
+00002df0: 3538 3637 3336 204d 2036 2e30 3337 3632  586736 M 6.03762
+00002e00: 392c 3139 2e32 3031 3732 3720 4c20 3134  9,19.201727 L 14
+00002e10: 2e36 3432 3930 392c 3139 2e32 3031 3732  .642909,19.20172
+00002e20: 3720 4d20 302e 3931 3138 3030 3237 2c33  7 M 0.91180027,3
+00002e30: 2e37 3233 3038 3038 204c 2033 2e39 3633  .7230808 L 3.963
+00002e40: 3537 3935 2c31 2e34 3130 3333 3631 204c  5795,1.4103361 L
+00002e50: 2036 2e32 3332 3836 3839 2c34 2e35 3230   6.2328689,4.520
+00002e60: 3534 3738 204d 2037 2e35 3939 3834 3836  5478 M 7.5998486
+00002e70: 2c36 2e33 3432 3132 3438 204c 2031 302e  ,6.3421248 L 10.
+00002e80: 3235 3930 3535 2c33 2e35 3731 3331 3038  259055,3.5713108
+00002e90: 204c 2031 322e 3937 3738 3132 2c36 2e32   L 12.977812,6.2
+00002ea0: 3831 3434 3238 204d 2031 342e 3430 3738  814428 M 14.4078
+00002eb0: 3839 2c34 2e37 3132 3035 3238 204c 2031  89,4.7120528 L 1
+00002ec0: 362e 3731 3539 3436 2c31 2e36 3331 3630  6.715946,1.63160
+00002ed0: 3835 204c 2031 392e 3733 3835 3036 2c33  85 L 19.738506,3
+00002ee0: 2e39 3833 3836 3238 220a 2020 2020 2020  .9838628".      
+00002ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f00: 2020 2020 2020 2020 2020 7374 796c 653d            style=
+00002f10: 2273 7472 6f6b 653a 2024 706c 616e 6574  "stroke: $planet
+00002f20: 735f 636f 6c6f 725f 383b 2073 7472 6f6b  s_color_8; strok
+00002f30: 652d 7769 6474 683a 2032 7078 3b20 6669  e-width: 2px; fi
+00002f40: 6c6c 3a20 6e6f 6e65 220a 2020 2020 2020  ll: none".      
+00002f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f60: 2020 2020 2020 2f3e 0a20 2020 2020 2020        />.       
+00002f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f80: 203c 2f67 3e0a 2020 2020 2020 2020 2020   </g>.          
+00002f90: 2020 2020 2020 2020 2020 3c2f 673e 0a20            </g>. 
+00002fa0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00002fb0: 2f73 796d 626f 6c3e 0a20 2020 2020 2020  /symbol>.       
+00002fc0: 2020 2020 2020 2020 203c 7379 6d62 6f6c           <symbol
+00002fd0: 2069 643d 2250 6c75 746f 223e 0a20 2020   id="Pluto">.   
+00002fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ff0: 203c 6720 7472 616e 7366 6f72 6d3d 2274   <g transform="t
+00003000: 7261 6e73 6c61 7465 2830 2c33 2922 3e0a  ranslate(0,3)">.
+00003010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003020: 2020 2020 2020 2020 3c67 2074 7261 6e73          <g trans
+00003030: 666f 726d 3d22 7363 616c 6528 2e39 2922  form="scale(.9)"
+00003040: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00003050: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+00003060: 6174 680a 2020 2020 2020 2020 2020 2020  ath.            
+00003070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003080: 2020 2020 643d 224d 2037 2e32 3938 3833      d="M 7.29883
+00003090: 3839 2c31 382e 3136 3936 3731 204c 2031  89,18.169671 L 1
+000030a0: 372e 3137 3032 3939 2c31 382e 3136 3936  7.170299,18.1696
+000030b0: 3731 204d 2031 322e 3233 3435 3639 2c32  71 M 12.234569,2
+000030c0: 332e 3130 3534 3031 204c 2031 322e 3233  3.105401 L 12.23
+000030d0: 3435 3639 2c31 322e 3631 3639 3831 204d  4569,12.616981 M
+000030e0: 2031 362e 3535 3333 3039 2c35 2e32 3133   16.553309,5.213
+000030f0: 3336 3039 2043 2031 362e 3535 3333 3039  3609 C 16.553309
+00003100: 2c37 2e35 3937 3332 3039 2031 342e 3631  ,7.5973209 14.61
+00003110: 3834 3939 2c39 2e35 3332 3133 3039 2031  8499,9.5321309 1
+00003120: 322e 3233 3435 3339 2c39 2e35 3332 3133  2.234539,9.53213
+00003130: 3039 2043 2039 2e38 3530 3538 3839 2c39  09 C 9.8505889,9
+00003140: 2e35 3332 3133 3039 2037 2e39 3135 3737  .5321309 7.91577
+00003150: 3839 2c37 2e35 3937 3332 3039 2037 2e39  89,7.5973209 7.9
+00003160: 3135 3737 3839 2c35 2e32 3133 3336 3039  157789,5.2133609
+00003170: 2043 2037 2e39 3135 3737 3839 2c32 2e38   C 7.9157789,2.8
+00003180: 3239 3431 3039 2039 2e38 3530 3538 3839  294109 9.8505889
+00003190: 2c30 2e38 3934 3630 3038 3720 3132 2e32  ,0.89460087 12.2
+000031a0: 3334 3533 392c 302e 3839 3436 3030 3837  34539,0.89460087
+000031b0: 2043 2031 342e 3631 3834 3939 2c30 2e38   C 14.618499,0.8
+000031c0: 3934 3630 3038 3720 3136 2e35 3533 3330  9460087 16.55330
+000031d0: 392c 322e 3832 3934 3130 3920 3136 2e35  9,2.8294109 16.5
+000031e0: 3533 3330 392c 352e 3231 3333 3630 3920  53309,5.2133609 
+000031f0: 7a20 4d20 3139 2e36 3338 3133 392c 352e  z M 19.638139,5.
+00003200: 3231 3333 3630 3920 4320 3139 2e36 3338  2133609 C 19.638
+00003210: 3133 392c 392e 3330 3031 3530 3920 3136  139,9.3001509 16
+00003220: 2e33 3231 3332 392c 3132 2e36 3136 3936  .321329,12.61696
+00003230: 3120 3132 2e32 3334 3533 392c 3132 2e36  1 12.234539,12.6
+00003240: 3136 3936 3120 4320 382e 3134 3737 3538  16961 C 8.147758
+00003250: 392c 3132 2e36 3136 3936 3120 342e 3833  9,12.616961 4.83
+00003260: 3039 3438 392c 392e 3330 3031 3530 3920  09489,9.3001509 
+00003270: 342e 3833 3039 3438 392c 352e 3231 3333  4.8309489,5.2133
+00003280: 3630 3920 4320 342e 3833 3039 3438 392c  609 C 4.8309489,
+00003290: 352e 3231 3333 3630 3920 342e 3833 3039  5.2133609 4.8309
+000032a0: 3438 392c 352e 3231 3333 3630 3920 342e  489,5.2133609 4.
+000032b0: 3833 3039 3438 392c 352e 3231 3333 3630  8309489,5.213360
+000032c0: 3922 0a20 2020 2020 2020 2020 2020 2020  9".             
+000032d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032e0: 2020 2073 7479 6c65 3d22 7374 726f 6b65     style="stroke
+000032f0: 3a20 2470 6c61 6e65 7473 5f63 6f6c 6f72  : $planets_color
+00003300: 5f39 3b20 7374 726f 6b65 2d77 6964 7468  _9; stroke-width
+00003310: 3a20 3270 783b 2066 696c 6c3a 206e 6f6e  : 2px; fill: non
+00003320: 6522 0a20 2020 2020 2020 2020 2020 2020  e".             
+00003330: 2020 2020 2020 2020 2020 2020 2020 202f                 /
+00003340: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00003350: 2020 2020 2020 2020 2020 3c2f 673e 0a20            </g>. 
+00003360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003370: 2020 203c 2f67 3e0a 2020 2020 2020 2020     </g>.        
+00003380: 2020 2020 2020 2020 3c2f 7379 6d62 6f6c          </symbol
+00003390: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000033a0: 2020 3c73 796d 626f 6c20 6964 3d22 4d65    <symbol id="Me
+000033b0: 616e 5f4e 6f64 6522 3e0a 2020 2020 2020  an_Node">.      
+000033c0: 2020 2020 2020 2020 2020 2020 2020 3c67                <g
+000033d0: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
+000033e0: 736c 6174 6528 302c 3329 223e 0a20 2020  slate(0,3)">.   
+000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003400: 2020 2020 203c 7061 7468 0a20 2020 2020       <path.     
 00003410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003420: 2020 3c67 2074 7261 6e73 666f 726d 3d22    <g transform="
-00003430: 7472 616e 736c 6174 6528 302c 3329 223e  translate(0,3)">
-00003440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003450: 2020 2020 2020 2020 203c 7061 7468 0a20           <path. 
-00003460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003470: 2020 2020 2020 2020 2020 2064 3d22 4d20             d="M 
-00003480: 382e 3830 3936 3034 362c 302e 3037 3536  8.8096046,0.0756
-00003490: 3636 3839 3720 4320 362e 3431 3537 3533  66897 C 6.415753
-000034a0: 362c 302e 3636 3132 3339 3632 2034 2e33  6,0.66123962 4.3
-000034b0: 3736 3737 3639 2c32 2e35 3330 3638 3337  767769,2.5306837
-000034c0: 2033 2e36 3633 3436 3536 2c34 2e39 3030   3.6634656,4.900
-000034d0: 3735 3134 2043 2033 2e30 3533 3630 3731  7514 C 3.0536071
-000034e0: 2c36 2e36 3830 3932 3634 2033 2e36 3836  ,6.6809264 3.686
-000034f0: 3836 3832 2c38 2e36 3233 3839 3031 2034  8682,8.6238901 4
-00003500: 2e35 3837 3839 3838 2c31 302e 3138 3634  .5878988,10.1864
-00003510: 3337 2043 2035 2e31 3332 3339 3937 2c31  37 C 5.1323997,1
-00003520: 312e 3132 3436 3232 2035 2e39 3631 3537  1.124622 5.96157
-00003530: 3533 2c31 312e 3930 3839 3520 362e 3139  53,11.90895 6.19
-00003540: 3037 3330 322c 3133 2e30 3037 3930 3620  07302,13.007906 
-00003550: 4320 362e 3539 3137 3230 322c 3134 2e34  C 6.5917202,14.4
-00003560: 3834 3438 3820 362e 3438 3837 3135 362c  84488 6.4887156,
-00003570: 3136 2e33 3837 3532 3320 352e 3137 3233  16.387523 5.1723
-00003580: 3738 382c 3137 2e33 3832 3537 3620 4320  788,17.382576 C 
-00003590: 342e 3333 3239 3937 342c 3138 2e30 3533  4.3329974,18.053
-000035a0: 3431 3320 332e 3037 3735 3734 312c 3137  413 3.0775741,17
-000035b0: 2e34 3535 3033 3420 322e 3832 3030 3133  .455034 2.820013
-000035c0: 362c 3136 2e34 3831 3139 3620 4320 322e  6,16.481196 C 2.
-000035d0: 3339 3136 3535 322c 3135 2e31 3030 3739  3916552,15.10079
-000035e0: 3320 332e 3332 3331 3839 382c 3133 2e33  3 3.3231898,13.3
-000035f0: 3936 3435 3620 342e 3737 3933 3331 362c  96456 4.7793316,
-00003600: 3133 2e31 3633 3830 3620 4320 352e 3531  13.163806 C 5.51
-00003610: 3537 3836 312c 3133 2e34 3438 3438 3920  57861,13.448489 
-00003620: 352e 3733 3632 3335 332c 3133 2e30 3038  5.7362353,13.008
-00003630: 3333 3120 342e 3938 3830 3531 2c31 322e  331 4.988051,12.
-00003640: 3733 3931 3031 2043 2033 2e34 3736 3736  739101 C 3.47676
-00003650: 3936 2c31 312e 3938 3037 3631 2031 2e32  96,11.980761 1.2
-00003660: 3433 3138 3936 2c31 322e 3833 3936 3920  431896,12.83969 
-00003670: 312e 3033 3531 3437 362c 3134 2e36 3335  1.0351476,14.635
-00003680: 3339 3420 4320 302e 3737 3434 3537 3135  394 C 0.77445715
-00003690: 2c31 362e 3239 3835 3832 2031 2e39 3532  ,16.298582 1.952
-000036a0: 3838 3437 2c31 372e 3939 3138 3335 2033  8847,17.991835 3
-000036b0: 2e35 3839 3539 3633 2c31 382e 3335 3734  .5895963,18.3574
-000036c0: 3539 2043 2035 2e34 3237 3636 3632 2c31  59 C 5.4276662,1
-000036d0: 382e 3939 3431 3635 2037 2e36 3636 3138  8.994165 7.66618
-000036e0: 3339 2c31 372e 3936 3835 3334 2038 2e32  39,17.968534 8.2
-000036f0: 3937 3930 3339 2c31 362e 3131 3031 3632  979039,16.110162
-00003700: 2043 2038 2e38 3537 3130 3235 2c31 342e   C 8.8571025,14.
-00003710: 3731 3635 3237 2038 2e35 3436 3534 3831  716527 8.5465481
-00003720: 2c31 332e 3138 3631 3339 2038 2e30 3238  ,13.186139 8.028
-00003730: 3938 3638 2c31 312e 3833 3236 3533 2043  9868,11.832653 C
-00003740: 2037 2e34 3730 3238 3835 2c31 302e 3230   7.4702885,10.20
-00003750: 3638 3834 2036 2e32 3535 3336 3633 2c38  6884 6.2553663,8
-00003760: 2e38 3730 3936 3734 2035 2e39 3239 3930  .8709674 5.92990
-00003770: 3536 2c37 2e31 3532 3538 3338 2043 2035  56,7.1525838 C 5
-00003780: 2e34 3931 3436 2c35 2e34 3932 3939 3635  .49146,5.4929965
-00003790: 2035 2e38 3837 3534 3938 2c33 2e35 3733   5.8875498,3.573
-000037a0: 3536 3239 2037 2e32 3332 3936 3037 2c32  5629 7.2329607,2
-000037b0: 2e34 3332 3732 3133 2043 2038 2e37 3338  .4327213 C 8.738
-000037c0: 3835 3931 2c31 2e30 3133 3434 3531 2031  8591,1.0134451 1
-000037d0: 312e 3331 3839 3331 2c30 2e37 3535 3730  1.318931,0.75570
-000037e0: 3832 2031 322e 3931 3938 3138 2c32 2e31  82 12.919818,2.1
-000037f0: 3632 3737 3233 2043 2031 342e 3839 3131  627723 C 14.8911
-00003800: 3734 2c33 2e36 3736 3933 3435 2031 352e  74,3.6769345 15.
-00003810: 3239 3530 3635 2c36 2e35 3639 3230 3238  295065,6.5692028
-00003820: 2031 342e 3333 3032 3337 2c38 2e37 3637   14.330237,8.767
-00003830: 3139 3333 2043 2031 332e 3931 3034 3834  1933 C 13.910484
-00003840: 2c39 2e39 3139 3336 3538 2031 332e 3135  ,9.9193658 13.15
-00003850: 3433 3533 2c31 302e 3930 3236 3739 2031  4353,10.902679 1
-00003860: 322e 3631 3538 3737 2c31 312e 3939 3132  2.615877,11.9912
-00003870: 3939 2043 2031 322e 3033 3830 3435 2c31  99 C 12.038045,1
-00003880: 332e 3534 3832 3620 3132 2e30 3830 3539  3.54826 12.08059
-00003890: 392c 3135 2e33 3634 3831 3320 3132 2e37  9,15.364813 12.7
-000038a0: 3737 3435 352c 3136 2e38 3735 3136 3320  77455,16.875163 
-000038b0: 4320 3134 2e30 3736 3934 362c 3139 2e31  C 14.076946,19.1
-000038c0: 3130 3934 3320 3137 2e39 3033 3337 362c  10943 17.903376,
-000038d0: 3138 2e39 3435 3033 3320 3139 2e30 3432  18.945033 19.042
-000038e0: 3037 382c 3136 2e36 3238 3730 3320 4320  078,16.628703 C 
-000038f0: 3139 2e37 3537 3234 322c 3135 2e32 3631  19.757242,15.261
-00003900: 3232 3720 3139 2e33 3036 3831 392c 3133  227 19.306819,13
-00003910: 2e32 3434 3932 3920 3137 2e37 3635 392c  .244929 17.7659,
-00003920: 3132 2e36 3731 3930 3220 4320 3136 2e37  12.671902 C 16.7
-00003930: 3538 3335 2c31 322e 3231 3039 3631 2031  5835,12.210961 1
-00003940: 352e 3436 3230 3933 2c31 322e 3434 3239  5.462093,12.4429
-00003950: 3531 2031 342e 3732 3933 3636 2c31 332e  51 14.729366,13.
-00003960: 3239 3030 3134 2043 2031 352e 3637 3938  290014 C 15.6798
-00003970: 3439 2c31 332e 3237 3631 3533 2031 362e  49,13.276153 16.
-00003980: 3938 3032 3934 2c31 332e 3236 3237 3534  980294,13.262754
-00003990: 2031 372e 3334 3335 3032 2c31 342e 3336   17.343502,14.36
-000039a0: 3432 3033 2043 2031 372e 3930 3332 3633  4203 C 17.903263
-000039b0: 2c31 352e 3439 3236 3739 2031 372e 3736  ,15.492679 17.76
-000039c0: 3936 3737 2c31 372e 3330 3539 3732 2031  9677,17.305972 1
-000039d0: 362e 3431 3439 3439 2c31 372e 3738 3138  6.414949,17.7818
-000039e0: 3935 2043 2031 352e 3231 3834 3138 2c31  95 C 15.218418,1
-000039f0: 382e 3133 3038 3420 3134 2e31 3530 3330  8.13084 14.15030
-00003a00: 332c 3136 2e39 3032 3934 3720 3134 2e30  3,16.902947 14.0
-00003a10: 3932 3138 342c 3135 2e37 3831 3636 3620  92184,15.781666 
-00003a20: 4320 3133 2e37 3832 3131 372c 3134 2e31  C 13.782117,14.1
-00003a30: 3031 3430 3320 3134 2e31 3430 3334 362c  01403 14.140346,
-00003a40: 3132 2e32 3730 3331 3520 3135 2e32 3735  12.270315 15.275
-00003a50: 3139 2c31 302e 3935 3830 3432 2043 2031  19,10.958042 C 1
-00003a60: 362e 3531 3938 3933 2c39 2e34 3934 3837  6.519893,9.49487
-00003a70: 3633 2031 372e 3235 3635 3235 2c37 2e35  63 17.256525,7.5
-00003a80: 3234 3036 3539 2031 362e 3836 3735 3236  240659 16.867526
-00003a90: 2c35 2e35 3939 3437 3531 2043 2031 362e  ,5.5994751 C 16.
-00003aa0: 3336 3430 392c 322e 3536 3537 3234 3920  36409,2.5657249 
-00003ab0: 3133 2e36 3035 3030 312c 302e 3036 3537  13.605001,0.0657
-00003ac0: 3630 3534 3320 3130 2e35 3037 3330 392c  60543 10.507309,
-00003ad0: 2d30 2e30 3034 3735 3437 3236 3520 4320  -0.0047547265 C 
-00003ae0: 392e 3934 3130 3733 2c2d 302e 3031 3538  9.941073,-0.0158
-00003af0: 3330 3639 3220 392e 3337 3232 3539 342c  30692 9.3722594,
-00003b00: 302e 3030 3933 3437 3836 3139 2038 2e38  0.0093478619 8.8
-00003b10: 3039 3630 3436 2c30 2e30 3735 3636 3638  096046,0.0756668
-00003b20: 3937 207a 220a 2020 2020 2020 2020 2020  97 z".          
-00003b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b40: 2020 7374 796c 653d 2266 696c 6c3a 2024    style="fill: $
-00003b50: 706c 616e 6574 735f 636f 6c6f 725f 3130  planets_color_10
-00003b60: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00003b70: 2020 2020 2020 2020 2020 2f3e 0a20 2020            />.   
-00003b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b90: 203c 2f67 3e0a 2020 2020 2020 2020 2020   </g>.          
-00003ba0: 2020 2020 2020 3c2f 7379 6d62 6f6c 3e0a        </symbol>.
-00003bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bc0: 3c73 796d 626f 6c20 6964 3d22 5472 7565  <symbol id="True
-00003bd0: 5f4e 6f64 6522 3e0a 2020 2020 2020 2020  _Node">.        
-00003be0: 2020 2020 2020 2020 2020 2020 3c67 2074              <g t
-00003bf0: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-00003c00: 6174 6528 302c 3329 223e 0a20 2020 2020  ate(0,3)">.     
-00003c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c20: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-00003c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c40: 2020 2020 2064 3d22 4d20 382e 3830 3936       d="M 8.8096
-00003c50: 3034 362c 302e 3037 3536 3636 3839 3720  046,0.075666897 
-00003c60: 4320 362e 3431 3537 3533 362c 302e 3636  C 6.4157536,0.66
-00003c70: 3132 3339 3632 2034 2e33 3736 3737 3639  123962 4.3767769
-00003c80: 2c32 2e35 3330 3638 3337 2033 2e36 3633  ,2.5306837 3.663
-00003c90: 3436 3536 2c34 2e39 3030 3735 3134 2043  4656,4.9007514 C
-00003ca0: 2033 2e30 3533 3630 3731 2c36 2e36 3830   3.0536071,6.680
-00003cb0: 3932 3634 2033 2e36 3836 3836 3832 2c38  9264 3.6868682,8
-00003cc0: 2e36 3233 3839 3031 2034 2e35 3837 3839  .6238901 4.58789
-00003cd0: 3838 2c31 302e 3138 3634 3337 2043 2035  88,10.186437 C 5
-00003ce0: 2e31 3332 3339 3937 2c31 312e 3132 3436  .1323997,11.1246
-00003cf0: 3232 2035 2e39 3631 3537 3533 2c31 312e  22 5.9615753,11.
-00003d00: 3930 3839 3520 362e 3139 3037 3330 322c  90895 6.1907302,
-00003d10: 3133 2e30 3037 3930 3620 4320 362e 3539  13.007906 C 6.59
-00003d20: 3137 3230 322c 3134 2e34 3834 3438 3820  17202,14.484488 
-00003d30: 362e 3438 3837 3135 362c 3136 2e33 3837  6.4887156,16.387
-00003d40: 3532 3320 352e 3137 3233 3738 382c 3137  523 5.1723788,17
-00003d50: 2e33 3832 3537 3620 4320 342e 3333 3239  .382576 C 4.3329
-00003d60: 3937 342c 3138 2e30 3533 3431 3320 332e  974,18.053413 3.
-00003d70: 3037 3735 3734 312c 3137 2e34 3535 3033  0775741,17.45503
-00003d80: 3420 322e 3832 3030 3133 362c 3136 2e34  4 2.8200136,16.4
-00003d90: 3831 3139 3620 4320 322e 3339 3136 3535  81196 C 2.391655
-00003da0: 322c 3135 2e31 3030 3739 3320 332e 3332  2,15.100793 3.32
-00003db0: 3331 3839 382c 3133 2e33 3936 3435 3620  31898,13.396456 
-00003dc0: 342e 3737 3933 3331 362c 3133 2e31 3633  4.7793316,13.163
-00003dd0: 3830 3620 4320 352e 3531 3537 3836 312c  806 C 5.5157861,
-00003de0: 3133 2e34 3438 3438 3920 352e 3733 3632  13.448489 5.7362
-00003df0: 3335 332c 3133 2e30 3038 3333 3120 342e  353,13.008331 4.
-00003e00: 3938 3830 3531 2c31 322e 3733 3931 3031  988051,12.739101
-00003e10: 2043 2033 2e34 3736 3736 3936 2c31 312e   C 3.4767696,11.
-00003e20: 3938 3037 3631 2031 2e32 3433 3138 3936  980761 1.2431896
-00003e30: 2c31 322e 3833 3936 3920 312e 3033 3531  ,12.83969 1.0351
-00003e40: 3437 362c 3134 2e36 3335 3339 3420 4320  476,14.635394 C 
-00003e50: 302e 3737 3434 3537 3135 2c31 362e 3239  0.77445715,16.29
-00003e60: 3835 3832 2031 2e39 3532 3838 3437 2c31  8582 1.9528847,1
-00003e70: 372e 3939 3138 3335 2033 2e35 3839 3539  7.991835 3.58959
-00003e80: 3633 2c31 382e 3335 3734 3539 2043 2035  63,18.357459 C 5
-00003e90: 2e34 3237 3636 3632 2c31 382e 3939 3431  .4276662,18.9941
-00003ea0: 3635 2037 2e36 3636 3138 3339 2c31 372e  65 7.6661839,17.
-00003eb0: 3936 3835 3334 2038 2e32 3937 3930 3339  968534 8.2979039
-00003ec0: 2c31 362e 3131 3031 3632 2043 2038 2e38  ,16.110162 C 8.8
-00003ed0: 3537 3130 3235 2c31 342e 3731 3635 3237  571025,14.716527
-00003ee0: 2038 2e35 3436 3534 3831 2c31 332e 3138   8.5465481,13.18
-00003ef0: 3631 3339 2038 2e30 3238 3938 3638 2c31  6139 8.0289868,1
-00003f00: 312e 3833 3236 3533 2043 2037 2e34 3730  1.832653 C 7.470
-00003f10: 3238 3835 2c31 302e 3230 3638 3834 2036  2885,10.206884 6
-00003f20: 2e32 3535 3336 3633 2c38 2e38 3730 3936  .2553663,8.87096
-00003f30: 3734 2035 2e39 3239 3930 3536 2c37 2e31  74 5.9299056,7.1
-00003f40: 3532 3538 3338 2043 2035 2e34 3931 3436  525838 C 5.49146
-00003f50: 2c35 2e34 3932 3939 3635 2035 2e38 3837  ,5.4929965 5.887
-00003f60: 3534 3938 2c33 2e35 3733 3536 3239 2037  5498,3.5735629 7
-00003f70: 2e32 3332 3936 3037 2c32 2e34 3332 3732  .2329607,2.43272
-00003f80: 3133 2043 2038 2e37 3338 3835 3931 2c31  13 C 8.7388591,1
-00003f90: 2e30 3133 3434 3531 2031 312e 3331 3839  .0134451 11.3189
-00003fa0: 3331 2c30 2e37 3535 3730 3832 2031 322e  31,0.7557082 12.
-00003fb0: 3931 3938 3138 2c32 2e31 3632 3737 3233  919818,2.1627723
-00003fc0: 2043 2031 342e 3839 3131 3734 2c33 2e36   C 14.891174,3.6
-00003fd0: 3736 3933 3435 2031 352e 3239 3530 3635  769345 15.295065
-00003fe0: 2c36 2e35 3639 3230 3238 2031 342e 3333  ,6.5692028 14.33
-00003ff0: 3032 3337 2c38 2e37 3637 3139 3333 2043  0237,8.7671933 C
-00004000: 2031 332e 3931 3034 3834 2c39 2e39 3139   13.910484,9.919
-00004010: 3336 3538 2031 332e 3135 3433 3533 2c31  3658 13.154353,1
-00004020: 302e 3930 3236 3739 2031 322e 3631 3538  0.902679 12.6158
-00004030: 3737 2c31 312e 3939 3132 3939 2043 2031  77,11.991299 C 1
-00004040: 322e 3033 3830 3435 2c31 332e 3534 3832  2.038045,13.5482
-00004050: 3620 3132 2e30 3830 3539 392c 3135 2e33  6 12.080599,15.3
-00004060: 3634 3831 3320 3132 2e37 3737 3435 352c  64813 12.777455,
-00004070: 3136 2e38 3735 3136 3320 4320 3134 2e30  16.875163 C 14.0
-00004080: 3736 3934 362c 3139 2e31 3130 3934 3320  76946,19.110943 
-00004090: 3137 2e39 3033 3337 362c 3138 2e39 3435  17.903376,18.945
-000040a0: 3033 3320 3139 2e30 3432 3037 382c 3136  033 19.042078,16
-000040b0: 2e36 3238 3730 3320 4320 3139 2e37 3537  .628703 C 19.757
-000040c0: 3234 322c 3135 2e32 3631 3232 3720 3139  242,15.261227 19
-000040d0: 2e33 3036 3831 392c 3133 2e32 3434 3932  .306819,13.24492
-000040e0: 3920 3137 2e37 3635 392c 3132 2e36 3731  9 17.7659,12.671
-000040f0: 3930 3220 4320 3136 2e37 3538 3335 2c31  902 C 16.75835,1
-00004100: 322e 3231 3039 3631 2031 352e 3436 3230  2.210961 15.4620
-00004110: 3933 2c31 322e 3434 3239 3531 2031 342e  93,12.442951 14.
-00004120: 3732 3933 3636 2c31 332e 3239 3030 3134  729366,13.290014
-00004130: 2043 2031 352e 3637 3938 3439 2c31 332e   C 15.679849,13.
-00004140: 3237 3631 3533 2031 362e 3938 3032 3934  276153 16.980294
-00004150: 2c31 332e 3236 3237 3534 2031 372e 3334  ,13.262754 17.34
-00004160: 3335 3032 2c31 342e 3336 3432 3033 2043  3502,14.364203 C
-00004170: 2031 372e 3930 3332 3633 2c31 352e 3439   17.903263,15.49
-00004180: 3236 3739 2031 372e 3736 3936 3737 2c31  2679 17.769677,1
-00004190: 372e 3330 3539 3732 2031 362e 3431 3439  7.305972 16.4149
-000041a0: 3439 2c31 372e 3738 3138 3935 2043 2031  49,17.781895 C 1
-000041b0: 352e 3231 3834 3138 2c31 382e 3133 3038  5.218418,18.1308
-000041c0: 3420 3134 2e31 3530 3330 332c 3136 2e39  4 14.150303,16.9
-000041d0: 3032 3934 3720 3134 2e30 3932 3138 342c  02947 14.092184,
-000041e0: 3135 2e37 3831 3636 3620 4320 3133 2e37  15.781666 C 13.7
-000041f0: 3832 3131 372c 3134 2e31 3031 3430 3320  82117,14.101403 
-00004200: 3134 2e31 3430 3334 362c 3132 2e32 3730  14.140346,12.270
-00004210: 3331 3520 3135 2e32 3735 3139 2c31 302e  315 15.27519,10.
-00004220: 3935 3830 3432 2043 2031 362e 3531 3938  958042 C 16.5198
-00004230: 3933 2c39 2e34 3934 3837 3633 2031 372e  93,9.4948763 17.
-00004240: 3235 3635 3235 2c37 2e35 3234 3036 3539  256525,7.5240659
-00004250: 2031 362e 3836 3735 3236 2c35 2e35 3939   16.867526,5.599
-00004260: 3437 3531 2043 2031 362e 3336 3430 392c  4751 C 16.36409,
-00004270: 322e 3536 3537 3234 3920 3133 2e36 3035  2.5657249 13.605
-00004280: 3030 312c 302e 3036 3537 3630 3534 3320  001,0.065760543 
-00004290: 3130 2e35 3037 3330 392c 2d30 2e30 3034  10.507309,-0.004
-000042a0: 3735 3437 3236 3520 4320 392e 3934 3130  7547265 C 9.9410
-000042b0: 3733 2c2d 302e 3031 3538 3330 3639 3220  73,-0.015830692 
-000042c0: 392e 3337 3232 3539 342c 302e 3030 3933  9.3722594,0.0093
-000042d0: 3437 3836 3139 2038 2e38 3039 3630 3436  478619 8.8096046
-000042e0: 2c30 2e30 3735 3636 3638 3937 207a 220a  ,0.075666897 z".
-000042f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004300: 2020 2020 2020 2020 2020 2020 7374 796c              styl
-00004310: 653d 2266 696c 6c3a 2024 706c 616e 6574  e="fill: $planet
-00004320: 735f 636f 6c6f 725f 3131 220a 2020 2020  s_color_11".    
-00004330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004340: 2020 2020 2f3e 0a20 2020 2020 2020 2020      />.         
-00004350: 2020 2020 2020 2020 2020 203c 2f67 3e0a             </g>.
-00004360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004370: 3c2f 7379 6d62 6f6c 3e0a 2020 2020 2020  </symbol>.      
-00004380: 2020 2020 2020 2020 2020 3c73 796d 626f            <symbo
-00004390: 6c20 6964 3d22 4368 6972 6f6e 223e 0a09  l id="Chiron">..
-000043a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043b0: 3c70 6174 680a 0920 2020 2020 2020 2020  <path..         
-000043c0: 2020 2020 2020 2020 2064 3d22 4d20 3130           d="M 10
-000043d0: 2e30 3139 3837 332c 3133 2e30 3638 3938  .019873,13.06898
-000043e0: 3120 4c20 3130 2e31 3835 3534 322c 302e  1 L 10.185542,0.
-000043f0: 3830 3935 3134 3331 204d 2031 302e 3139  80951431 M 10.19
-00004400: 3535 3931 2c36 2e37 3434 3239 3031 204c  5591,6.7442901 L
-00004410: 2031 352e 3439 3639 3833 2c32 2e32 3731   15.496983,2.271
-00004420: 3234 3038 204d 2031 302e 3231 3438 3331  2408 M 10.214831
-00004430: 2c36 2e36 3332 3137 3236 204c 2031 352e  ,6.6321726 L 15.
-00004440: 3531 3632 3137 2c31 312e 3130 3532 3136  516217,11.105216
-00004450: 204d 2031 372e 3139 3239 3334 2c31 372e   M 17.192934,17.
-00004460: 3939 3837 3734 2043 2031 372e 3139 3239  998774 C 17.1929
-00004470: 3334 2c32 302e 3836 3436 2031 342e 3836  34,20.8646 14.86
-00004480: 3730 3532 2c32 332e 3139 3034 3837 2031  7052,23.190487 1
-00004490: 322e 3030 3132 3236 2c32 332e 3139 3034  2.001226,23.1904
-000044a0: 3837 2043 2039 2e31 3335 3339 3838 2c32  87 C 9.1353988,2
-000044b0: 332e 3139 3034 3837 2036 2e38 3039 3531  3.190487 6.80951
-000044c0: 3238 2c32 302e 3836 3436 2036 2e38 3039  28,20.8646 6.809
-000044d0: 3531 3238 2c31 372e 3939 3837 3734 2043  5128,17.998774 C
-000044e0: 2036 2e38 3039 3531 3238 2c31 352e 3133   6.8095128,15.13
-000044f0: 3239 3533 2039 2e31 3335 3339 3838 2c31  2953 9.1353988,1
-00004500: 322e 3830 3730 3636 2031 322e 3030 3132  2.807066 12.0012
-00004510: 3236 2c31 322e 3830 3730 3636 2043 2031  26,12.807066 C 1
-00004520: 342e 3836 3730 3532 2c31 322e 3830 3730  4.867052,12.8070
-00004530: 3636 2031 372e 3139 3239 3334 2c31 352e  66 17.192934,15.
-00004540: 3133 3239 3533 2031 372e 3139 3239 3334  132953 17.192934
-00004550: 2c31 372e 3939 3837 3734 207a 2022 0a09  ,17.998774 z "..
+00003420: 2020 2020 2020 2064 3d22 4d20 382e 3830         d="M 8.80
+00003430: 3936 3034 362c 302e 3037 3536 3636 3839  96046,0.07566689
+00003440: 3720 4320 362e 3431 3537 3533 362c 302e  7 C 6.4157536,0.
+00003450: 3636 3132 3339 3632 2034 2e33 3736 3737  66123962 4.37677
+00003460: 3639 2c32 2e35 3330 3638 3337 2033 2e36  69,2.5306837 3.6
+00003470: 3633 3436 3536 2c34 2e39 3030 3735 3134  634656,4.9007514
+00003480: 2043 2033 2e30 3533 3630 3731 2c36 2e36   C 3.0536071,6.6
+00003490: 3830 3932 3634 2033 2e36 3836 3836 3832  809264 3.6868682
+000034a0: 2c38 2e36 3233 3839 3031 2034 2e35 3837  ,8.6238901 4.587
+000034b0: 3839 3838 2c31 302e 3138 3634 3337 2043  8988,10.186437 C
+000034c0: 2035 2e31 3332 3339 3937 2c31 312e 3132   5.1323997,11.12
+000034d0: 3436 3232 2035 2e39 3631 3537 3533 2c31  4622 5.9615753,1
+000034e0: 312e 3930 3839 3520 362e 3139 3037 3330  1.90895 6.190730
+000034f0: 322c 3133 2e30 3037 3930 3620 4320 362e  2,13.007906 C 6.
+00003500: 3539 3137 3230 322c 3134 2e34 3834 3438  5917202,14.48448
+00003510: 3820 362e 3438 3837 3135 362c 3136 2e33  8 6.4887156,16.3
+00003520: 3837 3532 3320 352e 3137 3233 3738 382c  87523 5.1723788,
+00003530: 3137 2e33 3832 3537 3620 4320 342e 3333  17.382576 C 4.33
+00003540: 3239 3937 342c 3138 2e30 3533 3431 3320  29974,18.053413 
+00003550: 332e 3037 3735 3734 312c 3137 2e34 3535  3.0775741,17.455
+00003560: 3033 3420 322e 3832 3030 3133 362c 3136  034 2.8200136,16
+00003570: 2e34 3831 3139 3620 4320 322e 3339 3136  .481196 C 2.3916
+00003580: 3535 322c 3135 2e31 3030 3739 3320 332e  552,15.100793 3.
+00003590: 3332 3331 3839 382c 3133 2e33 3936 3435  3231898,13.39645
+000035a0: 3620 342e 3737 3933 3331 362c 3133 2e31  6 4.7793316,13.1
+000035b0: 3633 3830 3620 4320 352e 3531 3537 3836  63806 C 5.515786
+000035c0: 312c 3133 2e34 3438 3438 3920 352e 3733  1,13.448489 5.73
+000035d0: 3632 3335 332c 3133 2e30 3038 3333 3120  62353,13.008331 
+000035e0: 342e 3938 3830 3531 2c31 322e 3733 3931  4.988051,12.7391
+000035f0: 3031 2043 2033 2e34 3736 3736 3936 2c31  01 C 3.4767696,1
+00003600: 312e 3938 3037 3631 2031 2e32 3433 3138  1.980761 1.24318
+00003610: 3936 2c31 322e 3833 3936 3920 312e 3033  96,12.83969 1.03
+00003620: 3531 3437 362c 3134 2e36 3335 3339 3420  51476,14.635394 
+00003630: 4320 302e 3737 3434 3537 3135 2c31 362e  C 0.77445715,16.
+00003640: 3239 3835 3832 2031 2e39 3532 3838 3437  298582 1.9528847
+00003650: 2c31 372e 3939 3138 3335 2033 2e35 3839  ,17.991835 3.589
+00003660: 3539 3633 2c31 382e 3335 3734 3539 2043  5963,18.357459 C
+00003670: 2035 2e34 3237 3636 3632 2c31 382e 3939   5.4276662,18.99
+00003680: 3431 3635 2037 2e36 3636 3138 3339 2c31  4165 7.6661839,1
+00003690: 372e 3936 3835 3334 2038 2e32 3937 3930  7.968534 8.29790
+000036a0: 3339 2c31 362e 3131 3031 3632 2043 2038  39,16.110162 C 8
+000036b0: 2e38 3537 3130 3235 2c31 342e 3731 3635  .8571025,14.7165
+000036c0: 3237 2038 2e35 3436 3534 3831 2c31 332e  27 8.5465481,13.
+000036d0: 3138 3631 3339 2038 2e30 3238 3938 3638  186139 8.0289868
+000036e0: 2c31 312e 3833 3236 3533 2043 2037 2e34  ,11.832653 C 7.4
+000036f0: 3730 3238 3835 2c31 302e 3230 3638 3834  702885,10.206884
+00003700: 2036 2e32 3535 3336 3633 2c38 2e38 3730   6.2553663,8.870
+00003710: 3936 3734 2035 2e39 3239 3930 3536 2c37  9674 5.9299056,7
+00003720: 2e31 3532 3538 3338 2043 2035 2e34 3931  .1525838 C 5.491
+00003730: 3436 2c35 2e34 3932 3939 3635 2035 2e38  46,5.4929965 5.8
+00003740: 3837 3534 3938 2c33 2e35 3733 3536 3239  875498,3.5735629
+00003750: 2037 2e32 3332 3936 3037 2c32 2e34 3332   7.2329607,2.432
+00003760: 3732 3133 2043 2038 2e37 3338 3835 3931  7213 C 8.7388591
+00003770: 2c31 2e30 3133 3434 3531 2031 312e 3331  ,1.0134451 11.31
+00003780: 3839 3331 2c30 2e37 3535 3730 3832 2031  8931,0.7557082 1
+00003790: 322e 3931 3938 3138 2c32 2e31 3632 3737  2.919818,2.16277
+000037a0: 3233 2043 2031 342e 3839 3131 3734 2c33  23 C 14.891174,3
+000037b0: 2e36 3736 3933 3435 2031 352e 3239 3530  .6769345 15.2950
+000037c0: 3635 2c36 2e35 3639 3230 3238 2031 342e  65,6.5692028 14.
+000037d0: 3333 3032 3337 2c38 2e37 3637 3139 3333  330237,8.7671933
+000037e0: 2043 2031 332e 3931 3034 3834 2c39 2e39   C 13.910484,9.9
+000037f0: 3139 3336 3538 2031 332e 3135 3433 3533  193658 13.154353
+00003800: 2c31 302e 3930 3236 3739 2031 322e 3631  ,10.902679 12.61
+00003810: 3538 3737 2c31 312e 3939 3132 3939 2043  5877,11.991299 C
+00003820: 2031 322e 3033 3830 3435 2c31 332e 3534   12.038045,13.54
+00003830: 3832 3620 3132 2e30 3830 3539 392c 3135  826 12.080599,15
+00003840: 2e33 3634 3831 3320 3132 2e37 3737 3435  .364813 12.77745
+00003850: 352c 3136 2e38 3735 3136 3320 4320 3134  5,16.875163 C 14
+00003860: 2e30 3736 3934 362c 3139 2e31 3130 3934  .076946,19.11094
+00003870: 3320 3137 2e39 3033 3337 362c 3138 2e39  3 17.903376,18.9
+00003880: 3435 3033 3320 3139 2e30 3432 3037 382c  45033 19.042078,
+00003890: 3136 2e36 3238 3730 3320 4320 3139 2e37  16.628703 C 19.7
+000038a0: 3537 3234 322c 3135 2e32 3631 3232 3720  57242,15.261227 
+000038b0: 3139 2e33 3036 3831 392c 3133 2e32 3434  19.306819,13.244
+000038c0: 3932 3920 3137 2e37 3635 392c 3132 2e36  929 17.7659,12.6
+000038d0: 3731 3930 3220 4320 3136 2e37 3538 3335  71902 C 16.75835
+000038e0: 2c31 322e 3231 3039 3631 2031 352e 3436  ,12.210961 15.46
+000038f0: 3230 3933 2c31 322e 3434 3239 3531 2031  2093,12.442951 1
+00003900: 342e 3732 3933 3636 2c31 332e 3239 3030  4.729366,13.2900
+00003910: 3134 2043 2031 352e 3637 3938 3439 2c31  14 C 15.679849,1
+00003920: 332e 3237 3631 3533 2031 362e 3938 3032  3.276153 16.9802
+00003930: 3934 2c31 332e 3236 3237 3534 2031 372e  94,13.262754 17.
+00003940: 3334 3335 3032 2c31 342e 3336 3432 3033  343502,14.364203
+00003950: 2043 2031 372e 3930 3332 3633 2c31 352e   C 17.903263,15.
+00003960: 3439 3236 3739 2031 372e 3736 3936 3737  492679 17.769677
+00003970: 2c31 372e 3330 3539 3732 2031 362e 3431  ,17.305972 16.41
+00003980: 3439 3439 2c31 372e 3738 3138 3935 2043  4949,17.781895 C
+00003990: 2031 352e 3231 3834 3138 2c31 382e 3133   15.218418,18.13
+000039a0: 3038 3420 3134 2e31 3530 3330 332c 3136  084 14.150303,16
+000039b0: 2e39 3032 3934 3720 3134 2e30 3932 3138  .902947 14.09218
+000039c0: 342c 3135 2e37 3831 3636 3620 4320 3133  4,15.781666 C 13
+000039d0: 2e37 3832 3131 372c 3134 2e31 3031 3430  .782117,14.10140
+000039e0: 3320 3134 2e31 3430 3334 362c 3132 2e32  3 14.140346,12.2
+000039f0: 3730 3331 3520 3135 2e32 3735 3139 2c31  70315 15.27519,1
+00003a00: 302e 3935 3830 3432 2043 2031 362e 3531  0.958042 C 16.51
+00003a10: 3938 3933 2c39 2e34 3934 3837 3633 2031  9893,9.4948763 1
+00003a20: 372e 3235 3635 3235 2c37 2e35 3234 3036  7.256525,7.52406
+00003a30: 3539 2031 362e 3836 3735 3236 2c35 2e35  59 16.867526,5.5
+00003a40: 3939 3437 3531 2043 2031 362e 3336 3430  994751 C 16.3640
+00003a50: 392c 322e 3536 3537 3234 3920 3133 2e36  9,2.5657249 13.6
+00003a60: 3035 3030 312c 302e 3036 3537 3630 3534  05001,0.06576054
+00003a70: 3320 3130 2e35 3037 3330 392c 2d30 2e30  3 10.507309,-0.0
+00003a80: 3034 3735 3437 3236 3520 4320 392e 3934  047547265 C 9.94
+00003a90: 3130 3733 2c2d 302e 3031 3538 3330 3639  1073,-0.01583069
+00003aa0: 3220 392e 3337 3232 3539 342c 302e 3030  2 9.3722594,0.00
+00003ab0: 3933 3437 3836 3139 2038 2e38 3039 3630  93478619 8.80960
+00003ac0: 3436 2c30 2e30 3735 3636 3638 3937 207a  46,0.075666897 z
+00003ad0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00003ae0: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00003af0: 796c 653d 2266 696c 6c3a 2024 706c 616e  yle="fill: $plan
+00003b00: 6574 735f 636f 6c6f 725f 3130 220a 2020  ets_color_10".  
+00003b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b20: 2020 2020 2020 2f3e 0a20 2020 2020 2020        />.       
+00003b30: 2020 2020 2020 2020 2020 2020 203c 2f67               </g
+00003b40: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00003b50: 2020 3c2f 7379 6d62 6f6c 3e0a 2020 2020    </symbol>.    
+00003b60: 2020 2020 2020 2020 2020 2020 3c73 796d              <sym
+00003b70: 626f 6c20 6964 3d22 5472 7565 5f4e 6f64  bol id="True_Nod
+00003b80: 6522 3e0a 2020 2020 2020 2020 2020 2020  e">.            
+00003b90: 2020 2020 2020 2020 3c67 2074 7261 6e73          <g trans
+00003ba0: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
+00003bb0: 302c 3329 223e 0a20 2020 2020 2020 2020  0,3)">.         
+00003bc0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00003bd0: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
+00003be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bf0: 2064 3d22 4d20 382e 3830 3936 3034 362c   d="M 8.8096046,
+00003c00: 302e 3037 3536 3636 3839 3720 4320 362e  0.075666897 C 6.
+00003c10: 3431 3537 3533 362c 302e 3636 3132 3339  4157536,0.661239
+00003c20: 3632 2034 2e33 3736 3737 3639 2c32 2e35  62 4.3767769,2.5
+00003c30: 3330 3638 3337 2033 2e36 3633 3436 3536  306837 3.6634656
+00003c40: 2c34 2e39 3030 3735 3134 2043 2033 2e30  ,4.9007514 C 3.0
+00003c50: 3533 3630 3731 2c36 2e36 3830 3932 3634  536071,6.6809264
+00003c60: 2033 2e36 3836 3836 3832 2c38 2e36 3233   3.6868682,8.623
+00003c70: 3839 3031 2034 2e35 3837 3839 3838 2c31  8901 4.5878988,1
+00003c80: 302e 3138 3634 3337 2043 2035 2e31 3332  0.186437 C 5.132
+00003c90: 3339 3937 2c31 312e 3132 3436 3232 2035  3997,11.124622 5
+00003ca0: 2e39 3631 3537 3533 2c31 312e 3930 3839  .9615753,11.9089
+00003cb0: 3520 362e 3139 3037 3330 322c 3133 2e30  5 6.1907302,13.0
+00003cc0: 3037 3930 3620 4320 362e 3539 3137 3230  07906 C 6.591720
+00003cd0: 322c 3134 2e34 3834 3438 3820 362e 3438  2,14.484488 6.48
+00003ce0: 3837 3135 362c 3136 2e33 3837 3532 3320  87156,16.387523 
+00003cf0: 352e 3137 3233 3738 382c 3137 2e33 3832  5.1723788,17.382
+00003d00: 3537 3620 4320 342e 3333 3239 3937 342c  576 C 4.3329974,
+00003d10: 3138 2e30 3533 3431 3320 332e 3037 3735  18.053413 3.0775
+00003d20: 3734 312c 3137 2e34 3535 3033 3420 322e  741,17.455034 2.
+00003d30: 3832 3030 3133 362c 3136 2e34 3831 3139  8200136,16.48119
+00003d40: 3620 4320 322e 3339 3136 3535 322c 3135  6 C 2.3916552,15
+00003d50: 2e31 3030 3739 3320 332e 3332 3331 3839  .100793 3.323189
+00003d60: 382c 3133 2e33 3936 3435 3620 342e 3737  8,13.396456 4.77
+00003d70: 3933 3331 362c 3133 2e31 3633 3830 3620  93316,13.163806 
+00003d80: 4320 352e 3531 3537 3836 312c 3133 2e34  C 5.5157861,13.4
+00003d90: 3438 3438 3920 352e 3733 3632 3335 332c  48489 5.7362353,
+00003da0: 3133 2e30 3038 3333 3120 342e 3938 3830  13.008331 4.9880
+00003db0: 3531 2c31 322e 3733 3931 3031 2043 2033  51,12.739101 C 3
+00003dc0: 2e34 3736 3736 3936 2c31 312e 3938 3037  .4767696,11.9807
+00003dd0: 3631 2031 2e32 3433 3138 3936 2c31 322e  61 1.2431896,12.
+00003de0: 3833 3936 3920 312e 3033 3531 3437 362c  83969 1.0351476,
+00003df0: 3134 2e36 3335 3339 3420 4320 302e 3737  14.635394 C 0.77
+00003e00: 3434 3537 3135 2c31 362e 3239 3835 3832  445715,16.298582
+00003e10: 2031 2e39 3532 3838 3437 2c31 372e 3939   1.9528847,17.99
+00003e20: 3138 3335 2033 2e35 3839 3539 3633 2c31  1835 3.5895963,1
+00003e30: 382e 3335 3734 3539 2043 2035 2e34 3237  8.357459 C 5.427
+00003e40: 3636 3632 2c31 382e 3939 3431 3635 2037  6662,18.994165 7
+00003e50: 2e36 3636 3138 3339 2c31 372e 3936 3835  .6661839,17.9685
+00003e60: 3334 2038 2e32 3937 3930 3339 2c31 362e  34 8.2979039,16.
+00003e70: 3131 3031 3632 2043 2038 2e38 3537 3130  110162 C 8.85710
+00003e80: 3235 2c31 342e 3731 3635 3237 2038 2e35  25,14.716527 8.5
+00003e90: 3436 3534 3831 2c31 332e 3138 3631 3339  465481,13.186139
+00003ea0: 2038 2e30 3238 3938 3638 2c31 312e 3833   8.0289868,11.83
+00003eb0: 3236 3533 2043 2037 2e34 3730 3238 3835  2653 C 7.4702885
+00003ec0: 2c31 302e 3230 3638 3834 2036 2e32 3535  ,10.206884 6.255
+00003ed0: 3336 3633 2c38 2e38 3730 3936 3734 2035  3663,8.8709674 5
+00003ee0: 2e39 3239 3930 3536 2c37 2e31 3532 3538  .9299056,7.15258
+00003ef0: 3338 2043 2035 2e34 3931 3436 2c35 2e34  38 C 5.49146,5.4
+00003f00: 3932 3939 3635 2035 2e38 3837 3534 3938  929965 5.8875498
+00003f10: 2c33 2e35 3733 3536 3239 2037 2e32 3332  ,3.5735629 7.232
+00003f20: 3936 3037 2c32 2e34 3332 3732 3133 2043  9607,2.4327213 C
+00003f30: 2038 2e37 3338 3835 3931 2c31 2e30 3133   8.7388591,1.013
+00003f40: 3434 3531 2031 312e 3331 3839 3331 2c30  4451 11.318931,0
+00003f50: 2e37 3535 3730 3832 2031 322e 3931 3938  .7557082 12.9198
+00003f60: 3138 2c32 2e31 3632 3737 3233 2043 2031  18,2.1627723 C 1
+00003f70: 342e 3839 3131 3734 2c33 2e36 3736 3933  4.891174,3.67693
+00003f80: 3435 2031 352e 3239 3530 3635 2c36 2e35  45 15.295065,6.5
+00003f90: 3639 3230 3238 2031 342e 3333 3032 3337  692028 14.330237
+00003fa0: 2c38 2e37 3637 3139 3333 2043 2031 332e  ,8.7671933 C 13.
+00003fb0: 3931 3034 3834 2c39 2e39 3139 3336 3538  910484,9.9193658
+00003fc0: 2031 332e 3135 3433 3533 2c31 302e 3930   13.154353,10.90
+00003fd0: 3236 3739 2031 322e 3631 3538 3737 2c31  2679 12.615877,1
+00003fe0: 312e 3939 3132 3939 2043 2031 322e 3033  1.991299 C 12.03
+00003ff0: 3830 3435 2c31 332e 3534 3832 3620 3132  8045,13.54826 12
+00004000: 2e30 3830 3539 392c 3135 2e33 3634 3831  .080599,15.36481
+00004010: 3320 3132 2e37 3737 3435 352c 3136 2e38  3 12.777455,16.8
+00004020: 3735 3136 3320 4320 3134 2e30 3736 3934  75163 C 14.07694
+00004030: 362c 3139 2e31 3130 3934 3320 3137 2e39  6,19.110943 17.9
+00004040: 3033 3337 362c 3138 2e39 3435 3033 3320  03376,18.945033 
+00004050: 3139 2e30 3432 3037 382c 3136 2e36 3238  19.042078,16.628
+00004060: 3730 3320 4320 3139 2e37 3537 3234 322c  703 C 19.757242,
+00004070: 3135 2e32 3631 3232 3720 3139 2e33 3036  15.261227 19.306
+00004080: 3831 392c 3133 2e32 3434 3932 3920 3137  819,13.244929 17
+00004090: 2e37 3635 392c 3132 2e36 3731 3930 3220  .7659,12.671902 
+000040a0: 4320 3136 2e37 3538 3335 2c31 322e 3231  C 16.75835,12.21
+000040b0: 3039 3631 2031 352e 3436 3230 3933 2c31  0961 15.462093,1
+000040c0: 322e 3434 3239 3531 2031 342e 3732 3933  2.442951 14.7293
+000040d0: 3636 2c31 332e 3239 3030 3134 2043 2031  66,13.290014 C 1
+000040e0: 352e 3637 3938 3439 2c31 332e 3237 3631  5.679849,13.2761
+000040f0: 3533 2031 362e 3938 3032 3934 2c31 332e  53 16.980294,13.
+00004100: 3236 3237 3534 2031 372e 3334 3335 3032  262754 17.343502
+00004110: 2c31 342e 3336 3432 3033 2043 2031 372e  ,14.364203 C 17.
+00004120: 3930 3332 3633 2c31 352e 3439 3236 3739  903263,15.492679
+00004130: 2031 372e 3736 3936 3737 2c31 372e 3330   17.769677,17.30
+00004140: 3539 3732 2031 362e 3431 3439 3439 2c31  5972 16.414949,1
+00004150: 372e 3738 3138 3935 2043 2031 352e 3231  7.781895 C 15.21
+00004160: 3834 3138 2c31 382e 3133 3038 3420 3134  8418,18.13084 14
+00004170: 2e31 3530 3330 332c 3136 2e39 3032 3934  .150303,16.90294
+00004180: 3720 3134 2e30 3932 3138 342c 3135 2e37  7 14.092184,15.7
+00004190: 3831 3636 3620 4320 3133 2e37 3832 3131  81666 C 13.78211
+000041a0: 372c 3134 2e31 3031 3430 3320 3134 2e31  7,14.101403 14.1
+000041b0: 3430 3334 362c 3132 2e32 3730 3331 3520  40346,12.270315 
+000041c0: 3135 2e32 3735 3139 2c31 302e 3935 3830  15.27519,10.9580
+000041d0: 3432 2043 2031 362e 3531 3938 3933 2c39  42 C 16.519893,9
+000041e0: 2e34 3934 3837 3633 2031 372e 3235 3635  .4948763 17.2565
+000041f0: 3235 2c37 2e35 3234 3036 3539 2031 362e  25,7.5240659 16.
+00004200: 3836 3735 3236 2c35 2e35 3939 3437 3531  867526,5.5994751
+00004210: 2043 2031 362e 3336 3430 392c 322e 3536   C 16.36409,2.56
+00004220: 3537 3234 3920 3133 2e36 3035 3030 312c  57249 13.605001,
+00004230: 302e 3036 3537 3630 3534 3320 3130 2e35  0.065760543 10.5
+00004240: 3037 3330 392c 2d30 2e30 3034 3735 3437  07309,-0.0047547
+00004250: 3236 3520 4320 392e 3934 3130 3733 2c2d  265 C 9.941073,-
+00004260: 302e 3031 3538 3330 3639 3220 392e 3337  0.015830692 9.37
+00004270: 3232 3539 342c 302e 3030 3933 3437 3836  22594,0.00934786
+00004280: 3139 2038 2e38 3039 3630 3436 2c30 2e30  19 8.8096046,0.0
+00004290: 3735 3636 3638 3937 207a 220a 2020 2020  75666897 z".    
+000042a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042b0: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+000042c0: 696c 6c3a 2024 706c 616e 6574 735f 636f  ill: $planets_co
+000042d0: 6c6f 725f 3131 220a 2020 2020 2020 2020  lor_11".        
+000042e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042f0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00004300: 2020 2020 2020 203c 2f67 3e0a 2020 2020         </g>.    
+00004310: 2020 2020 2020 2020 2020 2020 3c2f 7379              </sy
+00004320: 6d62 6f6c 3e0a 2020 2020 2020 2020 2020  mbol>.          
+00004330: 2020 2020 2020 3c73 796d 626f 6c20 6964        <symbol id
+00004340: 3d22 4368 6972 6f6e 223e 0a09 2020 2020  ="Chiron">..    
+00004350: 2020 2020 2020 2020 2020 2020 3c70 6174              <pat
+00004360: 680a 0920 2020 2020 2020 2020 2020 2020  h..             
+00004370: 2020 2020 2064 3d22 4d20 3130 2e30 3139       d="M 10.019
+00004380: 3837 332c 3133 2e30 3638 3938 3120 4c20  873,13.068981 L 
+00004390: 3130 2e31 3835 3534 322c 302e 3830 3935  10.185542,0.8095
+000043a0: 3134 3331 204d 2031 302e 3139 3535 3931  1431 M 10.195591
+000043b0: 2c36 2e37 3434 3239 3031 204c 2031 352e  ,6.7442901 L 15.
+000043c0: 3439 3639 3833 2c32 2e32 3731 3234 3038  496983,2.2712408
+000043d0: 204d 2031 302e 3231 3438 3331 2c36 2e36   M 10.214831,6.6
+000043e0: 3332 3137 3236 204c 2031 352e 3531 3632  321726 L 15.5162
+000043f0: 3137 2c31 312e 3130 3532 3136 204d 2031  17,11.105216 M 1
+00004400: 372e 3139 3239 3334 2c31 372e 3939 3837  7.192934,17.9987
+00004410: 3734 2043 2031 372e 3139 3239 3334 2c32  74 C 17.192934,2
+00004420: 302e 3836 3436 2031 342e 3836 3730 3532  0.8646 14.867052
+00004430: 2c32 332e 3139 3034 3837 2031 322e 3030  ,23.190487 12.00
+00004440: 3132 3236 2c32 332e 3139 3034 3837 2043  1226,23.190487 C
+00004450: 2039 2e31 3335 3339 3838 2c32 332e 3139   9.1353988,23.19
+00004460: 3034 3837 2036 2e38 3039 3531 3238 2c32  0487 6.8095128,2
+00004470: 302e 3836 3436 2036 2e38 3039 3531 3238  0.8646 6.8095128
+00004480: 2c31 372e 3939 3837 3734 2043 2036 2e38  ,17.998774 C 6.8
+00004490: 3039 3531 3238 2c31 352e 3133 3239 3533  095128,15.132953
+000044a0: 2039 2e31 3335 3339 3838 2c31 322e 3830   9.1353988,12.80
+000044b0: 3730 3636 2031 322e 3030 3132 3236 2c31  7066 12.001226,1
+000044c0: 322e 3830 3730 3636 2043 2031 342e 3836  2.807066 C 14.86
+000044d0: 3730 3532 2c31 322e 3830 3730 3636 2031  7052,12.807066 1
+000044e0: 372e 3139 3239 3334 2c31 352e 3133 3239  7.192934,15.1329
+000044f0: 3533 2031 372e 3139 3239 3334 2c31 372e  53 17.192934,17.
+00004500: 3939 3837 3734 207a 2022 0a09 2020 2020  998774 z "..    
+00004510: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00004520: 796c 653d 2273 7472 6f6b 653a 2024 706c  yle="stroke: $pl
+00004530: 616e 6574 735f 636f 6c6f 725f 3136 3b73  anets_color_16;s
+00004540: 7472 6f6b 652d 7769 6474 683a 3270 783b  troke-width:2px;
+00004550: 2066 696c 6c3a 6e6f 6e65 3b22 202f 3e0a   fill:none;" />.
 00004560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004570: 2020 7374 796c 653d 2273 7472 6f6b 653a    style="stroke:
-00004580: 2024 706c 616e 6574 735f 636f 6c6f 725f   $planets_color_
-00004590: 3136 3b73 7472 6f6b 652d 7769 6474 683a  16;stroke-width:
-000045a0: 3270 783b 2066 696c 6c3a 6e6f 6e65 3b22  2px; fill:none;"
-000045b0: 202f 3e0a 2020 2020 2020 2020 2020 2020   />.            
-000045c0: 2020 2020 3c2f 7379 6d62 6f6c 3e0a 2020      </symbol>.  
-000045d0: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-000045e0: 796d 626f 6c20 6964 3d22 4669 7273 745f  ymbol id="First_
-000045f0: 486f 7573 6522 3e0a 2020 2020 2020 2020  House">.        
-00004600: 2020 2020 2020 2020 2020 2020 3c74 6578              <tex
-00004610: 7420 793d 2232 3022 2073 7479 6c65 3d22  t y="20" style="
-00004620: 666f 6e74 2d73 697a 653a 2032 3270 783b  font-size: 22px;
-00004630: 2066 696c 6c3a 2024 706c 616e 6574 735f   fill: $planets_
-00004640: 636f 6c6f 725f 3132 223e 4173 3c2f 7465  color_12">As</te
-00004650: 7874 3e0a 2020 2020 2020 2020 2020 2020  xt>.            
-00004660: 2020 2020 3c2f 7379 6d62 6f6c 3e0a 2020      </symbol>.  
-00004670: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-00004680: 796d 626f 6c20 6964 3d22 5465 6e74 685f  ymbol id="Tenth_
-00004690: 486f 7573 6522 3e0a 2020 2020 2020 2020  House">.        
-000046a0: 2020 2020 2020 2020 2020 2020 3c74 6578              <tex
-000046b0: 7420 793d 2232 3022 2073 7479 6c65 3d22  t y="20" style="
-000046c0: 666f 6e74 2d73 697a 653a 2032 3070 783b  font-size: 20px;
-000046d0: 2066 696c 6c3a 2024 706c 616e 6574 735f   fill: $planets_
-000046e0: 636f 6c6f 725f 3133 223e 4d63 3c2f 7465  color_13">Mc</te
-000046f0: 7874 3e0a 2020 2020 2020 2020 2020 2020  xt>.            
-00004700: 2020 2020 3c2f 7379 6d62 6f6c 3e0a 2020      </symbol>.  
-00004710: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-00004720: 796d 626f 6c20 6964 3d22 5365 7665 6e74  ymbol id="Sevent
-00004730: 685f 486f 7573 6522 3e0a 2020 2020 2020  h_House">.      
-00004740: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
-00004750: 6578 7420 793d 2232 3022 2073 7479 6c65  ext y="20" style
-00004760: 3d22 666f 6e74 2d73 697a 653a 2032 3270  ="font-size: 22p
-00004770: 783b 2066 696c 6c3a 2024 706c 616e 6574  x; fill: $planet
-00004780: 735f 636f 6c6f 725f 3134 223e 4473 3c2f  s_color_14">Ds</
-00004790: 7465 7874 3e0a 2020 2020 2020 2020 2020  text>.          
-000047a0: 2020 2020 2020 3c2f 7379 6d62 6f6c 3e0a        </symbol>.
-000047b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047c0: 3c73 796d 626f 6c20 6964 3d22 466f 7572  <symbol id="Four
-000047d0: 7468 5f48 6f75 7365 223e 0a20 2020 2020  th_House">.     
-000047e0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000047f0: 7465 7874 2079 3d22 3230 2220 7374 796c  text y="20" styl
-00004800: 653d 2266 6f6e 742d 7369 7a65 3a20 3232  e="font-size: 22
-00004810: 7078 3b20 6669 6c6c 3a20 2470 6c61 6e65  px; fill: $plane
-00004820: 7473 5f63 6f6c 6f72 5f31 3522 3e49 633c  ts_color_15">Ic<
-00004830: 2f74 6578 743e 0a20 2020 2020 2020 2020  /text>.         
-00004840: 2020 2020 2020 203c 2f73 796d 626f 6c3e         </symbol>
-00004850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004860: 203c 212d 2d20 5a6f 6469 6163 202d 2d3e   <!-- Zodiac -->
-00004870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004880: 203c 7379 6d62 6f6c 2069 643d 2261 7269   <symbol id="ari
-00004890: 6573 223e 0a20 2020 2020 2020 2020 2020  es">.           
-000048a0: 2020 2020 2020 2020 203c 7061 7468 0a20           <path. 
-000048b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048c0: 2020 2020 2020 2064 3d22 4d20 3134 2e38         d="M 14.8
-000048d0: 3333 3533 362c 3331 2043 2031 342e 3833  33536,31 C 14.83
-000048e0: 3231 3836 2c32 392e 3732 3832 3520 3134  2186,29.72825 14
-000048f0: 2e38 3435 3933 362c 3238 2e34 3535 3834  .845936,28.45584
-00004900: 2031 342e 3738 3033 3436 2c32 372e 3138   14.780346,27.18
-00004910: 3532 3320 4320 3134 2e36 3430 3932 362c  523 C 14.640926,
-00004920: 3234 2e32 3330 3436 2031 342e 3237 3139  24.23046 14.2719
-00004930: 3237 2c32 312e 3238 3937 3920 3133 2e37  27,21.28979 13.7
-00004940: 3631 3635 372c 3138 2e33 3737 3620 4320  61657,18.3776 C 
-00004950: 3133 2e33 3231 3938 372c 3135 2e39 3139  13.321987,15.919
-00004960: 3131 2031 322e 3738 3737 3837 2c31 332e  11 12.787787,13.
-00004970: 3436 3938 3320 3131 2e39 3930 3531 372c  46983 11.990517,
-00004980: 3131 2e31 3030 3735 2043 2031 312e 3533  11.10075 C 11.53
-00004990: 3032 3637 2c39 2e37 3632 3433 2031 302e  0267,9.76243 10.
-000049a0: 3939 3238 3837 2c38 2e34 3439 3132 2031  992887,8.44912 1
-000049b0: 302e 3335 3730 3837 2c37 2e31 3834 3920  0.357087,7.1849 
-000049c0: 4320 392e 3737 3634 3036 352c 362e 3035  C 9.7764065,6.05
-000049d0: 3420 392e 3131 3433 3436 352c 342e 3934  4 9.1143465,4.94
-000049e0: 3239 3620 382e 3231 3630 3036 352c 342e  296 8.2160065,4.
-000049f0: 3033 3439 3420 4320 372e 3632 3832 3436  03494 C 7.628246
-00004a00: 352c 332e 3434 3635 2036 2e39 3030 3732  5,3.4465 6.90072
-00004a10: 3635 2c32 2e39 3435 3335 2036 2e30 3634  65,2.94535 6.064
-00004a20: 3937 3635 2c32 2e38 3136 3234 2043 2035  9765,2.81624 C 5
-00004a30: 2e33 3233 3732 3636 2c32 2e37 3031 3432  .3237266,2.70142
-00004a40: 2034 2e35 3330 3436 3636 2c32 2e38 3735   4.5304666,2.875
-00004a50: 3731 2033 2e39 3335 3639 3636 2c33 2e33  71 3.9356966,3.3
-00004a60: 3433 3834 2043 2033 2e32 3133 3635 3635  4384 C 3.2136565
-00004a70: 2c33 2e39 3035 3139 2032 2e37 3635 3433  ,3.90519 2.76543
-00004a80: 3635 2c34 2e37 3536 3235 2032 2e35 3433  65,4.75625 2.543
-00004a90: 3833 3635 2c35 2e36 3332 3839 2043 2032  8365,5.63289 C 2
-00004aa0: 2e33 3035 3337 3635 2c36 2e35 3939 3935  .3053765,6.59995
-00004ab0: 2032 2e32 3935 3937 3635 2c37 2e36 3133   2.2959765,7.613
-00004ac0: 3538 2032 2e34 3239 3231 3635 2c38 2e35  58 2.4292165,8.5
-00004ad0: 3937 3320 4320 322e 3634 3634 3436 352c  973 C 2.6464465,
-00004ae0: 3130 2e31 3535 3837 2033 2e32 3638 3936  10.15587 3.26896
-00004af0: 3635 2c31 312e 3633 3235 3820 342e 3038  65,11.63258 4.08
-00004b00: 3135 3436 362c 3132 2e39 3639 3038 2043  15466,12.96908 C
-00004b10: 2033 2e32 3932 3434 3635 2c31 322e 3936   3.2924465,12.96
-00004b20: 3930 3820 322e 3530 3333 3436 352c 3132  908 2.5033465,12
-00004b30: 2e39 3639 3038 2031 2e37 3134 3234 3635  .96908 1.7142465
-00004b40: 2c31 322e 3936 3930 3820 4320 302e 3839  ,12.96908 C 0.89
-00004b50: 3732 3436 3531 2c31 312e 3438 3438 3120  724651,11.48481 
-00004b60: 302e 3235 3739 3936 3531 2c39 2e38 3732  0.25799651,9.872
-00004b70: 3939 2030 2e30 3630 3235 3635 3134 2c38  99 0.060256514,8
-00004b80: 2e31 3738 3939 2043 202d 302e 3037 3132  .17899 C -0.0712
-00004b90: 3033 3438 362c 372e 3030 3639 3520 302e  03486,7.00695 0.
-00004ba0: 3030 3337 3136 3531 3338 2c35 2e37 3939  0037165138,5.799
-00004bb0: 3033 2030 2e33 3731 3439 3635 312c 342e  03 0.37149651,4.
-00004bc0: 3637 3432 3120 4320 302e 3736 3434 3236  67421 C 0.764426
-00004bd0: 3531 2c33 2e34 3734 3939 2031 2e35 3139  51,3.47499 1.519
-00004be0: 3538 3635 2c32 2e33 3933 3220 322e 3532  5865,2.3932 2.52
-00004bf0: 3332 3536 352c 312e 3633 3034 2043 2033  32565,1.6304 C 3
-00004c00: 2e32 3830 3936 3635 2c31 2e30 3534 3738  .2809665,1.05478
-00004c10: 2034 2e32 3035 3933 3636 2c30 2e37 3132   4.2059366,0.712
-00004c20: 3638 2035 2e31 3531 3934 3636 2c30 2e36  68 5.1519466,0.6
-00004c30: 3337 3831 2043 2036 2e31 3933 3832 3635  3781 C 6.1938265
-00004c40: 2c30 2e35 3434 3936 2037 2e32 3631 3034  ,0.54496 7.26104
-00004c50: 3635 2c30 2e37 3436 3139 2038 2e31 3930  65,0.74619 8.190
-00004c60: 3932 3635 2c31 2e32 3239 3736 2043 2039  9265,1.22976 C 9
-00004c70: 2e33 3939 3836 3635 2c31 2e38 3530 3231  .3998665,1.85021
-00004c80: 2031 302e 3336 3336 3737 2c32 2e38 3539   10.363677,2.859
-00004c90: 3434 2031 312e 3134 3532 3737 2c33 2e39  44 11.145277,3.9
-00004ca0: 3537 3636 2043 2031 322e 3139 3033 3437  5766 C 12.190347
-00004cb0: 2c35 2e34 3431 3437 2031 322e 3936 3530  ,5.44147 12.9650
-00004cc0: 3637 2c37 2e31 3031 3031 2031 332e 3538  67,7.10101 13.58
-00004cd0: 3432 3837 2c38 2e38 3033 3832 2043 2031  4287,8.80382 C 1
-00004ce0: 342e 3633 3037 3636 2c31 312e 3731 3736  4.630766,11.7176
-00004cf0: 2031 352e 3231 3236 3236 2c31 342e 3737   15.212626,14.77
-00004d00: 3836 3120 3135 2e35 3735 3134 362c 3137  861 15.575146,17
-00004d10: 2e38 3437 3935 2043 2031 352e 3636 3438  .84795 C 15.6648
-00004d20: 3336 2c31 382e 3631 3634 3820 3135 2e37  36,18.61648 15.7
-00004d30: 3339 3535 362c 3139 2e33 3836 3735 2031  39556,19.38675 1
-00004d40: 352e 3830 3134 3436 2c32 302e 3135 3830  5.801446,20.1580
-00004d50: 3320 4320 3135 2e39 3333 3630 362c 3230  3 C 15.933606,20
-00004d60: 2e31 3538 3033 2031 362e 3036 3537 3736  .15803 16.065776
-00004d70: 2c32 302e 3135 3830 3320 3136 2e31 3937  ,20.15803 16.197
-00004d80: 3933 362c 3230 2e31 3538 3033 2043 2031  936,20.15803 C 1
-00004d90: 362e 3433 3135 3136 2c31 362e 3738 3333  6.431516,16.7833
-00004da0: 3220 3136 2e39 3139 3036 362c 3133 2e34  2 16.919066,13.4
-00004db0: 3037 3631 2031 372e 3932 3032 3336 2c31  0761 17.920236,1
-00004dc0: 302e 3137 3032 3920 4320 3138 2e35 3336  0.17029 C 18.536
-00004dd0: 3734 362c 382e 3139 3838 3620 3139 2e33  746,8.19886 19.3
-00004de0: 3433 3231 362c 362e 3237 3333 2032 302e  43216,6.2733 20.
-00004df0: 3436 3031 3036 2c34 2e35 3332 3039 2043  460106,4.53209 C
-00004e00: 2032 312e 3233 3239 3636 2c33 2e33 3432   21.232966,3.342
-00004e10: 3436 2032 322e 3137 3833 3936 2c32 2e32  46 22.178396,2.2
-00004e20: 3236 3931 2032 332e 3339 3332 3336 2c31  2691 23.393236,1
-00004e30: 2e34 3734 3733 2043 2032 342e 3330 3339  .47473 C 24.3039
-00004e40: 3436 2c30 2e39 3036 2032 352e 3337 3534  46,0.906 25.3754
-00004e50: 3036 2c30 2e35 3933 3135 2032 362e 3434  06,0.59315 26.44
-00004e60: 3938 3336 2c30 2e36 3137 3434 2043 2032  9836,0.61744 C 2
-00004e70: 372e 3430 3630 3736 2c30 2e36 3236 3520  7.406076,0.6265 
-00004e80: 3238 2e33 3636 3333 362c 302e 3838 3431  28.366336,0.8841
-00004e90: 3420 3239 2e31 3733 3338 362c 312e 3430  4 29.173386,1.40
-00004ea0: 3537 3120 4320 3239 2e39 3138 3237 362c  571 C 29.918276,
-00004eb0: 312e 3838 3431 3720 3330 2e35 3336 3732  1.88417 30.53672
-00004ec0: 362c 322e 3534 3832 3520 3331 2e30 3037  6,2.54825 31.007
-00004ed0: 3330 362c 332e 3239 3638 3820 4320 3331  306,3.29688 C 31
-00004ee0: 2e36 3430 3337 362c 342e 3330 3938 3120  .640376,4.30981 
-00004ef0: 3331 2e39 3432 3738 362c 352e 3530 3336  31.942786,5.5036
-00004f00: 2033 312e 3939 3035 3236 2c36 2e36 3931   31.990526,6.691
-00004f10: 3439 2043 2033 322e 3036 3433 3636 2c38  49 C 32.064366,8
-00004f20: 2e32 3438 3938 2033 312e 3730 3033 3036  .24898 31.700306
-00004f30: 2c39 2e37 3938 3431 2033 312e 3131 3831  ,9.79841 31.1181
-00004f40: 3336 2c31 312e 3233 3430 3920 4320 3330  36,11.23409 C 30
-00004f50: 2e38 3738 3035 362c 3131 2e38 3237 3734  .878056,11.82774
-00004f60: 2033 302e 3630 3037 3436 2c31 322e 3430   30.600746,12.40
-00004f70: 3538 3420 3330 2e32 3936 3739 362c 3132  584 30.296796,12
-00004f80: 2e39 3639 3038 2043 2032 392e 3530 3338  .96908 C 29.5038
-00004f90: 3036 2c31 322e 3936 3930 3820 3238 2e37  06,12.96908 28.7
-00004fa0: 3130 3832 362c 3132 2e39 3639 3038 2032  10826,12.96908 2
-00004fb0: 372e 3931 3738 3336 2c31 322e 3936 3930  7.917836,12.9690
-00004fc0: 3820 4320 3238 2e36 3935 3634 362c 3131  8 C 28.695646,11
-00004fd0: 2e35 3638 3235 2032 392e 3333 3039 3036  .56825 29.330906
-00004fe0: 2c31 302e 3036 3034 3420 3239 2e35 3635  ,10.06044 29.565
-00004ff0: 3735 362c 382e 3436 3438 3520 4320 3239  756,8.46485 C 29
-00005000: 2e37 3035 3433 362c 372e 3439 3035 3320  .705436,7.49053 
-00005010: 3239 2e36 3839 3937 362c 362e 3438 3733  29.689976,6.4873
-00005020: 3920 3239 2e34 3639 3733 362c 352e 3532  9 29.469736,5.52
-00005030: 3631 3620 4320 3239 2e32 3636 3538 362c  616 C 29.266586,
-00005040: 342e 3637 3239 3620 3238 2e38 3730 3935  4.67296 28.87095
-00005050: 362c 332e 3833 3335 3420 3238 2e32 3031  6,3.83354 28.201
-00005060: 3237 362c 332e 3235 3037 3920 4320 3237  276,3.25079 C 27
-00005070: 2e37 3138 3338 362c 322e 3832 3236 3320  .718386,2.82263 
-00005080: 3237 2e30 3738 3436 362c 322e 3539 3032  27.078466,2.5902
-00005090: 3120 3236 2e34 3336 3231 362c 322e 3538  1 26.436216,2.58
-000050a0: 3434 3620 4320 3235 2e36 3830 3330 362c  446 C 25.680306,
-000050b0: 322e 3536 3035 3920 3234 2e39 3530 3038  2.56059 24.95008
-000050c0: 362c 322e 3837 3330 3320 3234 2e33 3538  6,2.87303 24.358
-000050d0: 3333 362c 332e 3332 3837 3920 4320 3233  336,3.32879 C 23
-000050e0: 2e34 3934 3535 362c 332e 3939 3330 3720  .494556,3.99307 
-000050f0: 3232 2e38 3434 3938 362c 342e 3839 3139  22.844986,4.8919
-00005100: 3820 3232 2e32 3832 3935 362c 352e 3831  8 22.282956,5.81
-00005110: 3637 3920 4320 3231 2e34 3531 3735 362c  679 C 21.451756,
-00005120: 372e 3231 3037 3220 3230 2e38 3131 3433  7.21072 20.81143
-00005130: 362c 382e 3731 3031 3820 3230 2e32 3530  6,8.71018 20.250
-00005140: 3339 362c 3130 2e32 3331 3234 2043 2031  396,10.23124 C 1
-00005150: 392e 3433 3735 3836 2c31 322e 3439 3830  9.437586,12.4980
-00005160: 3220 3138 2e38 3933 3332 362c 3134 2e38  2 18.893326,14.8
-00005170: 3531 3636 2031 382e 3434 3032 3836 2c31  5166 18.440286,1
-00005180: 372e 3231 3433 3220 4320 3137 2e38 3339  7.21432 C 17.839
-00005190: 3031 362c 3230 2e34 3033 3235 2031 372e  016,20.40325 17.
-000051a0: 3431 3332 3136 2c32 332e 3632 3931 2031  413216,23.6291 1
-000051b0: 372e 3234 3631 3336 2c32 362e 3837 3135  7.246136,26.8715
-000051c0: 2043 2031 372e 3138 3337 3936 2c32 382e   C 17.183796,28.
-000051d0: 3031 3835 3720 3137 2e31 3733 3936 362c  01857 17.173966,
-000051e0: 3239 2e31 3637 3435 2031 372e 3137 3735  29.16745 17.1775
-000051f0: 3136 2c33 302e 3331 3539 3520 4320 3137  16,30.31595 C 17
-00005200: 2e31 3737 3531 362c 3330 2e35 3433 3937  .177516,30.54397
-00005210: 2031 372e 3137 3735 3136 2c33 302e 3737   17.177516,30.77
-00005220: 3139 3820 3137 2e31 3737 3531 362c 3331  198 17.177516,31
-00005230: 2043 2031 362e 3339 3631 3836 2c33 3120   C 16.396186,31 
-00005240: 3135 2e36 3134 3835 362c 3331 2031 342e  15.614856,31 14.
-00005250: 3833 3335 3336 2c33 3120 7a22 0a20 2020  833536,31 z".   
-00005260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005270: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00005280: 3a20 247a 6f64 6961 635f 636f 6c6f 725f  : $zodiac_color_
-00005290: 3022 0a20 2020 2020 2020 2020 2020 2020  0".             
-000052a0: 2020 2020 2020 202f 3e0a 2020 2020 2020         />.      
-000052b0: 2020 2020 2020 2020 2020 3c2f 7379 6d62            </symb
-000052c0: 6f6c 3e0a 2020 2020 2020 2020 2020 2020  ol>.            
-000052d0: 2020 2020 3c73 796d 626f 6c20 6964 3d22      <symbol id="
-000052e0: 7461 7572 7573 223e 0a20 2020 2020 2020  taurus">.       
-000052f0: 2020 2020 2020 2020 2020 2020 203c 7061               <pa
-00005300: 7468 0a20 2020 2020 2020 2020 2020 2020  th.             
-00005310: 2020 2020 2020 2020 2020 2064 3d22 4d20             d="M 
-00005320: 3131 2e32 3131 3132 352c 3131 2e39 3630  11.211125,11.960
-00005330: 3034 3320 4320 392e 3938 3536 3139 372c  043 C 9.9856197,
-00005340: 3131 2e34 3832 3038 3520 382e 3832 3733  11.482085 8.8273
-00005350: 3530 372c 3130 2e37 3537 3236 3320 372e  507,10.757263 7.
-00005360: 3939 3934 3136 342c 392e 3732 3236 3620  9994164,9.72266 
-00005370: 4320 362e 3935 3430 3538 342c 382e 3434  C 6.9540584,8.44
-00005380: 3839 3530 3820 362e 3231 3139 3532 342c  89508 6.2119524,
-00005390: 362e 3936 3936 3039 3720 352e 3430 3638  6.9696097 5.4068
-000053a0: 3139 392c 352e 3534 3232 3531 3520 4320  199,5.5422515 C 
-000053b0: 342e 3931 3533 3333 362c 342e 3634 3335  4.9153336,4.6435
-000053c0: 3933 3120 342e 3335 3838 3435 322c 332e  931 4.3588452,3.
-000053d0: 3736 3034 3132 3820 332e 3630 3032 3638  7604128 3.600268
-000053e0: 362c 332e 3036 3031 3033 3620 4320 332e  6,3.0601036 C 3.
-000053f0: 3038 3737 3337 312c 322e 3538 3330 3339  0877371,2.583039
-00005400: 3920 322e 3436 3939 3433 332c 322e 3139  9 2.4699433,2.19
-00005410: 3737 3132 3920 312e 3737 3931 3332 312c  77129 1.7791321,
-00005420: 322e 3034 3632 3137 3820 4320 312e 3435  2.0462178 C 1.45
-00005430: 3134 3836 372c 312e 3936 3633 3435 3120  14867,1.9663451 
-00005440: 312e 3131 3237 3639 382c 312e 3936 3334  1.1127698,1.9634
-00005450: 3036 3520 302e 3737 3735 3636 3438 2c31  065 0.77756648,1
-00005460: 2e39 3639 3332 3033 2043 2030 2e36 3737  .9693203 C 0.677
-00005470: 3530 3133 382c 312e 3938 3234 3830 3320  50138,1.9824803 
-00005480: 302e 3539 3833 3335 3038 2c31 2e39 3734  0.59833508,1.974
-00005490: 3735 3935 2030 2e36 3333 3639 3038 382c  7595 0.63369088,
-000054a0: 312e 3835 3238 3333 3320 4320 302e 3633  1.8528333 C 0.63
-000054b0: 3336 3930 3838 2c31 2e32 3730 3336 3138  369088,1.2703618
-000054c0: 2030 2e36 3333 3639 3038 382c 302e 3638   0.63369088,0.68
-000054d0: 3738 3930 3233 2030 2e36 3333 3639 3038  789023 0.6336908
-000054e0: 382c 302e 3130 3534 3030 3434 2043 2031  8,0.10540044 C 1
-000054f0: 2e31 3736 3933 2c30 2e31 3131 3738 3838  .17693,0.1117888
-00005500: 3420 312e 3732 3130 3239 322c 302e 3039  4 1.7210292,0.09
-00005510: 3031 3539 3634 3120 322e 3236 3336 3039  0159641 2.263609
-00005520: 352c 302e 3132 3136 3939 3834 2043 2033  5,0.12169984 C 3
-00005530: 2e33 3439 3337 3339 2c30 2e32 3132 3038  .3493739,0.21208
-00005540: 3539 3420 342e 3336 3635 3132 392c 302e  594 4.3665129,0.
-00005550: 3731 3538 3731 3231 2035 2e31 3931 3739  71587121 5.19179
-00005560: 3335 2c31 2e34 3039 3735 3535 2043 2036  35,1.4097555 C 6
-00005570: 2e32 3634 3738 3434 2c32 2e33 3031 3333  .2647844,2.30133
-00005580: 3220 372e 3038 3838 3735 342c 332e 3434  2 7.0888754,3.44
-00005590: 3934 3832 3720 372e 3739 3131 3631 342c  94827 7.7911614,
-000055a0: 342e 3634 3336 3437 3920 4320 382e 3239  4.6436479 C 8.29
-000055b0: 3133 3033 342c 352e 3530 3436 3838 2038  13034,5.504688 8
-000055c0: 2e37 3732 3137 3537 2c36 2e33 3736 3735  .7721757,6.37675
-000055d0: 3235 2039 2e32 3734 3331 3237 2c37 2e32  25 9.2743127,7.2
-000055e0: 3336 3630 3632 2043 2039 2e37 3538 3830  366062 C 9.75880
-000055f0: 3837 2c38 2e30 3436 3335 3639 2031 302e  87,8.0463569 10.
-00005600: 3330 3736 3438 2c38 2e38 3234 3738 3635  307648,8.8247865
-00005610: 2031 302e 3937 3135 3339 2c39 2e34 3938   10.971539,9.498
-00005620: 3939 3438 2043 2031 312e 3535 3837 3137  9948 C 11.558717
-00005630: 2c31 302e 3039 3436 3939 2031 322e 3236  ,10.094699 12.26
-00005640: 3135 372c 3130 2e35 3836 3936 3720 3133  157,10.586967 13
-00005650: 2e30 3532 3934 2c31 302e 3837 3131 3339  .05294,10.871139
-00005660: 2043 2031 342e 3135 3039 3636 2c31 312e   C 14.150966,11.
-00005670: 3237 3633 3632 2031 352e 3333 3930 3436  276362 15.339046
-00005680: 2c31 312e 3335 3935 3536 2031 362e 3530  ,11.359556 16.50
-00005690: 3032 3434 2c31 312e 3331 3436 3337 2043  0244,11.314637 C
-000056a0: 2031 372e 3534 3332 3034 2c31 312e 3236   17.543204,11.26
-000056b0: 3236 3732 2031 382e 3630 3230 3638 2c31  2672 18.602068,1
-000056c0: 312e 3036 3936 3136 2031 392e 3532 3937  1.069616 19.5297
-000056d0: 3932 2c31 302e 3537 3137 3435 2043 2032  92,10.571745 C 2
-000056e0: 302e 3430 3133 3335 2c31 302e 3131 3436  0.401335,10.1146
-000056f0: 3637 2032 312e 3130 3338 3034 2c39 2e33  67 21.103804,9.3
-00005700: 3937 3039 3134 2032 312e 3730 3030 342c  970914 21.70004,
-00005710: 382e 3632 3637 3635 3920 4320 3232 2e33  8.6267659 C 22.3
-00005720: 3835 3038 372c 372e 3734 3131 3934 3620  85087,7.7411946 
-00005730: 3232 2e39 3036 3937 2c36 2e37 3437 3733  22.90697,6.74773
-00005740: 3331 2032 332e 3437 3237 2c35 2e37 3835  31 23.4727,5.785
-00005750: 3930 3331 2043 2032 332e 3937 3332 3939  9031 C 23.973299
-00005760: 2c34 2e39 3332 3134 3538 2032 342e 3434  ,4.9321458 24.44
-00005770: 3535 3136 2c34 2e30 3538 3630 3238 2032  5516,4.0586028 2
-00005780: 352e 3033 3232 3931 2c33 2e32 3538 3930  5.032291,3.25890
-00005790: 3931 2043 2032 352e 3731 3138 3636 2c32  91 C 25.711866,2
-000057a0: 2e33 3234 3738 3633 2032 362e 3531 3636  .3247863 26.5166
-000057b0: 3332 2c31 2e34 3535 3832 3437 2032 372e  32,1.4558247 27.
-000057c0: 3530 3737 3636 2c30 2e38 3435 3939 3237  507766,0.8459927
-000057d0: 3720 4320 3238 2e32 3636 3437 312c 302e  7 C 28.266471,0.
-000057e0: 3338 3332 3338 3934 2032 392e 3134 3633  38323894 29.1463
-000057f0: 3737 2c30 2e30 3936 3534 3830 3431 2033  77,0.096548041 3
-00005800: 302e 3034 3038 3332 2c30 2e31 3036 3635  0.040832,0.10665
-00005810: 3938 3420 4320 3330 2e34 3530 3432 362c  984 C 30.450426,
-00005820: 302e 3130 3230 3630 3234 2033 302e 3836  0.10206024 30.86
-00005830: 3030 3734 2c30 2e31 3037 3933 3735 3420  0074,0.10793754 
-00005840: 3331 2e32 3639 3636 372c 302e 3130 3534  31.269667,0.1054
-00005850: 3030 3434 2043 2033 312e 3236 3936 3637  0044 C 31.269667
-00005860: 2c30 2e37 3236 3731 3331 3520 3331 2e32  ,0.72671315 31.2
-00005870: 3639 3636 372c 312e 3334 3830 3235 3820  69667,1.3480258 
-00005880: 3331 2e32 3639 3636 372c 312e 3936 3933  31.269667,1.9693
-00005890: 3230 3320 4320 3330 2e38 3336 3534 2c31  203 C 30.83654,1
-000058a0: 2e39 3636 3130 3738 2033 302e 3339 3533  .9661078 30.3953
-000058b0: 3631 2c31 2e39 3538 3336 3838 2032 392e  61,1.9583688 29.
-000058c0: 3937 3630 3638 2c32 2e30 3834 3035 3520  976068,2.084055 
-000058d0: 4320 3239 2e31 3139 3933 342c 322e 3331  C 29.119934,2.31
-000058e0: 3836 3731 3820 3238 2e34 3030 3438 332c  86718 28.400483,
-000058f0: 322e 3839 3235 3634 3620 3237 2e38 3236  2.8925646 27.826
-00005900: 3933 392c 332e 3535 3137 3639 3320 4320  939,3.5517693 C 
-00005910: 3237 2e32 3336 3032 382c 342e 3232 3335  27.236028,4.2235
-00005920: 3836 3520 3236 2e37 3838 3236 312c 352e  865 26.788261,5.
-00005930: 3030 3238 3337 3420 3236 2e33 3631 3636  0028374 26.36166
-00005940: 362c 352e 3738 3433 3639 3920 4320 3235  6,5.7843699 C 25
-00005950: 2e36 3233 3131 2c37 2e31 3031 3038 3139  .62311,7.1010819
-00005960: 2032 342e 3932 3631 3638 2c38 2e34 3534   24.926168,8.454
-00005970: 3339 2032 332e 3937 3439 3436 2c39 2e36  39 23.974946,9.6
-00005980: 3335 3732 3337 2043 2032 332e 3539 3335  357237 C 23.5935
-00005990: 3534 2c31 302e 3131 3532 3838 2032 332e  54,10.115288 23.
-000059a0: 3135 3231 3138 2c31 302e 3534 3738 3136  152118,10.547816
-000059b0: 2032 322e 3635 3235 3036 2c31 302e 3930   22.652506,10.90
-000059c0: 3433 3431 2043 2032 322e 3034 3938 312c  4341 C 22.04981,
-000059d0: 3131 2e33 3431 3236 3720 3231 2e33 3833  11.341267 21.383
-000059e0: 3337 352c 3131 2e36 3835 3332 3620 3230  375,11.685326 20
-000059f0: 2e36 3932 3231 362c 3131 2e39 3630 3034  .692216,11.96004
-00005a00: 3320 4320 3232 2e33 3438 3938 312c 3132  3 C 22.348981,12
-00005a10: 2e38 3635 3235 3420 3233 2e38 3238 3330  .865254 23.82830
-00005a20: 382c 3134 2e31 3232 3634 3620 3234 2e38  8,14.122646 24.8
-00005a30: 3936 3333 392c 3135 2e36 3834 3033 3120  96339,15.684031 
-00005a40: 4320 3235 2e37 3936 3530 342c 3136 2e39  C 25.796504,16.9
-00005a50: 3836 3038 3720 3236 2e33 3934 3331 342c  86087 26.394314,
-00005a60: 3138 2e34 3939 3135 3820 3236 2e35 3932  18.499158 26.592
-00005a70: 3934 332c 3230 2e30 3730 3039 2043 2032  943,20.07009 C 2
-00005a80: 362e 3738 3636 3332 2c32 312e 3535 3231  6.786632,21.5521
-00005a90: 3531 2032 362e 3637 3934 3438 2c32 332e  51 26.679448,23.
-00005aa0: 3037 3737 3820 3236 2e32 3436 3339 342c  07778 26.246394,
-00005ab0: 3234 2e35 3130 3139 3420 4320 3235 2e37  24.510194 C 25.7
-00005ac0: 3934 3132 352c 3235 2e39 3931 3033 3220  94125,25.991032 
-00005ad0: 3234 2e39 3736 3338 342c 3237 2e33 3439  24.976384,27.349
-00005ae0: 3530 3520 3233 2e39 3235 3937 352c 3238  505 23.925975,28
-00005af0: 2e34 3835 3030 3720 4320 3232 2e36 3635  .485007 C 22.665
-00005b00: 3634 362c 3239 2e38 3636 3135 2032 312e  646,29.86615 21.
-00005b10: 3038 3539 3938 2c33 302e 3938 3437 3332  085998,30.984732
-00005b20: 2031 392e 3330 3132 3432 2c33 312e 3537   19.301242,31.57
-00005b30: 3639 3332 2043 2031 372e 3535 3232 3038  6932 C 17.552208
-00005b40: 2c33 322e 3135 3734 3134 2031 352e 3635  ,32.157414 15.65
-00005b50: 3238 3032 2c33 322e 3234 3636 3134 2031  2802,32.246614 1
-00005b60: 332e 3834 3630 3836 2c33 312e 3930 3237  3.846086,31.9027
-00005b70: 3536 2043 2031 322e 3232 3031 3933 2c33  56 C 12.220193,3
-00005b80: 312e 3538 3434 3839 2031 302e 3638 3537  1.584489 10.6857
-00005b90: 3635 2c33 302e 3834 3538 3520 392e 3430  65,30.84585 9.40
-00005ba0: 3038 3736 372c 3239 2e38 3035 3632 3520  08767,29.805625 
-00005bb0: 4320 382e 3330 3031 3432 342c 3238 2e39  C 8.3001424,28.9
-00005bc0: 3233 3330 3320 372e 3333 3534 3639 342c  23303 7.3354694,
-00005bd0: 3237 2e38 3631 3831 3520 362e 3630 3637  27.861815 6.6067
-00005be0: 3737 342c 3236 2e36 3532 3935 3620 4320  774,26.652956 C 
-00005bf0: 352e 3834 3135 3032 372c 3235 2e33 3735  5.8415027,25.375
-00005c00: 3233 3120 352e 3337 3036 3538 392c 3233  231 5.3706589,23
-00005c10: 2e39 3233 3431 3520 352e 3234 3738 3436  .923415 5.247846
-00005c20: 382c 3232 2e34 3339 3731 3220 4320 352e  8,22.439712 C 5.
-00005c30: 3038 3233 3538 382c 3230 2e35 3936 3620  0823588,20.5966 
-00005c40: 352e 3339 3339 3931 352c 3138 2e37 3031  5.3939915,18.701
-00005c50: 3435 2036 2e32 3136 3237 3034 2c31 372e  45 6.2162704,17.
-00005c60: 3033 3732 3132 2043 2037 2e31 3136 3633  037212 C 7.11663
-00005c70: 3634 2c31 352e 3139 3133 3632 2038 2e35  64,15.191362 8.5
-00005c80: 3634 3332 3234 2c31 332e 3633 3439 3935  643224,13.634995
-00005c90: 2031 302e 3238 3335 3436 2c31 322e 3531   10.283546,12.51
-00005ca0: 3735 3633 2043 2031 302e 3538 3532 3937  7563 C 10.585297
-00005cb0: 2c31 322e 3331 3937 3434 2031 302e 3839  ,12.319744 10.89
-00005cc0: 3530 3038 2c31 322e 3133 3430 3632 2031  5008,12.134062 1
-00005cd0: 312e 3231 3131 3235 2c31 312e 3936 3030  1.211125,11.9600
-00005ce0: 3433 207a 204d 2031 352e 3935 3739 322c  43 z M 15.95792,
-00005cf0: 3239 2e36 3035 3330 3520 4320 3137 2e34  29.605305 C 17.4
-00005d00: 3639 3637 342c 3239 2e36 3133 3933 3820  69674,29.613938 
-00005d10: 3138 2e39 3935 3730 332c 3239 2e32 3238  18.995703,29.228
-00005d20: 3036 3420 3230 2e32 3737 3937 342c 3238  064 20.277974,28
-00005d30: 2e34 3138 3133 2043 2032 312e 3238 3234  .41813 C 21.2824
-00005d40: 3331 2c32 372e 3738 3934 3632 2032 322e  31,27.789462 22.
-00005d50: 3135 3336 3237 2c32 362e 3935 3235 3333  153627,26.952533
-00005d60: 2032 322e 3833 3739 3432 2c32 352e 3938   22.837942,25.98
-00005d70: 3737 3635 2043 2032 332e 3539 3634 3038  7765 C 23.596408
-00005d80: 2c32 342e 3930 3135 3236 2032 342e 3035  ,24.901526 24.05
-00005d90: 3635 3833 2c32 332e 3631 3237 3935 2032  6583,23.612795 2
-00005da0: 342e 3136 3031 3434 2c32 322e 3239 3332  4.160144,22.2932
-00005db0: 3138 2043 2032 342e 3239 3937 3535 2c32  18 C 24.299755,2
-00005dc0: 302e 3639 3333 3031 2032 342e 3030 3932  0.693301 24.0092
-00005dd0: 3232 2c31 392e 3033 3638 3032 2032 332e  22,19.036802 23.
-00005de0: 3231 3332 3034 2c31 372e 3633 3037 3831  213204,17.630781
-00005df0: 2043 2032 322e 3633 3532 3836 2c31 362e   C 22.635286,16.
-00005e00: 3539 3739 3320 3231 2e38 3233 3731 322c  59793 21.823712,
-00005e10: 3135 2e37 3031 3935 3520 3230 2e38 3832  15.701955 20.882
-00005e20: 3335 342c 3134 2e39 3836 3232 3320 4320  354,14.986223 C 
-00005e30: 3139 2e39 3537 3836 392c 3134 2e32 3835  19.957869,14.285
-00005e40: 3731 3320 3138 2e38 3734 3333 372c 3133  713 18.874337,13
-00005e50: 2e37 3936 3536 3620 3137 2e37 3334 3830  .796566 17.73480
-00005e60: 372c 3133 2e35 3732 3931 3920 4320 3136  7,13.572919 C 16
-00005e70: 2e35 3630 3537 392c 3133 2e33 3339 3330  .560579,13.33930
-00005e80: 3620 3135 2e33 3339 3535 392c 3133 2e33  6 15.339559,13.3
-00005e90: 3435 3534 3820 3134 2e31 3635 3434 312c  45548 14.165441,
-00005ea0: 3133 2e35 3736 3037 3720 4320 3132 2e38  13.576077 C 12.8
-00005eb0: 3832 3031 372c 3133 2e38 3336 3438 3420  82017,13.836484 
-00005ec0: 3131 2e36 3730 3834 322c 3134 2e34 3238  11.670842,14.428
-00005ed0: 3030 3920 3130 2e36 3731 3233 342c 3135  009 10.671234,15
-00005ee0: 2e32 3731 3138 2043 2039 2e34 3337 3437  .27118 C 9.43747
-00005ef0: 3637 2c31 362e 3239 3439 3034 2038 2e34  67,16.294904 8.4
-00005f00: 3639 3038 3834 2c31 372e 3636 3339 3634  690884,17.663964
-00005f10: 2038 2e30 3239 3335 3534 2c31 392e 3231   8.0293554,19.21
-00005f20: 3137 3838 2043 2037 2e36 3533 3135 3934  1788 C 7.6531594
-00005f30: 2c32 302e 3532 3336 3633 2037 2e36 3133  ,20.523663 7.613
-00005f40: 3333 3834 2c32 312e 3932 3637 3832 2037  3384,21.926782 7
-00005f50: 2e38 3834 3233 3534 2c32 332e 3236 3235  .8842354,23.2625
-00005f60: 3439 2043 2038 2e31 3530 3934 3134 2c32  49 C 8.1509414,2
-00005f70: 342e 3533 3232 3631 2038 2e37 3631 3238  4.532261 8.76128
-00005f80: 3737 2c32 352e 3732 3337 3235 2039 2e36  77,25.723725 9.6
-00005f90: 3230 3834 3337 2c32 362e 3639 3538 3836  208437,26.695886
-00005fa0: 2043 2031 302e 3530 3232 3838 2c32 372e   C 10.502288,27.
-00005fb0: 3730 3630 3132 2031 312e 3539 3734 3034  706012 11.597404
-00005fc0: 2c32 382e 3535 3033 3838 2031 322e 3835  ,28.550388 12.85
-00005fd0: 3430 3733 2c32 392e 3033 3938 3038 2043  4073,29.039808 C
-00005fe0: 2031 332e 3833 3830 372c 3239 2e34 3333   13.83807,29.433
-00005ff0: 3138 3520 3134 2e39 3030 3333 372c 3239  185 14.900337,29
-00006000: 2e36 3036 3630 3120 3135 2e39 3537 3932  .606601 15.95792
-00006010: 2c32 392e 3630 3533 3035 207a 220a 2020  ,29.605305 z".  
-00006020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006030: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-00006040: 6c3a 2024 7a6f 6469 6163 5f63 6f6c 6f72  l: $zodiac_color
-00006050: 5f31 220a 2020 2020 2020 2020 2020 2020  _1".            
-00006060: 2020 2020 2020 2020 2f3e 0a20 2020 2020          />.     
-00006070: 2020 2020 2020 2020 2020 203c 2f73 796d             </sym
-00006080: 626f 6c3e 0a20 2020 2020 2020 2020 2020  bol>.           
-00006090: 2020 2020 203c 7379 6d62 6f6c 2069 643d       <symbol id=
-000060a0: 2267 656d 696e 6922 3e0a 2020 2020 2020  "gemini">.      
-000060b0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-000060c0: 6174 680a 2020 2020 2020 2020 2020 2020  ath.            
-000060d0: 2020 2020 2020 2020 2020 2020 643d 224d              d="M
-000060e0: 2030 2e35 3635 3439 3239 322c 3332 2043   0.56549292,32 C
-000060f0: 2030 2e35 3635 3439 3239 322c 3331 2e32   0.56549292,31.2
-00006100: 3134 3233 3820 302e 3536 3534 3932 3932  14238 0.56549292
-00006110: 2c33 302e 3432 3834 3635 2030 2e35 3635  ,30.428465 0.565
-00006120: 3439 3239 322c 3239 2e36 3432 3730 3320  49292,29.642703 
-00006130: 4320 322e 3936 3735 3131 392c 3239 2e30  C 2.9675119,29.0
-00006140: 3131 3131 3620 352e 3430 3233 3537 332c  11116 5.4023573,
-00006150: 3238 2e34 3836 3135 3520 372e 3836 3937  28.486155 7.8697
-00006160: 3730 342c 3238 2e31 3838 3739 3220 4320  704,28.188792 C 
-00006170: 372e 3836 3937 3730 342c 3230 2e30 3438  7.8697704,20.048
-00006180: 3831 3720 372e 3836 3937 3730 342c 3131  817 7.8697704,11
-00006190: 2e39 3038 3833 3220 372e 3836 3937 3730  .908832 7.869770
-000061a0: 342c 332e 3736 3838 3537 3120 4320 352e  4,3.7688571 C 5.
-000061b0: 3339 3736 3134 362c 332e 3533 3839 3537  3976146,3.538957
-000061c0: 3120 322e 3935 3030 3632 392c 332e 3036  1 2.9500629,3.06
-000061d0: 3136 3339 3120 302e 3536 3534 3932 3932  16391 0.56549292
-000061e0: 2c32 2e33 3731 3431 3038 2043 2030 2e35  ,2.3714108 C 0.5
-000061f0: 3635 3439 3239 322c 312e 3538 3039 3432  6549292,1.580942
-00006200: 3320 302e 3536 3534 3932 3932 2c30 2e37  3 0.56549292,0.7
-00006210: 3930 3437 3339 2030 2e35 3635 3439 3239  904739 0.5654929
-00006220: 322c 2d35 652d 3036 2043 2034 2e31 3330  2,-5e-06 C 4.130
-00006230: 3034 3539 2c30 2e39 3830 3933 3036 2037  0459,0.9809306 7
-00006240: 2e38 3138 3430 3738 2c31 2e34 3336 3235  .8184078,1.43625
-00006250: 3220 3131 2e35 3032 3830 332c 312e 3634  2 11.502803,1.64
-00006260: 3238 3639 3520 4320 3134 2e36 3939 3431  28695 C 14.69941
-00006270: 2c31 2e38 3131 3535 3734 2031 372e 3930  ,1.8115574 17.90
-00006280: 3537 332c 312e 3830 3730 3438 3220 3231  573,1.8070482 21
-00006290: 2e31 3031 3631 312c 312e 3632 3430 3735  .101611,1.624075
-000062a0: 3820 4320 3234 2e36 3737 3233 342c 312e  8 C 24.677234,1.
-000062b0: 3430 3831 3931 2032 382e 3235 3437 3432  408191 28.254742
-000062c0: 2c30 2e39 3532 3536 3839 2033 312e 3731  ,0.9525689 31.71
-000062d0: 3434 3236 2c2d 3565 2d30 3620 4320 3331  4426,-5e-06 C 31
-000062e0: 2e37 3134 3432 362c 302e 3739 3034 3733  .714426,0.790473
-000062f0: 3920 3331 2e37 3134 3432 362c 312e 3538  9 31.714426,1.58
-00006300: 3039 3432 3320 3331 2e37 3134 3432 362c  09423 31.714426,
-00006310: 322e 3337 3134 3130 3820 4320 3239 2e33  2.3714108 C 29.3
-00006320: 3234 3530 322c 332e 3035 3933 3438 3120  24502,3.0593481 
-00006330: 3236 2e38 3732 3832 392c 332e 3533 3836  26.872829,3.5386
-00006340: 3637 3120 3234 2e33 3936 3034 352c 332e  671 24.396045,3.
-00006350: 3736 3838 3537 3120 4320 3234 2e33 3936  7688571 C 24.396
-00006360: 3034 352c 3131 2e39 3038 3833 3220 3234  045,11.908832 24
-00006370: 2e33 3936 3034 352c 3230 2e30 3438 3831  .396045,20.04881
-00006380: 3720 3234 2e33 3936 3034 352c 3238 2e31  7 24.396045,28.1
-00006390: 3838 3739 3220 4320 3236 2e38 3638 3033  88792 C 26.86803
-000063a0: 352c 3238 2e34 3836 3730 3420 3239 2e33  5,28.486704 29.3
-000063b0: 3037 3136 372c 3239 2e30 3133 3135 3820  07167,29.013158 
-000063c0: 3331 2e37 3134 3432 362c 3239 2e36 3432  31.714426,29.642
-000063d0: 3730 3320 4320 3331 2e37 3134 3432 362c  703 C 31.714426,
-000063e0: 3330 2e34 3238 3436 3520 3331 2e37 3134  30.428465 31.714
-000063f0: 3432 362c 3331 2e32 3134 3233 3820 3331  426,31.214238 31
-00006400: 2e37 3134 3432 362c 3332 2043 2032 362e  .714426,32 C 26.
-00006410: 3037 3137 372c 3330 2e35 3132 3836 3620  07177,30.512866 
-00006420: 3230 2e32 3036 3433 322c 3239 2e39 3933  20.206432,29.993
-00006430: 3932 3820 3134 2e33 3833 3237 312c 3330  928 14.383271,30
-00006440: 2e31 3239 3237 3820 4320 392e 3732 3831  .129278 C 9.7281
-00006450: 3533 362c 3330 2e32 3430 3139 3620 352e  536,30.240196 5.
-00006460: 3037 3231 3334 392c 3330 2e38 3038 3737  0721349,30.80877
-00006470: 3720 302e 3536 3534 3932 3932 2c33 3220  7 0.56549292,32 
-00006480: 7a20 4d20 3130 2e37 3034 3035 332c 3238  z M 10.704053,28
-00006490: 2e30 3139 3431 2043 2031 322e 3938 3434  .01941 C 12.9844
-000064a0: 3438 2c32 372e 3736 3533 3637 2031 352e  48,27.765367 15.
-000064b0: 3238 3332 3234 2c32 372e 3732 3237 3833  283224,27.722783
-000064c0: 2031 372e 3537 3535 3339 2c32 372e 3736   17.575539,27.76
-000064d0: 3638 3038 2043 2031 382e 3930 3638 3836  6808 C 18.906886
-000064e0: 2c32 372e 3739 3639 3132 2032 302e 3233  ,27.796912 20.23
-000064f0: 3831 342c 3237 2e38 3730 3036 3520 3231  814,27.870065 21
-00006500: 2e35 3631 3736 322c 3238 2e30 3139 3431  .561762,28.01941
-00006510: 2043 2032 312e 3536 3137 3632 2c32 302e   C 21.561762,20.
-00006520: 3030 3137 3636 2032 312e 3536 3137 3632  001766 21.561762
-00006530: 2c31 312e 3938 3431 3231 2032 312e 3536  ,11.984121 21.56
-00006540: 3137 3632 2c33 2e39 3636 3437 3731 2043  1762,3.9664771 C
-00006550: 2031 392e 3138 3933 3038 2c34 2e31 3231   19.189308,4.121
-00006560: 3037 3731 2031 362e 3831 3030 3831 2c34  0771 16.810081,4
-00006570: 2e31 3339 3331 3131 2031 342e 3433 3335  .1393111 14.4335
-00006580: 3135 2c34 2e31 3039 3336 3331 2043 2031  15,4.1093631 C 1
-00006590: 332e 3138 3935 3236 2c34 2e30 3930 3038  3.189526,4.09008
-000065a0: 3231 2031 312e 3934 3535 3035 2c34 2e30  21 11.945505,4.0
-000065b0: 3530 3230 3431 2031 302e 3730 3430 3533  502041 10.704053
-000065c0: 2c33 2e39 3636 3437 3731 2043 2031 302e  ,3.9664771 C 10.
-000065d0: 3730 3430 3533 2c31 312e 3938 3431 3231  704053,11.984121
-000065e0: 2031 302e 3730 3430 3533 2c32 302e 3030   10.704053,20.00
-000065f0: 3137 3636 2031 302e 3730 3430 3533 2c32  1766 10.704053,2
-00006600: 382e 3031 3934 3120 7a20 220a 2020 2020  8.01941 z ".    
-00006610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006620: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-00006630: 2024 7a6f 6469 6163 5f63 6f6c 6f72 5f32   $zodiac_color_2
-00006640: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00006650: 2020 2020 2020 2f3e 0a20 2020 2020 2020        />.       
-00006660: 2020 2020 2020 2020 203c 2f73 796d 626f           </symbo
-00006670: 6c3e 0a20 2020 2020 2020 2020 2020 2020  l>.             
-00006680: 2020 203c 7379 6d62 6f6c 2069 643d 2263     <symbol id="c
-00006690: 616e 6365 7222 3e0a 2020 2020 2020 2020  ancer">.        
-000066a0: 2020 2020 2020 2020 2020 2020 3c70 6174              <pat
-000066b0: 680a 2020 2020 2020 2020 2020 2020 2020  h.              
-000066c0: 2020 2020 2020 2020 2020 643d 224d 2030            d="M 0
-000066d0: 2c32 352e 3632 3934 3832 204c 2030 2c32  ,25.629482 L 0,2
-000066e0: 322e 3930 3831 3031 2043 2035 2e32 3437  2.908101 C 5.247
-000066f0: 3935 3039 2c32 352e 3330 3439 3134 2031  9509,25.304914 1
-00006700: 302e 3333 3334 3634 2c32 362e 3439 3038  0.333464,26.4908
-00006710: 3337 2031 352e 3233 3135 3531 2c32 362e  37 15.231551,26.
-00006720: 3439 3038 3337 2043 2031 382e 3434 3237  490837 C 18.4427
-00006730: 3937 2c32 362e 3439 3038 3337 2032 312e  97,26.490837 21.
-00006740: 3035 3432 3737 2c32 362e 3037 3838 3834  054277,26.078884
-00006750: 2032 332e 3036 3539 3932 2c32 352e 3234   23.065992,25.24
-00006760: 3234 3937 2043 2032 312e 3739 3134 3839  2497 C 21.791489
-00006770: 2c32 342e 3539 3333 3620 3230 2e38 3239  ,24.59336 20.829
-00006780: 3336 352c 3233 2e37 3639 3435 3520 3230  365,23.769455 20
-00006790: 2e31 3932 3131 342c 3232 2e37 3833 3236  .192114,22.78326
-000067a0: 3720 4320 3139 2e35 3534 3836 332c 3231  7 C 19.554863,21
-000067b0: 2e37 3937 3037 3820 3139 2e32 3239 3939  .797078 19.22999
-000067c0: 2c32 302e 3633 3631 3232 2031 392e 3232  ,20.636122 19.22
-000067d0: 3939 392c 3139 2e33 3030 3339 3820 4320  999,19.300398 C 
-000067e0: 3139 2e32 3239 3939 2c31 372e 3535 3237  19.22999,17.5527
-000067f0: 3232 2031 392e 3836 3732 3431 2c31 362e  22 19.867241,16.
-00006800: 3035 3437 3134 2032 312e 3132 3932 3438  054714 21.129248
-00006810: 2c31 342e 3739 3338 3931 2043 2032 322e  ,14.793891 C 22.
-00006820: 3337 3837 362c 3133 2e35 3435 3535 3120  37876,13.545551 
-00006830: 3233 2e39 3033 3136 352c 3132 2e39 3231  23.903165,12.921
-00006840: 3338 3120 3235 2e36 3532 3438 312c 3132  381 25.652481,12
-00006850: 2e39 3231 3338 3120 4320 3237 2e34 3031  .921381 C 27.401
-00006860: 3739 382c 3132 2e39 3231 3338 3120 3238  798,12.921381 28
-00006870: 2e38 3838 3731 382c 3133 2e35 3435 3535  .888718,13.54555
-00006880: 3120 3330 2e31 3338 3233 2c31 342e 3738  1 30.13823,14.78
-00006890: 3134 3037 2043 2033 312e 3337 3532 3436  1407 C 31.375246
-000068a0: 2c31 362e 3032 3937 3437 2033 322e 3030  ,16.029747 32.00
-000068b0: 3030 3032 2c31 372e 3531 3532 3732 2033  0002,17.515272 3
-000068c0: 322e 3030 3030 3032 2c31 392e 3237 3534  2.000002,19.2754
-000068d0: 3331 2043 2033 322e 3030 3030 3032 2c32  31 C 32.000002,2
-000068e0: 322e 3035 3932 3320 3330 2e33 3030 3636  2.05923 30.30066
-000068f0: 362c 3234 2e33 3831 3134 3220 3236 2e38  6,24.381142 26.8
-00006900: 3839 3439 382c 3236 2e32 3238 3638 3520  89498,26.228685 
-00006910: 4320 3233 2e34 3738 3333 312c 3238 2e30  C 23.478331,28.0
-00006920: 3736 3232 3820 3139 2e32 3035 2c32 3920  76228 19.205,29 
-00006930: 3134 2e30 3639 3530 352c 3239 2043 2039  14.069505,29 C 9
-00006940: 2e36 3231 3234 3239 2c32 3920 342e 3933  .6212429,29 4.93
-00006950: 3535 3732 392c 3237 2e38 3838 3937 3720  55729,27.888977 
-00006960: 302c 3235 2e36 3239 3438 3220 7a20 4d20  0,25.629482 z M 
-00006970: 3230 2e39 3136 3833 312c 3139 2e33 3132  20.916831,19.312
-00006980: 3838 3220 4320 3230 2e39 3136 3833 312c  882 C 20.916831,
-00006990: 3230 2e35 3836 3138 3820 3231 2e33 3739  20.586188 21.379
-000069a0: 3135 2c32 312e 3638 3437 3238 2032 322e  15,21.684728 22.
-000069b0: 3331 3632 3834 2c32 322e 3630 3834 3939  316284,22.608499
-000069c0: 2043 2032 332e 3234 3039 3233 2c32 332e   C 23.240923,23.
-000069d0: 3533 3232 3731 2032 342e 3336 3534 3834  532271 24.365484
-000069e0: 2c32 332e 3939 3431 3537 2032 352e 3635  ,23.994157 25.65
-000069f0: 3234 3831 2c32 332e 3939 3431 3537 2043  2481,23.994157 C
-00006a00: 2032 362e 3935 3139 3734 2c32 332e 3939   26.951974,23.99
-00006a10: 3431 3537 2032 382e 3035 3135 3435 2c32  4157 28.051545,2
-00006a20: 332e 3533 3232 3731 2032 382e 3936 3336  3.532271 28.9636
-00006a30: 3838 2c32 322e 3634 3539 3439 2043 2032  88,22.645949 C 2
-00006a40: 392e 3836 3333 3337 2c32 312e 3734 3731  9.863337,21.7471
-00006a50: 3435 2033 302e 3331 3331 3631 2c32 302e  45 30.313161,20.
-00006a60: 3634 3836 3035 2033 302e 3331 3331 3631  648605 30.313161
-00006a70: 2c31 392e 3335 3033 3332 2043 2033 302e  ,19.350332 C 30.
-00006a80: 3331 3331 3631 2c31 382e 3032 3730 3931  313161,18.027091
-00006a90: 2032 392e 3836 3333 3337 2c31 362e 3930   29.863337,16.90
-00006aa0: 3335 3835 2032 382e 3935 3131 3933 2c31  3585 28.951193,1
-00006ab0: 352e 3937 3938 3134 2043 2032 382e 3033  5.979814 C 28.03
-00006ac0: 3930 3439 2c31 352e 3035 3630 3432 2032  9049,15.056042 2
-00006ad0: 362e 3933 3934 3739 2c31 342e 3539 3431  6.939479,14.5941
-00006ae0: 3536 2032 352e 3633 3939 3836 2c31 342e  56 25.639986,14.
-00006af0: 3539 3431 3536 2043 2032 342e 3332 3739  594156 C 24.3279
-00006b00: 3939 2c31 342e 3539 3431 3536 2032 332e  99,14.594156 23.
-00006b10: 3231 3539 3333 2c31 352e 3035 3630 3432  215933,15.056042
-00006b20: 2032 322e 3239 3132 3934 2c31 352e 3937   22.291294,15.97
-00006b30: 3938 3134 2043 2032 312e 3337 3931 352c  9814 C 21.37915,
-00006b40: 3136 2e38 3931 3130 3220 3230 2e39 3136  16.891102 20.916
-00006b50: 3833 312c 3138 2e30 3032 3132 3520 3230  831,18.002125 20
-00006b60: 2e39 3136 3833 312c 3139 2e33 3132 3838  .916831,19.31288
-00006b70: 3220 7a20 4d20 3332 2e30 3030 3030 322c  2 z M 32.000002,
-00006b80: 372e 3331 3633 3334 3120 4c20 3332 2e30  7.3163341 L 32.0
-00006b90: 3030 3030 322c 3130 2e30 3337 3731 3520  00002,10.037715 
-00006ba0: 4320 3236 2e37 3339 3535 372c 372e 3634  C 26.739557,7.64
-00006bb0: 3039 3032 3520 3231 2e36 3636 3533 382c  09025 21.666538,
-00006bc0: 362e 3434 3234 3936 3220 3136 2e37 3535  6.4424962 16.755
-00006bd0: 3935 362c 362e 3434 3234 3936 3220 4320  956,6.4424962 C 
-00006be0: 3133 2e35 3537 3230 352c 362e 3434 3234  13.557205,6.4424
-00006bf0: 3936 3220 3130 2e39 3333 3233 2c36 2e38  962 10.93323,6.8
-00006c00: 3534 3434 3833 2038 2e39 3039 3032 3039  544483 8.9090209
-00006c10: 2c37 2e37 3033 3331 3935 2043 2031 302e  ,7.7033195 C 10.
-00006c20: 3230 3835 3133 2c38 2e33 3532 3435 3633  208513,8.3524563
-00006c30: 2031 312e 3137 3036 3337 2c39 2e31 3736   11.170637,9.176
-00006c40: 3336 3037 2031 312e 3739 3533 3933 2c31  3607 11.795393,1
-00006c50: 302e 3136 3235 3439 2043 2031 322e 3434  0.162549 C 12.44
-00006c60: 3531 342c 3131 2e31 3438 3733 3820 3132  514,11.148738 12
-00006c70: 2e37 3537 3531 382c 3132 2e33 3039 3639  .757518,12.30969
-00006c80: 3420 3132 2e37 3537 3531 382c 3133 2e36  4 12.757518,13.6
-00006c90: 3435 3431 3820 4320 3132 2e37 3537 3531  45418 C 12.75751
-00006ca0: 382c 3135 2e33 3933 3039 3420 3132 2e31  8,15.393094 12.1
-00006cb0: 3332 3736 322c 3136 2e38 3931 3130 3220  32762,16.891102 
-00006cc0: 3130 2e38 3730 3735 352c 3138 2e31 3531  10.870755,18.151
-00006cd0: 3932 3520 4320 392e 3630 3837 3436 392c  925 C 9.6087469,
-00006ce0: 3139 2e34 3030 3236 3520 382e 3039 3638  19.400265 8.0968
-00006cf0: 3337 392c 3230 2e30 3234 3433 3520 362e  379,20.024435 6.
-00006d00: 3333 3530 3235 392c 3230 2e30 3234 3433  3350259,20.02443
-00006d10: 3520 4320 342e 3538 3537 3038 392c 3230  5 C 4.5857089,20
-00006d20: 2e30 3234 3433 3520 332e 3039 3837 3839  .024435 3.098789
-00006d30: 392c 3139 2e34 3132 3734 3920 312e 3836  9,19.412749 1.86
-00006d40: 3137 3732 392c 3138 2e31 3634 3430 3920  17729,18.164409 
-00006d50: 4320 302e 3632 3437 3536 2c31 362e 3932  C 0.624756,16.92
-00006d60: 3835 3532 2030 2c31 352e 3433 3035 3434  8552 0,15.430544
-00006d70: 2030 2c31 332e 3638 3238 3638 2043 2030   0,13.682868 C 0
-00006d80: 2c31 302e 3838 3635 3836 2031 2e36 3939  ,10.886586 1.699
-00006d90: 3333 3634 2c38 2e35 3532 3139 3037 2035  3364,8.5521907 5
-00006da0: 2e31 3130 3530 3339 2c36 2e37 3034 3634  .1105039,6.70464
-00006db0: 3735 2043 2038 2e35 3039 3137 3639 2c34  75 C 8.5091769,4
-00006dc0: 2e38 3537 3130 3434 2031 322e 3739 3530  .8571044 12.7950
-00006dd0: 3033 2c33 2e39 3333 3333 3237 2031 372e  03,3.9333327 17.
-00006de0: 3933 3034 3937 2c33 2e39 3333 3333 3237  930497,3.9333327
-00006df0: 2043 2032 322e 3337 3837 362c 332e 3933   C 22.37876,3.93
-00006e00: 3333 3332 3720 3237 2e30 3634 3433 2c35  33327 27.06443,5
-00006e10: 2e30 3536 3833 3838 2033 322e 3030 3030  .0568388 32.0000
-00006e20: 3032 2c37 2e33 3136 3333 3431 207a 204d  02,7.3163341 z M
-00006e30: 2031 312e 3038 3331 3732 2c31 332e 3633   11.083172,13.63
-00006e40: 3239 3335 2043 2031 312e 3038 3331 3732  2935 C 11.083172
-00006e50: 2c31 322e 3334 3731 3434 2031 302e 3632  ,12.347144 10.62
-00006e60: 3038 3532 2c31 312e 3234 3836 3035 2039  0852,11.248605 9
-00006e70: 2e36 3833 3731 3739 2c31 302e 3332 3438  .6837179,10.3248
-00006e80: 3334 2043 2038 2e37 3436 3538 3339 2c39  34 C 8.7465839,9
-00006e90: 2e34 3133 3534 3533 2037 2e36 3232 3032  .4135453 7.62202
-00006ea0: 3239 2c38 2e39 3531 3635 3935 2036 2e33  29,8.9516595 6.3
-00006eb0: 3232 3533 3039 2c38 2e39 3531 3635 3935  225309,8.9516595
-00006ec0: 2043 2035 2e30 3233 3033 3739 2c38 2e39   C 5.0230379,8.9
-00006ed0: 3531 3635 3935 2033 2e39 3233 3436 3739  516595 3.9234679
-00006ee0: 2c39 2e34 3031 3036 3139 2033 2e30 3233  ,9.4010619 3.023
-00006ef0: 3831 3839 2c31 302e 3239 3938 3637 2043  8189,10.299867 C
-00006f00: 2032 2e31 3234 3137 3039 2c31 312e 3139   2.1241709,11.19
-00006f10: 3836 3732 2031 2e36 3734 3334 3631 2c31  8672 1.6743461,1
-00006f20: 322e 3239 3732 3131 2031 2e36 3734 3334  2.297211 1.67434
-00006f30: 3631 2c31 332e 3539 3534 3834 2043 2031  61,13.595484 C 1
-00006f40: 2e36 3734 3334 3631 2c31 342e 3931 3837  .6743461,14.9187
-00006f50: 3235 2032 2e31 3336 3636 3539 2c31 362e  25 2.1366659,16.
-00006f60: 3034 3232 3331 2033 2e30 3438 3830 3839  042231 3.0488089
-00006f70: 2c31 362e 3936 3630 3032 2043 2033 2e39  ,16.966002 C 3.9
-00006f80: 3438 3435 3739 2c31 372e 3838 3937 3734  484579,17.889774
-00006f90: 2035 2e30 3630 3532 3339 2c31 382e 3335   5.0605239,18.35
-00006fa0: 3136 3620 362e 3336 3030 3135 392c 3138  166 6.3600159,18
-00006fb0: 2e33 3531 3636 2043 2037 2e36 3539 3530  .35166 C 7.65950
-00006fc0: 3839 2c31 382e 3335 3136 3620 382e 3738  89,18.35166 8.78
-00006fd0: 3430 3638 392c 3137 2e38 3839 3737 3420  40689,17.889774 
-00006fe0: 392e 3639 3632 3132 392c 3136 2e39 3636  9.6962129,16.966
-00006ff0: 3030 3220 4320 3130 2e36 3230 3835 322c  002 C 10.620852,
-00007000: 3136 2e30 3432 3233 3120 3131 2e30 3833  16.042231 11.083
-00007010: 3137 322c 3134 2e39 3331 3230 3820 3131  172,14.931208 11
-00007020: 2e30 3833 3137 322c 3133 2e36 3332 3933  .083172,13.63293
-00007030: 3520 7a20 220a 2020 2020 2020 2020 2020  5 z ".          
-00007040: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00007050: 796c 653d 2266 696c 6c3a 2024 7a6f 6469  yle="fill: $zodi
-00007060: 6163 5f63 6f6c 6f72 5f33 220a 2020 2020  ac_color_3".    
-00007070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007080: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00007090: 2020 203c 2f73 796d 626f 6c3e 0a20 2020     </symbol>.   
-000070a0: 2020 2020 2020 2020 2020 2020 203c 7379               <sy
-000070b0: 6d62 6f6c 2069 643d 226c 656f 223e 0a20  mbol id="leo">. 
-000070c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070d0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-000070e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070f0: 2064 3d22 4d20 3238 2e30 3231 3337 312c   d="M 28.021371,
-00007100: 3239 2e34 3830 3832 3120 4320 3237 2e33  29.480821 C 27.3
-00007110: 3738 3333 392c 3330 2e30 3639 3934 3820  78339,30.069948 
-00007120: 3236 2e36 3837 3939 322c 3330 2e36 3132  26.687992,30.612
-00007130: 3339 3220 3235 2e39 3333 3630 322c 3331  392 25.933602,31
-00007140: 2e30 3532 3335 3920 4320 3235 2e33 3034  .052359 C 25.304
-00007150: 3339 342c 3331 2e34 3138 3730 3120 3234  394,31.418701 24
-00007160: 2e36 3237 3432 392c 3331 2e37 3132 3039  .627429,31.71209
-00007170: 3120 3233 2e39 3135 3032 322c 3331 2e38  1 23.915022,31.8
-00007180: 3730 3437 3220 4320 3233 2e34 3837 3830  70472 C 23.48780
-00007190: 372c 3331 2e39 3636 2032 332e 3034 3839  7,31.966 23.0489
-000071a0: 3737 2c33 322e 3031 3032 3632 2032 322e  77,32.010262 22.
-000071b0: 3631 3132 3739 2c33 312e 3939 3739 3938  611279,31.997998
-000071c0: 2043 2032 312e 3939 3630 3835 2c33 312e   C 21.996085,31.
-000071d0: 3938 3431 3537 2032 312e 3338 3033 3435  984157 21.380345
-000071e0: 2c33 312e 3837 3734 3534 2032 302e 3830  ,31.877454 20.80
-000071f0: 3439 3131 2c33 312e 3635 3634 3236 2043  4911,31.656426 C
-00007200: 2032 302e 3237 3334 3539 2c33 312e 3435   20.273459,31.45
-00007210: 3337 3920 3139 2e37 3830 3432 2c33 312e  379 19.78042,31.
-00007220: 3135 3339 3033 2031 392e 3335 3034 3535  153903 19.350455
-00007230: 2c33 302e 3738 3230 3238 2043 2031 392e  ,30.782028 C 19.
-00007240: 3031 3539 342c 3330 2e34 3933 3736 3920  01594,30.493769 
-00007250: 3138 2e37 3138 3030 322c 3330 2e31 3632  18.718002,30.162
-00007260: 3735 3720 3138 2e34 3637 3736 322c 3239  757 18.467762,29
-00007270: 2e37 3938 3834 3620 4320 3138 2e31 3538  .798846 C 18.158
-00007280: 3738 312c 3239 2e33 3439 3633 3320 3137  781,29.349633 17
-00007290: 2e39 3239 3738 322c 3238 2e38 3435 3733  .929782,28.84573
-000072a0: 3920 3137 2e37 3934 3732 352c 3238 2e33  9 17.794725,28.3
-000072b0: 3137 3437 3920 4320 3137 2e36 3335 3934  17479 C 17.63594
-000072c0: 2c32 372e 3730 3038 3731 2031 372e 3630  ,27.700871 17.60
-000072d0: 3133 3535 2c32 372e 3035 3632 3337 2031  1355,27.056237 1
-000072e0: 372e 3635 3838 3936 2c32 362e 3432 3334  7.658896,26.4234
-000072f0: 3032 2043 2031 372e 3731 3634 3835 2c32  02 C 17.716485,2
-00007300: 352e 3738 3338 3732 2031 372e 3834 3830  5.783872 17.8480
-00007310: 3133 2c32 352e 3135 3333 3036 2031 382e  13,25.153306 18.
-00007320: 3030 3834 3439 2c32 342e 3533 3233 3534  008449,24.532354
-00007330: 2043 2031 382e 3235 3639 3035 2c32 332e   C 18.256905,23.
-00007340: 3538 3036 3131 2031 382e 3537 3738 3733  580611 18.577873
-00007350: 2c32 322e 3634 3933 3520 3138 2e39 3238  ,22.64935 18.928
-00007360: 3439 312c 3231 2e37 3330 3837 3320 4320  491,21.730873 C 
-00007370: 3139 2e34 3434 3935 382c 3230 2e33 3833  19.444958,20.383
-00007380: 3731 3620 3230 2e30 3330 3137 342c 3139  716 20.030174,19
-00007390: 2e30 3633 3938 3820 3230 2e36 3434 3937  .063988 20.64497
-000073a0: 312c 3137 2e37 3539 3134 3420 4320 3231  1,17.759144 C 21
-000073b0: 2e31 3337 3230 352c 3136 2e37 3130 3130  .137205,16.71010
-000073c0: 3120 3231 2e36 3239 3433 372c 3135 2e36  1 21.629437,15.6
-000073d0: 3631 3036 2032 322e 3132 3136 3639 2c31  6106 22.121669,1
-000073e0: 342e 3631 3230 3137 2043 2032 322e 3536  4.612017 C 22.56
-000073f0: 3332 3237 2c31 332e 3636 3532 3038 2032  3227,13.665208 2
-00007400: 322e 3936 3537 3433 2c31 322e 3639 3834  2.965743,12.6984
-00007410: 3520 3233 2e32 3836 3035 322c 3131 2e37  5 23.286052,11.7
-00007420: 3033 3433 3220 4320 3233 2e35 3134 3039  03432 C 23.51409
-00007430: 392c 3130 2e39 3930 3731 2032 332e 3730  9,10.99071 23.70
-00007440: 3132 3535 2c31 302e 3236 3235 3034 2032  1255,10.262504 2
-00007450: 332e 3830 3131 3831 2c39 2e35 3230 3032  3.801181,9.52002
-00007460: 3836 2043 2032 332e 3835 3231 3936 2c39  86 C 23.852196,9
-00007470: 2e31 3430 3537 3436 2032 332e 3837 3735  .1405746 23.8775
-00007480: 3837 2c38 2e37 3537 3339 3136 2032 332e  87,8.7573916 23.
-00007490: 3836 3933 3131 2c38 2e33 3734 3437 3636  869311,8.3744766
-000074a0: 2043 2032 332e 3835 3638 3939 2c37 2e35   C 23.856899,7.5
-000074b0: 3836 3933 3134 2032 332e 3735 3035 3439  869314 23.750549
-000074c0: 2c36 2e37 3936 3536 3138 2032 332e 3530  ,6.7965618 23.50
-000074d0: 3533 3031 2c36 2e30 3436 3336 3335 2043  5301,6.0463635 C
-000074e0: 2032 332e 3330 3130 3538 2c35 2e34 3138   23.301058,5.418
-000074f0: 3630 3520 3232 2e39 3936 3535 392c 342e  605 22.996559,4.
-00007500: 3832 3234 3637 3420 3232 2e35 3937 3430  8224674 22.59740
-00007510: 312c 342e 3239 3631 3432 3120 4320 3232  1,4.2961421 C 22
-00007520: 2e33 3731 3130 372c 332e 3939 3731 3838  .371107,3.997188
-00007530: 3120 3232 2e31 3135 3838 2c33 2e37 3230  1 22.11588,3.720
-00007540: 3335 3332 2032 312e 3833 3931 3332 2c33  3532 21.839132,3
-00007550: 2e34 3637 3533 3333 2043 2032 312e 3337  .4675333 C 21.37
-00007560: 3933 382c 332e 3034 3837 3533 3220 3230  938,3.0487532 20
-00007570: 2e38 3438 3631 2c32 2e37 3038 3234 3234  .84861,2.7082424
-00007580: 2032 302e 3237 3538 3236 2c32 2e34 3636   20.275826,2.466
-00007590: 3031 3734 2043 2031 392e 3632 3332 3031  0174 C 19.623201
-000075a0: 2c32 2e31 3838 3432 3920 3138 2e39 3231  ,2.188429 18.921
-000075b0: 3335 312c 322e 3033 3733 3937 2031 382e  351,2.037397 18.
-000075c0: 3231 3535 382c 312e 3938 3334 3937 3320  21558,1.9834973 
-000075d0: 4320 3137 2e37 3038 3935 322c 312e 3934  C 17.708952,1.94
-000075e0: 3535 3838 3220 3137 2e31 3938 3639 312c  55882 17.198691,
-000075f0: 312e 3935 3034 3538 3220 3136 2e36 3933  1.9504582 16.693
-00007600: 3338 342c 322e 3030 3433 3035 3420 4320  384,2.0043054 C 
-00007610: 3136 2e30 3138 3434 352c 322e 3037 3635  16.018445,2.0765
-00007620: 3630 3820 3135 2e33 3530 3832 382c 322e  608 15.350828,2.
-00007630: 3234 3437 3736 3620 3134 2e37 3334 3137  2447766 14.73417
-00007640: 312c 322e 3533 3133 3038 3320 4320 3134  1,2.5313083 C 14
-00007650: 2e31 3737 3130 352c 322e 3738 3838 3537  .177105,2.788857
-00007660: 2031 332e 3636 3530 3433 2c33 2e31 3432   13.665043,3.142
-00007670: 3339 3735 2031 332e 3232 3433 3138 2c33  3975 13.224318,3
-00007680: 2e35 3639 3334 3739 2043 2031 322e 3739  .5693479 C 12.79
-00007690: 3535 3335 2c33 2e39 3935 3133 3333 2031  5535,3.9951333 1
-000076a0: 322e 3433 3534 3537 2c34 2e34 3931 3234  2.435457,4.49124
-000076b0: 3138 2031 322e 3137 3237 3139 2c35 2e30  18 12.172719,5.0
-000076c0: 3335 3837 3733 2043 2031 312e 3839 3030  358773 C 11.8900
-000076d0: 3934 2c35 2e36 3138 3134 3637 2031 312e  94,5.6181467 11.
-000076e0: 3731 3936 3432 2c36 2e32 3531 3330 3831  719642,6.2513081
-000076f0: 2031 312e 3634 3339 3437 2c36 2e38 3933   11.643947,6.893
-00007700: 3130 3239 2043 2031 312e 3536 3230 3137  1029 C 11.562017
-00007710: 2c37 2e35 3834 3433 3233 2031 312e 3538  ,7.5844323 11.58
-00007720: 3238 322c 382e 3238 3537 3339 3620 3131  282,8.2857396 11
-00007730: 2e36 3830 3533 332c 382e 3937 3433 3033  .680533,8.974303
-00007740: 3620 4320 3131 2e38 3036 3038 312c 392e  6 C 11.806081,9.
-00007750: 3836 3137 3630 3620 3132 2e30 3438 3937  8617606 12.04897
-00007760: 352c 3130 2e37 3239 3135 3220 3132 2e33  5,10.729152 12.3
-00007770: 3534 3033 332c 3131 2e35 3730 3639 3120  54033,11.570691 
-00007780: 4320 3132 2e35 3938 3739 382c 3132 2e32  C 12.598798,12.2
-00007790: 3434 3833 3720 3132 2e38 3835 3439 392c  44837 12.885499,
-000077a0: 3132 2e39 3033 3131 3720 3133 2e31 3938  12.903117 13.198
-000077b0: 3339 382c 3133 2e35 3438 3236 3820 4320  398,13.548268 C 
-000077c0: 3133 2e34 3039 3936 342c 3133 2e39 3837  13.409964,13.987
-000077d0: 3638 3220 3133 2e36 3231 3931 312c 3134  682 13.621911,14
-000077e0: 2e34 3236 3931 3520 3133 2e38 3333 3137  .426915 13.83317
-000077f0: 312c 3134 2e38 3636 3437 3520 4320 3134  1,14.866475 C 14
-00007800: 2e31 3830 3438 382c 3135 2e35 3936 2031  .180488,15.596 1
-00007810: 342e 3530 3738 3633 2c31 362e 3333 3631  4.507863,16.3361
-00007820: 3136 2031 342e 3738 3137 342c 3137 2e30  16 14.78174,17.0
-00007830: 3936 3636 3420 4320 3134 2e39 3534 3633  96664 C 14.95463
-00007840: 392c 3137 2e35 3830 3930 3320 3135 2e31  9,17.580903 15.1
-00007850: 3037 3734 312c 3138 2e30 3733 3839 3820  07741,18.073898 
-00007860: 3135 2e32 3034 3636 342c 3138 2e35 3739  15.204664,18.579
-00007870: 3436 3820 4320 3135 2e32 3630 3631 352c  468 C 15.260615,
-00007880: 3138 2e38 3734 3430 3420 3135 2e32 3935  18.874404 15.295
-00007890: 3930 352c 3139 2e31 3734 3439 3220 3135  905,19.174492 15
-000078a0: 2e32 3838 3530 312c 3139 2e34 3735 3039  .288501,19.47509
-000078b0: 3620 4320 3135 2e32 3739 3533 312c 3230  6 C 15.279531,20
-000078c0: 2e31 3230 3036 3420 3135 2e31 3634 3035  .120064 15.16405
-000078d0: 382c 3230 2e37 3634 3537 3520 3134 2e39  8,20.764575 14.9
-000078e0: 3336 3332 2c32 312e 3336 3835 3633 2043  3632,21.368563 C
-000078f0: 2031 342e 3730 3235 3632 2c32 312e 3939   14.702562,21.99
-00007900: 3239 3338 2031 342e 3335 3133 3936 2c32  2938 14.351396,2
-00007910: 322e 3537 3033 3737 2031 332e 3932 3236  2.570377 13.9226
-00007920: 3134 2c32 332e 3037 3937 3239 2043 2031  14,23.079729 C 1
-00007930: 332e 3539 3631 3638 2c32 332e 3436 3637  3.596168,23.4667
-00007940: 3638 2031 332e 3232 3934 3435 2c32 332e  68 13.229445,23.
-00007950: 3832 3033 3035 2031 322e 3832 3830 312c  820305 12.82801,
-00007960: 3234 2e31 3239 3030 3620 4320 3132 2e33  24.129006 C 12.3
-00007970: 3030 3439 342c 3234 2e35 3334 3635 3320  00494,24.534653 
-00007980: 3131 2e37 3037 3032 312c 3234 2e38 3536  11.707021,24.856
-00007990: 3237 3720 3131 2e30 3734 3335 2c32 352e  277 11.07435,25.
-000079a0: 3036 3430 3431 2043 2031 302e 3432 3830  064041 C 10.4280
-000079b0: 3533 2c32 352e 3237 3739 3039 2039 2e37  53,25.277909 9.7
-000079c0: 3434 3933 3735 2c32 352e 3337 3231 3933  449375,25.372193
-000079d0: 2039 2e30 3635 3033 3939 2c32 352e 3336   9.0650399,25.36
-000079e0: 3337 3637 2043 2038 2e33 3735 3935 3933  3767 C 8.3759593
-000079f0: 2c32 352e 3335 3638 3639 2037 2e36 3835  ,25.356869 7.685
-00007a00: 3530 3138 2c32 352e 3234 3735 3931 2037  5018,25.247591 7
-00007a10: 2e30 3335 3538 3139 2c32 352e 3031 3535  .0355819,25.0155
-00007a20: 3537 2043 2036 2e34 3232 3234 3337 2c32  57 C 6.4222437,2
-00007a30: 342e 3739 3831 3338 2035 2e38 3438 3936  4.798138 5.84896
-00007a40: 3837 2c32 342e 3437 3137 3036 2035 2e33  87,24.471706 5.3
-00007a50: 3432 3931 3138 2c32 342e 3036 3331 3333  429118,24.063133
-00007a60: 2043 2035 2e30 3433 3936 3935 2c32 332e   C 5.0439695,23.
-00007a70: 3832 3233 3238 2034 2e37 3637 3734 3931  822328 4.7677491
-00007a80: 2c32 332e 3535 3338 3938 2034 2e35 3132  ,23.553898 4.512
-00007a90: 3335 3733 2c32 332e 3236 3735 2043 2034  3573,23.2675 C 4
-00007aa0: 2e30 3735 3535 3331 2c32 322e 3737 3536  .0755531,22.7756
-00007ab0: 3438 2033 2e37 3134 3137 3432 2c32 322e  48 3.7141742,22.
-00007ac0: 3231 3439 3434 2033 2e34 3631 3635 3138  214944 3.4616518
-00007ad0: 2c32 312e 3630 3638 3434 2043 2033 2e32  ,21.606844 C 3.2
-00007ae0: 3033 3737 3737 2c32 302e 3938 3939 3520  037777,20.98995 
-00007af0: 332e 3035 3934 3337 382c 3230 2e33 3238  3.0594378,20.328
-00007b00: 3235 3920 332e 3031 3537 3932 382c 3139  259 3.0157928,19
-00007b10: 2e36 3631 3830 3620 4320 322e 3936 3933  .661806 C 2.9693
-00007b20: 3031 382c 3138 2e39 3535 3433 3320 332e  018,18.955433 3.
-00007b30: 3032 3331 3833 382c 3138 2e32 3339 3339  0231838,18.23939
-00007b40: 3720 332e 3230 3737 3130 342c 3137 2e35  7 3.2077104,17.5
-00007b50: 3534 3734 2043 2033 2e33 3732 3732 3235  5474 C 3.3727225
-00007b60: 2c31 362e 3933 3732 3333 2033 2e36 3434  ,16.937233 3.644
-00007b70: 3733 3733 2c31 362e 3334 3931 3934 2034  7373,16.349194 4
-00007b80: 2e30 3034 3133 3939 2c31 352e 3832 3039  .0041399,15.8209
-00007b90: 3031 2043 2034 2e33 3032 3734 332c 3135  01 C 4.302743,15
-00007ba0: 2e33 3739 3930 3620 342e 3636 3037 3230  .379906 4.660720
-00007bb0: 382c 3134 2e39 3831 3038 3420 352e 3035  8,14.981084 5.05
-00007bc0: 3236 3132 362c 3134 2e36 3231 3237 3320  26126,14.621273 
-00007bd0: 4320 352e 3534 3231 3339 392c 3134 2e31  C 5.5421399,14.1
-00007be0: 3733 3436 3720 362e 3130 3133 3632 392c  73467 6.1013629,
-00007bf0: 3133 2e37 3938 3733 3420 362e 3731 3231  13.798734 6.7121
-00007c00: 3934 332c 3133 2e35 3337 3637 3320 4320  943,13.537673 C 
-00007c10: 372e 3330 3230 3838 372c 3133 2e32 3833  7.3020887,13.283
-00007c20: 3931 2037 2e39 3336 3832 3231 2c31 332e  91 7.9368221,13.
-00007c30: 3133 3837 3631 2038 2e35 3737 3136 3235  138761 8.5771625
-00007c40: 2c31 332e 3039 3737 3439 2043 2038 2e38  ,13.097749 C 8.8
-00007c50: 3937 3135 3834 2c31 332e 3037 3637 3137  971584,13.076717
-00007c60: 2039 2e32 3138 3938 3337 2c31 332e 3037   9.2189837,13.07
-00007c70: 3934 3733 2039 2e35 3338 3039 3233 2c31  9473 9.5380923,1
-00007c80: 332e 3131 3233 3736 2043 2031 302e 3031  3.112376 C 10.01
-00007c90: 3833 3235 2c31 332e 3136 3038 3634 2031  8325,13.160864 1
-00007ca0: 302e 3439 3134 3135 2c31 332e 3236 3735  0.491415,13.2675
-00007cb0: 3220 3130 2e39 3531 3837 372c 3133 2e34  2 10.951877,13.4
-00007cc0: 3130 3835 3120 4320 3130 2e34 3736 3637  10851 C 10.47667
-00007cd0: 382c 3132 2e34 3933 3236 3220 3130 2e30  8,12.493262 10.0
-00007ce0: 3536 3935 312c 3131 2e35 3434 3035 3520  56951,11.544055 
-00007cf0: 392e 3734 3538 3136 362c 3130 2e35 3537  9.7458166,10.557
-00007d00: 3635 3820 4320 392e 3439 3136 3432 2c39  658 C 9.491642,9
-00007d10: 2e37 3438 3832 3836 2039 2e33 3130 3936  .7488286 9.31096
-00007d20: 3139 2c38 2e39 3132 3835 3436 2039 2e32  19,8.9128546 9.2
-00007d30: 3632 3234 3136 2c38 2e30 3634 3937 3236  622416,8.0649726
-00007d40: 2043 2039 2e32 3336 3330 352c 372e 3630   C 9.236305,7.60
-00007d50: 3331 3330 3820 392e 3235 3036 3137 2c37  31308 9.250617,7
-00007d60: 2e31 3339 3132 3937 2039 2e33 3031 3236  .1391297 9.30126
-00007d70: 3539 2c36 2e36 3739 3431 3037 2043 2039  59,6.6794107 C 9
-00007d80: 2e33 3836 3235 3037 2c35 2e39 3133 3236  .3862507,5.91326
-00007d90: 3835 2039 2e35 3836 3838 3032 2c35 2e31  85 9.5868802,5.1
-00007da0: 3538 3230 3338 2039 2e39 3132 3735 3337  582038 9.9127537
-00007db0: 2c34 2e34 3538 3834 3837 2043 2031 302e  ,4.4588487 C 10.
-00007dc0: 3233 3335 3437 2c33 2e37 3636 3438 3936  233547,3.7664896
-00007dd0: 2031 302e 3637 3531 3731 2c33 2e31 3332   10.675171,3.132
-00007de0: 3532 2031 312e 3139 3937 3438 2c32 2e35  52 11.199748,2.5
-00007df0: 3739 3331 3838 2043 2031 312e 3835 3135  793188 C 11.8515
-00007e00: 3031 2c31 2e38 3932 3730 3738 2031 322e  01,1.8927078 12.
-00007e10: 3631 3936 3034 2c31 2e33 3134 3437 3436  619604,1.3144746
-00007e20: 2031 332e 3436 3739 3735 2c30 2e38 3933   13.467975,0.893
-00007e30: 3033 3637 3220 4320 3134 2e32 3337 3534  03672 C 14.23754
-00007e40: 362c 302e 3530 3931 3037 3832 2031 352e  6,0.50910782 15.
-00007e50: 3036 3935 3637 2c30 2e32 3536 3137 3134  069567,0.2561714
-00007e60: 3220 3135 2e39 3138 3339 312c 302e 3132  2 15.918391,0.12
-00007e70: 3330 3836 3932 2043 2031 362e 3734 3434  308692 C 16.7444
-00007e80: 3539 2c2d 302e 3030 3732 3337 3238 3338  59,-0.0072372838
-00007e90: 2031 372e 3538 3534 3532 2c2d 302e 3032   17.585452,-0.02
-00007ea0: 3639 3837 3738 3420 3138 2e34 3138 3937  6987784 18.41897
-00007eb0: 372c 302e 3032 3933 3836 3631 3620 4320  7,0.029386616 C 
-00007ec0: 3139 2e33 3639 3239 352c 302e 3039 3533  19.369295,0.0953
-00007ed0: 3637 3931 3620 3230 2e33 3135 3438 342c  67916 20.315484,
-00007ee0: 302e 3237 3935 3837 3132 2032 312e 3230  0.27958712 21.20
-00007ef0: 3633 3538 2c30 2e36 3231 3337 3631 3220  6358,0.62137612 
-00007f00: 4320 3231 2e39 3731 3237 392c 302e 3931  C 21.971279,0.91
-00007f10: 3335 3739 3032 2032 322e 3639 3136 3433  357902 22.691643
-00007f20: 2c31 2e33 3233 3830 3735 2032 332e 3332  ,1.3238075 23.32
-00007f30: 3834 3331 2c31 2e38 3339 3038 3536 2043  8431,1.8390856 C
-00007f40: 2032 332e 3632 3130 3632 2c32 2e30 3735   23.621062,2.075
-00007f50: 3336 3637 2032 332e 3839 3732 3931 2c32  3667 23.897291,2
-00007f60: 2e33 3332 3231 3638 2032 342e 3135 3035  .3322168 24.1505
-00007f70: 3133 2c32 2e36 3130 3435 3132 2043 2032  13,2.6104512 C 2
-00007f80: 342e 3638 3533 3536 2c33 2e31 3933 3336  4.685356,3.19336
-00007f90: 3534 2032 352e 3132 3734 3837 2c33 2e38  54 25.127487,3.8
-00007fa0: 3631 3236 3734 2032 352e 3435 3331 3936  612674 25.453196
-00007fb0: 2c34 2e35 3832 3334 3520 4320 3235 2e38  ,4.582345 C 25.8
-00007fc0: 3137 3834 312c 352e 3338 3537 3830 3520  17841,5.3857805 
-00007fd0: 3236 2e30 3338 3334 372c 362e 3235 3033  26.038347,6.2503
-00007fe0: 3236 3220 3236 2e31 3430 3731 392c 372e  262 26.140719,7.
-00007ff0: 3132 3534 3238 3220 4320 3236 2e32 3031  1254282 C 26.201
-00008000: 3435 382c 372e 3633 3732 3137 3120 3236  458,7.6372171 26
-00008010: 2e32 3230 3834 392c 382e 3135 3332 3237  .220849,8.153227
-00008020: 3620 3236 2e32 3132 3435 2c38 2e36 3638  6 26.21245,8.668
-00008030: 3334 3136 2043 2032 362e 3230 3137 3235  3416 C 26.201725
-00008040: 2c39 2e34 3036 3936 3936 2032 362e 3134  ,9.4069696 26.14
-00008050: 3730 3233 2c31 302e 3134 3638 3631 2032  7023,10.146861 2
-00008060: 362e 3031 3130 3531 2c31 302e 3837 3336  6.011051,10.8736
-00008070: 3531 2043 2032 352e 3935 3738 3839 2c31  51 C 25.957889,1
-00008080: 312e 3135 3831 3432 2032 352e 3839 3035  1.158142 25.8905
-00008090: 3432 2c31 312e 3433 3939 3732 2032 352e  42,11.439972 25.
-000080a0: 3830 3835 3536 2c31 312e 3731 3735 3338  808556,11.717538
-000080b0: 2043 2032 352e 3638 3831 3836 2c31 322e   C 25.688186,12.
-000080c0: 3133 3739 3137 2032 352e 3533 3639 3638  137917 25.536968
-000080d0: 2c31 322e 3534 3836 3938 2032 352e 3337  ,12.548698 25.37
-000080e0: 3932 3132 2c31 322e 3935 3632 3631 2043  9212,12.956261 C
-000080f0: 2032 352e 3037 3739 3633 2c31 332e 3732   25.077963,13.72
-00008100: 3738 3437 2032 342e 3734 3537 3635 2c31  7847 24.745765,1
-00008110: 342e 3438 3639 3038 2032 342e 3430 3539  4.486908 24.4059
-00008120: 3038 2c31 352e 3234 3231 3331 2043 2032  08,15.242131 C 2
-00008130: 342e 3234 3836 312c 3135 2e35 3931 3837  4.24861,15.59187
-00008140: 3320 3234 2e30 3837 3630 382c 3135 2e39  3 24.087608,15.9
-00008150: 3339 3932 3620 3233 2e39 3236 3935 392c  39926 23.926959,
-00008160: 3136 2e32 3838 3133 3420 4320 3233 2e35  16.288134 C 23.5
-00008170: 3733 3933 322c 3137 2e30 3538 3837 3420  73932,17.058874 
-00008180: 3233 2e32 3230 3930 342c 3137 2e38 3239  23.220904,17.829
-00008190: 3631 3520 3232 2e38 3637 3837 362c 3138  615 22.867876,18
-000081a0: 2e36 3030 3335 3520 4320 3232 2e32 3738  .600355 C 22.278
-000081b0: 3831 322c 3139 2e38 3830 3035 3920 3231  812,19.880059 21
-000081c0: 2e37 3036 3234 352c 3231 2e31 3637 3920  .706245,21.1679 
-000081d0: 3231 2e31 3832 3037 2c32 322e 3437 3537  21.18207,22.4757
-000081e0: 3331 2043 2032 302e 3837 3536 3933 2c32  31 C 20.875693,2
-000081f0: 332e 3234 3432 3532 2032 302e 3538 3337  3.244252 20.5837
-00008200: 3936 2c32 342e 3031 3933 3936 2032 302e  96,24.019396 20.
-00008210: 3333 3936 3439 2c32 342e 3831 3032 3037  339649,24.810207
-00008220: 2043 2032 302e 3230 3533 3631 2c32 352e   C 20.205361,25.
-00008230: 3235 3036 3237 2032 302e 3038 3333 3839  250627 20.083389
-00008240: 2c32 352e 3639 3631 3336 2032 302e 3030  ,25.696136 20.00
-00008250: 3738 3635 2c32 362e 3135 3038 3234 2043  7865,26.150824 C
-00008260: 2031 392e 3937 3031 3836 2c32 362e 3338   19.970186,26.38
-00008270: 3034 3433 2031 392e 3934 3635 3235 2c32  0443 19.946525,2
-00008280: 362e 3631 3332 3232 2031 392e 3935 3432  6.613222 19.9542
-00008290: 3331 2c32 362e 3834 3631 3435 2043 2031  31,26.846145 C 1
-000082a0: 392e 3936 3338 3737 2c32 372e 3237 3530  9.963877,27.2750
-000082b0: 3236 2032 302e 3033 3738 3137 2c32 372e  26 20.037817,27.
-000082c0: 3730 3537 3620 3230 2e32 3032 3532 332c  70576 20.202523,
-000082d0: 3238 2e31 3033 3236 3320 4320 3230 2e33  28.103263 C 20.3
-000082e0: 3335 3538 342c 3238 2e34 3236 3830 3620  35584,28.426806 
-000082f0: 3230 2e35 3239 3231 372c 3238 2e37 3234  20.529217,28.724
-00008300: 3933 2032 302e 3736 3931 3638 2c32 382e  93 20.769168,28.
-00008310: 3937 3933 3633 2043 2032 312e 3030 3731  979363 C 21.0071
-00008320: 3331 2c32 392e 3234 3433 3438 2032 312e  31,29.244348 21.
-00008330: 3239 3634 3839 2c32 392e 3436 3435 3639  296489,29.464569
-00008340: 2032 312e 3632 3035 3738 2c32 392e 3631   21.620578,29.61
-00008350: 3333 3834 2043 2032 312e 3936 3636 3139  3384 C 21.966619
-00008360: 2c32 392e 3737 3338 3133 2032 322e 3334  ,29.773813 22.34
-00008370: 3732 342c 3239 2e38 3531 3733 3420 3232  724,29.851734 22
-00008380: 2e37 3237 3433 2c32 392e 3836 3337 3338  .72743,29.863738
-00008390: 2043 2032 332e 3039 3130 3236 2c32 392e   C 23.091026,29.
-000083a0: 3837 3736 3535 2032 332e 3435 3530 362c  877655 23.45506,
-000083b0: 3239 2e38 3232 3530 3320 3233 2e38 3033  29.822503 23.803
-000083c0: 3537 372c 3239 2e37 3230 3334 3320 4320  577,29.720343 C 
-000083d0: 3234 2e33 3130 3533 332c 3239 2e35 3731  24.310533,29.571
-000083e0: 3737 2032 342e 3738 3633 3033 2c32 392e  77 24.786303,29.
-000083f0: 3333 3137 3331 2032 352e 3233 3238 3437  331731 25.232847
-00008400: 2c32 392e 3035 3230 3434 2043 2032 352e  ,29.052044 C 25.
-00008410: 3733 3436 3438 2c32 382e 3733 3635 3337  734648,28.736537
-00008420: 2032 362e 3230 3138 3637 2c32 382e 3336   26.201867,28.36
-00008430: 3837 3739 2032 362e 3634 3535 3531 2c32  8779 26.645551,2
-00008440: 372e 3937 3634 3438 2043 2032 372e 3130  7.976448 C 27.10
-00008450: 3431 3538 2c32 382e 3437 3739 3036 2032  4158,28.477906 2
-00008460: 372e 3536 3237 3635 2c32 382e 3937 3933  7.562765,28.9793
-00008470: 3633 2032 382e 3032 3133 3731 2c32 392e  63 28.021371,29.
-00008480: 3438 3038 3231 207a 204d 2034 2e37 3439  480821 z M 4.749
-00008490: 3032 3735 2c31 392e 3230 3637 3639 2043  0275,19.206769 C
-000084a0: 2034 2e37 3438 3431 3432 2c31 392e 3735   4.7484142,19.75
-000084b0: 3530 3532 2034 2e38 3333 3635 3434 2c32  5052 4.8336544,2
-000084c0: 302e 3330 3538 3737 2035 2e30 3234 3531  0.305877 5.02451
-000084d0: 3231 2c32 302e 3832 3039 3120 4320 352e  21,20.82091 C 5.
-000084e0: 3230 3231 3834 312c 3231 2e33 3034 3332  2021841,21.30432
-000084f0: 3520 352e 3437 3235 3732 342c 3231 2e37  5 5.4725724,21.7
-00008500: 3532 3133 3820 352e 3831 3030 3439 332c  52138 5.8100493,
-00008510: 3232 2e31 3430 3634 3420 4320 362e 3035  22.140644 C 6.05
-00008520: 3436 3830 362c 3232 2e34 3233 3437 3720  46806,22.423477 
-00008530: 362e 3333 3437 3533 322c 3232 2e36 3735  6.3347532,22.675
-00008540: 3738 3720 362e 3634 3138 3238 312c 3232  787 6.6418281,22
-00008550: 2e38 3839 3138 3820 4320 372e 3034 3030  .889188 C 7.0400
-00008560: 3237 372c 3233 2e31 3635 3934 3120 372e  277,23.165941 7.
-00008570: 3438 3837 3033 362c 3233 2e33 3639 3831  4887036,23.36981
-00008580: 3320 372e 3935 3935 3330 312c 3233 2e34  3 7.9595301,23.4
-00008590: 3836 3037 3920 4320 382e 3432 3330 3437  86079 C 8.423047
-000085a0: 342c 3233 2e36 3031 3135 3120 382e 3930  4,23.601151 8.90
-000085b0: 3439 3937 312c 3233 2e36 3335 3438 3720  49971,23.635487 
-000085c0: 392e 3338 3039 3632 2c32 332e 3630 3335  9.380962,23.6035
-000085d0: 3634 2043 2039 2e38 3637 3135 3639 2c32  64 C 9.8671569,2
-000085e0: 332e 3537 3033 3038 2031 302e 3334 3838  3.570308 10.3488
-000085f0: 3132 2c32 332e 3435 3435 3634 2031 302e  12,23.454564 10.
-00008600: 3739 3233 3232 2c32 332e 3235 3133 3520  792322,23.25135 
-00008610: 4320 3131 2e32 3539 3330 392c 3233 2e30  C 11.259309,23.0
-00008620: 3339 3031 3820 3131 2e36 3830 3335 332c  39018 11.680353,
-00008630: 3232 2e37 3332 3930 3120 3132 2e30 3433  22.732901 12.043
-00008640: 3337 362c 3232 2e33 3731 3733 3120 4320  376,22.371731 C 
-00008650: 3132 2e34 3135 3734 382c 3232 2e30 3033  12.415748,22.003
-00008660: 3336 3420 3132 2e37 3239 3536 332c 3231  364 12.729563,21
-00008670: 2e35 3733 3136 3820 3132 2e39 3439 3136  .573168 12.94916
-00008680: 2c32 312e 3039 3637 3438 2043 2031 332e  ,21.096748 C 13.
-00008690: 3136 3631 3336 2c32 302e 3632 3934 3535  166136,20.629455
-000086a0: 2031 332e 3239 3031 3534 2c32 302e 3132   13.290154,20.12
-000086b0: 3132 3138 2031 332e 3332 3830 3635 2c31  1218 13.328065,1
-000086c0: 392e 3630 3739 3838 2043 2031 332e 3335  9.607988 C 13.35
-000086d0: 3931 312c 3139 2e31 3830 3430 3120 3133  911,19.180401 13
-000086e0: 2e33 3339 3434 342c 3138 2e37 3438 3337  .339444,18.74837
-000086f0: 3720 3133 2e32 3631 3038 332c 3138 2e33  7 13.261083,18.3
-00008700: 3236 3634 3420 4320 3133 2e31 3639 3533  26644 C 13.16953
-00008710: 332c 3137 2e38 3332 3433 3920 3132 2e39  3,17.832439 12.9
-00008720: 3930 3634 322c 3137 2e33 3534 3120 3132  90642,17.3541 12
-00008730: 2e37 3330 3431 342c 3136 2e39 3233 3836  .730414,16.92386
-00008740: 3320 4320 3132 2e35 3436 3730 352c 3136  3 C 12.546705,16
-00008750: 2e36 3139 3232 3620 3132 2e33 3234 3833  .619226 12.32483
-00008760: 342c 3136 2e33 3337 3937 2031 322e 3037  4,16.33797 12.07
-00008770: 3438 2c31 362e 3038 3531 3234 2043 2031  48,16.085124 C 1
-00008780: 312e 3730 3735 3031 2c31 352e 3732 3037  1.707501,15.7207
-00008790: 3635 2031 312e 3238 3036 3135 2c31 352e  65 11.280615,15.
-000087a0: 3431 3335 3033 2031 302e 3830 3831 3037  413503 10.808107
-000087b0: 2c31 352e 3230 3037 3420 4320 3130 2e33  ,15.20074 C 10.3
-000087c0: 3533 3836 332c 3134 2e39 3934 3631 3520  53863,14.994615 
-000087d0: 392e 3836 3130 3037 372c 3134 2e38 3738  9.8610077,14.878
-000087e0: 3332 3520 392e 3336 3338 3933 372c 3134  325 9.3638937,14
-000087f0: 2e38 3434 3934 3920 4320 382e 3831 3930  .844949 C 8.8190
-00008800: 3131 382c 3134 2e38 3038 3036 3620 382e  118,14.808066 8.
-00008810: 3236 3531 3436 342c 3134 2e38 3538 3533  2651464,14.85853
-00008820: 3420 372e 3734 3239 3637 392c 3135 2e30  4 7.7429679,15.0
-00008830: 3232 3633 3420 4320 372e 3238 3031 3432  22634 C 7.280142
-00008840: 312c 3135 2e31 3636 3638 2036 2e38 3436  1,15.16668 6.846
-00008850: 3730 3238 2c31 352e 3430 3030 3039 2036  7028,15.400009 6
-00008860: 2e34 3635 3037 3337 2c31 352e 3639 3832  .4650737,15.6982
-00008870: 3133 2043 2036 2e30 3538 3638 3638 2c31  13 C 6.0586868,1
-00008880: 362e 3031 3533 3239 2035 2e37 3033 3831  6.015329 5.70381
-00008890: 3632 2c31 362e 3339 3931 3734 2035 2e34  62,16.399174 5.4
-000088a0: 3233 3531 3835 2c31 362e 3833 3230 3235  235185,16.832025
-000088b0: 2043 2035 2e31 3533 3134 3839 2c31 372e   C 5.1531489,17.
-000088c0: 3234 3932 3333 2034 2e39 3539 3239 3832  249233 4.9592982
-000088d0: 2c31 372e 3731 3536 3331 2034 2e38 3533  ,17.715631 4.853
-000088e0: 3936 3239 2c31 382e 3230 3135 3131 2043  9629,18.201511 C
-000088f0: 2034 2e37 3831 3739 3533 2c31 382e 3533   4.7817953,18.53
-00008900: 3133 3536 2034 2e37 3438 3935 3035 2c31  1356 4.7489505,1
-00008910: 382e 3836 3932 3838 2034 2e37 3439 3032  8.869288 4.74902
-00008920: 3735 2c31 392e 3230 3637 3639 207a 2022  75,19.206769 z "
-00008930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008940: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-00008950: 6669 6c6c 3a20 247a 6f64 6961 635f 636f  fill: $zodiac_co
-00008960: 6c6f 725f 3422 0a20 2020 2020 2020 2020  lor_4".         
-00008970: 2020 2020 2020 2020 2020 202f 3e0a 2020             />.  
-00008980: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00008990: 7379 6d62 6f6c 3e0a 2020 2020 2020 2020  symbol>.        
-000089a0: 2020 2020 2020 2020 3c73 796d 626f 6c20          <symbol 
-000089b0: 6964 3d22 7669 7267 6f22 3e0a 2020 2020  id="virgo">.    
-000089c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089d0: 3c70 6174 680a 2020 2020 2020 2020 2020  <path.          
-000089e0: 2020 2020 2020 2020 2020 2020 2020 643d                d=
-000089f0: 224d 2037 2e31 3633 3238 3535 2c39 2e37  "M 7.1632855,9.7
-00008a00: 3438 3833 3633 2043 2037 2e31 3633 3238  488363 C 7.16328
-00008a10: 3535 2c31 342e 3934 3938 3639 2037 2e31  55,14.949869 7.1
-00008a20: 3633 3238 3535 2c32 302e 3135 3039 3033  632855,20.150903
-00008a30: 2037 2e31 3633 3238 3535 2c32 352e 3335   7.1632855,25.35
-00008a40: 3139 3336 2043 2036 2e33 3331 3035 3435  1936 C 6.3310545
-00008a50: 2c32 352e 3335 3139 3336 2035 2e34 3938  ,25.351936 5.498
-00008a60: 3832 3335 2c32 352e 3335 3139 3336 2034  8235,25.351936 4
-00008a70: 2e36 3636 3539 3235 2c32 352e 3335 3139  .6665925,25.3519
-00008a80: 3336 2043 2034 2e36 3636 3539 3235 2c31  36 C 4.6665925,1
-00008a90: 392e 3332 3831 3634 2034 2e36 3636 3539  9.328164 4.66659
-00008aa0: 3235 2c31 332e 3330 3433 3932 2034 2e36  25,13.304392 4.6
-00008ab0: 3636 3539 3235 2c37 2e32 3830 3631 3938  665925,7.2806198
-00008ac0: 2043 2034 2e36 3637 3334 3235 2c36 2e31   C 4.6673425,6.1
-00008ad0: 3035 3832 3636 2034 2e35 3133 3738 3235  058266 4.5137825
-00008ae0: 2c34 2e39 3238 3932 3837 2034 2e31 3835  ,4.9289287 4.185
-00008af0: 3733 3435 2c33 2e37 3939 3838 3220 4320  7345,3.799882 C 
-00008b00: 332e 3837 3138 3739 352c 322e 3731 3339  3.8718795,2.7139
-00008b10: 3830 3720 332e 3339 3638 3936 352c 312e  807 3.3968965,1.
-00008b20: 3637 3537 3630 3620 322e 3738 3934 3134  6757606 2.789414
-00008b30: 392c 302e 3732 3234 3935 3435 2043 2032  9,0.72249545 C 2
-00008b40: 2e37 3334 3830 3037 2c30 2e36 3334 3436  .7348007,0.63446
-00008b50: 3537 2032 2e36 3730 3632 3537 2c30 2e35  57 2.6706257,0.5
-00008b60: 3432 3635 3931 3920 322e 3631 3931 3239  4265919 2.619129
-00008b70: 332c 302e 3435 3839 3134 3720 4320 332e  3,0.4589147 C 3.
-00008b80: 3439 3632 3138 352c 302e 3435 3839 3134  4962185,0.458914
-00008b90: 3720 342e 3337 3333 3036 352c 302e 3435  7 4.3733065,0.45
-00008ba0: 3839 3134 3720 352e 3235 3033 3936 352c  89147 5.2503965,
-00008bb0: 302e 3435 3839 3134 3720 4320 352e 3739  0.4589147 C 5.79
-00008bc0: 3831 3936 352c 312e 3230 3939 3638 3320  81965,1.2099683 
-00008bd0: 362e 3231 3339 3734 352c 322e 3035 3039  6.2139745,2.0509
-00008be0: 3539 3320 362e 3532 3735 3931 352c 322e  593 6.5275915,2.
-00008bf0: 3932 3430 3037 3320 4320 362e 3831 3431  9240073 C 6.8141
-00008c00: 3637 352c 332e 3732 3230 3834 3820 372e  675,3.7220848 7.
-00008c10: 3031 3737 3134 352c 342e 3534 3832 3134  0177145,4.548214
-00008c20: 3320 372e 3136 3332 3835 352c 352e 3338  3 7.1632855,5.38
-00008c30: 3239 3435 3520 4320 372e 3630 3731 3434  29455 C 7.607144
-00008c40: 352c 342e 3239 3539 3631 3320 382e 3132  5,4.2959613 8.12
-00008c50: 3333 3637 352c 332e 3233 3535 3036 3220  33675,3.2355062 
-00008c60: 382e 3735 3131 3336 352c 322e 3234 3138  8.7511365,2.2418
-00008c70: 3430 3520 4320 392e 3134 3933 3936 352c  405 C 9.1493965,
-00008c80: 312e 3631 3234 3630 3120 392e 3539 3332  1.6124601 9.5932
-00008c90: 3737 352c 312e 3031 3034 3538 3320 3130  775,1.0104583 10
-00008ca0: 2e30 3934 3732 372c 302e 3435 3839 3134  .094727,0.458914
-00008cb0: 3720 4320 3130 2e39 3130 3339 362c 302e  7 C 10.910396,0.
-00008cc0: 3330 3539 3433 3535 2031 312e 3732 3630  30594355 11.7260
-00008cd0: 3635 2c30 2e31 3532 3937 3131 3620 3132  65,0.15297116 12
-00008ce0: 2e35 3431 3733 342c 342e 3434 3038 3932  .541734,4.440892
-00008cf0: 3165 2d31 3520 4320 3133 2e31 3135 3432  1e-15 C 13.11542
-00008d00: 382c 302e 3733 3736 3233 3535 2031 332e  8,0.73762355 13.
-00008d10: 3535 3638 3538 2c31 2e35 3732 3038 3933  556858,1.5720893
-00008d20: 2031 332e 3838 3631 3239 2c32 2e34 3434   13.886129,2.444
-00008d30: 3637 3039 2043 2031 342e 3237 3135 3935  6709 C 14.271595
-00008d40: 2c33 2e34 3636 3033 3532 2031 342e 3530  ,3.4660352 14.50
-00008d50: 3931 362c 342e 3533 3832 3734 3520 3134  916,4.5382745 14
-00008d60: 2e36 3531 3531 322c 352e 3631 3839 3439  .651512,5.618949
-00008d70: 3220 4320 3134 2e36 3536 3338 332c 352e  2 C 14.656383,5.
-00008d80: 3635 3630 3239 3520 3134 2e36 3631 3134  6560295 14.66114
-00008d90: 312c 352e 3639 3331 3233 3420 3134 2e36  1,5.6931234 14.6
-00008da0: 3635 3738 362c 352e 3733 3032 3332 3320  65786,5.7302323 
-00008db0: 4320 3135 2e30 3338 3839 332c 342e 3535  C 15.038893,4.55
-00008dc0: 3438 3634 3920 3135 2e35 3930 3537 312c  48649 15.590571,
-00008dd0: 332e 3434 3034 3139 3120 3136 2e32 3538  3.4404191 16.258
-00008de0: 3132 322c 322e 3430 3437 3732 3620 4320  122,2.4047726 C 
-00008df0: 3136 2e36 3936 3633 362c 312e 3732 3431  16.696636,1.7241
-00008e00: 3237 3720 3137 2e31 3835 3030 342c 312e  277 17.185004,1.
-00008e10: 3037 3631 3136 3620 3137 2e37 3039 3031  0761166 17.70901
-00008e20: 392c 302e 3435 3839 3134 3720 4320 3138  9,0.4589147 C 18
-00008e30: 2e35 3132 3236 372c 302e 3330 3539 3433  .512267,0.305943
-00008e40: 3535 2031 392e 3331 3535 3134 2c30 2e31  55 19.315514,0.1
-00008e50: 3532 3937 3131 3620 3230 2e31 3138 3736  5297116 20.11876
-00008e60: 322c 342e 3434 3038 3932 3165 2d31 3520  2,4.4408921e-15 
-00008e70: 4320 3230 2e37 3236 3535 392c 302e 3833  C 20.726559,0.83
-00008e80: 3934 3536 3635 2032 312e 3232 3238 3736  945665 21.222876
-00008e90: 2c31 2e37 3631 3736 3132 2032 312e 3536  ,1.7617612 21.56
-00008ea0: 3532 3435 2c32 2e37 3430 3431 3534 2043  5245,2.7404154 C
-00008eb0: 2032 312e 3839 3831 3634 2c33 2e36 3837   21.898164,3.687
-00008ec0: 3230 3335 2032 322e 3038 3530 3536 2c34  2035 22.085056,4
-00008ed0: 2e36 3833 3633 3339 2032 322e 3133 3131  .6836339 22.1311
-00008ee0: 3537 2c35 2e36 3835 3630 3936 2043 2032  57,5.6856096 C 2
-00008ef0: 322e 3134 3336 3038 2c35 2e39 3237 3033  2.143608,5.92703
-00008f00: 3620 3232 2e31 3433 3639 362c 362e 3136  6 22.143696,6.16
-00008f10: 3837 3837 3320 3232 2e31 3433 3434 342c  87873 22.143444,
-00008f20: 362e 3431 3034 3534 3220 4320 3232 2e31  6.4104542 C 22.1
-00008f30: 3433 3434 342c 372e 3932 3432 3832 3320  43444,7.9242823 
-00008f40: 3232 2e31 3433 3434 342c 392e 3433 3831  22.143444,9.4381
-00008f50: 3039 3220 3232 2e31 3433 3434 342c 3130  092 22.143444,10
-00008f60: 2e39 3531 3933 3720 4320 3232 2e34 3831  .951937 C 22.481
-00008f70: 3334 392c 392e 3939 3830 3235 3320 3232  349,9.9980253 22
-00008f80: 2e38 3538 3939 322c 392e 3035 3636 3737  .858992,9.056677
-00008f90: 3920 3233 2e33 3039 3635 392c 382e 3134  9 23.309659,8.14
-00008fa0: 3938 3635 2043 2032 332e 3539 3633 342c  9865 C 23.59634,
-00008fb0: 372e 3537 3533 3431 2032 332e 3931 3233  7.575341 23.9123
-00008fc0: 3236 2c37 2e30 3133 3937 3739 2032 342e  26,7.0139779 24.
-00008fd0: 3237 3939 3137 2c36 2e34 3836 3832 3134  279917,6.4868214
-00008fe0: 2043 2032 342e 3936 3732 3332 2c36 2e32   C 24.967232,6.2
-00008ff0: 3334 3632 3534 2032 352e 3635 3435 3438  346254 25.654548
-00009000: 2c35 2e39 3832 3432 3832 2032 362e 3334  ,5.9824282 26.34
-00009010: 3138 3633 2c35 2e37 3330 3233 3233 2043  1863,5.7302323 C
-00009020: 2032 372e 3134 3634 3431 2c36 2e39 3730   27.146441,6.970
-00009030: 3637 3632 2032 372e 3830 3637 3537 2c38  6762 27.806757,8
-00009040: 2e33 3038 3039 3838 2032 382e 3236 3234  .3080988 28.2624
-00009050: 3532 2c39 2e37 3135 3434 3735 2043 2032  52,9.7154475 C 2
-00009060: 382e 3637 3930 3231 2c31 302e 3939 3731  8.679021,10.9971
-00009070: 3238 2032 382e 3932 3330 3137 2c31 322e  28 28.923017,12.
-00009080: 3333 3436 3235 2032 382e 3938 3338 3739  334625 28.983879
-00009090: 2c31 332e 3638 3037 3938 2043 2032 392e  ,13.680798 C 29.
-000090a0: 3034 3939 3936 2c31 352e 3135 3138 3620  049996,15.15186 
-000090b0: 3238 2e39 3133 3737 2c31 362e 3633 3339  28.91377,16.6339
-000090c0: 3736 2032 382e 3535 3632 3534 2c31 382e  76 28.556254,18.
-000090d0: 3036 3334 3031 2043 2032 382e 3135 3936  063401 C 28.1596
-000090e0: 3435 2c31 392e 3635 3437 3937 2032 372e  45,19.654797 27.
-000090f0: 3439 3132 3738 2c32 312e 3137 3536 3620  491278,21.17566 
-00009100: 3236 2e36 3038 3734 362c 3232 2e35 3537  26.608746,22.557
-00009110: 3634 3920 4320 3235 2e37 3936 3539 352c  649 C 25.796595,
-00009120: 3233 2e38 3331 3637 3220 3234 2e38 3131  23.831672 24.811
-00009130: 3934 2c32 342e 3939 3035 3332 2032 332e  94,24.990532 23.
-00009140: 3732 3930 3533 2c32 362e 3034 3236 3231  729053,26.042621
-00009150: 2043 2032 332e 3337 3632 3135 2c32 362e   C 23.376215,26.
-00009160: 3338 3534 3338 2032 332e 3031 3236 3738  385438 23.012678
-00009170: 2c32 362e 3731 3732 3238 2032 322e 3634  ,26.717228 22.64
-00009180: 3032 3938 2c32 372e 3033 3837 3538 2043  0298,27.038758 C
-00009190: 2032 322e 3733 3039 3036 2c32 372e 3730   22.730906,27.70
-000091a0: 3332 3239 2032 322e 3934 3638 3131 2c32  3229 22.946811,2
-000091b0: 382e 3334 3532 3820 3233 2e32 3235 3738  8.34528 23.22578
-000091c0: 312c 3238 2e39 3533 3335 3420 4320 3233  1,28.953354 C 23
-000091d0: 2e35 3733 3039 2c32 392e 3730 3735 3631  .57309,29.707561
-000091e0: 2032 342e 3031 3636 3931 2c33 302e 3431   24.016691,30.41
-000091f0: 3339 3938 2032 342e 3530 3336 3139 2c33  3998 24.503619,3
-00009200: 312e 3038 3534 3836 2043 2032 342e 3733  1.085486 C 24.73
-00009210: 3032 3139 2c33 312e 3339 3734 3037 2032  0219,31.397407 2
-00009220: 342e 3936 3730 3539 2c33 312e 3730 3138  4.967059,31.7018
-00009230: 3438 2032 352e 3231 3135 3139 2c33 312e  48 25.211519,31.
-00009240: 3939 3939 3938 2043 2032 342e 3233 3433  999998 C 24.2343
-00009250: 3732 2c33 312e 3939 3939 3938 2032 332e  72,31.999998 23.
-00009260: 3235 3732 3236 2c33 312e 3939 3939 3938  257226,31.999998
-00009270: 2032 322e 3238 3030 3739 2c33 312e 3939   22.280079,31.99
-00009280: 3939 3938 2043 2032 312e 3831 3537 3136  9998 C 21.815716
-00009290: 2c33 312e 3431 3332 3138 2032 312e 3433  ,31.413218 21.43
-000092a0: 3233 3638 2c33 302e 3736 3633 3137 2032  2368,30.766317 2
-000092b0: 312e 3130 3033 3435 2c33 302e 3039 3730  1.100345,30.0970
-000092c0: 3731 2043 2032 302e 3833 3337 3436 2c32  71 C 20.833746,2
-000092d0: 392e 3535 3834 3535 2032 302e 3630 3037  9.558455 20.6007
-000092e0: 3536 2c32 392e 3030 3336 3733 2032 302e  56,29.003673 20.
-000092f0: 3339 3230 3332 2c32 382e 3434 3033 3038  392032,28.440308
-00009300: 2043 2031 392e 3339 3634 3232 2c32 392e   C 19.396422,29.
-00009310: 3030 3436 3338 2031 382e 3332 3333 3931  004638 18.323391
-00009320: 2c32 392e 3432 3338 3239 2031 372e 3232  ,29.423829 17.22
-00009330: 3437 3932 2c32 392e 3734 3031 3233 2043  4792,29.740123 C
-00009340: 2031 362e 3338 3439 3731 2c32 392e 3938   16.384971,29.98
-00009350: 3136 3038 2031 352e 3532 3836 312c 3330  1608 15.52861,30
-00009360: 2e31 3633 3338 3520 3134 2e36 3635 3738  .163385 14.66578
-00009370: 362c 3330 2e33 3030 3737 3320 4320 3134  6,30.300773 C 14
-00009380: 2e36 3635 3738 362c 3239 2e35 3839 3636  .665786,29.58966
-00009390: 3220 3134 2e36 3635 3738 362c 3238 2e38  2 14.665786,28.8
-000093a0: 3738 3535 3120 3134 2e36 3635 3738 362c  78551 14.665786,
-000093b0: 3238 2e31 3637 3434 2043 2031 352e 3831  28.16744 C 15.81
-000093c0: 3235 3032 2c32 372e 3933 3338 3831 2031  2502,27.933881 1
-000093d0: 362e 3934 3636 3031 2c32 372e 3632 3534  6.946601,27.6254
-000093e0: 3236 2031 382e 3033 3635 3639 2c32 372e  26 18.036569,27.
-000093f0: 3139 3732 3331 2043 2031 382e 3638 3134  197231 C 18.6814
-00009400: 3833 2c32 362e 3934 3333 3539 2031 392e  83,26.943359 19.
-00009410: 3331 3034 3632 2c32 362e 3634 3637 3833  310462,26.646783
-00009420: 2031 392e 3930 3735 3939 2c32 362e 3239   19.907599,26.29
-00009430: 3435 3732 2043 2031 392e 3733 3037 3337  4572 C 19.730737
-00009440: 2c32 352e 3139 3936 3120 3139 2e36 3433  ,25.19961 19.643
-00009450: 3233 322c 3234 2e30 3930 3239 2031 392e  232,24.09029 19.
-00009460: 3634 3637 3531 2c32 322e 3938 3131 3734  646751,22.981174
-00009470: 2043 2031 392e 3634 3637 342c 3137 2e39   C 19.64674,17.9
-00009480: 3438 3837 3720 3139 2e36 3436 3737 322c  48877 19.646772,
-00009490: 3132 2e39 3136 3537 3820 3139 2e36 3436  12.916578 19.646
-000094a0: 3733 352c 372e 3838 3432 3831 3120 4320  735,7.8842811 C 
-000094b0: 3139 2e36 3434 3935 312c 362e 3935 3032  19.644951,6.9502
-000094c0: 3032 3420 3139 2e35 3937 3032 362c 362e  024 19.597026,6.
-000094d0: 3031 3431 3238 2031 392e 3435 3536 3737  014128 19.455677
-000094e0: 2c35 2e30 3839 3939 3636 2043 2031 392e  ,5.0899966 C 19.
-000094f0: 3334 3835 3232 2c34 2e33 3938 3235 3731  348522,4.3982571
-00009500: 2031 392e 3138 3839 3536 2c33 2e37 3131   19.188956,3.711
-00009510: 3234 3720 3138 2e39 3330 3932 342c 332e  247 18.930924,3.
-00009520: 3035 3930 3935 3720 4320 3138 2e38 3330  0590957 C 18.830
-00009530: 3037 362c 322e 3830 3530 3935 3120 3138  076,2.8050951 18
-00009540: 2e37 3133 3739 382c 322e 3535 3639 3733  .713798,2.556973
-00009550: 3520 3138 2e35 3738 3531 342c 322e 3331  5 18.578514,2.31
-00009560: 3933 3739 3820 4320 3137 2e37 3338 3937  93798 C 17.73897
-00009570: 372c 332e 3232 3234 3536 3920 3137 2e30  7,3.2224569 17.0
-00009580: 3437 3935 392c 342e 3235 3538 3334 3820  47959,4.2558348 
-00009590: 3136 2e34 3739 3730 362c 352e 3334 3735  16.479706,5.3475
-000095a0: 3934 3120 4320 3135 2e38 3234 3432 392c  941 C 15.824429,
-000095b0: 362e 3630 3734 3837 3420 3135 2e33 3237  6.6074874 15.327
-000095c0: 3634 372c 372e 3934 3437 3739 3720 3134  647,7.9447797 14
-000095d0: 2e39 3337 3336 332c 392e 3330 3834 3138  .937363,9.308418
-000095e0: 3720 4320 3134 2e38 3430 3439 392c 392e  7 C 14.840499,9.
-000095f0: 3634 3834 3833 3220 3134 2e37 3439 3034  6484832 14.74904
-00009600: 392c 392e 3939 3032 3934 3320 3134 2e36  9,9.9902943 14.6
-00009610: 3635 3738 362c 3130 2e33 3333 3834 2043  65786,10.33384 C
-00009620: 2031 342e 3636 3537 3836 2c31 352e 3333   14.665786,15.33
-00009630: 3938 3732 2031 342e 3636 3537 3836 2c32  9872 14.665786,2
-00009640: 302e 3334 3539 3034 2031 342e 3636 3537  0.345904 14.6657
-00009650: 3836 2c32 352e 3335 3139 3336 2043 2031  86,25.351936 C 1
-00009660: 332e 3832 3934 3135 2c32 352e 3335 3139  3.829415,25.3519
-00009670: 3336 2031 322e 3939 3330 3433 2c32 352e  36 12.993043,25.
-00009680: 3335 3139 3336 2031 322e 3135 3636 3732  351936 12.156672
-00009690: 2c32 352e 3335 3139 3336 2043 2031 322e  ,25.351936 C 12.
-000096a0: 3135 3636 3631 2c31 392e 3830 3831 3034  156661,19.808104
-000096b0: 2031 322e 3135 3636 3934 2c31 342e 3236   12.156694,14.26
-000096c0: 3432 3732 2031 322e 3135 3636 3535 2c38  4272 12.156655,8
-000096d0: 2e37 3230 3433 3938 2043 2031 322e 3135  .7204398 C 12.15
-000096e0: 3438 3636 2c37 2e36 3935 3936 3336 2031  4866,7.6959636 1
-000096f0: 322e 3131 3630 3635 2c36 2e36 3730 3132  2.116065,6.67012
-00009700: 3433 2031 312e 3939 3735 3233 2c35 2e36  43 11.997523,5.6
-00009710: 3531 3938 3131 2043 2031 312e 3931 3631  519811 C 11.9161
-00009720: 3631 2c34 2e39 3636 3532 3633 2031 312e  61,4.9665263 11.
-00009730: 3739 3939 3538 2c34 2e32 3833 3033 3938  799958,4.2830398
-00009740: 2031 312e 3630 3636 3131 2c33 2e36 3139   11.606611,3.619
-00009750: 3531 3336 2043 2031 312e 3437 3336 3433  5136 C 11.473643
-00009760: 2c33 2e31 3638 3438 3938 2031 312e 3330  ,3.1684898 11.30
-00009770: 3530 3338 2c32 2e37 3234 3436 3837 2031  5038,2.7244687 1
-00009780: 312e 3036 3335 3932 2c32 2e33 3139 3337  1.063592,2.31937
-00009790: 3938 2043 2031 302e 3130 3134 3034 2c33  98 C 10.101404,3
-000097a0: 2e34 3338 3036 3939 2039 2e32 3932 3138  .4380699 9.29218
-000097b0: 3035 2c34 2e36 3834 3236 3339 2038 2e36  05,4.6842639 8.6
-000097c0: 3331 3730 3735 2c36 2e30 3032 3220 4320  317075,6.0022 C 
-000097d0: 382e 3032 3932 3034 352c 372e 3230 3330  8.0292045,7.2030
-000097e0: 3433 3320 372e 3534 3736 3131 352c 382e  433 7.5476115,8.
-000097f0: 3436 3233 3732 3220 372e 3136 3332 3835  4623722 7.163285
-00009800: 352c 392e 3734 3838 3336 3320 7a20 4d20  5,9.7488363 z M 
-00009810: 3232 2e31 3433 3434 342c 3234 2e37 3036  22.143444,24.706
-00009820: 3937 3520 4320 3233 2e30 3736 3231 312c  975 C 23.076211,
-00009830: 3233 2e37 3630 3437 3220 3233 2e39 3039  23.760472 23.909
-00009840: 3835 392c 3232 2e37 3132 3631 3420 3234  859,22.712614 24
-00009850: 2e35 3837 3631 382c 3231 2e35 3638 3833  .587618,21.56883
-00009860: 3820 4320 3234 2e39 3134 3737 312c 3231  8 C 24.914771,21
-00009870: 2e30 3136 3635 3320 3235 2e32 3036 3835  .016653 25.20685
-00009880: 312c 3230 2e34 3433 3432 3920 3235 2e34  1,20.443429 25.4
-00009890: 3536 3138 392c 3139 2e38 3532 3034 3820  56189,19.852048 
-000098a0: 4320 3235 2e39 3239 3438 392c 3138 2e37  C 25.929489,18.7
-000098b0: 3137 3539 3420 3236 2e32 3434 3831 372c  17594 26.244817,
-000098c0: 3137 2e35 3138 3039 3620 3236 2e33 3935  17.518096 26.395
-000098d0: 3135 332c 3136 2e32 3938 3437 3620 4320  153,16.298476 C 
-000098e0: 3236 2e34 3931 3439 322c 3135 2e35 3136  26.491492,15.516
-000098f0: 3937 3120 3236 2e35 3233 3630 332c 3134  971 26.523603,14
-00009900: 2e37 3237 3530 3120 3236 2e34 3930 3930  .727501 26.49090
-00009910: 322c 3133 2e39 3430 3737 3520 4320 3236  2,13.940775 C 26
-00009920: 2e34 3430 3939 362c 3132 2e37 3536 3135  .440996,12.75615
-00009930: 3920 3236 2e32 3331 3232 372c 3131 2e35  9 26.231227,11.5
-00009940: 3738 3830 3220 3235 2e38 3732 3739 332c  78802 25.872793,
-00009950: 3130 2e34 3438 3537 2043 2032 352e 3638  10.44857 C 25.68
-00009960: 3630 3836 2c39 2e38 3538 3338 3833 2032  6086,9.8583883 2
-00009970: 352e 3435 3938 3034 2c39 2e32 3830 3834  5.459804,9.28084
-00009980: 3431 2032 352e 3139 3930 3938 2c38 2e37  41 25.199098,8.7
-00009990: 3139 3337 3934 2043 2032 342e 3530 3432  193794 C 24.5042
-000099a0: 3332 2c39 2e35 3733 3339 3620 3233 2e39  32,9.573396 23.9
-000099b0: 3333 3132 362c 3130 2e35 3232 3039 3920  33126,10.522099 
-000099c0: 3233 2e34 3438 3939 312c 3131 2e35 3038  23.448991,11.508
-000099d0: 3931 3420 4320 3232 2e39 3236 3238 392c  914 C 22.926289,
-000099e0: 3132 2e35 3736 3234 3520 3232 2e35 3033  12.576245 22.503
-000099f0: 3237 372c 3133 2e36 3839 3935 3720 3232  277,13.689957 22
-00009a00: 2e31 3433 3434 342c 3134 2e38 3231 3730  .143444,14.82170
-00009a10: 3420 4320 3232 2e31 3433 3434 342c 3138  4 C 22.143444,18
-00009a20: 2e31 3136 3739 3520 3232 2e31 3433 3434  .116795 22.14344
-00009a30: 342c 3231 2e34 3131 3838 3420 3232 2e31  4,21.411884 22.1
-00009a40: 3433 3434 342c 3234 2e37 3036 3937 3520  43444,24.706975 
-00009a50: 7a20 220a 2020 2020 2020 2020 2020 2020  z ".            
-00009a60: 2020 2020 2020 2020 2020 2020 7374 796c              styl
-00009a70: 653d 2266 696c 6c3a 2024 7a6f 6469 6163  e="fill: $zodiac
-00009a80: 5f63 6f6c 6f72 5f35 220a 2020 2020 2020  _color_5".      
-00009a90: 2020 2020 2020 2020 2020 2020 2020 2f3e                />
-00009aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009ab0: 203c 2f73 796d 626f 6c3e 0a20 2020 2020   </symbol>.     
-00009ac0: 2020 2020 2020 2020 2020 203c 7379 6d62             <symb
-00009ad0: 6f6c 2069 643d 226c 6962 7261 223e 0a20  ol id="libra">. 
-00009ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009af0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-00009b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b10: 2064 3d22 4d20 2d35 2e35 3936 3235 652d   d="M -5.59625e-
-00009b20: 3036 2c32 392e 3139 3037 3039 2043 202d  06,29.190709 C -
-00009b30: 352e 3539 3632 3565 2d30 362c 3238 2e32  5.59625e-06,28.2
-00009b40: 3033 3732 3220 2d35 2e35 3936 3235 652d  03722 -5.59625e-
-00009b50: 3036 2c32 372e 3231 3637 3335 202d 352e  06,27.216735 -5.
-00009b60: 3539 3632 3565 2d30 362c 3236 2e32 3239  59625e-06,26.229
-00009b70: 3733 3520 4320 3130 2e36 3636 3636 372c  735 C 10.666667,
-00009b80: 3236 2e32 3239 3733 3520 3231 2e33 3333  26.229735 21.333
-00009b90: 3332 372c 3236 2e32 3239 3733 3520 3332  327,26.229735 32
-00009ba0: 2c32 362e 3232 3937 3335 2043 2033 322c  ,26.229735 C 32,
-00009bb0: 3237 2e32 3136 3733 3520 3332 2c32 382e  27.216735 32,28.
-00009bc0: 3230 3337 3232 2033 322c 3239 2e31 3930  203722 32,29.190
-00009bd0: 3730 3920 4320 3231 2e33 3333 3332 372c  709 C 21.333327,
-00009be0: 3239 2e31 3930 3730 3920 3130 2e36 3636  29.190709 10.666
-00009bf0: 3636 372c 3239 2e31 3930 3730 3920 2d35  667,29.190709 -5
-00009c00: 2e35 3936 3235 652d 3036 2c32 392e 3139  .59625e-06,29.19
-00009c10: 3037 3039 207a 204d 2031 322e 3634 3837  0709 z M 12.6487
-00009c20: 352c 3137 2e35 3039 3631 2043 2031 322e  5,17.50961 C 12.
-00009c30: 3634 3837 352c 3138 2e34 3332 3434 3620  64875,18.432446 
-00009c40: 3132 2e36 3438 3735 2c31 392e 3335 3532  12.64875,19.3552
-00009c50: 3833 2031 322e 3634 3837 352c 3230 2e32  83 12.64875,20.2
-00009c60: 3738 3133 3320 4320 382e 3433 3235 3032  78133 C 8.432502
-00009c70: 332c 3230 2e32 3738 3133 3320 342e 3231  3,20.278133 4.21
-00009c80: 3632 3431 382c 3230 2e32 3738 3133 3320  62418,20.278133 
-00009c90: 2d35 2e35 3936 3235 652d 3036 2c32 302e  -5.59625e-06,20.
-00009ca0: 3237 3831 3333 2043 202d 352e 3539 3632  278133 C -5.5962
-00009cb0: 3565 2d30 362c 3139 2e32 3836 3137 3620  5e-06,19.286176 
-00009cc0: 2d35 2e35 3936 3235 652d 3036 2c31 382e  -5.59625e-06,18.
-00009cd0: 3239 3432 3331 202d 352e 3539 3632 3565  294231 -5.59625e
-00009ce0: 2d30 362c 3137 2e33 3032 3238 3620 4320  -06,17.302286 C 
-00009cf0: 322e 3935 3538 3137 2c31 372e 3330 3232  2.955817,17.3022
-00009d00: 3836 2035 2e39 3131 3633 3936 2c31 372e  86 5.9116396,17.
-00009d10: 3330 3232 3836 2038 2e38 3637 3436 3233  302286 8.8674623
-00009d20: 2c31 372e 3330 3232 3836 2043 2037 2e38  ,17.302286 C 7.8
-00009d30: 3333 3030 3139 2c31 362e 3235 3833 3139  330019,16.258319
-00009d40: 2037 2e30 3132 3132 3437 2c31 342e 3937   7.0121247,14.97
-00009d50: 3034 3236 2036 2e36 3632 3531 3731 2c31  0426 6.6625171,1
-00009d60: 332e 3533 3336 3038 2043 2036 2e33 3635  3.533608 C 6.365
-00009d70: 3130 3634 2c31 322e 3333 3537 3732 2036  1064,12.335772 6
-00009d80: 2e33 3939 3338 3239 2c31 312e 3037 3335  .3993829,11.0735
-00009d90: 3338 2036 2e36 3339 3338 3337 2c39 2e38  38 6.6393837,9.8
-00009da0: 3639 3033 3935 2043 2036 2e39 3435 3130  690395 C 6.94510
-00009db0: 3935 2c38 2e33 3535 3736 3136 2037 2e36  95,8.3557616 7.6
-00009dc0: 3932 3338 3939 2c36 2e39 3438 3432 3933  923899,6.9484293
-00009dd0: 2038 2e37 3137 3938 3739 2c35 2e37 3938   8.7179879,5.798
-00009de0: 3932 3033 2043 2039 2e38 3732 3436 3833  9203 C 9.8724683
-00009df0: 2c34 2e34 3932 3237 3632 2031 312e 3334  ,4.4922762 11.34
-00009e00: 3534 3437 2c33 2e34 3339 3339 3537 2031  5447,3.4393957 1
-00009e10: 332e 3031 3636 3535 2c32 2e39 3037 3339  3.016655,2.90739
-00009e20: 3237 2043 2031 342e 3531 3939 3039 2c32  27 C 14.519909,2
-00009e30: 2e34 3235 3136 3133 2031 362e 3134 3030  .4251613 16.1400
-00009e40: 3831 2c32 2e33 3337 3738 3435 2031 372e  81,2.3377845 17.
-00009e50: 3639 3532 3731 2c32 2e35 3839 3436 3631  695271,2.5894661
-00009e60: 2043 2031 392e 3236 3634 3339 2c32 2e38   C 19.266439,2.8
-00009e70: 3435 3237 3236 2032 302e 3735 3631 3133  452726 20.756113
-00009e80: 2c33 2e35 3336 3735 3238 2032 312e 3938  ,3.5367528 21.98
-00009e90: 3631 3332 2c34 2e35 3432 3437 3732 2043  6132,4.5424772 C
-00009ea0: 2032 332e 3238 3639 3938 2c35 2e36 3032   23.286998,5.602
-00009eb0: 3234 3132 2032 342e 3338 3536 3834 2c36  2412 24.385684,6
-00009ec0: 2e39 3531 3531 3332 2032 342e 3938 3632  .9515132 24.9862
-00009ed0: 3031 2c38 2e35 3238 3838 3837 2043 2032  01,8.5288887 C 2
-00009ee0: 352e 3436 3330 3632 2c39 2e37 3732 3635  5.463062,9.77265
-00009ef0: 3739 2032 352e 3634 3031 3237 2c31 312e  79 25.640127,11.
-00009f00: 3132 3633 3934 2032 352e 3533 3335 3537  126394 25.533557
-00009f10: 2c31 322e 3435 3231 3636 2043 2032 352e  ,12.452166 C 25.
-00009f20: 3431 3636 3738 2c31 332e 3832 3033 3434  416678,13.820344
-00009f30: 2032 342e 3837 3839 3237 2c31 352e 3133   24.878927,15.13
-00009f40: 3539 3032 2032 342e 3036 3134 3532 2c31  5902 24.061452,1
-00009f50: 362e 3233 3438 3538 2043 2032 332e 3738  6.234858 C 23.78
-00009f60: 3336 3033 2c31 362e 3631 3235 3131 2032  3603,16.612511 2
-00009f70: 332e 3437 3631 3138 2c31 362e 3936 3830  3.476118,16.9680
-00009f80: 3536 2032 332e 3134 3733 352c 3137 2e33  56 23.14735,17.3
-00009f90: 3032 3331 3320 4320 3236 2e30 3938 3233  02313 C 26.09823
-00009fa0: 332c 3137 2e33 3032 3320 3239 2e30 3439  3,17.3023 29.049
-00009fb0: 3131 362c 3137 2e33 3032 3320 3332 2c31  116,17.3023 32,1
-00009fc0: 372e 3330 3232 3836 2043 2033 322c 3138  7.302286 C 32,18
-00009fd0: 2e32 3934 3233 3120 3332 2c31 392e 3238  .294231 32,19.28
-00009fe0: 3631 3736 2033 322c 3230 2e32 3738 3133  6176 32,20.27813
-00009ff0: 3320 4320 3237 2e37 3833 3733 392c 3230  3 C 27.783739,20
-0000a000: 2e32 3738 3133 3320 3233 2e35 3637 3439  .278133 23.56749
-0000a010: 322c 3230 2e32 3738 3133 3320 3139 2e33  2,20.278133 19.3
-0000a020: 3531 3234 342c 3230 2e32 3738 3133 3320  51244,20.278133 
-0000a030: 4320 3139 2e33 3531 3234 342c 3139 2e33  C 19.351244,19.3
-0000a040: 3535 3238 3320 3139 2e33 3531 3234 342c  55283 19.351244,
-0000a050: 3138 2e34 3332 3434 3620 3139 2e33 3531  18.432446 19.351
-0000a060: 3234 342c 3137 2e35 3039 3631 2043 2032  244,17.50961 C 2
-0000a070: 302e 3437 3634 3739 2c31 362e 3738 3731  0.476479,16.7871
-0000a080: 3939 2032 312e 3436 3938 3436 2c31 352e  99 21.469846,15.
-0000a090: 3830 3334 3133 2032 322e 3032 3831 352c  803413 22.02815,
-0000a0a0: 3134 2e35 3735 3333 3720 4320 3232 2e35  14.575337 C 22.5
-0000a0b0: 3834 3630 332c 3133 2e33 3632 3934 2032  84603,13.36294 2
-0000a0c0: 322e 3730 3638 392c 3131 2e39 3734 3238  2.70689,11.97428
-0000a0d0: 2032 322e 3436 3932 3734 2c31 302e 3636   22.469274,10.66
-0000a0e0: 3839 3736 2043 2032 322e 3233 3937 3532  8976 C 22.239752
-0000a0f0: 2c39 2e34 3137 3630 3736 2032 312e 3537  ,9.4176076 21.57
-0000a100: 3436 3138 2c38 2e32 3731 3337 3736 2032  4618,8.2713776 2
-0000a110: 302e 3637 3134 3531 2c37 2e33 3833 3237  0.671451,7.38327
-0000a120: 3033 2043 2031 392e 3735 3135 3633 2c36  03 C 19.751563,6
-0000a130: 2e34 3532 3430 3520 3138 2e35 3631 3632  .452405 18.56162
-0000a140: 2c35 2e37 3731 3836 3820 3137 2e32 3635  ,5.771868 17.265
-0000a150: 3934 312c 352e 3534 3039 3636 3920 4320  941,5.5409669 C 
-0000a160: 3135 2e37 3238 3234 312c 352e 3236 3434  15.728241,5.2644
-0000a170: 3036 2031 342e 3037 3533 3833 2c35 2e34  06 14.075383,5.4
-0000a180: 3836 3431 3938 2031 322e 3732 3533 372c  864198 12.72537,
-0000a190: 362e 3239 3533 3631 2043 2031 312e 3832  6.295361 C 11.82
-0000a1a0: 3335 3333 2c36 2e38 3335 3630 3037 2031  3533,6.8356007 1
-0000a1b0: 312e 3034 3938 3734 2c37 2e35 3834 3835  1.049874,7.58485
-0000a1c0: 3520 3130 2e34 3538 3534 352c 382e 3435  5 10.458545,8.45
-0000a1d0: 3135 3730 3320 4320 392e 3735 3333 3939  15703 C 9.753399
-0000a1e0: 372c 392e 3438 3734 3137 3920 392e 3430  7,9.4874179 9.40
-0000a1f0: 3737 3431 312c 3130 2e37 3436 3738 3920  77411,10.746789 
-0000a200: 392e 3433 3133 3935 392c 3131 2e39 3935  9.4313959,11.995
-0000a210: 3334 3720 4320 392e 3433 3636 3734 322c  347 C 9.4366742,
-0000a220: 3133 2e31 3938 3837 2039 2e37 3639 3133  13.19887 9.76913
-0000a230: 3034 2c31 342e 3430 3937 3434 2031 302e  04,14.409744 10.
-0000a240: 3434 3730 3234 2c31 352e 3431 3039 3739  447024,15.410979
-0000a250: 2043 2031 312e 3031 3432 3135 2c31 362e   C 11.014215,16.
-0000a260: 3236 3234 3537 2031 312e 3739 3237 3632  262457 11.792762
-0000a270: 2c31 362e 3935 3635 3533 2031 322e 3634  ,16.956553 12.64
-0000a280: 3837 352c 3137 2e35 3039 3631 207a 2022  875,17.50961 z "
-0000a290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a2a0: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-0000a2b0: 6669 6c6c 3a20 247a 6f64 6961 635f 636f  fill: $zodiac_co
-0000a2c0: 6c6f 725f 3622 0a20 2020 2020 2020 2020  lor_6".         
-0000a2d0: 2020 2020 2020 2020 2020 202f 3e0a 2020             />.  
-0000a2e0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-0000a2f0: 7379 6d62 6f6c 3e0a 2020 2020 2020 2020  symbol>.        
-0000a300: 2020 2020 2020 2020 3c73 796d 626f 6c20          <symbol 
-0000a310: 6964 3d22 7363 6f72 7069 6f22 3e0a 2020  id="scorpio">.  
-0000a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a330: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
-0000a340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a350: 643d 224d 2032 2e30 3731 3737 352c 3235  d="M 2.071775,25
-0000a360: 2e31 3039 3339 3220 4320 322e 3037 3137  .109392 C 2.0717
-0000a370: 3534 322c 3139 2e32 3433 3339 3220 322e  542,19.243392 2.
-0000a380: 3037 3138 3136 362c 3133 2e33 3737 3339  0718166,13.37739
-0000a390: 3220 322e 3037 3137 3433 322c 372e 3531  2 2.0717432,7.51
-0000a3a0: 3133 3932 3120 4320 322e 3036 3932 3437  13921 C 2.069247
-0000a3b0: 352c 362e 3334 3332 3236 3520 312e 3935  5,6.3432265 1.95
-0000a3c0: 3833 3939 372c 352e 3137 3036 3932 3220  83997,5.1706922 
-0000a3d0: 312e 3637 3731 3632 312c 342e 3033 3532  1.6771621,4.0352
-0000a3e0: 3632 3620 4320 312e 3433 3733 3139 362c  626 C 1.4373196,
-0000a3f0: 332e 3036 3632 3537 3520 312e 3036 3835  3.0662575 1.0685
-0000a400: 3934 2c32 2e31 3235 3134 3335 2030 2e35  94,2.1251435 0.5
-0000a410: 3435 3338 3034 382c 312e 3237 3336 3937  4538048,1.273697
-0000a420: 3120 4320 302e 3337 3935 3732 3038 2c31  1 C 0.37957208,1
-0000a430: 2e30 3033 3530 3632 2030 2e31 3938 3636  .0035062 0.19866
-0000a440: 3435 382c 302e 3734 3235 3934 2030 2e30  458,0.742594 0.0
-0000a450: 3033 3233 3933 3736 342c 302e 3439 3330  032393764,0.4930
-0000a460: 3635 3120 4320 302e 3838 3435 3038 3938  651 C 0.88450898
-0000a470: 2c30 2e34 3933 3036 3531 2031 2e37 3635  ,0.4930651 1.765
-0000a480: 3737 3836 2c30 2e34 3933 3036 3531 2032  7786,0.4930651 2
-0000a490: 2e36 3437 3034 3833 2c30 2e34 3933 3036  .6470483,0.49306
-0000a4a0: 3531 2043 2033 2e32 3334 3035 3333 2c31  51 C 3.2340533,1
-0000a4b0: 2e33 3839 3439 3331 2033 2e36 3938 3333  .3894931 3.69833
-0000a4c0: 3233 2c32 2e33 3635 3139 3031 2034 2e30  23,2.3651901 4.0
-0000a4d0: 3335 3632 3733 2c33 2e33 3832 3334 3234  356273,3.3823424
-0000a4e0: 2043 2034 2e32 3437 3936 3133 2c34 2e30   C 4.2479613,4.0
-0000a4f0: 3231 3033 3733 2034 2e34 3131 3438 3133  210373 4.4114813
-0000a500: 2c34 2e36 3735 3636 3620 342e 3533 3139  ,4.675666 4.5319
-0000a510: 3836 332c 352e 3333 3738 3333 2043 2035  863,5.337833 C 5
-0000a520: 2e30 3438 3531 3933 2c34 2e30 3630 3139  .0485193,4.06019
-0000a530: 3738 2035 2e36 3834 3634 3933 2c32 2e38  78 5.6846493,2.8
-0000a540: 3236 3833 3839 2036 2e34 3736 3731 3733  268389 6.4767173
-0000a550: 2c31 2e36 3937 3936 3520 4320 362e 3736  ,1.697965 C 6.76
-0000a560: 3939 3339 332c 312e 3238 3031 3036 3920  99393,1.2801069 
-0000a570: 372e 3038 3433 3633 332c 302e 3837 3730  7.0843633,0.8770
-0000a580: 3638 3820 372e 3432 3035 3932 332c 302e  688 7.4205923,0.
-0000a590: 3439 3330 3635 3120 4320 382e 3231 3231  4930651 C 8.2121
-0000a5a0: 3033 332c 302e 3333 3336 3137 3120 392e  033,0.3336171 9.
-0000a5b0: 3030 3336 3133 332c 302e 3137 3431 3639  0036133,0.174169
-0000a5c0: 2039 2e37 3935 3132 3433 2c30 2e30 3134   9.7951243,0.014
-0000a5d0: 3732 3130 3033 2043 2031 302e 3332 3138  721003 C 10.3218
-0000a5e0: 2c30 2e36 3239 3035 3834 2031 302e 3732  ,0.6290584 10.72
-0000a5f0: 3739 372c 312e 3334 3030 3030 3520 3131  797,1.3400005 11
-0000a600: 2e30 3337 3731 342c 322e 3038 3631 3538  .037714,2.086158
-0000a610: 3520 4320 3131 2e34 3031 3335 382c 322e  5 C 11.401358,2.
-0000a620: 3936 3239 3235 3320 3131 2e36 3338 3033  9629253 11.63803
-0000a630: 392c 332e 3838 3830 3031 3220 3131 2e37  9,3.8880012 11.7
-0000a640: 3938 3132 352c 342e 3832 3233 3935 2043  98125,4.822395 C
-0000a650: 2031 312e 3834 3139 3732 2c35 2e30 3739   11.841972,5.079
-0000a660: 3137 3633 2031 312e 3837 3938 3837 2c35  1763 11.879887,5
-0000a670: 2e33 3336 3936 3538 2031 312e 3931 3236  .3369658 11.9126
-0000a680: 3139 2c35 2e35 3935 3430 3239 2043 2031  19,5.5954029 C 1
-0000a690: 322e 3334 3038 3231 2c34 2e33 3630 3233  2.340821,4.36023
-0000a6a0: 3938 2031 322e 3935 3035 342c 332e 3139  98 12.95054,3.19
-0000a6b0: 3239 3637 3220 3133 2e36 3734 3534 332c  29672 13.674543,
-0000a6c0: 322e 3130 3639 3030 3220 4320 3134 2e30  2.1069002 C 14.0
-0000a6d0: 3436 3534 2c31 2e35 3438 3733 3736 2031  4654,1.5487376 1
-0000a6e0: 342e 3434 3839 3137 2c31 2e30 3131 3133  4.448917,1.01113
-0000a6f0: 3736 2031 342e 3837 3436 3634 2c30 2e34  76 14.874664,0.4
-0000a700: 3933 3036 3531 2043 2031 352e 3638 3234  930651 C 15.6824
-0000a710: 3935 2c30 2e33 3333 3631 3731 2031 362e  95,0.3336171 16.
-0000a720: 3439 3033 3235 2c30 2e31 3734 3136 3920  490325,0.174169 
-0000a730: 3137 2e32 3938 3135 362c 302e 3031 3437  17.298156,0.0147
-0000a740: 3231 3030 3320 4320 3137 2e38 3831 3130  21003 C 17.88110
-0000a750: 372c 302e 3830 3238 3632 3920 3138 2e33  7,0.8028629 18.3
-0000a760: 3436 3437 322c 312e 3637 3833 3335 3720  46472,1.6783357 
-0000a770: 3138 2e36 3730 3933 2c32 2e36 3034 3032  18.67093,2.60402
-0000a780: 3734 2043 2031 392e 3032 3735 342c 332e  74 C 19.02754,3.
-0000a790: 3631 3633 3635 3520 3139 2e32 3136 3233  6163655 19.21623
-0000a7a0: 382c 342e 3638 3431 3135 3620 3139 2e32  8,4.6841156 19.2
-0000a7b0: 3636 3336 392c 352e 3735 3532 3838 3820  66369,5.7552888 
-0000a7c0: 4320 3139 2e32 3830 3034 2c36 2e30 3232  C 19.28004,6.022
-0000a7d0: 3135 3231 2031 392e 3238 3134 3434 2c36  1521 19.281444,6
-0000a7e0: 2e32 3839 3337 3733 2031 392e 3238 3130  .2893773 19.2810
-0000a7f0: 3132 2c36 2e35 3536 3532 3339 2043 2031  12,6.5565239 C 1
-0000a800: 392e 3238 3130 3239 2c31 312e 3632 3730  9.281029,11.6270
-0000a810: 3831 2031 392e 3238 3039 3739 2c31 362e  81 19.280979,16.
-0000a820: 3639 3736 3339 2031 392e 3238 3130 3338  697639 19.281038
-0000a830: 2c32 312e 3736 3831 3937 2043 2031 392e  ,21.768197 C 19.
-0000a840: 3238 3233 3737 2c32 322e 3438 3537 3438  282377,22.485748
-0000a850: 2031 392e 3239 3236 3939 2c32 332e 3230   19.292699,23.20
-0000a860: 3336 3339 2031 392e 3333 3430 3333 2c32  3639 19.334033,2
-0000a870: 332e 3932 3031 3235 2043 2031 392e 3335  3.920125 C 19.35
-0000a880: 3432 3937 2c32 342e 3234 3936 3333 2031  4297,24.249633 1
-0000a890: 392e 3337 3838 3331 2c32 342e 3537 3934  9.378831,24.5794
-0000a8a0: 3238 2031 392e 3432 3838 3236 2c32 342e  28 19.428826,24.
-0000a8b0: 3930 3539 3433 2043 2031 392e 3434 3434  905943 C 19.4444
-0000a8c0: 3931 2c32 352e 3031 3230 3535 2031 392e  91,25.012055 19.
-0000a8d0: 3437 3232 3738 2c32 352e 3131 3539 3134  472278,25.115914
-0000a8e0: 2031 392e 3530 3039 3437 2c32 352e 3231   19.500947,25.21
-0000a8f0: 3931 3220 4320 3139 2e35 3939 3838 342c  912 C 19.599884,
-0000a900: 3235 2e35 3636 3932 3620 3139 2e37 3537  25.566926 19.757
-0000a910: 3631 352c 3235 2e38 3938 3431 3820 3139  615,25.898418 19
-0000a920: 2e39 3730 3532 2c32 362e 3139 3037 3631  .97052,26.190761
-0000a930: 2043 2032 302e 3035 3333 3831 2c32 362e   C 20.053381,26.
-0000a940: 3330 3430 3032 2032 302e 3134 3230 3639  304002 20.142069
-0000a950: 2c32 362e 3431 3333 3931 2032 302e 3234  ,26.413391 20.24
-0000a960: 3034 3237 2c32 362e 3531 3335 3332 2043  0427,26.513532 C
-0000a970: 2032 302e 3533 3737 3331 2c32 362e 3831   20.537731,26.81
-0000a980: 3337 3338 2032 302e 3930 3637 3931 2c32  3738 20.906791,2
-0000a990: 372e 3033 3531 3939 2032 312e 3239 3735  7.035199 21.2975
-0000a9a0: 3333 2c32 372e 3139 3036 3520 4320 3231  33,27.19065 C 21
-0000a9b0: 2e37 3833 3732 372c 3237 2e33 3833 3939  .783727,27.38399
-0000a9c0: 3720 3232 2e33 3032 3132 312c 3237 2e34  7 22.302121,27.4
-0000a9d0: 3833 3638 3220 3232 2e38 3231 3234 362c  83682 22.821246,
-0000a9e0: 3237 2e35 3334 3236 3220 4320 3233 2e31  27.534262 C 23.1
-0000a9f0: 3436 3032 322c 3237 2e35 3636 3030 3920  46022,27.566009 
-0000aa00: 3233 2e34 3732 3437 352c 3237 2e35 3736  23.472475,27.576
-0000aa10: 3030 3820 3233 2e37 3938 3637 322c 3237  008 23.798672,27
-0000aa20: 2e35 3734 3730 3420 4320 3234 2e32 3731  .574704 C 24.271
-0000aa30: 3536 312c 3237 2e35 3734 3730 3420 3234  561,27.574704 24
-0000aa40: 2e37 3434 3435 322c 3237 2e35 3734 3730  .744452,27.57470
-0000aa50: 3420 3235 2e32 3137 3334 322c 3237 2e35  4 25.217342,27.5
-0000aa60: 3734 3730 3420 4320 3235 2e32 3137 3334  74704 C 25.21734
-0000aa70: 322c 3236 2e37 3532 3933 3320 3235 2e32  2,26.752933 25.2
-0000aa80: 3137 3334 322c 3235 2e39 3331 3136 3320  17342,25.931163 
-0000aa90: 3235 2e32 3137 3334 322c 3235 2e31 3039  25.217342,25.109
-0000aaa0: 3339 3220 4320 3236 2e35 3134 3736 372c  392 C 26.514767,
-0000aab0: 3236 2e32 3832 3736 3620 3237 2e38 3132  26.282766 27.812
-0000aac0: 3139 322c 3237 2e34 3536 3134 2032 392e  192,27.45614 29.
-0000aad0: 3130 3936 3137 2c32 382e 3632 3935 3134  109617,28.629514
-0000aae0: 2043 2032 372e 3831 3231 3932 2c32 392e   C 27.812192,29.
-0000aaf0: 3735 3739 3136 2032 362e 3531 3437 3637  757916 26.514767
-0000ab00: 2c33 302e 3838 3633 3137 2032 352e 3231  ,30.886317 25.21
-0000ab10: 3733 3432 2c33 322e 3031 3437 3139 2043  7342,32.014719 C
-0000ab20: 2032 352e 3231 3733 3432 2c33 312e 3231   25.217342,31.21
-0000ab30: 3734 3739 2032 352e 3231 3733 3432 2c33  7479 25.217342,3
-0000ab40: 302e 3432 3032 3339 2032 352e 3231 3733  0.420239 25.2173
-0000ab50: 3432 2c32 392e 3632 3239 3938 2043 2032  42,29.622998 C 2
-0000ab60: 342e 3434 3938 3339 2c32 392e 3632 3239  4.449839,29.6229
-0000ab70: 3331 2032 332e 3638 3233 3334 2c32 392e  31 23.682334,29.
-0000ab80: 3632 3331 3334 2032 322e 3931 3438 332c  623134 22.91483,
-0000ab90: 3239 2e36 3232 3839 3520 4320 3232 2e31  29.622895 C 22.1
-0000aba0: 3735 3234 372c 3239 2e36 3139 3238 3220  75247,29.619282 
-0000abb0: 3231 2e34 3331 3838 392c 3239 2e35 3531  21.431889,29.551
-0000abc0: 3335 2032 302e 3731 3435 3534 2c32 392e  35 20.714554,29.
-0000abd0: 3336 3437 3238 2043 2032 302e 3132 3437  364728 C 20.1247
-0000abe0: 3934 2c32 392e 3231 3130 3833 2031 392e  94,29.211083 19.
-0000abf0: 3535 3234 3332 2c32 382e 3937 3230 3933  552432,28.972093
-0000ac00: 2031 392e 3035 3139 3037 2c32 382e 3632   19.051907,28.62
-0000ac10: 3036 3736 2043 2031 382e 3638 3735 3531  0676 C 18.687551
-0000ac20: 2c32 382e 3336 3632 3537 2031 382e 3336  ,28.366257 18.36
-0000ac30: 3535 3433 2c32 382e 3035 3137 3336 2031  5543,28.051736 1
-0000ac40: 382e 3130 3039 3839 2c32 372e 3639 3433  8.100989,27.6943
-0000ac50: 3834 2043 2031 372e 3732 3533 3138 2c32  84 C 17.725318,2
-0000ac60: 372e 3138 3934 3636 2031 372e 3436 3031  7.189466 17.4601
-0000ac70: 352c 3236 2e36 3039 3435 2031 372e 3237  5,26.60945 17.27
-0000ac80: 3237 3134 2c32 362e 3031 3033 3438 2043  2714,26.010348 C
-0000ac90: 2031 372e 3034 3338 3236 2c32 352e 3237   17.043826,25.27
-0000aca0: 3632 3636 2031 362e 3932 3534 3238 2c32  6266 16.925428,2
-0000acb0: 342e 3531 3138 2031 362e 3836 3631 3835  4.5118 16.866185
-0000acc0: 2c32 332e 3734 3633 3634 2043 2031 362e  ,23.746364 C 16.
-0000acd0: 3833 3132 3131 2c32 332e 3239 3534 3134  831211,23.295414
-0000ace0: 2031 362e 3831 3934 3739 2c32 322e 3834   16.819479,22.84
-0000acf0: 3320 3136 2e38 3230 3830 312c 3232 2e33  3 16.820801,22.3
-0000ad00: 3930 3738 3520 4320 3136 2e38 3230 3739  90785 C 16.82079
-0000ad10: 2c31 372e 3437 3335 3033 2031 362e 3832  ,17.473503 16.82
-0000ad20: 3038 3233 2c31 322e 3535 3632 3231 2031  0823,12.556221 1
-0000ad30: 362e 3832 3037 3835 2c37 2e36 3338 3933  6.820785,7.63893
-0000ad40: 3832 2043 2031 362e 3831 3839 3936 2c36  82 C 16.818996,6
-0000ad50: 2e37 3632 3231 3932 2031 362e 3737 3735  .7622192 16.7775
-0000ad60: 3933 2c35 2e38 3833 3635 3932 2031 362e  93,5.8836592 16.
-0000ad70: 3635 3039 3737 2c35 2e30 3135 3435 3233  650977,5.0154523
-0000ad80: 2043 2031 362e 3535 3934 372c 342e 3339   C 16.55947,4.39
-0000ad90: 3833 3331 3920 3136 2e34 3235 3434 342c  83319 16.425444,
-0000ada0: 332e 3738 3434 3132 3720 3136 2e32 3033  3.7844127 16.203
-0000adb0: 3934 332c 332e 3230 3031 3033 3120 4320  943,3.2001031 C 
-0000adc0: 3136 2e30 3831 3939 362c 322e 3838 3032  16.081996,2.8802
-0000add0: 3230 3820 3135 2e39 3332 3633 322c 322e  208 15.932632,2.
-0000ade0: 3536 3936 3230 3920 3135 2e37 3433 3639  5696209 15.74369
-0000adf0: 342c 322e 3238 3337 3839 3420 4320 3134  4,2.2837894 C 14
-0000ae00: 2e38 3135 3331 352c 332e 3335 3534 3935  .815315,3.355495
-0000ae10: 2031 342e 3033 3835 3839 2c34 2e35 3536   14.038589,4.556
-0000ae20: 3331 3138 2031 332e 3432 3038 3936 2c35  3118 13.420896,5
-0000ae30: 2e38 3332 3634 3639 2043 2031 322e 3734  .8326469 C 12.74
-0000ae40: 3132 3339 2c37 2e32 3334 3834 3738 2031  1239,7.2348478 1
-0000ae50: 322e 3235 3032 3234 2c38 2e37 3234 3636  2.250224,8.72466
-0000ae60: 3320 3131 2e39 3132 3631 392c 3130 2e32  3 11.912619,10.2
-0000ae70: 3434 3938 3820 4320 3131 2e39 3132 3631  44988 C 11.91261
-0000ae80: 392c 3135 2e31 3939 3739 2031 312e 3931  9,15.19979 11.91
-0000ae90: 3236 3139 2c32 302e 3135 3435 3920 3131  2619,20.15459 11
-0000aea0: 2e39 3132 3631 392c 3235 2e31 3039 3339  .912619,25.10939
-0000aeb0: 3220 4320 3131 2e30 3932 3534 392c 3235  2 C 11.092549,25
-0000aec0: 2e31 3039 3339 3220 3130 2e32 3732 3437  .109392 10.27247
-0000aed0: 382c 3235 2e31 3039 3339 3220 392e 3435  8,25.109392 9.45
-0000aee0: 3234 3038 332c 3235 2e31 3039 3339 3220  24083,25.109392 
-0000aef0: 4320 392e 3435 3233 3937 332c 3139 2e35  C 9.4523973,19.5
-0000af00: 3734 3331 3920 392e 3435 3234 3330 332c  74319 9.4524303,
-0000af10: 3134 2e30 3339 3234 3620 392e 3435 3233  14.039246 9.4523
-0000af20: 3932 332c 382e 3530 3431 3733 3320 4320  923,8.5041733 C 
-0000af30: 392e 3435 3036 3134 332c 372e 3530 3434  9.4506143,7.5044
-0000af40: 3038 3220 392e 3431 3330 3134 332c 362e  082 9.4130143,6.
-0000af50: 3530 3332 3131 3820 392e 3239 3536 3639  5032118 9.295669
-0000af60: 332c 352e 3530 3938 3239 3620 4320 392e  3,5.5098296 C 9.
-0000af70: 3231 3437 3532 332c 342e 3833 3832 3237  2147523,4.838227
-0000af80: 2039 2e30 3938 3630 3433 2c34 2e31 3638   9.0986043,4.168
-0000af90: 3536 3835 2038 2e39 3033 3738 3833 2c33  5685 8.9037883,3
-0000afa0: 2e35 3139 3938 3136 2043 2038 2e37 3733  .5199816 C 8.773
-0000afb0: 3433 3233 2c33 2e30 3930 3530 3833 2038  4323,3.0905083 8
-0000afc0: 2e36 3038 3033 3733 2c32 2e36 3638 3633  .6080373,2.66863
-0000afd0: 3720 382e 3337 3533 3031 332c 322e 3238  7 8.3753013,2.28
-0000afe0: 3337 3839 3420 4320 372e 3433 3335 3434  37894 C 7.433544
-0000aff0: 332c 332e 3334 3433 3739 2036 2e36 3434  3,3.344379 6.644
-0000b000: 3034 3033 2c34 2e35 3336 3932 3931 2036  0403,4.5369291 6
-0000b010: 2e30 3036 3438 3033 2c35 2e38 3033 3639  .0064803,5.80369
-0000b020: 3336 2043 2035 2e33 3831 3534 3833 2c37  36 C 5.3815483,7
-0000b030: 2e30 3434 3134 3036 2034 2e38 3938 3730  .0441406 4.89870
-0000b040: 3533 2c38 2e33 3533 3839 3120 342e 3533  53,8.353891 4.53
-0000b050: 3139 3836 332c 392e 3639 3330 3532 3320  19863,9.6930523 
-0000b060: 4320 342e 3533 3139 3836 332c 3134 2e38  C 4.5319863,14.8
-0000b070: 3331 3833 3320 342e 3533 3139 3836 332c  31833 4.5319863,
-0000b080: 3139 2e39 3730 3631 3220 342e 3533 3139  19.970612 4.5319
-0000b090: 3836 332c 3235 2e31 3039 3339 3220 4320  863,25.109392 C 
-0000b0a0: 332e 3731 3139 3135 332c 3235 2e31 3039  3.7119153,25.109
-0000b0b0: 3339 3220 322e 3839 3138 3435 342c 3235  392 2.8918454,25
-0000b0c0: 2e31 3039 3339 3220 322e 3037 3137 3735  .109392 2.071775
-0000b0d0: 2c32 352e 3130 3933 3932 207a 220a 2020  ,25.109392 z".  
-0000b0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0f0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-0000b100: 6c3a 2024 7a6f 6469 6163 5f63 6f6c 6f72  l: $zodiac_color
-0000b110: 5f37 220a 2020 2020 2020 2020 2020 2020  _7".            
-0000b120: 2020 2020 2020 2020 2f3e 0a20 2020 2020          />.     
-0000b130: 2020 2020 2020 2020 2020 203c 2f73 796d             </sym
-0000b140: 626f 6c3e 0a20 2020 2020 2020 2020 2020  bol>.           
-0000b150: 2020 2020 203c 7379 6d62 6f6c 2069 643d       <symbol id=
-0000b160: 2273 6167 6974 7461 7269 7573 223e 0a20  "sagittarius">. 
-0000b170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b180: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-0000b190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1a0: 2064 3d22 4d20 3239 2e38 3932 3934 322c   d="M 29.892942,
-0000b1b0: 322e 3039 3538 3730 3620 4c20 3332 2c31  2.0958706 L 32,1
-0000b1c0: 372e 3131 3632 3736 204c 2032 382e 3939  7.116276 L 28.99
-0000b1d0: 3835 3739 2c31 372e 3538 3730 3838 204c  8579,17.587088 L
-0000b1e0: 2032 372e 3435 3233 3933 2c36 2e36 3336   27.452393,6.636
-0000b1f0: 3932 3335 204c 2031 332e 3733 3337 3736  9235 L 13.733776
-0000b200: 2c32 302e 3431 3139 3537 204c 2032 302e  ,20.411957 L 20.
-0000b210: 3139 3133 3739 2c32 362e 3836 3636 3320  191379,26.86663 
-0000b220: 4c20 3138 2e30 3338 3834 352c 3239 2e30  L 18.038845,29.0
-0000b230: 3233 3235 3120 4c20 3131 2e35 3831 3234  23251 L 11.58124
-0000b240: 322c 3232 2e35 3533 3339 204c 2032 2e30  2,22.55339 L 2.0
-0000b250: 3931 3930 312c 3331 2e39 3939 3939 3520  91901,31.999995 
-0000b260: 4c20 312e 3565 2d30 362c 3239 2e39 3034  L 1.5e-06,29.904
-0000b270: 3132 3420 4c20 392e 3437 3431 3834 2c32  124 L 9.474184,2
-0000b280: 302e 3434 3233 3332 204c 2033 2e30 3331  0.442332 L 3.031
-0000b290: 3734 2c31 332e 3937 3234 3720 4c20 352e  74,13.97247 L 5.
-0000b2a0: 3135 3339 3537 2c31 312e 3831 3538 3520  153957,11.81585 
-0000b2b0: 4c20 3131 2e36 3131 3536 2c31 382e 3238  L 11.61156,18.28
-0000b2c0: 3537 3131 204c 2032 352e 3336 3034 3933  5711 L 25.360493
-0000b2d0: 2c34 2e35 3431 3035 3239 204c 2031 342e  ,4.5410529 L 14.
-0000b2e0: 3433 3130 3736 2c33 2e30 3037 3131 3836  431076,3.0071186
-0000b2f0: 204c 2031 342e 3930 3039 3936 2c2d 342e   L 14.900996,-4.
-0000b300: 3434 3038 3932 3165 2d31 3620 4c20 3239  4408921e-16 L 29
-0000b310: 2e38 3932 3934 322c 322e 3039 3538 3730  .892942,2.095870
-0000b320: 3620 7a20 220a 2020 2020 2020 2020 2020  6 z ".          
-0000b330: 2020 2020 2020 2020 2020 2020 2020 7374                st
-0000b340: 796c 653d 2266 696c 6c3a 2024 7a6f 6469  yle="fill: $zodi
-0000b350: 6163 5f63 6f6c 6f72 5f38 220a 2020 2020  ac_color_8".    
-0000b360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b370: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-0000b380: 2020 203c 2f73 796d 626f 6c3e 0a20 2020     </symbol>.   
-0000b390: 2020 2020 2020 2020 2020 2020 203c 7379               <sy
-0000b3a0: 6d62 6f6c 2069 643d 2263 6170 7269 636f  mbol id="caprico
-0000b3b0: 726e 223e 0a20 2020 2020 2020 2020 2020  rn">.           
-0000b3c0: 2020 2020 2020 2020 203c 7061 7468 0a20           <path. 
-0000b3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3e0: 2020 2020 2020 2064 3d22 4d20 362e 3130         d="M 6.10
-0000b3f0: 3933 3535 392c 3138 2e39 3034 3737 3420  93559,18.904774 
-0000b400: 4320 362e 3130 3932 3339 322c 3138 2e35  C 6.1092392,18.5
-0000b410: 3839 3535 2036 2e31 3039 3630 3432 2c31  8955 6.1096042,1
-0000b420: 382e 3237 3433 3235 2036 2e31 3039 3134  8.274325 6.10914
-0000b430: 3733 2c31 372e 3935 3931 3033 2043 2036  73,17.959103 C 6
-0000b440: 2e31 3033 3633 3839 2c31 372e 3134 3632  .1036389,17.1462
-0000b450: 3334 2036 2e30 3336 3435 3837 2c31 362e  34 6.0364587,16.
-0000b460: 3333 3530 3635 2035 2e39 3436 3339 3638  335065 5.9463968
-0000b470: 2c31 352e 3532 3736 3131 2043 2035 2e38  ,15.527611 C 5.8
-0000b480: 3032 3031 3933 2c31 342e 3235 3436 3432  020193,14.254642
-0000b490: 2035 2e35 3936 3039 3433 2c31 322e 3938   5.5960943,12.98
-0000b4a0: 3934 3635 2035 2e33 3636 3533 3133 2c31  9465 5.3665313,1
-0000b4b0: 312e 3732 3933 3338 2043 2035 2e32 3235  1.729338 C 5.225
-0000b4c0: 3836 3034 2c31 302e 3935 3639 3237 2035  8604,10.956927 5
-0000b4d0: 2e30 3730 3434 2c31 302e 3138 3732 3220  .07044,10.18722 
-0000b4e0: 342e 3930 3335 3537 2c39 2e34 3230 3035  4.903557,9.42005
-0000b4f0: 3437 2043 2034 2e37 3231 3830 3237 2c38  47 C 4.7218027,8
-0000b500: 2e35 3933 3130 3532 2034 2e35 3236 3233  .5931052 4.52623
-0000b510: 3839 2c37 2e37 3638 3439 3037 2034 2e32  89,7.7684907 4.2
-0000b520: 3835 3333 3336 2c36 2e39 3536 3532 3437  853336,6.9565247
-0000b530: 2043 2034 2e31 3533 3230 3336 2c36 2e35   C 4.1532036,6.5
-0000b540: 3136 3935 3534 2034 2e30 3039 3931 3339  169554 4.0099139
-0000b550: 2c36 2e30 3739 3533 2033 2e38 3235 3133  ,6.07953 3.82513
-0000b560: 3334 2c35 2e36 3538 3838 3536 2043 2033  34,5.6588856 C 3
-0000b570: 2e36 3538 3932 3334 2c35 2e32 3833 3631  .6589234,5.28361
-0000b580: 3531 2033 2e34 3437 3231 3638 2c34 2e39  51 3.4472168,4.9
-0000b590: 3236 3935 3239 2033 2e31 3834 3334 3939  269529 3.1843499
-0000b5a0: 2c34 2e36 3131 3038 3838 2043 2032 2e39  ,4.6110888 C 2.9
-0000b5b0: 3030 3932 3039 2c34 2e32 3730 3039 3239  009209,4.2700929
-0000b5c0: 2032 2e35 3531 3435 3238 2c33 2e39 3832   2.5514528,3.982
-0000b5d0: 3030 3131 2032 2e31 3534 3638 3531 2c33  0011 2.1546851,3
-0000b5e0: 2e37 3832 3336 3431 2043 2031 2e37 3237  .7823641 C 1.727
-0000b5f0: 3238 3436 2c33 2e35 3635 3232 3631 2031  2846,3.5652261 1
-0000b600: 2e32 3531 3938 3437 2c33 2e34 3532 3537  .2519847,3.45257
-0000b610: 3137 2030 2e37 3734 3938 3437 382c 332e  17 0.77498478,3.
-0000b620: 3432 3230 3438 3620 4320 302e 3538 3730  4220486 C 0.5870
-0000b630: 3136 3737 2c33 2e34 3038 3937 3036 2030  1677,3.4089706 0
-0000b640: 2e33 3938 3539 3637 352c 332e 3431 3239  .39859675,3.4129
-0000b650: 3732 3820 302e 3231 3033 3431 392c 332e  728 0.2103419,3.
-0000b660: 3431 3232 3935 2043 2030 2e31 3430 3230  412295 C 0.14020
-0000b670: 3339 312c 332e 3431 3232 3935 2030 2e30  391,3.412295 0.0
-0000b680: 3730 3036 3436 3833 2c33 2e34 3132 3239  70064683,3.41229
-0000b690: 3520 2d37 2e33 3330 3237 3765 2d30 352c  5 -7.330277e-05,
-0000b6a0: 332e 3431 3232 3935 2043 202d 372e 3333  3.412295 C -7.33
-0000b6b0: 3032 3737 652d 3035 2c32 2e37 3239 3533  0277e-05,2.72953
-0000b6c0: 3335 202d 372e 3333 3032 3737 652d 3035  35 -7.330277e-05
-0000b6d0: 2c32 2e30 3436 3737 3220 2d37 2e33 3330  ,2.046772 -7.330
-0000b6e0: 3237 3765 2d30 352c 312e 3336 3430 3130  277e-05,1.364010
-0000b6f0: 3620 4320 302e 3632 3736 3334 3534 2c31  6 C 0.62763454,1
-0000b700: 2e33 3634 3033 3137 2031 2e32 3535 3334  .3640317 1.25534
-0000b710: 3234 2c31 2e33 3633 3936 3936 2031 2e38  24,1.3639696 1.8
-0000b720: 3833 3035 3032 2c31 2e33 3634 3034 3136  830502,1.3640416
-0000b730: 2043 2032 2e34 3439 3434 342c 312e 3336   C 2.449444,1.36
-0000b740: 3538 3531 3520 332e 3032 3130 3939 2c31  58515 3.021099,1
-0000b750: 2e34 3339 3131 3536 2033 2e35 3535 3031  .4391156 3.55501
-0000b760: 312c 312e 3633 3433 3239 3520 4320 332e  1,1.6343295 C 3.
-0000b770: 3938 3336 3639 342c 312e 3739 3031 3037  9836694,1.790107
-0000b780: 3120 342e 3338 3332 3836 392c 322e 3032  1 4.3832869,2.02
-0000b790: 3931 3538 2034 2e37 3134 3738 382c 322e  9158 4.714788,2.
-0000b7a0: 3334 3331 3737 3420 4320 352e 3036 3932  3431774 C 5.0692
-0000b7b0: 3535 342c 322e 3637 3634 3830 3520 352e  554,2.6764805 5.
-0000b7c0: 3334 3335 3931 312c 332e 3038 3834 3836  3435911,3.088486
-0000b7d0: 3120 352e 3534 3432 3334 392c 332e 3533  1 5.5442349,3.53
-0000b7e0: 3031 3633 3220 4320 352e 3834 3731 3630  01632 C 5.847160
-0000b7f0: 382c 342e 3138 3435 3437 3920 362e 3038  8,4.1845479 6.08
-0000b800: 3633 3437 342c 342e 3836 3634 3233 2036  63474,4.866423 6
-0000b810: 2e32 3939 3537 3634 2c35 2e35 3534 3632  .2995764,5.55462
-0000b820: 3035 2043 2036 2e36 3331 3632 3134 2c36  05 C 6.6316214,6
-0000b830: 2e36 3335 3035 3720 362e 3839 3630 3035  .635057 6.896005
-0000b840: 372c 372e 3733 3530 3636 3420 372e 3133  7,7.7350664 7.13
-0000b850: 3138 3332 322c 382e 3834 3030 3838 3620  18322,8.8400886 
-0000b860: 4320 372e 3332 3737 3433 372c 392e 3736  C 7.3277437,9.76
-0000b870: 3231 3930 3220 372e 3530 3135 3335 392c  21902 7.5015359,
-0000b880: 3130 2e36 3838 3838 3320 372e 3636 3135  10.688883 7.6615
-0000b890: 3438 332c 3131 2e36 3137 3834 3720 4320  483,11.617847 C 
-0000b8a0: 382e 3038 3137 3833 392c 392e 3734 3030  8.0817839,9.7400
-0000b8b0: 3139 3120 382e 3635 3231 3732 332c 372e  191 8.6521723,7.
-0000b8c0: 3839 3130 3831 3220 392e 3433 3635 3035  8910812 9.436505
-0000b8d0: 312c 362e 3133 3139 3739 3720 4320 3130  1,6.1319797 C 10
-0000b8e0: 2e31 3232 3636 352c 342e 3539 3238 3133  .122665,4.592813
-0000b8f0: 3220 3130 2e39 3736 3733 372c 332e 3132  2 10.976737,3.12
-0000b900: 3338 3233 3320 3132 2e30 3233 3337 322c  38233 12.023372,
-0000b910: 312e 3830 3038 3733 3620 4320 3132 2e31  1.8008736 C 12.1
-0000b920: 3432 3434 322c 312e 3635 3431 3739 3220  42442,1.6541792 
-0000b930: 3132 2e32 3538 3639 2c31 2e35 3030 3439  12.25869,1.50049
-0000b940: 3333 2031 322e 3338 3536 3037 2c31 2e33  33 12.385607,1.3
-0000b950: 3632 3937 3238 2043 2031 332e 3438 3036  629728 C 13.4806
-0000b960: 3931 2c31 2e31 3532 3238 3338 2031 342e  91,1.1522838 14.
-0000b970: 3537 3537 3737 2c30 2e39 3431 3539 3334  575777,0.9415934
-0000b980: 3920 3135 2e36 3730 3836 312c 302e 3733  9 15.670861,0.73
-0000b990: 3039 3034 3437 2043 2031 362e 3031 3034  090447 C 16.0104
-0000b9a0: 3932 2c31 2e35 3031 3536 3539 2031 362e  92,1.5015659 16.
-0000b9b0: 3237 3438 3832 2c32 2e33 3033 3135 3839  274882,2.3031589
-0000b9c0: 2031 362e 3530 3437 3237 2c33 2e31 3132   16.504727,3.112
-0000b9d0: 3633 3937 2043 2031 362e 3834 3731 3233  6397 C 16.847123
-0000b9e0: 2c34 2e33 3237 3339 3237 2031 372e 3130  ,4.3273927 17.10
-0000b9f0: 3930 3231 2c35 2e35 3633 3339 3731 2031  9021,5.5633971 1
-0000ba00: 372e 3333 3333 3032 2c36 2e38 3034 3930  7.333302,6.80490
-0000ba10: 3832 2043 2031 372e 3436 3536 3835 2c37  82 C 17.465685,7
-0000ba20: 2e35 3339 3231 3435 2031 372e 3538 3235  .5392145 17.5825
-0000ba30: 3636 2c38 2e32 3736 3233 3036 2031 372e  66,8.2762306 17.
-0000ba40: 3639 3035 342c 392e 3031 3434 3931 3920  69054,9.0144919 
-0000ba50: 4320 3137 2e38 3431 3031 312c 3130 2e30  C 17.841011,10.0
-0000ba60: 3130 3535 3420 3137 2e39 3931 3438 2c31  10554 17.99148,1
-0000ba70: 312e 3030 3636 3135 2031 382e 3134 3139  1.006615 18.1419
-0000ba80: 3531 2c31 322e 3030 3236 3736 2043 2031  51,12.002676 C 1
-0000ba90: 382e 3233 3632 3236 2c31 322e 3638 3139  8.236226,12.6819
-0000baa0: 3832 2031 382e 3333 3034 3638 2c31 332e  82 18.330468,13.
-0000bab0: 3336 3133 3439 2031 382e 3431 3330 3531  361349 18.413051
-0000bac0: 2c31 342e 3034 3231 3935 2043 2031 382e  ,14.042195 C 18.
-0000bad0: 3434 3836 3639 2c31 342e 3334 3036 3234  448669,14.340624
-0000bae0: 2031 382e 3437 3930 3639 2c31 342e 3633   18.479069,14.63
-0000baf0: 3936 3538 2031 382e 3531 3733 342c 3134  9658 18.51734,14
-0000bb00: 2e39 3337 3737 3420 4320 3138 2e36 3138  .937774 C 18.618
-0000bb10: 3933 342c 3135 2e37 3435 3730 3820 3138  934,15.745708 18
-0000bb20: 2e37 3431 3936 372c 3136 2e35 3531 3739  .741967,16.55179
-0000bb30: 3520 3138 2e39 3136 3938 372c 3137 2e33  5 18.916987,17.3
-0000bb40: 3437 3338 3120 4320 3138 2e39 3936 3233  47381 C 18.99623
-0000bb50: 342c 3137 2e37 3034 3532 3220 3139 2e30  4,17.704522 19.0
-0000bb60: 3836 3134 312c 3138 2e30 3539 3631 3320  86141,18.059613 
-0000bb70: 3139 2e31 3937 3434 322c 3138 2e34 3038  19.197442,18.408
-0000bb80: 3232 2043 2031 392e 3635 3435 3634 2c31  22 C 19.654564,1
-0000bb90: 372e 3533 3430 3134 2032 302e 3230 3330  7.534014 20.2030
-0000bba0: 3731 2c31 362e 3730 3132 3735 2032 302e  71,16.701275 20.
-0000bbb0: 3838 3037 3036 2c31 352e 3938 3133 3533  880706,15.981353
-0000bbc0: 2043 2032 312e 3434 3533 3737 2c31 352e   C 21.445377,15.
-0000bbd0: 3338 3037 3731 2032 322e 3130 3433 3138  380771 22.104318
-0000bbe0: 2c31 342e 3836 3335 3037 2032 322e 3834  ,14.863507 22.84
-0000bbf0: 3233 3136 2c31 342e 3439 3235 3836 2043  2316,14.492586 C
-0000bc00: 2032 332e 3531 3834 3334 2c31 342e 3135   23.518434,14.15
-0000bc10: 3035 3733 2032 342e 3235 3730 3535 2c31  0573 24.257055,1
-0000bc20: 332e 3933 3630 3235 2032 352e 3030 3934  3.936025 25.0094
-0000bc30: 3534 2c31 332e 3835 3033 3034 2043 2032  54,13.850304 C 2
-0000bc40: 352e 3536 3639 3839 2c31 332e 3738 3733  5.566989,13.7873
-0000bc50: 3620 3236 2e31 3332 3231 382c 3133 2e37  6 26.132218,13.7
-0000bc60: 3834 3836 3920 3236 2e36 3839 3431 2c31  84869 26.68941,1
-0000bc70: 332e 3835 3320 4320 3237 2e33 3730 3631  3.853 C 27.37061
-0000bc80: 362c 3133 2e39 3336 3037 3620 3238 2e30  6,13.936076 28.0
-0000bc90: 3338 3837 362c 3134 2e31 3333 3120 3238  38876,14.1331 28
-0000bca0: 2e36 3531 3036 312c 3134 2e34 3434 3136  .651061,14.44416
-0000bcb0: 3920 4320 3239 2e32 3334 3138 372c 3134  9 C 29.234187,14
-0000bcc0: 2e37 3338 3731 3320 3239 2e37 3633 3830  .738713 29.76380
-0000bcd0: 352c 3135 2e31 3333 3738 3520 3330 2e32  5,15.133785 30.2
-0000bce0: 3237 3530 312c 3135 2e35 3932 3834 3720  27501,15.592847 
-0000bcf0: 4320 3330 2e37 3137 3133 2c31 362e 3037  C 30.71713,16.07
-0000bd00: 3135 3137 2033 312e 3133 3338 3035 2c31  1517 31.133805,1
-0000bd10: 362e 3632 3832 3132 2033 312e 3433 3139  6.628212 31.4319
-0000bd20: 342c 3137 2e32 3435 3636 3220 4320 3331  4,17.245662 C 31
-0000bd30: 2e37 3233 3539 2c31 372e 3834 3536 3833  .72359,17.845683
-0000bd40: 2033 312e 3930 3030 3738 2c31 382e 3439   31.900078,18.49
-0000bd50: 3932 3332 2033 312e 3936 3634 3639 2c31  9232 31.966469,1
-0000bd60: 392e 3136 3233 3938 2043 2033 322e 3031  9.162398 C 32.01
-0000bd70: 3536 3132 2c31 392e 3635 3138 3631 2033  5612,19.651861 3
-0000bd80: 322e 3030 3933 3235 2c32 302e 3134 3633  2.009325,20.1463
-0000bd90: 3538 2033 312e 3935 3736 3034 2c32 302e  58 31.957604,20.
-0000bda0: 3633 3533 3336 2043 2033 312e 3837 3934  635336 C 31.8794
-0000bdb0: 322c 3231 2e33 3636 3138 3720 3331 2e36  2,21.366187 31.6
-0000bdc0: 3831 3834 382c 3232 2e30 3835 3834 3920  81848,22.085849 
-0000bdd0: 3331 2e33 3539 3030 372c 3232 2e37 3436  31.359007,22.746
-0000bde0: 3938 3820 4320 3331 2e30 3335 3434 322c  988 C 31.035442,
-0000bdf0: 3233 2e34 3133 3539 3620 3330 2e35 3837  23.413596 30.587
-0000be00: 3136 352c 3234 2e30 3136 3731 3820 3330  165,24.016718 30
-0000be10: 2e30 3537 3635 2c32 342e 3533 3339 3937  .05765,24.533997
-0000be20: 2043 2032 392e 3535 3633 3834 2c32 352e   C 29.556384,25.
-0000be30: 3032 3538 3933 2032 382e 3937 3639 3137  025893 28.976917
-0000be40: 2c32 352e 3434 3135 3231 2032 382e 3333  ,25.441521 28.33
-0000be50: 3739 3833 2c32 352e 3733 3535 3535 2043  7983,25.735555 C
-0000be60: 2032 372e 3732 3034 3331 2c32 362e 3032   27.720431,26.02
-0000be70: 3136 3639 2032 372e 3035 3133 3238 2c32  1669 27.051328,2
-0000be80: 362e 3139 3133 3232 2032 362e 3337 3339  6.191322 26.3739
-0000be90: 382c 3236 2e32 3531 3237 3120 4320 3235  8,26.251271 C 25
-0000bea0: 2e39 3033 3534 392c 3236 2e32 3933 3334  .903549,26.29334
-0000beb0: 3920 3235 2e34 3239 3530 392c 3236 2e32  9 25.429509,26.2
-0000bec0: 3834 3235 3920 3234 2e39 3539 3335 312c  84259 24.959351,
-0000bed0: 3236 2e32 3433 3233 3320 4320 3234 2e31  26.243233 C 24.1
-0000bee0: 3032 3436 342c 3236 2e31 3636 3832 3820  02464,26.166828 
-0000bef0: 3233 2e32 3537 3134 352c 3235 2e39 3535  23.257145,25.955
-0000bf00: 3232 3720 3232 2e34 3638 3435 312c 3235  227 22.468451,25
-0000bf10: 2e36 3130 3939 3120 4320 3231 2e36 3130  .610991 C 21.610
-0000bf20: 3633 322c 3235 2e32 3338 3632 3120 3230  632,25.238621 20
-0000bf30: 2e38 3233 3530 312c 3234 2e37 3133 3534  .823501,24.71354
-0000bf40: 3720 3230 2e31 3236 3036 352c 3234 2e30  7 20.126065,24.0
-0000bf50: 3932 3630 3320 4320 3139 2e39 3231 3034  92603 C 19.92104
-0000bf60: 342c 3233 2e39 3130 3336 3920 3139 2e37  4,23.910369 19.7
-0000bf70: 3233 3333 362c 3233 2e37 3139 3935 3120  23336,23.719951 
-0000bf80: 3139 2e35 3332 3731 362c 3233 2e35 3232  19.532716,23.522
-0000bf90: 3732 3420 4320 3139 2e31 3131 3834 392c  724 C 19.111849,
-0000bfa0: 3234 2e36 3235 3639 3220 3138 2e36 3635  24.625692 18.665
-0000bfb0: 3233 372c 3235 2e37 3139 3834 3420 3138  237,25.719844 18
-0000bfc0: 2e31 3537 3134 2c32 362e 3738 3538 3520  .15714,26.78585 
-0000bfd0: 4320 3137 2e38 3430 3431 2c32 372e 3434  C 17.84041,27.44
-0000bfe0: 3634 3836 2031 372e 3530 3134 3638 2c32  6486 17.501468,2
-0000bff0: 382e 3039 3830 3735 2031 372e 3130 3638  8.098075 17.1068
-0000c000: 3131 2c32 382e 3731 3539 3838 2043 2031  11,28.715988 C 1
-0000c010: 362e 3836 3532 3837 2c32 392e 3039 3038  6.865287,29.0908
-0000c020: 3735 2031 362e 3630 3339 3834 2c32 392e  75 16.603984,29.
-0000c030: 3435 3538 3433 2031 362e 3239 3431 3637  455843 16.294167
-0000c040: 2c32 392e 3737 3738 3633 2043 2031 352e  ,29.777863 C 15.
-0000c050: 3934 3836 3435 2c33 302e 3133 3735 3332  948645,30.137532
-0000c060: 2031 352e 3532 3630 3936 2c33 302e 3431   15.526096,30.41
-0000c070: 3732 3820 3135 2e30 3734 3132 342c 3330  728 15.074124,30
-0000c080: 2e36 3235 3035 3320 4320 3134 2e35 3030  .625053 C 14.500
-0000c090: 3039 312c 3330 2e38 3839 3039 3520 3133  091,30.889095 13
-0000c0a0: 2e38 3832 3030 312c 3331 2e30 3435 3336  .882001,31.04536
-0000c0b0: 2031 332e 3235 3931 3032 2c33 312e 3134   13.259102,31.14
-0000c0c0: 3130 3433 2043 2031 322e 3631 3833 3234  1043 C 12.618324
-0000c0d0: 2c33 312e 3233 3838 3320 3131 2e39 3639  ,31.23883 11.969
-0000c0e0: 3235 352c 3331 2e32 3731 3436 3620 3131  255,31.271466 11
-0000c0f0: 2e33 3231 3536 362c 3331 2e32 3638 3936  .321566,31.26896
-0000c100: 3320 4320 3130 2e35 3938 3236 312c 3331  3 C 10.598261,31
-0000c110: 2e32 3638 3936 3320 392e 3837 3439 3537  .268963 9.874957
-0000c120: 322c 3331 2e32 3638 3936 3320 392e 3135  2,31.268963 9.15
-0000c130: 3136 3532 392c 3331 2e32 3638 3936 3320  16529,31.268963 
-0000c140: 4320 392e 3135 3136 3532 392c 3330 2e35  C 9.1516529,30.5
-0000c150: 3737 3932 3520 392e 3135 3136 3532 392c  77925 9.1516529,
-0000c160: 3239 2e38 3836 3838 3920 392e 3135 3136  29.886889 9.1516
-0000c170: 3532 392c 3239 2e31 3935 3835 3120 4320  529,29.195851 C 
-0000c180: 392e 3532 3834 3139 372c 3239 2e31 3935  9.5284197,29.195
-0000c190: 3734 3620 392e 3930 3531 3837 372c 3239  746 9.9051877,29
-0000c1a0: 2e31 3936 3037 2031 302e 3238 3139 3534  .19607 10.281954
-0000c1b0: 2c32 392e 3139 3536 3732 2043 2031 302e  ,29.195672 C 10.
-0000c1c0: 3938 3030 3735 2c32 392e 3139 3135 3120  980075,29.19151 
-0000c1d0: 3131 2e36 3830 3734 362c 3239 2e31 3434  11.680746,29.144
-0000c1e0: 3131 3620 3132 2e33 3635 3839 362c 3239  116 12.365896,29
-0000c1f0: 2e30 3034 3833 3520 4320 3132 2e38 3739  .004835 C 12.879
-0000c200: 3231 322c 3238 2e38 3939 3138 3520 3133  212,28.899185 13
-0000c210: 2e33 3836 3431 352c 3238 2e37 3430 3535  .386415,28.74055
-0000c220: 2031 332e 3834 3631 3737 2c32 382e 3438   13.846177,28.48
-0000c230: 3533 3932 2043 2031 342e 3138 3033 3836  5392 C 14.180386
-0000c240: 2c32 382e 3330 3030 3937 2031 342e 3438  ,28.300097 14.48
-0000c250: 3634 3734 2c32 382e 3035 3934 3520 3134  6474,28.05945 14
-0000c260: 2e37 3238 3638 2c32 372e 3736 3236 3937  .72868,27.762697
-0000c270: 2043 2031 342e 3936 3835 3239 2c32 372e   C 14.968529,27.
-0000c280: 3437 3031 3720 3135 2e31 3636 3836 2c32  47017 15.16686,2
-0000c290: 372e 3134 3633 3837 2031 352e 3335 3232  7.146387 15.3522
-0000c2a0: 3038 2c32 362e 3831 3734 3438 2043 2031  08,26.817448 C 1
-0000c2b0: 352e 3638 3436 3835 2c32 362e 3232 3037  5.684685,26.2207
-0000c2c0: 3238 2031 352e 3936 3933 3631 2c32 352e  28 15.969361,25.
-0000c2d0: 3539 3837 3937 2031 362e 3233 3739 3038  598797 16.237908
-0000c2e0: 2c32 342e 3937 3131 3639 2043 2031 362e  ,24.971169 C 16.
-0000c2f0: 3639 3936 3239 2c32 332e 3838 3437 3238  699629,23.884728
-0000c300: 2031 372e 3130 3735 3133 2c32 322e 3737   17.107513,22.77
-0000c310: 3632 3734 2031 372e 3439 3439 3635 2c32  6274 17.494965,2
-0000c320: 312e 3636 3134 3831 2043 2031 372e 3535  1.661481 C 17.55
-0000c330: 3831 312c 3231 2e34 3739 3335 3220 3137  811,21.479352 17
-0000c340: 2e36 3230 362c 3231 2e32 3936 3939 3520  .6206,21.296995 
-0000c350: 3137 2e36 3832 3530 322c 3231 2e31 3134  17.682502,21.114
-0000c360: 3433 3820 4320 3137 2e33 3832 3230 362c  438 C 17.382206,
-0000c370: 3230 2e35 3835 3939 3420 3137 2e31 3030  20.585994 17.100
-0000c380: 3433 352c 3230 2e30 3435 3733 3520 3136  435,20.045735 16
-0000c390: 2e38 3637 3435 2c31 392e 3438 3339 3237  .86745,19.483927
-0000c3a0: 2043 2031 362e 3732 3734 3438 2c31 392e   C 16.727448,19.
-0000c3b0: 3134 3439 3036 2031 362e 3630 3633 3136  144906 16.606316
-0000c3c0: 2c31 382e 3739 3639 3737 2031 362e 3532  ,18.796977 16.52
-0000c3d0: 3731 3337 2c31 382e 3433 3834 3038 2043  7137,18.438408 C
-0000c3e0: 2031 362e 3433 3239 3631 2c31 382e 3031   16.432961,18.01
-0000c3f0: 3836 3239 2031 362e 3336 3236 3035 2c31  8629 16.362605,1
-0000c400: 372e 3539 3339 3631 2031 362e 3239 3439  7.593961 16.2949
-0000c410: 3534 2c31 372e 3136 3932 3436 2043 2031  54,17.169246 C 1
-0000c420: 362e 3134 3531 3632 2c31 362e 3231 3131  6.145162,16.2111
-0000c430: 3032 2031 362e 3032 3233 3138 2c31 352e  02 16.022318,15.
-0000c440: 3234 3920 3135 2e39 3033 3436 372c 3134  249 15.903467,14
-0000c450: 2e32 3836 3631 3220 4320 3135 2e36 3933  .286612 C 15.693
-0000c460: 3437 382c 3132 2e37 3035 3938 3620 3135  478,12.705986 15
-0000c470: 2e34 3833 3438 392c 3131 2e31 3235 3336  .483489,11.12536
-0000c480: 3120 3135 2e32 3733 352c 392e 3534 3437  1 15.2735,9.5447
-0000c490: 3334 3420 4320 3135 2e31 3230 3637 362c  344 C 15.120676,
-0000c4a0: 382e 3338 3030 3135 3320 3134 2e39 3434  8.3800153 14.944
-0000c4b0: 3731 332c 372e 3231 3735 3633 2031 342e  713,7.217563 14.
-0000c4c0: 3730 3935 352c 362e 3036 3633 3436 3520  70955,6.0663465 
-0000c4d0: 4320 3134 2e35 3635 3539 342c 352e 3336  C 14.565594,5.36
-0000c4e0: 3935 3834 3720 3134 2e34 3031 3834 362c  95847 14.401846,
-0000c4f0: 342e 3637 3537 3035 3420 3134 2e31 3832  4.6757054 14.182
-0000c500: 3832 2c33 2e39 3938 3330 3932 2043 2031  82,3.9983092 C 1
-0000c510: 342e 3037 3932 3334 2c33 2e36 3830 3838  4.079234,3.68088
-0000c520: 3334 2031 332e 3936 3333 3434 2c33 2e33  34 13.963344,3.3
-0000c530: 3636 3833 3535 2031 332e 3832 3036 3438  668355 13.820648
-0000c540: 2c33 2e30 3634 3730 3733 2043 2031 332e  ,3.0647073 C 13.
-0000c550: 3033 3333 3332 2c33 2e39 3937 3731 3231  033332,3.9977121
-0000c560: 2031 322e 3337 3036 3835 2c35 2e30 3330   12.370685,5.030
-0000c570: 3339 3735 2031 312e 3739 3534 3637 2c36  3975 11.795467,6
-0000c580: 2e31 3035 3532 3039 2043 2031 312e 3133  .1055209 C 11.13
-0000c590: 3039 3032 2c37 2e33 3439 3636 2031 302e  0902,7.34966 10.
-0000c5a0: 3538 3238 332c 382e 3635 3331 3334 3820  58283,8.6531348 
-0000c5b0: 3130 2e31 3038 3630 362c 392e 3938 3035  10.108606,9.9805
-0000c5c0: 3934 3520 4320 392e 3538 3737 3835 352c  945 C 9.5877855,
-0000c5d0: 3131 2e34 3237 3930 3620 392e 3135 3834  11.427906 9.1584
-0000c5e0: 3635 322c 3132 2e39 3131 3431 3320 382e  652,12.911413 8.
-0000c5f0: 3838 3732 3838 352c 3134 2e34 3236 3630  8872885,14.42660
-0000c600: 3320 4320 382e 3639 3830 3536 342c 3135  3 C 8.6980564,15
-0000c610: 2e34 3836 3537 3520 382e 3538 3831 3032  .486575 8.588102
-0000c620: 382c 3136 2e35 3632 3438 3720 382e 3539  8,16.562487 8.59
-0000c630: 3238 3633 372c 3137 2e36 3339 3835 3520  28637,17.639855 
-0000c640: 4320 382e 3539 3238 3633 372c 3138 2e30  C 8.5928637,18.0
-0000c650: 3631 3439 3520 382e 3539 3238 3633 372c  61495 8.5928637,
-0000c660: 3138 2e34 3833 3133 3420 382e 3539 3238  18.483134 8.5928
-0000c670: 3633 372c 3138 2e39 3034 3737 3420 4320  637,18.904774 C 
-0000c680: 372e 3736 3530 3237 332c 3138 2e39 3034  7.7650273,18.904
-0000c690: 3737 3420 362e 3933 3731 3932 322c 3138  774 6.9371922,18
-0000c6a0: 2e39 3034 3737 3420 362e 3130 3933 3535  .904774 6.109355
-0000c6b0: 392c 3138 2e39 3034 3737 3420 7a20 4d20  9,18.904774 z M 
-0000c6c0: 3230 2e30 3931 3530 352c 3231 2e34 3132  20.091505,21.412
-0000c6d0: 3337 2043 2032 302e 3730 3339 3839 2c32  37 C 20.703989,2
-0000c6e0: 322e 3039 3133 3033 2032 312e 3337 3632  2.091303 21.3762
-0000c6f0: 3136 2c32 322e 3732 3230 3220 3232 2e31  16,22.72202 22.1
-0000c700: 3330 3836 372c 3233 2e32 3431 3230 3620  30867,23.241206 
-0000c710: 4320 3232 2e37 3630 3237 362c 3233 2e36  C 22.760276,23.6
-0000c720: 3733 3638 2032 332e 3435 3131 3536 2c32  7368 23.451156,2
-0000c730: 342e 3032 3633 3035 2032 342e 3138 3938  4.026305 24.1898
-0000c740: 3735 2c32 342e 3232 3831 3739 2043 2032  75,24.228179 C 2
-0000c750: 342e 3835 3138 3136 2c32 342e 3431 3034  4.851816,24.4104
-0000c760: 3036 2032 352e 3535 3034 3239 2c32 342e  06 25.550429,24.
-0000c770: 3436 3436 3431 2032 362e 3233 3134 3037  464641 26.231407
-0000c780: 2c32 342e 3337 3235 3836 2043 2032 362e  ,24.372586 C 26.
-0000c790: 3734 3335 3132 2c32 342e 3330 3335 3633  743512,24.303563
-0000c7a0: 2032 372e 3234 3433 3532 2c32 342e 3134   27.244352,24.14
-0000c7b0: 3234 3439 2032 372e 3639 3437 3337 2c32  2449 27.694737,2
-0000c7c0: 332e 3838 3830 3837 2043 2032 382e 3037  3.888087 C 28.07
-0000c7d0: 3339 3939 2c32 332e 3637 3533 3734 2032  3999,23.675374 2
-0000c7e0: 382e 3431 3536 3539 2c32 332e 3339 3839  8.415659,23.3989
-0000c7f0: 3435 2032 382e 3731 3335 3137 2c32 332e  45 28.713517,23.
-0000c800: 3038 3238 3537 2043 2032 392e 3038 3334  082857 C 29.0834
-0000c810: 3837 2c32 322e 3639 3632 3332 2032 392e  87,22.696232 29.
-0000c820: 3338 3137 3035 2c32 322e 3234 3035 3737  381705,22.240577
-0000c830: 2032 392e 3538 3235 3037 2c32 312e 3734   29.582507,21.74
-0000c840: 3433 3532 2043 2032 392e 3830 3637 3536  4352 C 29.806756
-0000c850: 2c32 312e 3139 3435 3034 2032 392e 3931  ,21.194504 29.91
-0000c860: 3138 3934 2c32 302e 3630 3037 3637 2032  1894,20.600767 2
-0000c870: 392e 3932 3436 3736 2c32 302e 3030 3834  9.924676,20.0084
-0000c880: 3820 4320 3239 2e39 3337 3535 332c 3139  8 C 29.937553,19
-0000c890: 2e35 3135 3135 3620 3239 2e38 3739 3034  .515156 29.87904
-0000c8a0: 362c 3139 2e30 3137 3932 3120 3239 2e37  6,19.017921 29.7
-0000c8b0: 3239 3435 352c 3138 2e35 3436 3735 3620  29455,18.546756 
-0000c8c0: 4320 3239 2e35 3736 3730 392c 3138 2e30  C 29.576709,18.0
-0000c8d0: 3630 3535 3820 3239 2e33 3236 3834 312c  60558 29.326841,
-0000c8e0: 3137 2e36 3036 3339 3520 3239 2e30 3035  17.606395 29.005
-0000c8f0: 3334 2c31 372e 3231 3134 3120 4320 3238  34,17.21141 C 28
-0000c900: 2e36 3531 3434 332c 3136 2e37 3736 3531  .651443,16.77651
-0000c910: 3320 3238 2e32 3139 3438 392c 3136 2e34  3 28.219489,16.4
-0000c920: 3030 3533 3720 3237 2e37 3232 3732 372c  00537 27.722727,
-0000c930: 3136 2e31 3337 3336 3420 4320 3237 2e32  16.137364 C 27.2
-0000c940: 3835 3137 352c 3135 2e39 3033 3934 3620  85175,15.903946 
-0000c950: 3236 2e38 3030 3536 332c 3135 2e37 3632  26.800563,15.762
-0000c960: 3430 3220 3236 2e33 3037 3630 322c 3135  402 26.307602,15
-0000c970: 2e37 3132 3532 3820 4320 3235 2e36 3338  .712528 C 25.638
-0000c980: 3532 392c 3135 2e36 3434 3838 3920 3234  529,15.644889 24
-0000c990: 2e39 3532 3537 362c 3135 2e37 3235 3134  .952576,15.72514
-0000c9a0: 3620 3234 2e33 3232 3838 372c 3135 2e39  6 24.322887,15.9
-0000c9b0: 3633 3839 3620 4320 3233 2e37 3331 3738  63896 C 23.73178
-0000c9c0: 312c 3136 2e31 3835 3738 3120 3233 2e31  1,16.185781 23.1
-0000c9d0: 3936 3933 362c 3136 2e35 3431 3432 2032  96936,16.54142 2
-0000c9e0: 322e 3733 3533 382c 3136 2e39 3639 3534  2.73538,16.96954
-0000c9f0: 3220 4320 3232 2e31 3730 3139 372c 3137  2 C 22.170197,17
-0000ca00: 2e34 3933 3337 3620 3231 2e37 3037 3137  .493376 21.70717
-0000ca10: 362c 3138 2e31 3138 3236 3320 3231 2e33  6,18.118263 21.3
-0000ca20: 3132 3536 2c31 382e 3737 3737 2043 2032  1256,18.7777 C 2
-0000ca30: 302e 3831 3539 3833 2c31 392e 3631 3038  0.815983,19.6108
-0000ca40: 3337 2032 302e 3432 3433 3731 2c32 302e  37 20.424371,20.
-0000ca50: 3530 3236 3837 2032 302e 3039 3135 3035  502687 20.091505
-0000ca60: 2c32 312e 3431 3233 3720 7a20 220a 2020  ,21.41237 z ".  
-0000ca70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca80: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-0000ca90: 6c3a 2024 7a6f 6469 6163 5f63 6f6c 6f72  l: $zodiac_color
-0000caa0: 5f39 220a 2020 2020 2020 2020 2020 2020  _9".            
-0000cab0: 2020 2020 2020 2020 2f3e 0a20 2020 2020          />.     
-0000cac0: 2020 2020 2020 2020 2020 203c 2f73 796d             </sym
-0000cad0: 626f 6c3e 0a20 2020 2020 2020 2020 2020  bol>.           
-0000cae0: 2020 2020 203c 7379 6d62 6f6c 2069 643d       <symbol id=
-0000caf0: 2261 7175 6172 6975 7322 3e0a 2020 2020  "aquarius">.    
-0000cb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb10: 3c70 6174 680a 2020 2020 2020 2020 2020  <path.          
-0000cb20: 2020 2020 2020 2020 2020 2020 2020 643d                d=
-0000cb30: 224d 2032 652d 3036 2c32 342e 3730 3136  "M 2e-06,24.7016
-0000cb40: 3537 204c 2039 2e36 3737 3131 2c31 382e  57 L 9.67711,18.
-0000cb50: 3332 3236 3834 204c 2031 312e 3739 3735  322684 L 11.7975
-0000cb60: 3932 2c32 332e 3236 3431 3432 204c 2031  92,23.264142 L 1
-0000cb70: 392e 3238 3939 3631 2c31 382e 3332 3236  9.289961,18.3226
-0000cb80: 3834 204c 2032 312e 3338 3437 342c 3233  84 L 21.38474,23
-0000cb90: 2e32 3634 3134 3220 4c20 3238 2e38 3839  .264142 L 28.889
-0000cba0: 3936 2c31 382e 3332 3236 3834 204c 2033  96,18.322684 L 3
-0000cbb0: 312e 3938 3731 3439 2c32 352e 3630 3031  1.987149,25.6001
-0000cbc0: 3034 204c 2032 392e 3938 3233 332c 3236  04 L 29.98233,26
-0000cbd0: 2e34 3835 3731 3620 4c20 3237 2e39 3133  .485716 L 27.913
-0000cbe0: 3235 332c 3231 2e35 3434 3235 3820 4c20  253,21.544258 L 
-0000cbf0: 3230 2e33 3832 3333 2c32 362e 3438 3537  20.38233,26.4857
-0000cc00: 3136 204c 2031 382e 3238 3735 3531 2c32  16 L 18.287551,2
-0000cc10: 312e 3534 3432 3538 204c 2031 302e 3832  1.544258 L 10.82
-0000cc20: 3038 3835 2c32 362e 3438 3537 3136 204c  0885,26.485716 L
-0000cc30: 2038 2e37 3133 3235 342c 3231 2e35 3434   8.713254,21.544
-0000cc40: 3235 3820 4c20 312e 3138 3233 3331 2c32  258 L 1.182331,2
-0000cc50: 362e 3438 3537 3136 204c 2032 652d 3036  6.485716 L 2e-06
-0000cc60: 2c32 342e 3730 3136 3537 207a 204d 2030  ,24.701657 z M 0
-0000cc70: 2e30 3132 3835 332c 3131 2e33 3931 3830  .012853,11.39180
-0000cc80: 3820 4c20 392e 3638 3939 3631 2c35 204c  8 L 9.689961,5 L
-0000cc90: 2031 312e 3831 3034 3433 2c39 2e39 3431   11.810443,9.941
-0000cca0: 3435 3820 4c20 3139 2e33 3135 3636 342c  458 L 19.315664,
-0000ccb0: 3520 4c20 3231 2e34 3130 3434 332c 392e  5 L 21.410443,9.
-0000ccc0: 3934 3134 3538 204c 2032 382e 3930 3238  941458 L 28.9028
-0000ccd0: 3132 2c35 204c 2033 322c 3132 2e32 3737  12,5 L 32,12.277
-0000cce0: 3432 204c 2032 392e 3939 3531 3831 2c31  42 L 29.995181,1
-0000ccf0: 332e 3136 3330 3332 204c 2032 372e 3932  3.163032 L 27.92
-0000cd00: 3631 3035 2c38 2e32 3231 3537 3420 4c20  6105,8.221574 L 
-0000cd10: 3230 2e33 3832 3333 2c31 332e 3136 3330  20.38233,13.1630
-0000cd20: 3332 204c 2031 382e 3238 3735 3531 2c38  32 L 18.287551,8
-0000cd30: 2e32 3231 3537 3420 4c20 3130 2e38 3230  .221574 L 10.820
-0000cd40: 3838 352c 3133 2e31 3633 3033 3220 4c20  885,13.163032 L 
-0000cd50: 382e 3733 3839 3537 2c38 2e32 3231 3537  8.738957,8.22157
-0000cd60: 3420 4c20 312e 3230 3830 3334 2c31 332e  4 L 1.208034,13.
-0000cd70: 3136 3330 3332 204c 2030 2e30 3132 3835  163032 L 0.01285
-0000cd80: 332c 3131 2e33 3931 3830 3820 7a20 220a  3,11.391808 z ".
-0000cd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cda0: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
-0000cdb0: 696c 6c3a 2024 7a6f 6469 6163 5f63 6f6c  ill: $zodiac_col
-0000cdc0: 6f72 5f31 3022 0a20 2020 2020 2020 2020  or_10".         
-0000cdd0: 2020 2020 2020 2020 2020 202f 3e0a 2020             />.  
-0000cde0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-0000cdf0: 7379 6d62 6f6c 3e0a 2020 2020 2020 2020  symbol>.        
-0000ce00: 2020 2020 2020 2020 3c73 796d 626f 6c20          <symbol 
-0000ce10: 6964 3d22 7069 7363 6573 223e 0a20 2020  id="pisces">.   
-0000ce20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce30: 203c 7061 7468 0a20 2020 2020 2020 2020   <path.         
-0000ce40: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000ce50: 3d22 4d20 3133 2e32 3838 3132 322c 3136  ="M 13.288122,16
-0000ce60: 2e34 3933 3539 3320 4320 3133 2e32 3838  .493593 C 13.288
-0000ce70: 3334 312c 3138 2e30 3633 3639 3920 3133  341,18.063699 13
-0000ce80: 2e30 3534 3638 2c31 392e 3632 3833 3632  .05468,19.628362
-0000ce90: 2031 322e 3635 3939 3235 2c32 312e 3134   12.659925,21.14
-0000cea0: 3631 3536 2043 2031 322e 3335 3737 3034  6156 C 12.357704
-0000ceb0: 2c32 322e 3330 3732 3434 2031 312e 3936  ,22.307244 11.96
-0000cec0: 3332 3133 2c32 332e 3434 3334 3039 2031  3213,23.443409 1
-0000ced0: 312e 3530 3033 372c 3234 2e35 3439 3935  1.50037,24.54995
-0000cee0: 3820 4320 3130 2e36 3836 3138 382c 3236  8 C 10.686188,26
-0000cef0: 2e34 3738 3439 3320 392e 3636 3631 3735  .478493 9.666175
-0000cf00: 372c 3238 2e33 3232 3035 3320 382e 3434  7,28.322053 8.44
-0000cf10: 3037 3139 372c 3330 2e30 3230 3037 3620  07197,30.020076 
-0000cf20: 4320 372e 3934 3730 3935 372c 3330 2e37  C 7.9470957,30.7
-0000cf30: 3034 3635 2037 2e34 3230 3738 3037 2c33  0465 7.4207807,3
-0000cf40: 312e 3336 3536 3439 2036 2e38 3634 3039  1.365649 6.86409
-0000cf50: 3237 2c33 3220 4320 352e 3735 3534 3534  27,32 C 5.755454
-0000cf60: 2c33 3220 342e 3634 3638 3135 332c 3332  ,32 4.6468153,32
-0000cf70: 2033 2e35 3338 3137 3636 2c33 3220 4320   3.5381766,32 C 
-0000cf80: 352e 3035 3232 3033 342c 3330 2e34 3034  5.0522034,30.404
-0000cf90: 3035 3520 362e 3430 3937 3932 372c 3238  055 6.4097927,28
-0000cfa0: 2e36 3530 3837 3220 372e 3439 3831 3530  .650872 7.498150
-0000cfb0: 372c 3236 2e37 3336 3333 3520 4320 382e  7,26.736335 C 8.
-0000cfc0: 3433 3235 3034 372c 3235 2e30 3935 3232  4325047,25.09522
-0000cfd0: 3620 392e 3136 3330 3030 372c 3233 2e33  6 9.1630007,23.3
-0000cfe0: 3334 3839 3620 392e 3632 3835 3737 372c  34896 9.6285777,
-0000cff0: 3231 2e35 3033 3537 3920 4320 3130 2e30  21.503579 C 10.0
-0000d000: 3436 3233 382c 3139 2e38 3638 3633 3620  46238,19.868636 
-0000d010: 3130 2e32 3531 3637 352c 3138 2e31 3830  10.251675,18.180
-0000d020: 3731 3120 3130 2e32 3530 3735 362c 3136  711 10.250756,16
-0000d030: 2e34 3933 3539 3320 4320 382e 3038 3931  .493593 C 8.0891
-0000d040: 3633 372c 3136 2e34 3933 3539 3320 352e  637,16.493593 5.
-0000d050: 3932 3735 3730 372c 3136 2e34 3933 3539  9275707,16.49359
-0000d060: 3320 332e 3736 3539 3739 312c 3136 2e34  3 3.7659791,16.4
-0000d070: 3933 3539 3320 4320 332e 3736 3539 3739  93593 C 3.765979
-0000d080: 312c 3135 2e37 3334 3231 3920 332e 3736  1,15.734219 3.76
-0000d090: 3539 3739 312c 3134 2e39 3734 3834 3620  59791,14.974846 
-0000d0a0: 332e 3736 3539 3739 312c 3134 2e32 3135  3.7659791,14.215
-0000d0b0: 3437 3220 4320 352e 3932 3735 3730 372c  472 C 5.9275707,
-0000d0c0: 3134 2e32 3135 3437 3220 382e 3038 3931  14.215472 8.0891
-0000d0d0: 3633 372c 3134 2e32 3135 3437 3220 3130  637,14.215472 10
-0000d0e0: 2e32 3530 3735 362c 3134 2e32 3135 3437  .250756,14.21547
-0000d0f0: 3220 4320 3130 2e31 3535 3936 322c 3132  2 C 10.155962,12
-0000d100: 2e34 3937 3939 3120 392e 3831 3234 3836  .497991 9.812486
-0000d110: 372c 3130 2e37 3936 3437 2039 2e32 3534  7,10.79647 9.254
-0000d120: 3634 3837 2c39 2e31 3730 3034 3320 4320  6487,9.170043 C 
-0000d130: 382e 3631 3035 3436 372c 372e 3238 3634  8.6105467,7.2864
-0000d140: 2037 2e36 3836 3231 3037 2c35 2e35 3035   7.6862107,5.505
-0000d150: 3639 3120 362e 3538 3330 3636 372c 332e  691 6.5830667,3.
-0000d160: 3835 3132 3534 2043 2035 2e36 3734 3330  851254 C 5.67430
-0000d170: 3331 2c32 2e34 3837 3930 3820 342e 3634  31,2.487908 4.64
-0000d180: 3531 3235 2c31 2e32 3037 3039 3839 2033  5125,1.2070989 3
-0000d190: 2e35 3338 3137 3636 2c33 652d 3037 2043  .5381766,3e-07 C
-0000d1a0: 2034 2e35 3836 3036 382c 3365 2d30 3720   4.586068,3e-07 
-0000d1b0: 352e 3633 3339 3539 332c 3365 2d30 3720  5.6339593,3e-07 
-0000d1c0: 362e 3638 3138 3530 372c 3365 2d30 3720  6.6818507,3e-07 
-0000d1d0: 4320 382e 3135 3939 3339 372c 312e 3537  C 8.1599397,1.57
-0000d1e0: 3538 3437 3620 392e 3436 3235 3835 372c  58476 9.4625857,
-0000d1f0: 332e 3332 3136 3520 3130 2e35 3034 3333  3.32165 10.50433
-0000d200: 352c 352e 3231 3632 3331 2043 2031 312e  5,5.216231 C 11.
-0000d210: 3436 3030 3434 2c36 2e39 3530 3234 3820  460044,6.950248 
-0000d220: 3132 2e31 3933 3035 362c 382e 3830 3639  12.193056,8.8069
-0000d230: 3139 2031 322e 3637 3637 3238 2c31 302e  19 12.676728,10.
-0000d240: 3732 3639 3835 2043 2031 322e 3936 3631  726985 C 12.9661
-0000d250: 3731 2c31 312e 3837 3236 3435 2031 332e  71,11.872645 13.
-0000d260: 3136 3833 3634 2c31 332e 3034 3030 3036  168364,13.040006
-0000d270: 2031 332e 3238 3831 3232 2c31 342e 3231   13.288122,14.21
-0000d280: 3534 3732 2043 2031 352e 3338 3339 3035  5472 C 15.383905
-0000d290: 2c31 342e 3231 3534 3732 2031 372e 3437  ,14.215472 17.47
-0000d2a0: 3936 3838 2c31 342e 3231 3534 3732 2031  9688,14.215472 1
-0000d2b0: 392e 3537 3534 372c 3134 2e32 3135 3437  9.57547,14.21547
-0000d2c0: 3220 4320 3139 2e37 3836 3838 322c 3132  2 C 19.786882,12
-0000d2d0: 2e31 3837 3735 3820 3230 2e32 3435 3838  .187758 20.24588
-0000d2e0: 342c 3130 2e31 3834 3133 2032 302e 3936  4,10.18413 20.96
-0000d2f0: 3332 3439 2c38 2e32 3735 3034 3120 4320  3249,8.275041 C 
-0000d300: 3231 2e36 3730 3432 392c 362e 3338 3637  21.670429,6.3867
-0000d310: 3732 2032 322e 3632 3836 3535 2c34 2e35  72 22.628655,4.5
-0000d320: 3934 3834 3920 3233 2e37 3836 3533 332c  94849 23.786533,
-0000d330: 322e 3934 3439 3136 2043 2032 342e 3531  2.944916 C 24.51
-0000d340: 3334 3135 2c31 2e39 3037 3832 3239 2032  3415,1.9078229 2
-0000d350: 352e 3331 3735 3838 2c30 2e39 3235 3536  5.317588,0.92556
-0000d360: 3837 2032 362e 3138 3137 3432 2c33 652d  87 26.181742,3e-
-0000d370: 3037 2043 2032 372e 3232 3936 3333 2c33  07 C 27.229633,3
-0000d380: 652d 3037 2032 382e 3237 3735 3235 2c33  e-07 28.277525,3
-0000d390: 652d 3037 2032 392e 3332 3534 3136 2c33  e-07 29.325416,3
-0000d3a0: 652d 3037 2043 2032 372e 3835 3436 3138  e-07 C 27.854618
-0000d3b0: 2c31 2e36 3034 3038 3837 2032 362e 3531  ,1.6040887 26.51
-0000d3c0: 3838 3439 2c33 2e33 3430 3034 3720 3235  8849,3.340047 25
-0000d3d0: 2e34 3234 3932 312c 352e 3232 3430 3136  .424921,5.224016
-0000d3e0: 2043 2032 342e 3437 3034 3538 2c36 2e38   C 24.470458,6.8
-0000d3f0: 3637 3033 2032 332e 3730 3439 3935 2c38  6703 23.704995,8
-0000d400: 2e36 3235 3439 3820 3233 2e32 3135 3137  .625498 23.21517
-0000d410: 352c 3130 2e34 3633 3336 3420 4320 3232  5,10.463364 C 22
-0000d420: 2e38 3837 3534 372c 3131 2e36 3839 3233  .887547,11.68923
-0000d430: 3220 3232 2e36 3833 3238 312c 3132 2e39  2 22.683281,12.9
-0000d440: 3438 3339 3220 3232 2e36 3132 3833 372c  48392 22.612837,
-0000d450: 3134 2e32 3135 3437 3220 4320 3234 2e37  14.215472 C 24.7
-0000d460: 3734 3432 382c 3134 2e32 3135 3437 3220  74428,14.215472 
-0000d470: 3236 2e39 3336 3032 322c 3134 2e32 3135  26.936022,14.215
-0000d480: 3437 3220 3239 2e30 3937 3631 342c 3134  472 29.097614,14
-0000d490: 2e32 3135 3437 3220 4320 3239 2e30 3937  .215472 C 29.097
-0000d4a0: 3631 342c 3134 2e39 3734 3834 3620 3239  614,14.974846 29
-0000d4b0: 2e30 3937 3631 342c 3135 2e37 3334 3231  .097614,15.73421
-0000d4c0: 3920 3239 2e30 3937 3631 342c 3136 2e34  9 29.097614,16.4
-0000d4d0: 3933 3539 3320 4320 3236 2e39 3336 3032  93593 C 26.93602
-0000d4e0: 322c 3136 2e34 3933 3539 3320 3234 2e37  2,16.493593 24.7
-0000d4f0: 3734 3432 382c 3136 2e34 3933 3539 3320  74428,16.493593 
-0000d500: 3232 2e36 3132 3833 372c 3136 2e34 3933  22.612837,16.493
-0000d510: 3539 3320 4320 3232 2e36 3131 3539 312c  593 C 22.611591,
-0000d520: 3138 2e33 3130 3031 3320 3232 2e38 3530  18.310013 22.850
-0000d530: 3534 342c 3230 2e31 3237 3334 3720 3233  544,20.127347 23
-0000d540: 2e33 3334 3435 342c 3231 2e38 3738 3532  .334454,21.87852
-0000d550: 3420 4320 3233 2e38 3337 3332 322c 3233  4 C 23.837322,23
-0000d560: 2e37 3037 3239 3320 3234 2e36 3034 3336  .707293 24.60436
-0000d570: 392c 3235 2e34 3539 3439 3420 3235 2e35  9,25.459494 25.5
-0000d580: 3730 3639 342c 3237 2e30 3930 3130 3520  70694,27.090105 
-0000d590: 4320 3236 2e36 3232 3732 372c 3238 2e38  C 26.622727,28.8
-0000d5a0: 3637 3736 3520 3237 2e39 3035 3038 332c  67765 27.905083,
-0000d5b0: 3330 2e35 3032 3732 3320 3239 2e33 3235  30.502723 29.325
-0000d5c0: 3431 362c 3332 2043 2032 382e 3232 3138  416,32 C 28.2218
-0000d5d0: 3339 2c33 3220 3237 2e31 3138 3236 342c  39,32 27.118264,
-0000d5e0: 3332 2032 362e 3031 3436 3837 2c33 3220  32 26.014687,32 
-0000d5f0: 4320 3234 2e36 3934 3433 352c 3330 2e35  C 24.694435,30.5
-0000d600: 3038 3337 3720 3233 2e35 3439 3139 372c  08377 23.549197,
-0000d610: 3238 2e38 3633 3331 3520 3232 2e35 3937  28.863315 22.597
-0000d620: 3331 332c 3237 2e31 3133 3832 3120 4320  313,27.113821 C 
-0000d630: 3232 2e31 3034 3238 2c32 362e 3230 3737  22.10428,26.2077
-0000d640: 3938 2032 312e 3636 3035 3333 2c32 352e  98 21.660533,25.
-0000d650: 3237 3439 3120 3231 2e32 3638 3236 352c  27491 21.268265,
-0000d660: 3234 2e33 3230 3933 3520 4320 3230 2e36  24.320935 C 20.6
-0000d670: 3233 3633 342c 3232 2e37 3337 3733 3920  23634,22.737739 
-0000d680: 3230 2e31 3135 3631 332c 3231 2e30 3933  20.115613,21.093
-0000d690: 3732 3920 3139 2e38 3238 3932 322c 3139  729 19.828922,19
-0000d6a0: 2e34 3036 3732 3120 4320 3139 2e36 3635  .406721 C 19.665
-0000d6b0: 3538 352c 3138 2e34 3434 3736 3820 3139  585,18.444768 19
-0000d6c0: 2e35 3735 3430 322c 3137 2e34 3639 3630  .575402,17.46960
-0000d6d0: 3320 3139 2e35 3735 3437 2c31 362e 3439  3 19.57547,16.49
-0000d6e0: 3335 3933 2043 2031 372e 3437 3936 3838  3593 C 17.479688
-0000d6f0: 2c31 362e 3439 3335 3933 2031 352e 3338  ,16.493593 15.38
-0000d700: 3339 3035 2c31 362e 3439 3335 3933 2031  3905,16.493593 1
-0000d710: 332e 3238 3831 3232 2c31 362e 3439 3335  3.288122,16.4935
-0000d720: 3933 207a 2022 0a20 2020 2020 2020 2020  93 z ".         
-0000d730: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000d740: 7479 6c65 3d22 6669 6c6c 3a20 247a 6f64  tyle="fill: $zod
-0000d750: 6961 635f 636f 6c6f 725f 3131 220a 2020  iac_color_11".  
-0000d760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d770: 2020 2f3e 0a20 2020 2020 2020 2020 2020    />.           
-0000d780: 2020 2020 203c 2f73 796d 626f 6c3e 0a20       </symbol>. 
-0000d790: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000d7a0: 212d 2d20 4173 7065 6374 7320 3132 7831  !-- Aspects 12x1
-0000d7b0: 3220 2d2d 3e0a 2020 2020 2020 2020 2020  2 -->.          
-0000d7c0: 2020 2020 2020 3c73 796d 626f 6c20 6964        <symbol id
-0000d7d0: 3d22 6f72 6230 223e 0a20 2020 2020 2020  ="orb0">.       
-0000d7e0: 2020 2020 2020 2020 2020 2020 203c 7061               <pa
-0000d7f0: 7468 0a20 2020 2020 2020 2020 2020 2020  th.             
-0000d800: 2020 2020 2020 2020 2020 2064 3d22 4d20             d="M 
-0000d810: 362e 3036 3937 3533 392c 372e 3332 3334  6.0697539,7.3234
-0000d820: 3835 3220 4320 362e 3036 3937 3533 392c  852 C 6.0697539,
-0000d830: 382e 3733 3534 3838 3220 342e 3931 3733  8.7354882 4.9173
-0000d840: 3635 312c 392e 3838 3031 3434 3220 332e  651,9.8801442 3.
-0000d850: 3439 3538 3231 342c 392e 3838 3031 3434  4958214,9.880144
-0000d860: 3220 4320 322e 3037 3432 3737 352c 392e  2 C 2.0742775,9.
-0000d870: 3838 3031 3434 3220 302e 3932 3138 3838  8801442 0.921888
-0000d880: 3537 2c38 2e37 3335 3438 3832 2030 2e39  57,8.7354882 0.9
-0000d890: 3231 3838 3835 372c 372e 3332 3334 3835  2188857,7.323485
-0000d8a0: 3220 4320 302e 3932 3138 3838 3537 2c35  2 C 0.92188857,5
-0000d8b0: 2e39 3131 3438 3232 2032 2e30 3734 3237  .9114822 2.07427
-0000d8c0: 3735 2c34 2e37 3636 3832 3732 2033 2e34  75,4.7668272 3.4
-0000d8d0: 3935 3832 3134 2c34 2e37 3636 3832 3732  958214,4.7668272
-0000d8e0: 2043 2034 2e39 3137 3336 3531 2c34 2e37   C 4.9173651,4.7
-0000d8f0: 3636 3832 3732 2036 2e30 3639 3735 3339  668272 6.0697539
-0000d900: 2c35 2e39 3131 3438 3232 2036 2e30 3639  ,5.9114822 6.069
-0000d910: 3735 3339 2c37 2e33 3233 3438 3532 204c  7539,7.3234852 L
-0000d920: 2036 2e30 3639 3735 3339 2c37 2e33 3233   6.0697539,7.323
-0000d930: 3438 3532 207a 204d 2035 2e36 3235 3236  4852 z M 5.62526
-0000d940: 3039 2c35 2e32 3131 3332 3032 2043 2031  09,5.2113202 C 1
-0000d950: 302e 3037 3031 392c 302e 3736 3633 3930  0.07019,0.766390
-0000d960: 3138 2031 302e 3037 3031 392c 302e 3736  18 10.07019,0.76
-0000d970: 3633 3930 3138 2031 302e 3037 3031 392c  639018 10.07019,
-0000d980: 302e 3736 3633 3930 3138 220a 2020 2020  0.76639018".    
-0000d990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9a0: 2020 2020 7374 796c 653d 220a 2020 2020      style=".    
+00004570: 3c2f 7379 6d62 6f6c 3e0a 2020 2020 2020  </symbol>.      
+00004580: 2020 2020 2020 2020 2020 3c73 796d 626f            <symbo
+00004590: 6c20 6964 3d22 4669 7273 745f 486f 7573  l id="First_Hous
+000045a0: 6522 3e0a 2020 2020 2020 2020 2020 2020  e">.            
+000045b0: 2020 2020 2020 2020 3c74 6578 7420 793d          <text y=
+000045c0: 2232 3022 2073 7479 6c65 3d22 666f 6e74  "20" style="font
+000045d0: 2d73 697a 653a 2032 3270 783b 2066 696c  -size: 22px; fil
+000045e0: 6c3a 2024 706c 616e 6574 735f 636f 6c6f  l: $planets_colo
+000045f0: 725f 3132 223e 4173 3c2f 7465 7874 3e0a  r_12">As</text>.
+00004600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004610: 3c2f 7379 6d62 6f6c 3e0a 2020 2020 2020  </symbol>.      
+00004620: 2020 2020 2020 2020 2020 3c73 796d 626f            <symbo
+00004630: 6c20 6964 3d22 5465 6e74 685f 486f 7573  l id="Tenth_Hous
+00004640: 6522 3e0a 2020 2020 2020 2020 2020 2020  e">.            
+00004650: 2020 2020 2020 2020 3c74 6578 7420 793d          <text y=
+00004660: 2232 3022 2073 7479 6c65 3d22 666f 6e74  "20" style="font
+00004670: 2d73 697a 653a 2032 3070 783b 2066 696c  -size: 20px; fil
+00004680: 6c3a 2024 706c 616e 6574 735f 636f 6c6f  l: $planets_colo
+00004690: 725f 3133 223e 4d63 3c2f 7465 7874 3e0a  r_13">Mc</text>.
+000046a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046b0: 3c2f 7379 6d62 6f6c 3e0a 2020 2020 2020  </symbol>.      
+000046c0: 2020 2020 2020 2020 2020 3c73 796d 626f            <symbo
+000046d0: 6c20 6964 3d22 5365 7665 6e74 685f 486f  l id="Seventh_Ho
+000046e0: 7573 6522 3e0a 2020 2020 2020 2020 2020  use">.          
+000046f0: 2020 2020 2020 2020 2020 3c74 6578 7420            <text 
+00004700: 793d 2232 3022 2073 7479 6c65 3d22 666f  y="20" style="fo
+00004710: 6e74 2d73 697a 653a 2032 3270 783b 2066  nt-size: 22px; f
+00004720: 696c 6c3a 2024 706c 616e 6574 735f 636f  ill: $planets_co
+00004730: 6c6f 725f 3134 223e 4473 3c2f 7465 7874  lor_14">Ds</text
+00004740: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00004750: 2020 3c2f 7379 6d62 6f6c 3e0a 2020 2020    </symbol>.    
+00004760: 2020 2020 2020 2020 2020 2020 3c73 796d              <sym
+00004770: 626f 6c20 6964 3d22 466f 7572 7468 5f48  bol id="Fourth_H
+00004780: 6f75 7365 223e 0a20 2020 2020 2020 2020  ouse">.         
+00004790: 2020 2020 2020 2020 2020 203c 7465 7874             <text
+000047a0: 2079 3d22 3230 2220 7374 796c 653d 2266   y="20" style="f
+000047b0: 6f6e 742d 7369 7a65 3a20 3232 7078 3b20  ont-size: 22px; 
+000047c0: 6669 6c6c 3a20 2470 6c61 6e65 7473 5f63  fill: $planets_c
+000047d0: 6f6c 6f72 5f31 3522 3e49 633c 2f74 6578  olor_15">Ic</tex
+000047e0: 743e 0a20 2020 2020 2020 2020 2020 2020  t>.             
+000047f0: 2020 203c 2f73 796d 626f 6c3e 0a20 2020     </symbol>.   
+00004800: 2020 2020 2020 2020 2020 2020 203c 212d               <!-
+00004810: 2d20 5a6f 6469 6163 202d 2d3e 0a20 2020  - Zodiac -->.   
+00004820: 2020 2020 2020 2020 2020 2020 203c 7379               <sy
+00004830: 6d62 6f6c 2069 643d 2261 7269 6573 223e  mbol id="aries">
+00004840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004850: 2020 2020 203c 7061 7468 0a20 2020 2020       <path.     
+00004860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004870: 2020 2064 3d22 4d20 3134 2e38 3333 3533     d="M 14.83353
+00004880: 362c 3331 2043 2031 342e 3833 3231 3836  6,31 C 14.832186
+00004890: 2c32 392e 3732 3832 3520 3134 2e38 3435  ,29.72825 14.845
+000048a0: 3933 362c 3238 2e34 3535 3834 2031 342e  936,28.45584 14.
+000048b0: 3738 3033 3436 2c32 372e 3138 3532 3320  780346,27.18523 
+000048c0: 4320 3134 2e36 3430 3932 362c 3234 2e32  C 14.640926,24.2
+000048d0: 3330 3436 2031 342e 3237 3139 3237 2c32  3046 14.271927,2
+000048e0: 312e 3238 3937 3920 3133 2e37 3631 3635  1.28979 13.76165
+000048f0: 372c 3138 2e33 3737 3620 4320 3133 2e33  7,18.3776 C 13.3
+00004900: 3231 3938 372c 3135 2e39 3139 3131 2031  21987,15.91911 1
+00004910: 322e 3738 3737 3837 2c31 332e 3436 3938  2.787787,13.4698
+00004920: 3320 3131 2e39 3930 3531 372c 3131 2e31  3 11.990517,11.1
+00004930: 3030 3735 2043 2031 312e 3533 3032 3637  0075 C 11.530267
+00004940: 2c39 2e37 3632 3433 2031 302e 3939 3238  ,9.76243 10.9928
+00004950: 3837 2c38 2e34 3439 3132 2031 302e 3335  87,8.44912 10.35
+00004960: 3730 3837 2c37 2e31 3834 3920 4320 392e  7087,7.1849 C 9.
+00004970: 3737 3634 3036 352c 362e 3035 3420 392e  7764065,6.054 9.
+00004980: 3131 3433 3436 352c 342e 3934 3239 3620  1143465,4.94296 
+00004990: 382e 3231 3630 3036 352c 342e 3033 3439  8.2160065,4.0349
+000049a0: 3420 4320 372e 3632 3832 3436 352c 332e  4 C 7.6282465,3.
+000049b0: 3434 3635 2036 2e39 3030 3732 3635 2c32  4465 6.9007265,2
+000049c0: 2e39 3435 3335 2036 2e30 3634 3937 3635  .94535 6.0649765
+000049d0: 2c32 2e38 3136 3234 2043 2035 2e33 3233  ,2.81624 C 5.323
+000049e0: 3732 3636 2c32 2e37 3031 3432 2034 2e35  7266,2.70142 4.5
+000049f0: 3330 3436 3636 2c32 2e38 3735 3731 2033  304666,2.87571 3
+00004a00: 2e39 3335 3639 3636 2c33 2e33 3433 3834  .9356966,3.34384
+00004a10: 2043 2033 2e32 3133 3635 3635 2c33 2e39   C 3.2136565,3.9
+00004a20: 3035 3139 2032 2e37 3635 3433 3635 2c34  0519 2.7654365,4
+00004a30: 2e37 3536 3235 2032 2e35 3433 3833 3635  .75625 2.5438365
+00004a40: 2c35 2e36 3332 3839 2043 2032 2e33 3035  ,5.63289 C 2.305
+00004a50: 3337 3635 2c36 2e35 3939 3935 2032 2e32  3765,6.59995 2.2
+00004a60: 3935 3937 3635 2c37 2e36 3133 3538 2032  959765,7.61358 2
+00004a70: 2e34 3239 3231 3635 2c38 2e35 3937 3320  .4292165,8.5973 
+00004a80: 4320 322e 3634 3634 3436 352c 3130 2e31  C 2.6464465,10.1
+00004a90: 3535 3837 2033 2e32 3638 3936 3635 2c31  5587 3.2689665,1
+00004aa0: 312e 3633 3235 3820 342e 3038 3135 3436  1.63258 4.081546
+00004ab0: 362c 3132 2e39 3639 3038 2043 2033 2e32  6,12.96908 C 3.2
+00004ac0: 3932 3434 3635 2c31 322e 3936 3930 3820  924465,12.96908 
+00004ad0: 322e 3530 3333 3436 352c 3132 2e39 3639  2.5033465,12.969
+00004ae0: 3038 2031 2e37 3134 3234 3635 2c31 322e  08 1.7142465,12.
+00004af0: 3936 3930 3820 4320 302e 3839 3732 3436  96908 C 0.897246
+00004b00: 3531 2c31 312e 3438 3438 3120 302e 3235  51,11.48481 0.25
+00004b10: 3739 3936 3531 2c39 2e38 3732 3939 2030  799651,9.87299 0
+00004b20: 2e30 3630 3235 3635 3134 2c38 2e31 3738  .060256514,8.178
+00004b30: 3939 2043 202d 302e 3037 3132 3033 3438  99 C -0.07120348
+00004b40: 362c 372e 3030 3639 3520 302e 3030 3337  6,7.00695 0.0037
+00004b50: 3136 3531 3338 2c35 2e37 3939 3033 2030  165138,5.79903 0
+00004b60: 2e33 3731 3439 3635 312c 342e 3637 3432  .37149651,4.6742
+00004b70: 3120 4320 302e 3736 3434 3236 3531 2c33  1 C 0.76442651,3
+00004b80: 2e34 3734 3939 2031 2e35 3139 3538 3635  .47499 1.5195865
+00004b90: 2c32 2e33 3933 3220 322e 3532 3332 3536  ,2.3932 2.523256
+00004ba0: 352c 312e 3633 3034 2043 2033 2e32 3830  5,1.6304 C 3.280
+00004bb0: 3936 3635 2c31 2e30 3534 3738 2034 2e32  9665,1.05478 4.2
+00004bc0: 3035 3933 3636 2c30 2e37 3132 3638 2035  059366,0.71268 5
+00004bd0: 2e31 3531 3934 3636 2c30 2e36 3337 3831  .1519466,0.63781
+00004be0: 2043 2036 2e31 3933 3832 3635 2c30 2e35   C 6.1938265,0.5
+00004bf0: 3434 3936 2037 2e32 3631 3034 3635 2c30  4496 7.2610465,0
+00004c00: 2e37 3436 3139 2038 2e31 3930 3932 3635  .74619 8.1909265
+00004c10: 2c31 2e32 3239 3736 2043 2039 2e33 3939  ,1.22976 C 9.399
+00004c20: 3836 3635 2c31 2e38 3530 3231 2031 302e  8665,1.85021 10.
+00004c30: 3336 3336 3737 2c32 2e38 3539 3434 2031  363677,2.85944 1
+00004c40: 312e 3134 3532 3737 2c33 2e39 3537 3636  1.145277,3.95766
+00004c50: 2043 2031 322e 3139 3033 3437 2c35 2e34   C 12.190347,5.4
+00004c60: 3431 3437 2031 322e 3936 3530 3637 2c37  4147 12.965067,7
+00004c70: 2e31 3031 3031 2031 332e 3538 3432 3837  .10101 13.584287
+00004c80: 2c38 2e38 3033 3832 2043 2031 342e 3633  ,8.80382 C 14.63
+00004c90: 3037 3636 2c31 312e 3731 3736 2031 352e  0766,11.7176 15.
+00004ca0: 3231 3236 3236 2c31 342e 3737 3836 3120  212626,14.77861 
+00004cb0: 3135 2e35 3735 3134 362c 3137 2e38 3437  15.575146,17.847
+00004cc0: 3935 2043 2031 352e 3636 3438 3336 2c31  95 C 15.664836,1
+00004cd0: 382e 3631 3634 3820 3135 2e37 3339 3535  8.61648 15.73955
+00004ce0: 362c 3139 2e33 3836 3735 2031 352e 3830  6,19.38675 15.80
+00004cf0: 3134 3436 2c32 302e 3135 3830 3320 4320  1446,20.15803 C 
+00004d00: 3135 2e39 3333 3630 362c 3230 2e31 3538  15.933606,20.158
+00004d10: 3033 2031 362e 3036 3537 3736 2c32 302e  03 16.065776,20.
+00004d20: 3135 3830 3320 3136 2e31 3937 3933 362c  15803 16.197936,
+00004d30: 3230 2e31 3538 3033 2043 2031 362e 3433  20.15803 C 16.43
+00004d40: 3135 3136 2c31 362e 3738 3333 3220 3136  1516,16.78332 16
+00004d50: 2e39 3139 3036 362c 3133 2e34 3037 3631  .919066,13.40761
+00004d60: 2031 372e 3932 3032 3336 2c31 302e 3137   17.920236,10.17
+00004d70: 3032 3920 4320 3138 2e35 3336 3734 362c  029 C 18.536746,
+00004d80: 382e 3139 3838 3620 3139 2e33 3433 3231  8.19886 19.34321
+00004d90: 362c 362e 3237 3333 2032 302e 3436 3031  6,6.2733 20.4601
+00004da0: 3036 2c34 2e35 3332 3039 2043 2032 312e  06,4.53209 C 21.
+00004db0: 3233 3239 3636 2c33 2e33 3432 3436 2032  232966,3.34246 2
+00004dc0: 322e 3137 3833 3936 2c32 2e32 3236 3931  2.178396,2.22691
+00004dd0: 2032 332e 3339 3332 3336 2c31 2e34 3734   23.393236,1.474
+00004de0: 3733 2043 2032 342e 3330 3339 3436 2c30  73 C 24.303946,0
+00004df0: 2e39 3036 2032 352e 3337 3534 3036 2c30  .906 25.375406,0
+00004e00: 2e35 3933 3135 2032 362e 3434 3938 3336  .59315 26.449836
+00004e10: 2c30 2e36 3137 3434 2043 2032 372e 3430  ,0.61744 C 27.40
+00004e20: 3630 3736 2c30 2e36 3236 3520 3238 2e33  6076,0.6265 28.3
+00004e30: 3636 3333 362c 302e 3838 3431 3420 3239  66336,0.88414 29
+00004e40: 2e31 3733 3338 362c 312e 3430 3537 3120  .173386,1.40571 
+00004e50: 4320 3239 2e39 3138 3237 362c 312e 3838  C 29.918276,1.88
+00004e60: 3431 3720 3330 2e35 3336 3732 362c 322e  417 30.536726,2.
+00004e70: 3534 3832 3520 3331 2e30 3037 3330 362c  54825 31.007306,
+00004e80: 332e 3239 3638 3820 4320 3331 2e36 3430  3.29688 C 31.640
+00004e90: 3337 362c 342e 3330 3938 3120 3331 2e39  376,4.30981 31.9
+00004ea0: 3432 3738 362c 352e 3530 3336 2033 312e  42786,5.5036 31.
+00004eb0: 3939 3035 3236 2c36 2e36 3931 3439 2043  990526,6.69149 C
+00004ec0: 2033 322e 3036 3433 3636 2c38 2e32 3438   32.064366,8.248
+00004ed0: 3938 2033 312e 3730 3033 3036 2c39 2e37  98 31.700306,9.7
+00004ee0: 3938 3431 2033 312e 3131 3831 3336 2c31  9841 31.118136,1
+00004ef0: 312e 3233 3430 3920 4320 3330 2e38 3738  1.23409 C 30.878
+00004f00: 3035 362c 3131 2e38 3237 3734 2033 302e  056,11.82774 30.
+00004f10: 3630 3037 3436 2c31 322e 3430 3538 3420  600746,12.40584 
+00004f20: 3330 2e32 3936 3739 362c 3132 2e39 3639  30.296796,12.969
+00004f30: 3038 2043 2032 392e 3530 3338 3036 2c31  08 C 29.503806,1
+00004f40: 322e 3936 3930 3820 3238 2e37 3130 3832  2.96908 28.71082
+00004f50: 362c 3132 2e39 3639 3038 2032 372e 3931  6,12.96908 27.91
+00004f60: 3738 3336 2c31 322e 3936 3930 3820 4320  7836,12.96908 C 
+00004f70: 3238 2e36 3935 3634 362c 3131 2e35 3638  28.695646,11.568
+00004f80: 3235 2032 392e 3333 3039 3036 2c31 302e  25 29.330906,10.
+00004f90: 3036 3034 3420 3239 2e35 3635 3735 362c  06044 29.565756,
+00004fa0: 382e 3436 3438 3520 4320 3239 2e37 3035  8.46485 C 29.705
+00004fb0: 3433 362c 372e 3439 3035 3320 3239 2e36  436,7.49053 29.6
+00004fc0: 3839 3937 362c 362e 3438 3733 3920 3239  89976,6.48739 29
+00004fd0: 2e34 3639 3733 362c 352e 3532 3631 3620  .469736,5.52616 
+00004fe0: 4320 3239 2e32 3636 3538 362c 342e 3637  C 29.266586,4.67
+00004ff0: 3239 3620 3238 2e38 3730 3935 362c 332e  296 28.870956,3.
+00005000: 3833 3335 3420 3238 2e32 3031 3237 362c  83354 28.201276,
+00005010: 332e 3235 3037 3920 4320 3237 2e37 3138  3.25079 C 27.718
+00005020: 3338 362c 322e 3832 3236 3320 3237 2e30  386,2.82263 27.0
+00005030: 3738 3436 362c 322e 3539 3032 3120 3236  78466,2.59021 26
+00005040: 2e34 3336 3231 362c 322e 3538 3434 3620  .436216,2.58446 
+00005050: 4320 3235 2e36 3830 3330 362c 322e 3536  C 25.680306,2.56
+00005060: 3035 3920 3234 2e39 3530 3038 362c 322e  059 24.950086,2.
+00005070: 3837 3330 3320 3234 2e33 3538 3333 362c  87303 24.358336,
+00005080: 332e 3332 3837 3920 4320 3233 2e34 3934  3.32879 C 23.494
+00005090: 3535 362c 332e 3939 3330 3720 3232 2e38  556,3.99307 22.8
+000050a0: 3434 3938 362c 342e 3839 3139 3820 3232  44986,4.89198 22
+000050b0: 2e32 3832 3935 362c 352e 3831 3637 3920  .282956,5.81679 
+000050c0: 4320 3231 2e34 3531 3735 362c 372e 3231  C 21.451756,7.21
+000050d0: 3037 3220 3230 2e38 3131 3433 362c 382e  072 20.811436,8.
+000050e0: 3731 3031 3820 3230 2e32 3530 3339 362c  71018 20.250396,
+000050f0: 3130 2e32 3331 3234 2043 2031 392e 3433  10.23124 C 19.43
+00005100: 3735 3836 2c31 322e 3439 3830 3220 3138  7586,12.49802 18
+00005110: 2e38 3933 3332 362c 3134 2e38 3531 3636  .893326,14.85166
+00005120: 2031 382e 3434 3032 3836 2c31 372e 3231   18.440286,17.21
+00005130: 3433 3220 4320 3137 2e38 3339 3031 362c  432 C 17.839016,
+00005140: 3230 2e34 3033 3235 2031 372e 3431 3332  20.40325 17.4132
+00005150: 3136 2c32 332e 3632 3931 2031 372e 3234  16,23.6291 17.24
+00005160: 3631 3336 2c32 362e 3837 3135 2043 2031  6136,26.8715 C 1
+00005170: 372e 3138 3337 3936 2c32 382e 3031 3835  7.183796,28.0185
+00005180: 3720 3137 2e31 3733 3936 362c 3239 2e31  7 17.173966,29.1
+00005190: 3637 3435 2031 372e 3137 3735 3136 2c33  6745 17.177516,3
+000051a0: 302e 3331 3539 3520 4320 3137 2e31 3737  0.31595 C 17.177
+000051b0: 3531 362c 3330 2e35 3433 3937 2031 372e  516,30.54397 17.
+000051c0: 3137 3735 3136 2c33 302e 3737 3139 3820  177516,30.77198 
+000051d0: 3137 2e31 3737 3531 362c 3331 2043 2031  17.177516,31 C 1
+000051e0: 362e 3339 3631 3836 2c33 3120 3135 2e36  6.396186,31 15.6
+000051f0: 3134 3835 362c 3331 2031 342e 3833 3335  14856,31 14.8335
+00005200: 3336 2c33 3120 7a22 0a20 2020 2020 2020  36,31 z".       
+00005210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005220: 2073 7479 6c65 3d22 6669 6c6c 3a20 247a   style="fill: $z
+00005230: 6f64 6961 635f 636f 6c6f 725f 3022 0a20  odiac_color_0". 
+00005240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005250: 2020 202f 3e0a 2020 2020 2020 2020 2020     />.          
+00005260: 2020 2020 2020 3c2f 7379 6d62 6f6c 3e0a        </symbol>.
+00005270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005280: 3c73 796d 626f 6c20 6964 3d22 7461 7572  <symbol id="taur
+00005290: 7573 223e 0a20 2020 2020 2020 2020 2020  us">.           
+000052a0: 2020 2020 2020 2020 203c 7061 7468 0a20           <path. 
+000052b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052c0: 2020 2020 2020 2064 3d22 4d20 3131 2e32         d="M 11.2
+000052d0: 3131 3132 352c 3131 2e39 3630 3034 3320  11125,11.960043 
+000052e0: 4320 392e 3938 3536 3139 372c 3131 2e34  C 9.9856197,11.4
+000052f0: 3832 3038 3520 382e 3832 3733 3530 372c  82085 8.8273507,
+00005300: 3130 2e37 3537 3236 3320 372e 3939 3934  10.757263 7.9994
+00005310: 3136 342c 392e 3732 3236 3620 4320 362e  164,9.72266 C 6.
+00005320: 3935 3430 3538 342c 382e 3434 3839 3530  9540584,8.448950
+00005330: 3820 362e 3231 3139 3532 342c 362e 3936  8 6.2119524,6.96
+00005340: 3936 3039 3720 352e 3430 3638 3139 392c  96097 5.4068199,
+00005350: 352e 3534 3232 3531 3520 4320 342e 3931  5.5422515 C 4.91
+00005360: 3533 3333 362c 342e 3634 3335 3933 3120  53336,4.6435931 
+00005370: 342e 3335 3838 3435 322c 332e 3736 3034  4.3588452,3.7604
+00005380: 3132 3820 332e 3630 3032 3638 362c 332e  128 3.6002686,3.
+00005390: 3036 3031 3033 3620 4320 332e 3038 3737  0601036 C 3.0877
+000053a0: 3337 312c 322e 3538 3330 3339 3920 322e  371,2.5830399 2.
+000053b0: 3436 3939 3433 332c 322e 3139 3737 3132  4699433,2.197712
+000053c0: 3920 312e 3737 3931 3332 312c 322e 3034  9 1.7791321,2.04
+000053d0: 3632 3137 3820 4320 312e 3435 3134 3836  62178 C 1.451486
+000053e0: 372c 312e 3936 3633 3435 3120 312e 3131  7,1.9663451 1.11
+000053f0: 3237 3639 382c 312e 3936 3334 3036 3520  27698,1.9634065 
+00005400: 302e 3737 3735 3636 3438 2c31 2e39 3639  0.77756648,1.969
+00005410: 3332 3033 2043 2030 2e36 3737 3530 3133  3203 C 0.6775013
+00005420: 382c 312e 3938 3234 3830 3320 302e 3539  8,1.9824803 0.59
+00005430: 3833 3335 3038 2c31 2e39 3734 3735 3935  833508,1.9747595
+00005440: 2030 2e36 3333 3639 3038 382c 312e 3835   0.63369088,1.85
+00005450: 3238 3333 3320 4320 302e 3633 3336 3930  28333 C 0.633690
+00005460: 3838 2c31 2e32 3730 3336 3138 2030 2e36  88,1.2703618 0.6
+00005470: 3333 3639 3038 382c 302e 3638 3738 3930  3369088,0.687890
+00005480: 3233 2030 2e36 3333 3639 3038 382c 302e  23 0.63369088,0.
+00005490: 3130 3534 3030 3434 2043 2031 2e31 3736  10540044 C 1.176
+000054a0: 3933 2c30 2e31 3131 3738 3838 3420 312e  93,0.11178884 1.
+000054b0: 3732 3130 3239 322c 302e 3039 3031 3539  7210292,0.090159
+000054c0: 3634 3120 322e 3236 3336 3039 352c 302e  641 2.2636095,0.
+000054d0: 3132 3136 3939 3834 2043 2033 2e33 3439  12169984 C 3.349
+000054e0: 3337 3339 2c30 2e32 3132 3038 3539 3420  3739,0.21208594 
+000054f0: 342e 3336 3635 3132 392c 302e 3731 3538  4.3665129,0.7158
+00005500: 3731 3231 2035 2e31 3931 3739 3335 2c31  7121 5.1917935,1
+00005510: 2e34 3039 3735 3535 2043 2036 2e32 3634  .4097555 C 6.264
+00005520: 3738 3434 2c32 2e33 3031 3333 3220 372e  7844,2.301332 7.
+00005530: 3038 3838 3735 342c 332e 3434 3934 3832  0888754,3.449482
+00005540: 3720 372e 3739 3131 3631 342c 342e 3634  7 7.7911614,4.64
+00005550: 3336 3437 3920 4320 382e 3239 3133 3033  36479 C 8.291303
+00005560: 342c 352e 3530 3436 3838 2038 2e37 3732  4,5.504688 8.772
+00005570: 3137 3537 2c36 2e33 3736 3735 3235 2039  1757,6.3767525 9
+00005580: 2e32 3734 3331 3237 2c37 2e32 3336 3630  .2743127,7.23660
+00005590: 3632 2043 2039 2e37 3538 3830 3837 2c38  62 C 9.7588087,8
+000055a0: 2e30 3436 3335 3639 2031 302e 3330 3736  .0463569 10.3076
+000055b0: 3438 2c38 2e38 3234 3738 3635 2031 302e  48,8.8247865 10.
+000055c0: 3937 3135 3339 2c39 2e34 3938 3939 3438  971539,9.4989948
+000055d0: 2043 2031 312e 3535 3837 3137 2c31 302e   C 11.558717,10.
+000055e0: 3039 3436 3939 2031 322e 3236 3135 372c  094699 12.26157,
+000055f0: 3130 2e35 3836 3936 3720 3133 2e30 3532  10.586967 13.052
+00005600: 3934 2c31 302e 3837 3131 3339 2043 2031  94,10.871139 C 1
+00005610: 342e 3135 3039 3636 2c31 312e 3237 3633  4.150966,11.2763
+00005620: 3632 2031 352e 3333 3930 3436 2c31 312e  62 15.339046,11.
+00005630: 3335 3935 3536 2031 362e 3530 3032 3434  359556 16.500244
+00005640: 2c31 312e 3331 3436 3337 2043 2031 372e  ,11.314637 C 17.
+00005650: 3534 3332 3034 2c31 312e 3236 3236 3732  543204,11.262672
+00005660: 2031 382e 3630 3230 3638 2c31 312e 3036   18.602068,11.06
+00005670: 3936 3136 2031 392e 3532 3937 3932 2c31  9616 19.529792,1
+00005680: 302e 3537 3137 3435 2043 2032 302e 3430  0.571745 C 20.40
+00005690: 3133 3335 2c31 302e 3131 3436 3637 2032  1335,10.114667 2
+000056a0: 312e 3130 3338 3034 2c39 2e33 3937 3039  1.103804,9.39709
+000056b0: 3134 2032 312e 3730 3030 342c 382e 3632  14 21.70004,8.62
+000056c0: 3637 3635 3920 4320 3232 2e33 3835 3038  67659 C 22.38508
+000056d0: 372c 372e 3734 3131 3934 3620 3232 2e39  7,7.7411946 22.9
+000056e0: 3036 3937 2c36 2e37 3437 3733 3331 2032  0697,6.7477331 2
+000056f0: 332e 3437 3237 2c35 2e37 3835 3930 3331  3.4727,5.7859031
+00005700: 2043 2032 332e 3937 3332 3939 2c34 2e39   C 23.973299,4.9
+00005710: 3332 3134 3538 2032 342e 3434 3535 3136  321458 24.445516
+00005720: 2c34 2e30 3538 3630 3238 2032 352e 3033  ,4.0586028 25.03
+00005730: 3232 3931 2c33 2e32 3538 3930 3931 2043  2291,3.2589091 C
+00005740: 2032 352e 3731 3138 3636 2c32 2e33 3234   25.711866,2.324
+00005750: 3738 3633 2032 362e 3531 3636 3332 2c31  7863 26.516632,1
+00005760: 2e34 3535 3832 3437 2032 372e 3530 3737  .4558247 27.5077
+00005770: 3636 2c30 2e38 3435 3939 3237 3720 4320  66,0.84599277 C 
+00005780: 3238 2e32 3636 3437 312c 302e 3338 3332  28.266471,0.3832
+00005790: 3338 3934 2032 392e 3134 3633 3737 2c30  3894 29.146377,0
+000057a0: 2e30 3936 3534 3830 3431 2033 302e 3034  .096548041 30.04
+000057b0: 3038 3332 2c30 2e31 3036 3635 3938 3420  0832,0.10665984 
+000057c0: 4320 3330 2e34 3530 3432 362c 302e 3130  C 30.450426,0.10
+000057d0: 3230 3630 3234 2033 302e 3836 3030 3734  206024 30.860074
+000057e0: 2c30 2e31 3037 3933 3735 3420 3331 2e32  ,0.10793754 31.2
+000057f0: 3639 3636 372c 302e 3130 3534 3030 3434  69667,0.10540044
+00005800: 2043 2033 312e 3236 3936 3637 2c30 2e37   C 31.269667,0.7
+00005810: 3236 3731 3331 3520 3331 2e32 3639 3636  2671315 31.26966
+00005820: 372c 312e 3334 3830 3235 3820 3331 2e32  7,1.3480258 31.2
+00005830: 3639 3636 372c 312e 3936 3933 3230 3320  69667,1.9693203 
+00005840: 4320 3330 2e38 3336 3534 2c31 2e39 3636  C 30.83654,1.966
+00005850: 3130 3738 2033 302e 3339 3533 3631 2c31  1078 30.395361,1
+00005860: 2e39 3538 3336 3838 2032 392e 3937 3630  .9583688 29.9760
+00005870: 3638 2c32 2e30 3834 3035 3520 4320 3239  68,2.084055 C 29
+00005880: 2e31 3139 3933 342c 322e 3331 3836 3731  .119934,2.318671
+00005890: 3820 3238 2e34 3030 3438 332c 322e 3839  8 28.400483,2.89
+000058a0: 3235 3634 3620 3237 2e38 3236 3933 392c  25646 27.826939,
+000058b0: 332e 3535 3137 3639 3320 4320 3237 2e32  3.5517693 C 27.2
+000058c0: 3336 3032 382c 342e 3232 3335 3836 3520  36028,4.2235865 
+000058d0: 3236 2e37 3838 3236 312c 352e 3030 3238  26.788261,5.0028
+000058e0: 3337 3420 3236 2e33 3631 3636 362c 352e  374 26.361666,5.
+000058f0: 3738 3433 3639 3920 4320 3235 2e36 3233  7843699 C 25.623
+00005900: 3131 2c37 2e31 3031 3038 3139 2032 342e  11,7.1010819 24.
+00005910: 3932 3631 3638 2c38 2e34 3534 3339 2032  926168,8.45439 2
+00005920: 332e 3937 3439 3436 2c39 2e36 3335 3732  3.974946,9.63572
+00005930: 3337 2043 2032 332e 3539 3335 3534 2c31  37 C 23.593554,1
+00005940: 302e 3131 3532 3838 2032 332e 3135 3231  0.115288 23.1521
+00005950: 3138 2c31 302e 3534 3738 3136 2032 322e  18,10.547816 22.
+00005960: 3635 3235 3036 2c31 302e 3930 3433 3431  652506,10.904341
+00005970: 2043 2032 322e 3034 3938 312c 3131 2e33   C 22.04981,11.3
+00005980: 3431 3236 3720 3231 2e33 3833 3337 352c  41267 21.383375,
+00005990: 3131 2e36 3835 3332 3620 3230 2e36 3932  11.685326 20.692
+000059a0: 3231 362c 3131 2e39 3630 3034 3320 4320  216,11.960043 C 
+000059b0: 3232 2e33 3438 3938 312c 3132 2e38 3635  22.348981,12.865
+000059c0: 3235 3420 3233 2e38 3238 3330 382c 3134  254 23.828308,14
+000059d0: 2e31 3232 3634 3620 3234 2e38 3936 3333  .122646 24.89633
+000059e0: 392c 3135 2e36 3834 3033 3120 4320 3235  9,15.684031 C 25
+000059f0: 2e37 3936 3530 342c 3136 2e39 3836 3038  .796504,16.98608
+00005a00: 3720 3236 2e33 3934 3331 342c 3138 2e34  7 26.394314,18.4
+00005a10: 3939 3135 3820 3236 2e35 3932 3934 332c  99158 26.592943,
+00005a20: 3230 2e30 3730 3039 2043 2032 362e 3738  20.07009 C 26.78
+00005a30: 3636 3332 2c32 312e 3535 3231 3531 2032  6632,21.552151 2
+00005a40: 362e 3637 3934 3438 2c32 332e 3037 3737  6.679448,23.0777
+00005a50: 3820 3236 2e32 3436 3339 342c 3234 2e35  8 26.246394,24.5
+00005a60: 3130 3139 3420 4320 3235 2e37 3934 3132  10194 C 25.79412
+00005a70: 352c 3235 2e39 3931 3033 3220 3234 2e39  5,25.991032 24.9
+00005a80: 3736 3338 342c 3237 2e33 3439 3530 3520  76384,27.349505 
+00005a90: 3233 2e39 3235 3937 352c 3238 2e34 3835  23.925975,28.485
+00005aa0: 3030 3720 4320 3232 2e36 3635 3634 362c  007 C 22.665646,
+00005ab0: 3239 2e38 3636 3135 2032 312e 3038 3539  29.86615 21.0859
+00005ac0: 3938 2c33 302e 3938 3437 3332 2031 392e  98,30.984732 19.
+00005ad0: 3330 3132 3432 2c33 312e 3537 3639 3332  301242,31.576932
+00005ae0: 2043 2031 372e 3535 3232 3038 2c33 322e   C 17.552208,32.
+00005af0: 3135 3734 3134 2031 352e 3635 3238 3032  157414 15.652802
+00005b00: 2c33 322e 3234 3636 3134 2031 332e 3834  ,32.246614 13.84
+00005b10: 3630 3836 2c33 312e 3930 3237 3536 2043  6086,31.902756 C
+00005b20: 2031 322e 3232 3031 3933 2c33 312e 3538   12.220193,31.58
+00005b30: 3434 3839 2031 302e 3638 3537 3635 2c33  4489 10.685765,3
+00005b40: 302e 3834 3538 3520 392e 3430 3038 3736  0.84585 9.400876
+00005b50: 372c 3239 2e38 3035 3632 3520 4320 382e  7,29.805625 C 8.
+00005b60: 3330 3031 3432 342c 3238 2e39 3233 3330  3001424,28.92330
+00005b70: 3320 372e 3333 3534 3639 342c 3237 2e38  3 7.3354694,27.8
+00005b80: 3631 3831 3520 362e 3630 3637 3737 342c  61815 6.6067774,
+00005b90: 3236 2e36 3532 3935 3620 4320 352e 3834  26.652956 C 5.84
+00005ba0: 3135 3032 372c 3235 2e33 3735 3233 3120  15027,25.375231 
+00005bb0: 352e 3337 3036 3538 392c 3233 2e39 3233  5.3706589,23.923
+00005bc0: 3431 3520 352e 3234 3738 3436 382c 3232  415 5.2478468,22
+00005bd0: 2e34 3339 3731 3220 4320 352e 3038 3233  .439712 C 5.0823
+00005be0: 3538 382c 3230 2e35 3936 3620 352e 3339  588,20.5966 5.39
+00005bf0: 3339 3931 352c 3138 2e37 3031 3435 2036  39915,18.70145 6
+00005c00: 2e32 3136 3237 3034 2c31 372e 3033 3732  .2162704,17.0372
+00005c10: 3132 2043 2037 2e31 3136 3633 3634 2c31  12 C 7.1166364,1
+00005c20: 352e 3139 3133 3632 2038 2e35 3634 3332  5.191362 8.56432
+00005c30: 3234 2c31 332e 3633 3439 3935 2031 302e  24,13.634995 10.
+00005c40: 3238 3335 3436 2c31 322e 3531 3735 3633  283546,12.517563
+00005c50: 2043 2031 302e 3538 3532 3937 2c31 322e   C 10.585297,12.
+00005c60: 3331 3937 3434 2031 302e 3839 3530 3038  319744 10.895008
+00005c70: 2c31 322e 3133 3430 3632 2031 312e 3231  ,12.134062 11.21
+00005c80: 3131 3235 2c31 312e 3936 3030 3433 207a  1125,11.960043 z
+00005c90: 204d 2031 352e 3935 3739 322c 3239 2e36   M 15.95792,29.6
+00005ca0: 3035 3330 3520 4320 3137 2e34 3639 3637  05305 C 17.46967
+00005cb0: 342c 3239 2e36 3133 3933 3820 3138 2e39  4,29.613938 18.9
+00005cc0: 3935 3730 332c 3239 2e32 3238 3036 3420  95703,29.228064 
+00005cd0: 3230 2e32 3737 3937 342c 3238 2e34 3138  20.277974,28.418
+00005ce0: 3133 2043 2032 312e 3238 3234 3331 2c32  13 C 21.282431,2
+00005cf0: 372e 3738 3934 3632 2032 322e 3135 3336  7.789462 22.1536
+00005d00: 3237 2c32 362e 3935 3235 3333 2032 322e  27,26.952533 22.
+00005d10: 3833 3739 3432 2c32 352e 3938 3737 3635  837942,25.987765
+00005d20: 2043 2032 332e 3539 3634 3038 2c32 342e   C 23.596408,24.
+00005d30: 3930 3135 3236 2032 342e 3035 3635 3833  901526 24.056583
+00005d40: 2c32 332e 3631 3237 3935 2032 342e 3136  ,23.612795 24.16
+00005d50: 3031 3434 2c32 322e 3239 3332 3138 2043  0144,22.293218 C
+00005d60: 2032 342e 3239 3937 3535 2c32 302e 3639   24.299755,20.69
+00005d70: 3333 3031 2032 342e 3030 3932 3232 2c31  3301 24.009222,1
+00005d80: 392e 3033 3638 3032 2032 332e 3231 3332  9.036802 23.2132
+00005d90: 3034 2c31 372e 3633 3037 3831 2043 2032  04,17.630781 C 2
+00005da0: 322e 3633 3532 3836 2c31 362e 3539 3739  2.635286,16.5979
+00005db0: 3320 3231 2e38 3233 3731 322c 3135 2e37  3 21.823712,15.7
+00005dc0: 3031 3935 3520 3230 2e38 3832 3335 342c  01955 20.882354,
+00005dd0: 3134 2e39 3836 3232 3320 4320 3139 2e39  14.986223 C 19.9
+00005de0: 3537 3836 392c 3134 2e32 3835 3731 3320  57869,14.285713 
+00005df0: 3138 2e38 3734 3333 372c 3133 2e37 3936  18.874337,13.796
+00005e00: 3536 3620 3137 2e37 3334 3830 372c 3133  566 17.734807,13
+00005e10: 2e35 3732 3931 3920 4320 3136 2e35 3630  .572919 C 16.560
+00005e20: 3537 392c 3133 2e33 3339 3330 3620 3135  579,13.339306 15
+00005e30: 2e33 3339 3535 392c 3133 2e33 3435 3534  .339559,13.34554
+00005e40: 3820 3134 2e31 3635 3434 312c 3133 2e35  8 14.165441,13.5
+00005e50: 3736 3037 3720 4320 3132 2e38 3832 3031  76077 C 12.88201
+00005e60: 372c 3133 2e38 3336 3438 3420 3131 2e36  7,13.836484 11.6
+00005e70: 3730 3834 322c 3134 2e34 3238 3030 3920  70842,14.428009 
+00005e80: 3130 2e36 3731 3233 342c 3135 2e32 3731  10.671234,15.271
+00005e90: 3138 2043 2039 2e34 3337 3437 3637 2c31  18 C 9.4374767,1
+00005ea0: 362e 3239 3439 3034 2038 2e34 3639 3038  6.294904 8.46908
+00005eb0: 3834 2c31 372e 3636 3339 3634 2038 2e30  84,17.663964 8.0
+00005ec0: 3239 3335 3534 2c31 392e 3231 3137 3838  293554,19.211788
+00005ed0: 2043 2037 2e36 3533 3135 3934 2c32 302e   C 7.6531594,20.
+00005ee0: 3532 3336 3633 2037 2e36 3133 3333 3834  523663 7.6133384
+00005ef0: 2c32 312e 3932 3637 3832 2037 2e38 3834  ,21.926782 7.884
+00005f00: 3233 3534 2c32 332e 3236 3235 3439 2043  2354,23.262549 C
+00005f10: 2038 2e31 3530 3934 3134 2c32 342e 3533   8.1509414,24.53
+00005f20: 3232 3631 2038 2e37 3631 3238 3737 2c32  2261 8.7612877,2
+00005f30: 352e 3732 3337 3235 2039 2e36 3230 3834  5.723725 9.62084
+00005f40: 3337 2c32 362e 3639 3538 3836 2043 2031  37,26.695886 C 1
+00005f50: 302e 3530 3232 3838 2c32 372e 3730 3630  0.502288,27.7060
+00005f60: 3132 2031 312e 3539 3734 3034 2c32 382e  12 11.597404,28.
+00005f70: 3535 3033 3838 2031 322e 3835 3430 3733  550388 12.854073
+00005f80: 2c32 392e 3033 3938 3038 2043 2031 332e  ,29.039808 C 13.
+00005f90: 3833 3830 372c 3239 2e34 3333 3138 3520  83807,29.433185 
+00005fa0: 3134 2e39 3030 3333 372c 3239 2e36 3036  14.900337,29.606
+00005fb0: 3630 3120 3135 2e39 3537 3932 2c32 392e  601 15.95792,29.
+00005fc0: 3630 3533 3035 207a 220a 2020 2020 2020  605305 z".      
+00005fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fe0: 2020 7374 796c 653d 2266 696c 6c3a 2024    style="fill: $
+00005ff0: 7a6f 6469 6163 5f63 6f6c 6f72 5f31 220a  zodiac_color_1".
+00006000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006010: 2020 2020 2f3e 0a20 2020 2020 2020 2020      />.         
+00006020: 2020 2020 2020 203c 2f73 796d 626f 6c3e         </symbol>
+00006030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006040: 203c 7379 6d62 6f6c 2069 643d 2267 656d   <symbol id="gem
+00006050: 696e 6922 3e0a 2020 2020 2020 2020 2020  ini">.          
+00006060: 2020 2020 2020 2020 2020 3c70 6174 680a            <path.
+00006070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006080: 2020 2020 2020 2020 643d 224d 2030 2e35          d="M 0.5
+00006090: 3635 3439 3239 322c 3332 2043 2030 2e35  6549292,32 C 0.5
+000060a0: 3635 3439 3239 322c 3331 2e32 3134 3233  6549292,31.21423
+000060b0: 3820 302e 3536 3534 3932 3932 2c33 302e  8 0.56549292,30.
+000060c0: 3432 3834 3635 2030 2e35 3635 3439 3239  428465 0.5654929
+000060d0: 322c 3239 2e36 3432 3730 3320 4320 322e  2,29.642703 C 2.
+000060e0: 3936 3735 3131 392c 3239 2e30 3131 3131  9675119,29.01111
+000060f0: 3620 352e 3430 3233 3537 332c 3238 2e34  6 5.4023573,28.4
+00006100: 3836 3135 3520 372e 3836 3937 3730 342c  86155 7.8697704,
+00006110: 3238 2e31 3838 3739 3220 4320 372e 3836  28.188792 C 7.86
+00006120: 3937 3730 342c 3230 2e30 3438 3831 3720  97704,20.048817 
+00006130: 372e 3836 3937 3730 342c 3131 2e39 3038  7.8697704,11.908
+00006140: 3833 3220 372e 3836 3937 3730 342c 332e  832 7.8697704,3.
+00006150: 3736 3838 3537 3120 4320 352e 3339 3736  7688571 C 5.3976
+00006160: 3134 362c 332e 3533 3839 3537 3120 322e  146,3.5389571 2.
+00006170: 3935 3030 3632 392c 332e 3036 3136 3339  9500629,3.061639
+00006180: 3120 302e 3536 3534 3932 3932 2c32 2e33  1 0.56549292,2.3
+00006190: 3731 3431 3038 2043 2030 2e35 3635 3439  714108 C 0.56549
+000061a0: 3239 322c 312e 3538 3039 3432 3320 302e  292,1.5809423 0.
+000061b0: 3536 3534 3932 3932 2c30 2e37 3930 3437  56549292,0.79047
+000061c0: 3339 2030 2e35 3635 3439 3239 322c 2d35  39 0.56549292,-5
+000061d0: 652d 3036 2043 2034 2e31 3330 3034 3539  e-06 C 4.1300459
+000061e0: 2c30 2e39 3830 3933 3036 2037 2e38 3138  ,0.9809306 7.818
+000061f0: 3430 3738 2c31 2e34 3336 3235 3220 3131  4078,1.436252 11
+00006200: 2e35 3032 3830 332c 312e 3634 3238 3639  .502803,1.642869
+00006210: 3520 4320 3134 2e36 3939 3431 2c31 2e38  5 C 14.69941,1.8
+00006220: 3131 3535 3734 2031 372e 3930 3537 332c  115574 17.90573,
+00006230: 312e 3830 3730 3438 3220 3231 2e31 3031  1.8070482 21.101
+00006240: 3631 312c 312e 3632 3430 3735 3820 4320  611,1.6240758 C 
+00006250: 3234 2e36 3737 3233 342c 312e 3430 3831  24.677234,1.4081
+00006260: 3931 2032 382e 3235 3437 3432 2c30 2e39  91 28.254742,0.9
+00006270: 3532 3536 3839 2033 312e 3731 3434 3236  525689 31.714426
+00006280: 2c2d 3565 2d30 3620 4320 3331 2e37 3134  ,-5e-06 C 31.714
+00006290: 3432 362c 302e 3739 3034 3733 3920 3331  426,0.7904739 31
+000062a0: 2e37 3134 3432 362c 312e 3538 3039 3432  .714426,1.580942
+000062b0: 3320 3331 2e37 3134 3432 362c 322e 3337  3 31.714426,2.37
+000062c0: 3134 3130 3820 4320 3239 2e33 3234 3530  14108 C 29.32450
+000062d0: 322c 332e 3035 3933 3438 3120 3236 2e38  2,3.0593481 26.8
+000062e0: 3732 3832 392c 332e 3533 3836 3637 3120  72829,3.5386671 
+000062f0: 3234 2e33 3936 3034 352c 332e 3736 3838  24.396045,3.7688
+00006300: 3537 3120 4320 3234 2e33 3936 3034 352c  571 C 24.396045,
+00006310: 3131 2e39 3038 3833 3220 3234 2e33 3936  11.908832 24.396
+00006320: 3034 352c 3230 2e30 3438 3831 3720 3234  045,20.048817 24
+00006330: 2e33 3936 3034 352c 3238 2e31 3838 3739  .396045,28.18879
+00006340: 3220 4320 3236 2e38 3638 3033 352c 3238  2 C 26.868035,28
+00006350: 2e34 3836 3730 3420 3239 2e33 3037 3136  .486704 29.30716
+00006360: 372c 3239 2e30 3133 3135 3820 3331 2e37  7,29.013158 31.7
+00006370: 3134 3432 362c 3239 2e36 3432 3730 3320  14426,29.642703 
+00006380: 4320 3331 2e37 3134 3432 362c 3330 2e34  C 31.714426,30.4
+00006390: 3238 3436 3520 3331 2e37 3134 3432 362c  28465 31.714426,
+000063a0: 3331 2e32 3134 3233 3820 3331 2e37 3134  31.214238 31.714
+000063b0: 3432 362c 3332 2043 2032 362e 3037 3137  426,32 C 26.0717
+000063c0: 372c 3330 2e35 3132 3836 3620 3230 2e32  7,30.512866 20.2
+000063d0: 3036 3433 322c 3239 2e39 3933 3932 3820  06432,29.993928 
+000063e0: 3134 2e33 3833 3237 312c 3330 2e31 3239  14.383271,30.129
+000063f0: 3237 3820 4320 392e 3732 3831 3533 362c  278 C 9.7281536,
+00006400: 3330 2e32 3430 3139 3620 352e 3037 3231  30.240196 5.0721
+00006410: 3334 392c 3330 2e38 3038 3737 3720 302e  349,30.808777 0.
+00006420: 3536 3534 3932 3932 2c33 3220 7a20 4d20  56549292,32 z M 
+00006430: 3130 2e37 3034 3035 332c 3238 2e30 3139  10.704053,28.019
+00006440: 3431 2043 2031 322e 3938 3434 3438 2c32  41 C 12.984448,2
+00006450: 372e 3736 3533 3637 2031 352e 3238 3332  7.765367 15.2832
+00006460: 3234 2c32 372e 3732 3237 3833 2031 372e  24,27.722783 17.
+00006470: 3537 3535 3339 2c32 372e 3736 3638 3038  575539,27.766808
+00006480: 2043 2031 382e 3930 3638 3836 2c32 372e   C 18.906886,27.
+00006490: 3739 3639 3132 2032 302e 3233 3831 342c  796912 20.23814,
+000064a0: 3237 2e38 3730 3036 3520 3231 2e35 3631  27.870065 21.561
+000064b0: 3736 322c 3238 2e30 3139 3431 2043 2032  762,28.01941 C 2
+000064c0: 312e 3536 3137 3632 2c32 302e 3030 3137  1.561762,20.0017
+000064d0: 3636 2032 312e 3536 3137 3632 2c31 312e  66 21.561762,11.
+000064e0: 3938 3431 3231 2032 312e 3536 3137 3632  984121 21.561762
+000064f0: 2c33 2e39 3636 3437 3731 2043 2031 392e  ,3.9664771 C 19.
+00006500: 3138 3933 3038 2c34 2e31 3231 3037 3731  189308,4.1210771
+00006510: 2031 362e 3831 3030 3831 2c34 2e31 3339   16.810081,4.139
+00006520: 3331 3131 2031 342e 3433 3335 3135 2c34  3111 14.433515,4
+00006530: 2e31 3039 3336 3331 2043 2031 332e 3138  .1093631 C 13.18
+00006540: 3935 3236 2c34 2e30 3930 3038 3231 2031  9526,4.0900821 1
+00006550: 312e 3934 3535 3035 2c34 2e30 3530 3230  1.945505,4.05020
+00006560: 3431 2031 302e 3730 3430 3533 2c33 2e39  41 10.704053,3.9
+00006570: 3636 3437 3731 2043 2031 302e 3730 3430  664771 C 10.7040
+00006580: 3533 2c31 312e 3938 3431 3231 2031 302e  53,11.984121 10.
+00006590: 3730 3430 3533 2c32 302e 3030 3137 3636  704053,20.001766
+000065a0: 2031 302e 3730 3430 3533 2c32 382e 3031   10.704053,28.01
+000065b0: 3934 3120 7a20 220a 2020 2020 2020 2020  941 z ".        
+000065c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065d0: 7374 796c 653d 2266 696c 6c3a 2024 7a6f  style="fill: $zo
+000065e0: 6469 6163 5f63 6f6c 6f72 5f32 220a 2020  diac_color_2".  
+000065f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006600: 2020 2f3e 0a20 2020 2020 2020 2020 2020    />.           
+00006610: 2020 2020 203c 2f73 796d 626f 6c3e 0a20       </symbol>. 
+00006620: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00006630: 7379 6d62 6f6c 2069 643d 2263 616e 6365  symbol id="cance
+00006640: 7222 3e0a 2020 2020 2020 2020 2020 2020  r">.            
+00006650: 2020 2020 2020 2020 3c70 6174 680a 2020          <path.  
+00006660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006670: 2020 2020 2020 643d 224d 2030 2c32 352e        d="M 0,25.
+00006680: 3632 3934 3832 204c 2030 2c32 322e 3930  629482 L 0,22.90
+00006690: 3831 3031 2043 2035 2e32 3437 3935 3039  8101 C 5.2479509
+000066a0: 2c32 352e 3330 3439 3134 2031 302e 3333  ,25.304914 10.33
+000066b0: 3334 3634 2c32 362e 3439 3038 3337 2031  3464,26.490837 1
+000066c0: 352e 3233 3135 3531 2c32 362e 3439 3038  5.231551,26.4908
+000066d0: 3337 2043 2031 382e 3434 3237 3937 2c32  37 C 18.442797,2
+000066e0: 362e 3439 3038 3337 2032 312e 3035 3432  6.490837 21.0542
+000066f0: 3737 2c32 362e 3037 3838 3834 2032 332e  77,26.078884 23.
+00006700: 3036 3539 3932 2c32 352e 3234 3234 3937  065992,25.242497
+00006710: 2043 2032 312e 3739 3134 3839 2c32 342e   C 21.791489,24.
+00006720: 3539 3333 3620 3230 2e38 3239 3336 352c  59336 20.829365,
+00006730: 3233 2e37 3639 3435 3520 3230 2e31 3932  23.769455 20.192
+00006740: 3131 342c 3232 2e37 3833 3236 3720 4320  114,22.783267 C 
+00006750: 3139 2e35 3534 3836 332c 3231 2e37 3937  19.554863,21.797
+00006760: 3037 3820 3139 2e32 3239 3939 2c32 302e  078 19.22999,20.
+00006770: 3633 3631 3232 2031 392e 3232 3939 392c  636122 19.22999,
+00006780: 3139 2e33 3030 3339 3820 4320 3139 2e32  19.300398 C 19.2
+00006790: 3239 3939 2c31 372e 3535 3237 3232 2031  2999,17.552722 1
+000067a0: 392e 3836 3732 3431 2c31 362e 3035 3437  9.867241,16.0547
+000067b0: 3134 2032 312e 3132 3932 3438 2c31 342e  14 21.129248,14.
+000067c0: 3739 3338 3931 2043 2032 322e 3337 3837  793891 C 22.3787
+000067d0: 362c 3133 2e35 3435 3535 3120 3233 2e39  6,13.545551 23.9
+000067e0: 3033 3136 352c 3132 2e39 3231 3338 3120  03165,12.921381 
+000067f0: 3235 2e36 3532 3438 312c 3132 2e39 3231  25.652481,12.921
+00006800: 3338 3120 4320 3237 2e34 3031 3739 382c  381 C 27.401798,
+00006810: 3132 2e39 3231 3338 3120 3238 2e38 3838  12.921381 28.888
+00006820: 3731 382c 3133 2e35 3435 3535 3120 3330  718,13.545551 30
+00006830: 2e31 3338 3233 2c31 342e 3738 3134 3037  .13823,14.781407
+00006840: 2043 2033 312e 3337 3532 3436 2c31 362e   C 31.375246,16.
+00006850: 3032 3937 3437 2033 322e 3030 3030 3032  029747 32.000002
+00006860: 2c31 372e 3531 3532 3732 2033 322e 3030  ,17.515272 32.00
+00006870: 3030 3032 2c31 392e 3237 3534 3331 2043  0002,19.275431 C
+00006880: 2033 322e 3030 3030 3032 2c32 322e 3035   32.000002,22.05
+00006890: 3932 3320 3330 2e33 3030 3636 362c 3234  923 30.300666,24
+000068a0: 2e33 3831 3134 3220 3236 2e38 3839 3439  .381142 26.88949
+000068b0: 382c 3236 2e32 3238 3638 3520 4320 3233  8,26.228685 C 23
+000068c0: 2e34 3738 3333 312c 3238 2e30 3736 3232  .478331,28.07622
+000068d0: 3820 3139 2e32 3035 2c32 3920 3134 2e30  8 19.205,29 14.0
+000068e0: 3639 3530 352c 3239 2043 2039 2e36 3231  69505,29 C 9.621
+000068f0: 3234 3239 2c32 3920 342e 3933 3535 3732  2429,29 4.935572
+00006900: 392c 3237 2e38 3838 3937 3720 302c 3235  9,27.888977 0,25
+00006910: 2e36 3239 3438 3220 7a20 4d20 3230 2e39  .629482 z M 20.9
+00006920: 3136 3833 312c 3139 2e33 3132 3838 3220  16831,19.312882 
+00006930: 4320 3230 2e39 3136 3833 312c 3230 2e35  C 20.916831,20.5
+00006940: 3836 3138 3820 3231 2e33 3739 3135 2c32  86188 21.37915,2
+00006950: 312e 3638 3437 3238 2032 322e 3331 3632  1.684728 22.3162
+00006960: 3834 2c32 322e 3630 3834 3939 2043 2032  84,22.608499 C 2
+00006970: 332e 3234 3039 3233 2c32 332e 3533 3232  3.240923,23.5322
+00006980: 3731 2032 342e 3336 3534 3834 2c32 332e  71 24.365484,23.
+00006990: 3939 3431 3537 2032 352e 3635 3234 3831  994157 25.652481
+000069a0: 2c32 332e 3939 3431 3537 2043 2032 362e  ,23.994157 C 26.
+000069b0: 3935 3139 3734 2c32 332e 3939 3431 3537  951974,23.994157
+000069c0: 2032 382e 3035 3135 3435 2c32 332e 3533   28.051545,23.53
+000069d0: 3232 3731 2032 382e 3936 3336 3838 2c32  2271 28.963688,2
+000069e0: 322e 3634 3539 3439 2043 2032 392e 3836  2.645949 C 29.86
+000069f0: 3333 3337 2c32 312e 3734 3731 3435 2033  3337,21.747145 3
+00006a00: 302e 3331 3331 3631 2c32 302e 3634 3836  0.313161,20.6486
+00006a10: 3035 2033 302e 3331 3331 3631 2c31 392e  05 30.313161,19.
+00006a20: 3335 3033 3332 2043 2033 302e 3331 3331  350332 C 30.3131
+00006a30: 3631 2c31 382e 3032 3730 3931 2032 392e  61,18.027091 29.
+00006a40: 3836 3333 3337 2c31 362e 3930 3335 3835  863337,16.903585
+00006a50: 2032 382e 3935 3131 3933 2c31 352e 3937   28.951193,15.97
+00006a60: 3938 3134 2043 2032 382e 3033 3930 3439  9814 C 28.039049
+00006a70: 2c31 352e 3035 3630 3432 2032 362e 3933  ,15.056042 26.93
+00006a80: 3934 3739 2c31 342e 3539 3431 3536 2032  9479,14.594156 2
+00006a90: 352e 3633 3939 3836 2c31 342e 3539 3431  5.639986,14.5941
+00006aa0: 3536 2043 2032 342e 3332 3739 3939 2c31  56 C 24.327999,1
+00006ab0: 342e 3539 3431 3536 2032 332e 3231 3539  4.594156 23.2159
+00006ac0: 3333 2c31 352e 3035 3630 3432 2032 322e  33,15.056042 22.
+00006ad0: 3239 3132 3934 2c31 352e 3937 3938 3134  291294,15.979814
+00006ae0: 2043 2032 312e 3337 3931 352c 3136 2e38   C 21.37915,16.8
+00006af0: 3931 3130 3220 3230 2e39 3136 3833 312c  91102 20.916831,
+00006b00: 3138 2e30 3032 3132 3520 3230 2e39 3136  18.002125 20.916
+00006b10: 3833 312c 3139 2e33 3132 3838 3220 7a20  831,19.312882 z 
+00006b20: 4d20 3332 2e30 3030 3030 322c 372e 3331  M 32.000002,7.31
+00006b30: 3633 3334 3120 4c20 3332 2e30 3030 3030  63341 L 32.00000
+00006b40: 322c 3130 2e30 3337 3731 3520 4320 3236  2,10.037715 C 26
+00006b50: 2e37 3339 3535 372c 372e 3634 3039 3032  .739557,7.640902
+00006b60: 3520 3231 2e36 3636 3533 382c 362e 3434  5 21.666538,6.44
+00006b70: 3234 3936 3220 3136 2e37 3535 3935 362c  24962 16.755956,
+00006b80: 362e 3434 3234 3936 3220 4320 3133 2e35  6.4424962 C 13.5
+00006b90: 3537 3230 352c 362e 3434 3234 3936 3220  57205,6.4424962 
+00006ba0: 3130 2e39 3333 3233 2c36 2e38 3534 3434  10.93323,6.85444
+00006bb0: 3833 2038 2e39 3039 3032 3039 2c37 2e37  83 8.9090209,7.7
+00006bc0: 3033 3331 3935 2043 2031 302e 3230 3835  033195 C 10.2085
+00006bd0: 3133 2c38 2e33 3532 3435 3633 2031 312e  13,8.3524563 11.
+00006be0: 3137 3036 3337 2c39 2e31 3736 3336 3037  170637,9.1763607
+00006bf0: 2031 312e 3739 3533 3933 2c31 302e 3136   11.795393,10.16
+00006c00: 3235 3439 2043 2031 322e 3434 3531 342c  2549 C 12.44514,
+00006c10: 3131 2e31 3438 3733 3820 3132 2e37 3537  11.148738 12.757
+00006c20: 3531 382c 3132 2e33 3039 3639 3420 3132  518,12.309694 12
+00006c30: 2e37 3537 3531 382c 3133 2e36 3435 3431  .757518,13.64541
+00006c40: 3820 4320 3132 2e37 3537 3531 382c 3135  8 C 12.757518,15
+00006c50: 2e33 3933 3039 3420 3132 2e31 3332 3736  .393094 12.13276
+00006c60: 322c 3136 2e38 3931 3130 3220 3130 2e38  2,16.891102 10.8
+00006c70: 3730 3735 352c 3138 2e31 3531 3932 3520  70755,18.151925 
+00006c80: 4320 392e 3630 3837 3436 392c 3139 2e34  C 9.6087469,19.4
+00006c90: 3030 3236 3520 382e 3039 3638 3337 392c  00265 8.0968379,
+00006ca0: 3230 2e30 3234 3433 3520 362e 3333 3530  20.024435 6.3350
+00006cb0: 3235 392c 3230 2e30 3234 3433 3520 4320  259,20.024435 C 
+00006cc0: 342e 3538 3537 3038 392c 3230 2e30 3234  4.5857089,20.024
+00006cd0: 3433 3520 332e 3039 3837 3839 392c 3139  435 3.0987899,19
+00006ce0: 2e34 3132 3734 3920 312e 3836 3137 3732  .412749 1.861772
+00006cf0: 392c 3138 2e31 3634 3430 3920 4320 302e  9,18.164409 C 0.
+00006d00: 3632 3437 3536 2c31 362e 3932 3835 3532  624756,16.928552
+00006d10: 2030 2c31 352e 3433 3035 3434 2030 2c31   0,15.430544 0,1
+00006d20: 332e 3638 3238 3638 2043 2030 2c31 302e  3.682868 C 0,10.
+00006d30: 3838 3635 3836 2031 2e36 3939 3333 3634  886586 1.6993364
+00006d40: 2c38 2e35 3532 3139 3037 2035 2e31 3130  ,8.5521907 5.110
+00006d50: 3530 3339 2c36 2e37 3034 3634 3735 2043  5039,6.7046475 C
+00006d60: 2038 2e35 3039 3137 3639 2c34 2e38 3537   8.5091769,4.857
+00006d70: 3130 3434 2031 322e 3739 3530 3033 2c33  1044 12.795003,3
+00006d80: 2e39 3333 3333 3237 2031 372e 3933 3034  .9333327 17.9304
+00006d90: 3937 2c33 2e39 3333 3333 3237 2043 2032  97,3.9333327 C 2
+00006da0: 322e 3337 3837 362c 332e 3933 3333 3332  2.37876,3.933332
+00006db0: 3720 3237 2e30 3634 3433 2c35 2e30 3536  7 27.06443,5.056
+00006dc0: 3833 3838 2033 322e 3030 3030 3032 2c37  8388 32.000002,7
+00006dd0: 2e33 3136 3333 3431 207a 204d 2031 312e  .3163341 z M 11.
+00006de0: 3038 3331 3732 2c31 332e 3633 3239 3335  083172,13.632935
+00006df0: 2043 2031 312e 3038 3331 3732 2c31 322e   C 11.083172,12.
+00006e00: 3334 3731 3434 2031 302e 3632 3038 3532  347144 10.620852
+00006e10: 2c31 312e 3234 3836 3035 2039 2e36 3833  ,11.248605 9.683
+00006e20: 3731 3739 2c31 302e 3332 3438 3334 2043  7179,10.324834 C
+00006e30: 2038 2e37 3436 3538 3339 2c39 2e34 3133   8.7465839,9.413
+00006e40: 3534 3533 2037 2e36 3232 3032 3239 2c38  5453 7.6220229,8
+00006e50: 2e39 3531 3635 3935 2036 2e33 3232 3533  .9516595 6.32253
+00006e60: 3039 2c38 2e39 3531 3635 3935 2043 2035  09,8.9516595 C 5
+00006e70: 2e30 3233 3033 3739 2c38 2e39 3531 3635  .0230379,8.95165
+00006e80: 3935 2033 2e39 3233 3436 3739 2c39 2e34  95 3.9234679,9.4
+00006e90: 3031 3036 3139 2033 2e30 3233 3831 3839  010619 3.0238189
+00006ea0: 2c31 302e 3239 3938 3637 2043 2032 2e31  ,10.299867 C 2.1
+00006eb0: 3234 3137 3039 2c31 312e 3139 3836 3732  241709,11.198672
+00006ec0: 2031 2e36 3734 3334 3631 2c31 322e 3239   1.6743461,12.29
+00006ed0: 3732 3131 2031 2e36 3734 3334 3631 2c31  7211 1.6743461,1
+00006ee0: 332e 3539 3534 3834 2043 2031 2e36 3734  3.595484 C 1.674
+00006ef0: 3334 3631 2c31 342e 3931 3837 3235 2032  3461,14.918725 2
+00006f00: 2e31 3336 3636 3539 2c31 362e 3034 3232  .1366659,16.0422
+00006f10: 3331 2033 2e30 3438 3830 3839 2c31 362e  31 3.0488089,16.
+00006f20: 3936 3630 3032 2043 2033 2e39 3438 3435  966002 C 3.94845
+00006f30: 3739 2c31 372e 3838 3937 3734 2035 2e30  79,17.889774 5.0
+00006f40: 3630 3532 3339 2c31 382e 3335 3136 3620  605239,18.35166 
+00006f50: 362e 3336 3030 3135 392c 3138 2e33 3531  6.3600159,18.351
+00006f60: 3636 2043 2037 2e36 3539 3530 3839 2c31  66 C 7.6595089,1
+00006f70: 382e 3335 3136 3620 382e 3738 3430 3638  8.35166 8.784068
+00006f80: 392c 3137 2e38 3839 3737 3420 392e 3639  9,17.889774 9.69
+00006f90: 3632 3132 392c 3136 2e39 3636 3030 3220  62129,16.966002 
+00006fa0: 4320 3130 2e36 3230 3835 322c 3136 2e30  C 10.620852,16.0
+00006fb0: 3432 3233 3120 3131 2e30 3833 3137 322c  42231 11.083172,
+00006fc0: 3134 2e39 3331 3230 3820 3131 2e30 3833  14.931208 11.083
+00006fd0: 3137 322c 3133 2e36 3332 3933 3520 7a20  172,13.632935 z 
+00006fe0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00006ff0: 2020 2020 2020 2020 2020 7374 796c 653d            style=
+00007000: 2266 696c 6c3a 2024 7a6f 6469 6163 5f63  "fill: $zodiac_c
+00007010: 6f6c 6f72 5f33 220a 2020 2020 2020 2020  olor_3".        
+00007020: 2020 2020 2020 2020 2020 2020 2f3e 0a20              />. 
+00007030: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00007040: 2f73 796d 626f 6c3e 0a20 2020 2020 2020  /symbol>.       
+00007050: 2020 2020 2020 2020 203c 7379 6d62 6f6c           <symbol
+00007060: 2069 643d 226c 656f 223e 0a20 2020 2020   id="leo">.     
+00007070: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00007080: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
+00007090: 2020 2020 2020 2020 2020 2020 2064 3d22               d="
+000070a0: 4d20 3238 2e30 3231 3337 312c 3239 2e34  M 28.021371,29.4
+000070b0: 3830 3832 3120 4320 3237 2e33 3738 3333  80821 C 27.37833
+000070c0: 392c 3330 2e30 3639 3934 3820 3236 2e36  9,30.069948 26.6
+000070d0: 3837 3939 322c 3330 2e36 3132 3339 3220  87992,30.612392 
+000070e0: 3235 2e39 3333 3630 322c 3331 2e30 3532  25.933602,31.052
+000070f0: 3335 3920 4320 3235 2e33 3034 3339 342c  359 C 25.304394,
+00007100: 3331 2e34 3138 3730 3120 3234 2e36 3237  31.418701 24.627
+00007110: 3432 392c 3331 2e37 3132 3039 3120 3233  429,31.712091 23
+00007120: 2e39 3135 3032 322c 3331 2e38 3730 3437  .915022,31.87047
+00007130: 3220 4320 3233 2e34 3837 3830 372c 3331  2 C 23.487807,31
+00007140: 2e39 3636 2032 332e 3034 3839 3737 2c33  .966 23.048977,3
+00007150: 322e 3031 3032 3632 2032 322e 3631 3132  2.010262 22.6112
+00007160: 3739 2c33 312e 3939 3739 3938 2043 2032  79,31.997998 C 2
+00007170: 312e 3939 3630 3835 2c33 312e 3938 3431  1.996085,31.9841
+00007180: 3537 2032 312e 3338 3033 3435 2c33 312e  57 21.380345,31.
+00007190: 3837 3734 3534 2032 302e 3830 3439 3131  877454 20.804911
+000071a0: 2c33 312e 3635 3634 3236 2043 2032 302e  ,31.656426 C 20.
+000071b0: 3237 3334 3539 2c33 312e 3435 3337 3920  273459,31.45379 
+000071c0: 3139 2e37 3830 3432 2c33 312e 3135 3339  19.78042,31.1539
+000071d0: 3033 2031 392e 3335 3034 3535 2c33 302e  03 19.350455,30.
+000071e0: 3738 3230 3238 2043 2031 392e 3031 3539  782028 C 19.0159
+000071f0: 342c 3330 2e34 3933 3736 3920 3138 2e37  4,30.493769 18.7
+00007200: 3138 3030 322c 3330 2e31 3632 3735 3720  18002,30.162757 
+00007210: 3138 2e34 3637 3736 322c 3239 2e37 3938  18.467762,29.798
+00007220: 3834 3620 4320 3138 2e31 3538 3738 312c  846 C 18.158781,
+00007230: 3239 2e33 3439 3633 3320 3137 2e39 3239  29.349633 17.929
+00007240: 3738 322c 3238 2e38 3435 3733 3920 3137  782,28.845739 17
+00007250: 2e37 3934 3732 352c 3238 2e33 3137 3437  .794725,28.31747
+00007260: 3920 4320 3137 2e36 3335 3934 2c32 372e  9 C 17.63594,27.
+00007270: 3730 3038 3731 2031 372e 3630 3133 3535  700871 17.601355
+00007280: 2c32 372e 3035 3632 3337 2031 372e 3635  ,27.056237 17.65
+00007290: 3838 3936 2c32 362e 3432 3334 3032 2043  8896,26.423402 C
+000072a0: 2031 372e 3731 3634 3835 2c32 352e 3738   17.716485,25.78
+000072b0: 3338 3732 2031 372e 3834 3830 3133 2c32  3872 17.848013,2
+000072c0: 352e 3135 3333 3036 2031 382e 3030 3834  5.153306 18.0084
+000072d0: 3439 2c32 342e 3533 3233 3534 2043 2031  49,24.532354 C 1
+000072e0: 382e 3235 3639 3035 2c32 332e 3538 3036  8.256905,23.5806
+000072f0: 3131 2031 382e 3537 3738 3733 2c32 322e  11 18.577873,22.
+00007300: 3634 3933 3520 3138 2e39 3238 3439 312c  64935 18.928491,
+00007310: 3231 2e37 3330 3837 3320 4320 3139 2e34  21.730873 C 19.4
+00007320: 3434 3935 382c 3230 2e33 3833 3731 3620  44958,20.383716 
+00007330: 3230 2e30 3330 3137 342c 3139 2e30 3633  20.030174,19.063
+00007340: 3938 3820 3230 2e36 3434 3937 312c 3137  988 20.644971,17
+00007350: 2e37 3539 3134 3420 4320 3231 2e31 3337  .759144 C 21.137
+00007360: 3230 352c 3136 2e37 3130 3130 3120 3231  205,16.710101 21
+00007370: 2e36 3239 3433 372c 3135 2e36 3631 3036  .629437,15.66106
+00007380: 2032 322e 3132 3136 3639 2c31 342e 3631   22.121669,14.61
+00007390: 3230 3137 2043 2032 322e 3536 3332 3237  2017 C 22.563227
+000073a0: 2c31 332e 3636 3532 3038 2032 322e 3936  ,13.665208 22.96
+000073b0: 3537 3433 2c31 322e 3639 3834 3520 3233  5743,12.69845 23
+000073c0: 2e32 3836 3035 322c 3131 2e37 3033 3433  .286052,11.70343
+000073d0: 3220 4320 3233 2e35 3134 3039 392c 3130  2 C 23.514099,10
+000073e0: 2e39 3930 3731 2032 332e 3730 3132 3535  .99071 23.701255
+000073f0: 2c31 302e 3236 3235 3034 2032 332e 3830  ,10.262504 23.80
+00007400: 3131 3831 2c39 2e35 3230 3032 3836 2043  1181,9.5200286 C
+00007410: 2032 332e 3835 3231 3936 2c39 2e31 3430   23.852196,9.140
+00007420: 3537 3436 2032 332e 3837 3735 3837 2c38  5746 23.877587,8
+00007430: 2e37 3537 3339 3136 2032 332e 3836 3933  .7573916 23.8693
+00007440: 3131 2c38 2e33 3734 3437 3636 2043 2032  11,8.3744766 C 2
+00007450: 332e 3835 3638 3939 2c37 2e35 3836 3933  3.856899,7.58693
+00007460: 3134 2032 332e 3735 3035 3439 2c36 2e37  14 23.750549,6.7
+00007470: 3936 3536 3138 2032 332e 3530 3533 3031  965618 23.505301
+00007480: 2c36 2e30 3436 3336 3335 2043 2032 332e  ,6.0463635 C 23.
+00007490: 3330 3130 3538 2c35 2e34 3138 3630 3520  301058,5.418605 
+000074a0: 3232 2e39 3936 3535 392c 342e 3832 3234  22.996559,4.8224
+000074b0: 3637 3420 3232 2e35 3937 3430 312c 342e  674 22.597401,4.
+000074c0: 3239 3631 3432 3120 4320 3232 2e33 3731  2961421 C 22.371
+000074d0: 3130 372c 332e 3939 3731 3838 3120 3232  107,3.9971881 22
+000074e0: 2e31 3135 3838 2c33 2e37 3230 3335 3332  .11588,3.7203532
+000074f0: 2032 312e 3833 3931 3332 2c33 2e34 3637   21.839132,3.467
+00007500: 3533 3333 2043 2032 312e 3337 3933 382c  5333 C 21.37938,
+00007510: 332e 3034 3837 3533 3220 3230 2e38 3438  3.0487532 20.848
+00007520: 3631 2c32 2e37 3038 3234 3234 2032 302e  61,2.7082424 20.
+00007530: 3237 3538 3236 2c32 2e34 3636 3031 3734  275826,2.4660174
+00007540: 2043 2031 392e 3632 3332 3031 2c32 2e31   C 19.623201,2.1
+00007550: 3838 3432 3920 3138 2e39 3231 3335 312c  88429 18.921351,
+00007560: 322e 3033 3733 3937 2031 382e 3231 3535  2.037397 18.2155
+00007570: 382c 312e 3938 3334 3937 3320 4320 3137  8,1.9834973 C 17
+00007580: 2e37 3038 3935 322c 312e 3934 3535 3838  .708952,1.945588
+00007590: 3220 3137 2e31 3938 3639 312c 312e 3935  2 17.198691,1.95
+000075a0: 3034 3538 3220 3136 2e36 3933 3338 342c  04582 16.693384,
+000075b0: 322e 3030 3433 3035 3420 4320 3136 2e30  2.0043054 C 16.0
+000075c0: 3138 3434 352c 322e 3037 3635 3630 3820  18445,2.0765608 
+000075d0: 3135 2e33 3530 3832 382c 322e 3234 3437  15.350828,2.2447
+000075e0: 3736 3620 3134 2e37 3334 3137 312c 322e  766 14.734171,2.
+000075f0: 3533 3133 3038 3320 4320 3134 2e31 3737  5313083 C 14.177
+00007600: 3130 352c 322e 3738 3838 3537 2031 332e  105,2.788857 13.
+00007610: 3636 3530 3433 2c33 2e31 3432 3339 3735  665043,3.1423975
+00007620: 2031 332e 3232 3433 3138 2c33 2e35 3639   13.224318,3.569
+00007630: 3334 3739 2043 2031 322e 3739 3535 3335  3479 C 12.795535
+00007640: 2c33 2e39 3935 3133 3333 2031 322e 3433  ,3.9951333 12.43
+00007650: 3534 3537 2c34 2e34 3931 3234 3138 2031  5457,4.4912418 1
+00007660: 322e 3137 3237 3139 2c35 2e30 3335 3837  2.172719,5.03587
+00007670: 3733 2043 2031 312e 3839 3030 3934 2c35  73 C 11.890094,5
+00007680: 2e36 3138 3134 3637 2031 312e 3731 3936  .6181467 11.7196
+00007690: 3432 2c36 2e32 3531 3330 3831 2031 312e  42,6.2513081 11.
+000076a0: 3634 3339 3437 2c36 2e38 3933 3130 3239  643947,6.8931029
+000076b0: 2043 2031 312e 3536 3230 3137 2c37 2e35   C 11.562017,7.5
+000076c0: 3834 3433 3233 2031 312e 3538 3238 322c  844323 11.58282,
+000076d0: 382e 3238 3537 3339 3620 3131 2e36 3830  8.2857396 11.680
+000076e0: 3533 332c 382e 3937 3433 3033 3620 4320  533,8.9743036 C 
+000076f0: 3131 2e38 3036 3038 312c 392e 3836 3137  11.806081,9.8617
+00007700: 3630 3620 3132 2e30 3438 3937 352c 3130  606 12.048975,10
+00007710: 2e37 3239 3135 3220 3132 2e33 3534 3033  .729152 12.35403
+00007720: 332c 3131 2e35 3730 3639 3120 4320 3132  3,11.570691 C 12
+00007730: 2e35 3938 3739 382c 3132 2e32 3434 3833  .598798,12.24483
+00007740: 3720 3132 2e38 3835 3439 392c 3132 2e39  7 12.885499,12.9
+00007750: 3033 3131 3720 3133 2e31 3938 3339 382c  03117 13.198398,
+00007760: 3133 2e35 3438 3236 3820 4320 3133 2e34  13.548268 C 13.4
+00007770: 3039 3936 342c 3133 2e39 3837 3638 3220  09964,13.987682 
+00007780: 3133 2e36 3231 3931 312c 3134 2e34 3236  13.621911,14.426
+00007790: 3931 3520 3133 2e38 3333 3137 312c 3134  915 13.833171,14
+000077a0: 2e38 3636 3437 3520 4320 3134 2e31 3830  .866475 C 14.180
+000077b0: 3438 382c 3135 2e35 3936 2031 342e 3530  488,15.596 14.50
+000077c0: 3738 3633 2c31 362e 3333 3631 3136 2031  7863,16.336116 1
+000077d0: 342e 3738 3137 342c 3137 2e30 3936 3636  4.78174,17.09666
+000077e0: 3420 4320 3134 2e39 3534 3633 392c 3137  4 C 14.954639,17
+000077f0: 2e35 3830 3930 3320 3135 2e31 3037 3734  .580903 15.10774
+00007800: 312c 3138 2e30 3733 3839 3820 3135 2e32  1,18.073898 15.2
+00007810: 3034 3636 342c 3138 2e35 3739 3436 3820  04664,18.579468 
+00007820: 4320 3135 2e32 3630 3631 352c 3138 2e38  C 15.260615,18.8
+00007830: 3734 3430 3420 3135 2e32 3935 3930 352c  74404 15.295905,
+00007840: 3139 2e31 3734 3439 3220 3135 2e32 3838  19.174492 15.288
+00007850: 3530 312c 3139 2e34 3735 3039 3620 4320  501,19.475096 C 
+00007860: 3135 2e32 3739 3533 312c 3230 2e31 3230  15.279531,20.120
+00007870: 3036 3420 3135 2e31 3634 3035 382c 3230  064 15.164058,20
+00007880: 2e37 3634 3537 3520 3134 2e39 3336 3332  .764575 14.93632
+00007890: 2c32 312e 3336 3835 3633 2043 2031 342e  ,21.368563 C 14.
+000078a0: 3730 3235 3632 2c32 312e 3939 3239 3338  702562,21.992938
+000078b0: 2031 342e 3335 3133 3936 2c32 322e 3537   14.351396,22.57
+000078c0: 3033 3737 2031 332e 3932 3236 3134 2c32  0377 13.922614,2
+000078d0: 332e 3037 3937 3239 2043 2031 332e 3539  3.079729 C 13.59
+000078e0: 3631 3638 2c32 332e 3436 3637 3638 2031  6168,23.466768 1
+000078f0: 332e 3232 3934 3435 2c32 332e 3832 3033  3.229445,23.8203
+00007900: 3035 2031 322e 3832 3830 312c 3234 2e31  05 12.82801,24.1
+00007910: 3239 3030 3620 4320 3132 2e33 3030 3439  29006 C 12.30049
+00007920: 342c 3234 2e35 3334 3635 3320 3131 2e37  4,24.534653 11.7
+00007930: 3037 3032 312c 3234 2e38 3536 3237 3720  07021,24.856277 
+00007940: 3131 2e30 3734 3335 2c32 352e 3036 3430  11.07435,25.0640
+00007950: 3431 2043 2031 302e 3432 3830 3533 2c32  41 C 10.428053,2
+00007960: 352e 3237 3739 3039 2039 2e37 3434 3933  5.277909 9.74493
+00007970: 3735 2c32 352e 3337 3231 3933 2039 2e30  75,25.372193 9.0
+00007980: 3635 3033 3939 2c32 352e 3336 3337 3637  650399,25.363767
+00007990: 2043 2038 2e33 3735 3935 3933 2c32 352e   C 8.3759593,25.
+000079a0: 3335 3638 3639 2037 2e36 3835 3530 3138  356869 7.6855018
+000079b0: 2c32 352e 3234 3735 3931 2037 2e30 3335  ,25.247591 7.035
+000079c0: 3538 3139 2c32 352e 3031 3535 3537 2043  5819,25.015557 C
+000079d0: 2036 2e34 3232 3234 3337 2c32 342e 3739   6.4222437,24.79
+000079e0: 3831 3338 2035 2e38 3438 3936 3837 2c32  8138 5.8489687,2
+000079f0: 342e 3437 3137 3036 2035 2e33 3432 3931  4.471706 5.34291
+00007a00: 3138 2c32 342e 3036 3331 3333 2043 2035  18,24.063133 C 5
+00007a10: 2e30 3433 3936 3935 2c32 332e 3832 3233  .0439695,23.8223
+00007a20: 3238 2034 2e37 3637 3734 3931 2c32 332e  28 4.7677491,23.
+00007a30: 3535 3338 3938 2034 2e35 3132 3335 3733  553898 4.5123573
+00007a40: 2c32 332e 3236 3735 2043 2034 2e30 3735  ,23.2675 C 4.075
+00007a50: 3535 3331 2c32 322e 3737 3536 3438 2033  5531,22.775648 3
+00007a60: 2e37 3134 3137 3432 2c32 322e 3231 3439  .7141742,22.2149
+00007a70: 3434 2033 2e34 3631 3635 3138 2c32 312e  44 3.4616518,21.
+00007a80: 3630 3638 3434 2043 2033 2e32 3033 3737  606844 C 3.20377
+00007a90: 3737 2c32 302e 3938 3939 3520 332e 3035  77,20.98995 3.05
+00007aa0: 3934 3337 382c 3230 2e33 3238 3235 3920  94378,20.328259 
+00007ab0: 332e 3031 3537 3932 382c 3139 2e36 3631  3.0157928,19.661
+00007ac0: 3830 3620 4320 322e 3936 3933 3031 382c  806 C 2.9693018,
+00007ad0: 3138 2e39 3535 3433 3320 332e 3032 3331  18.955433 3.0231
+00007ae0: 3833 382c 3138 2e32 3339 3339 3720 332e  838,18.239397 3.
+00007af0: 3230 3737 3130 342c 3137 2e35 3534 3734  2077104,17.55474
+00007b00: 2043 2033 2e33 3732 3732 3235 2c31 362e   C 3.3727225,16.
+00007b10: 3933 3732 3333 2033 2e36 3434 3733 3733  937233 3.6447373
+00007b20: 2c31 362e 3334 3931 3934 2034 2e30 3034  ,16.349194 4.004
+00007b30: 3133 3939 2c31 352e 3832 3039 3031 2043  1399,15.820901 C
+00007b40: 2034 2e33 3032 3734 332c 3135 2e33 3739   4.302743,15.379
+00007b50: 3930 3620 342e 3636 3037 3230 382c 3134  906 4.6607208,14
+00007b60: 2e39 3831 3038 3420 352e 3035 3236 3132  .981084 5.052612
+00007b70: 362c 3134 2e36 3231 3237 3320 4320 352e  6,14.621273 C 5.
+00007b80: 3534 3231 3339 392c 3134 2e31 3733 3436  5421399,14.17346
+00007b90: 3720 362e 3130 3133 3632 392c 3133 2e37  7 6.1013629,13.7
+00007ba0: 3938 3733 3420 362e 3731 3231 3934 332c  98734 6.7121943,
+00007bb0: 3133 2e35 3337 3637 3320 4320 372e 3330  13.537673 C 7.30
+00007bc0: 3230 3838 372c 3133 2e32 3833 3931 2037  20887,13.28391 7
+00007bd0: 2e39 3336 3832 3231 2c31 332e 3133 3837  .9368221,13.1387
+00007be0: 3631 2038 2e35 3737 3136 3235 2c31 332e  61 8.5771625,13.
+00007bf0: 3039 3737 3439 2043 2038 2e38 3937 3135  097749 C 8.89715
+00007c00: 3834 2c31 332e 3037 3637 3137 2039 2e32  84,13.076717 9.2
+00007c10: 3138 3938 3337 2c31 332e 3037 3934 3733  189837,13.079473
+00007c20: 2039 2e35 3338 3039 3233 2c31 332e 3131   9.5380923,13.11
+00007c30: 3233 3736 2043 2031 302e 3031 3833 3235  2376 C 10.018325
+00007c40: 2c31 332e 3136 3038 3634 2031 302e 3439  ,13.160864 10.49
+00007c50: 3134 3135 2c31 332e 3236 3735 3220 3130  1415,13.26752 10
+00007c60: 2e39 3531 3837 372c 3133 2e34 3130 3835  .951877,13.41085
+00007c70: 3120 4320 3130 2e34 3736 3637 382c 3132  1 C 10.476678,12
+00007c80: 2e34 3933 3236 3220 3130 2e30 3536 3935  .493262 10.05695
+00007c90: 312c 3131 2e35 3434 3035 3520 392e 3734  1,11.544055 9.74
+00007ca0: 3538 3136 362c 3130 2e35 3537 3635 3820  58166,10.557658 
+00007cb0: 4320 392e 3439 3136 3432 2c39 2e37 3438  C 9.491642,9.748
+00007cc0: 3832 3836 2039 2e33 3130 3936 3139 2c38  8286 9.3109619,8
+00007cd0: 2e39 3132 3835 3436 2039 2e32 3632 3234  .9128546 9.26224
+00007ce0: 3136 2c38 2e30 3634 3937 3236 2043 2039  16,8.0649726 C 9
+00007cf0: 2e32 3336 3330 352c 372e 3630 3331 3330  .236305,7.603130
+00007d00: 3820 392e 3235 3036 3137 2c37 2e31 3339  8 9.250617,7.139
+00007d10: 3132 3937 2039 2e33 3031 3236 3539 2c36  1297 9.3012659,6
+00007d20: 2e36 3739 3431 3037 2043 2039 2e33 3836  .6794107 C 9.386
+00007d30: 3235 3037 2c35 2e39 3133 3236 3835 2039  2507,5.9132685 9
+00007d40: 2e35 3836 3838 3032 2c35 2e31 3538 3230  .5868802,5.15820
+00007d50: 3338 2039 2e39 3132 3735 3337 2c34 2e34  38 9.9127537,4.4
+00007d60: 3538 3834 3837 2043 2031 302e 3233 3335  588487 C 10.2335
+00007d70: 3437 2c33 2e37 3636 3438 3936 2031 302e  47,3.7664896 10.
+00007d80: 3637 3531 3731 2c33 2e31 3332 3532 2031  675171,3.13252 1
+00007d90: 312e 3139 3937 3438 2c32 2e35 3739 3331  1.199748,2.57931
+00007da0: 3838 2043 2031 312e 3835 3135 3031 2c31  88 C 11.851501,1
+00007db0: 2e38 3932 3730 3738 2031 322e 3631 3936  .8927078 12.6196
+00007dc0: 3034 2c31 2e33 3134 3437 3436 2031 332e  04,1.3144746 13.
+00007dd0: 3436 3739 3735 2c30 2e38 3933 3033 3637  467975,0.8930367
+00007de0: 3220 4320 3134 2e32 3337 3534 362c 302e  2 C 14.237546,0.
+00007df0: 3530 3931 3037 3832 2031 352e 3036 3935  50910782 15.0695
+00007e00: 3637 2c30 2e32 3536 3137 3134 3220 3135  67,0.25617142 15
+00007e10: 2e39 3138 3339 312c 302e 3132 3330 3836  .918391,0.123086
+00007e20: 3932 2043 2031 362e 3734 3434 3539 2c2d  92 C 16.744459,-
+00007e30: 302e 3030 3732 3337 3238 3338 2031 372e  0.0072372838 17.
+00007e40: 3538 3534 3532 2c2d 302e 3032 3639 3837  585452,-0.026987
+00007e50: 3738 3420 3138 2e34 3138 3937 372c 302e  784 18.418977,0.
+00007e60: 3032 3933 3836 3631 3620 4320 3139 2e33  029386616 C 19.3
+00007e70: 3639 3239 352c 302e 3039 3533 3637 3931  69295,0.09536791
+00007e80: 3620 3230 2e33 3135 3438 342c 302e 3237  6 20.315484,0.27
+00007e90: 3935 3837 3132 2032 312e 3230 3633 3538  958712 21.206358
+00007ea0: 2c30 2e36 3231 3337 3631 3220 4320 3231  ,0.62137612 C 21
+00007eb0: 2e39 3731 3237 392c 302e 3931 3335 3739  .971279,0.913579
+00007ec0: 3032 2032 322e 3639 3136 3433 2c31 2e33  02 22.691643,1.3
+00007ed0: 3233 3830 3735 2032 332e 3332 3834 3331  238075 23.328431
+00007ee0: 2c31 2e38 3339 3038 3536 2043 2032 332e  ,1.8390856 C 23.
+00007ef0: 3632 3130 3632 2c32 2e30 3735 3336 3637  621062,2.0753667
+00007f00: 2032 332e 3839 3732 3931 2c32 2e33 3332   23.897291,2.332
+00007f10: 3231 3638 2032 342e 3135 3035 3133 2c32  2168 24.150513,2
+00007f20: 2e36 3130 3435 3132 2043 2032 342e 3638  .6104512 C 24.68
+00007f30: 3533 3536 2c33 2e31 3933 3336 3534 2032  5356,3.1933654 2
+00007f40: 352e 3132 3734 3837 2c33 2e38 3631 3236  5.127487,3.86126
+00007f50: 3734 2032 352e 3435 3331 3936 2c34 2e35  74 25.453196,4.5
+00007f60: 3832 3334 3520 4320 3235 2e38 3137 3834  82345 C 25.81784
+00007f70: 312c 352e 3338 3537 3830 3520 3236 2e30  1,5.3857805 26.0
+00007f80: 3338 3334 372c 362e 3235 3033 3236 3220  38347,6.2503262 
+00007f90: 3236 2e31 3430 3731 392c 372e 3132 3534  26.140719,7.1254
+00007fa0: 3238 3220 4320 3236 2e32 3031 3435 382c  282 C 26.201458,
+00007fb0: 372e 3633 3732 3137 3120 3236 2e32 3230  7.6372171 26.220
+00007fc0: 3834 392c 382e 3135 3332 3237 3620 3236  849,8.1532276 26
+00007fd0: 2e32 3132 3435 2c38 2e36 3638 3334 3136  .21245,8.6683416
+00007fe0: 2043 2032 362e 3230 3137 3235 2c39 2e34   C 26.201725,9.4
+00007ff0: 3036 3936 3936 2032 362e 3134 3730 3233  069696 26.147023
+00008000: 2c31 302e 3134 3638 3631 2032 362e 3031  ,10.146861 26.01
+00008010: 3130 3531 2c31 302e 3837 3336 3531 2043  1051,10.873651 C
+00008020: 2032 352e 3935 3738 3839 2c31 312e 3135   25.957889,11.15
+00008030: 3831 3432 2032 352e 3839 3035 3432 2c31  8142 25.890542,1
+00008040: 312e 3433 3939 3732 2032 352e 3830 3835  1.439972 25.8085
+00008050: 3536 2c31 312e 3731 3735 3338 2043 2032  56,11.717538 C 2
+00008060: 352e 3638 3831 3836 2c31 322e 3133 3739  5.688186,12.1379
+00008070: 3137 2032 352e 3533 3639 3638 2c31 322e  17 25.536968,12.
+00008080: 3534 3836 3938 2032 352e 3337 3932 3132  548698 25.379212
+00008090: 2c31 322e 3935 3632 3631 2043 2032 352e  ,12.956261 C 25.
+000080a0: 3037 3739 3633 2c31 332e 3732 3738 3437  077963,13.727847
+000080b0: 2032 342e 3734 3537 3635 2c31 342e 3438   24.745765,14.48
+000080c0: 3639 3038 2032 342e 3430 3539 3038 2c31  6908 24.405908,1
+000080d0: 352e 3234 3231 3331 2043 2032 342e 3234  5.242131 C 24.24
+000080e0: 3836 312c 3135 2e35 3931 3837 3320 3234  861,15.591873 24
+000080f0: 2e30 3837 3630 382c 3135 2e39 3339 3932  .087608,15.93992
+00008100: 3620 3233 2e39 3236 3935 392c 3136 2e32  6 23.926959,16.2
+00008110: 3838 3133 3420 4320 3233 2e35 3733 3933  88134 C 23.57393
+00008120: 322c 3137 2e30 3538 3837 3420 3233 2e32  2,17.058874 23.2
+00008130: 3230 3930 342c 3137 2e38 3239 3631 3520  20904,17.829615 
+00008140: 3232 2e38 3637 3837 362c 3138 2e36 3030  22.867876,18.600
+00008150: 3335 3520 4320 3232 2e32 3738 3831 322c  355 C 22.278812,
+00008160: 3139 2e38 3830 3035 3920 3231 2e37 3036  19.880059 21.706
+00008170: 3234 352c 3231 2e31 3637 3920 3231 2e31  245,21.1679 21.1
+00008180: 3832 3037 2c32 322e 3437 3537 3331 2043  8207,22.475731 C
+00008190: 2032 302e 3837 3536 3933 2c32 332e 3234   20.875693,23.24
+000081a0: 3432 3532 2032 302e 3538 3337 3936 2c32  4252 20.583796,2
+000081b0: 342e 3031 3933 3936 2032 302e 3333 3936  4.019396 20.3396
+000081c0: 3439 2c32 342e 3831 3032 3037 2043 2032  49,24.810207 C 2
+000081d0: 302e 3230 3533 3631 2c32 352e 3235 3036  0.205361,25.2506
+000081e0: 3237 2032 302e 3038 3333 3839 2c32 352e  27 20.083389,25.
+000081f0: 3639 3631 3336 2032 302e 3030 3738 3635  696136 20.007865
+00008200: 2c32 362e 3135 3038 3234 2043 2031 392e  ,26.150824 C 19.
+00008210: 3937 3031 3836 2c32 362e 3338 3034 3433  970186,26.380443
+00008220: 2031 392e 3934 3635 3235 2c32 362e 3631   19.946525,26.61
+00008230: 3332 3232 2031 392e 3935 3432 3331 2c32  3222 19.954231,2
+00008240: 362e 3834 3631 3435 2043 2031 392e 3936  6.846145 C 19.96
+00008250: 3338 3737 2c32 372e 3237 3530 3236 2032  3877,27.275026 2
+00008260: 302e 3033 3738 3137 2c32 372e 3730 3537  0.037817,27.7057
+00008270: 3620 3230 2e32 3032 3532 332c 3238 2e31  6 20.202523,28.1
+00008280: 3033 3236 3320 4320 3230 2e33 3335 3538  03263 C 20.33558
+00008290: 342c 3238 2e34 3236 3830 3620 3230 2e35  4,28.426806 20.5
+000082a0: 3239 3231 372c 3238 2e37 3234 3933 2032  29217,28.72493 2
+000082b0: 302e 3736 3931 3638 2c32 382e 3937 3933  0.769168,28.9793
+000082c0: 3633 2043 2032 312e 3030 3731 3331 2c32  63 C 21.007131,2
+000082d0: 392e 3234 3433 3438 2032 312e 3239 3634  9.244348 21.2964
+000082e0: 3839 2c32 392e 3436 3435 3639 2032 312e  89,29.464569 21.
+000082f0: 3632 3035 3738 2c32 392e 3631 3333 3834  620578,29.613384
+00008300: 2043 2032 312e 3936 3636 3139 2c32 392e   C 21.966619,29.
+00008310: 3737 3338 3133 2032 322e 3334 3732 342c  773813 22.34724,
+00008320: 3239 2e38 3531 3733 3420 3232 2e37 3237  29.851734 22.727
+00008330: 3433 2c32 392e 3836 3337 3338 2043 2032  43,29.863738 C 2
+00008340: 332e 3039 3130 3236 2c32 392e 3837 3736  3.091026,29.8776
+00008350: 3535 2032 332e 3435 3530 362c 3239 2e38  55 23.45506,29.8
+00008360: 3232 3530 3320 3233 2e38 3033 3537 372c  22503 23.803577,
+00008370: 3239 2e37 3230 3334 3320 4320 3234 2e33  29.720343 C 24.3
+00008380: 3130 3533 332c 3239 2e35 3731 3737 2032  10533,29.57177 2
+00008390: 342e 3738 3633 3033 2c32 392e 3333 3137  4.786303,29.3317
+000083a0: 3331 2032 352e 3233 3238 3437 2c32 392e  31 25.232847,29.
+000083b0: 3035 3230 3434 2043 2032 352e 3733 3436  052044 C 25.7346
+000083c0: 3438 2c32 382e 3733 3635 3337 2032 362e  48,28.736537 26.
+000083d0: 3230 3138 3637 2c32 382e 3336 3837 3739  201867,28.368779
+000083e0: 2032 362e 3634 3535 3531 2c32 372e 3937   26.645551,27.97
+000083f0: 3634 3438 2043 2032 372e 3130 3431 3538  6448 C 27.104158
+00008400: 2c32 382e 3437 3739 3036 2032 372e 3536  ,28.477906 27.56
+00008410: 3237 3635 2c32 382e 3937 3933 3633 2032  2765,28.979363 2
+00008420: 382e 3032 3133 3731 2c32 392e 3438 3038  8.021371,29.4808
+00008430: 3231 207a 204d 2034 2e37 3439 3032 3735  21 z M 4.7490275
+00008440: 2c31 392e 3230 3637 3639 2043 2034 2e37  ,19.206769 C 4.7
+00008450: 3438 3431 3432 2c31 392e 3735 3530 3532  484142,19.755052
+00008460: 2034 2e38 3333 3635 3434 2c32 302e 3330   4.8336544,20.30
+00008470: 3538 3737 2035 2e30 3234 3531 3231 2c32  5877 5.0245121,2
+00008480: 302e 3832 3039 3120 4320 352e 3230 3231  0.82091 C 5.2021
+00008490: 3834 312c 3231 2e33 3034 3332 3520 352e  841,21.304325 5.
+000084a0: 3437 3235 3732 342c 3231 2e37 3532 3133  4725724,21.75213
+000084b0: 3820 352e 3831 3030 3439 332c 3232 2e31  8 5.8100493,22.1
+000084c0: 3430 3634 3420 4320 362e 3035 3436 3830  40644 C 6.054680
+000084d0: 362c 3232 2e34 3233 3437 3720 362e 3333  6,22.423477 6.33
+000084e0: 3437 3533 322c 3232 2e36 3735 3738 3720  47532,22.675787 
+000084f0: 362e 3634 3138 3238 312c 3232 2e38 3839  6.6418281,22.889
+00008500: 3138 3820 4320 372e 3034 3030 3237 372c  188 C 7.0400277,
+00008510: 3233 2e31 3635 3934 3120 372e 3438 3837  23.165941 7.4887
+00008520: 3033 362c 3233 2e33 3639 3831 3320 372e  036,23.369813 7.
+00008530: 3935 3935 3330 312c 3233 2e34 3836 3037  9595301,23.48607
+00008540: 3920 4320 382e 3432 3330 3437 342c 3233  9 C 8.4230474,23
+00008550: 2e36 3031 3135 3120 382e 3930 3439 3937  .601151 8.904997
+00008560: 312c 3233 2e36 3335 3438 3720 392e 3338  1,23.635487 9.38
+00008570: 3039 3632 2c32 332e 3630 3335 3634 2043  0962,23.603564 C
+00008580: 2039 2e38 3637 3135 3639 2c32 332e 3537   9.8671569,23.57
+00008590: 3033 3038 2031 302e 3334 3838 3132 2c32  0308 10.348812,2
+000085a0: 332e 3435 3435 3634 2031 302e 3739 3233  3.454564 10.7923
+000085b0: 3232 2c32 332e 3235 3133 3520 4320 3131  22,23.25135 C 11
+000085c0: 2e32 3539 3330 392c 3233 2e30 3339 3031  .259309,23.03901
+000085d0: 3820 3131 2e36 3830 3335 332c 3232 2e37  8 11.680353,22.7
+000085e0: 3332 3930 3120 3132 2e30 3433 3337 362c  32901 12.043376,
+000085f0: 3232 2e33 3731 3733 3120 4320 3132 2e34  22.371731 C 12.4
+00008600: 3135 3734 382c 3232 2e30 3033 3336 3420  15748,22.003364 
+00008610: 3132 2e37 3239 3536 332c 3231 2e35 3733  12.729563,21.573
+00008620: 3136 3820 3132 2e39 3439 3136 2c32 312e  168 12.94916,21.
+00008630: 3039 3637 3438 2043 2031 332e 3136 3631  096748 C 13.1661
+00008640: 3336 2c32 302e 3632 3934 3535 2031 332e  36,20.629455 13.
+00008650: 3239 3031 3534 2c32 302e 3132 3132 3138  290154,20.121218
+00008660: 2031 332e 3332 3830 3635 2c31 392e 3630   13.328065,19.60
+00008670: 3739 3838 2043 2031 332e 3335 3931 312c  7988 C 13.35911,
+00008680: 3139 2e31 3830 3430 3120 3133 2e33 3339  19.180401 13.339
+00008690: 3434 342c 3138 2e37 3438 3337 3720 3133  444,18.748377 13
+000086a0: 2e32 3631 3038 332c 3138 2e33 3236 3634  .261083,18.32664
+000086b0: 3420 4320 3133 2e31 3639 3533 332c 3137  4 C 13.169533,17
+000086c0: 2e38 3332 3433 3920 3132 2e39 3930 3634  .832439 12.99064
+000086d0: 322c 3137 2e33 3534 3120 3132 2e37 3330  2,17.3541 12.730
+000086e0: 3431 342c 3136 2e39 3233 3836 3320 4320  414,16.923863 C 
+000086f0: 3132 2e35 3436 3730 352c 3136 2e36 3139  12.546705,16.619
+00008700: 3232 3620 3132 2e33 3234 3833 342c 3136  226 12.324834,16
+00008710: 2e33 3337 3937 2031 322e 3037 3438 2c31  .33797 12.0748,1
+00008720: 362e 3038 3531 3234 2043 2031 312e 3730  6.085124 C 11.70
+00008730: 3735 3031 2c31 352e 3732 3037 3635 2031  7501,15.720765 1
+00008740: 312e 3238 3036 3135 2c31 352e 3431 3335  1.280615,15.4135
+00008750: 3033 2031 302e 3830 3831 3037 2c31 352e  03 10.808107,15.
+00008760: 3230 3037 3420 4320 3130 2e33 3533 3836  20074 C 10.35386
+00008770: 332c 3134 2e39 3934 3631 3520 392e 3836  3,14.994615 9.86
+00008780: 3130 3037 372c 3134 2e38 3738 3332 3520  10077,14.878325 
+00008790: 392e 3336 3338 3933 372c 3134 2e38 3434  9.3638937,14.844
+000087a0: 3934 3920 4320 382e 3831 3930 3131 382c  949 C 8.8190118,
+000087b0: 3134 2e38 3038 3036 3620 382e 3236 3531  14.808066 8.2651
+000087c0: 3436 342c 3134 2e38 3538 3533 3420 372e  464,14.858534 7.
+000087d0: 3734 3239 3637 392c 3135 2e30 3232 3633  7429679,15.02263
+000087e0: 3420 4320 372e 3238 3031 3432 312c 3135  4 C 7.2801421,15
+000087f0: 2e31 3636 3638 2036 2e38 3436 3730 3238  .16668 6.8467028
+00008800: 2c31 352e 3430 3030 3039 2036 2e34 3635  ,15.400009 6.465
+00008810: 3037 3337 2c31 352e 3639 3832 3133 2043  0737,15.698213 C
+00008820: 2036 2e30 3538 3638 3638 2c31 362e 3031   6.0586868,16.01
+00008830: 3533 3239 2035 2e37 3033 3831 3632 2c31  5329 5.7038162,1
+00008840: 362e 3339 3931 3734 2035 2e34 3233 3531  6.399174 5.42351
+00008850: 3835 2c31 362e 3833 3230 3235 2043 2035  85,16.832025 C 5
+00008860: 2e31 3533 3134 3839 2c31 372e 3234 3932  .1531489,17.2492
+00008870: 3333 2034 2e39 3539 3239 3832 2c31 372e  33 4.9592982,17.
+00008880: 3731 3536 3331 2034 2e38 3533 3936 3239  715631 4.8539629
+00008890: 2c31 382e 3230 3135 3131 2043 2034 2e37  ,18.201511 C 4.7
+000088a0: 3831 3739 3533 2c31 382e 3533 3133 3536  817953,18.531356
+000088b0: 2034 2e37 3438 3935 3035 2c31 382e 3836   4.7489505,18.86
+000088c0: 3932 3838 2034 2e37 3439 3032 3735 2c31  9288 4.7490275,1
+000088d0: 392e 3230 3637 3639 207a 2022 0a20 2020  9.206769 z ".   
+000088e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088f0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00008900: 3a20 247a 6f64 6961 635f 636f 6c6f 725f  : $zodiac_color_
+00008910: 3422 0a20 2020 2020 2020 2020 2020 2020  4".             
+00008920: 2020 2020 2020 202f 3e0a 2020 2020 2020         />.      
+00008930: 2020 2020 2020 2020 2020 3c2f 7379 6d62            </symb
+00008940: 6f6c 3e0a 2020 2020 2020 2020 2020 2020  ol>.            
+00008950: 2020 2020 3c73 796d 626f 6c20 6964 3d22      <symbol id="
+00008960: 7669 7267 6f22 3e0a 2020 2020 2020 2020  virgo">.        
+00008970: 2020 2020 2020 2020 2020 2020 3c70 6174              <pat
+00008980: 680a 2020 2020 2020 2020 2020 2020 2020  h.              
+00008990: 2020 2020 2020 2020 2020 643d 224d 2037            d="M 7
+000089a0: 2e31 3633 3238 3535 2c39 2e37 3438 3833  .1632855,9.74883
+000089b0: 3633 2043 2037 2e31 3633 3238 3535 2c31  63 C 7.1632855,1
+000089c0: 342e 3934 3938 3639 2037 2e31 3633 3238  4.949869 7.16328
+000089d0: 3535 2c32 302e 3135 3039 3033 2037 2e31  55,20.150903 7.1
+000089e0: 3633 3238 3535 2c32 352e 3335 3139 3336  632855,25.351936
+000089f0: 2043 2036 2e33 3331 3035 3435 2c32 352e   C 6.3310545,25.
+00008a00: 3335 3139 3336 2035 2e34 3938 3832 3335  351936 5.4988235
+00008a10: 2c32 352e 3335 3139 3336 2034 2e36 3636  ,25.351936 4.666
+00008a20: 3539 3235 2c32 352e 3335 3139 3336 2043  5925,25.351936 C
+00008a30: 2034 2e36 3636 3539 3235 2c31 392e 3332   4.6665925,19.32
+00008a40: 3831 3634 2034 2e36 3636 3539 3235 2c31  8164 4.6665925,1
+00008a50: 332e 3330 3433 3932 2034 2e36 3636 3539  3.304392 4.66659
+00008a60: 3235 2c37 2e32 3830 3631 3938 2043 2034  25,7.2806198 C 4
+00008a70: 2e36 3637 3334 3235 2c36 2e31 3035 3832  .6673425,6.10582
+00008a80: 3636 2034 2e35 3133 3738 3235 2c34 2e39  66 4.5137825,4.9
+00008a90: 3238 3932 3837 2034 2e31 3835 3733 3435  289287 4.1857345
+00008aa0: 2c33 2e37 3939 3838 3220 4320 332e 3837  ,3.799882 C 3.87
+00008ab0: 3138 3739 352c 322e 3731 3339 3830 3720  18795,2.7139807 
+00008ac0: 332e 3339 3638 3936 352c 312e 3637 3537  3.3968965,1.6757
+00008ad0: 3630 3620 322e 3738 3934 3134 392c 302e  606 2.7894149,0.
+00008ae0: 3732 3234 3935 3435 2043 2032 2e37 3334  72249545 C 2.734
+00008af0: 3830 3037 2c30 2e36 3334 3436 3537 2032  8007,0.6344657 2
+00008b00: 2e36 3730 3632 3537 2c30 2e35 3432 3635  .6706257,0.54265
+00008b10: 3931 3920 322e 3631 3931 3239 332c 302e  919 2.6191293,0.
+00008b20: 3435 3839 3134 3720 4320 332e 3439 3632  4589147 C 3.4962
+00008b30: 3138 352c 302e 3435 3839 3134 3720 342e  185,0.4589147 4.
+00008b40: 3337 3333 3036 352c 302e 3435 3839 3134  3733065,0.458914
+00008b50: 3720 352e 3235 3033 3936 352c 302e 3435  7 5.2503965,0.45
+00008b60: 3839 3134 3720 4320 352e 3739 3831 3936  89147 C 5.798196
+00008b70: 352c 312e 3230 3939 3638 3320 362e 3231  5,1.2099683 6.21
+00008b80: 3339 3734 352c 322e 3035 3039 3539 3320  39745,2.0509593 
+00008b90: 362e 3532 3735 3931 352c 322e 3932 3430  6.5275915,2.9240
+00008ba0: 3037 3320 4320 362e 3831 3431 3637 352c  073 C 6.8141675,
+00008bb0: 332e 3732 3230 3834 3820 372e 3031 3737  3.7220848 7.0177
+00008bc0: 3134 352c 342e 3534 3832 3134 3320 372e  145,4.5482143 7.
+00008bd0: 3136 3332 3835 352c 352e 3338 3239 3435  1632855,5.382945
+00008be0: 3520 4320 372e 3630 3731 3434 352c 342e  5 C 7.6071445,4.
+00008bf0: 3239 3539 3631 3320 382e 3132 3333 3637  2959613 8.123367
+00008c00: 352c 332e 3233 3535 3036 3220 382e 3735  5,3.2355062 8.75
+00008c10: 3131 3336 352c 322e 3234 3138 3430 3520  11365,2.2418405 
+00008c20: 4320 392e 3134 3933 3936 352c 312e 3631  C 9.1493965,1.61
+00008c30: 3234 3630 3120 392e 3539 3332 3737 352c  24601 9.5932775,
+00008c40: 312e 3031 3034 3538 3320 3130 2e30 3934  1.0104583 10.094
+00008c50: 3732 372c 302e 3435 3839 3134 3720 4320  727,0.4589147 C 
+00008c60: 3130 2e39 3130 3339 362c 302e 3330 3539  10.910396,0.3059
+00008c70: 3433 3535 2031 312e 3732 3630 3635 2c30  4355 11.726065,0
+00008c80: 2e31 3532 3937 3131 3620 3132 2e35 3431  .15297116 12.541
+00008c90: 3733 342c 342e 3434 3038 3932 3165 2d31  734,4.4408921e-1
+00008ca0: 3520 4320 3133 2e31 3135 3432 382c 302e  5 C 13.115428,0.
+00008cb0: 3733 3736 3233 3535 2031 332e 3535 3638  73762355 13.5568
+00008cc0: 3538 2c31 2e35 3732 3038 3933 2031 332e  58,1.5720893 13.
+00008cd0: 3838 3631 3239 2c32 2e34 3434 3637 3039  886129,2.4446709
+00008ce0: 2043 2031 342e 3237 3135 3935 2c33 2e34   C 14.271595,3.4
+00008cf0: 3636 3033 3532 2031 342e 3530 3931 362c  660352 14.50916,
+00008d00: 342e 3533 3832 3734 3520 3134 2e36 3531  4.5382745 14.651
+00008d10: 3531 322c 352e 3631 3839 3439 3220 4320  512,5.6189492 C 
+00008d20: 3134 2e36 3536 3338 332c 352e 3635 3630  14.656383,5.6560
+00008d30: 3239 3520 3134 2e36 3631 3134 312c 352e  295 14.661141,5.
+00008d40: 3639 3331 3233 3420 3134 2e36 3635 3738  6931234 14.66578
+00008d50: 362c 352e 3733 3032 3332 3320 4320 3135  6,5.7302323 C 15
+00008d60: 2e30 3338 3839 332c 342e 3535 3438 3634  .038893,4.554864
+00008d70: 3920 3135 2e35 3930 3537 312c 332e 3434  9 15.590571,3.44
+00008d80: 3034 3139 3120 3136 2e32 3538 3132 322c  04191 16.258122,
+00008d90: 322e 3430 3437 3732 3620 4320 3136 2e36  2.4047726 C 16.6
+00008da0: 3936 3633 362c 312e 3732 3431 3237 3720  96636,1.7241277 
+00008db0: 3137 2e31 3835 3030 342c 312e 3037 3631  17.185004,1.0761
+00008dc0: 3136 3620 3137 2e37 3039 3031 392c 302e  166 17.709019,0.
+00008dd0: 3435 3839 3134 3720 4320 3138 2e35 3132  4589147 C 18.512
+00008de0: 3236 372c 302e 3330 3539 3433 3535 2031  267,0.30594355 1
+00008df0: 392e 3331 3535 3134 2c30 2e31 3532 3937  9.315514,0.15297
+00008e00: 3131 3620 3230 2e31 3138 3736 322c 342e  116 20.118762,4.
+00008e10: 3434 3038 3932 3165 2d31 3520 4320 3230  4408921e-15 C 20
+00008e20: 2e37 3236 3535 392c 302e 3833 3934 3536  .726559,0.839456
+00008e30: 3635 2032 312e 3232 3238 3736 2c31 2e37  65 21.222876,1.7
+00008e40: 3631 3736 3132 2032 312e 3536 3532 3435  617612 21.565245
+00008e50: 2c32 2e37 3430 3431 3534 2043 2032 312e  ,2.7404154 C 21.
+00008e60: 3839 3831 3634 2c33 2e36 3837 3230 3335  898164,3.6872035
+00008e70: 2032 322e 3038 3530 3536 2c34 2e36 3833   22.085056,4.683
+00008e80: 3633 3339 2032 322e 3133 3131 3537 2c35  6339 22.131157,5
+00008e90: 2e36 3835 3630 3936 2043 2032 322e 3134  .6856096 C 22.14
+00008ea0: 3336 3038 2c35 2e39 3237 3033 3620 3232  3608,5.927036 22
+00008eb0: 2e31 3433 3639 362c 362e 3136 3837 3837  .143696,6.168787
+00008ec0: 3320 3232 2e31 3433 3434 342c 362e 3431  3 22.143444,6.41
+00008ed0: 3034 3534 3220 4320 3232 2e31 3433 3434  04542 C 22.14344
+00008ee0: 342c 372e 3932 3432 3832 3320 3232 2e31  4,7.9242823 22.1
+00008ef0: 3433 3434 342c 392e 3433 3831 3039 3220  43444,9.4381092 
+00008f00: 3232 2e31 3433 3434 342c 3130 2e39 3531  22.143444,10.951
+00008f10: 3933 3720 4320 3232 2e34 3831 3334 392c  937 C 22.481349,
+00008f20: 392e 3939 3830 3235 3320 3232 2e38 3538  9.9980253 22.858
+00008f30: 3939 322c 392e 3035 3636 3737 3920 3233  992,9.0566779 23
+00008f40: 2e33 3039 3635 392c 382e 3134 3938 3635  .309659,8.149865
+00008f50: 2043 2032 332e 3539 3633 342c 372e 3537   C 23.59634,7.57
+00008f60: 3533 3431 2032 332e 3931 3233 3236 2c37  5341 23.912326,7
+00008f70: 2e30 3133 3937 3739 2032 342e 3237 3939  .0139779 24.2799
+00008f80: 3137 2c36 2e34 3836 3832 3134 2043 2032  17,6.4868214 C 2
+00008f90: 342e 3936 3732 3332 2c36 2e32 3334 3632  4.967232,6.23462
+00008fa0: 3534 2032 352e 3635 3435 3438 2c35 2e39  54 25.654548,5.9
+00008fb0: 3832 3432 3832 2032 362e 3334 3138 3633  824282 26.341863
+00008fc0: 2c35 2e37 3330 3233 3233 2043 2032 372e  ,5.7302323 C 27.
+00008fd0: 3134 3634 3431 2c36 2e39 3730 3637 3632  146441,6.9706762
+00008fe0: 2032 372e 3830 3637 3537 2c38 2e33 3038   27.806757,8.308
+00008ff0: 3039 3838 2032 382e 3236 3234 3532 2c39  0988 28.262452,9
+00009000: 2e37 3135 3434 3735 2043 2032 382e 3637  .7154475 C 28.67
+00009010: 3930 3231 2c31 302e 3939 3731 3238 2032  9021,10.997128 2
+00009020: 382e 3932 3330 3137 2c31 322e 3333 3436  8.923017,12.3346
+00009030: 3235 2032 382e 3938 3338 3739 2c31 332e  25 28.983879,13.
+00009040: 3638 3037 3938 2043 2032 392e 3034 3939  680798 C 29.0499
+00009050: 3936 2c31 352e 3135 3138 3620 3238 2e39  96,15.15186 28.9
+00009060: 3133 3737 2c31 362e 3633 3339 3736 2032  1377,16.633976 2
+00009070: 382e 3535 3632 3534 2c31 382e 3036 3334  8.556254,18.0634
+00009080: 3031 2043 2032 382e 3135 3936 3435 2c31  01 C 28.159645,1
+00009090: 392e 3635 3437 3937 2032 372e 3439 3132  9.654797 27.4912
+000090a0: 3738 2c32 312e 3137 3536 3620 3236 2e36  78,21.17566 26.6
+000090b0: 3038 3734 362c 3232 2e35 3537 3634 3920  08746,22.557649 
+000090c0: 4320 3235 2e37 3936 3539 352c 3233 2e38  C 25.796595,23.8
+000090d0: 3331 3637 3220 3234 2e38 3131 3934 2c32  31672 24.81194,2
+000090e0: 342e 3939 3035 3332 2032 332e 3732 3930  4.990532 23.7290
+000090f0: 3533 2c32 362e 3034 3236 3231 2043 2032  53,26.042621 C 2
+00009100: 332e 3337 3632 3135 2c32 362e 3338 3534  3.376215,26.3854
+00009110: 3338 2032 332e 3031 3236 3738 2c32 362e  38 23.012678,26.
+00009120: 3731 3732 3238 2032 322e 3634 3032 3938  717228 22.640298
+00009130: 2c32 372e 3033 3837 3538 2043 2032 322e  ,27.038758 C 22.
+00009140: 3733 3039 3036 2c32 372e 3730 3332 3239  730906,27.703229
+00009150: 2032 322e 3934 3638 3131 2c32 382e 3334   22.946811,28.34
+00009160: 3532 3820 3233 2e32 3235 3738 312c 3238  528 23.225781,28
+00009170: 2e39 3533 3335 3420 4320 3233 2e35 3733  .953354 C 23.573
+00009180: 3039 2c32 392e 3730 3735 3631 2032 342e  09,29.707561 24.
+00009190: 3031 3636 3931 2c33 302e 3431 3339 3938  016691,30.413998
+000091a0: 2032 342e 3530 3336 3139 2c33 312e 3038   24.503619,31.08
+000091b0: 3534 3836 2043 2032 342e 3733 3032 3139  5486 C 24.730219
+000091c0: 2c33 312e 3339 3734 3037 2032 342e 3936  ,31.397407 24.96
+000091d0: 3730 3539 2c33 312e 3730 3138 3438 2032  7059,31.701848 2
+000091e0: 352e 3231 3135 3139 2c33 312e 3939 3939  5.211519,31.9999
+000091f0: 3938 2043 2032 342e 3233 3433 3732 2c33  98 C 24.234372,3
+00009200: 312e 3939 3939 3938 2032 332e 3235 3732  1.999998 23.2572
+00009210: 3236 2c33 312e 3939 3939 3938 2032 322e  26,31.999998 22.
+00009220: 3238 3030 3739 2c33 312e 3939 3939 3938  280079,31.999998
+00009230: 2043 2032 312e 3831 3537 3136 2c33 312e   C 21.815716,31.
+00009240: 3431 3332 3138 2032 312e 3433 3233 3638  413218 21.432368
+00009250: 2c33 302e 3736 3633 3137 2032 312e 3130  ,30.766317 21.10
+00009260: 3033 3435 2c33 302e 3039 3730 3731 2043  0345,30.097071 C
+00009270: 2032 302e 3833 3337 3436 2c32 392e 3535   20.833746,29.55
+00009280: 3834 3535 2032 302e 3630 3037 3536 2c32  8455 20.600756,2
+00009290: 392e 3030 3336 3733 2032 302e 3339 3230  9.003673 20.3920
+000092a0: 3332 2c32 382e 3434 3033 3038 2043 2031  32,28.440308 C 1
+000092b0: 392e 3339 3634 3232 2c32 392e 3030 3436  9.396422,29.0046
+000092c0: 3338 2031 382e 3332 3333 3931 2c32 392e  38 18.323391,29.
+000092d0: 3432 3338 3239 2031 372e 3232 3437 3932  423829 17.224792
+000092e0: 2c32 392e 3734 3031 3233 2043 2031 362e  ,29.740123 C 16.
+000092f0: 3338 3439 3731 2c32 392e 3938 3136 3038  384971,29.981608
+00009300: 2031 352e 3532 3836 312c 3330 2e31 3633   15.52861,30.163
+00009310: 3338 3520 3134 2e36 3635 3738 362c 3330  385 14.665786,30
+00009320: 2e33 3030 3737 3320 4320 3134 2e36 3635  .300773 C 14.665
+00009330: 3738 362c 3239 2e35 3839 3636 3220 3134  786,29.589662 14
+00009340: 2e36 3635 3738 362c 3238 2e38 3738 3535  .665786,28.87855
+00009350: 3120 3134 2e36 3635 3738 362c 3238 2e31  1 14.665786,28.1
+00009360: 3637 3434 2043 2031 352e 3831 3235 3032  6744 C 15.812502
+00009370: 2c32 372e 3933 3338 3831 2031 362e 3934  ,27.933881 16.94
+00009380: 3636 3031 2c32 372e 3632 3534 3236 2031  6601,27.625426 1
+00009390: 382e 3033 3635 3639 2c32 372e 3139 3732  8.036569,27.1972
+000093a0: 3331 2043 2031 382e 3638 3134 3833 2c32  31 C 18.681483,2
+000093b0: 362e 3934 3333 3539 2031 392e 3331 3034  6.943359 19.3104
+000093c0: 3632 2c32 362e 3634 3637 3833 2031 392e  62,26.646783 19.
+000093d0: 3930 3735 3939 2c32 362e 3239 3435 3732  907599,26.294572
+000093e0: 2043 2031 392e 3733 3037 3337 2c32 352e   C 19.730737,25.
+000093f0: 3139 3936 3120 3139 2e36 3433 3233 322c  19961 19.643232,
+00009400: 3234 2e30 3930 3239 2031 392e 3634 3637  24.09029 19.6467
+00009410: 3531 2c32 322e 3938 3131 3734 2043 2031  51,22.981174 C 1
+00009420: 392e 3634 3637 342c 3137 2e39 3438 3837  9.64674,17.94887
+00009430: 3720 3139 2e36 3436 3737 322c 3132 2e39  7 19.646772,12.9
+00009440: 3136 3537 3820 3139 2e36 3436 3733 352c  16578 19.646735,
+00009450: 372e 3838 3432 3831 3120 4320 3139 2e36  7.8842811 C 19.6
+00009460: 3434 3935 312c 362e 3935 3032 3032 3420  44951,6.9502024 
+00009470: 3139 2e35 3937 3032 362c 362e 3031 3431  19.597026,6.0141
+00009480: 3238 2031 392e 3435 3536 3737 2c35 2e30  28 19.455677,5.0
+00009490: 3839 3939 3636 2043 2031 392e 3334 3835  899966 C 19.3485
+000094a0: 3232 2c34 2e33 3938 3235 3731 2031 392e  22,4.3982571 19.
+000094b0: 3138 3839 3536 2c33 2e37 3131 3234 3720  188956,3.711247 
+000094c0: 3138 2e39 3330 3932 342c 332e 3035 3930  18.930924,3.0590
+000094d0: 3935 3720 4320 3138 2e38 3330 3037 362c  957 C 18.830076,
+000094e0: 322e 3830 3530 3935 3120 3138 2e37 3133  2.8050951 18.713
+000094f0: 3739 382c 322e 3535 3639 3733 3520 3138  798,2.5569735 18
+00009500: 2e35 3738 3531 342c 322e 3331 3933 3739  .578514,2.319379
+00009510: 3820 4320 3137 2e37 3338 3937 372c 332e  8 C 17.738977,3.
+00009520: 3232 3234 3536 3920 3137 2e30 3437 3935  2224569 17.04795
+00009530: 392c 342e 3235 3538 3334 3820 3136 2e34  9,4.2558348 16.4
+00009540: 3739 3730 362c 352e 3334 3735 3934 3120  79706,5.3475941 
+00009550: 4320 3135 2e38 3234 3432 392c 362e 3630  C 15.824429,6.60
+00009560: 3734 3837 3420 3135 2e33 3237 3634 372c  74874 15.327647,
+00009570: 372e 3934 3437 3739 3720 3134 2e39 3337  7.9447797 14.937
+00009580: 3336 332c 392e 3330 3834 3138 3720 4320  363,9.3084187 C 
+00009590: 3134 2e38 3430 3439 392c 392e 3634 3834  14.840499,9.6484
+000095a0: 3833 3220 3134 2e37 3439 3034 392c 392e  832 14.749049,9.
+000095b0: 3939 3032 3934 3320 3134 2e36 3635 3738  9902943 14.66578
+000095c0: 362c 3130 2e33 3333 3834 2043 2031 342e  6,10.33384 C 14.
+000095d0: 3636 3537 3836 2c31 352e 3333 3938 3732  665786,15.339872
+000095e0: 2031 342e 3636 3537 3836 2c32 302e 3334   14.665786,20.34
+000095f0: 3539 3034 2031 342e 3636 3537 3836 2c32  5904 14.665786,2
+00009600: 352e 3335 3139 3336 2043 2031 332e 3832  5.351936 C 13.82
+00009610: 3934 3135 2c32 352e 3335 3139 3336 2031  9415,25.351936 1
+00009620: 322e 3939 3330 3433 2c32 352e 3335 3139  2.993043,25.3519
+00009630: 3336 2031 322e 3135 3636 3732 2c32 352e  36 12.156672,25.
+00009640: 3335 3139 3336 2043 2031 322e 3135 3636  351936 C 12.1566
+00009650: 3631 2c31 392e 3830 3831 3034 2031 322e  61,19.808104 12.
+00009660: 3135 3636 3934 2c31 342e 3236 3432 3732  156694,14.264272
+00009670: 2031 322e 3135 3636 3535 2c38 2e37 3230   12.156655,8.720
+00009680: 3433 3938 2043 2031 322e 3135 3438 3636  4398 C 12.154866
+00009690: 2c37 2e36 3935 3936 3336 2031 322e 3131  ,7.6959636 12.11
+000096a0: 3630 3635 2c36 2e36 3730 3132 3433 2031  6065,6.6701243 1
+000096b0: 312e 3939 3735 3233 2c35 2e36 3531 3938  1.997523,5.65198
+000096c0: 3131 2043 2031 312e 3931 3631 3631 2c34  11 C 11.916161,4
+000096d0: 2e39 3636 3532 3633 2031 312e 3739 3939  .9665263 11.7999
+000096e0: 3538 2c34 2e32 3833 3033 3938 2031 312e  58,4.2830398 11.
+000096f0: 3630 3636 3131 2c33 2e36 3139 3531 3336  606611,3.6195136
+00009700: 2043 2031 312e 3437 3336 3433 2c33 2e31   C 11.473643,3.1
+00009710: 3638 3438 3938 2031 312e 3330 3530 3338  684898 11.305038
+00009720: 2c32 2e37 3234 3436 3837 2031 312e 3036  ,2.7244687 11.06
+00009730: 3335 3932 2c32 2e33 3139 3337 3938 2043  3592,2.3193798 C
+00009740: 2031 302e 3130 3134 3034 2c33 2e34 3338   10.101404,3.438
+00009750: 3036 3939 2039 2e32 3932 3138 3035 2c34  0699 9.2921805,4
+00009760: 2e36 3834 3236 3339 2038 2e36 3331 3730  .6842639 8.63170
+00009770: 3735 2c36 2e30 3032 3220 4320 382e 3032  75,6.0022 C 8.02
+00009780: 3932 3034 352c 372e 3230 3330 3433 3320  92045,7.2030433 
+00009790: 372e 3534 3736 3131 352c 382e 3436 3233  7.5476115,8.4623
+000097a0: 3732 3220 372e 3136 3332 3835 352c 392e  722 7.1632855,9.
+000097b0: 3734 3838 3336 3320 7a20 4d20 3232 2e31  7488363 z M 22.1
+000097c0: 3433 3434 342c 3234 2e37 3036 3937 3520  43444,24.706975 
+000097d0: 4320 3233 2e30 3736 3231 312c 3233 2e37  C 23.076211,23.7
+000097e0: 3630 3437 3220 3233 2e39 3039 3835 392c  60472 23.909859,
+000097f0: 3232 2e37 3132 3631 3420 3234 2e35 3837  22.712614 24.587
+00009800: 3631 382c 3231 2e35 3638 3833 3820 4320  618,21.568838 C 
+00009810: 3234 2e39 3134 3737 312c 3231 2e30 3136  24.914771,21.016
+00009820: 3635 3320 3235 2e32 3036 3835 312c 3230  653 25.206851,20
+00009830: 2e34 3433 3432 3920 3235 2e34 3536 3138  .443429 25.45618
+00009840: 392c 3139 2e38 3532 3034 3820 4320 3235  9,19.852048 C 25
+00009850: 2e39 3239 3438 392c 3138 2e37 3137 3539  .929489,18.71759
+00009860: 3420 3236 2e32 3434 3831 372c 3137 2e35  4 26.244817,17.5
+00009870: 3138 3039 3620 3236 2e33 3935 3135 332c  18096 26.395153,
+00009880: 3136 2e32 3938 3437 3620 4320 3236 2e34  16.298476 C 26.4
+00009890: 3931 3439 322c 3135 2e35 3136 3937 3120  91492,15.516971 
+000098a0: 3236 2e35 3233 3630 332c 3134 2e37 3237  26.523603,14.727
+000098b0: 3530 3120 3236 2e34 3930 3930 322c 3133  501 26.490902,13
+000098c0: 2e39 3430 3737 3520 4320 3236 2e34 3430  .940775 C 26.440
+000098d0: 3939 362c 3132 2e37 3536 3135 3920 3236  996,12.756159 26
+000098e0: 2e32 3331 3232 372c 3131 2e35 3738 3830  .231227,11.57880
+000098f0: 3220 3235 2e38 3732 3739 332c 3130 2e34  2 25.872793,10.4
+00009900: 3438 3537 2043 2032 352e 3638 3630 3836  4857 C 25.686086
+00009910: 2c39 2e38 3538 3338 3833 2032 352e 3435  ,9.8583883 25.45
+00009920: 3938 3034 2c39 2e32 3830 3834 3431 2032  9804,9.2808441 2
+00009930: 352e 3139 3930 3938 2c38 2e37 3139 3337  5.199098,8.71937
+00009940: 3934 2043 2032 342e 3530 3432 3332 2c39  94 C 24.504232,9
+00009950: 2e35 3733 3339 3620 3233 2e39 3333 3132  .573396 23.93312
+00009960: 362c 3130 2e35 3232 3039 3920 3233 2e34  6,10.522099 23.4
+00009970: 3438 3939 312c 3131 2e35 3038 3931 3420  48991,11.508914 
+00009980: 4320 3232 2e39 3236 3238 392c 3132 2e35  C 22.926289,12.5
+00009990: 3736 3234 3520 3232 2e35 3033 3237 372c  76245 22.503277,
+000099a0: 3133 2e36 3839 3935 3720 3232 2e31 3433  13.689957 22.143
+000099b0: 3434 342c 3134 2e38 3231 3730 3420 4320  444,14.821704 C 
+000099c0: 3232 2e31 3433 3434 342c 3138 2e31 3136  22.143444,18.116
+000099d0: 3739 3520 3232 2e31 3433 3434 342c 3231  795 22.143444,21
+000099e0: 2e34 3131 3838 3420 3232 2e31 3433 3434  .411884 22.14344
+000099f0: 342c 3234 2e37 3036 3937 3520 7a20 220a  4,24.706975 z ".
+00009a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a10: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+00009a20: 696c 6c3a 2024 7a6f 6469 6163 5f63 6f6c  ill: $zodiac_col
+00009a30: 6f72 5f35 220a 2020 2020 2020 2020 2020  or_5".          
+00009a40: 2020 2020 2020 2020 2020 2f3e 0a20 2020            />.   
+00009a50: 2020 2020 2020 2020 2020 2020 203c 2f73               </s
+00009a60: 796d 626f 6c3e 0a20 2020 2020 2020 2020  ymbol>.         
+00009a70: 2020 2020 2020 203c 7379 6d62 6f6c 2069         <symbol i
+00009a80: 643d 226c 6962 7261 223e 0a20 2020 2020  d="libra">.     
+00009a90: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00009aa0: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
+00009ab0: 2020 2020 2020 2020 2020 2020 2064 3d22               d="
+00009ac0: 4d20 2d35 2e35 3936 3235 652d 3036 2c32  M -5.59625e-06,2
+00009ad0: 392e 3139 3037 3039 2043 202d 352e 3539  9.190709 C -5.59
+00009ae0: 3632 3565 2d30 362c 3238 2e32 3033 3732  625e-06,28.20372
+00009af0: 3220 2d35 2e35 3936 3235 652d 3036 2c32  2 -5.59625e-06,2
+00009b00: 372e 3231 3637 3335 202d 352e 3539 3632  7.216735 -5.5962
+00009b10: 3565 2d30 362c 3236 2e32 3239 3733 3520  5e-06,26.229735 
+00009b20: 4320 3130 2e36 3636 3636 372c 3236 2e32  C 10.666667,26.2
+00009b30: 3239 3733 3520 3231 2e33 3333 3332 372c  29735 21.333327,
+00009b40: 3236 2e32 3239 3733 3520 3332 2c32 362e  26.229735 32,26.
+00009b50: 3232 3937 3335 2043 2033 322c 3237 2e32  229735 C 32,27.2
+00009b60: 3136 3733 3520 3332 2c32 382e 3230 3337  16735 32,28.2037
+00009b70: 3232 2033 322c 3239 2e31 3930 3730 3920  22 32,29.190709 
+00009b80: 4320 3231 2e33 3333 3332 372c 3239 2e31  C 21.333327,29.1
+00009b90: 3930 3730 3920 3130 2e36 3636 3636 372c  90709 10.666667,
+00009ba0: 3239 2e31 3930 3730 3920 2d35 2e35 3936  29.190709 -5.596
+00009bb0: 3235 652d 3036 2c32 392e 3139 3037 3039  25e-06,29.190709
+00009bc0: 207a 204d 2031 322e 3634 3837 352c 3137   z M 12.64875,17
+00009bd0: 2e35 3039 3631 2043 2031 322e 3634 3837  .50961 C 12.6487
+00009be0: 352c 3138 2e34 3332 3434 3620 3132 2e36  5,18.432446 12.6
+00009bf0: 3438 3735 2c31 392e 3335 3532 3833 2031  4875,19.355283 1
+00009c00: 322e 3634 3837 352c 3230 2e32 3738 3133  2.64875,20.27813
+00009c10: 3320 4320 382e 3433 3235 3032 332c 3230  3 C 8.4325023,20
+00009c20: 2e32 3738 3133 3320 342e 3231 3632 3431  .278133 4.216241
+00009c30: 382c 3230 2e32 3738 3133 3320 2d35 2e35  8,20.278133 -5.5
+00009c40: 3936 3235 652d 3036 2c32 302e 3237 3831  9625e-06,20.2781
+00009c50: 3333 2043 202d 352e 3539 3632 3565 2d30  33 C -5.59625e-0
+00009c60: 362c 3139 2e32 3836 3137 3620 2d35 2e35  6,19.286176 -5.5
+00009c70: 3936 3235 652d 3036 2c31 382e 3239 3432  9625e-06,18.2942
+00009c80: 3331 202d 352e 3539 3632 3565 2d30 362c  31 -5.59625e-06,
+00009c90: 3137 2e33 3032 3238 3620 4320 322e 3935  17.302286 C 2.95
+00009ca0: 3538 3137 2c31 372e 3330 3232 3836 2035  5817,17.302286 5
+00009cb0: 2e39 3131 3633 3936 2c31 372e 3330 3232  .9116396,17.3022
+00009cc0: 3836 2038 2e38 3637 3436 3233 2c31 372e  86 8.8674623,17.
+00009cd0: 3330 3232 3836 2043 2037 2e38 3333 3030  302286 C 7.83300
+00009ce0: 3139 2c31 362e 3235 3833 3139 2037 2e30  19,16.258319 7.0
+00009cf0: 3132 3132 3437 2c31 342e 3937 3034 3236  121247,14.970426
+00009d00: 2036 2e36 3632 3531 3731 2c31 332e 3533   6.6625171,13.53
+00009d10: 3336 3038 2043 2036 2e33 3635 3130 3634  3608 C 6.3651064
+00009d20: 2c31 322e 3333 3537 3732 2036 2e33 3939  ,12.335772 6.399
+00009d30: 3338 3239 2c31 312e 3037 3335 3338 2036  3829,11.073538 6
+00009d40: 2e36 3339 3338 3337 2c39 2e38 3639 3033  .6393837,9.86903
+00009d50: 3935 2043 2036 2e39 3435 3130 3935 2c38  95 C 6.9451095,8
+00009d60: 2e33 3535 3736 3136 2037 2e36 3932 3338  .3557616 7.69238
+00009d70: 3939 2c36 2e39 3438 3432 3933 2038 2e37  99,6.9484293 8.7
+00009d80: 3137 3938 3739 2c35 2e37 3938 3932 3033  179879,5.7989203
+00009d90: 2043 2039 2e38 3732 3436 3833 2c34 2e34   C 9.8724683,4.4
+00009da0: 3932 3237 3632 2031 312e 3334 3534 3437  922762 11.345447
+00009db0: 2c33 2e34 3339 3339 3537 2031 332e 3031  ,3.4393957 13.01
+00009dc0: 3636 3535 2c32 2e39 3037 3339 3237 2043  6655,2.9073927 C
+00009dd0: 2031 342e 3531 3939 3039 2c32 2e34 3235   14.519909,2.425
+00009de0: 3136 3133 2031 362e 3134 3030 3831 2c32  1613 16.140081,2
+00009df0: 2e33 3337 3738 3435 2031 372e 3639 3532  .3377845 17.6952
+00009e00: 3731 2c32 2e35 3839 3436 3631 2043 2031  71,2.5894661 C 1
+00009e10: 392e 3236 3634 3339 2c32 2e38 3435 3237  9.266439,2.84527
+00009e20: 3236 2032 302e 3735 3631 3133 2c33 2e35  26 20.756113,3.5
+00009e30: 3336 3735 3238 2032 312e 3938 3631 3332  367528 21.986132
+00009e40: 2c34 2e35 3432 3437 3732 2043 2032 332e  ,4.5424772 C 23.
+00009e50: 3238 3639 3938 2c35 2e36 3032 3234 3132  286998,5.6022412
+00009e60: 2032 342e 3338 3536 3834 2c36 2e39 3531   24.385684,6.951
+00009e70: 3531 3332 2032 342e 3938 3632 3031 2c38  5132 24.986201,8
+00009e80: 2e35 3238 3838 3837 2043 2032 352e 3436  .5288887 C 25.46
+00009e90: 3330 3632 2c39 2e37 3732 3635 3739 2032  3062,9.7726579 2
+00009ea0: 352e 3634 3031 3237 2c31 312e 3132 3633  5.640127,11.1263
+00009eb0: 3934 2032 352e 3533 3335 3537 2c31 322e  94 25.533557,12.
+00009ec0: 3435 3231 3636 2043 2032 352e 3431 3636  452166 C 25.4166
+00009ed0: 3738 2c31 332e 3832 3033 3434 2032 342e  78,13.820344 24.
+00009ee0: 3837 3839 3237 2c31 352e 3133 3539 3032  878927,15.135902
+00009ef0: 2032 342e 3036 3134 3532 2c31 362e 3233   24.061452,16.23
+00009f00: 3438 3538 2043 2032 332e 3738 3336 3033  4858 C 23.783603
+00009f10: 2c31 362e 3631 3235 3131 2032 332e 3437  ,16.612511 23.47
+00009f20: 3631 3138 2c31 362e 3936 3830 3536 2032  6118,16.968056 2
+00009f30: 332e 3134 3733 352c 3137 2e33 3032 3331  3.14735,17.30231
+00009f40: 3320 4320 3236 2e30 3938 3233 332c 3137  3 C 26.098233,17
+00009f50: 2e33 3032 3320 3239 2e30 3439 3131 362c  .3023 29.049116,
+00009f60: 3137 2e33 3032 3320 3332 2c31 372e 3330  17.3023 32,17.30
+00009f70: 3232 3836 2043 2033 322c 3138 2e32 3934  2286 C 32,18.294
+00009f80: 3233 3120 3332 2c31 392e 3238 3631 3736  231 32,19.286176
+00009f90: 2033 322c 3230 2e32 3738 3133 3320 4320   32,20.278133 C 
+00009fa0: 3237 2e37 3833 3733 392c 3230 2e32 3738  27.783739,20.278
+00009fb0: 3133 3320 3233 2e35 3637 3439 322c 3230  133 23.567492,20
+00009fc0: 2e32 3738 3133 3320 3139 2e33 3531 3234  .278133 19.35124
+00009fd0: 342c 3230 2e32 3738 3133 3320 4320 3139  4,20.278133 C 19
+00009fe0: 2e33 3531 3234 342c 3139 2e33 3535 3238  .351244,19.35528
+00009ff0: 3320 3139 2e33 3531 3234 342c 3138 2e34  3 19.351244,18.4
+0000a000: 3332 3434 3620 3139 2e33 3531 3234 342c  32446 19.351244,
+0000a010: 3137 2e35 3039 3631 2043 2032 302e 3437  17.50961 C 20.47
+0000a020: 3634 3739 2c31 362e 3738 3731 3939 2032  6479,16.787199 2
+0000a030: 312e 3436 3938 3436 2c31 352e 3830 3334  1.469846,15.8034
+0000a040: 3133 2032 322e 3032 3831 352c 3134 2e35  13 22.02815,14.5
+0000a050: 3735 3333 3720 4320 3232 2e35 3834 3630  75337 C 22.58460
+0000a060: 332c 3133 2e33 3632 3934 2032 322e 3730  3,13.36294 22.70
+0000a070: 3638 392c 3131 2e39 3734 3238 2032 322e  689,11.97428 22.
+0000a080: 3436 3932 3734 2c31 302e 3636 3839 3736  469274,10.668976
+0000a090: 2043 2032 322e 3233 3937 3532 2c39 2e34   C 22.239752,9.4
+0000a0a0: 3137 3630 3736 2032 312e 3537 3436 3138  176076 21.574618
+0000a0b0: 2c38 2e32 3731 3337 3736 2032 302e 3637  ,8.2713776 20.67
+0000a0c0: 3134 3531 2c37 2e33 3833 3237 3033 2043  1451,7.3832703 C
+0000a0d0: 2031 392e 3735 3135 3633 2c36 2e34 3532   19.751563,6.452
+0000a0e0: 3430 3520 3138 2e35 3631 3632 2c35 2e37  405 18.56162,5.7
+0000a0f0: 3731 3836 3820 3137 2e32 3635 3934 312c  71868 17.265941,
+0000a100: 352e 3534 3039 3636 3920 4320 3135 2e37  5.5409669 C 15.7
+0000a110: 3238 3234 312c 352e 3236 3434 3036 2031  28241,5.264406 1
+0000a120: 342e 3037 3533 3833 2c35 2e34 3836 3431  4.075383,5.48641
+0000a130: 3938 2031 322e 3732 3533 372c 362e 3239  98 12.72537,6.29
+0000a140: 3533 3631 2043 2031 312e 3832 3335 3333  5361 C 11.823533
+0000a150: 2c36 2e38 3335 3630 3037 2031 312e 3034  ,6.8356007 11.04
+0000a160: 3938 3734 2c37 2e35 3834 3835 3520 3130  9874,7.584855 10
+0000a170: 2e34 3538 3534 352c 382e 3435 3135 3730  .458545,8.451570
+0000a180: 3320 4320 392e 3735 3333 3939 372c 392e  3 C 9.7533997,9.
+0000a190: 3438 3734 3137 3920 392e 3430 3737 3431  4874179 9.407741
+0000a1a0: 312c 3130 2e37 3436 3738 3920 392e 3433  1,10.746789 9.43
+0000a1b0: 3133 3935 392c 3131 2e39 3935 3334 3720  13959,11.995347 
+0000a1c0: 4320 392e 3433 3636 3734 322c 3133 2e31  C 9.4366742,13.1
+0000a1d0: 3938 3837 2039 2e37 3639 3133 3034 2c31  9887 9.7691304,1
+0000a1e0: 342e 3430 3937 3434 2031 302e 3434 3730  4.409744 10.4470
+0000a1f0: 3234 2c31 352e 3431 3039 3739 2043 2031  24,15.410979 C 1
+0000a200: 312e 3031 3432 3135 2c31 362e 3236 3234  1.014215,16.2624
+0000a210: 3537 2031 312e 3739 3237 3632 2c31 362e  57 11.792762,16.
+0000a220: 3935 3635 3533 2031 322e 3634 3837 352c  956553 12.64875,
+0000a230: 3137 2e35 3039 3631 207a 2022 0a20 2020  17.50961 z ".   
+0000a240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a250: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+0000a260: 3a20 247a 6f64 6961 635f 636f 6c6f 725f  : $zodiac_color_
+0000a270: 3622 0a20 2020 2020 2020 2020 2020 2020  6".             
+0000a280: 2020 2020 2020 202f 3e0a 2020 2020 2020         />.      
+0000a290: 2020 2020 2020 2020 2020 3c2f 7379 6d62            </symb
+0000a2a0: 6f6c 3e0a 2020 2020 2020 2020 2020 2020  ol>.            
+0000a2b0: 2020 2020 3c73 796d 626f 6c20 6964 3d22      <symbol id="
+0000a2c0: 7363 6f72 7069 6f22 3e0a 2020 2020 2020  scorpio">.      
+0000a2d0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+0000a2e0: 6174 680a 2020 2020 2020 2020 2020 2020  ath.            
+0000a2f0: 2020 2020 2020 2020 2020 2020 643d 224d              d="M
+0000a300: 2032 2e30 3731 3737 352c 3235 2e31 3039   2.071775,25.109
+0000a310: 3339 3220 4320 322e 3037 3137 3534 322c  392 C 2.0717542,
+0000a320: 3139 2e32 3433 3339 3220 322e 3037 3138  19.243392 2.0718
+0000a330: 3136 362c 3133 2e33 3737 3339 3220 322e  166,13.377392 2.
+0000a340: 3037 3137 3433 322c 372e 3531 3133 3932  0717432,7.511392
+0000a350: 3120 4320 322e 3036 3932 3437 352c 362e  1 C 2.0692475,6.
+0000a360: 3334 3332 3236 3520 312e 3935 3833 3939  3432265 1.958399
+0000a370: 372c 352e 3137 3036 3932 3220 312e 3637  7,5.1706922 1.67
+0000a380: 3731 3632 312c 342e 3033 3532 3632 3620  71621,4.0352626 
+0000a390: 4320 312e 3433 3733 3139 362c 332e 3036  C 1.4373196,3.06
+0000a3a0: 3632 3537 3520 312e 3036 3835 3934 2c32  62575 1.068594,2
+0000a3b0: 2e31 3235 3134 3335 2030 2e35 3435 3338  .1251435 0.54538
+0000a3c0: 3034 382c 312e 3237 3336 3937 3120 4320  048,1.2736971 C 
+0000a3d0: 302e 3337 3935 3732 3038 2c31 2e30 3033  0.37957208,1.003
+0000a3e0: 3530 3632 2030 2e31 3938 3636 3435 382c  5062 0.19866458,
+0000a3f0: 302e 3734 3235 3934 2030 2e30 3033 3233  0.742594 0.00323
+0000a400: 3933 3736 342c 302e 3439 3330 3635 3120  93764,0.4930651 
+0000a410: 4320 302e 3838 3435 3038 3938 2c30 2e34  C 0.88450898,0.4
+0000a420: 3933 3036 3531 2031 2e37 3635 3737 3836  930651 1.7657786
+0000a430: 2c30 2e34 3933 3036 3531 2032 2e36 3437  ,0.4930651 2.647
+0000a440: 3034 3833 2c30 2e34 3933 3036 3531 2043  0483,0.4930651 C
+0000a450: 2033 2e32 3334 3035 3333 2c31 2e33 3839   3.2340533,1.389
+0000a460: 3439 3331 2033 2e36 3938 3333 3233 2c32  4931 3.6983323,2
+0000a470: 2e33 3635 3139 3031 2034 2e30 3335 3632  .3651901 4.03562
+0000a480: 3733 2c33 2e33 3832 3334 3234 2043 2034  73,3.3823424 C 4
+0000a490: 2e32 3437 3936 3133 2c34 2e30 3231 3033  .2479613,4.02103
+0000a4a0: 3733 2034 2e34 3131 3438 3133 2c34 2e36  73 4.4114813,4.6
+0000a4b0: 3735 3636 3620 342e 3533 3139 3836 332c  75666 4.5319863,
+0000a4c0: 352e 3333 3738 3333 2043 2035 2e30 3438  5.337833 C 5.048
+0000a4d0: 3531 3933 2c34 2e30 3630 3139 3738 2035  5193,4.0601978 5
+0000a4e0: 2e36 3834 3634 3933 2c32 2e38 3236 3833  .6846493,2.82683
+0000a4f0: 3839 2036 2e34 3736 3731 3733 2c31 2e36  89 6.4767173,1.6
+0000a500: 3937 3936 3520 4320 362e 3736 3939 3339  97965 C 6.769939
+0000a510: 332c 312e 3238 3031 3036 3920 372e 3038  3,1.2801069 7.08
+0000a520: 3433 3633 332c 302e 3837 3730 3638 3820  43633,0.8770688 
+0000a530: 372e 3432 3035 3932 332c 302e 3439 3330  7.4205923,0.4930
+0000a540: 3635 3120 4320 382e 3231 3231 3033 332c  651 C 8.2121033,
+0000a550: 302e 3333 3336 3137 3120 392e 3030 3336  0.3336171 9.0036
+0000a560: 3133 332c 302e 3137 3431 3639 2039 2e37  133,0.174169 9.7
+0000a570: 3935 3132 3433 2c30 2e30 3134 3732 3130  951243,0.0147210
+0000a580: 3033 2043 2031 302e 3332 3138 2c30 2e36  03 C 10.3218,0.6
+0000a590: 3239 3035 3834 2031 302e 3732 3739 372c  290584 10.72797,
+0000a5a0: 312e 3334 3030 3030 3520 3131 2e30 3337  1.3400005 11.037
+0000a5b0: 3731 342c 322e 3038 3631 3538 3520 4320  714,2.0861585 C 
+0000a5c0: 3131 2e34 3031 3335 382c 322e 3936 3239  11.401358,2.9629
+0000a5d0: 3235 3320 3131 2e36 3338 3033 392c 332e  253 11.638039,3.
+0000a5e0: 3838 3830 3031 3220 3131 2e37 3938 3132  8880012 11.79812
+0000a5f0: 352c 342e 3832 3233 3935 2043 2031 312e  5,4.822395 C 11.
+0000a600: 3834 3139 3732 2c35 2e30 3739 3137 3633  841972,5.0791763
+0000a610: 2031 312e 3837 3938 3837 2c35 2e33 3336   11.879887,5.336
+0000a620: 3936 3538 2031 312e 3931 3236 3139 2c35  9658 11.912619,5
+0000a630: 2e35 3935 3430 3239 2043 2031 322e 3334  .5954029 C 12.34
+0000a640: 3038 3231 2c34 2e33 3630 3233 3938 2031  0821,4.3602398 1
+0000a650: 322e 3935 3035 342c 332e 3139 3239 3637  2.95054,3.192967
+0000a660: 3220 3133 2e36 3734 3534 332c 322e 3130  2 13.674543,2.10
+0000a670: 3639 3030 3220 4320 3134 2e30 3436 3534  69002 C 14.04654
+0000a680: 2c31 2e35 3438 3733 3736 2031 342e 3434  ,1.5487376 14.44
+0000a690: 3839 3137 2c31 2e30 3131 3133 3736 2031  8917,1.0111376 1
+0000a6a0: 342e 3837 3436 3634 2c30 2e34 3933 3036  4.874664,0.49306
+0000a6b0: 3531 2043 2031 352e 3638 3234 3935 2c30  51 C 15.682495,0
+0000a6c0: 2e33 3333 3631 3731 2031 362e 3439 3033  .3336171 16.4903
+0000a6d0: 3235 2c30 2e31 3734 3136 3920 3137 2e32  25,0.174169 17.2
+0000a6e0: 3938 3135 362c 302e 3031 3437 3231 3030  98156,0.01472100
+0000a6f0: 3320 4320 3137 2e38 3831 3130 372c 302e  3 C 17.881107,0.
+0000a700: 3830 3238 3632 3920 3138 2e33 3436 3437  8028629 18.34647
+0000a710: 322c 312e 3637 3833 3335 3720 3138 2e36  2,1.6783357 18.6
+0000a720: 3730 3933 2c32 2e36 3034 3032 3734 2043  7093,2.6040274 C
+0000a730: 2031 392e 3032 3735 342c 332e 3631 3633   19.02754,3.6163
+0000a740: 3635 3520 3139 2e32 3136 3233 382c 342e  655 19.216238,4.
+0000a750: 3638 3431 3135 3620 3139 2e32 3636 3336  6841156 19.26636
+0000a760: 392c 352e 3735 3532 3838 3820 4320 3139  9,5.7552888 C 19
+0000a770: 2e32 3830 3034 2c36 2e30 3232 3135 3231  .28004,6.0221521
+0000a780: 2031 392e 3238 3134 3434 2c36 2e32 3839   19.281444,6.289
+0000a790: 3337 3733 2031 392e 3238 3130 3132 2c36  3773 19.281012,6
+0000a7a0: 2e35 3536 3532 3339 2043 2031 392e 3238  .5565239 C 19.28
+0000a7b0: 3130 3239 2c31 312e 3632 3730 3831 2031  1029,11.627081 1
+0000a7c0: 392e 3238 3039 3739 2c31 362e 3639 3736  9.280979,16.6976
+0000a7d0: 3339 2031 392e 3238 3130 3338 2c32 312e  39 19.281038,21.
+0000a7e0: 3736 3831 3937 2043 2031 392e 3238 3233  768197 C 19.2823
+0000a7f0: 3737 2c32 322e 3438 3537 3438 2031 392e  77,22.485748 19.
+0000a800: 3239 3236 3939 2c32 332e 3230 3336 3339  292699,23.203639
+0000a810: 2031 392e 3333 3430 3333 2c32 332e 3932   19.334033,23.92
+0000a820: 3031 3235 2043 2031 392e 3335 3432 3937  0125 C 19.354297
+0000a830: 2c32 342e 3234 3936 3333 2031 392e 3337  ,24.249633 19.37
+0000a840: 3838 3331 2c32 342e 3537 3934 3238 2031  8831,24.579428 1
+0000a850: 392e 3432 3838 3236 2c32 342e 3930 3539  9.428826,24.9059
+0000a860: 3433 2043 2031 392e 3434 3434 3931 2c32  43 C 19.444491,2
+0000a870: 352e 3031 3230 3535 2031 392e 3437 3232  5.012055 19.4722
+0000a880: 3738 2c32 352e 3131 3539 3134 2031 392e  78,25.115914 19.
+0000a890: 3530 3039 3437 2c32 352e 3231 3931 3220  500947,25.21912 
+0000a8a0: 4320 3139 2e35 3939 3838 342c 3235 2e35  C 19.599884,25.5
+0000a8b0: 3636 3932 3620 3139 2e37 3537 3631 352c  66926 19.757615,
+0000a8c0: 3235 2e38 3938 3431 3820 3139 2e39 3730  25.898418 19.970
+0000a8d0: 3532 2c32 362e 3139 3037 3631 2043 2032  52,26.190761 C 2
+0000a8e0: 302e 3035 3333 3831 2c32 362e 3330 3430  0.053381,26.3040
+0000a8f0: 3032 2032 302e 3134 3230 3639 2c32 362e  02 20.142069,26.
+0000a900: 3431 3333 3931 2032 302e 3234 3034 3237  413391 20.240427
+0000a910: 2c32 362e 3531 3335 3332 2043 2032 302e  ,26.513532 C 20.
+0000a920: 3533 3737 3331 2c32 362e 3831 3337 3338  537731,26.813738
+0000a930: 2032 302e 3930 3637 3931 2c32 372e 3033   20.906791,27.03
+0000a940: 3531 3939 2032 312e 3239 3735 3333 2c32  5199 21.297533,2
+0000a950: 372e 3139 3036 3520 4320 3231 2e37 3833  7.19065 C 21.783
+0000a960: 3732 372c 3237 2e33 3833 3939 3720 3232  727,27.383997 22
+0000a970: 2e33 3032 3132 312c 3237 2e34 3833 3638  .302121,27.48368
+0000a980: 3220 3232 2e38 3231 3234 362c 3237 2e35  2 22.821246,27.5
+0000a990: 3334 3236 3220 4320 3233 2e31 3436 3032  34262 C 23.14602
+0000a9a0: 322c 3237 2e35 3636 3030 3920 3233 2e34  2,27.566009 23.4
+0000a9b0: 3732 3437 352c 3237 2e35 3736 3030 3820  72475,27.576008 
+0000a9c0: 3233 2e37 3938 3637 322c 3237 2e35 3734  23.798672,27.574
+0000a9d0: 3730 3420 4320 3234 2e32 3731 3536 312c  704 C 24.271561,
+0000a9e0: 3237 2e35 3734 3730 3420 3234 2e37 3434  27.574704 24.744
+0000a9f0: 3435 322c 3237 2e35 3734 3730 3420 3235  452,27.574704 25
+0000aa00: 2e32 3137 3334 322c 3237 2e35 3734 3730  .217342,27.57470
+0000aa10: 3420 4320 3235 2e32 3137 3334 322c 3236  4 C 25.217342,26
+0000aa20: 2e37 3532 3933 3320 3235 2e32 3137 3334  .752933 25.21734
+0000aa30: 322c 3235 2e39 3331 3136 3320 3235 2e32  2,25.931163 25.2
+0000aa40: 3137 3334 322c 3235 2e31 3039 3339 3220  17342,25.109392 
+0000aa50: 4320 3236 2e35 3134 3736 372c 3236 2e32  C 26.514767,26.2
+0000aa60: 3832 3736 3620 3237 2e38 3132 3139 322c  82766 27.812192,
+0000aa70: 3237 2e34 3536 3134 2032 392e 3130 3936  27.45614 29.1096
+0000aa80: 3137 2c32 382e 3632 3935 3134 2043 2032  17,28.629514 C 2
+0000aa90: 372e 3831 3231 3932 2c32 392e 3735 3739  7.812192,29.7579
+0000aaa0: 3136 2032 362e 3531 3437 3637 2c33 302e  16 26.514767,30.
+0000aab0: 3838 3633 3137 2032 352e 3231 3733 3432  886317 25.217342
+0000aac0: 2c33 322e 3031 3437 3139 2043 2032 352e  ,32.014719 C 25.
+0000aad0: 3231 3733 3432 2c33 312e 3231 3734 3739  217342,31.217479
+0000aae0: 2032 352e 3231 3733 3432 2c33 302e 3432   25.217342,30.42
+0000aaf0: 3032 3339 2032 352e 3231 3733 3432 2c32  0239 25.217342,2
+0000ab00: 392e 3632 3239 3938 2043 2032 342e 3434  9.622998 C 24.44
+0000ab10: 3938 3339 2c32 392e 3632 3239 3331 2032  9839,29.622931 2
+0000ab20: 332e 3638 3233 3334 2c32 392e 3632 3331  3.682334,29.6231
+0000ab30: 3334 2032 322e 3931 3438 332c 3239 2e36  34 22.91483,29.6
+0000ab40: 3232 3839 3520 4320 3232 2e31 3735 3234  22895 C 22.17524
+0000ab50: 372c 3239 2e36 3139 3238 3220 3231 2e34  7,29.619282 21.4
+0000ab60: 3331 3838 392c 3239 2e35 3531 3335 2032  31889,29.55135 2
+0000ab70: 302e 3731 3435 3534 2c32 392e 3336 3437  0.714554,29.3647
+0000ab80: 3238 2043 2032 302e 3132 3437 3934 2c32  28 C 20.124794,2
+0000ab90: 392e 3231 3130 3833 2031 392e 3535 3234  9.211083 19.5524
+0000aba0: 3332 2c32 382e 3937 3230 3933 2031 392e  32,28.972093 19.
+0000abb0: 3035 3139 3037 2c32 382e 3632 3036 3736  051907,28.620676
+0000abc0: 2043 2031 382e 3638 3735 3531 2c32 382e   C 18.687551,28.
+0000abd0: 3336 3632 3537 2031 382e 3336 3535 3433  366257 18.365543
+0000abe0: 2c32 382e 3035 3137 3336 2031 382e 3130  ,28.051736 18.10
+0000abf0: 3039 3839 2c32 372e 3639 3433 3834 2043  0989,27.694384 C
+0000ac00: 2031 372e 3732 3533 3138 2c32 372e 3138   17.725318,27.18
+0000ac10: 3934 3636 2031 372e 3436 3031 352c 3236  9466 17.46015,26
+0000ac20: 2e36 3039 3435 2031 372e 3237 3237 3134  .60945 17.272714
+0000ac30: 2c32 362e 3031 3033 3438 2043 2031 372e  ,26.010348 C 17.
+0000ac40: 3034 3338 3236 2c32 352e 3237 3632 3636  043826,25.276266
+0000ac50: 2031 362e 3932 3534 3238 2c32 342e 3531   16.925428,24.51
+0000ac60: 3138 2031 362e 3836 3631 3835 2c32 332e  18 16.866185,23.
+0000ac70: 3734 3633 3634 2043 2031 362e 3833 3132  746364 C 16.8312
+0000ac80: 3131 2c32 332e 3239 3534 3134 2031 362e  11,23.295414 16.
+0000ac90: 3831 3934 3739 2c32 322e 3834 3320 3136  819479,22.843 16
+0000aca0: 2e38 3230 3830 312c 3232 2e33 3930 3738  .820801,22.39078
+0000acb0: 3520 4320 3136 2e38 3230 3739 2c31 372e  5 C 16.82079,17.
+0000acc0: 3437 3335 3033 2031 362e 3832 3038 3233  473503 16.820823
+0000acd0: 2c31 322e 3535 3632 3231 2031 362e 3832  ,12.556221 16.82
+0000ace0: 3037 3835 2c37 2e36 3338 3933 3832 2043  0785,7.6389382 C
+0000acf0: 2031 362e 3831 3839 3936 2c36 2e37 3632   16.818996,6.762
+0000ad00: 3231 3932 2031 362e 3737 3735 3933 2c35  2192 16.777593,5
+0000ad10: 2e38 3833 3635 3932 2031 362e 3635 3039  .8836592 16.6509
+0000ad20: 3737 2c35 2e30 3135 3435 3233 2043 2031  77,5.0154523 C 1
+0000ad30: 362e 3535 3934 372c 342e 3339 3833 3331  6.55947,4.398331
+0000ad40: 3920 3136 2e34 3235 3434 342c 332e 3738  9 16.425444,3.78
+0000ad50: 3434 3132 3720 3136 2e32 3033 3934 332c  44127 16.203943,
+0000ad60: 332e 3230 3031 3033 3120 4320 3136 2e30  3.2001031 C 16.0
+0000ad70: 3831 3939 362c 322e 3838 3032 3230 3820  81996,2.8802208 
+0000ad80: 3135 2e39 3332 3633 322c 322e 3536 3936  15.932632,2.5696
+0000ad90: 3230 3920 3135 2e37 3433 3639 342c 322e  209 15.743694,2.
+0000ada0: 3238 3337 3839 3420 4320 3134 2e38 3135  2837894 C 14.815
+0000adb0: 3331 352c 332e 3335 3534 3935 2031 342e  315,3.355495 14.
+0000adc0: 3033 3835 3839 2c34 2e35 3536 3331 3138  038589,4.5563118
+0000add0: 2031 332e 3432 3038 3936 2c35 2e38 3332   13.420896,5.832
+0000ade0: 3634 3639 2043 2031 322e 3734 3132 3339  6469 C 12.741239
+0000adf0: 2c37 2e32 3334 3834 3738 2031 322e 3235  ,7.2348478 12.25
+0000ae00: 3032 3234 2c38 2e37 3234 3636 3320 3131  0224,8.724663 11
+0000ae10: 2e39 3132 3631 392c 3130 2e32 3434 3938  .912619,10.24498
+0000ae20: 3820 4320 3131 2e39 3132 3631 392c 3135  8 C 11.912619,15
+0000ae30: 2e31 3939 3739 2031 312e 3931 3236 3139  .19979 11.912619
+0000ae40: 2c32 302e 3135 3435 3920 3131 2e39 3132  ,20.15459 11.912
+0000ae50: 3631 392c 3235 2e31 3039 3339 3220 4320  619,25.109392 C 
+0000ae60: 3131 2e30 3932 3534 392c 3235 2e31 3039  11.092549,25.109
+0000ae70: 3339 3220 3130 2e32 3732 3437 382c 3235  392 10.272478,25
+0000ae80: 2e31 3039 3339 3220 392e 3435 3234 3038  .109392 9.452408
+0000ae90: 332c 3235 2e31 3039 3339 3220 4320 392e  3,25.109392 C 9.
+0000aea0: 3435 3233 3937 332c 3139 2e35 3734 3331  4523973,19.57431
+0000aeb0: 3920 392e 3435 3234 3330 332c 3134 2e30  9 9.4524303,14.0
+0000aec0: 3339 3234 3620 392e 3435 3233 3932 332c  39246 9.4523923,
+0000aed0: 382e 3530 3431 3733 3320 4320 392e 3435  8.5041733 C 9.45
+0000aee0: 3036 3134 332c 372e 3530 3434 3038 3220  06143,7.5044082 
+0000aef0: 392e 3431 3330 3134 332c 362e 3530 3332  9.4130143,6.5032
+0000af00: 3131 3820 392e 3239 3536 3639 332c 352e  118 9.2956693,5.
+0000af10: 3530 3938 3239 3620 4320 392e 3231 3437  5098296 C 9.2147
+0000af20: 3532 332c 342e 3833 3832 3237 2039 2e30  523,4.838227 9.0
+0000af30: 3938 3630 3433 2c34 2e31 3638 3536 3835  986043,4.1685685
+0000af40: 2038 2e39 3033 3738 3833 2c33 2e35 3139   8.9037883,3.519
+0000af50: 3938 3136 2043 2038 2e37 3733 3433 3233  9816 C 8.7734323
+0000af60: 2c33 2e30 3930 3530 3833 2038 2e36 3038  ,3.0905083 8.608
+0000af70: 3033 3733 2c32 2e36 3638 3633 3720 382e  0373,2.668637 8.
+0000af80: 3337 3533 3031 332c 322e 3238 3337 3839  3753013,2.283789
+0000af90: 3420 4320 372e 3433 3335 3434 332c 332e  4 C 7.4335443,3.
+0000afa0: 3334 3433 3739 2036 2e36 3434 3034 3033  344379 6.6440403
+0000afb0: 2c34 2e35 3336 3932 3931 2036 2e30 3036  ,4.5369291 6.006
+0000afc0: 3438 3033 2c35 2e38 3033 3639 3336 2043  4803,5.8036936 C
+0000afd0: 2035 2e33 3831 3534 3833 2c37 2e30 3434   5.3815483,7.044
+0000afe0: 3134 3036 2034 2e38 3938 3730 3533 2c38  1406 4.8987053,8
+0000aff0: 2e33 3533 3839 3120 342e 3533 3139 3836  .353891 4.531986
+0000b000: 332c 392e 3639 3330 3532 3320 4320 342e  3,9.6930523 C 4.
+0000b010: 3533 3139 3836 332c 3134 2e38 3331 3833  5319863,14.83183
+0000b020: 3320 342e 3533 3139 3836 332c 3139 2e39  3 4.5319863,19.9
+0000b030: 3730 3631 3220 342e 3533 3139 3836 332c  70612 4.5319863,
+0000b040: 3235 2e31 3039 3339 3220 4320 332e 3731  25.109392 C 3.71
+0000b050: 3139 3135 332c 3235 2e31 3039 3339 3220  19153,25.109392 
+0000b060: 322e 3839 3138 3435 342c 3235 2e31 3039  2.8918454,25.109
+0000b070: 3339 3220 322e 3037 3137 3735 2c32 352e  392 2.071775,25.
+0000b080: 3130 3933 3932 207a 220a 2020 2020 2020  109392 z".      
+0000b090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0a0: 2020 7374 796c 653d 2266 696c 6c3a 2024    style="fill: $
+0000b0b0: 7a6f 6469 6163 5f63 6f6c 6f72 5f37 220a  zodiac_color_7".
+0000b0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0d0: 2020 2020 2f3e 0a20 2020 2020 2020 2020      />.         
+0000b0e0: 2020 2020 2020 203c 2f73 796d 626f 6c3e         </symbol>
+0000b0f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b100: 203c 7379 6d62 6f6c 2069 643d 2273 6167   <symbol id="sag
+0000b110: 6974 7461 7269 7573 223e 0a20 2020 2020  ittarius">.     
+0000b120: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000b130: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
+0000b140: 2020 2020 2020 2020 2020 2020 2064 3d22               d="
+0000b150: 4d20 3239 2e38 3932 3934 322c 322e 3039  M 29.892942,2.09
+0000b160: 3538 3730 3620 4c20 3332 2c31 372e 3131  58706 L 32,17.11
+0000b170: 3632 3736 204c 2032 382e 3939 3835 3739  6276 L 28.998579
+0000b180: 2c31 372e 3538 3730 3838 204c 2032 372e  ,17.587088 L 27.
+0000b190: 3435 3233 3933 2c36 2e36 3336 3932 3335  452393,6.6369235
+0000b1a0: 204c 2031 332e 3733 3337 3736 2c32 302e   L 13.733776,20.
+0000b1b0: 3431 3139 3537 204c 2032 302e 3139 3133  411957 L 20.1913
+0000b1c0: 3739 2c32 362e 3836 3636 3320 4c20 3138  79,26.86663 L 18
+0000b1d0: 2e30 3338 3834 352c 3239 2e30 3233 3235  .038845,29.02325
+0000b1e0: 3120 4c20 3131 2e35 3831 3234 322c 3232  1 L 11.581242,22
+0000b1f0: 2e35 3533 3339 204c 2032 2e30 3931 3930  .55339 L 2.09190
+0000b200: 312c 3331 2e39 3939 3939 3520 4c20 312e  1,31.999995 L 1.
+0000b210: 3565 2d30 362c 3239 2e39 3034 3132 3420  5e-06,29.904124 
+0000b220: 4c20 392e 3437 3431 3834 2c32 302e 3434  L 9.474184,20.44
+0000b230: 3233 3332 204c 2033 2e30 3331 3734 2c31  2332 L 3.03174,1
+0000b240: 332e 3937 3234 3720 4c20 352e 3135 3339  3.97247 L 5.1539
+0000b250: 3537 2c31 312e 3831 3538 3520 4c20 3131  57,11.81585 L 11
+0000b260: 2e36 3131 3536 2c31 382e 3238 3537 3131  .61156,18.285711
+0000b270: 204c 2032 352e 3336 3034 3933 2c34 2e35   L 25.360493,4.5
+0000b280: 3431 3035 3239 204c 2031 342e 3433 3130  410529 L 14.4310
+0000b290: 3736 2c33 2e30 3037 3131 3836 204c 2031  76,3.0071186 L 1
+0000b2a0: 342e 3930 3039 3936 2c2d 342e 3434 3038  4.900996,-4.4408
+0000b2b0: 3932 3165 2d31 3620 4c20 3239 2e38 3932  921e-16 L 29.892
+0000b2c0: 3934 322c 322e 3039 3538 3730 3620 7a20  942,2.0958706 z 
+0000b2d0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000b2e0: 2020 2020 2020 2020 2020 7374 796c 653d            style=
+0000b2f0: 2266 696c 6c3a 2024 7a6f 6469 6163 5f63  "fill: $zodiac_c
+0000b300: 6f6c 6f72 5f38 220a 2020 2020 2020 2020  olor_8".        
+0000b310: 2020 2020 2020 2020 2020 2020 2f3e 0a20              />. 
+0000b320: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000b330: 2f73 796d 626f 6c3e 0a20 2020 2020 2020  /symbol>.       
+0000b340: 2020 2020 2020 2020 203c 7379 6d62 6f6c           <symbol
+0000b350: 2069 643d 2263 6170 7269 636f 726e 223e   id="capricorn">
+0000b360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b370: 2020 2020 203c 7061 7468 0a20 2020 2020       <path.     
+0000b380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b390: 2020 2064 3d22 4d20 362e 3130 3933 3535     d="M 6.109355
+0000b3a0: 392c 3138 2e39 3034 3737 3420 4320 362e  9,18.904774 C 6.
+0000b3b0: 3130 3932 3339 322c 3138 2e35 3839 3535  1092392,18.58955
+0000b3c0: 2036 2e31 3039 3630 3432 2c31 382e 3237   6.1096042,18.27
+0000b3d0: 3433 3235 2036 2e31 3039 3134 3733 2c31  4325 6.1091473,1
+0000b3e0: 372e 3935 3931 3033 2043 2036 2e31 3033  7.959103 C 6.103
+0000b3f0: 3633 3839 2c31 372e 3134 3632 3334 2036  6389,17.146234 6
+0000b400: 2e30 3336 3435 3837 2c31 362e 3333 3530  .0364587,16.3350
+0000b410: 3635 2035 2e39 3436 3339 3638 2c31 352e  65 5.9463968,15.
+0000b420: 3532 3736 3131 2043 2035 2e38 3032 3031  527611 C 5.80201
+0000b430: 3933 2c31 342e 3235 3436 3432 2035 2e35  93,14.254642 5.5
+0000b440: 3936 3039 3433 2c31 322e 3938 3934 3635  960943,12.989465
+0000b450: 2035 2e33 3636 3533 3133 2c31 312e 3732   5.3665313,11.72
+0000b460: 3933 3338 2043 2035 2e32 3235 3836 3034  9338 C 5.2258604
+0000b470: 2c31 302e 3935 3639 3237 2035 2e30 3730  ,10.956927 5.070
+0000b480: 3434 2c31 302e 3138 3732 3220 342e 3930  44,10.18722 4.90
+0000b490: 3335 3537 2c39 2e34 3230 3035 3437 2043  3557,9.4200547 C
+0000b4a0: 2034 2e37 3231 3830 3237 2c38 2e35 3933   4.7218027,8.593
+0000b4b0: 3130 3532 2034 2e35 3236 3233 3839 2c37  1052 4.5262389,7
+0000b4c0: 2e37 3638 3439 3037 2034 2e32 3835 3333  .7684907 4.28533
+0000b4d0: 3336 2c36 2e39 3536 3532 3437 2043 2034  36,6.9565247 C 4
+0000b4e0: 2e31 3533 3230 3336 2c36 2e35 3136 3935  .1532036,6.51695
+0000b4f0: 3534 2034 2e30 3039 3931 3339 2c36 2e30  54 4.0099139,6.0
+0000b500: 3739 3533 2033 2e38 3235 3133 3334 2c35  7953 3.8251334,5
+0000b510: 2e36 3538 3838 3536 2043 2033 2e36 3538  .6588856 C 3.658
+0000b520: 3932 3334 2c35 2e32 3833 3631 3531 2033  9234,5.2836151 3
+0000b530: 2e34 3437 3231 3638 2c34 2e39 3236 3935  .4472168,4.92695
+0000b540: 3239 2033 2e31 3834 3334 3939 2c34 2e36  29 3.1843499,4.6
+0000b550: 3131 3038 3838 2043 2032 2e39 3030 3932  110888 C 2.90092
+0000b560: 3039 2c34 2e32 3730 3039 3239 2032 2e35  09,4.2700929 2.5
+0000b570: 3531 3435 3238 2c33 2e39 3832 3030 3131  514528,3.9820011
+0000b580: 2032 2e31 3534 3638 3531 2c33 2e37 3832   2.1546851,3.782
+0000b590: 3336 3431 2043 2031 2e37 3237 3238 3436  3641 C 1.7272846
+0000b5a0: 2c33 2e35 3635 3232 3631 2031 2e32 3531  ,3.5652261 1.251
+0000b5b0: 3938 3437 2c33 2e34 3532 3537 3137 2030  9847,3.4525717 0
+0000b5c0: 2e37 3734 3938 3437 382c 332e 3432 3230  .77498478,3.4220
+0000b5d0: 3438 3620 4320 302e 3538 3730 3136 3737  486 C 0.58701677
+0000b5e0: 2c33 2e34 3038 3937 3036 2030 2e33 3938  ,3.4089706 0.398
+0000b5f0: 3539 3637 352c 332e 3431 3239 3732 3820  59675,3.4129728 
+0000b600: 302e 3231 3033 3431 392c 332e 3431 3232  0.2103419,3.4122
+0000b610: 3935 2043 2030 2e31 3430 3230 3339 312c  95 C 0.14020391,
+0000b620: 332e 3431 3232 3935 2030 2e30 3730 3036  3.412295 0.07006
+0000b630: 3436 3833 2c33 2e34 3132 3239 3520 2d37  4683,3.412295 -7
+0000b640: 2e33 3330 3237 3765 2d30 352c 332e 3431  .330277e-05,3.41
+0000b650: 3232 3935 2043 202d 372e 3333 3032 3737  2295 C -7.330277
+0000b660: 652d 3035 2c32 2e37 3239 3533 3335 202d  e-05,2.7295335 -
+0000b670: 372e 3333 3032 3737 652d 3035 2c32 2e30  7.330277e-05,2.0
+0000b680: 3436 3737 3220 2d37 2e33 3330 3237 3765  46772 -7.330277e
+0000b690: 2d30 352c 312e 3336 3430 3130 3620 4320  -05,1.3640106 C 
+0000b6a0: 302e 3632 3736 3334 3534 2c31 2e33 3634  0.62763454,1.364
+0000b6b0: 3033 3137 2031 2e32 3535 3334 3234 2c31  0317 1.2553424,1
+0000b6c0: 2e33 3633 3936 3936 2031 2e38 3833 3035  .3639696 1.88305
+0000b6d0: 3032 2c31 2e33 3634 3034 3136 2043 2032  02,1.3640416 C 2
+0000b6e0: 2e34 3439 3434 342c 312e 3336 3538 3531  .449444,1.365851
+0000b6f0: 3520 332e 3032 3130 3939 2c31 2e34 3339  5 3.021099,1.439
+0000b700: 3131 3536 2033 2e35 3535 3031 312c 312e  1156 3.555011,1.
+0000b710: 3633 3433 3239 3520 4320 332e 3938 3336  6343295 C 3.9836
+0000b720: 3639 342c 312e 3739 3031 3037 3120 342e  694,1.7901071 4.
+0000b730: 3338 3332 3836 392c 322e 3032 3931 3538  3832869,2.029158
+0000b740: 2034 2e37 3134 3738 382c 322e 3334 3331   4.714788,2.3431
+0000b750: 3737 3420 4320 352e 3036 3932 3535 342c  774 C 5.0692554,
+0000b760: 322e 3637 3634 3830 3520 352e 3334 3335  2.6764805 5.3435
+0000b770: 3931 312c 332e 3038 3834 3836 3120 352e  911,3.0884861 5.
+0000b780: 3534 3432 3334 392c 332e 3533 3031 3633  5442349,3.530163
+0000b790: 3220 4320 352e 3834 3731 3630 382c 342e  2 C 5.8471608,4.
+0000b7a0: 3138 3435 3437 3920 362e 3038 3633 3437  1845479 6.086347
+0000b7b0: 342c 342e 3836 3634 3233 2036 2e32 3939  4,4.866423 6.299
+0000b7c0: 3537 3634 2c35 2e35 3534 3632 3035 2043  5764,5.5546205 C
+0000b7d0: 2036 2e36 3331 3632 3134 2c36 2e36 3335   6.6316214,6.635
+0000b7e0: 3035 3720 362e 3839 3630 3035 372c 372e  057 6.8960057,7.
+0000b7f0: 3733 3530 3636 3420 372e 3133 3138 3332  7350664 7.131832
+0000b800: 322c 382e 3834 3030 3838 3620 4320 372e  2,8.8400886 C 7.
+0000b810: 3332 3737 3433 372c 392e 3736 3231 3930  3277437,9.762190
+0000b820: 3220 372e 3530 3135 3335 392c 3130 2e36  2 7.5015359,10.6
+0000b830: 3838 3838 3320 372e 3636 3135 3438 332c  88883 7.6615483,
+0000b840: 3131 2e36 3137 3834 3720 4320 382e 3038  11.617847 C 8.08
+0000b850: 3137 3833 392c 392e 3734 3030 3139 3120  17839,9.7400191 
+0000b860: 382e 3635 3231 3732 332c 372e 3839 3130  8.6521723,7.8910
+0000b870: 3831 3220 392e 3433 3635 3035 312c 362e  812 9.4365051,6.
+0000b880: 3133 3139 3739 3720 4320 3130 2e31 3232  1319797 C 10.122
+0000b890: 3636 352c 342e 3539 3238 3133 3220 3130  665,4.5928132 10
+0000b8a0: 2e39 3736 3733 372c 332e 3132 3338 3233  .976737,3.123823
+0000b8b0: 3320 3132 2e30 3233 3337 322c 312e 3830  3 12.023372,1.80
+0000b8c0: 3038 3733 3620 4320 3132 2e31 3432 3434  08736 C 12.14244
+0000b8d0: 322c 312e 3635 3431 3739 3220 3132 2e32  2,1.6541792 12.2
+0000b8e0: 3538 3639 2c31 2e35 3030 3439 3333 2031  5869,1.5004933 1
+0000b8f0: 322e 3338 3536 3037 2c31 2e33 3632 3937  2.385607,1.36297
+0000b900: 3238 2043 2031 332e 3438 3036 3931 2c31  28 C 13.480691,1
+0000b910: 2e31 3532 3238 3338 2031 342e 3537 3537  .1522838 14.5757
+0000b920: 3737 2c30 2e39 3431 3539 3334 3920 3135  77,0.94159349 15
+0000b930: 2e36 3730 3836 312c 302e 3733 3039 3034  .670861,0.730904
+0000b940: 3437 2043 2031 362e 3031 3034 3932 2c31  47 C 16.010492,1
+0000b950: 2e35 3031 3536 3539 2031 362e 3237 3438  .5015659 16.2748
+0000b960: 3832 2c32 2e33 3033 3135 3839 2031 362e  82,2.3031589 16.
+0000b970: 3530 3437 3237 2c33 2e31 3132 3633 3937  504727,3.1126397
+0000b980: 2043 2031 362e 3834 3731 3233 2c34 2e33   C 16.847123,4.3
+0000b990: 3237 3339 3237 2031 372e 3130 3930 3231  273927 17.109021
+0000b9a0: 2c35 2e35 3633 3339 3731 2031 372e 3333  ,5.5633971 17.33
+0000b9b0: 3333 3032 2c36 2e38 3034 3930 3832 2043  3302,6.8049082 C
+0000b9c0: 2031 372e 3436 3536 3835 2c37 2e35 3339   17.465685,7.539
+0000b9d0: 3231 3435 2031 372e 3538 3235 3636 2c38  2145 17.582566,8
+0000b9e0: 2e32 3736 3233 3036 2031 372e 3639 3035  .2762306 17.6905
+0000b9f0: 342c 392e 3031 3434 3931 3920 4320 3137  4,9.0144919 C 17
+0000ba00: 2e38 3431 3031 312c 3130 2e30 3130 3535  .841011,10.01055
+0000ba10: 3420 3137 2e39 3931 3438 2c31 312e 3030  4 17.99148,11.00
+0000ba20: 3636 3135 2031 382e 3134 3139 3531 2c31  6615 18.141951,1
+0000ba30: 322e 3030 3236 3736 2043 2031 382e 3233  2.002676 C 18.23
+0000ba40: 3632 3236 2c31 322e 3638 3139 3832 2031  6226,12.681982 1
+0000ba50: 382e 3333 3034 3638 2c31 332e 3336 3133  8.330468,13.3613
+0000ba60: 3439 2031 382e 3431 3330 3531 2c31 342e  49 18.413051,14.
+0000ba70: 3034 3231 3935 2043 2031 382e 3434 3836  042195 C 18.4486
+0000ba80: 3639 2c31 342e 3334 3036 3234 2031 382e  69,14.340624 18.
+0000ba90: 3437 3930 3639 2c31 342e 3633 3936 3538  479069,14.639658
+0000baa0: 2031 382e 3531 3733 342c 3134 2e39 3337   18.51734,14.937
+0000bab0: 3737 3420 4320 3138 2e36 3138 3933 342c  774 C 18.618934,
+0000bac0: 3135 2e37 3435 3730 3820 3138 2e37 3431  15.745708 18.741
+0000bad0: 3936 372c 3136 2e35 3531 3739 3520 3138  967,16.551795 18
+0000bae0: 2e39 3136 3938 372c 3137 2e33 3437 3338  .916987,17.34738
+0000baf0: 3120 4320 3138 2e39 3936 3233 342c 3137  1 C 18.996234,17
+0000bb00: 2e37 3034 3532 3220 3139 2e30 3836 3134  .704522 19.08614
+0000bb10: 312c 3138 2e30 3539 3631 3320 3139 2e31  1,18.059613 19.1
+0000bb20: 3937 3434 322c 3138 2e34 3038 3232 2043  97442,18.40822 C
+0000bb30: 2031 392e 3635 3435 3634 2c31 372e 3533   19.654564,17.53
+0000bb40: 3430 3134 2032 302e 3230 3330 3731 2c31  4014 20.203071,1
+0000bb50: 362e 3730 3132 3735 2032 302e 3838 3037  6.701275 20.8807
+0000bb60: 3036 2c31 352e 3938 3133 3533 2043 2032  06,15.981353 C 2
+0000bb70: 312e 3434 3533 3737 2c31 352e 3338 3037  1.445377,15.3807
+0000bb80: 3731 2032 322e 3130 3433 3138 2c31 342e  71 22.104318,14.
+0000bb90: 3836 3335 3037 2032 322e 3834 3233 3136  863507 22.842316
+0000bba0: 2c31 342e 3439 3235 3836 2043 2032 332e  ,14.492586 C 23.
+0000bbb0: 3531 3834 3334 2c31 342e 3135 3035 3733  518434,14.150573
+0000bbc0: 2032 342e 3235 3730 3535 2c31 332e 3933   24.257055,13.93
+0000bbd0: 3630 3235 2032 352e 3030 3934 3534 2c31  6025 25.009454,1
+0000bbe0: 332e 3835 3033 3034 2043 2032 352e 3536  3.850304 C 25.56
+0000bbf0: 3639 3839 2c31 332e 3738 3733 3620 3236  6989,13.78736 26
+0000bc00: 2e31 3332 3231 382c 3133 2e37 3834 3836  .132218,13.78486
+0000bc10: 3920 3236 2e36 3839 3431 2c31 332e 3835  9 26.68941,13.85
+0000bc20: 3320 4320 3237 2e33 3730 3631 362c 3133  3 C 27.370616,13
+0000bc30: 2e39 3336 3037 3620 3238 2e30 3338 3837  .936076 28.03887
+0000bc40: 362c 3134 2e31 3333 3120 3238 2e36 3531  6,14.1331 28.651
+0000bc50: 3036 312c 3134 2e34 3434 3136 3920 4320  061,14.444169 C 
+0000bc60: 3239 2e32 3334 3138 372c 3134 2e37 3338  29.234187,14.738
+0000bc70: 3731 3320 3239 2e37 3633 3830 352c 3135  713 29.763805,15
+0000bc80: 2e31 3333 3738 3520 3330 2e32 3237 3530  .133785 30.22750
+0000bc90: 312c 3135 2e35 3932 3834 3720 4320 3330  1,15.592847 C 30
+0000bca0: 2e37 3137 3133 2c31 362e 3037 3135 3137  .71713,16.071517
+0000bcb0: 2033 312e 3133 3338 3035 2c31 362e 3632   31.133805,16.62
+0000bcc0: 3832 3132 2033 312e 3433 3139 342c 3137  8212 31.43194,17
+0000bcd0: 2e32 3435 3636 3220 4320 3331 2e37 3233  .245662 C 31.723
+0000bce0: 3539 2c31 372e 3834 3536 3833 2033 312e  59,17.845683 31.
+0000bcf0: 3930 3030 3738 2c31 382e 3439 3932 3332  900078,18.499232
+0000bd00: 2033 312e 3936 3634 3639 2c31 392e 3136   31.966469,19.16
+0000bd10: 3233 3938 2043 2033 322e 3031 3536 3132  2398 C 32.015612
+0000bd20: 2c31 392e 3635 3138 3631 2033 322e 3030  ,19.651861 32.00
+0000bd30: 3933 3235 2c32 302e 3134 3633 3538 2033  9325,20.146358 3
+0000bd40: 312e 3935 3736 3034 2c32 302e 3633 3533  1.957604,20.6353
+0000bd50: 3336 2043 2033 312e 3837 3934 322c 3231  36 C 31.87942,21
+0000bd60: 2e33 3636 3138 3720 3331 2e36 3831 3834  .366187 31.68184
+0000bd70: 382c 3232 2e30 3835 3834 3920 3331 2e33  8,22.085849 31.3
+0000bd80: 3539 3030 372c 3232 2e37 3436 3938 3820  59007,22.746988 
+0000bd90: 4320 3331 2e30 3335 3434 322c 3233 2e34  C 31.035442,23.4
+0000bda0: 3133 3539 3620 3330 2e35 3837 3136 352c  13596 30.587165,
+0000bdb0: 3234 2e30 3136 3731 3820 3330 2e30 3537  24.016718 30.057
+0000bdc0: 3635 2c32 342e 3533 3339 3937 2043 2032  65,24.533997 C 2
+0000bdd0: 392e 3535 3633 3834 2c32 352e 3032 3538  9.556384,25.0258
+0000bde0: 3933 2032 382e 3937 3639 3137 2c32 352e  93 28.976917,25.
+0000bdf0: 3434 3135 3231 2032 382e 3333 3739 3833  441521 28.337983
+0000be00: 2c32 352e 3733 3535 3535 2043 2032 372e  ,25.735555 C 27.
+0000be10: 3732 3034 3331 2c32 362e 3032 3136 3639  720431,26.021669
+0000be20: 2032 372e 3035 3133 3238 2c32 362e 3139   27.051328,26.19
+0000be30: 3133 3232 2032 362e 3337 3339 382c 3236  1322 26.37398,26
+0000be40: 2e32 3531 3237 3120 4320 3235 2e39 3033  .251271 C 25.903
+0000be50: 3534 392c 3236 2e32 3933 3334 3920 3235  549,26.293349 25
+0000be60: 2e34 3239 3530 392c 3236 2e32 3834 3235  .429509,26.28425
+0000be70: 3920 3234 2e39 3539 3335 312c 3236 2e32  9 24.959351,26.2
+0000be80: 3433 3233 3320 4320 3234 2e31 3032 3436  43233 C 24.10246
+0000be90: 342c 3236 2e31 3636 3832 3820 3233 2e32  4,26.166828 23.2
+0000bea0: 3537 3134 352c 3235 2e39 3535 3232 3720  57145,25.955227 
+0000beb0: 3232 2e34 3638 3435 312c 3235 2e36 3130  22.468451,25.610
+0000bec0: 3939 3120 4320 3231 2e36 3130 3633 322c  991 C 21.610632,
+0000bed0: 3235 2e32 3338 3632 3120 3230 2e38 3233  25.238621 20.823
+0000bee0: 3530 312c 3234 2e37 3133 3534 3720 3230  501,24.713547 20
+0000bef0: 2e31 3236 3036 352c 3234 2e30 3932 3630  .126065,24.09260
+0000bf00: 3320 4320 3139 2e39 3231 3034 342c 3233  3 C 19.921044,23
+0000bf10: 2e39 3130 3336 3920 3139 2e37 3233 3333  .910369 19.72333
+0000bf20: 362c 3233 2e37 3139 3935 3120 3139 2e35  6,23.719951 19.5
+0000bf30: 3332 3731 362c 3233 2e35 3232 3732 3420  32716,23.522724 
+0000bf40: 4320 3139 2e31 3131 3834 392c 3234 2e36  C 19.111849,24.6
+0000bf50: 3235 3639 3220 3138 2e36 3635 3233 372c  25692 18.665237,
+0000bf60: 3235 2e37 3139 3834 3420 3138 2e31 3537  25.719844 18.157
+0000bf70: 3134 2c32 362e 3738 3538 3520 4320 3137  14,26.78585 C 17
+0000bf80: 2e38 3430 3431 2c32 372e 3434 3634 3836  .84041,27.446486
+0000bf90: 2031 372e 3530 3134 3638 2c32 382e 3039   17.501468,28.09
+0000bfa0: 3830 3735 2031 372e 3130 3638 3131 2c32  8075 17.106811,2
+0000bfb0: 382e 3731 3539 3838 2043 2031 362e 3836  8.715988 C 16.86
+0000bfc0: 3532 3837 2c32 392e 3039 3038 3735 2031  5287,29.090875 1
+0000bfd0: 362e 3630 3339 3834 2c32 392e 3435 3538  6.603984,29.4558
+0000bfe0: 3433 2031 362e 3239 3431 3637 2c32 392e  43 16.294167,29.
+0000bff0: 3737 3738 3633 2043 2031 352e 3934 3836  777863 C 15.9486
+0000c000: 3435 2c33 302e 3133 3735 3332 2031 352e  45,30.137532 15.
+0000c010: 3532 3630 3936 2c33 302e 3431 3732 3820  526096,30.41728 
+0000c020: 3135 2e30 3734 3132 342c 3330 2e36 3235  15.074124,30.625
+0000c030: 3035 3320 4320 3134 2e35 3030 3039 312c  053 C 14.500091,
+0000c040: 3330 2e38 3839 3039 3520 3133 2e38 3832  30.889095 13.882
+0000c050: 3030 312c 3331 2e30 3435 3336 2031 332e  001,31.04536 13.
+0000c060: 3235 3931 3032 2c33 312e 3134 3130 3433  259102,31.141043
+0000c070: 2043 2031 322e 3631 3833 3234 2c33 312e   C 12.618324,31.
+0000c080: 3233 3838 3320 3131 2e39 3639 3235 352c  23883 11.969255,
+0000c090: 3331 2e32 3731 3436 3620 3131 2e33 3231  31.271466 11.321
+0000c0a0: 3536 362c 3331 2e32 3638 3936 3320 4320  566,31.268963 C 
+0000c0b0: 3130 2e35 3938 3236 312c 3331 2e32 3638  10.598261,31.268
+0000c0c0: 3936 3320 392e 3837 3439 3537 322c 3331  963 9.8749572,31
+0000c0d0: 2e32 3638 3936 3320 392e 3135 3136 3532  .268963 9.151652
+0000c0e0: 392c 3331 2e32 3638 3936 3320 4320 392e  9,31.268963 C 9.
+0000c0f0: 3135 3136 3532 392c 3330 2e35 3737 3932  1516529,30.57792
+0000c100: 3520 392e 3135 3136 3532 392c 3239 2e38  5 9.1516529,29.8
+0000c110: 3836 3838 3920 392e 3135 3136 3532 392c  86889 9.1516529,
+0000c120: 3239 2e31 3935 3835 3120 4320 392e 3532  29.195851 C 9.52
+0000c130: 3834 3139 372c 3239 2e31 3935 3734 3620  84197,29.195746 
+0000c140: 392e 3930 3531 3837 372c 3239 2e31 3936  9.9051877,29.196
+0000c150: 3037 2031 302e 3238 3139 3534 2c32 392e  07 10.281954,29.
+0000c160: 3139 3536 3732 2043 2031 302e 3938 3030  195672 C 10.9800
+0000c170: 3735 2c32 392e 3139 3135 3120 3131 2e36  75,29.19151 11.6
+0000c180: 3830 3734 362c 3239 2e31 3434 3131 3620  80746,29.144116 
+0000c190: 3132 2e33 3635 3839 362c 3239 2e30 3034  12.365896,29.004
+0000c1a0: 3833 3520 4320 3132 2e38 3739 3231 322c  835 C 12.879212,
+0000c1b0: 3238 2e38 3939 3138 3520 3133 2e33 3836  28.899185 13.386
+0000c1c0: 3431 352c 3238 2e37 3430 3535 2031 332e  415,28.74055 13.
+0000c1d0: 3834 3631 3737 2c32 382e 3438 3533 3932  846177,28.485392
+0000c1e0: 2043 2031 342e 3138 3033 3836 2c32 382e   C 14.180386,28.
+0000c1f0: 3330 3030 3937 2031 342e 3438 3634 3734  300097 14.486474
+0000c200: 2c32 382e 3035 3934 3520 3134 2e37 3238  ,28.05945 14.728
+0000c210: 3638 2c32 372e 3736 3236 3937 2043 2031  68,27.762697 C 1
+0000c220: 342e 3936 3835 3239 2c32 372e 3437 3031  4.968529,27.4701
+0000c230: 3720 3135 2e31 3636 3836 2c32 372e 3134  7 15.16686,27.14
+0000c240: 3633 3837 2031 352e 3335 3232 3038 2c32  6387 15.352208,2
+0000c250: 362e 3831 3734 3438 2043 2031 352e 3638  6.817448 C 15.68
+0000c260: 3436 3835 2c32 362e 3232 3037 3238 2031  4685,26.220728 1
+0000c270: 352e 3936 3933 3631 2c32 352e 3539 3837  5.969361,25.5987
+0000c280: 3937 2031 362e 3233 3739 3038 2c32 342e  97 16.237908,24.
+0000c290: 3937 3131 3639 2043 2031 362e 3639 3936  971169 C 16.6996
+0000c2a0: 3239 2c32 332e 3838 3437 3238 2031 372e  29,23.884728 17.
+0000c2b0: 3130 3735 3133 2c32 322e 3737 3632 3734  107513,22.776274
+0000c2c0: 2031 372e 3439 3439 3635 2c32 312e 3636   17.494965,21.66
+0000c2d0: 3134 3831 2043 2031 372e 3535 3831 312c  1481 C 17.55811,
+0000c2e0: 3231 2e34 3739 3335 3220 3137 2e36 3230  21.479352 17.620
+0000c2f0: 362c 3231 2e32 3936 3939 3520 3137 2e36  6,21.296995 17.6
+0000c300: 3832 3530 322c 3231 2e31 3134 3433 3820  82502,21.114438 
+0000c310: 4320 3137 2e33 3832 3230 362c 3230 2e35  C 17.382206,20.5
+0000c320: 3835 3939 3420 3137 2e31 3030 3433 352c  85994 17.100435,
+0000c330: 3230 2e30 3435 3733 3520 3136 2e38 3637  20.045735 16.867
+0000c340: 3435 2c31 392e 3438 3339 3237 2043 2031  45,19.483927 C 1
+0000c350: 362e 3732 3734 3438 2c31 392e 3134 3439  6.727448,19.1449
+0000c360: 3036 2031 362e 3630 3633 3136 2c31 382e  06 16.606316,18.
+0000c370: 3739 3639 3737 2031 362e 3532 3731 3337  796977 16.527137
+0000c380: 2c31 382e 3433 3834 3038 2043 2031 362e  ,18.438408 C 16.
+0000c390: 3433 3239 3631 2c31 382e 3031 3836 3239  432961,18.018629
+0000c3a0: 2031 362e 3336 3236 3035 2c31 372e 3539   16.362605,17.59
+0000c3b0: 3339 3631 2031 362e 3239 3439 3534 2c31  3961 16.294954,1
+0000c3c0: 372e 3136 3932 3436 2043 2031 362e 3134  7.169246 C 16.14
+0000c3d0: 3531 3632 2c31 362e 3231 3131 3032 2031  5162,16.211102 1
+0000c3e0: 362e 3032 3233 3138 2c31 352e 3234 3920  6.022318,15.249 
+0000c3f0: 3135 2e39 3033 3436 372c 3134 2e32 3836  15.903467,14.286
+0000c400: 3631 3220 4320 3135 2e36 3933 3437 382c  612 C 15.693478,
+0000c410: 3132 2e37 3035 3938 3620 3135 2e34 3833  12.705986 15.483
+0000c420: 3438 392c 3131 2e31 3235 3336 3120 3135  489,11.125361 15
+0000c430: 2e32 3733 352c 392e 3534 3437 3334 3420  .2735,9.5447344 
+0000c440: 4320 3135 2e31 3230 3637 362c 382e 3338  C 15.120676,8.38
+0000c450: 3030 3135 3320 3134 2e39 3434 3731 332c  00153 14.944713,
+0000c460: 372e 3231 3735 3633 2031 342e 3730 3935  7.217563 14.7095
+0000c470: 352c 362e 3036 3633 3436 3520 4320 3134  5,6.0663465 C 14
+0000c480: 2e35 3635 3539 342c 352e 3336 3935 3834  .565594,5.369584
+0000c490: 3720 3134 2e34 3031 3834 362c 342e 3637  7 14.401846,4.67
+0000c4a0: 3537 3035 3420 3134 2e31 3832 3832 2c33  57054 14.18282,3
+0000c4b0: 2e39 3938 3330 3932 2043 2031 342e 3037  .9983092 C 14.07
+0000c4c0: 3932 3334 2c33 2e36 3830 3838 3334 2031  9234,3.6808834 1
+0000c4d0: 332e 3936 3333 3434 2c33 2e33 3636 3833  3.963344,3.36683
+0000c4e0: 3535 2031 332e 3832 3036 3438 2c33 2e30  55 13.820648,3.0
+0000c4f0: 3634 3730 3733 2043 2031 332e 3033 3333  647073 C 13.0333
+0000c500: 3332 2c33 2e39 3937 3731 3231 2031 322e  32,3.9977121 12.
+0000c510: 3337 3036 3835 2c35 2e30 3330 3339 3735  370685,5.0303975
+0000c520: 2031 312e 3739 3534 3637 2c36 2e31 3035   11.795467,6.105
+0000c530: 3532 3039 2043 2031 312e 3133 3039 3032  5209 C 11.130902
+0000c540: 2c37 2e33 3439 3636 2031 302e 3538 3238  ,7.34966 10.5828
+0000c550: 332c 382e 3635 3331 3334 3820 3130 2e31  3,8.6531348 10.1
+0000c560: 3038 3630 362c 392e 3938 3035 3934 3520  08606,9.9805945 
+0000c570: 4320 392e 3538 3737 3835 352c 3131 2e34  C 9.5877855,11.4
+0000c580: 3237 3930 3620 392e 3135 3834 3635 322c  27906 9.1584652,
+0000c590: 3132 2e39 3131 3431 3320 382e 3838 3732  12.911413 8.8872
+0000c5a0: 3838 352c 3134 2e34 3236 3630 3320 4320  885,14.426603 C 
+0000c5b0: 382e 3639 3830 3536 342c 3135 2e34 3836  8.6980564,15.486
+0000c5c0: 3537 3520 382e 3538 3831 3032 382c 3136  575 8.5881028,16
+0000c5d0: 2e35 3632 3438 3720 382e 3539 3238 3633  .562487 8.592863
+0000c5e0: 372c 3137 2e36 3339 3835 3520 4320 382e  7,17.639855 C 8.
+0000c5f0: 3539 3238 3633 372c 3138 2e30 3631 3439  5928637,18.06149
+0000c600: 3520 382e 3539 3238 3633 372c 3138 2e34  5 8.5928637,18.4
+0000c610: 3833 3133 3420 382e 3539 3238 3633 372c  83134 8.5928637,
+0000c620: 3138 2e39 3034 3737 3420 4320 372e 3736  18.904774 C 7.76
+0000c630: 3530 3237 332c 3138 2e39 3034 3737 3420  50273,18.904774 
+0000c640: 362e 3933 3731 3932 322c 3138 2e39 3034  6.9371922,18.904
+0000c650: 3737 3420 362e 3130 3933 3535 392c 3138  774 6.1093559,18
+0000c660: 2e39 3034 3737 3420 7a20 4d20 3230 2e30  .904774 z M 20.0
+0000c670: 3931 3530 352c 3231 2e34 3132 3337 2043  91505,21.41237 C
+0000c680: 2032 302e 3730 3339 3839 2c32 322e 3039   20.703989,22.09
+0000c690: 3133 3033 2032 312e 3337 3632 3136 2c32  1303 21.376216,2
+0000c6a0: 322e 3732 3230 3220 3232 2e31 3330 3836  2.72202 22.13086
+0000c6b0: 372c 3233 2e32 3431 3230 3620 4320 3232  7,23.241206 C 22
+0000c6c0: 2e37 3630 3237 362c 3233 2e36 3733 3638  .760276,23.67368
+0000c6d0: 2032 332e 3435 3131 3536 2c32 342e 3032   23.451156,24.02
+0000c6e0: 3633 3035 2032 342e 3138 3938 3735 2c32  6305 24.189875,2
+0000c6f0: 342e 3232 3831 3739 2043 2032 342e 3835  4.228179 C 24.85
+0000c700: 3138 3136 2c32 342e 3431 3034 3036 2032  1816,24.410406 2
+0000c710: 352e 3535 3034 3239 2c32 342e 3436 3436  5.550429,24.4646
+0000c720: 3431 2032 362e 3233 3134 3037 2c32 342e  41 26.231407,24.
+0000c730: 3337 3235 3836 2043 2032 362e 3734 3335  372586 C 26.7435
+0000c740: 3132 2c32 342e 3330 3335 3633 2032 372e  12,24.303563 27.
+0000c750: 3234 3433 3532 2c32 342e 3134 3234 3439  244352,24.142449
+0000c760: 2032 372e 3639 3437 3337 2c32 332e 3838   27.694737,23.88
+0000c770: 3830 3837 2043 2032 382e 3037 3339 3939  8087 C 28.073999
+0000c780: 2c32 332e 3637 3533 3734 2032 382e 3431  ,23.675374 28.41
+0000c790: 3536 3539 2c32 332e 3339 3839 3435 2032  5659,23.398945 2
+0000c7a0: 382e 3731 3335 3137 2c32 332e 3038 3238  8.713517,23.0828
+0000c7b0: 3537 2043 2032 392e 3038 3334 3837 2c32  57 C 29.083487,2
+0000c7c0: 322e 3639 3632 3332 2032 392e 3338 3137  2.696232 29.3817
+0000c7d0: 3035 2c32 322e 3234 3035 3737 2032 392e  05,22.240577 29.
+0000c7e0: 3538 3235 3037 2c32 312e 3734 3433 3532  582507,21.744352
+0000c7f0: 2043 2032 392e 3830 3637 3536 2c32 312e   C 29.806756,21.
+0000c800: 3139 3435 3034 2032 392e 3931 3138 3934  194504 29.911894
+0000c810: 2c32 302e 3630 3037 3637 2032 392e 3932  ,20.600767 29.92
+0000c820: 3436 3736 2c32 302e 3030 3834 3820 4320  4676,20.00848 C 
+0000c830: 3239 2e39 3337 3535 332c 3139 2e35 3135  29.937553,19.515
+0000c840: 3135 3620 3239 2e38 3739 3034 362c 3139  156 29.879046,19
+0000c850: 2e30 3137 3932 3120 3239 2e37 3239 3435  .017921 29.72945
+0000c860: 352c 3138 2e35 3436 3735 3620 4320 3239  5,18.546756 C 29
+0000c870: 2e35 3736 3730 392c 3138 2e30 3630 3535  .576709,18.06055
+0000c880: 3820 3239 2e33 3236 3834 312c 3137 2e36  8 29.326841,17.6
+0000c890: 3036 3339 3520 3239 2e30 3035 3334 2c31  06395 29.00534,1
+0000c8a0: 372e 3231 3134 3120 4320 3238 2e36 3531  7.21141 C 28.651
+0000c8b0: 3434 332c 3136 2e37 3736 3531 3320 3238  443,16.776513 28
+0000c8c0: 2e32 3139 3438 392c 3136 2e34 3030 3533  .219489,16.40053
+0000c8d0: 3720 3237 2e37 3232 3732 372c 3136 2e31  7 27.722727,16.1
+0000c8e0: 3337 3336 3420 4320 3237 2e32 3835 3137  37364 C 27.28517
+0000c8f0: 352c 3135 2e39 3033 3934 3620 3236 2e38  5,15.903946 26.8
+0000c900: 3030 3536 332c 3135 2e37 3632 3430 3220  00563,15.762402 
+0000c910: 3236 2e33 3037 3630 322c 3135 2e37 3132  26.307602,15.712
+0000c920: 3532 3820 4320 3235 2e36 3338 3532 392c  528 C 25.638529,
+0000c930: 3135 2e36 3434 3838 3920 3234 2e39 3532  15.644889 24.952
+0000c940: 3537 362c 3135 2e37 3235 3134 3620 3234  576,15.725146 24
+0000c950: 2e33 3232 3838 372c 3135 2e39 3633 3839  .322887,15.96389
+0000c960: 3620 4320 3233 2e37 3331 3738 312c 3136  6 C 23.731781,16
+0000c970: 2e31 3835 3738 3120 3233 2e31 3936 3933  .185781 23.19693
+0000c980: 362c 3136 2e35 3431 3432 2032 322e 3733  6,16.54142 22.73
+0000c990: 3533 382c 3136 2e39 3639 3534 3220 4320  538,16.969542 C 
+0000c9a0: 3232 2e31 3730 3139 372c 3137 2e34 3933  22.170197,17.493
+0000c9b0: 3337 3620 3231 2e37 3037 3137 362c 3138  376 21.707176,18
+0000c9c0: 2e31 3138 3236 3320 3231 2e33 3132 3536  .118263 21.31256
+0000c9d0: 2c31 382e 3737 3737 2043 2032 302e 3831  ,18.7777 C 20.81
+0000c9e0: 3539 3833 2c31 392e 3631 3038 3337 2032  5983,19.610837 2
+0000c9f0: 302e 3432 3433 3731 2c32 302e 3530 3236  0.424371,20.5026
+0000ca00: 3837 2032 302e 3039 3135 3035 2c32 312e  87 20.091505,21.
+0000ca10: 3431 3233 3720 7a20 220a 2020 2020 2020  41237 z ".      
+0000ca20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca30: 2020 7374 796c 653d 2266 696c 6c3a 2024    style="fill: $
+0000ca40: 7a6f 6469 6163 5f63 6f6c 6f72 5f39 220a  zodiac_color_9".
+0000ca50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca60: 2020 2020 2f3e 0a20 2020 2020 2020 2020      />.         
+0000ca70: 2020 2020 2020 203c 2f73 796d 626f 6c3e         </symbol>
+0000ca80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ca90: 203c 7379 6d62 6f6c 2069 643d 2261 7175   <symbol id="aqu
+0000caa0: 6172 6975 7322 3e0a 2020 2020 2020 2020  arius">.        
+0000cab0: 2020 2020 2020 2020 2020 2020 3c70 6174              <pat
+0000cac0: 680a 2020 2020 2020 2020 2020 2020 2020  h.              
+0000cad0: 2020 2020 2020 2020 2020 643d 224d 2032            d="M 2
+0000cae0: 652d 3036 2c32 342e 3730 3136 3537 204c  e-06,24.701657 L
+0000caf0: 2039 2e36 3737 3131 2c31 382e 3332 3236   9.67711,18.3226
+0000cb00: 3834 204c 2031 312e 3739 3735 3932 2c32  84 L 11.797592,2
+0000cb10: 332e 3236 3431 3432 204c 2031 392e 3238  3.264142 L 19.28
+0000cb20: 3939 3631 2c31 382e 3332 3236 3834 204c  9961,18.322684 L
+0000cb30: 2032 312e 3338 3437 342c 3233 2e32 3634   21.38474,23.264
+0000cb40: 3134 3220 4c20 3238 2e38 3839 3936 2c31  142 L 28.88996,1
+0000cb50: 382e 3332 3236 3834 204c 2033 312e 3938  8.322684 L 31.98
+0000cb60: 3731 3439 2c32 352e 3630 3031 3034 204c  7149,25.600104 L
+0000cb70: 2032 392e 3938 3233 332c 3236 2e34 3835   29.98233,26.485
+0000cb80: 3731 3620 4c20 3237 2e39 3133 3235 332c  716 L 27.913253,
+0000cb90: 3231 2e35 3434 3235 3820 4c20 3230 2e33  21.544258 L 20.3
+0000cba0: 3832 3333 2c32 362e 3438 3537 3136 204c  8233,26.485716 L
+0000cbb0: 2031 382e 3238 3735 3531 2c32 312e 3534   18.287551,21.54
+0000cbc0: 3432 3538 204c 2031 302e 3832 3038 3835  4258 L 10.820885
+0000cbd0: 2c32 362e 3438 3537 3136 204c 2038 2e37  ,26.485716 L 8.7
+0000cbe0: 3133 3235 342c 3231 2e35 3434 3235 3820  13254,21.544258 
+0000cbf0: 4c20 312e 3138 3233 3331 2c32 362e 3438  L 1.182331,26.48
+0000cc00: 3537 3136 204c 2032 652d 3036 2c32 342e  5716 L 2e-06,24.
+0000cc10: 3730 3136 3537 207a 204d 2030 2e30 3132  701657 z M 0.012
+0000cc20: 3835 332c 3131 2e33 3931 3830 3820 4c20  853,11.391808 L 
+0000cc30: 392e 3638 3939 3631 2c35 204c 2031 312e  9.689961,5 L 11.
+0000cc40: 3831 3034 3433 2c39 2e39 3431 3435 3820  810443,9.941458 
+0000cc50: 4c20 3139 2e33 3135 3636 342c 3520 4c20  L 19.315664,5 L 
+0000cc60: 3231 2e34 3130 3434 332c 392e 3934 3134  21.410443,9.9414
+0000cc70: 3538 204c 2032 382e 3930 3238 3132 2c35  58 L 28.902812,5
+0000cc80: 204c 2033 322c 3132 2e32 3737 3432 204c   L 32,12.27742 L
+0000cc90: 2032 392e 3939 3531 3831 2c31 332e 3136   29.995181,13.16
+0000cca0: 3330 3332 204c 2032 372e 3932 3631 3035  3032 L 27.926105
+0000ccb0: 2c38 2e32 3231 3537 3420 4c20 3230 2e33  ,8.221574 L 20.3
+0000ccc0: 3832 3333 2c31 332e 3136 3330 3332 204c  8233,13.163032 L
+0000ccd0: 2031 382e 3238 3735 3531 2c38 2e32 3231   18.287551,8.221
+0000cce0: 3537 3420 4c20 3130 2e38 3230 3838 352c  574 L 10.820885,
+0000ccf0: 3133 2e31 3633 3033 3220 4c20 382e 3733  13.163032 L 8.73
+0000cd00: 3839 3537 2c38 2e32 3231 3537 3420 4c20  8957,8.221574 L 
+0000cd10: 312e 3230 3830 3334 2c31 332e 3136 3330  1.208034,13.1630
+0000cd20: 3332 204c 2030 2e30 3132 3835 332c 3131  32 L 0.012853,11
+0000cd30: 2e33 3931 3830 3820 7a20 220a 2020 2020  .391808 z ".    
+0000cd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd50: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+0000cd60: 2024 7a6f 6469 6163 5f63 6f6c 6f72 5f31   $zodiac_color_1
+0000cd70: 3022 0a20 2020 2020 2020 2020 2020 2020  0".             
+0000cd80: 2020 2020 2020 202f 3e0a 2020 2020 2020         />.      
+0000cd90: 2020 2020 2020 2020 2020 3c2f 7379 6d62            </symb
+0000cda0: 6f6c 3e0a 2020 2020 2020 2020 2020 2020  ol>.            
+0000cdb0: 2020 2020 3c73 796d 626f 6c20 6964 3d22      <symbol id="
+0000cdc0: 7069 7363 6573 223e 0a20 2020 2020 2020  pisces">.       
+0000cdd0: 2020 2020 2020 2020 2020 2020 203c 7061               <pa
+0000cde0: 7468 0a20 2020 2020 2020 2020 2020 2020  th.             
+0000cdf0: 2020 2020 2020 2020 2020 2064 3d22 4d20             d="M 
+0000ce00: 3133 2e32 3838 3132 322c 3136 2e34 3933  13.288122,16.493
+0000ce10: 3539 3320 4320 3133 2e32 3838 3334 312c  593 C 13.288341,
+0000ce20: 3138 2e30 3633 3639 3920 3133 2e30 3534  18.063699 13.054
+0000ce30: 3638 2c31 392e 3632 3833 3632 2031 322e  68,19.628362 12.
+0000ce40: 3635 3939 3235 2c32 312e 3134 3631 3536  659925,21.146156
+0000ce50: 2043 2031 322e 3335 3737 3034 2c32 322e   C 12.357704,22.
+0000ce60: 3330 3732 3434 2031 312e 3936 3332 3133  307244 11.963213
+0000ce70: 2c32 332e 3434 3334 3039 2031 312e 3530  ,23.443409 11.50
+0000ce80: 3033 372c 3234 2e35 3439 3935 3820 4320  037,24.549958 C 
+0000ce90: 3130 2e36 3836 3138 382c 3236 2e34 3738  10.686188,26.478
+0000cea0: 3439 3320 392e 3636 3631 3735 372c 3238  493 9.6661757,28
+0000ceb0: 2e33 3232 3035 3320 382e 3434 3037 3139  .322053 8.440719
+0000cec0: 372c 3330 2e30 3230 3037 3620 4320 372e  7,30.020076 C 7.
+0000ced0: 3934 3730 3935 372c 3330 2e37 3034 3635  9470957,30.70465
+0000cee0: 2037 2e34 3230 3738 3037 2c33 312e 3336   7.4207807,31.36
+0000cef0: 3536 3439 2036 2e38 3634 3039 3237 2c33  5649 6.8640927,3
+0000cf00: 3220 4320 352e 3735 3534 3534 2c33 3220  2 C 5.755454,32 
+0000cf10: 342e 3634 3638 3135 332c 3332 2033 2e35  4.6468153,32 3.5
+0000cf20: 3338 3137 3636 2c33 3220 4320 352e 3035  381766,32 C 5.05
+0000cf30: 3232 3033 342c 3330 2e34 3034 3035 3520  22034,30.404055 
+0000cf40: 362e 3430 3937 3932 372c 3238 2e36 3530  6.4097927,28.650
+0000cf50: 3837 3220 372e 3439 3831 3530 372c 3236  872 7.4981507,26
+0000cf60: 2e37 3336 3333 3520 4320 382e 3433 3235  .736335 C 8.4325
+0000cf70: 3034 372c 3235 2e30 3935 3232 3620 392e  047,25.095226 9.
+0000cf80: 3136 3330 3030 372c 3233 2e33 3334 3839  1630007,23.33489
+0000cf90: 3620 392e 3632 3835 3737 372c 3231 2e35  6 9.6285777,21.5
+0000cfa0: 3033 3537 3920 4320 3130 2e30 3436 3233  03579 C 10.04623
+0000cfb0: 382c 3139 2e38 3638 3633 3620 3130 2e32  8,19.868636 10.2
+0000cfc0: 3531 3637 352c 3138 2e31 3830 3731 3120  51675,18.180711 
+0000cfd0: 3130 2e32 3530 3735 362c 3136 2e34 3933  10.250756,16.493
+0000cfe0: 3539 3320 4320 382e 3038 3931 3633 372c  593 C 8.0891637,
+0000cff0: 3136 2e34 3933 3539 3320 352e 3932 3735  16.493593 5.9275
+0000d000: 3730 372c 3136 2e34 3933 3539 3320 332e  707,16.493593 3.
+0000d010: 3736 3539 3739 312c 3136 2e34 3933 3539  7659791,16.49359
+0000d020: 3320 4320 332e 3736 3539 3739 312c 3135  3 C 3.7659791,15
+0000d030: 2e37 3334 3231 3920 332e 3736 3539 3739  .734219 3.765979
+0000d040: 312c 3134 2e39 3734 3834 3620 332e 3736  1,14.974846 3.76
+0000d050: 3539 3739 312c 3134 2e32 3135 3437 3220  59791,14.215472 
+0000d060: 4320 352e 3932 3735 3730 372c 3134 2e32  C 5.9275707,14.2
+0000d070: 3135 3437 3220 382e 3038 3931 3633 372c  15472 8.0891637,
+0000d080: 3134 2e32 3135 3437 3220 3130 2e32 3530  14.215472 10.250
+0000d090: 3735 362c 3134 2e32 3135 3437 3220 4320  756,14.215472 C 
+0000d0a0: 3130 2e31 3535 3936 322c 3132 2e34 3937  10.155962,12.497
+0000d0b0: 3939 3120 392e 3831 3234 3836 372c 3130  991 9.8124867,10
+0000d0c0: 2e37 3936 3437 2039 2e32 3534 3634 3837  .79647 9.2546487
+0000d0d0: 2c39 2e31 3730 3034 3320 4320 382e 3631  ,9.170043 C 8.61
+0000d0e0: 3035 3436 372c 372e 3238 3634 2037 2e36  05467,7.2864 7.6
+0000d0f0: 3836 3231 3037 2c35 2e35 3035 3639 3120  862107,5.505691 
+0000d100: 362e 3538 3330 3636 372c 332e 3835 3132  6.5830667,3.8512
+0000d110: 3534 2043 2035 2e36 3734 3330 3331 2c32  54 C 5.6743031,2
+0000d120: 2e34 3837 3930 3820 342e 3634 3531 3235  .487908 4.645125
+0000d130: 2c31 2e32 3037 3039 3839 2033 2e35 3338  ,1.2070989 3.538
+0000d140: 3137 3636 2c33 652d 3037 2043 2034 2e35  1766,3e-07 C 4.5
+0000d150: 3836 3036 382c 3365 2d30 3720 352e 3633  86068,3e-07 5.63
+0000d160: 3339 3539 332c 3365 2d30 3720 362e 3638  39593,3e-07 6.68
+0000d170: 3138 3530 372c 3365 2d30 3720 4320 382e  18507,3e-07 C 8.
+0000d180: 3135 3939 3339 372c 312e 3537 3538 3437  1599397,1.575847
+0000d190: 3620 392e 3436 3235 3835 372c 332e 3332  6 9.4625857,3.32
+0000d1a0: 3136 3520 3130 2e35 3034 3333 352c 352e  165 10.504335,5.
+0000d1b0: 3231 3632 3331 2043 2031 312e 3436 3030  216231 C 11.4600
+0000d1c0: 3434 2c36 2e39 3530 3234 3820 3132 2e31  44,6.950248 12.1
+0000d1d0: 3933 3035 362c 382e 3830 3639 3139 2031  93056,8.806919 1
+0000d1e0: 322e 3637 3637 3238 2c31 302e 3732 3639  2.676728,10.7269
+0000d1f0: 3835 2043 2031 322e 3936 3631 3731 2c31  85 C 12.966171,1
+0000d200: 312e 3837 3236 3435 2031 332e 3136 3833  1.872645 13.1683
+0000d210: 3634 2c31 332e 3034 3030 3036 2031 332e  64,13.040006 13.
+0000d220: 3238 3831 3232 2c31 342e 3231 3534 3732  288122,14.215472
+0000d230: 2043 2031 352e 3338 3339 3035 2c31 342e   C 15.383905,14.
+0000d240: 3231 3534 3732 2031 372e 3437 3936 3838  215472 17.479688
+0000d250: 2c31 342e 3231 3534 3732 2031 392e 3537  ,14.215472 19.57
+0000d260: 3534 372c 3134 2e32 3135 3437 3220 4320  547,14.215472 C 
+0000d270: 3139 2e37 3836 3838 322c 3132 2e31 3837  19.786882,12.187
+0000d280: 3735 3820 3230 2e32 3435 3838 342c 3130  758 20.245884,10
+0000d290: 2e31 3834 3133 2032 302e 3936 3332 3439  .18413 20.963249
+0000d2a0: 2c38 2e32 3735 3034 3120 4320 3231 2e36  ,8.275041 C 21.6
+0000d2b0: 3730 3432 392c 362e 3338 3637 3732 2032  70429,6.386772 2
+0000d2c0: 322e 3632 3836 3535 2c34 2e35 3934 3834  2.628655,4.59484
+0000d2d0: 3920 3233 2e37 3836 3533 332c 322e 3934  9 23.786533,2.94
+0000d2e0: 3439 3136 2043 2032 342e 3531 3334 3135  4916 C 24.513415
+0000d2f0: 2c31 2e39 3037 3832 3239 2032 352e 3331  ,1.9078229 25.31
+0000d300: 3735 3838 2c30 2e39 3235 3536 3837 2032  7588,0.9255687 2
+0000d310: 362e 3138 3137 3432 2c33 652d 3037 2043  6.181742,3e-07 C
+0000d320: 2032 372e 3232 3936 3333 2c33 652d 3037   27.229633,3e-07
+0000d330: 2032 382e 3237 3735 3235 2c33 652d 3037   28.277525,3e-07
+0000d340: 2032 392e 3332 3534 3136 2c33 652d 3037   29.325416,3e-07
+0000d350: 2043 2032 372e 3835 3436 3138 2c31 2e36   C 27.854618,1.6
+0000d360: 3034 3038 3837 2032 362e 3531 3838 3439  040887 26.518849
+0000d370: 2c33 2e33 3430 3034 3720 3235 2e34 3234  ,3.340047 25.424
+0000d380: 3932 312c 352e 3232 3430 3136 2043 2032  921,5.224016 C 2
+0000d390: 342e 3437 3034 3538 2c36 2e38 3637 3033  4.470458,6.86703
+0000d3a0: 2032 332e 3730 3439 3935 2c38 2e36 3235   23.704995,8.625
+0000d3b0: 3439 3820 3233 2e32 3135 3137 352c 3130  498 23.215175,10
+0000d3c0: 2e34 3633 3336 3420 4320 3232 2e38 3837  .463364 C 22.887
+0000d3d0: 3534 372c 3131 2e36 3839 3233 3220 3232  547,11.689232 22
+0000d3e0: 2e36 3833 3238 312c 3132 2e39 3438 3339  .683281,12.94839
+0000d3f0: 3220 3232 2e36 3132 3833 372c 3134 2e32  2 22.612837,14.2
+0000d400: 3135 3437 3220 4320 3234 2e37 3734 3432  15472 C 24.77442
+0000d410: 382c 3134 2e32 3135 3437 3220 3236 2e39  8,14.215472 26.9
+0000d420: 3336 3032 322c 3134 2e32 3135 3437 3220  36022,14.215472 
+0000d430: 3239 2e30 3937 3631 342c 3134 2e32 3135  29.097614,14.215
+0000d440: 3437 3220 4320 3239 2e30 3937 3631 342c  472 C 29.097614,
+0000d450: 3134 2e39 3734 3834 3620 3239 2e30 3937  14.974846 29.097
+0000d460: 3631 342c 3135 2e37 3334 3231 3920 3239  614,15.734219 29
+0000d470: 2e30 3937 3631 342c 3136 2e34 3933 3539  .097614,16.49359
+0000d480: 3320 4320 3236 2e39 3336 3032 322c 3136  3 C 26.936022,16
+0000d490: 2e34 3933 3539 3320 3234 2e37 3734 3432  .493593 24.77442
+0000d4a0: 382c 3136 2e34 3933 3539 3320 3232 2e36  8,16.493593 22.6
+0000d4b0: 3132 3833 372c 3136 2e34 3933 3539 3320  12837,16.493593 
+0000d4c0: 4320 3232 2e36 3131 3539 312c 3138 2e33  C 22.611591,18.3
+0000d4d0: 3130 3031 3320 3232 2e38 3530 3534 342c  10013 22.850544,
+0000d4e0: 3230 2e31 3237 3334 3720 3233 2e33 3334  20.127347 23.334
+0000d4f0: 3435 342c 3231 2e38 3738 3532 3420 4320  454,21.878524 C 
+0000d500: 3233 2e38 3337 3332 322c 3233 2e37 3037  23.837322,23.707
+0000d510: 3239 3320 3234 2e36 3034 3336 392c 3235  293 24.604369,25
+0000d520: 2e34 3539 3439 3420 3235 2e35 3730 3639  .459494 25.57069
+0000d530: 342c 3237 2e30 3930 3130 3520 4320 3236  4,27.090105 C 26
+0000d540: 2e36 3232 3732 372c 3238 2e38 3637 3736  .622727,28.86776
+0000d550: 3520 3237 2e39 3035 3038 332c 3330 2e35  5 27.905083,30.5
+0000d560: 3032 3732 3320 3239 2e33 3235 3431 362c  02723 29.325416,
+0000d570: 3332 2043 2032 382e 3232 3138 3339 2c33  32 C 28.221839,3
+0000d580: 3220 3237 2e31 3138 3236 342c 3332 2032  2 27.118264,32 2
+0000d590: 362e 3031 3436 3837 2c33 3220 4320 3234  6.014687,32 C 24
+0000d5a0: 2e36 3934 3433 352c 3330 2e35 3038 3337  .694435,30.50837
+0000d5b0: 3720 3233 2e35 3439 3139 372c 3238 2e38  7 23.549197,28.8
+0000d5c0: 3633 3331 3520 3232 2e35 3937 3331 332c  63315 22.597313,
+0000d5d0: 3237 2e31 3133 3832 3120 4320 3232 2e31  27.113821 C 22.1
+0000d5e0: 3034 3238 2c32 362e 3230 3737 3938 2032  0428,26.207798 2
+0000d5f0: 312e 3636 3035 3333 2c32 352e 3237 3439  1.660533,25.2749
+0000d600: 3120 3231 2e32 3638 3236 352c 3234 2e33  1 21.268265,24.3
+0000d610: 3230 3933 3520 4320 3230 2e36 3233 3633  20935 C 20.62363
+0000d620: 342c 3232 2e37 3337 3733 3920 3230 2e31  4,22.737739 20.1
+0000d630: 3135 3631 332c 3231 2e30 3933 3732 3920  15613,21.093729 
+0000d640: 3139 2e38 3238 3932 322c 3139 2e34 3036  19.828922,19.406
+0000d650: 3732 3120 4320 3139 2e36 3635 3538 352c  721 C 19.665585,
+0000d660: 3138 2e34 3434 3736 3820 3139 2e35 3735  18.444768 19.575
+0000d670: 3430 322c 3137 2e34 3639 3630 3320 3139  402,17.469603 19
+0000d680: 2e35 3735 3437 2c31 362e 3439 3335 3933  .57547,16.493593
+0000d690: 2043 2031 372e 3437 3936 3838 2c31 362e   C 17.479688,16.
+0000d6a0: 3439 3335 3933 2031 352e 3338 3339 3035  493593 15.383905
+0000d6b0: 2c31 362e 3439 3335 3933 2031 332e 3238  ,16.493593 13.28
+0000d6c0: 3831 3232 2c31 362e 3439 3335 3933 207a  8122,16.493593 z
+0000d6d0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+0000d6e0: 2020 2020 2020 2020 2020 2073 7479 6c65             style
+0000d6f0: 3d22 6669 6c6c 3a20 247a 6f64 6961 635f  ="fill: $zodiac_
+0000d700: 636f 6c6f 725f 3131 220a 2020 2020 2020  color_11".      
+0000d710: 2020 2020 2020 2020 2020 2020 2020 2f3e                />
+0000d720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d730: 203c 2f73 796d 626f 6c3e 0a20 2020 2020   </symbol>.     
+0000d740: 2020 2020 2020 2020 2020 203c 212d 2d20             <!-- 
+0000d750: 4173 7065 6374 7320 3132 7831 3220 2d2d  Aspects 12x12 --
+0000d760: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000d770: 2020 3c73 796d 626f 6c20 6964 3d22 6f72    <symbol id="or
+0000d780: 6230 223e 0a20 2020 2020 2020 2020 2020  b0">.           
+0000d790: 2020 2020 2020 2020 203c 7061 7468 0a20           <path. 
+0000d7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7b0: 2020 2020 2020 2064 3d22 4d20 362e 3036         d="M 6.06
+0000d7c0: 3937 3533 392c 372e 3332 3334 3835 3220  97539,7.3234852 
+0000d7d0: 4320 362e 3036 3937 3533 392c 382e 3733  C 6.0697539,8.73
+0000d7e0: 3534 3838 3220 342e 3931 3733 3635 312c  54882 4.9173651,
+0000d7f0: 392e 3838 3031 3434 3220 332e 3439 3538  9.8801442 3.4958
+0000d800: 3231 342c 392e 3838 3031 3434 3220 4320  214,9.8801442 C 
+0000d810: 322e 3037 3432 3737 352c 392e 3838 3031  2.0742775,9.8801
+0000d820: 3434 3220 302e 3932 3138 3838 3537 2c38  442 0.92188857,8
+0000d830: 2e37 3335 3438 3832 2030 2e39 3231 3838  .7354882 0.92188
+0000d840: 3835 372c 372e 3332 3334 3835 3220 4320  857,7.3234852 C 
+0000d850: 302e 3932 3138 3838 3537 2c35 2e39 3131  0.92188857,5.911
+0000d860: 3438 3232 2032 2e30 3734 3237 3735 2c34  4822 2.0742775,4
+0000d870: 2e37 3636 3832 3732 2033 2e34 3935 3832  .7668272 3.49582
+0000d880: 3134 2c34 2e37 3636 3832 3732 2043 2034  14,4.7668272 C 4
+0000d890: 2e39 3137 3336 3531 2c34 2e37 3636 3832  .9173651,4.76682
+0000d8a0: 3732 2036 2e30 3639 3735 3339 2c35 2e39  72 6.0697539,5.9
+0000d8b0: 3131 3438 3232 2036 2e30 3639 3735 3339  114822 6.0697539
+0000d8c0: 2c37 2e33 3233 3438 3532 204c 2036 2e30  ,7.3234852 L 6.0
+0000d8d0: 3639 3735 3339 2c37 2e33 3233 3438 3532  697539,7.3234852
+0000d8e0: 207a 204d 2035 2e36 3235 3236 3039 2c35   z M 5.6252609,5
+0000d8f0: 2e32 3131 3332 3032 2043 2031 302e 3037  .2113202 C 10.07
+0000d900: 3031 392c 302e 3736 3633 3930 3138 2031  019,0.76639018 1
+0000d910: 302e 3037 3031 392c 302e 3736 3633 3930  0.07019,0.766390
+0000d920: 3138 2031 302e 3037 3031 392c 302e 3736  18 10.07019,0.76
+0000d930: 3633 3930 3138 220a 2020 2020 2020 2020  639018".        
+0000d940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d950: 7374 796c 653d 220a 2020 2020 2020 2020  style=".        
+0000d960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d970: 2020 2020 6f70 6163 6974 793a 2031 3b0a      opacity: 1;.
+0000d980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d990: 2020 2020 2020 2020 2020 2020 6669 6c6c              fill
+0000d9a0: 3a20 6e6f 6e65 3b0a 2020 2020 2020 2020  : none;.        
 0000d9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9c0: 2020 2020 2020 2020 6f70 6163 6974 793a          opacity:
-0000d9d0: 2031 3b0a 2020 2020 2020 2020 2020 2020   1;.            
+0000d9c0: 2020 2020 6669 6c6c 2d6f 7061 6369 7479      fill-opacity
+0000d9d0: 3a20 313b 0a20 2020 2020 2020 2020 2020  : 1;.           
 0000d9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9f0: 6669 6c6c 3a20 6e6f 6e65 3b0a 2020 2020  fill: none;.    
-0000da00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da10: 2020 2020 2020 2020 6669 6c6c 2d6f 7061          fill-opa
-0000da20: 6369 7479 3a20 313b 0a20 2020 2020 2020  city: 1;.       
-0000da30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da40: 2020 2020 2066 696c 6c2d 7275 6c65 3a20       fill-rule: 
-0000da50: 6e6f 6e7a 6572 6f3b 0a20 2020 2020 2020  nonzero;.       
-0000da60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da70: 2020 2020 2073 7472 6f6b 653a 2024 6f72       stroke: $or
-0000da80: 625f 636f 6c6f 725f 303b 0a20 2020 2020  b_color_0;.     
-0000da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000daa0: 2020 2020 2020 2073 7472 6f6b 652d 7769         stroke-wi
-0000dab0: 6474 683a 2031 2e34 3736 3333 3036 343b  dth: 1.47633064;
-0000dac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dad0: 2020 2020 2020 2020 2020 2020 2073 7472               str
-0000dae0: 6f6b 652d 6c69 6e65 6361 703a 2062 7574  oke-linecap: but
-0000daf0: 743b 0a20 2020 2020 2020 2020 2020 2020  t;.             
-0000db00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000db10: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a20  troke-linejoin: 
-0000db20: 6d69 7465 723b 0a20 2020 2020 2020 2020  miter;.         
-0000db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db40: 2020 2073 7472 6f6b 652d 6d69 7465 726c     stroke-miterl
-0000db50: 696d 6974 3a20 343b 0a20 2020 2020 2020  imit: 4;.       
-0000db60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db70: 2020 2020 2073 7472 6f6b 652d 6461 7368       stroke-dash
-0000db80: 6172 7261 793a 206e 6f6e 653b 0a20 2020  array: none;.   
-0000db90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dba0: 2020 2020 2020 2020 2073 7472 6f6b 652d           stroke-
-0000dbb0: 6f70 6163 6974 793a 2031 3b0a 2020 2020  opacity: 1;.    
-0000dbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbd0: 2020 2020 220a 2020 2020 2020 2020 2020      ".          
-0000dbe0: 2020 2020 2020 2020 2020 2f3e 0a20 2020            />.   
-0000dbf0: 2020 2020 2020 2020 2020 2020 203c 2f73               </s
-0000dc00: 796d 626f 6c3e 0a20 2020 2020 2020 2020  ymbol>.         
-0000dc10: 2020 2020 2020 203c 7379 6d62 6f6c 2069         <symbol i
-0000dc20: 643d 226f 7262 3330 223e 0a20 2020 2020  d="orb30">.     
-0000dc30: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000dc40: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
-0000dc50: 2020 2020 2020 2020 2020 2020 2064 3d22               d="
-0000dc60: 4d20 302e 3831 3637 3531 3534 2c36 2e31  M 0.81675154,6.1
-0000dc70: 3334 3233 3938 2043 2031 312e 3334 3636  342398 C 11.3466
-0000dc80: 3135 2c36 2e31 3632 3031 3438 2031 312e  15,6.1620148 11.
-0000dc90: 3334 3636 3135 2c36 2e31 3632 3031 3438  346615,6.1620148
-0000dca0: 2031 312e 3334 3636 3135 2c36 2e31 3632   11.346615,6.162
-0000dcb0: 3031 3438 204d 2031 302e 3631 3231 3834  0148 M 10.612184
-0000dcc0: 2c30 2e37 3539 3935 3737 3320 4320 352e  ,0.75995773 C 5.
-0000dcd0: 3731 3338 3437 392c 352e 3930 3332 3130  7138479,5.903210
-0000dce0: 3820 352e 3731 3338 3437 392c 352e 3930  8 5.7138479,5.90
-0000dcf0: 3332 3130 3820 352e 3731 3338 3437 392c  32108 5.7138479,
-0000dd00: 352e 3930 3332 3130 3820 4d20 312e 3330  5.9032108 M 1.30
-0000dd10: 3533 3435 312c 302e 3735 3939 3537 3733  53451,0.75995773
-0000dd20: 2043 2035 2e38 3830 3731 3839 2c36 2e31   C 5.8807189,6.1
-0000dd30: 3932 3531 3638 2035 2e38 3830 3731 3839  925168 5.8807189
-0000dd40: 2c36 2e31 3932 3531 3638 2035 2e38 3830  ,6.1925168 5.880
-0000dd50: 3731 3839 2c36 2e31 3932 3531 3638 220a  7189,6.1925168".
+0000d9f0: 2066 696c 6c2d 7275 6c65 3a20 6e6f 6e7a   fill-rule: nonz
+0000da00: 6572 6f3b 0a20 2020 2020 2020 2020 2020  ero;.           
+0000da10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da20: 2073 7472 6f6b 653a 2024 6f72 625f 636f   stroke: $orb_co
+0000da30: 6c6f 725f 303b 0a20 2020 2020 2020 2020  lor_0;.         
+0000da40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da50: 2020 2073 7472 6f6b 652d 7769 6474 683a     stroke-width:
+0000da60: 2031 2e34 3736 3333 3036 343b 0a20 2020   1.47633064;.   
+0000da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da80: 2020 2020 2020 2020 2073 7472 6f6b 652d           stroke-
+0000da90: 6c69 6e65 6361 703a 2062 7574 743b 0a20  linecap: butt;. 
+0000daa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dab0: 2020 2020 2020 2020 2020 2073 7472 6f6b             strok
+0000dac0: 652d 6c69 6e65 6a6f 696e 3a20 6d69 7465  e-linejoin: mite
+0000dad0: 723b 0a20 2020 2020 2020 2020 2020 2020  r;.             
+0000dae0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000daf0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+0000db00: 3a20 343b 0a20 2020 2020 2020 2020 2020  : 4;.           
+0000db10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db20: 2073 7472 6f6b 652d 6461 7368 6172 7261   stroke-dasharra
+0000db30: 793a 206e 6f6e 653b 0a20 2020 2020 2020  y: none;.       
+0000db40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db50: 2020 2020 2073 7472 6f6b 652d 6f70 6163       stroke-opac
+0000db60: 6974 793a 2031 3b0a 2020 2020 2020 2020  ity: 1;.        
+0000db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db80: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000db90: 2020 2020 2020 2f3e 0a20 2020 2020 2020        />.       
+0000dba0: 2020 2020 2020 2020 203c 2f73 796d 626f           </symbo
+0000dbb0: 6c3e 0a20 2020 2020 2020 2020 2020 2020  l>.             
+0000dbc0: 2020 203c 7379 6d62 6f6c 2069 643d 226f     <symbol id="o
+0000dbd0: 7262 3330 223e 0a20 2020 2020 2020 2020  rb30">.         
+0000dbe0: 2020 2020 2020 2020 2020 203c 7061 7468             <path
+0000dbf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dc00: 2020 2020 2020 2020 2064 3d22 4d20 302e           d="M 0.
+0000dc10: 3831 3637 3531 3534 2c36 2e31 3334 3233  81675154,6.13423
+0000dc20: 3938 2043 2031 312e 3334 3636 3135 2c36  98 C 11.346615,6
+0000dc30: 2e31 3632 3031 3438 2031 312e 3334 3636  .1620148 11.3466
+0000dc40: 3135 2c36 2e31 3632 3031 3438 2031 312e  15,6.1620148 11.
+0000dc50: 3334 3636 3135 2c36 2e31 3632 3031 3438  346615,6.1620148
+0000dc60: 204d 2031 302e 3631 3231 3834 2c30 2e37   M 10.612184,0.7
+0000dc70: 3539 3935 3737 3320 4320 352e 3731 3338  5995773 C 5.7138
+0000dc80: 3437 392c 352e 3930 3332 3130 3820 352e  479,5.9032108 5.
+0000dc90: 3731 3338 3437 392c 352e 3930 3332 3130  7138479,5.903210
+0000dca0: 3820 352e 3731 3338 3437 392c 352e 3930  8 5.7138479,5.90
+0000dcb0: 3332 3130 3820 4d20 312e 3330 3533 3435  32108 M 1.305345
+0000dcc0: 312c 302e 3735 3939 3537 3733 2043 2035  1,0.75995773 C 5
+0000dcd0: 2e38 3830 3731 3839 2c36 2e31 3932 3531  .8807189,6.19251
+0000dce0: 3638 2035 2e38 3830 3731 3839 2c36 2e31  68 5.8807189,6.1
+0000dcf0: 3932 3531 3638 2035 2e38 3830 3731 3839  925168 5.8807189
+0000dd00: 2c36 2e31 3932 3531 3638 220a 2020 2020  ,6.1925168".    
+0000dd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd20: 2020 2020 7374 796c 653d 220a 2020 2020      style=".    
+0000dd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd40: 2020 2020 2020 2020 6f70 6163 6974 793a          opacity:
+0000dd50: 2031 3b0a 2020 2020 2020 2020 2020 2020   1;.            
 0000dd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd70: 2020 2020 2020 2020 7374 796c 653d 220a          style=".
+0000dd70: 6669 6c6c 3a20 6e6f 6e65 3b0a 2020 2020  fill: none;.    
 0000dd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd90: 2020 2020 2020 2020 2020 2020 6f70 6163              opac
-0000dda0: 6974 793a 2031 3b0a 2020 2020 2020 2020  ity: 1;.        
+0000dd90: 2020 2020 2020 2020 6669 6c6c 2d6f 7061          fill-opa
+0000dda0: 6369 7479 3a20 313b 0a20 2020 2020 2020  city: 1;.       
 0000ddb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddc0: 2020 2020 6669 6c6c 3a20 6e6f 6e65 3b0a      fill: none;.
-0000ddd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dde0: 2020 2020 2020 2020 2020 2020 6669 6c6c              fill
-0000ddf0: 2d6f 7061 6369 7479 3a20 313b 0a20 2020  -opacity: 1;.   
-0000de00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de10: 2020 2020 2020 2020 2066 696c 6c2d 7275           fill-ru
-0000de20: 6c65 3a20 6e6f 6e7a 6572 6f3b 0a20 2020  le: nonzero;.   
-0000de30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de40: 2020 2020 2020 2020 2073 7472 6f6b 653a           stroke:
-0000de50: 2024 6f72 625f 636f 6c6f 725f 3330 3b0a   $orb_color_30;.
-0000de60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de70: 2020 2020 2020 2020 2020 2020 7374 726f              stro
-0000de80: 6b65 2d77 6964 7468 3a20 312e 3437 3633  ke-width: 1.4763
-0000de90: 3330 3634 3b0a 2020 2020 2020 2020 2020  3064;.          
-0000dea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000deb0: 2020 7374 726f 6b65 2d6c 696e 6563 6170    stroke-linecap
-0000dec0: 3a20 6275 7474 3b0a 2020 2020 2020 2020  : butt;.        
-0000ded0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dee0: 2020 2020 7374 726f 6b65 2d6c 696e 656a      stroke-linej
-0000def0: 6f69 6e3a 206d 6974 6572 3b0a 2020 2020  oin: miter;.    
-0000df00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df10: 2020 2020 2020 2020 7374 726f 6b65 2d6d          stroke-m
-0000df20: 6974 6572 6c69 6d69 743a 2034 3b0a 2020  iterlimit: 4;.  
-0000df30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df40: 2020 2020 2020 2020 2020 7374 726f 6b65            stroke
-0000df50: 2d64 6173 6861 7272 6179 3a20 6e6f 6e65  -dasharray: none
-0000df60: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-0000df70: 2020 2020 2020 2020 2020 2020 2020 7374                st
-0000df80: 726f 6b65 2d6f 7061 6369 7479 3a20 313b  roke-opacity: 1;
-0000df90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dfa0: 2020 2020 2020 2020 2022 0a20 2020 2020           ".     
-0000dfb0: 2020 2020 2020 2020 2020 2020 2020 202f                 /
-0000dfc0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000dfd0: 2020 3c2f 7379 6d62 6f6c 3e0a 2020 2020    </symbol>.    
-0000dfe0: 2020 2020 2020 2020 2020 2020 3c73 796d              <sym
-0000dff0: 626f 6c20 6964 3d22 6f72 6234 3522 3e0a  bol id="orb45">.
-0000e000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e010: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
-0000e020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e030: 2020 643d 224d 2039 2e38 3130 3031 3738    d="M 9.8100178
-0000e040: 2c39 2e35 3932 3139 3636 2043 2036 2e39  ,9.5921966 C 6.9
-0000e050: 3634 3036 3538 2c39 2e35 3932 3139 3536  640658,9.5921956
-0000e060: 2034 2e31 3138 3131 3235 2c39 2e35 3932   4.1181125,9.592
-0000e070: 3139 3636 2031 2e32 3732 3136 2c39 2e35  1966 1.27216,9.5
-0000e080: 3932 3139 3636 2043 2032 2e36 3935 3133  921966 C 2.69513
-0000e090: 3632 2c36 2e37 3436 3234 3431 2034 2e31  62,6.7462441 4.1
-0000e0a0: 3138 3131 3235 2c33 2e39 3030 3239 3035  181125,3.9002905
-0000e0b0: 2035 2e35 3431 3038 3838 2c31 2e30 3534   5.5410888,1.054
-0000e0c0: 3333 3739 220a 2020 2020 2020 2020 2020  3379".          
-0000e0d0: 2020 2020 2020 2020 2020 2020 2020 7374                st
-0000e0e0: 796c 653d 220a 2020 2020 2020 2020 2020  yle=".          
-0000e0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e100: 2020 6f70 6163 6974 793a 2031 3b0a 2020    opacity: 1;.  
+0000ddc0: 2020 2020 2066 696c 6c2d 7275 6c65 3a20       fill-rule: 
+0000ddd0: 6e6f 6e7a 6572 6f3b 0a20 2020 2020 2020  nonzero;.       
+0000dde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ddf0: 2020 2020 2073 7472 6f6b 653a 2024 6f72       stroke: $or
+0000de00: 625f 636f 6c6f 725f 3330 3b0a 2020 2020  b_color_30;.    
+0000de10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de20: 2020 2020 2020 2020 7374 726f 6b65 2d77          stroke-w
+0000de30: 6964 7468 3a20 312e 3437 3633 3330 3634  idth: 1.47633064
+0000de40: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+0000de50: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0000de60: 726f 6b65 2d6c 696e 6563 6170 3a20 6275  roke-linecap: bu
+0000de70: 7474 3b0a 2020 2020 2020 2020 2020 2020  tt;.            
+0000de80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de90: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+0000dea0: 206d 6974 6572 3b0a 2020 2020 2020 2020   miter;.        
+0000deb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dec0: 2020 2020 7374 726f 6b65 2d6d 6974 6572      stroke-miter
+0000ded0: 6c69 6d69 743a 2034 3b0a 2020 2020 2020  limit: 4;.      
+0000dee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000def0: 2020 2020 2020 7374 726f 6b65 2d64 6173        stroke-das
+0000df00: 6861 7272 6179 3a20 6e6f 6e65 3b0a 2020  harray: none;.  
+0000df10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df20: 2020 2020 2020 2020 2020 7374 726f 6b65            stroke
+0000df30: 2d6f 7061 6369 7479 3a20 313b 0a20 2020  -opacity: 1;.   
+0000df40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df50: 2020 2020 2022 0a20 2020 2020 2020 2020       ".         
+0000df60: 2020 2020 2020 2020 2020 202f 3e0a 2020             />.  
+0000df70: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+0000df80: 7379 6d62 6f6c 3e0a 2020 2020 2020 2020  symbol>.        
+0000df90: 2020 2020 2020 2020 3c73 796d 626f 6c20          <symbol 
+0000dfa0: 6964 3d22 6f72 6234 3522 3e0a 2020 2020  id="orb45">.    
+0000dfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfc0: 3c70 6174 680a 2020 2020 2020 2020 2020  <path.          
+0000dfd0: 2020 2020 2020 2020 2020 2020 2020 643d                d=
+0000dfe0: 224d 2039 2e38 3130 3031 3738 2c39 2e35  "M 9.8100178,9.5
+0000dff0: 3932 3139 3636 2043 2036 2e39 3634 3036  921966 C 6.96406
+0000e000: 3538 2c39 2e35 3932 3139 3536 2034 2e31  58,9.5921956 4.1
+0000e010: 3138 3131 3235 2c39 2e35 3932 3139 3636  181125,9.5921966
+0000e020: 2031 2e32 3732 3136 2c39 2e35 3932 3139   1.27216,9.59219
+0000e030: 3636 2043 2032 2e36 3935 3133 3632 2c36  66 C 2.6951362,6
+0000e040: 2e37 3436 3234 3431 2034 2e31 3138 3131  .7462441 4.11811
+0000e050: 3235 2c33 2e39 3030 3239 3035 2035 2e35  25,3.9002905 5.5
+0000e060: 3431 3038 3838 2c31 2e30 3534 3333 3739  410888,1.0543379
+0000e070: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000e080: 2020 2020 2020 2020 2020 7374 796c 653d            style=
+0000e090: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000e0a0: 2020 2020 2020 2020 2020 2020 2020 6f70                op
+0000e0b0: 6163 6974 793a 2031 3b0a 2020 2020 2020  acity: 1;.      
+0000e0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0d0: 2020 2020 2020 6669 6c6c 3a20 6e6f 6e65        fill: none
+0000e0e0: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+0000e0f0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+0000e100: 6c6c 2d6f 7061 6369 7479 3a20 313b 0a20  ll-opacity: 1;. 
 0000e110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e120: 2020 2020 2020 2020 2020 6669 6c6c 3a20            fill: 
-0000e130: 6e6f 6e65 3b0a 2020 2020 2020 2020 2020  none;.          
+0000e120: 2020 2020 2020 2020 2020 2066 696c 6c2d             fill-
+0000e130: 7275 6c65 3a20 6e6f 6e7a 6572 6f3b 0a20  rule: nonzero;. 
 0000e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e150: 2020 6669 6c6c 2d6f 7061 6369 7479 3a20    fill-opacity: 
-0000e160: 313b 0a20 2020 2020 2020 2020 2020 2020  1;.             
-0000e170: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000e180: 696c 6c2d 7275 6c65 3a20 6e6f 6e7a 6572  ill-rule: nonzer
-0000e190: 6f3b 0a20 2020 2020 2020 2020 2020 2020  o;.             
-0000e1a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e1b0: 7472 6f6b 653a 2024 6f72 625f 636f 6c6f  troke: $orb_colo
-0000e1c0: 725f 3435 3b0a 2020 2020 2020 2020 2020  r_45;.          
-0000e1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1e0: 2020 7374 726f 6b65 2d77 6964 7468 3a20    stroke-width: 
-0000e1f0: 312e 3437 3633 3330 3634 3b0a 2020 2020  1.47633064;.    
-0000e200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e210: 2020 2020 2020 2020 7374 726f 6b65 2d6c          stroke-l
-0000e220: 696e 6563 6170 3a20 6275 7474 3b0a 2020  inecap: butt;.  
-0000e230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e240: 2020 2020 2020 2020 2020 7374 726f 6b65            stroke
-0000e250: 2d6c 696e 656a 6f69 6e3a 206d 6974 6572  -linejoin: miter
-0000e260: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-0000e270: 2020 2020 2020 2020 2020 2020 2020 7374                st
-0000e280: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-0000e290: 2034 3b0a 2020 2020 2020 2020 2020 2020   4;.            
-0000e2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2b0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-0000e2c0: 3a20 6e6f 6e65 3b0a 2020 2020 2020 2020  : none;.        
-0000e2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2e0: 2020 2020 7374 726f 6b65 2d6f 7061 6369      stroke-opaci
-0000e2f0: 7479 3a20 313b 0a20 2020 2020 2020 2020  ty: 1;.         
-0000e300: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000e310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e320: 2020 2020 202f 3e0a 2020 2020 2020 2020       />.        
-0000e330: 2020 2020 2020 2020 3c2f 7379 6d62 6f6c          </symbol
-0000e340: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000e350: 2020 3c73 796d 626f 6c20 6964 3d22 6f72    <symbol id="or
-0000e360: 6236 3022 3e0a 2020 2020 2020 2020 2020  b60">.          
-0000e370: 2020 2020 2020 2020 2020 3c70 6174 680a            <path.
-0000e380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e390: 2020 2020 2020 2020 643d 224d 2030 2e38          d="M 0.8
-0000e3a0: 3831 3832 3434 312c 302e 3731 3831 3437  8182441,0.718147
-0000e3b0: 3635 2043 2033 2e33 3830 3638 3732 2c33  65 C 3.3806872,3
-0000e3c0: 2e32 3137 3630 3037 2035 2e38 3739 3535  .2176007 5.87955
-0000e3d0: 3032 2c35 2e37 3137 3035 3237 2038 2e33  02,5.7170527 8.3
-0000e3e0: 3738 3431 3332 2c38 2e32 3136 3530 3537  784132,8.2165057
-0000e3f0: 204d 2038 2e36 3131 3933 3632 2c34 2e34   M 8.6119362,4.4
-0000e400: 3033 3635 3537 2043 2035 2e39 3634 3034  036557 C 5.96404
-0000e410: 3432 2c34 2e34 3033 3635 3537 2033 2e33  42,4.4036557 3.3
-0000e420: 3136 3135 3334 2c34 2e34 3033 3635 3537  161534,4.4036557
-0000e430: 2030 2e36 3638 3236 3232 312c 342e 3430   0.66826221,4.40
-0000e440: 3336 3535 3720 4d20 302e 3834 3932 3537  36557 M 0.849257
-0000e450: 3831 2c38 2e31 3934 3439 3737 2043 2033  81,8.1944977 C 3
-0000e460: 2e33 3736 3438 3532 2c35 2e37 3232 3433  .3764852,5.72243
-0000e470: 3337 2035 2e39 3033 3731 3332 2c33 2e32  37 5.9037132,3.2
-0000e480: 3530 3337 3037 2038 2e34 3330 3934 3032  503707 8.4309402
-0000e490: 2c30 2e37 3738 3330 3736 3522 0a20 2020  ,0.77830765".   
-0000e4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4b0: 2020 2020 2073 7479 6c65 3d22 0a20 2020       style=".   
+0000e150: 2020 2020 2020 2020 2020 2073 7472 6f6b             strok
+0000e160: 653a 2024 6f72 625f 636f 6c6f 725f 3435  e: $orb_color_45
+0000e170: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+0000e180: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0000e190: 726f 6b65 2d77 6964 7468 3a20 312e 3437  roke-width: 1.47
+0000e1a0: 3633 3330 3634 3b0a 2020 2020 2020 2020  633064;.        
+0000e1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1c0: 2020 2020 7374 726f 6b65 2d6c 696e 6563      stroke-linec
+0000e1d0: 6170 3a20 6275 7474 3b0a 2020 2020 2020  ap: butt;.      
+0000e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1f0: 2020 2020 2020 7374 726f 6b65 2d6c 696e        stroke-lin
+0000e200: 656a 6f69 6e3a 206d 6974 6572 3b0a 2020  ejoin: miter;.  
+0000e210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e220: 2020 2020 2020 2020 2020 7374 726f 6b65            stroke
+0000e230: 2d6d 6974 6572 6c69 6d69 743a 2034 3b0a  -miterlimit: 4;.
+0000e240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e250: 2020 2020 2020 2020 2020 2020 7374 726f              stro
+0000e260: 6b65 2d64 6173 6861 7272 6179 3a20 6e6f  ke-dasharray: no
+0000e270: 6e65 3b0a 2020 2020 2020 2020 2020 2020  ne;.            
+0000e280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e290: 7374 726f 6b65 2d6f 7061 6369 7479 3a20  stroke-opacity: 
+0000e2a0: 313b 0a20 2020 2020 2020 2020 2020 2020  1;.             
+0000e2b0: 2020 2020 2020 2020 2020 2022 0a20 2020             ".   
+0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2d0: 202f 3e0a 2020 2020 2020 2020 2020 2020   />.            
+0000e2e0: 2020 2020 3c2f 7379 6d62 6f6c 3e0a 2020      </symbol>.  
+0000e2f0: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
+0000e300: 796d 626f 6c20 6964 3d22 6f72 6236 3022  ymbol id="orb60"
+0000e310: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000e320: 2020 2020 2020 3c70 6174 680a 2020 2020        <path.    
+0000e330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e340: 2020 2020 643d 224d 2030 2e38 3831 3832      d="M 0.88182
+0000e350: 3434 312c 302e 3731 3831 3437 3635 2043  441,0.71814765 C
+0000e360: 2033 2e33 3830 3638 3732 2c33 2e32 3137   3.3806872,3.217
+0000e370: 3630 3037 2035 2e38 3739 3535 3032 2c35  6007 5.8795502,5
+0000e380: 2e37 3137 3035 3237 2038 2e33 3738 3431  .7170527 8.37841
+0000e390: 3332 2c38 2e32 3136 3530 3537 204d 2038  32,8.2165057 M 8
+0000e3a0: 2e36 3131 3933 3632 2c34 2e34 3033 3635  .6119362,4.40365
+0000e3b0: 3537 2043 2035 2e39 3634 3034 3432 2c34  57 C 5.9640442,4
+0000e3c0: 2e34 3033 3635 3537 2033 2e33 3136 3135  .4036557 3.31615
+0000e3d0: 3334 2c34 2e34 3033 3635 3537 2030 2e36  34,4.4036557 0.6
+0000e3e0: 3638 3236 3232 312c 342e 3430 3336 3535  6826221,4.403655
+0000e3f0: 3720 4d20 302e 3834 3932 3537 3831 2c38  7 M 0.84925781,8
+0000e400: 2e31 3934 3439 3737 2043 2033 2e33 3736  .1944977 C 3.376
+0000e410: 3438 3532 2c35 2e37 3232 3433 3337 2035  4852,5.7224337 5
+0000e420: 2e39 3033 3731 3332 2c33 2e32 3530 3337  .9037132,3.25037
+0000e430: 3037 2038 2e34 3330 3934 3032 2c30 2e37  07 8.4309402,0.7
+0000e440: 3738 3330 3736 3522 0a20 2020 2020 2020  7830765".       
+0000e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e460: 2073 7479 6c65 3d22 0a20 2020 2020 2020   style=".       
+0000e470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e480: 2020 2020 206f 7061 6369 7479 3a20 313b       opacity: 1;
+0000e490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e4a0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+0000e4b0: 6c3a 206e 6f6e 653b 0a20 2020 2020 2020  l: none;.       
 0000e4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4d0: 2020 2020 2020 2020 206f 7061 6369 7479           opacity
-0000e4e0: 3a20 313b 0a20 2020 2020 2020 2020 2020  : 1;.           
+0000e4d0: 2020 2020 2066 696c 6c2d 6f70 6163 6974       fill-opacit
+0000e4e0: 793a 2031 3b0a 2020 2020 2020 2020 2020  y: 1;.          
 0000e4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e500: 2066 696c 6c3a 206e 6f6e 653b 0a20 2020   fill: none;.   
-0000e510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e520: 2020 2020 2020 2020 2066 696c 6c2d 6f70           fill-op
-0000e530: 6163 6974 793a 2031 3b0a 2020 2020 2020  acity: 1;.      
-0000e540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e550: 2020 2020 2020 6669 6c6c 2d72 756c 653a        fill-rule:
-0000e560: 206e 6f6e 7a65 726f 3b0a 2020 2020 2020   nonzero;.      
-0000e570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e580: 2020 2020 2020 7374 726f 6b65 3a20 246f        stroke: $o
-0000e590: 7262 5f63 6f6c 6f72 5f36 303b 0a20 2020  rb_color_60;.   
-0000e5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5b0: 2020 2020 2020 2020 2073 7472 6f6b 652d           stroke-
-0000e5c0: 7769 6474 683a 2031 2e34 3736 3333 3036  width: 1.4763306
-0000e5d0: 343b 0a20 2020 2020 2020 2020 2020 2020  4;.             
-0000e5e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e5f0: 7472 6f6b 652d 6c69 6e65 6361 703a 2062  troke-linecap: b
-0000e600: 7574 743b 0a20 2020 2020 2020 2020 2020  utt;.           
-0000e610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e620: 2073 7472 6f6b 652d 6c69 6e65 6a6f 696e   stroke-linejoin
-0000e630: 3a20 6d69 7465 723b 0a20 2020 2020 2020  : miter;.       
-0000e640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e650: 2020 2020 2073 7472 6f6b 652d 6d69 7465       stroke-mite
-0000e660: 726c 696d 6974 3a20 343b 0a20 2020 2020  rlimit: 4;.     
-0000e670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e680: 2020 2020 2020 2073 7472 6f6b 652d 6461         stroke-da
-0000e690: 7368 6172 7261 793a 206e 6f6e 653b 0a20  sharray: none;. 
-0000e6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6b0: 2020 2020 2020 2020 2020 2073 7472 6f6b             strok
-0000e6c0: 652d 6f70 6163 6974 793a 2031 3b0a 2020  e-opacity: 1;.  
-0000e6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6e0: 2020 2020 2020 220a 2020 2020 2020 2020        ".        
-0000e6f0: 2020 2020 2020 2020 2020 2020 2f3e 0a20              />. 
-0000e700: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000e710: 2f73 796d 626f 6c3e 0a20 2020 2020 2020  /symbol>.       
-0000e720: 2020 2020 2020 2020 203c 7379 6d62 6f6c           <symbol
-0000e730: 2069 643d 226f 7262 3732 223e 0a20 2020   id="orb72">.   
-0000e740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e750: 203c 7061 7468 0a20 2020 2020 2020 2020   <path.         
-0000e760: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000e770: 3d22 4d20 382e 3931 3635 3034 342c 352e  ="M 8.9165044,5.
-0000e780: 3634 3137 3433 3820 4320 382e 3931 3635  6417438 C 8.9165
-0000e790: 3034 342c 372e 3936 3837 3636 3320 372e  044,7.9687663 7.
-0000e7a0: 3237 3432 3834 342c 392e 3835 3531 3839  2742844,9.855189
-0000e7b0: 3320 352e 3234 3835 3033 342c 392e 3835  3 5.2485034,9.85
-0000e7c0: 3531 3839 3320 4320 332e 3232 3237 3232  51893 C 3.222722
-0000e7d0: 342c 392e 3835 3531 3839 3320 312e 3538  4,9.8551893 1.58
-0000e7e0: 3035 3032 372c 372e 3936 3837 3636 3320  05027,7.9687663 
-0000e7f0: 312e 3538 3035 3032 372c 352e 3634 3137  1.5805027,5.6417
-0000e800: 3433 3820 4320 312e 3538 3035 3032 372c  438 C 1.5805027,
-0000e810: 332e 3331 3437 3230 3820 332e 3232 3237  3.3147208 3.2227
-0000e820: 3232 342c 312e 3432 3832 3936 3720 352e  224,1.4282967 5.
-0000e830: 3234 3835 3033 342c 312e 3432 3832 3936  2485034,1.428296
-0000e840: 3720 4320 372e 3237 3432 3834 342c 312e  7 C 7.2742844,1.
-0000e850: 3432 3832 3936 3720 382e 3931 3635 3034  4282967 8.916504
-0000e860: 342c 332e 3331 3437 3230 3820 382e 3931  4,3.3147208 8.91
-0000e870: 3635 3034 342c 352e 3634 3137 3433 3820  65044,5.6417438 
-0000e880: 4c20 382e 3931 3635 3034 342c 352e 3634  L 8.9165044,5.64
-0000e890: 3137 3433 3820 7a20 4d20 352e 3437 3032  17438 z M 5.4702
-0000e8a0: 3633 342c 362e 3734 3633 3335 3820 4320  634,6.7463358 C 
-0000e8b0: 392e 3035 3131 3830 342c 3130 2e31 3139  9.0511804,10.119
-0000e8c0: 3232 3820 392e 3035 3131 3830 342c 3130  228 9.0511804,10
-0000e8d0: 2e31 3139 3232 3820 392e 3035 3131 3830  .119228 9.051180
-0000e8e0: 342c 3130 2e31 3139 3232 3822 0a20 2020  4,10.119228".   
-0000e8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e900: 2020 2020 2073 7479 6c65 3d22 0a20 2020       style=".   
+0000e500: 2020 6669 6c6c 2d72 756c 653a 206e 6f6e    fill-rule: non
+0000e510: 7a65 726f 3b0a 2020 2020 2020 2020 2020  zero;.          
+0000e520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e530: 2020 7374 726f 6b65 3a20 246f 7262 5f63    stroke: $orb_c
+0000e540: 6f6c 6f72 5f36 303b 0a20 2020 2020 2020  olor_60;.       
+0000e550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e560: 2020 2020 2073 7472 6f6b 652d 7769 6474       stroke-widt
+0000e570: 683a 2031 2e34 3736 3333 3036 343b 0a20  h: 1.47633064;. 
+0000e580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e590: 2020 2020 2020 2020 2020 2073 7472 6f6b             strok
+0000e5a0: 652d 6c69 6e65 6361 703a 2062 7574 743b  e-linecap: butt;
+0000e5b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e5c0: 2020 2020 2020 2020 2020 2020 2073 7472               str
+0000e5d0: 6f6b 652d 6c69 6e65 6a6f 696e 3a20 6d69  oke-linejoin: mi
+0000e5e0: 7465 723b 0a20 2020 2020 2020 2020 2020  ter;.           
+0000e5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e600: 2073 7472 6f6b 652d 6d69 7465 726c 696d   stroke-miterlim
+0000e610: 6974 3a20 343b 0a20 2020 2020 2020 2020  it: 4;.         
+0000e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e630: 2020 2073 7472 6f6b 652d 6461 7368 6172     stroke-dashar
+0000e640: 7261 793a 206e 6f6e 653b 0a20 2020 2020  ray: none;.     
+0000e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e660: 2020 2020 2020 2073 7472 6f6b 652d 6f70         stroke-op
+0000e670: 6163 6974 793a 2031 3b0a 2020 2020 2020  acity: 1;.      
+0000e680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e690: 2020 220a 2020 2020 2020 2020 2020 2020    ".            
+0000e6a0: 2020 2020 2020 2020 2f3e 0a20 2020 2020          />.     
+0000e6b0: 2020 2020 2020 2020 2020 203c 2f73 796d             </sym
+0000e6c0: 626f 6c3e 0a20 2020 2020 2020 2020 2020  bol>.           
+0000e6d0: 2020 2020 203c 7379 6d62 6f6c 2069 643d       <symbol id=
+0000e6e0: 226f 7262 3732 223e 0a20 2020 2020 2020  "orb72">.       
+0000e6f0: 2020 2020 2020 2020 2020 2020 203c 7061               <pa
+0000e700: 7468 0a20 2020 2020 2020 2020 2020 2020  th.             
+0000e710: 2020 2020 2020 2020 2020 2064 3d22 4d20             d="M 
+0000e720: 382e 3931 3635 3034 342c 352e 3634 3137  8.9165044,5.6417
+0000e730: 3433 3820 4320 382e 3931 3635 3034 342c  438 C 8.9165044,
+0000e740: 372e 3936 3837 3636 3320 372e 3237 3432  7.9687663 7.2742
+0000e750: 3834 342c 392e 3835 3531 3839 3320 352e  844,9.8551893 5.
+0000e760: 3234 3835 3033 342c 392e 3835 3531 3839  2485034,9.855189
+0000e770: 3320 4320 332e 3232 3237 3232 342c 392e  3 C 3.2227224,9.
+0000e780: 3835 3531 3839 3320 312e 3538 3035 3032  8551893 1.580502
+0000e790: 372c 372e 3936 3837 3636 3320 312e 3538  7,7.9687663 1.58
+0000e7a0: 3035 3032 372c 352e 3634 3137 3433 3820  05027,5.6417438 
+0000e7b0: 4320 312e 3538 3035 3032 372c 332e 3331  C 1.5805027,3.31
+0000e7c0: 3437 3230 3820 332e 3232 3237 3232 342c  47208 3.2227224,
+0000e7d0: 312e 3432 3832 3936 3720 352e 3234 3835  1.4282967 5.2485
+0000e7e0: 3033 342c 312e 3432 3832 3936 3720 4320  034,1.4282967 C 
+0000e7f0: 372e 3237 3432 3834 342c 312e 3432 3832  7.2742844,1.4282
+0000e800: 3936 3720 382e 3931 3635 3034 342c 332e  967 8.9165044,3.
+0000e810: 3331 3437 3230 3820 382e 3931 3635 3034  3147208 8.916504
+0000e820: 342c 352e 3634 3137 3433 3820 4c20 382e  4,5.6417438 L 8.
+0000e830: 3931 3635 3034 342c 352e 3634 3137 3433  9165044,5.641743
+0000e840: 3820 7a20 4d20 352e 3437 3032 3633 342c  8 z M 5.4702634,
+0000e850: 362e 3734 3633 3335 3820 4320 392e 3035  6.7463358 C 9.05
+0000e860: 3131 3830 342c 3130 2e31 3139 3232 3820  11804,10.119228 
+0000e870: 392e 3035 3131 3830 342c 3130 2e31 3139  9.0511804,10.119
+0000e880: 3232 3820 392e 3035 3131 3830 342c 3130  228 9.0511804,10
+0000e890: 2e31 3139 3232 3822 0a20 2020 2020 2020  .119228".       
+0000e8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8b0: 2073 7479 6c65 3d22 0a20 2020 2020 2020   style=".       
+0000e8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8d0: 2020 2020 206f 7061 6369 7479 3a20 313b       opacity: 1;
+0000e8e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e8f0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+0000e900: 6c3a 206e 6f6e 653b 0a20 2020 2020 2020  l: none;.       
 0000e910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e920: 2020 2020 2020 2020 206f 7061 6369 7479           opacity
-0000e930: 3a20 313b 0a20 2020 2020 2020 2020 2020  : 1;.           
+0000e920: 2020 2020 2066 696c 6c2d 6f70 6163 6974       fill-opacit
+0000e930: 793a 2031 3b0a 2020 2020 2020 2020 2020  y: 1;.          
 0000e940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e950: 2066 696c 6c3a 206e 6f6e 653b 0a20 2020   fill: none;.   
-0000e960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e970: 2020 2020 2020 2020 2066 696c 6c2d 6f70           fill-op
-0000e980: 6163 6974 793a 2031 3b0a 2020 2020 2020  acity: 1;.      
-0000e990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9a0: 2020 2020 2020 6669 6c6c 2d72 756c 653a        fill-rule:
-0000e9b0: 206e 6f6e 7a65 726f 3b0a 2020 2020 2020   nonzero;.      
-0000e9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9d0: 2020 2020 2020 7374 726f 6b65 3a20 246f        stroke: $o
-0000e9e0: 7262 5f63 6f6c 6f72 5f37 323b 0a20 2020  rb_color_72;.   
-0000e9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea00: 2020 2020 2020 2020 2073 7472 6f6b 652d           stroke-
-0000ea10: 7769 6474 683a 2031 2e34 3736 3333 3036  width: 1.4763306
-0000ea20: 343b 0a20 2020 2020 2020 2020 2020 2020  4;.             
-0000ea30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ea40: 7472 6f6b 652d 6c69 6e65 6361 703a 2062  troke-linecap: b
-0000ea50: 7574 743b 0a20 2020 2020 2020 2020 2020  utt;.           
-0000ea60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea70: 2073 7472 6f6b 652d 6c69 6e65 6a6f 696e   stroke-linejoin
-0000ea80: 3a20 6d69 7465 723b 0a20 2020 2020 2020  : miter;.       
-0000ea90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eaa0: 2020 2020 2073 7472 6f6b 652d 6d69 7465       stroke-mite
-0000eab0: 726c 696d 6974 3a20 343b 0a20 2020 2020  rlimit: 4;.     
-0000eac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ead0: 2020 2020 2020 2073 7472 6f6b 652d 6461         stroke-da
-0000eae0: 7368 6172 7261 793a 206e 6f6e 653b 0a20  sharray: none;. 
-0000eaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb00: 2020 2020 2020 2020 2020 2073 7472 6f6b             strok
-0000eb10: 652d 6f70 6163 6974 793a 2031 3b0a 2020  e-opacity: 1;.  
-0000eb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb30: 2020 2020 2020 220a 2020 2020 2020 2020        ".        
-0000eb40: 2020 2020 2020 2020 2020 2020 2f3e 0a20              />. 
-0000eb50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000eb60: 2f73 796d 626f 6c3e 0a20 2020 2020 2020  /symbol>.       
-0000eb70: 2020 2020 2020 2020 203c 7379 6d62 6f6c           <symbol
-0000eb80: 2069 643d 226f 7262 3930 223e 0a20 2020   id="orb90">.   
-0000eb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eba0: 203c 7265 6374 0a20 2020 2020 2020 2020   <rect.         
-0000ebb0: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-0000ebc0: 6569 6768 743d 2238 2e30 3836 3139 3522  eight="8.086195"
-0000ebd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ebe0: 2020 2020 2020 2020 2077 6964 7468 3d22           width="
-0000ebf0: 382e 3731 3538 3133 3622 0a20 2020 2020  8.7158136".     
-0000ec00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec10: 2020 2078 3d22 312e 3138 3331 3832 3622     x="1.1831826"
-0000ec20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ec30: 2020 2020 2020 2020 2079 3d22 312e 3138           y="1.18
-0000ec40: 3932 3534 3522 0a20 2020 2020 2020 2020  92545".         
-0000ec50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ec60: 7479 6c65 3d22 0a20 2020 2020 2020 2020  tyle=".         
-0000ec70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec80: 2020 206f 7061 6369 7479 3a20 313b 0a20     opacity: 1;. 
+0000e950: 2020 6669 6c6c 2d72 756c 653a 206e 6f6e    fill-rule: non
+0000e960: 7a65 726f 3b0a 2020 2020 2020 2020 2020  zero;.          
+0000e970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e980: 2020 7374 726f 6b65 3a20 246f 7262 5f63    stroke: $orb_c
+0000e990: 6f6c 6f72 5f37 323b 0a20 2020 2020 2020  olor_72;.       
+0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9b0: 2020 2020 2073 7472 6f6b 652d 7769 6474       stroke-widt
+0000e9c0: 683a 2031 2e34 3736 3333 3036 343b 0a20  h: 1.47633064;. 
+0000e9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9e0: 2020 2020 2020 2020 2020 2073 7472 6f6b             strok
+0000e9f0: 652d 6c69 6e65 6361 703a 2062 7574 743b  e-linecap: butt;
+0000ea00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ea10: 2020 2020 2020 2020 2020 2020 2073 7472               str
+0000ea20: 6f6b 652d 6c69 6e65 6a6f 696e 3a20 6d69  oke-linejoin: mi
+0000ea30: 7465 723b 0a20 2020 2020 2020 2020 2020  ter;.           
+0000ea40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea50: 2073 7472 6f6b 652d 6d69 7465 726c 696d   stroke-miterlim
+0000ea60: 6974 3a20 343b 0a20 2020 2020 2020 2020  it: 4;.         
+0000ea70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea80: 2020 2073 7472 6f6b 652d 6461 7368 6172     stroke-dashar
+0000ea90: 7261 793a 206e 6f6e 653b 0a20 2020 2020  ray: none;.     
+0000eaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eab0: 2020 2020 2020 2073 7472 6f6b 652d 6f70         stroke-op
+0000eac0: 6163 6974 793a 2031 3b0a 2020 2020 2020  acity: 1;.      
+0000ead0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eae0: 2020 220a 2020 2020 2020 2020 2020 2020    ".            
+0000eaf0: 2020 2020 2020 2020 2f3e 0a20 2020 2020          />.     
+0000eb00: 2020 2020 2020 2020 2020 203c 2f73 796d             </sym
+0000eb10: 626f 6c3e 0a20 2020 2020 2020 2020 2020  bol>.           
+0000eb20: 2020 2020 203c 7379 6d62 6f6c 2069 643d       <symbol id=
+0000eb30: 226f 7262 3930 223e 0a20 2020 2020 2020  "orb90">.       
+0000eb40: 2020 2020 2020 2020 2020 2020 203c 7265               <re
+0000eb50: 6374 0a20 2020 2020 2020 2020 2020 2020  ct.             
+0000eb60: 2020 2020 2020 2020 2020 2068 6569 6768             heigh
+0000eb70: 743d 2238 2e30 3836 3139 3522 0a20 2020  t="8.086195".   
+0000eb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb90: 2020 2020 2077 6964 7468 3d22 382e 3731       width="8.71
+0000eba0: 3538 3133 3622 0a20 2020 2020 2020 2020  58136".         
+0000ebb0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+0000ebc0: 3d22 312e 3138 3331 3832 3622 0a20 2020  ="1.1831826".   
+0000ebd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebe0: 2020 2020 2079 3d22 312e 3138 3932 3534       y="1.189254
+0000ebf0: 3522 0a20 2020 2020 2020 2020 2020 2020  5".             
+0000ec00: 2020 2020 2020 2020 2020 2073 7479 6c65             style
+0000ec10: 3d22 0a20 2020 2020 2020 2020 2020 2020  =".             
+0000ec20: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000ec30: 7061 6369 7479 3a20 313b 0a20 2020 2020  pacity: 1;.     
+0000ec40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec50: 2020 2020 2020 2066 696c 6c3a 206e 6f6e         fill: non
+0000ec60: 653b 0a20 2020 2020 2020 2020 2020 2020  e;.             
+0000ec70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000ec80: 696c 6c2d 6f70 6163 6974 793a 2031 3b0a  ill-opacity: 1;.
 0000ec90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eca0: 2020 2020 2020 2020 2020 2066 696c 6c3a             fill:
-0000ecb0: 206e 6f6e 653b 0a20 2020 2020 2020 2020   none;.         
+0000eca0: 2020 2020 2020 2020 2020 2020 6669 6c6c              fill
+0000ecb0: 2d72 756c 653a 206e 6f6e 7a65 726f 3b0a  -rule: nonzero;.
 0000ecc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ecd0: 2020 2066 696c 6c2d 6f70 6163 6974 793a     fill-opacity:
-0000ece0: 2031 3b0a 2020 2020 2020 2020 2020 2020   1;.            
-0000ecf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed00: 6669 6c6c 2d72 756c 653a 206e 6f6e 7a65  fill-rule: nonze
-0000ed10: 726f 3b0a 2020 2020 2020 2020 2020 2020  ro;.            
-0000ed20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed30: 7374 726f 6b65 3a20 246f 7262 5f63 6f6c  stroke: $orb_col
-0000ed40: 6f72 5f39 303b 0a20 2020 2020 2020 2020  or_90;.         
-0000ed50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed60: 2020 2073 7472 6f6b 652d 7769 6474 683a     stroke-width:
-0000ed70: 2031 2e32 3530 3339 3531 383b 0a20 2020   1.25039518;.   
-0000ed80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed90: 2020 2020 2020 2020 2073 7472 6f6b 652d           stroke-
-0000eda0: 6c69 6e65 6361 703a 2062 7574 743b 0a20  linecap: butt;. 
-0000edb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000edc0: 2020 2020 2020 2020 2020 2073 7472 6f6b             strok
-0000edd0: 652d 6c69 6e65 6a6f 696e 3a20 6d69 7465  e-linejoin: mite
-0000ede0: 723b 0a20 2020 2020 2020 2020 2020 2020  r;.             
-0000edf0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ee00: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-0000ee10: 3a20 343b 0a20 2020 2020 2020 2020 2020  : 4;.           
-0000ee20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee30: 2073 7472 6f6b 652d 6461 7368 6172 7261   stroke-dasharra
-0000ee40: 793a 206e 6f6e 653b 0a20 2020 2020 2020  y: none;.       
-0000ee50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee60: 2020 2020 2073 7472 6f6b 652d 6f70 6163       stroke-opac
-0000ee70: 6974 793a 2031 3b0a 2020 2020 2020 2020  ity: 1;.        
-0000ee80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee90: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000eea0: 2020 2020 2020 2f3e 0a20 2020 2020 2020        />.       
-0000eeb0: 2020 2020 2020 2020 203c 2f73 796d 626f           </symbo
-0000eec0: 6c3e 0a20 2020 2020 2020 2020 2020 2020  l>.             
-0000eed0: 2020 203c 7379 6d62 6f6c 2069 643d 226f     <symbol id="o
-0000eee0: 7262 3132 3022 3e0a 2020 2020 2020 2020  rb120">.        
-0000eef0: 2020 2020 2020 2020 2020 2020 3c70 6174              <pat
-0000ef00: 680a 2020 2020 2020 2020 2020 2020 2020  h.              
-0000ef10: 2020 2020 2020 2020 2020 643d 224d 2031            d="M 1
-0000ef20: 2e31 3735 3530 3131 2c39 2e34 3937 3937  .1755011,9.49797
-0000ef30: 3320 4320 392e 3039 3537 3836 392c 392e  3 C 9.0957869,9.
-0000ef40: 3439 3739 3733 2039 2e30 3935 3738 3639  497973 9.0957869
-0000ef50: 2c39 2e34 3937 3937 3320 392e 3039 3537  ,9.497973 9.0957
-0000ef60: 3836 392c 392e 3439 3739 3733 204c 2035  869,9.497973 L 5
-0000ef70: 2e31 3335 3634 3338 2c31 2e34 3633 3930  .1356438,1.46390
-0000ef80: 3633 2043 2035 2e31 3335 3634 3338 2c31  63 C 5.1356438,1
-0000ef90: 2e34 3633 3930 3633 2035 2e31 3335 3634  .4639063 5.13564
-0000efa0: 3338 2c31 2e34 3633 3930 3633 2031 2e31  38,1.4639063 1.1
-0000efb0: 3735 3530 3131 2c39 2e34 3937 3937 3320  755011,9.497973 
-0000efc0: 7a22 0a20 2020 2020 2020 2020 2020 2020  z".             
-0000efd0: 2020 2020 2020 2020 2020 2073 7479 6c65             style
-0000efe0: 3d22 0a20 2020 2020 2020 2020 2020 2020  =".             
-0000eff0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000f000: 696c 6c3a 206e 6f6e 653b 0a20 2020 2020  ill: none;.     
-0000f010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f020: 2020 2020 2020 2066 696c 6c2d 7275 6c65         fill-rule
-0000f030: 3a20 6576 656e 6f64 643b 0a20 2020 2020  : evenodd;.     
-0000f040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f050: 2020 2020 2020 2073 7472 6f6b 653a 2024         stroke: $
-0000f060: 6f72 625f 636f 6c6f 725f 3132 303b 0a20  orb_color_120;. 
-0000f070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f080: 2020 2020 2020 2020 2020 2073 7472 6f6b             strok
-0000f090: 652d 7769 6474 683a 2031 2e31 3936 3534  e-width: 1.19654
-0000f0a0: 3632 3b0a 2020 2020 2020 2020 2020 2020  62;.            
-0000f0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0c0: 7374 726f 6b65 2d6c 696e 6563 6170 3a20  stroke-linecap: 
-0000f0d0: 6275 7474 3b0a 2020 2020 2020 2020 2020  butt;.          
-0000f0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0f0: 2020 7374 726f 6b65 2d6c 696e 656a 6f69    stroke-linejoi
-0000f100: 6e3a 206d 6974 6572 3b0a 2020 2020 2020  n: miter;.      
-0000f110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f120: 2020 2020 2020 7374 726f 6b65 2d6d 6974        stroke-mit
-0000f130: 6572 6c69 6d69 743a 2034 3b0a 2020 2020  erlimit: 4;.    
-0000f140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f150: 2020 2020 2020 2020 7374 726f 6b65 2d64          stroke-d
-0000f160: 6173 6861 7272 6179 3a20 6e6f 6e65 3b0a  asharray: none;.
-0000f170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f180: 2020 2020 2020 2020 2020 2020 7374 726f              stro
-0000f190: 6b65 2d6f 7061 6369 7479 3a20 313b 0a20  ke-opacity: 1;. 
-0000f1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1b0: 2020 2020 2020 2022 0a20 2020 2020 2020         ".       
-0000f1c0: 2020 2020 2020 2020 2020 2020 202f 3e0a               />.
-0000f1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1e0: 3c2f 7379 6d62 6f6c 3e0a 2020 2020 2020  </symbol>.      
-0000f1f0: 2020 2020 2020 2020 2020 3c73 796d 626f            <symbo
-0000f200: 6c20 6964 3d22 6f72 6231 3335 223e 0a20  l id="orb135">. 
-0000f210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f220: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-0000f230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f240: 2064 3d22 4d20 322e 3233 3838 3538 322c   d="M 2.2388582,
-0000f250: 312e 3731 3536 3939 3420 4c20 392e 3239  1.7156994 L 9.29
-0000f260: 3338 3135 342c 312e 3731 3536 3939 3420  38154,1.7156994 
-0000f270: 4c20 392e 3239 3338 3135 342c 372e 3738  L 9.2938154,7.78
-0000f280: 3131 3832 3720 4c20 322e 3233 3838 3538  11827 L 2.238858
-0000f290: 322c 372e 3738 3131 3832 3720 4c20 322e  2,7.7811827 L 2.
-0000f2a0: 3233 3838 3538 322c 312e 3731 3536 3939  2388582,1.715699
-0000f2b0: 3420 7a20 4d20 362e 3834 3631 3130 342c  4 z M 6.8461104,
-0000f2c0: 352e 3537 3334 3236 3720 4320 362e 3834  5.5734267 C 6.84
-0000f2d0: 3631 3130 342c 352e 3537 3334 3236 3720  61104,5.5734267 
-0000f2e0: 362e 3834 3631 3130 342c 352e 3537 3334  6.8461104,5.5734
-0000f2f0: 3236 3720 332e 3234 3638 3635 322c 3130  267 3.2468652,10
-0000f300: 2e33 3732 3432 2043 2038 2e30 3435 3835  .37242 C 8.04585
-0000f310: 3834 2c31 302e 3337 3234 3220 382e 3034  84,10.37242 8.04
-0000f320: 3538 3538 342c 3130 2e33 3732 3432 2038  58584,10.37242 8
-0000f330: 2e30 3435 3835 3834 2c31 302e 3337 3234  .0458584,10.3724
-0000f340: 3222 0a20 2020 2020 2020 2020 2020 2020  2".             
-0000f350: 2020 2020 2020 2020 2020 2073 7479 6c65             style
-0000f360: 3d22 0a20 2020 2020 2020 2020 2020 2020  =".             
-0000f370: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000f380: 696c 6c3a 206e 6f6e 653b 0a20 2020 2020  ill: none;.     
-0000f390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3a0: 2020 2020 2020 2066 696c 6c2d 7275 6c65         fill-rule
-0000f3b0: 3a20 6576 656e 6f64 643b 0a20 2020 2020  : evenodd;.     
-0000f3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3d0: 2020 2020 2020 2073 7472 6f6b 653a 2024         stroke: $
-0000f3e0: 6f72 625f 636f 6c6f 725f 3133 353b 0a20  orb_color_135;. 
-0000f3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f400: 2020 2020 2020 2020 2020 2073 7472 6f6b             strok
-0000f410: 652d 7769 6474 683a 2031 2e31 3936 3534  e-width: 1.19654
-0000f420: 3632 3b0a 2020 2020 2020 2020 2020 2020  62;.            
-0000f430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f440: 7374 726f 6b65 2d6c 696e 6563 6170 3a20  stroke-linecap: 
-0000f450: 6275 7474 3b0a 2020 2020 2020 2020 2020  butt;.          
-0000f460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f470: 2020 7374 726f 6b65 2d6c 696e 656a 6f69    stroke-linejoi
-0000f480: 6e3a 206d 6974 6572 3b0a 2020 2020 2020  n: miter;.      
-0000f490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f4a0: 2020 2020 2020 7374 726f 6b65 2d6d 6974        stroke-mit
-0000f4b0: 6572 6c69 6d69 743a 2034 3b0a 2020 2020  erlimit: 4;.    
-0000f4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f4d0: 2020 2020 2020 2020 7374 726f 6b65 2d64          stroke-d
-0000f4e0: 6173 6861 7272 6179 3a20 6e6f 6e65 3b0a  asharray: none;.
-0000f4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f500: 2020 2020 2020 2020 2020 2020 7374 726f              stro
-0000f510: 6b65 2d6f 7061 6369 7479 3a20 313b 0a20  ke-opacity: 1;. 
-0000f520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f530: 2020 2020 2020 2022 0a20 2020 2020 2020         ".       
-0000f540: 2020 2020 2020 2020 2020 2020 202f 3e0a               />.
-0000f550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f560: 3c2f 7379 6d62 6f6c 3e0a 2020 2020 2020  </symbol>.      
-0000f570: 2020 2020 2020 2020 2020 3c73 796d 626f            <symbo
-0000f580: 6c20 6964 3d22 6f72 6231 3434 223e 0a20  l id="orb144">. 
-0000f590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5a0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-0000f5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5c0: 2064 3d22 4d20 312e 3432 3435 3136 392c   d="M 1.4245169,
-0000f5d0: 312e 3239 3638 3539 3820 4320 312e 3432  1.2968598 C 1.42
-0000f5e0: 3435 3136 392c 392e 3637 3633 3132 3920  45169,9.6763129 
-0000f5f0: 312e 3432 3435 3136 392c 392e 3637 3633  1.4245169,9.6763
-0000f600: 3132 3920 312e 3432 3435 3136 392c 392e  129 1.4245169,9.
-0000f610: 3637 3633 3132 3920 4d20 312e 3932 3038  6763129 M 1.9208
-0000f620: 3333 312c 352e 3338 3638 3237 3920 4320  331,5.3868279 C 
-0000f630: 322e 3737 3232 3838 362c 352e 3333 3532  2.7722886,5.3352
-0000f640: 3433 3920 332e 3535 3431 3535 332c 352e  439 3.5541553,5.
-0000f650: 3638 3634 3132 3920 332e 3933 3635 3233  6864129 3.936523
-0000f660: 372c 362e 3239 3231 3536 3920 4320 342e  7,6.2921569 C 4.
-0000f670: 3331 3838 3932 2c36 2e38 3937 3930 3039  318892,6.8979009
-0000f680: 2034 2e32 3335 3136 3134 2c37 2e36 3532   4.2351614,7.652
-0000f690: 3731 3239 2033 2e37 3230 3636 3232 2c38  7129 3.7206622,8
-0000f6a0: 2e32 3338 3039 3839 2043 2033 2e32 3036  .2380989 C 3.206
-0000f6b0: 3136 3332 2c38 2e38 3233 3438 3439 2032  1632,8.8234849 2
-0000f6c0: 2e33 3530 3531 3031 2c39 2e31 3337 3438  .3505101,9.13748
-0000f6d0: 3239 2031 2e35 3134 3734 3731 2c39 2e30  29 1.5147471,9.0
-0000f6e0: 3437 3630 3139 204d 2039 2e38 3532 3836  476019 M 9.85286
-0000f6f0: 3339 2c35 2e35 3835 3132 3439 2043 2039  39,5.5851249 C 9
-0000f700: 2e38 3533 3034 3439 2c37 2e34 3739 3334  .8530449,7.47934
-0000f710: 3139 2038 2e38 3634 3936 3939 2c39 2e30  19 8.8649699,9.0
-0000f720: 3135 3035 3739 2037 2e36 3436 3035 3339  150579 7.6460539
-0000f730: 2c39 2e30 3135 3035 3739 2043 2036 2e34  ,9.0150579 C 6.4
-0000f740: 3237 3133 3839 2c39 2e30 3135 3035 3739  271389,9.0150579
-0000f750: 2035 2e34 3339 3036 3239 2c37 2e34 3739   5.4390629,7.479
-0000f760: 3334 3139 2035 2e34 3339 3234 3439 2c35  3419 5.4392449,5
-0000f770: 2e35 3835 3132 3439 2043 2035 2e34 3339  .5851249 C 5.439
-0000f780: 3036 3239 2c33 2e36 3930 3930 3838 2036  0629,3.6909088 6
-0000f790: 2e34 3237 3133 3839 2c32 2e31 3535 3139  .4271389,2.15519
-0000f7a0: 3238 2037 2e36 3436 3035 3339 2c32 2e31  28 7.6460539,2.1
-0000f7b0: 3535 3139 3238 2043 2038 2e38 3634 3936  551928 C 8.86496
-0000f7c0: 3939 2c32 2e31 3535 3139 3238 2039 2e38  99,2.1551928 9.8
-0000f7d0: 3533 3034 3439 2c33 2e36 3930 3930 3838  530449,3.6909088
-0000f7e0: 2039 2e38 3532 3836 3339 2c35 2e35 3835   9.8528639,5.585
-0000f7f0: 3132 3439 207a 204d 2038 2e32 3538 3034  1249 z M 8.25804
-0000f800: 3439 2c37 2e32 3632 3739 3539 2043 2031  49,7.2627959 C 1
-0000f810: 302e 3139 3832 3536 2c39 2e39 3830 3336  0.198256,9.98036
-0000f820: 3739 2031 302e 3139 3832 3536 2c39 2e39  79 10.198256,9.9
-0000f830: 3830 3336 3739 2031 302e 3139 3832 3536  803679 10.198256
-0000f840: 2c39 2e39 3830 3336 3739 220a 2020 2020  ,9.9803679".    
-0000f850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f860: 2020 2020 7374 796c 653d 220a 2020 2020      style=".    
+0000ecd0: 2020 2020 2020 2020 2020 2020 7374 726f              stro
+0000ece0: 6b65 3a20 246f 7262 5f63 6f6c 6f72 5f39  ke: $orb_color_9
+0000ecf0: 303b 0a20 2020 2020 2020 2020 2020 2020  0;.             
+0000ed00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ed10: 7472 6f6b 652d 7769 6474 683a 2031 2e32  troke-width: 1.2
+0000ed20: 3530 3339 3531 383b 0a20 2020 2020 2020  5039518;.       
+0000ed30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed40: 2020 2020 2073 7472 6f6b 652d 6c69 6e65       stroke-line
+0000ed50: 6361 703a 2062 7574 743b 0a20 2020 2020  cap: butt;.     
+0000ed60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed70: 2020 2020 2020 2073 7472 6f6b 652d 6c69         stroke-li
+0000ed80: 6e65 6a6f 696e 3a20 6d69 7465 723b 0a20  nejoin: miter;. 
+0000ed90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eda0: 2020 2020 2020 2020 2020 2073 7472 6f6b             strok
+0000edb0: 652d 6d69 7465 726c 696d 6974 3a20 343b  e-miterlimit: 4;
+0000edc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000edd0: 2020 2020 2020 2020 2020 2020 2073 7472               str
+0000ede0: 6f6b 652d 6461 7368 6172 7261 793a 206e  oke-dasharray: n
+0000edf0: 6f6e 653b 0a20 2020 2020 2020 2020 2020  one;.           
+0000ee00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee10: 2073 7472 6f6b 652d 6f70 6163 6974 793a   stroke-opacity:
+0000ee20: 2031 3b0a 2020 2020 2020 2020 2020 2020   1;.            
+0000ee30: 2020 2020 2020 2020 2020 2020 220a 2020              ".  
+0000ee40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee50: 2020 2f3e 0a20 2020 2020 2020 2020 2020    />.           
+0000ee60: 2020 2020 203c 2f73 796d 626f 6c3e 0a20       </symbol>. 
+0000ee70: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000ee80: 7379 6d62 6f6c 2069 643d 226f 7262 3132  symbol id="orb12
+0000ee90: 3022 3e0a 2020 2020 2020 2020 2020 2020  0">.            
+0000eea0: 2020 2020 2020 2020 3c70 6174 680a 2020          <path.  
+0000eeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eec0: 2020 2020 2020 643d 224d 2031 2e31 3735        d="M 1.175
+0000eed0: 3530 3131 2c39 2e34 3937 3937 3320 4320  5011,9.497973 C 
+0000eee0: 392e 3039 3537 3836 392c 392e 3439 3739  9.0957869,9.4979
+0000eef0: 3733 2039 2e30 3935 3738 3639 2c39 2e34  73 9.0957869,9.4
+0000ef00: 3937 3937 3320 392e 3039 3537 3836 392c  97973 9.0957869,
+0000ef10: 392e 3439 3739 3733 204c 2035 2e31 3335  9.497973 L 5.135
+0000ef20: 3634 3338 2c31 2e34 3633 3930 3633 2043  6438,1.4639063 C
+0000ef30: 2035 2e31 3335 3634 3338 2c31 2e34 3633   5.1356438,1.463
+0000ef40: 3930 3633 2035 2e31 3335 3634 3338 2c31  9063 5.1356438,1
+0000ef50: 2e34 3633 3930 3633 2031 2e31 3735 3530  .4639063 1.17550
+0000ef60: 3131 2c39 2e34 3937 3937 3320 7a22 0a20  11,9.497973 z". 
+0000ef70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef80: 2020 2020 2020 2073 7479 6c65 3d22 0a20         style=". 
+0000ef90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efa0: 2020 2020 2020 2020 2020 2066 696c 6c3a             fill:
+0000efb0: 206e 6f6e 653b 0a20 2020 2020 2020 2020   none;.         
+0000efc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efd0: 2020 2066 696c 6c2d 7275 6c65 3a20 6576     fill-rule: ev
+0000efe0: 656e 6f64 643b 0a20 2020 2020 2020 2020  enodd;.         
+0000eff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f000: 2020 2073 7472 6f6b 653a 2024 6f72 625f     stroke: $orb_
+0000f010: 636f 6c6f 725f 3132 303b 0a20 2020 2020  color_120;.     
+0000f020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f030: 2020 2020 2020 2073 7472 6f6b 652d 7769         stroke-wi
+0000f040: 6474 683a 2031 2e31 3936 3534 3632 3b0a  dth: 1.1965462;.
+0000f050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f060: 2020 2020 2020 2020 2020 2020 7374 726f              stro
+0000f070: 6b65 2d6c 696e 6563 6170 3a20 6275 7474  ke-linecap: butt
+0000f080: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+0000f090: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0000f0a0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 206d  roke-linejoin: m
+0000f0b0: 6974 6572 3b0a 2020 2020 2020 2020 2020  iter;.          
+0000f0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0d0: 2020 7374 726f 6b65 2d6d 6974 6572 6c69    stroke-miterli
+0000f0e0: 6d69 743a 2034 3b0a 2020 2020 2020 2020  mit: 4;.        
+0000f0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f100: 2020 2020 7374 726f 6b65 2d64 6173 6861      stroke-dasha
+0000f110: 7272 6179 3a20 6e6f 6e65 3b0a 2020 2020  rray: none;.    
+0000f120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f130: 2020 2020 2020 2020 7374 726f 6b65 2d6f          stroke-o
+0000f140: 7061 6369 7479 3a20 313b 0a20 2020 2020  pacity: 1;.     
+0000f150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f160: 2020 2022 0a20 2020 2020 2020 2020 2020     ".           
+0000f170: 2020 2020 2020 2020 202f 3e0a 2020 2020           />.    
+0000f180: 2020 2020 2020 2020 2020 2020 3c2f 7379              </sy
+0000f190: 6d62 6f6c 3e0a 2020 2020 2020 2020 2020  mbol>.          
+0000f1a0: 2020 2020 2020 3c73 796d 626f 6c20 6964        <symbol id
+0000f1b0: 3d22 6f72 6231 3335 223e 0a20 2020 2020  ="orb135">.     
+0000f1c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000f1d0: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
+0000f1e0: 2020 2020 2020 2020 2020 2020 2064 3d22               d="
+0000f1f0: 4d20 322e 3233 3838 3538 322c 312e 3731  M 2.2388582,1.71
+0000f200: 3536 3939 3420 4c20 392e 3239 3338 3135  56994 L 9.293815
+0000f210: 342c 312e 3731 3536 3939 3420 4c20 392e  4,1.7156994 L 9.
+0000f220: 3239 3338 3135 342c 372e 3738 3131 3832  2938154,7.781182
+0000f230: 3720 4c20 322e 3233 3838 3538 322c 372e  7 L 2.2388582,7.
+0000f240: 3738 3131 3832 3720 4c20 322e 3233 3838  7811827 L 2.2388
+0000f250: 3538 322c 312e 3731 3536 3939 3420 7a20  582,1.7156994 z 
+0000f260: 4d20 362e 3834 3631 3130 342c 352e 3537  M 6.8461104,5.57
+0000f270: 3334 3236 3720 4320 362e 3834 3631 3130  34267 C 6.846110
+0000f280: 342c 352e 3537 3334 3236 3720 362e 3834  4,5.5734267 6.84
+0000f290: 3631 3130 342c 352e 3537 3334 3236 3720  61104,5.5734267 
+0000f2a0: 332e 3234 3638 3635 322c 3130 2e33 3732  3.2468652,10.372
+0000f2b0: 3432 2043 2038 2e30 3435 3835 3834 2c31  42 C 8.0458584,1
+0000f2c0: 302e 3337 3234 3220 382e 3034 3538 3538  0.37242 8.045858
+0000f2d0: 342c 3130 2e33 3732 3432 2038 2e30 3435  4,10.37242 8.045
+0000f2e0: 3835 3834 2c31 302e 3337 3234 3222 0a20  8584,10.37242". 
+0000f2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f300: 2020 2020 2020 2073 7479 6c65 3d22 0a20         style=". 
+0000f310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f320: 2020 2020 2020 2020 2020 2066 696c 6c3a             fill:
+0000f330: 206e 6f6e 653b 0a20 2020 2020 2020 2020   none;.         
+0000f340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f350: 2020 2066 696c 6c2d 7275 6c65 3a20 6576     fill-rule: ev
+0000f360: 656e 6f64 643b 0a20 2020 2020 2020 2020  enodd;.         
+0000f370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f380: 2020 2073 7472 6f6b 653a 2024 6f72 625f     stroke: $orb_
+0000f390: 636f 6c6f 725f 3133 353b 0a20 2020 2020  color_135;.     
+0000f3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3b0: 2020 2020 2020 2073 7472 6f6b 652d 7769         stroke-wi
+0000f3c0: 6474 683a 2031 2e31 3936 3534 3632 3b0a  dth: 1.1965462;.
+0000f3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3e0: 2020 2020 2020 2020 2020 2020 7374 726f              stro
+0000f3f0: 6b65 2d6c 696e 6563 6170 3a20 6275 7474  ke-linecap: butt
+0000f400: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+0000f410: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0000f420: 726f 6b65 2d6c 696e 656a 6f69 6e3a 206d  roke-linejoin: m
+0000f430: 6974 6572 3b0a 2020 2020 2020 2020 2020  iter;.          
+0000f440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f450: 2020 7374 726f 6b65 2d6d 6974 6572 6c69    stroke-miterli
+0000f460: 6d69 743a 2034 3b0a 2020 2020 2020 2020  mit: 4;.        
+0000f470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f480: 2020 2020 7374 726f 6b65 2d64 6173 6861      stroke-dasha
+0000f490: 7272 6179 3a20 6e6f 6e65 3b0a 2020 2020  rray: none;.    
+0000f4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4b0: 2020 2020 2020 2020 7374 726f 6b65 2d6f          stroke-o
+0000f4c0: 7061 6369 7479 3a20 313b 0a20 2020 2020  pacity: 1;.     
+0000f4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4e0: 2020 2022 0a20 2020 2020 2020 2020 2020     ".           
+0000f4f0: 2020 2020 2020 2020 202f 3e0a 2020 2020           />.    
+0000f500: 2020 2020 2020 2020 2020 2020 3c2f 7379              </sy
+0000f510: 6d62 6f6c 3e0a 2020 2020 2020 2020 2020  mbol>.          
+0000f520: 2020 2020 2020 3c73 796d 626f 6c20 6964        <symbol id
+0000f530: 3d22 6f72 6231 3434 223e 0a20 2020 2020  ="orb144">.     
+0000f540: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000f550: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
+0000f560: 2020 2020 2020 2020 2020 2020 2064 3d22               d="
+0000f570: 4d20 312e 3432 3435 3136 392c 312e 3239  M 1.4245169,1.29
+0000f580: 3638 3539 3820 4320 312e 3432 3435 3136  68598 C 1.424516
+0000f590: 392c 392e 3637 3633 3132 3920 312e 3432  9,9.6763129 1.42
+0000f5a0: 3435 3136 392c 392e 3637 3633 3132 3920  45169,9.6763129 
+0000f5b0: 312e 3432 3435 3136 392c 392e 3637 3633  1.4245169,9.6763
+0000f5c0: 3132 3920 4d20 312e 3932 3038 3333 312c  129 M 1.9208331,
+0000f5d0: 352e 3338 3638 3237 3920 4320 322e 3737  5.3868279 C 2.77
+0000f5e0: 3232 3838 362c 352e 3333 3532 3433 3920  22886,5.3352439 
+0000f5f0: 332e 3535 3431 3535 332c 352e 3638 3634  3.5541553,5.6864
+0000f600: 3132 3920 332e 3933 3635 3233 372c 362e  129 3.9365237,6.
+0000f610: 3239 3231 3536 3920 4320 342e 3331 3838  2921569 C 4.3188
+0000f620: 3932 2c36 2e38 3937 3930 3039 2034 2e32  92,6.8979009 4.2
+0000f630: 3335 3136 3134 2c37 2e36 3532 3731 3239  351614,7.6527129
+0000f640: 2033 2e37 3230 3636 3232 2c38 2e32 3338   3.7206622,8.238
+0000f650: 3039 3839 2043 2033 2e32 3036 3136 3332  0989 C 3.2061632
+0000f660: 2c38 2e38 3233 3438 3439 2032 2e33 3530  ,8.8234849 2.350
+0000f670: 3531 3031 2c39 2e31 3337 3438 3239 2031  5101,9.1374829 1
+0000f680: 2e35 3134 3734 3731 2c39 2e30 3437 3630  .5147471,9.04760
+0000f690: 3139 204d 2039 2e38 3532 3836 3339 2c35  19 M 9.8528639,5
+0000f6a0: 2e35 3835 3132 3439 2043 2039 2e38 3533  .5851249 C 9.853
+0000f6b0: 3034 3439 2c37 2e34 3739 3334 3139 2038  0449,7.4793419 8
+0000f6c0: 2e38 3634 3936 3939 2c39 2e30 3135 3035  .8649699,9.01505
+0000f6d0: 3739 2037 2e36 3436 3035 3339 2c39 2e30  79 7.6460539,9.0
+0000f6e0: 3135 3035 3739 2043 2036 2e34 3237 3133  150579 C 6.42713
+0000f6f0: 3839 2c39 2e30 3135 3035 3739 2035 2e34  89,9.0150579 5.4
+0000f700: 3339 3036 3239 2c37 2e34 3739 3334 3139  390629,7.4793419
+0000f710: 2035 2e34 3339 3234 3439 2c35 2e35 3835   5.4392449,5.585
+0000f720: 3132 3439 2043 2035 2e34 3339 3036 3239  1249 C 5.4390629
+0000f730: 2c33 2e36 3930 3930 3838 2036 2e34 3237  ,3.6909088 6.427
+0000f740: 3133 3839 2c32 2e31 3535 3139 3238 2037  1389,2.1551928 7
+0000f750: 2e36 3436 3035 3339 2c32 2e31 3535 3139  .6460539,2.15519
+0000f760: 3238 2043 2038 2e38 3634 3936 3939 2c32  28 C 8.8649699,2
+0000f770: 2e31 3535 3139 3238 2039 2e38 3533 3034  .1551928 9.85304
+0000f780: 3439 2c33 2e36 3930 3930 3838 2039 2e38  49,3.6909088 9.8
+0000f790: 3532 3836 3339 2c35 2e35 3835 3132 3439  528639,5.5851249
+0000f7a0: 207a 204d 2038 2e32 3538 3034 3439 2c37   z M 8.2580449,7
+0000f7b0: 2e32 3632 3739 3539 2043 2031 302e 3139  .2627959 C 10.19
+0000f7c0: 3832 3536 2c39 2e39 3830 3336 3739 2031  8256,9.9803679 1
+0000f7d0: 302e 3139 3832 3536 2c39 2e39 3830 3336  0.198256,9.98036
+0000f7e0: 3739 2031 302e 3139 3832 3536 2c39 2e39  79 10.198256,9.9
+0000f7f0: 3830 3336 3739 220a 2020 2020 2020 2020  803679".        
+0000f800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f810: 7374 796c 653d 220a 2020 2020 2020 2020  style=".        
+0000f820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f830: 2020 2020 6f70 6163 6974 793a 2031 3b0a      opacity: 1;.
+0000f840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f850: 2020 2020 2020 2020 2020 2020 6669 6c6c              fill
+0000f860: 3a20 6e6f 6e65 3b0a 2020 2020 2020 2020  : none;.        
 0000f870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f880: 2020 2020 2020 2020 6f70 6163 6974 793a          opacity:
-0000f890: 2031 3b0a 2020 2020 2020 2020 2020 2020   1;.            
+0000f880: 2020 2020 6669 6c6c 2d6f 7061 6369 7479      fill-opacity
+0000f890: 3a20 313b 0a20 2020 2020 2020 2020 2020  : 1;.           
 0000f8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8b0: 6669 6c6c 3a20 6e6f 6e65 3b0a 2020 2020  fill: none;.    
-0000f8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8d0: 2020 2020 2020 2020 6669 6c6c 2d6f 7061          fill-opa
-0000f8e0: 6369 7479 3a20 313b 0a20 2020 2020 2020  city: 1;.       
-0000f8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f900: 2020 2020 2066 696c 6c2d 7275 6c65 3a20       fill-rule: 
-0000f910: 6e6f 6e7a 6572 6f3b 0a20 2020 2020 2020  nonzero;.       
-0000f920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f930: 2020 2020 2073 7472 6f6b 653a 2024 6f72       stroke: $or
-0000f940: 625f 636f 6c6f 725f 3134 343b 0a20 2020  b_color_144;.   
-0000f950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f960: 2020 2020 2020 2020 2073 7472 6f6b 652d           stroke-
-0000f970: 7769 6474 683a 2031 2e34 3736 3333 3036  width: 1.4763306
-0000f980: 343b 0a20 2020 2020 2020 2020 2020 2020  4;.             
-0000f990: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f9a0: 7472 6f6b 652d 6c69 6e65 6361 703a 2062  troke-linecap: b
-0000f9b0: 7574 743b 0a20 2020 2020 2020 2020 2020  utt;.           
-0000f9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f9d0: 2073 7472 6f6b 652d 6c69 6e65 6a6f 696e   stroke-linejoin
-0000f9e0: 3a20 6d69 7465 723b 0a20 2020 2020 2020  : miter;.       
-0000f9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa00: 2020 2020 2073 7472 6f6b 652d 6d69 7465       stroke-mite
-0000fa10: 726c 696d 6974 3a20 343b 0a20 2020 2020  rlimit: 4;.     
-0000fa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa30: 2020 2020 2020 2073 7472 6f6b 652d 6461         stroke-da
-0000fa40: 7368 6172 7261 793a 206e 6f6e 653b 0a20  sharray: none;. 
-0000fa50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa60: 2020 2020 2020 2020 2020 2073 7472 6f6b             strok
-0000fa70: 652d 6f70 6163 6974 793a 2031 3b0a 2020  e-opacity: 1;.  
-0000fa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa90: 2020 2020 2020 220a 2020 2020 2020 2020        ".        
-0000faa0: 2020 2020 2020 2020 2020 2020 2f3e 0a20              />. 
-0000fab0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000fac0: 2f73 796d 626f 6c3e 0a20 2020 2020 2020  /symbol>.       
-0000fad0: 2020 2020 2020 2020 203c 7379 6d62 6f6c           <symbol
-0000fae0: 2069 643d 226f 7262 3135 3022 3e0a 2020   id="orb150">.  
-0000faf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb00: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
-0000fb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb20: 643d 224d 2031 2e31 3737 3134 3736 2c33  d="M 1.1771476,3
-0000fb30: 2e38 3336 3535 3232 2043 2034 2e36 3837  .8365522 C 4.687
-0000fb40: 3130 322c 332e 3832 3732 3933 3620 382e  102,3.8272936 8.
-0000fb50: 3139 3730 3536 322c 332e 3831 3830 3335  1970562,3.818035
-0000fb60: 3320 3131 2e37 3037 3031 312c 332e 3830  3 11.707011,3.80
-0000fb70: 3837 3736 3720 4d20 3130 2e39 3732 3537  87767 M 10.97257
-0000fb80: 392c 392e 3231 3038 3334 3120 4320 392e  9,9.2108341 C 9.
-0000fb90: 3333 3938 3030 322c 372e 3439 3634 3136  3398002,7.496416
-0000fba0: 3120 372e 3730 3730 3232 322c 352e 3738  1 7.7070222,5.78
-0000fbb0: 3139 3938 3920 362e 3037 3432 3433 342c  19989 6.0742434,
-0000fbc0: 342e 3036 3735 3831 3320 4d20 312e 3636  4.0675813 M 1.66
-0000fbd0: 3537 3431 2c39 2e32 3130 3833 3431 2043  5741,9.2108341 C
-0000fbe0: 2033 2e31 3930 3836 3536 2c37 2e33 3939   3.1908656,7.399
-0000fbf0: 3938 3131 2034 2e37 3135 3939 3034 2c35  9811 4.7159904,5
-0000fc00: 2e35 3839 3132 3739 2036 2e32 3431 3131  .5891279 6.24111
-0000fc10: 352c 332e 3737 3832 3734 3822 0a20 2020  5,3.7782748".   
-0000fc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc30: 2020 2020 2073 7479 6c65 3d22 0a20 2020       style=".   
+0000f8b0: 2066 696c 6c2d 7275 6c65 3a20 6e6f 6e7a   fill-rule: nonz
+0000f8c0: 6572 6f3b 0a20 2020 2020 2020 2020 2020  ero;.           
+0000f8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8e0: 2073 7472 6f6b 653a 2024 6f72 625f 636f   stroke: $orb_co
+0000f8f0: 6c6f 725f 3134 343b 0a20 2020 2020 2020  lor_144;.       
+0000f900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f910: 2020 2020 2073 7472 6f6b 652d 7769 6474       stroke-widt
+0000f920: 683a 2031 2e34 3736 3333 3036 343b 0a20  h: 1.47633064;. 
+0000f930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f940: 2020 2020 2020 2020 2020 2073 7472 6f6b             strok
+0000f950: 652d 6c69 6e65 6361 703a 2062 7574 743b  e-linecap: butt;
+0000f960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f970: 2020 2020 2020 2020 2020 2020 2073 7472               str
+0000f980: 6f6b 652d 6c69 6e65 6a6f 696e 3a20 6d69  oke-linejoin: mi
+0000f990: 7465 723b 0a20 2020 2020 2020 2020 2020  ter;.           
+0000f9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9b0: 2073 7472 6f6b 652d 6d69 7465 726c 696d   stroke-miterlim
+0000f9c0: 6974 3a20 343b 0a20 2020 2020 2020 2020  it: 4;.         
+0000f9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9e0: 2020 2073 7472 6f6b 652d 6461 7368 6172     stroke-dashar
+0000f9f0: 7261 793a 206e 6f6e 653b 0a20 2020 2020  ray: none;.     
+0000fa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa10: 2020 2020 2020 2073 7472 6f6b 652d 6f70         stroke-op
+0000fa20: 6163 6974 793a 2031 3b0a 2020 2020 2020  acity: 1;.      
+0000fa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa40: 2020 220a 2020 2020 2020 2020 2020 2020    ".            
+0000fa50: 2020 2020 2020 2020 2f3e 0a20 2020 2020          />.     
+0000fa60: 2020 2020 2020 2020 2020 203c 2f73 796d             </sym
+0000fa70: 626f 6c3e 0a20 2020 2020 2020 2020 2020  bol>.           
+0000fa80: 2020 2020 203c 7379 6d62 6f6c 2069 643d       <symbol id=
+0000fa90: 226f 7262 3135 3022 3e0a 2020 2020 2020  "orb150">.      
+0000faa0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+0000fab0: 6174 680a 2020 2020 2020 2020 2020 2020  ath.            
+0000fac0: 2020 2020 2020 2020 2020 2020 643d 224d              d="M
+0000fad0: 2031 2e31 3737 3134 3736 2c33 2e38 3336   1.1771476,3.836
+0000fae0: 3535 3232 2043 2034 2e36 3837 3130 322c  5522 C 4.687102,
+0000faf0: 332e 3832 3732 3933 3620 382e 3139 3730  3.8272936 8.1970
+0000fb00: 3536 322c 332e 3831 3830 3335 3320 3131  562,3.8180353 11
+0000fb10: 2e37 3037 3031 312c 332e 3830 3837 3736  .707011,3.808776
+0000fb20: 3720 4d20 3130 2e39 3732 3537 392c 392e  7 M 10.972579,9.
+0000fb30: 3231 3038 3334 3120 4320 392e 3333 3938  2108341 C 9.3398
+0000fb40: 3030 322c 372e 3439 3634 3136 3120 372e  002,7.4964161 7.
+0000fb50: 3730 3730 3232 322c 352e 3738 3139 3938  7070222,5.781998
+0000fb60: 3920 362e 3037 3432 3433 342c 342e 3036  9 6.0742434,4.06
+0000fb70: 3735 3831 3320 4d20 312e 3636 3537 3431  75813 M 1.665741
+0000fb80: 2c39 2e32 3130 3833 3431 2043 2033 2e31  ,9.2108341 C 3.1
+0000fb90: 3930 3836 3536 2c37 2e33 3939 3938 3131  908656,7.3999811
+0000fba0: 2034 2e37 3135 3939 3034 2c35 2e35 3839   4.7159904,5.589
+0000fbb0: 3132 3739 2036 2e32 3431 3131 352c 332e  1279 6.241115,3.
+0000fbc0: 3737 3832 3734 3822 0a20 2020 2020 2020  7782748".       
+0000fbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbe0: 2073 7479 6c65 3d22 0a20 2020 2020 2020   style=".       
+0000fbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc00: 2020 2020 206f 7061 6369 7479 3a20 313b       opacity: 1;
+0000fc10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fc20: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+0000fc30: 6c3a 206e 6f6e 653b 0a20 2020 2020 2020  l: none;.       
 0000fc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc50: 2020 2020 2020 2020 206f 7061 6369 7479           opacity
-0000fc60: 3a20 313b 0a20 2020 2020 2020 2020 2020  : 1;.           
+0000fc50: 2020 2020 2066 696c 6c2d 6f70 6163 6974       fill-opacit
+0000fc60: 793a 2031 3b0a 2020 2020 2020 2020 2020  y: 1;.          
 0000fc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc80: 2066 696c 6c3a 206e 6f6e 653b 0a20 2020   fill: none;.   
-0000fc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fca0: 2020 2020 2020 2020 2066 696c 6c2d 6f70           fill-op
-0000fcb0: 6163 6974 793a 2031 3b0a 2020 2020 2020  acity: 1;.      
-0000fcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fcd0: 2020 2020 2020 6669 6c6c 2d72 756c 653a        fill-rule:
-0000fce0: 206e 6f6e 7a65 726f 3b0a 2020 2020 2020   nonzero;.      
-0000fcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd00: 2020 2020 2020 7374 726f 6b65 3a20 246f        stroke: $o
-0000fd10: 7262 5f63 6f6c 6f72 5f31 3530 3b0a 2020  rb_color_150;.  
-0000fd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd30: 2020 2020 2020 2020 2020 7374 726f 6b65            stroke
-0000fd40: 2d77 6964 7468 3a20 312e 3437 3633 3330  -width: 1.476330
-0000fd50: 3634 3b0a 2020 2020 2020 2020 2020 2020  64;.            
-0000fd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd70: 7374 726f 6b65 2d6c 696e 6563 6170 3a20  stroke-linecap: 
-0000fd80: 6275 7474 3b0a 2020 2020 2020 2020 2020  butt;.          
-0000fd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fda0: 2020 7374 726f 6b65 2d6c 696e 656a 6f69    stroke-linejoi
-0000fdb0: 6e3a 206d 6974 6572 3b0a 2020 2020 2020  n: miter;.      
-0000fdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fdd0: 2020 2020 2020 7374 726f 6b65 2d6d 6974        stroke-mit
-0000fde0: 6572 6c69 6d69 743a 2034 3b0a 2020 2020  erlimit: 4;.    
-0000fdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe00: 2020 2020 2020 2020 7374 726f 6b65 2d64          stroke-d
-0000fe10: 6173 6861 7272 6179 3a20 6e6f 6e65 3b0a  asharray: none;.
-0000fe20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe30: 2020 2020 2020 2020 2020 2020 7374 726f              stro
-0000fe40: 6b65 2d6f 7061 6369 7479 3a20 313b 0a20  ke-opacity: 1;. 
-0000fe50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe60: 2020 2020 2020 2022 0a20 2020 2020 2020         ".       
-0000fe70: 2020 2020 2020 2020 2020 2020 202f 3e0a               />.
-0000fe80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe90: 3c2f 7379 6d62 6f6c 3e0a 2020 2020 2020  </symbol>.      
-0000fea0: 2020 2020 2020 2020 2020 3c73 796d 626f            <symbo
-0000feb0: 6c20 6964 3d22 6f72 6231 3830 223e 0a20  l id="orb180">. 
-0000fec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fed0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-0000fee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fef0: 2064 3d22 4d20 352e 3234 3634 3133 372c   d="M 5.2464137,
-0000ff00: 392e 3130 3234 3131 3420 4320 352e 3236  9.1024114 C 5.26
-0000ff10: 3037 3636 372c 3130 2e30 3233 3133 2034  07667,10.02313 4
-0000ff20: 2e36 3432 3430 3437 2c31 302e 3931 3137  .6424047,10.9117
-0000ff30: 3536 2033 2e37 3736 3736 3637 2c31 312e  56 3.7767667,11.
-0000ff40: 3232 3337 3335 2043 2033 2e30 3034 3330  223735 C 3.00430
-0000ff50: 3037 2c31 312e 3531 3435 3232 2032 2e30  07,11.514522 2.0
-0000ff60: 3735 3639 3037 2c31 312e 3334 3537 3133  756907,11.345713
-0000ff70: 2031 2e34 3637 3831 3637 2c31 302e 3738   1.4678167,10.78
-0000ff80: 3238 3836 2043 2030 2e38 3730 3632 3836  2886 C 0.8706286
-0000ff90: 372c 3130 2e32 3437 3436 2030 2e35 3930  7,10.24746 0.590
-0000ffa0: 3735 3036 372c 392e 3338 3138 3039 3220  75067,9.3818092 
-0000ffb0: 302e 3737 3730 3735 3637 2c38 2e35 3939  0.77707567,8.599
-0000ffc0: 3536 3134 2043 2030 2e39 3538 3732 3836  5614 C 0.9587286
-0000ffd0: 372c 372e 3739 3230 3834 3320 312e 3631  7,7.7920843 1.61
-0000ffe0: 3235 3535 372c 372e 3130 3734 3433 3420  25557,7.1074434 
-0000fff0: 322e 3431 3934 3135 372c 362e 3930 3939  2.4194157,6.9099
-00010000: 3230 3520 4320 332e 3139 3030 3632 372c  205 C 3.1900627,
-00010010: 362e 3731 3036 3820 342e 3036 3231 3331  6.71068 4.062131
-00010020: 372c 362e 3934 3534 3936 3620 342e 3631  7,6.9454966 4.61
-00010030: 3030 3837 372c 372e 3532 3831 3035 3820  00877,7.5281058 
-00010040: 4320 352e 3031 3239 3535 372c 372e 3934  C 5.0129557,7.94
-00010050: 3533 3531 3620 352e 3235 3137 3934 372c  53516 5.2517947,
-00010060: 382e 3532 3130 3139 3420 352e 3234 3634  8.5210194 5.2464
-00010070: 3133 372c 392e 3130 3234 3131 3420 7a20  137,9.1024114 z 
-00010080: 4d20 3131 2e32 3436 3431 342c 332e 3130  M 11.246414,3.10
-00010090: 3234 3132 3920 4320 3131 2e32 3630 3736  24129 C 11.26076
-000100a0: 352c 342e 3032 3331 3331 3720 3130 2e36  5,4.0231317 10.6
-000100b0: 3432 3430 342c 342e 3931 3137 3537 3420  42404,4.9117574 
-000100c0: 392e 3737 3637 3635 372c 352e 3232 3337  9.7767657,5.2237
-000100d0: 3336 3120 4320 392e 3030 3432 3939 372c  361 C 9.0042997,
-000100e0: 352e 3531 3435 3233 3820 382e 3037 3536  5.5145238 8.0756
-000100f0: 3839 372c 352e 3334 3537 3133 3520 372e  897,5.3457135 7.
-00010100: 3436 3738 3134 372c 342e 3738 3238 3837  4678147,4.782887
-00010110: 3320 4320 362e 3837 3036 3237 372c 342e  3 C 6.8706277,4.
-00010120: 3234 3734 3631 3320 362e 3539 3037 3439  2474613 6.590749
-00010130: 372c 332e 3338 3138 3120 362e 3737 3730  7,3.38181 6.7770
-00010140: 3734 372c 322e 3539 3935 3632 3420 4320  747,2.5995624 C 
-00010150: 362e 3935 3837 3236 372c 312e 3739 3230  6.9587267,1.7920
-00010160: 3835 3320 372e 3631 3235 3534 372c 312e  853 7.6125547,1.
-00010170: 3130 3734 3434 3520 382e 3431 3934 3134  1074445 8.419414
-00010180: 372c 302e 3930 3939 3231 3520 4320 392e  7,0.9099215 C 9.
-00010190: 3139 3030 3631 372c 302e 3731 3036 3831  1900617,0.710681
-000101a0: 3220 3130 2e30 3632 3133 2c30 2e39 3435  2 10.06213,0.945
-000101b0: 3439 3832 2031 302e 3631 3030 3837 2c31  4982 10.610087,1
-000101c0: 2e35 3238 3130 3733 2043 2031 312e 3031  .5281073 C 11.01
-000101d0: 3239 3535 2c31 2e39 3435 3335 3239 2031  2955,1.9453529 1
-000101e0: 312e 3235 3137 3934 2c32 2e35 3231 3032  1.251794,2.52102
-000101f0: 3036 2031 312e 3234 3634 3134 2c33 2e31  06 11.246414,3.1
-00010200: 3032 3431 3239 207a 204d 2034 2e35 3038  024129 z M 4.508
-00010210: 3234 3937 2c37 2e35 3738 3734 3320 4320  2497,7.578743 C 
-00010220: 352e 3533 3438 3533 372c 362e 3539 3435  5.5348537,6.5945
-00010230: 3232 3620 362e 3536 3134 3537 372c 352e  226 6.5614577,5.
-00010240: 3631 3033 3032 3220 372e 3538 3830 3631  6103022 7.588061
-00010250: 372c 342e 3632 3630 3831 3822 0a20 2020  7,4.6260818".   
-00010260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010270: 2020 2020 2073 7479 6c65 3d22 0a20 2020       style=".   
+0000fc80: 2020 6669 6c6c 2d72 756c 653a 206e 6f6e    fill-rule: non
+0000fc90: 7a65 726f 3b0a 2020 2020 2020 2020 2020  zero;.          
+0000fca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcb0: 2020 7374 726f 6b65 3a20 246f 7262 5f63    stroke: $orb_c
+0000fcc0: 6f6c 6f72 5f31 3530 3b0a 2020 2020 2020  olor_150;.      
+0000fcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fce0: 2020 2020 2020 7374 726f 6b65 2d77 6964        stroke-wid
+0000fcf0: 7468 3a20 312e 3437 3633 3330 3634 3b0a  th: 1.47633064;.
+0000fd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd10: 2020 2020 2020 2020 2020 2020 7374 726f              stro
+0000fd20: 6b65 2d6c 696e 6563 6170 3a20 6275 7474  ke-linecap: butt
+0000fd30: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+0000fd40: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0000fd50: 726f 6b65 2d6c 696e 656a 6f69 6e3a 206d  roke-linejoin: m
+0000fd60: 6974 6572 3b0a 2020 2020 2020 2020 2020  iter;.          
+0000fd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd80: 2020 7374 726f 6b65 2d6d 6974 6572 6c69    stroke-miterli
+0000fd90: 6d69 743a 2034 3b0a 2020 2020 2020 2020  mit: 4;.        
+0000fda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fdb0: 2020 2020 7374 726f 6b65 2d64 6173 6861      stroke-dasha
+0000fdc0: 7272 6179 3a20 6e6f 6e65 3b0a 2020 2020  rray: none;.    
+0000fdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fde0: 2020 2020 2020 2020 7374 726f 6b65 2d6f          stroke-o
+0000fdf0: 7061 6369 7479 3a20 313b 0a20 2020 2020  pacity: 1;.     
+0000fe00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe10: 2020 2022 0a20 2020 2020 2020 2020 2020     ".           
+0000fe20: 2020 2020 2020 2020 202f 3e0a 2020 2020           />.    
+0000fe30: 2020 2020 2020 2020 2020 2020 3c2f 7379              </sy
+0000fe40: 6d62 6f6c 3e0a 2020 2020 2020 2020 2020  mbol>.          
+0000fe50: 2020 2020 2020 3c73 796d 626f 6c20 6964        <symbol id
+0000fe60: 3d22 6f72 6231 3830 223e 0a20 2020 2020  ="orb180">.     
+0000fe70: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000fe80: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
+0000fe90: 2020 2020 2020 2020 2020 2020 2064 3d22               d="
+0000fea0: 4d20 352e 3234 3634 3133 372c 392e 3130  M 5.2464137,9.10
+0000feb0: 3234 3131 3420 4320 352e 3236 3037 3636  24114 C 5.260766
+0000fec0: 372c 3130 2e30 3233 3133 2034 2e36 3432  7,10.02313 4.642
+0000fed0: 3430 3437 2c31 302e 3931 3137 3536 2033  4047,10.911756 3
+0000fee0: 2e37 3736 3736 3637 2c31 312e 3232 3337  .7767667,11.2237
+0000fef0: 3335 2043 2033 2e30 3034 3330 3037 2c31  35 C 3.0043007,1
+0000ff00: 312e 3531 3435 3232 2032 2e30 3735 3639  1.514522 2.07569
+0000ff10: 3037 2c31 312e 3334 3537 3133 2031 2e34  07,11.345713 1.4
+0000ff20: 3637 3831 3637 2c31 302e 3738 3238 3836  678167,10.782886
+0000ff30: 2043 2030 2e38 3730 3632 3836 372c 3130   C 0.87062867,10
+0000ff40: 2e32 3437 3436 2030 2e35 3930 3735 3036  .24746 0.5907506
+0000ff50: 372c 392e 3338 3138 3039 3220 302e 3737  7,9.3818092 0.77
+0000ff60: 3730 3735 3637 2c38 2e35 3939 3536 3134  707567,8.5995614
+0000ff70: 2043 2030 2e39 3538 3732 3836 372c 372e   C 0.95872867,7.
+0000ff80: 3739 3230 3834 3320 312e 3631 3235 3535  7920843 1.612555
+0000ff90: 372c 372e 3130 3734 3433 3420 322e 3431  7,7.1074434 2.41
+0000ffa0: 3934 3135 372c 362e 3930 3939 3230 3520  94157,6.9099205 
+0000ffb0: 4320 332e 3139 3030 3632 372c 362e 3731  C 3.1900627,6.71
+0000ffc0: 3036 3820 342e 3036 3231 3331 372c 362e  068 4.0621317,6.
+0000ffd0: 3934 3534 3936 3620 342e 3631 3030 3837  9454966 4.610087
+0000ffe0: 372c 372e 3532 3831 3035 3820 4320 352e  7,7.5281058 C 5.
+0000fff0: 3031 3239 3535 372c 372e 3934 3533 3531  0129557,7.945351
+00010000: 3620 352e 3235 3137 3934 372c 382e 3532  6 5.2517947,8.52
+00010010: 3130 3139 3420 352e 3234 3634 3133 372c  10194 5.2464137,
+00010020: 392e 3130 3234 3131 3420 7a20 4d20 3131  9.1024114 z M 11
+00010030: 2e32 3436 3431 342c 332e 3130 3234 3132  .246414,3.102412
+00010040: 3920 4320 3131 2e32 3630 3736 352c 342e  9 C 11.260765,4.
+00010050: 3032 3331 3331 3720 3130 2e36 3432 3430  0231317 10.64240
+00010060: 342c 342e 3931 3137 3537 3420 392e 3737  4,4.9117574 9.77
+00010070: 3637 3635 372c 352e 3232 3337 3336 3120  67657,5.2237361 
+00010080: 4320 392e 3030 3432 3939 372c 352e 3531  C 9.0042997,5.51
+00010090: 3435 3233 3820 382e 3037 3536 3839 372c  45238 8.0756897,
+000100a0: 352e 3334 3537 3133 3520 372e 3436 3738  5.3457135 7.4678
+000100b0: 3134 372c 342e 3738 3238 3837 3320 4320  147,4.7828873 C 
+000100c0: 362e 3837 3036 3237 372c 342e 3234 3734  6.8706277,4.2474
+000100d0: 3631 3320 362e 3539 3037 3439 372c 332e  613 6.5907497,3.
+000100e0: 3338 3138 3120 362e 3737 3730 3734 372c  38181 6.7770747,
+000100f0: 322e 3539 3935 3632 3420 4320 362e 3935  2.5995624 C 6.95
+00010100: 3837 3236 372c 312e 3739 3230 3835 3320  87267,1.7920853 
+00010110: 372e 3631 3235 3534 372c 312e 3130 3734  7.6125547,1.1074
+00010120: 3434 3520 382e 3431 3934 3134 372c 302e  445 8.4194147,0.
+00010130: 3930 3939 3231 3520 4320 392e 3139 3030  9099215 C 9.1900
+00010140: 3631 372c 302e 3731 3036 3831 3220 3130  617,0.7106812 10
+00010150: 2e30 3632 3133 2c30 2e39 3435 3439 3832  .06213,0.9454982
+00010160: 2031 302e 3631 3030 3837 2c31 2e35 3238   10.610087,1.528
+00010170: 3130 3733 2043 2031 312e 3031 3239 3535  1073 C 11.012955
+00010180: 2c31 2e39 3435 3335 3239 2031 312e 3235  ,1.9453529 11.25
+00010190: 3137 3934 2c32 2e35 3231 3032 3036 2031  1794,2.5210206 1
+000101a0: 312e 3234 3634 3134 2c33 2e31 3032 3431  1.246414,3.10241
+000101b0: 3239 207a 204d 2034 2e35 3038 3234 3937  29 z M 4.5082497
+000101c0: 2c37 2e35 3738 3734 3320 4320 352e 3533  ,7.578743 C 5.53
+000101d0: 3438 3533 372c 362e 3539 3435 3232 3620  48537,6.5945226 
+000101e0: 362e 3536 3134 3537 372c 352e 3631 3033  6.5614577,5.6103
+000101f0: 3032 3220 372e 3538 3830 3631 372c 342e  022 7.5880617,4.
+00010200: 3632 3630 3831 3822 0a20 2020 2020 2020  6260818".       
+00010210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010220: 2073 7479 6c65 3d22 0a20 2020 2020 2020   style=".       
+00010230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010240: 2020 2020 206f 7061 6369 7479 3a20 313b       opacity: 1;
+00010250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010260: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+00010270: 6c3a 206e 6f6e 653b 0a20 2020 2020 2020  l: none;.       
 00010280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010290: 2020 2020 2020 2020 206f 7061 6369 7479           opacity
-000102a0: 3a20 313b 0a20 2020 2020 2020 2020 2020  : 1;.           
+00010290: 2020 2020 2066 696c 6c2d 6f70 6163 6974       fill-opacit
+000102a0: 793a 2031 3b0a 2020 2020 2020 2020 2020  y: 1;.          
 000102b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102c0: 2066 696c 6c3a 206e 6f6e 653b 0a20 2020   fill: none;.   
-000102d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102e0: 2020 2020 2020 2020 2066 696c 6c2d 6f70           fill-op
-000102f0: 6163 6974 793a 2031 3b0a 2020 2020 2020  acity: 1;.      
-00010300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010310: 2020 2020 2020 6669 6c6c 2d72 756c 653a        fill-rule:
-00010320: 206e 6f6e 7a65 726f 3b0a 2020 2020 2020   nonzero;.      
-00010330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010340: 2020 2020 2020 7374 726f 6b65 3a20 246f        stroke: $o
-00010350: 7262 5f63 6f6c 6f72 5f31 3830 3b0a 2020  rb_color_180;.  
-00010360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010370: 2020 2020 2020 2020 2020 7374 726f 6b65            stroke
-00010380: 2d77 6964 7468 3a20 312e 3437 3633 3330  -width: 1.476330
-00010390: 3634 3b0a 2020 2020 2020 2020 2020 2020  64;.            
-000103a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103b0: 7374 726f 6b65 2d6c 696e 6563 6170 3a20  stroke-linecap: 
-000103c0: 6275 7474 3b0a 2020 2020 2020 2020 2020  butt;.          
-000103d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103e0: 2020 7374 726f 6b65 2d6c 696e 656a 6f69    stroke-linejoi
-000103f0: 6e3a 206d 6974 6572 3b0a 2020 2020 2020  n: miter;.      
-00010400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010410: 2020 2020 2020 7374 726f 6b65 2d6d 6974        stroke-mit
-00010420: 6572 6c69 6d69 743a 2034 3b0a 2020 2020  erlimit: 4;.    
-00010430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010440: 2020 2020 2020 2020 7374 726f 6b65 2d64          stroke-d
-00010450: 6173 6861 7272 6179 3a20 6e6f 6e65 3b0a  asharray: none;.
-00010460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010470: 2020 2020 2020 2020 2020 2020 7374 726f              stro
-00010480: 6b65 2d6f 7061 6369 7479 3a20 313b 0a20  ke-opacity: 1;. 
-00010490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104a0: 2020 2020 2020 2022 0a20 2020 2020 2020         ".       
-000104b0: 2020 2020 2020 2020 2020 2020 202f 3e0a               />.
-000104c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104d0: 3c2f 7379 6d62 6f6c 3e0a 2020 2020 2020  </symbol>.      
-000104e0: 2020 2020 2020 2020 2020 3c21 2d2d 2072            <!-- r
-000104f0: 6574 726f 6772 6164 6520 7379 6d62 6f6c  etrograde symbol
-00010500: 2028 3132 7831 3229 202d 2d3e 0a20 2020   (12x12) -->.   
-00010510: 2020 2020 2020 2020 2020 2020 203c 7379               <sy
-00010520: 6d62 6f6c 2069 643d 2272 6574 726f 6772  mbol id="retrogr
-00010530: 6164 6522 3e0a 2020 2020 2020 2020 2020  ade">.          
-00010540: 2020 2020 2020 2020 2020 3c70 6174 680a            <path.
-00010550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010560: 2020 2020 2020 2020 643d 224d 2035 2e31          d="M 5.1
-00010570: 3639 3530 3839 2c30 2e30 3635 3134 3330  695089,0.0651430
-00010580: 3720 4320 332e 3735 3937 3938 392c 302e  7 C 3.7597989,0.
-00010590: 3231 3539 3732 3037 2032 2e33 3331 3733  21597207 2.33173
-000105a0: 3439 2c30 2e33 3331 3439 3030 3720 302e  49,0.33149007 0.
-000105b0: 3931 3335 3831 3931 2c30 2e32 3335 3133  91358191,0.23513
-000105c0: 3130 3720 4320 312e 3534 3930 3332 392c  107 C 1.5490329,
-000105d0: 302e 3831 3930 3232 3037 2031 2e34 3032  0.81902207 1.402
-000105e0: 3438 3439 2c31 2e37 3130 3030 3131 2031  4849,1.7100011 1
-000105f0: 2e34 3232 3833 3739 2c32 2e34 3730 3034  .4228379,2.47004
-00010600: 3331 2043 2031 2e34 3137 3431 3539 2c35  31 C 1.4174159,5
-00010610: 2e32 3137 3434 3831 2031 2e34 3333 3737  .2174481 1.43377
-00010620: 3039 2c37 2e39 3635 3237 3331 2031 2e34  09,7.9652731 1.4
-00010630: 3134 3530 3139 2c31 302e 3731 3234 3131  145019,10.712411
-00010640: 2043 2031 2e35 3134 3934 3039 2c31 312e   C 1.5149409,11.
-00010650: 3137 3038 3438 2030 2e39 3637 3939 3739  170848 0.9679979
-00010660: 312c 3131 2e38 3334 3437 3120 302e 3930  1,11.834471 0.90
-00010670: 3238 3436 3931 2c31 312e 3936 3433 3032  284691,11.964302
-00010680: 2043 2031 2e39 3937 3638 3839 2c31 312e   C 1.9976889,11.
-00010690: 3936 3433 3032 2033 2e30 3932 3532 3939  964302 3.0925299
-000106a0: 2c31 312e 3936 3433 3032 2034 2e31 3837  ,11.964302 4.187
-000106b0: 3337 3139 2c31 312e 3936 3433 3032 2043  3719,11.964302 C
-000106c0: 2033 2e36 3031 3834 3339 2c31 312e 3537   3.6018439,11.57
-000106d0: 3739 3735 2033 2e36 3531 3039 3239 2c31  7975 3.6510929,1
-000106e0: 302e 3832 3030 3334 2033 2e36 3431 3733  0.820034 3.64173
-000106f0: 3939 2c31 302e 3231 3938 3338 2043 2033  99,10.219838 C 3
-00010700: 2e36 3431 3733 3939 2c38 2e38 3937 3436  .6417399,8.89746
-00010710: 3031 2033 2e36 3431 3733 3939 2c37 2e35  01 3.6417399,7.5
-00010720: 3735 3038 3331 2033 2e36 3431 3733 3939  750831 3.6417399
-00010730: 2c36 2e32 3532 3730 3531 2043 2034 2e35  ,6.2527051 C 4.5
-00010740: 3032 3632 3539 2c37 2e33 3937 3239 3131  026259,7.3972911
-00010750: 2035 2e33 3633 3531 3039 2c38 2e35 3431   5.3635109,8.541
-00010760: 3837 3731 2036 2e32 3234 3339 3539 2c39  8771 6.2243959,9
-00010770: 2e36 3836 3436 3331 2043 2035 2e36 3033  .6864631 C 5.603
-00010780: 3036 3939 2c31 302e 3031 3330 3439 2035  0699,10.013049 5
-00010790: 2e30 3732 3134 3339 2c31 302e 3439 3733  .0721439,10.4973
-000107a0: 3534 2034 2e33 3639 3234 3839 2c31 302e  54 4.3692489,10.
-000107b0: 3637 3233 3933 2043 2034 2e35 3735 3337  672393 C 4.57537
-000107c0: 3639 2c31 302e 3935 3537 3036 2034 2e37  69,10.955706 4.7
-000107d0: 3831 3530 3339 2c31 312e 3233 3930 3220  815039,11.23902 
-000107e0: 342e 3938 3736 3331 392c 3131 2e35 3232  4.9876319,11.522
-000107f0: 3333 3320 4320 352e 3439 3339 3231 392c  333 C 5.4939219,
-00010800: 3131 2e30 3138 3033 3620 362e 3134 3236  11.018036 6.1426
-00010810: 3338 392c 3130 2e36 3732 3231 3820 362e  389,10.672218 6.
-00010820: 3733 3336 3532 392c 3130 2e32 3634 3432  7336529,10.26442
-00010830: 3120 4320 372e 3338 3937 3033 392c 3131  1 C 7.3897039,11
-00010840: 2e32 3136 3931 3220 382e 3436 3937 3437  .216912 8.469747
-00010850: 392c 3132 2e30 3438 3339 3220 392e 3734  9,12.048392 9.74
-00010860: 3139 3339 392c 3132 2e30 3131 3537 3920  19399,12.011579 
-00010870: 4320 3130 2e31 3433 3630 332c 3132 2e30  C 10.143603,12.0
-00010880: 3032 3139 3920 3131 2e30 3637 3639 312c  02199 11.067691,
-00010890: 3131 2e38 3835 3832 3420 3131 2e30 3633  11.885824 11.063
-000108a0: 3737 352c 3131 2e36 3736 3037 3520 4320  775,11.676075 C 
-000108b0: 392e 3930 3034 3936 392c 3131 2e31 3238  9.9004969,11.128
-000108c0: 3035 3420 392e 3030 3138 3834 392c 3130  054 9.0018849,10
-000108d0: 2e31 3739 3038 3520 382e 3430 3639 3232  .179085 8.406922
-000108e0: 392c 392e 3130 3835 3034 3120 4320 382e  9,9.1085041 C 8.
-000108f0: 3936 3730 3433 392c 382e 3637 3536 3634  9670439,8.675664
-00010900: 3120 392e 3530 3536 3238 392c 382e 3138  1 9.5056289,8.18
-00010910: 3730 3035 3120 3130 2e31 3737 3338 322c  70051 10.177382,
-00010920: 372e 3930 3836 3733 3120 4320 3130 2e34  7.9086731 C 10.4
-00010930: 3139 3838 312c 372e 3836 3631 3530 3120  19881,7.8661501 
-00010940: 3130 2e30 3331 3636 382c 372e 3537 3633  10.031668,7.5763
-00010950: 3537 3120 392e 3938 3135 3033 392c 372e  571 9.9815039,7.
-00010960: 3431 3930 3935 3120 4320 392e 3738 3936  4190951 C 9.7896
-00010970: 3038 392c 362e 3930 3632 3933 3120 392e  089,6.9062931 9.
-00010980: 3632 3134 3337 392c 372e 3436 3934 3636  6214379,7.469466
-00010990: 3120 392e 3239 3530 3833 392c 372e 3632  1 9.2950839,7.62
-000109a0: 3339 3435 3120 4320 382e 3834 3533 3938  39451 C 8.845398
-000109b0: 392c 372e 3839 3237 3638 3120 382e 3330  9,7.8927681 8.30
-000109c0: 3738 3833 392c 382e 3336 3436 3031 3120  78839,8.3646011 
-000109d0: 372e 3836 3134 3435 392c 382e 3434 3534  7.8614459,8.4454
-000109e0: 3335 3120 4320 372e 3235 3531 3336 392c  351 C 7.2551369,
-000109f0: 372e 3538 3938 3637 3120 362e 3634 3838  7.5898671 6.6488
-00010a00: 3237 392c 362e 3733 3432 3939 3120 362e  279,6.7342991 6.
-00010a10: 3034 3235 3139 392c 352e 3837 3837 3332  0425199,5.878732
-00010a20: 3120 4320 372e 3234 3531 3933 392c 352e  1 C 7.2451939,5.
-00010a30: 3631 3734 3335 3120 382e 3538 3237 3833  6174351 8.582783
-00010a40: 392c 352e 3038 3533 3839 3120 392e 3037  9,5.0853891 9.07
-00010a50: 3034 3430 392c 332e 3933 3638 3938 3120  04409,3.9368981 
-00010a60: 4320 392e 3430 3633 3133 392c 332e 3131  C 9.4063139,3.11
-00010a70: 3230 3231 3120 392e 3236 3337 3333 392c  20211 9.2637339,
-00010a80: 322e 3136 3637 3933 3120 382e 3931 3037  2.1667931 8.9107
-00010a90: 3838 392c 312e 3337 3334 3730 3120 4320  889,1.3734701 C 
-00010aa0: 382e 3136 3834 3836 392c 302e 3431 3039  8.1684869,0.4109
-00010ab0: 3131 3037 2036 2e38 3639 3230 3439 2c2d  1107 6.8692049,-
-00010ac0: 302e 3037 3234 3531 3933 3120 352e 3631  0.072451931 5.61
-00010ad0: 3939 3732 392c 302e 3032 3531 3036 3037  99729,0.02510607
-00010ae0: 2043 2035 2e34 3639 3332 3739 2c30 2e30   C 5.4693279,0.0
-00010af0: 3332 3837 3230 3720 352e 3331 3930 3531  3287207 5.319051
-00010b00: 392c 302e 3034 3635 3130 3037 2035 2e31  9,0.04651007 5.1
-00010b10: 3639 3530 3839 2c30 2e30 3635 3134 3330  695089,0.0651430
-00010b20: 3720 4c20 352e 3136 3935 3038 392c 302e  7 L 5.1695089,0.
-00010b30: 3036 3531 3433 3037 207a 204d 2034 2e30  06514307 z M 4.0
-00010b40: 3035 3439 3439 2c30 2e39 3833 3037 3830  054949,0.9830780
-00010b50: 3620 4320 342e 3932 3734 3230 392c 302e  6 C 4.9274209,0.
-00010b60: 3837 3531 3630 3037 2036 2e30 3735 3238  87516007 6.07528
-00010b70: 3339 2c30 2e39 3536 3539 3430 3620 362e  39,0.95659406 6.
-00010b80: 3631 3139 3436 392c 312e 3737 3639 3832  6119469,1.776982
-00010b90: 3120 4320 372e 3139 3935 3438 392c 322e  1 C 7.1995489,2.
-00010ba0: 3734 3336 3233 3120 362e 3937 3731 3737  7436231 6.977177
-00010bb0: 392c 342e 3032 3737 3234 3120 362e 3233  9,4.0277241 6.23
-00010bc0: 3838 3835 392c 342e 3836 3934 3030 3120  88859,4.8694001 
-00010bd0: 4320 352e 3630 3533 3238 392c 352e 3535  C 5.6053289,5.55
-00010be0: 3439 3033 3120 342e 3535 3231 3035 392c  49031 4.5521059,
-00010bf0: 352e 3637 3830 3737 3120 332e 3634 3137  5.6780771 3.6417
-00010c00: 3339 392c 352e 3537 3237 3533 3120 4320  399,5.5727531 C 
-00010c10: 332e 3634 3137 3339 392c 342e 3036 3535  3.6417399,4.0655
-00010c20: 3237 3120 332e 3634 3137 3339 392c 322e  271 3.6417399,2.
-00010c30: 3535 3833 3030 3120 332e 3634 3137 3339  5583001 3.641739
-00010c40: 392c 312e 3035 3130 3733 3120 4320 332e  9,1.0510731 C 3.
-00010c50: 3736 3239 3931 392c 312e 3032 3834 3038  7629919,1.028408
-00010c60: 3120 332e 3838 3432 3432 392c 312e 3030  1 3.8842429,1.00
-00010c70: 3537 3433 3120 342e 3030 3534 3934 392c  57431 4.0054949,
-00010c80: 302e 3938 3330 3738 3036 207a 220a 2020  0.98307806 z".  
-00010c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ca0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-00010cb0: 6c3a 2024 7061 7065 725f 636f 6c6f 725f  l: $paper_color_
-00010cc0: 3022 0a20 2020 2020 2020 2020 2020 2020  0".             
-00010cd0: 2020 2020 2020 202f 3e0a 2020 2020 2020         />.      
-00010ce0: 2020 2020 2020 2020 2020 3c2f 7379 6d62            </symb
-00010cf0: 6f6c 3e0a 2020 2020 2020 2020 2020 2020  ol>.            
-00010d00: 2020 2020 3c67 2074 7261 6e73 666f 726d      <g transform
-00010d10: 3d22 7472 616e 736c 6174 6528 3530 2c35  ="translate(50,5
-00010d20: 3029 223e 0a20 2020 2020 2020 2020 2020  0)">.           
-00010d30: 2020 2020 2020 2020 203c 6720 7472 616e           <g tran
-00010d40: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
-00010d50: 2824 6369 7263 6c65 582c 2463 6972 636c  ($circleX,$circl
-00010d60: 6559 2922 3e0a 2020 2020 2020 2020 2020  eY)">.          
-00010d70: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
-00010d80: 2d2d 205a 6f64 6961 6320 2d2d 3e24 6d61  -- Zodiac -->$ma
-00010d90: 6b65 5a6f 6469 6163 203c 212d 2d20 4669  keZodiac <!-- Fi
-00010da0: 7273 7420 4369 7263 6c65 202d 2d3e 0a20  rst Circle -->. 
-00010db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010dc0: 2020 2020 2020 203c 6369 7263 6c65 2024         <circle $
-00010dd0: 6331 2073 7479 6c65 3d22 2463 3173 7479  c1 style="$c1sty
-00010de0: 6c65 2220 2f3e 0a20 2020 2020 2020 2020  le" />.         
-00010df0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00010e00: 212d 2d20 5365 636f 6e64 2043 6972 636c  !-- Second Circl
-00010e10: 6520 2d2d 3e0a 2020 2020 2020 2020 2020  e -->.          
-00010e20: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
-00010e30: 6972 636c 650a 2020 2020 2020 2020 2020  ircle.          
-00010e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e50: 2020 2463 3220 7374 796c 653d 2224 6332    $c2 style="$c2
-00010e60: 7374 796c 6522 202f 3e0a 2020 2020 2020  style" />.      
-00010e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e80: 2020 3c21 2d2d 2054 6869 7264 2043 6972    <!-- Third Cir
-00010e90: 636c 6520 2d2d 3e0a 2020 2020 2020 2020  cle -->.        
-00010ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010eb0: 3c63 6972 636c 6520 2463 3320 7374 796c  <circle $c3 styl
-00010ec0: 653d 2224 6333 7374 796c 6522 202f 3e0a  e="$c3style" />.
-00010ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ee0: 2020 2020 2020 2020 3c21 2d2d 2054 7261          <!-- Tra
-00010ef0: 6e73 6974 5269 6e67 202d 2d3e 2474 7261  nsitRing -->$tra
-00010f00: 6e73 6974 5269 6e67 203c 212d 2d20 4465  nsitRing <!-- De
-00010f10: 6772 6565 2052 696e 6720 2d2d 3e24 6465  gree Ring -->$de
-00010f20: 6772 6565 5269 6e67 203c 212d 2d20 486f  greeRing <!-- Ho
-00010f30: 7573 6573 202d 2d3e 0a20 2020 2020 2020  uses -->.       
-00010f40: 2020 2020 2020 2020 2020 2020 2024 6d61               $ma
-00010f50: 6b65 486f 7573 6573 0a20 2020 2020 2020  keHouses.       
-00010f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f70: 203c 212d 2d20 506c 616e 6574 7320 2d2d   <!-- Planets --
-00010f80: 3e24 6d61 6b65 506c 616e 6574 7320 3c21  >$makePlanets <!
-00010f90: 2d2d 2041 7370 6563 7473 202d 2d3e 246d  -- Aspects -->$m
-00010fa0: 616b 6541 7370 6563 7473 203c 2f67 3e0a  akeAspects </g>.
-00010fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fc0: 2020 2020 3c21 2d2d 206d 616b 6550 6174      <!-- makePat
-00010fd0: 7465 726e 7320 2d2d 3e24 6d61 6b65 5061  terns -->$makePa
-00010fe0: 7474 6572 6e73 203c 212d 2d20 4173 7065  tterns <!-- Aspe
-00010ff0: 6374 4772 6964 202d 2d3e 0a20 2020 2020  ctGrid -->.     
-00011000: 2020 2020 2020 2020 2020 2020 2020 2024                 $
-00011010: 6d61 6b65 4173 7065 6374 4772 6964 0a20  makeAspectGrid. 
-00011020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011030: 2020 203c 212d 2d20 456c 656d 656e 7473     <!-- Elements
-00011040: 202d 2d3e 246d 616b 6545 6c65 6d65 6e74   -->$makeElement
-00011050: 7320 3c21 2d2d 2050 6c61 6e65 7420 4772  s <!-- Planet Gr
-00011060: 6964 202d 2d3e 246d 616b 6550 6c61 6e65  id -->$makePlane
-00011070: 7447 7269 6420 3c21 2d2d 2048 6f75 7365  tGrid <!-- House
-00011080: 7320 4772 6964 202d 2d3e 0a20 2020 2020  s Grid -->.     
-00011090: 2020 2020 2020 2020 2020 2020 2020 2024                 $
-000110a0: 6d61 6b65 486f 7573 6573 4772 6964 0a20  makeHousesGrid. 
-000110b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000110c0: 2f67 3e0a 2020 2020 2020 2020 2020 2020  /g>.            
-000110d0: 3c2f 673e 0a20 2020 2020 2020 203c 2f67  </g>.        </g
-000110e0: 3e0a 2020 2020 3c2f 673e 0a3c 2f73 7667  >.    </g>.</svg
-000110f0: 3e0a                                     >.
+000102c0: 2020 6669 6c6c 2d72 756c 653a 206e 6f6e    fill-rule: non
+000102d0: 7a65 726f 3b0a 2020 2020 2020 2020 2020  zero;.          
+000102e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102f0: 2020 7374 726f 6b65 3a20 246f 7262 5f63    stroke: $orb_c
+00010300: 6f6c 6f72 5f31 3830 3b0a 2020 2020 2020  olor_180;.      
+00010310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010320: 2020 2020 2020 7374 726f 6b65 2d77 6964        stroke-wid
+00010330: 7468 3a20 312e 3437 3633 3330 3634 3b0a  th: 1.47633064;.
+00010340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010350: 2020 2020 2020 2020 2020 2020 7374 726f              stro
+00010360: 6b65 2d6c 696e 6563 6170 3a20 6275 7474  ke-linecap: butt
+00010370: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+00010380: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00010390: 726f 6b65 2d6c 696e 656a 6f69 6e3a 206d  roke-linejoin: m
+000103a0: 6974 6572 3b0a 2020 2020 2020 2020 2020  iter;.          
+000103b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103c0: 2020 7374 726f 6b65 2d6d 6974 6572 6c69    stroke-miterli
+000103d0: 6d69 743a 2034 3b0a 2020 2020 2020 2020  mit: 4;.        
+000103e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103f0: 2020 2020 7374 726f 6b65 2d64 6173 6861      stroke-dasha
+00010400: 7272 6179 3a20 6e6f 6e65 3b0a 2020 2020  rray: none;.    
+00010410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010420: 2020 2020 2020 2020 7374 726f 6b65 2d6f          stroke-o
+00010430: 7061 6369 7479 3a20 313b 0a20 2020 2020  pacity: 1;.     
+00010440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010450: 2020 2022 0a20 2020 2020 2020 2020 2020     ".           
+00010460: 2020 2020 2020 2020 202f 3e0a 2020 2020           />.    
+00010470: 2020 2020 2020 2020 2020 2020 3c2f 7379              </sy
+00010480: 6d62 6f6c 3e0a 2020 2020 2020 2020 2020  mbol>.          
+00010490: 2020 2020 2020 3c21 2d2d 2072 6574 726f        <!-- retro
+000104a0: 6772 6164 6520 7379 6d62 6f6c 2028 3132  grade symbol (12
+000104b0: 7831 3229 202d 2d3e 0a20 2020 2020 2020  x12) -->.       
+000104c0: 2020 2020 2020 2020 203c 7379 6d62 6f6c           <symbol
+000104d0: 2069 643d 2272 6574 726f 6772 6164 6522   id="retrograde"
+000104e0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000104f0: 2020 2020 2020 3c70 6174 680a 2020 2020        <path.    
+00010500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010510: 2020 2020 643d 224d 2035 2e31 3639 3530      d="M 5.16950
+00010520: 3839 2c30 2e30 3635 3134 3330 3720 4320  89,0.06514307 C 
+00010530: 332e 3735 3937 3938 392c 302e 3231 3539  3.7597989,0.2159
+00010540: 3732 3037 2032 2e33 3331 3733 3439 2c30  7207 2.3317349,0
+00010550: 2e33 3331 3439 3030 3720 302e 3931 3335  .33149007 0.9135
+00010560: 3831 3931 2c30 2e32 3335 3133 3130 3720  8191,0.23513107 
+00010570: 4320 312e 3534 3930 3332 392c 302e 3831  C 1.5490329,0.81
+00010580: 3930 3232 3037 2031 2e34 3032 3438 3439  902207 1.4024849
+00010590: 2c31 2e37 3130 3030 3131 2031 2e34 3232  ,1.7100011 1.422
+000105a0: 3833 3739 2c32 2e34 3730 3034 3331 2043  8379,2.4700431 C
+000105b0: 2031 2e34 3137 3431 3539 2c35 2e32 3137   1.4174159,5.217
+000105c0: 3434 3831 2031 2e34 3333 3737 3039 2c37  4481 1.4337709,7
+000105d0: 2e39 3635 3237 3331 2031 2e34 3134 3530  .9652731 1.41450
+000105e0: 3139 2c31 302e 3731 3234 3131 2043 2031  19,10.712411 C 1
+000105f0: 2e35 3134 3934 3039 2c31 312e 3137 3038  .5149409,11.1708
+00010600: 3438 2030 2e39 3637 3939 3739 312c 3131  48 0.96799791,11
+00010610: 2e38 3334 3437 3120 302e 3930 3238 3436  .834471 0.902846
+00010620: 3931 2c31 312e 3936 3433 3032 2043 2031  91,11.964302 C 1
+00010630: 2e39 3937 3638 3839 2c31 312e 3936 3433  .9976889,11.9643
+00010640: 3032 2033 2e30 3932 3532 3939 2c31 312e  02 3.0925299,11.
+00010650: 3936 3433 3032 2034 2e31 3837 3337 3139  964302 4.1873719
+00010660: 2c31 312e 3936 3433 3032 2043 2033 2e36  ,11.964302 C 3.6
+00010670: 3031 3834 3339 2c31 312e 3537 3739 3735  018439,11.577975
+00010680: 2033 2e36 3531 3039 3239 2c31 302e 3832   3.6510929,10.82
+00010690: 3030 3334 2033 2e36 3431 3733 3939 2c31  0034 3.6417399,1
+000106a0: 302e 3231 3938 3338 2043 2033 2e36 3431  0.219838 C 3.641
+000106b0: 3733 3939 2c38 2e38 3937 3436 3031 2033  7399,8.8974601 3
+000106c0: 2e36 3431 3733 3939 2c37 2e35 3735 3038  .6417399,7.57508
+000106d0: 3331 2033 2e36 3431 3733 3939 2c36 2e32  31 3.6417399,6.2
+000106e0: 3532 3730 3531 2043 2034 2e35 3032 3632  527051 C 4.50262
+000106f0: 3539 2c37 2e33 3937 3239 3131 2035 2e33  59,7.3972911 5.3
+00010700: 3633 3531 3039 2c38 2e35 3431 3837 3731  635109,8.5418771
+00010710: 2036 2e32 3234 3339 3539 2c39 2e36 3836   6.2243959,9.686
+00010720: 3436 3331 2043 2035 2e36 3033 3036 3939  4631 C 5.6030699
+00010730: 2c31 302e 3031 3330 3439 2035 2e30 3732  ,10.013049 5.072
+00010740: 3134 3339 2c31 302e 3439 3733 3534 2034  1439,10.497354 4
+00010750: 2e33 3639 3234 3839 2c31 302e 3637 3233  .3692489,10.6723
+00010760: 3933 2043 2034 2e35 3735 3337 3639 2c31  93 C 4.5753769,1
+00010770: 302e 3935 3537 3036 2034 2e37 3831 3530  0.955706 4.78150
+00010780: 3339 2c31 312e 3233 3930 3220 342e 3938  39,11.23902 4.98
+00010790: 3736 3331 392c 3131 2e35 3232 3333 3320  76319,11.522333 
+000107a0: 4320 352e 3439 3339 3231 392c 3131 2e30  C 5.4939219,11.0
+000107b0: 3138 3033 3620 362e 3134 3236 3338 392c  18036 6.1426389,
+000107c0: 3130 2e36 3732 3231 3820 362e 3733 3336  10.672218 6.7336
+000107d0: 3532 392c 3130 2e32 3634 3432 3120 4320  529,10.264421 C 
+000107e0: 372e 3338 3937 3033 392c 3131 2e32 3136  7.3897039,11.216
+000107f0: 3931 3220 382e 3436 3937 3437 392c 3132  912 8.4697479,12
+00010800: 2e30 3438 3339 3220 392e 3734 3139 3339  .048392 9.741939
+00010810: 392c 3132 2e30 3131 3537 3920 4320 3130  9,12.011579 C 10
+00010820: 2e31 3433 3630 332c 3132 2e30 3032 3139  .143603,12.00219
+00010830: 3920 3131 2e30 3637 3639 312c 3131 2e38  9 11.067691,11.8
+00010840: 3835 3832 3420 3131 2e30 3633 3737 352c  85824 11.063775,
+00010850: 3131 2e36 3736 3037 3520 4320 392e 3930  11.676075 C 9.90
+00010860: 3034 3936 392c 3131 2e31 3238 3035 3420  04969,11.128054 
+00010870: 392e 3030 3138 3834 392c 3130 2e31 3739  9.0018849,10.179
+00010880: 3038 3520 382e 3430 3639 3232 392c 392e  085 8.4069229,9.
+00010890: 3130 3835 3034 3120 4320 382e 3936 3730  1085041 C 8.9670
+000108a0: 3433 392c 382e 3637 3536 3634 3120 392e  439,8.6756641 9.
+000108b0: 3530 3536 3238 392c 382e 3138 3730 3035  5056289,8.187005
+000108c0: 3120 3130 2e31 3737 3338 322c 372e 3930  1 10.177382,7.90
+000108d0: 3836 3733 3120 4320 3130 2e34 3139 3838  86731 C 10.41988
+000108e0: 312c 372e 3836 3631 3530 3120 3130 2e30  1,7.8661501 10.0
+000108f0: 3331 3636 382c 372e 3537 3633 3537 3120  31668,7.5763571 
+00010900: 392e 3938 3135 3033 392c 372e 3431 3930  9.9815039,7.4190
+00010910: 3935 3120 4320 392e 3738 3936 3038 392c  951 C 9.7896089,
+00010920: 362e 3930 3632 3933 3120 392e 3632 3134  6.9062931 9.6214
+00010930: 3337 392c 372e 3436 3934 3636 3120 392e  379,7.4694661 9.
+00010940: 3239 3530 3833 392c 372e 3632 3339 3435  2950839,7.623945
+00010950: 3120 4320 382e 3834 3533 3938 392c 372e  1 C 8.8453989,7.
+00010960: 3839 3237 3638 3120 382e 3330 3738 3833  8927681 8.307883
+00010970: 392c 382e 3336 3436 3031 3120 372e 3836  9,8.3646011 7.86
+00010980: 3134 3435 392c 382e 3434 3534 3335 3120  14459,8.4454351 
+00010990: 4320 372e 3235 3531 3336 392c 372e 3538  C 7.2551369,7.58
+000109a0: 3938 3637 3120 362e 3634 3838 3237 392c  98671 6.6488279,
+000109b0: 362e 3733 3432 3939 3120 362e 3034 3235  6.7342991 6.0425
+000109c0: 3139 392c 352e 3837 3837 3332 3120 4320  199,5.8787321 C 
+000109d0: 372e 3234 3531 3933 392c 352e 3631 3734  7.2451939,5.6174
+000109e0: 3335 3120 382e 3538 3237 3833 392c 352e  351 8.5827839,5.
+000109f0: 3038 3533 3839 3120 392e 3037 3034 3430  0853891 9.070440
+00010a00: 392c 332e 3933 3638 3938 3120 4320 392e  9,3.9368981 C 9.
+00010a10: 3430 3633 3133 392c 332e 3131 3230 3231  4063139,3.112021
+00010a20: 3120 392e 3236 3337 3333 392c 322e 3136  1 9.2637339,2.16
+00010a30: 3637 3933 3120 382e 3931 3037 3838 392c  67931 8.9107889,
+00010a40: 312e 3337 3334 3730 3120 4320 382e 3136  1.3734701 C 8.16
+00010a50: 3834 3836 392c 302e 3431 3039 3131 3037  84869,0.41091107
+00010a60: 2036 2e38 3639 3230 3439 2c2d 302e 3037   6.8692049,-0.07
+00010a70: 3234 3531 3933 3120 352e 3631 3939 3732  2451931 5.619972
+00010a80: 392c 302e 3032 3531 3036 3037 2043 2035  9,0.02510607 C 5
+00010a90: 2e34 3639 3332 3739 2c30 2e30 3332 3837  .4693279,0.03287
+00010aa0: 3230 3720 352e 3331 3930 3531 392c 302e  207 5.3190519,0.
+00010ab0: 3034 3635 3130 3037 2035 2e31 3639 3530  04651007 5.16950
+00010ac0: 3839 2c30 2e30 3635 3134 3330 3720 4c20  89,0.06514307 L 
+00010ad0: 352e 3136 3935 3038 392c 302e 3036 3531  5.1695089,0.0651
+00010ae0: 3433 3037 207a 204d 2034 2e30 3035 3439  4307 z M 4.00549
+00010af0: 3439 2c30 2e39 3833 3037 3830 3620 4320  49,0.98307806 C 
+00010b00: 342e 3932 3734 3230 392c 302e 3837 3531  4.9274209,0.8751
+00010b10: 3630 3037 2036 2e30 3735 3238 3339 2c30  6007 6.0752839,0
+00010b20: 2e39 3536 3539 3430 3620 362e 3631 3139  .95659406 6.6119
+00010b30: 3436 392c 312e 3737 3639 3832 3120 4320  469,1.7769821 C 
+00010b40: 372e 3139 3935 3438 392c 322e 3734 3336  7.1995489,2.7436
+00010b50: 3233 3120 362e 3937 3731 3737 392c 342e  231 6.9771779,4.
+00010b60: 3032 3737 3234 3120 362e 3233 3838 3835  0277241 6.238885
+00010b70: 392c 342e 3836 3934 3030 3120 4320 352e  9,4.8694001 C 5.
+00010b80: 3630 3533 3238 392c 352e 3535 3439 3033  6053289,5.554903
+00010b90: 3120 342e 3535 3231 3035 392c 352e 3637  1 4.5521059,5.67
+00010ba0: 3830 3737 3120 332e 3634 3137 3339 392c  80771 3.6417399,
+00010bb0: 352e 3537 3237 3533 3120 4320 332e 3634  5.5727531 C 3.64
+00010bc0: 3137 3339 392c 342e 3036 3535 3237 3120  17399,4.0655271 
+00010bd0: 332e 3634 3137 3339 392c 322e 3535 3833  3.6417399,2.5583
+00010be0: 3030 3120 332e 3634 3137 3339 392c 312e  001 3.6417399,1.
+00010bf0: 3035 3130 3733 3120 4320 332e 3736 3239  0510731 C 3.7629
+00010c00: 3931 392c 312e 3032 3834 3038 3120 332e  919,1.0284081 3.
+00010c10: 3838 3432 3432 392c 312e 3030 3537 3433  8842429,1.005743
+00010c20: 3120 342e 3030 3534 3934 392c 302e 3938  1 4.0054949,0.98
+00010c30: 3330 3738 3036 207a 220a 2020 2020 2020  307806 z".      
+00010c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c50: 2020 7374 796c 653d 2266 696c 6c3a 2024    style="fill: $
+00010c60: 7061 7065 725f 636f 6c6f 725f 3022 0a20  paper_color_0". 
+00010c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c80: 2020 202f 3e0a 2020 2020 2020 2020 2020     />.          
+00010c90: 2020 2020 2020 3c2f 7379 6d62 6f6c 3e0a        </symbol>.
+00010ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010cb0: 3c67 2074 7261 6e73 666f 726d 3d22 7472  <g transform="tr
+00010cc0: 616e 736c 6174 6528 3530 2c35 3029 223e  anslate(50,50)">
+00010cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010ce0: 2020 2020 203c 6720 7472 616e 7366 6f72       <g transfor
+00010cf0: 6d3d 2274 7261 6e73 6c61 7465 2824 6369  m="translate($ci
+00010d00: 7263 6c65 582c 2463 6972 636c 6559 2922  rcleX,$circleY)"
+00010d10: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00010d20: 2020 2020 2020 2020 2020 3c21 2d2d 205a            <!-- Z
+00010d30: 6f64 6961 6320 2d2d 3e0a 2020 2020 2020  odiac -->.      
+00010d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d50: 2020 246d 616b 655a 6f64 6961 6320 0a0a    $makeZodiac ..
+00010d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d70: 2020 2020 2020 2020 3c21 2d2d 2046 6972          <!-- Fir
+00010d80: 7374 2043 6972 636c 6520 2d2d 3e0a 2020  st Circle -->.  
+00010d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010da0: 2020 2020 2020 3c63 6972 636c 6520 2463        <circle $c
+00010db0: 3120 7374 796c 653d 2224 6331 7374 796c  1 style="$c1styl
+00010dc0: 6522 202f 3e0a 0a20 2020 2020 2020 2020  e" />..         
+00010dd0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00010de0: 212d 2d20 5365 636f 6e64 2043 6972 636c  !-- Second Circl
+00010df0: 6520 2d2d 3e0a 2020 2020 2020 2020 2020  e -->.          
+00010e00: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
+00010e10: 6972 636c 6520 2463 3220 7374 796c 653d  ircle $c2 style=
+00010e20: 2224 6332 7374 796c 6522 202f 3e0a 0a20  "$c2style" />.. 
+00010e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e40: 2020 2020 2020 203c 212d 2d20 5468 6972         <!-- Thir
+00010e50: 6420 4369 7263 6c65 202d 2d3e 0a20 2020  d Circle -->.   
+00010e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e70: 2020 2020 203c 6369 7263 6c65 2024 6333       <circle $c3
+00010e80: 2073 7479 6c65 3d22 2463 3373 7479 6c65   style="$c3style
+00010e90: 2220 2f3e 0a0a 2020 2020 2020 2020 2020  " />..          
+00010ea0: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
+00010eb0: 2d2d 2054 7261 6e73 6974 5269 6e67 202d  -- TransitRing -
+00010ec0: 2d3e 0a20 2020 2020 2020 2020 2020 2020  ->.             
+00010ed0: 2020 2020 2020 2020 2020 2024 7472 616e             $tran
+00010ee0: 7369 7452 696e 6720 0a0a 2020 2020 2020  sitRing ..      
+00010ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f00: 2020 3c21 2d2d 2044 6567 7265 6520 5269    <!-- Degree Ri
+00010f10: 6e67 202d 2d3e 0a20 2020 2020 2020 2020  ng -->.         
+00010f20: 2020 2020 2020 2020 2020 2020 2020 2024                 $
+00010f30: 6465 6772 6565 5269 6e67 0a0a 2020 2020  degreeRing..    
+00010f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f50: 2020 2020 3c21 2d2d 2048 6f75 7365 7320      <!-- Houses 
+00010f60: 2d2d 3e0a 2020 2020 2020 2020 2020 2020  -->.            
+00010f70: 2020 2020 2020 2020 2020 2020 246d 616b              $mak
+00010f80: 6548 6f75 7365 730a 0a20 2020 2020 2020  eHouses..       
+00010f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fa0: 203c 212d 2d20 506c 616e 6574 7320 2d2d   <!-- Planets --
+00010fb0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00010fc0: 2020 2020 2020 2020 2020 246d 616b 6550            $makeP
+00010fd0: 6c61 6e65 7473 0a0a 2020 2020 2020 2020  lanets..        
+00010fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ff0: 3c21 2d2d 2041 7370 6563 7473 202d 2d3e  <!-- Aspects -->
+00011000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011010: 2020 2020 2020 2020 2024 6d61 6b65 4173           $makeAs
+00011020: 7065 6374 7320 0a20 2020 2020 2020 2020  pects .         
+00011030: 2020 2020 2020 2020 2020 203c 2f67 3e0a             </g>.
+00011040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011050: 2020 2020 203c 212d 2d20 6d61 6b65 5061       <!-- makePa
+00011060: 7474 6572 6e73 202d 2d3e 0a20 2020 2020  tterns -->.     
+00011070: 2020 2020 2020 2020 2020 2020 2020 2024                 $
+00011080: 6d61 6b65 5061 7474 6572 6e73 0a0a 2020  makePatterns..  
+00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110a0: 2020 3c21 2d2d 2041 7370 6563 7447 7269    <!-- AspectGri
+000110b0: 6420 2d2d 3e0a 2020 2020 2020 2020 2020  d -->.          
+000110c0: 2020 2020 2020 2020 2020 246d 616b 6541            $makeA
+000110d0: 7370 6563 7447 7269 640a 0a20 2020 2020  spectGrid..     
+000110e0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000110f0: 212d 2d20 456c 656d 656e 7473 202d 2d3e  !-- Elements -->
+00011100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011110: 2020 2020 2024 656c 656d 656e 7473 5f70       $elements_p
+00011120: 6572 6365 6e74 6167 6573 200a 0a20 2020  ercentages ..   
+00011130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011140: 203c 212d 2d20 506c 616e 6574 2047 7269   <!-- Planet Gri
+00011150: 6420 2d2d 3e0a 2020 2020 2020 2020 2020  d -->.          
+00011160: 2020 2020 2020 2020 2020 246d 616b 6550            $makeP
+00011170: 6c61 6e65 7447 7269 640a 0a20 2020 2020  lanetGrid..     
+00011180: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00011190: 212d 2d20 486f 7573 6573 2047 7269 6420  !-- Houses Grid 
+000111a0: 2d2d 3e0a 2020 2020 2020 2020 2020 2020  -->.            
+000111b0: 2020 2020 2020 2020 246d 616b 6548 6f75          $makeHou
+000111c0: 7365 7347 7269 640a 0a20 2020 2020 2020  sesGrid..       
+000111d0: 2020 2020 2020 2020 203c 2f67 3e0a 2020           </g>.  
+000111e0: 2020 2020 2020 2020 2020 3c2f 673e 0a20            </g>. 
+000111f0: 2020 2020 2020 203c 2f67 3e0a 2020 2020         </g>.    
+00011200: 3c2f 673e 0a3c 2f73 7667 3e0a            </g>.</svg>.
```

### Comparing `kerykeion-4.6.2/kerykeion/enums.py` & `kerykeion-4.7.0/kerykeion/enums.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.2/kerykeion/fetch_geonames.py` & `kerykeion-4.7.0/kerykeion/fetch_geonames.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.2/kerykeion/kr_types/chart_types.py` & `kerykeion-4.7.0/kerykeion/kr_types/chart_types.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,16 +32,21 @@
     lunar_phase_outline: str
     lunar_phase_rotate: float
     stringLocation: str
     stringDateTime: str
     stringLat: str
     stringLon: str
     stringPosition: str
+
+    # Font color
     paper_color_0: str
+    # Background color of the chart
     paper_color_1: str
+    
+    # Planets colors, from 1 to 15 (0 is the Sun)
     planets_color_0: str
     planets_color_1: str
     planets_color_2: str
     planets_color_3: str
     planets_color_4: str
     planets_color_5: str
     planets_color_6: str
@@ -50,39 +55,44 @@
     planets_color_9: str
     planets_color_10: str
     planets_color_11: str
     planets_color_12: str
     planets_color_13: str
     planets_color_14: str
     planets_color_15: str
+    
+    # Zodiac colors, from 0 to 11 (0 is Aries)
     zodiac_color_0: str
     zodiac_color_1: str
     zodiac_color_2: str
     zodiac_color_3: str
     zodiac_color_4: str
     zodiac_color_5: str
     zodiac_color_6: str
     zodiac_color_7: str
     zodiac_color_8: str
     zodiac_color_9: str
     zodiac_color_10: str
     zodiac_color_11: str
+
+    # Aspects colors, from 0 to 9 (0 is conjunction)
     orb_color_0: str
     orb_color_30: str
     orb_color_45: str
     orb_color_60: str
     orb_color_72: str
     orb_color_90: str
     orb_color_120: str
     orb_color_135: str
     orb_color_144: str
     orb_color_150: str
     orb_color_180: str
+
     cfgZoom: str
     cfgRotate: str
     cfgTranslate: str
     makeZodiac: str
     makeHouses: str
     makePlanets: str
-    makeElements: str
+    elements_percentages: str
     makePlanetGrid: str
     makeHousesGrid: str
```

### Comparing `kerykeion-4.6.2/kerykeion/kr_types/kr_literals.py` & `kerykeion-4.7.0/kerykeion/kr_types/kr_literals.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.2/kerykeion/kr_types/kr_models.py` & `kerykeion-4.7.0/kerykeion/kr_types/kr_models.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.2/kerykeion/kr_types/settings_models.py` & `kerykeion-4.7.0/kerykeion/kr_types/settings_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # -*- coding: utf-8 -*-
 """
     This is part of Kerykeion (C) 2024 Giacomo Battaglia
 """
 
 
-from json import load
 from pydantic import BaseModel, Field
-from pathlib import Path
-from typing import Dict, List, Union
+from typing import List
 
 
 class CustomBaseModel(BaseModel):
     """
     Extends the BaseModel class of Pydantic to add some useful methods.
     """
```

### Comparing `kerykeion-4.6.2/kerykeion/relationship_score.py` & `kerykeion-4.7.0/kerykeion/relationship_score.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.2/kerykeion/report.py` & `kerykeion-4.7.0/kerykeion/report.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.2/kerykeion/settings/kerykeion_settings.py` & `kerykeion-4.7.0/kerykeion/settings/kerykeion_settings.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.2/kerykeion/settings/kr.config.json` & `kerykeion-4.7.0/kerykeion/settings/kr.config.json`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.2/kerykeion/sweph/seas_18.se1` & `kerykeion-4.7.0/kerykeion/sweph/seas_18.se1`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.2/kerykeion/utilities.py` & `kerykeion-4.7.0/kerykeion/utilities.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.2/pyproject.toml` & `kerykeion-4.7.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kerykeion"
-version = "4.6.2"
+version = "4.7.0"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>"]
 description = "A python library for astrology."
 license = "AGPL-3.0"
 homepage = "https://github.com/g-battaglia/kerykeion"
 repository = "https://github.com/g-battaglia/kerykeion"
 keywords = [
     "astrology",
@@ -52,15 +52,15 @@
 [tool.poetry.scripts]
 create-docs = "scripts.docs:main"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 mypy = "^0.991"
 black = "^22.12.0"
-pdoc = "^12.3.0"
+pdoc = "^14.5.0"
 types-requests = "^2.28.11.7"
 types-pytz = "^2022.7.0.0"
 poethepoet = "^0.19.0"
 
 # MyPy Static Analysis
 [tool.mypy]
 ignore_missing_imports = true
```

### Comparing `kerykeion-4.6.2/PKG-INFO` & `kerykeion-4.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerykeion
-Version: 4.6.2
+Version: 4.7.0
 Summary: A python library for astrology.
 Home-page: https://github.com/g-battaglia/kerykeion
 License: AGPL-3.0
 Keywords: astrology,ephemeris,astrology library,birtchart,svg,zodiac,zodiac-sing,astronomical-algorithms,synastry,astrology-calculator
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kerykeion Version: 4.6.2 Summary: A python library
+Metadata-Version: 2.1 Name: kerykeion Version: 4.7.0 Summary: A python library
 for astrology. Home-page: https://github.com/g-battaglia/kerykeion License:
 AGPL-3.0 Keywords: astrology,ephemeris,astrology
 library,birtchart,svg,zodiac,zodiac-sing,astronomical-
 algorithms,synastry,astrology-calculator Author: Giacomo Battaglia Author-
 email: battaglia.giacomo@yahoo.it Requires-Python: >=3.9,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
```

