# Comparing `tmp/weather_swarm-0.0.4.tar.gz` & `tmp/weather_swarm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_swarm-0.0.4.tar", max compression
+gzip compressed data, was "weather_swarm-0.0.5.tar", max compression
```

## Comparing `weather_swarm-0.0.4.tar` & `weather_swarm-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     2791 2024-05-17 18:11:53.166879 weather_swarm-0.0.4/README.md
--rw-r--r--   0        0        0     1404 2024-05-17 18:29:00.659098 weather_swarm-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       74 2024-05-17 16:39:57.227269 weather_swarm-0.0.4/weather_swarm/__init__.py
--rw-r--r--   0        0        0     2529 2024-05-17 16:32:42.620789 weather_swarm-0.0.4/weather_swarm/llama.py
--rw-r--r--   0        0        0    10182 2024-05-09 18:48:47.262272 weather_swarm-0.0.4/weather_swarm/prompts.py
--rw-r--r--   0        0        0        0 2024-05-17 17:02:48.214105 weather_swarm-0.0.4/weather_swarm/tools/__init__.py
--rw-r--r--   0        0        0     7890 2024-05-09 18:51:04.425595 weather_swarm-0.0.4/weather_swarm/tools/baron_tools_schema.py
--rw-r--r--   0        0        0     2070 2024-05-17 17:04:26.838814 weather_swarm-0.0.4/weather_swarm/tools/find_lon_lat_tool.py
--rw-r--r--   0        0        0    29914 2024-05-17 18:05:30.452504 weather_swarm-0.0.4/weather_swarm/tools/tools.py
--rw-r--r--   0        0        0     5829 2024-05-17 18:18:22.746776 weather_swarm-0.0.4/weather_swarm/worker_agents.py
--rw-r--r--   0        0        0     3600 1970-01-01 00:00:00.000000 weather_swarm-0.0.4/setup.py
--rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 weather_swarm-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2912 2024-05-22 17:01:45.255416 weather_swarm-0.0.5/README.md
+-rw-r--r--   0        0        0     1385 2024-05-30 19:29:42.699516 weather_swarm-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 19:13:25.911821 weather_swarm-0.0.5/weather_swarm/__init__.py
+-rw-r--r--   0        0        0     9913 2024-05-30 19:14:34.673592 weather_swarm-0.0.5/weather_swarm/director_agent.py
+-rw-r--r--   0        0        0    10178 2024-05-24 19:21:17.493671 weather_swarm-0.0.5/weather_swarm/prompts.py
+-rw-r--r--   0        0        0      757 2024-05-30 16:18:01.722579 weather_swarm-0.0.5/weather_swarm/tool_schemas.py
+-rw-r--r--   0        0        0        0 2024-05-22 16:50:33.387606 weather_swarm-0.0.5/weather_swarm/tools/__init__.py
+-rw-r--r--   0        0        0     3770 2024-05-30 19:14:41.020988 weather_swarm-0.0.5/weather_swarm/tools/baron_tools_schema.py
+-rw-r--r--   0        0        0     3545 2024-05-24 17:39:31.442309 weather_swarm-0.0.5/weather_swarm/tools/get_geo_coordinates.py
+-rw-r--r--   0        0        0     3466 2024-05-29 15:36:53.440129 weather_swarm-0.0.5/weather_swarm/tools/simple_tool.py
+-rw-r--r--   0        0        0    30792 2024-05-30 16:18:01.847716 weather_swarm-0.0.5/weather_swarm/tools/tools.py
+-rw-r--r--   0        0        0     6592 2024-05-30 19:14:58.910209 weather_swarm-0.0.5/weather_swarm/worker_agents.py
+-rw-r--r--   0        0        0     3938 1970-01-01 00:00:00.000000 weather_swarm-0.0.5/PKG-INFO
```

### Comparing `weather_swarm-0.0.4/README.md` & `weather_swarm-0.0.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -71,14 +71,17 @@
     "create an essay on how to bake chicken"
 )
 
 print(completion_generator)
 
 ```
 
+# Documentation
+- [Llama3Hosted](docs/llama3_hosted.md)
+
 ## Contributing
 Contributions to Baron Weather are welcome and appreciated. Here's how you can contribute:
 
 1. Fork the Project
 2. Create your Feature Branch (`git checkout -b feature/YourAmazingFeature`)
 3. Commit your Changes (`git commit -m 'Add some YourAmazingFeature'`)
 4. Push to the Branch (`git push origin feature/YourAmazingFeature`)
@@ -90,15 +93,13 @@
 
 `pytest`
 
 ## Contact
 Project Maintainer - [Kye Gomez](mailto:kye@swarms.world) - [GitHub Profile](https://github.com/baronservices)
 
 
-## Acknowledgements
 # Todo
-- Make API server functional
-- Make Dockerfile
-- Create a team of specialized agents for different types of weather tools.
-- Create documentation for llama3,
-- Create dockerfile
-- Create documentation for the agents and how to use them
+- [ ] Add the schemas to the worker agents to output json
+- [ ] Implement the parser and the function calling mapping to execute the functions
+- [ ] Implement the HiearArchical Swarm and plug in and all the agents
+- [ ] Then, implement the API server wrapping the hiearchical swarm
+- [ ] Then, Deploy on the server 24/7
```

### Comparing `weather_swarm-0.0.4/pyproject.toml` & `weather_swarm-0.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "weather-swarm"
-version = "0.0.4"
+version = "0.0.5"
 description = "Weather Swarm - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/baronservices/weatherman_agent"
 documentation = "https://github.com/baronservices/weatherman_agent"  # Add this if you have documentation.
 readme = "README.md"  # Assuming you have a README.md
 repository = "https://github.com/baronservices/weatherman_agent"
@@ -20,15 +20,14 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.9"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 swarms = "*"
-transformers = "*"
 pydantic = "2.7.1"
 
 
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.6"
 types-toml = "^0.10.8.1"
```

### Comparing `weather_swarm-0.0.4/weather_swarm/prompts.py` & `weather_swarm-0.0.5/weather_swarm/prompts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 GLOSSARY_PROMPTS = """
 
 Glossary
- 
- 
 
 API Terminology
 Access_key
 A private access key or shared access key (not a secret and not an Application Key) used to access the Baron Weather API. View your access keys on your account page.
 
 Application Key
 Users’ personal and confidential key from which access keys are derived. The application key allows management of access keys. View your application key on your account page.
```

### Comparing `weather_swarm-0.0.4/weather_swarm/tools/tools.py` & `weather_swarm-0.0.5/weather_swarm/tools/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # coding: utf-8
 
 import base64
-import datetime
 import hashlib
 import hmac
 import shutil
 import time
 from urllib.request import urlopen
 from urllib.request import Request
 from urllib.error import URLError
 import os
 import json
 import codecs
 from dotenv import load_dotenv
+import datetime
 
 load_dotenv()
 
 latin1 = codecs.lookup("latin-1")
 
 host = os.environ.get(
     "BARON_API_HOST", "http://api.velocityweather.com/v1"
@@ -51,14 +51,15 @@
 
     signature = sig(key, secret)
     q = "?" if url.find("?") == -1 else "&"
     url += "{}{}".format(q, signature)
     return url
 
 
+########## [START] API REQUESTS ##########
 def request_pointquery_nws_watches_warning_all():
     uri = "/reports/alert/all-poly/point.json?lat=29.70&lon=-80.41"
     url = "%s/%s%s" % (host, access_key, uri)
     return sign_request(url, access_key, access_key_secret)
 
 
 def request_lightning_count():
@@ -77,17 +78,16 @@
     uri = "/reports/geocode/ipaddress.json"
     url = "%s/%s%s" % (host, access_key, uri)
     url = sign_request(url, access_key, access_key_secret)
     return sign_request(url, access_key, access_key_secret)
 
 
 def request_forecast(lat, lon):
-    uri = (
-        "/reports/pointforecast/basic.json?days=7&lat={}&lon={}"
-        .format(lat, lon)
+    uri = "/reports/pointforecast/basic.json?days=7&lat={}&lon={}".format(
+        lat, lon
     )
 
     url = "%s/%s%s" % (host, access_key, uri)
     url = sign_request(url, access_key, access_key_secret)
 
     try:
         response = urlopen(url)
@@ -150,15 +150,15 @@
 
             metars[siteid] = {"metar": metar, "forecast": forecast}
 
     with open("metar.json", "w") as metar_jsonfile:
         json.dump(metars, metar_jsonfile, indent=4, sort_keys=True)
 
 
-def request_metar_nearest(lat, lon):
+def request_metar_nearest(lat: float, lon: float):
     uri = (
         "/reports/metar/nearest.json?lat=%s&lon=%s&within_radius=500&max_age=75"
         % (
             lat,
             lon,
         )
     )
@@ -168,37 +168,55 @@
 
 def request_metar(station_id):
     uri = "/reports/metar/station/%s.json" % station_id
     url = "%s/%s%s" % (host, access_key, uri)
     return sign_request(url, access_key, access_key_secret)
 
 
-def request_ndfd_hourly(lat, lon, utc_datetime):
+def request_ndfd_hourly(
+    lat: float, lon: float, utc_datetime: datetime.datetime
+) -> str:
+    """
+    Requests NDFD hourly data for a specific latitude, longitude, and UTC datetime.
+
+    Args:
+        lat (float): The latitude of the location.
+        lon (float): The longitude of the location.
+        utc_datetime (datetime.datetime): The UTC datetime for the request.
+
+    Returns:
+        str: The signed URL for the request.
+    """
     datetime_str = (
         utc_datetime.replace(microsecond=0).isoformat() + "Z"
     )
-    uri = "/reports/ndfd/hourly.json?lat=%s&lon=%s&utc=%s" % (
-        lat,
-        lon,
-        datetime_str,
-    )
-    url = "%s/%s%s" % (host, access_key, uri)
+    uri = f"/reports/ndfd/hourly.json?lat={lat}&lon={lon}&utc={datetime_str}"
+    url = f"{host}/{access_key}{uri}"
     return sign_request(url, access_key, access_key_secret)
 
 
-def request_ndfd_basic(lat, lon, utc_datetime):
+def request_ndfd_basic(
+    lat: float, lon: float, utc_datetime: datetime.datetime
+) -> str:
+    """
+    Requests NDFD basic data for a specific latitude, longitude, and UTC datetime.
+
+    Args:
+        lat (float): The latitude of the location.
+        lon (float): The longitude of the location.
+        utc_datetime (datetime.datetime): The UTC datetime for the request.
+
+    Returns:
+        str: The signed URL for the request.
+    """
     datetime_str = (
         utc_datetime.replace(microsecond=0).isoformat() + "Z"
     )
-    uri = "/reports/ndfd/basic.json?lat=%s&lon=%s&utc=%s&days=7" % (
-        lat,
-        lon,
-        datetime_str,
-    )
-    url = "%s/%s%s" % (host, access_key, uri)
+    uri = f"/reports/ndfd/basic.json?lat={lat}&lon={lon}&utc={datetime_str}&days=7"
+    url = f"{host}/{access_key}{uri}"
     return sign_request(url, access_key, access_key_secret)
 
 
 def request_tile(product, product_config, z, x, y):
     url = "%s/%s/meta/tiles/product-instances/%s/%s" % (
         host,
         access_key,
@@ -686,17 +704,16 @@
         f.write(content)
 
 
 def request_geotiff(product, product_config, product_instance=""):
     if not product_instance:
         # For this example, we use the optional parameter "page_size" to limit the
         # list of product instances to the most recent instance.
-        meta_url = (
-            "{}/{}/meta/tiles/product-instances/{}/{}?page_size=1"
-            .format(host, access_key, product, product_config)
+        meta_url = "{}/{}/meta/tiles/product-instances/{}/{}?page_size=1".format(
+            host, access_key, product, product_config
         )
         meta_url = sign_request(
             meta_url, access_key, access_key_secret
         )
 
         try:
             response = urlopen(meta_url)
@@ -893,114 +910,114 @@
             )
             return
         url = "{}&older_than={}".format(
             url_template, content[-1]["time"]
         )
 
 
-def main():
-    url = request_metar_nearest("38", "-96")
-    print("*** request METAR nearest ***")
-    print(url)
-    print(urlopen(url).read())
-    print("")
+# def main():
+#     url = request_metar_nearest("38", "-96")
+#     print("*** request METAR nearest ***")
+#     print(url)
+#     print(urlopen(url).read())
+#     print("")
+
+#     point_query(
+#         "precip-totalaccum-24hr", "Standard-Mercator", -86.6, 34.4
+#     )
+
+#     forecast_time = datetime.datetime.utcnow()
+#     url = request_ndfd_basic(34.730301, -86.586098, forecast_time)
+#     print("*** request NDFD hourly ***")
+#     print(url)
+#     print(urlopen(url).read())
+#     print("")
+
+#     # /point/baron-hires-temp-f-2meter/Standard-Mercator/2024-05-02T12%3A00%3A00Z.jsonp?callback=_jqjsp&lat=30.173624550358536&lon=-95.3009033203125&ts=1714685100&sig=IOUh5xEZzyRqzT1MQctn1vxSqXM=&valid_time=*
+#     point_query(
+#         "baron-hires-maxreflectivity-dbz-all",
+#         "Mask1-Mercator",
+#         -86.6,
+#         34.4,
+#     )
+
+#     point_query(
+#         "baron-hires-windspeed-mph-10meter",
+#         "Standard-Mercator",
+#         -86.6,
+#         34.4,
+#     )
+
+#     # Get all product instances for a product.
+#     # for i, instance in enumerate(iter_product_instances('C39-0x0302-0', 'Standard-Mercator')):
+#     #    print('{:>3} {}'.format(i, instance['time']))
+
+#     # Or, alternatively, get the product instances using a wms-style request.
+#     # request_wms_capabilities('C39-0x0302-0', 'Standard-Mercator')
+
+#     # Request the whole world in the EPSG:4326 projection. Note that the proportions for
+#     # the image size in pixels and the image bounds are identical (2:1).
+#     # request_wms('C39-0x0302-0', 'Standard-Geodetic', [2048, 1024], [-90, -180, 90, 180])
+
+#     # Request the whole world in the EPSG:3857 projection. Note that the proportions for
+#     # the image size in pixels and the image bounds are identical (1:1).
+#     # request_wms('C39-0x0302-0', 'Standard-Mercator', [2048, 2048], [-20037508.342789244, -20037508.342789244, 20037508.342789244, 20037508.342789244])
+
+#     # filename, valid_times = request_geotiff('C39-0x0302-0', 'Standard-Mercator')
+
+#     """
+#     print("*** request point query ***")
+#     point_query('C09-0x0331-0', 'Standard-Mercator', -86, 34)
+#     print("")
+
+
+#     print("*** requesting METARS and Forecasts for North America ***")
+#     request_metar_northamerica()
+#     print("")
+
+
+#     url = request_metar("egll")
+#     print("*** request METAR ***")
+#     print(url)
+#     print(urlopen(url).read())
+#     print("")
+
+#     forecast_time = datetime.datetime.utcnow() + datetime.timedelta(hours=4)
+#     url = request_ndfd_hourly(34.730301, -86.586098, forecast_time)
+#     print("*** request NDFD hourly ***")
+#     print(url)
+#     print(urlopen(url).read())
+#     print("")
+
+#     request_tile("C39-0x0302-0", "Standard-Mercator", 1, 0, 1)
+#     url = request_storm_vector("mhx")
+#     print("*** request storm vectors ***")
+#     print(url)
+#     a = urlopen(url)
+#     print('JSON for storm vectors is %d bytes' % len(urlopen(url).read()))
+#     print("")
+#     url = request_geocodeip()
+#     print("*** geocode IP address ***")
+#     print(url)
+#     print(urlopen(url).read())
+#     print("")
+#     url = request_lightning_count()
+#     print("*** lightning count ***")
+#     print(url)
+#     print(urlopen(url).read())
+#     print("")
+
+#     date = datetime.datetime.now().date() + datetime.timedelta(days=1)
+#     bgfs_basic(-86.6, 34.4, date, 1)
+#     bgfs_extended(-86.6, 34.4, date, 1)
+#     bgfs_hourly(-86.6, 34.4, datetime.datetime.combine(date, datetime.time(hour=6)), 1)
+#     print("")
+
+#     point_query('C09-0x0331-0', 'Standard-Mercator', -86.6, 34.4)
+#     point_query_multi('C09-0x0331-0', 'Standard-Mercator', [(-86.6, 34.4), (-90.14, 38)])
+#     point_query_region('C09-0x0331-0', 'Standard-Mercator', 34.4, 34.1, -86.6, -86.5)
 
-    point_query(
-        "precip-totalaccum-24hr", "Standard-Mercator", -86.6, 34.4
-    )
-
-    forecast_time = datetime.datetime.utcnow()
-    url = request_ndfd_basic(34.730301, -86.586098, forecast_time)
-    print("*** request NDFD hourly ***")
-    print(url)
-    print(urlopen(url).read())
-    print("")
-
-    # /point/baron-hires-temp-f-2meter/Standard-Mercator/2024-05-02T12%3A00%3A00Z.jsonp?callback=_jqjsp&lat=30.173624550358536&lon=-95.3009033203125&ts=1714685100&sig=IOUh5xEZzyRqzT1MQctn1vxSqXM=&valid_time=*
-    point_query(
-        "baron-hires-maxreflectivity-dbz-all",
-        "Mask1-Mercator",
-        -86.6,
-        34.4,
-    )
-
-    point_query(
-        "baron-hires-windspeed-mph-10meter",
-        "Standard-Mercator",
-        -86.6,
-        34.4,
-    )
-
-    # Get all product instances for a product.
-    # for i, instance in enumerate(iter_product_instances('C39-0x0302-0', 'Standard-Mercator')):
-    #    print('{:>3} {}'.format(i, instance['time']))
-
-    # Or, alternatively, get the product instances using a wms-style request.
-    # request_wms_capabilities('C39-0x0302-0', 'Standard-Mercator')
-
-    # Request the whole world in the EPSG:4326 projection. Note that the proportions for
-    # the image size in pixels and the image bounds are identical (2:1).
-    # request_wms('C39-0x0302-0', 'Standard-Geodetic', [2048, 1024], [-90, -180, 90, 180])
-
-    # Request the whole world in the EPSG:3857 projection. Note that the proportions for
-    # the image size in pixels and the image bounds are identical (1:1).
-    # request_wms('C39-0x0302-0', 'Standard-Mercator', [2048, 2048], [-20037508.342789244, -20037508.342789244, 20037508.342789244, 20037508.342789244])
-
-    # filename, valid_times = request_geotiff('C39-0x0302-0', 'Standard-Mercator')
-
-    """
-    print("*** request point query ***")
-    point_query('C09-0x0331-0', 'Standard-Mercator', -86, 34)
-    print("")
-    
-    
-    print("*** requesting METARS and Forecasts for North America ***")
-    request_metar_northamerica()
-    print("")
-    
-    
-    url = request_metar("egll")
-    print("*** request METAR ***")
-    print(url)
-    print(urlopen(url).read())
-    print("")
-
-    forecast_time = datetime.datetime.utcnow() + datetime.timedelta(hours=4)
-    url = request_ndfd_hourly(34.730301, -86.586098, forecast_time)
-    print("*** request NDFD hourly ***")
-    print(url)
-    print(urlopen(url).read())
-    print("")
-
-    request_tile("C39-0x0302-0", "Standard-Mercator", 1, 0, 1)
-    url = request_storm_vector("mhx")
-    print("*** request storm vectors ***")
-    print(url)
-    a = urlopen(url)
-    print('JSON for storm vectors is %d bytes' % len(urlopen(url).read()))
-    print("")
-    url = request_geocodeip()
-    print("*** geocode IP address ***")
-    print(url)
-    print(urlopen(url).read())
-    print("")
-    url = request_lightning_count()
-    print("*** lightning count ***")
-    print(url)
-    print(urlopen(url).read())
-    print("")
-
-    date = datetime.datetime.now().date() + datetime.timedelta(days=1)
-    bgfs_basic(-86.6, 34.4, date, 1)
-    bgfs_extended(-86.6, 34.4, date, 1)
-    bgfs_hourly(-86.6, 34.4, datetime.datetime.combine(date, datetime.time(hour=6)), 1)
-    print("")
-
-    point_query('C09-0x0331-0', 'Standard-Mercator', -86.6, 34.4)
-    point_query_multi('C09-0x0331-0', 'Standard-Mercator', [(-86.6, 34.4), (-90.14, 38)])
-    point_query_region('C09-0x0331-0', 'Standard-Mercator', 34.4, 34.1, -86.6, -86.5)
-    
-    """
+#     """
 
 
-if __name__ == "__main__":
-    main()
+# if __name__ == "__main__":
+#     main()
```

### Comparing `weather_swarm-0.0.4/weather_swarm/worker_agents.py` & `weather_swarm-0.0.5/weather_swarm/worker_agents.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,31 @@
 from swarms import Agent
-from weather_swarm.llama import llama3Hosted
+from swarms import llama3Hosted
+from pydantic import BaseModel, Field
+from weather_swarm.tools.tools import (
+    request_metar_nearest,
+    point_query,
+    request_ndfd_basic,
+    point_query_region,
+    request_ndfd_hourly,
+)
+
+
+class WeatherRequest(BaseModel):
+    """
+    A class to represent the weather request.
+
+    Attributes
+    ----------
+    query : str
+        The user's query.
+    """
+
+    task: str = Field(..., title="The user's query")
+    tool: str = Field(None, title="The tool to execute")
 
 
 def current_temperature_retrieval_agent():
     return """
     ### Current Temperature Retrieval Agent
 
     **Prompt:**
@@ -141,90 +163,107 @@
     llm=llm,
     max_loops=1,
     autosave=True,
     dashboard=False,
     streaming_on=True,
     verbose=True,
     stopping_token="<DONE>",
-    interactive=True,
+    tools=[request_metar_nearest],
 )
 
 weather_narrator = Agent(
     agent_name="WeatherNarrator",
     system_prompt=current_weather_description_agent(),
     llm=llm,
     max_loops=1,
     autosave=True,
     dashboard=False,
     streaming_on=True,
     verbose=True,
     stopping_token="<DONE>",
-    interactive=True,
+    tools=[request_metar_nearest],
 )
 
 rain_gauge = Agent(
     agent_name="RainGauge",
     system_prompt=rainfall_accumulation_agent(),
     llm=llm,
     max_loops=1,
     autosave=True,
     dashboard=False,
     streaming_on=True,
     verbose=True,
     stopping_token="<DONE>",
-    interactive=True,
+    tools=[point_query],
 )
 
 cloud_predictor = Agent(
     agent_name="CloudPredictor",
     system_prompt=cloud_coverage_forecast_agent(),
     llm=llm,
     max_loops=1,
     autosave=True,
     dashboard=False,
     streaming_on=True,
     verbose=True,
     stopping_token="<DONE>",
-    interactive=True,
+    tools=[request_ndfd_basic],
 )
 
 rain_forecaster = Agent(
     agent_name="RainForecaster",
     system_prompt=precipitation_forecast_agent(),
     llm=llm,
     max_loops=1,
     autosave=True,
     dashboard=False,
     streaming_on=True,
     verbose=True,
     stopping_token="<DONE>",
-    interactive=True,
+    tools=[point_query_region],
 )
 
 temp_forecaster = Agent(
     agent_name="TempForecaster",
     system_prompt=maximum_temperature_forecast_agent(),
     llm=llm,
     max_loops=1,
+    verbose=True,
+    output_type=dict,
     autosave=True,
     dashboard=False,
     streaming_on=True,
-    verbose=True,
     stopping_token="<DONE>",
-    interactive=True,
+    tools=[request_ndfd_hourly],
 )
 
 wind_watcher = Agent(
     agent_name="WindWatcher",
     system_prompt=wind_speed_forecast_agent(),
     llm=llm,
     max_loops=1,
     autosave=True,
     dashboard=False,
     streaming_on=True,
     verbose=True,
     stopping_token="<DONE>",
-    interactive=True,
+    tools=[point_query_region],
 )
 
-# # Example usage
-# agents = [temp_tracker, weather_narrator, rain_gauge, cloud_predictor, rain_forecaster, temp_forecaster, wind_watcher]
+# Create a list
+agents = [
+    temp_tracker,
+    weather_narrator,
+    rain_gauge,
+    cloud_predictor,
+    rain_forecaster,
+    temp_forecaster,
+    wind_watcher,
+]
+
+# # Create a hierarchical swarm
+# swarm = HiearchicalSwarm(
+#     name = "WeatherSwarm",
+#     description="A swarm of weather agents",
+#     agents=agents,
+#     director =
+# )
```

### Comparing `weather_swarm-0.0.4/PKG-INFO` & `weather_swarm-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: weather-swarm
-Version: 0.0.4
+Version: 0.0.5
 Summary: Weather Swarm - Pytorch
 Home-page: https://github.com/baronservices/weatherman_agent
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: pydantic (==2.7.1)
 Requires-Dist: swarms
-Requires-Dist: transformers
 Project-URL: Documentation, https://github.com/baronservices/weatherman_agent
 Project-URL: Repository, https://github.com/baronservices/weatherman_agent
 Description-Content-Type: text/markdown
 
 # Baron Weather
 
 ## Overview
@@ -96,14 +96,17 @@
     "create an essay on how to bake chicken"
 )
 
 print(completion_generator)
 
 ```
 
+# Documentation
+- [Llama3Hosted](docs/llama3_hosted.md)
+
 ## Contributing
 Contributions to Baron Weather are welcome and appreciated. Here's how you can contribute:
 
 1. Fork the Project
 2. Create your Feature Branch (`git checkout -b feature/YourAmazingFeature`)
 3. Commit your Changes (`git commit -m 'Add some YourAmazingFeature'`)
 4. Push to the Branch (`git push origin feature/YourAmazingFeature`)
@@ -115,15 +118,13 @@
 
 `pytest`
 
 ## Contact
 Project Maintainer - [Kye Gomez](mailto:kye@swarms.world) - [GitHub Profile](https://github.com/baronservices)
 
 
-## Acknowledgements
 # Todo
-- Make API server functional
-- Make Dockerfile
-- Create a team of specialized agents for different types of weather tools.
-- Create documentation for llama3,
-- Create dockerfile
-- Create documentation for the agents and how to use them
+- [ ] Add the schemas to the worker agents to output json
+- [ ] Implement the parser and the function calling mapping to execute the functions
+- [ ] Implement the HiearArchical Swarm and plug in and all the agents
+- [ ] Then, implement the API server wrapping the hiearchical swarm
+- [ ] Then, Deploy on the server 24/7
```

