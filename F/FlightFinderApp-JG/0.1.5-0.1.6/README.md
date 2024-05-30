# Comparing `tmp/flightfinderapp_jg-0.1.5.tar.gz` & `tmp/flightfinderapp_jg-0.1.6.tar.gz`

## Comparing `flightfinderapp_jg-0.1.5.tar` & `flightfinderapp_jg-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     6344 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.5/Example.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.5/src/FlightFinderApp_JG/Constants.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.5/src/FlightFinderApp_JG/DestinationManager.py
--rw-r--r--   0        0        0     8343 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.5/src/FlightFinderApp_JG/FlightManager.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.5/src/FlightFinderApp_JG/SessionManager.py
--rw-r--r--   0        0        0    10946 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.5/src/FlightFinderApp_JG/__Parsers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.5/src/FlightFinderApp_JG/__init__.py
--rw-r--r--   0        0        0    10683 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.5/src/FlightFinderApp_JG/cli.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.5/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.5/LICENSE
--rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.5/README.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.6/Example.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.6/src/FlightFinderApp_JG/Constants.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.6/src/FlightFinderApp_JG/DestinationManager.py
+-rw-r--r--   0        0        0     8343 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.6/src/FlightFinderApp_JG/FlightManager.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.6/src/FlightFinderApp_JG/SessionManager.py
+-rw-r--r--   0        0        0    13409 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.6/src/FlightFinderApp_JG/__Parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.6/src/FlightFinderApp_JG/__init__.py
+-rw-r--r--   0        0        0    10683 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.6/src/FlightFinderApp_JG/cli.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.6/LICENSE
+-rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.6/README.md
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 flightfinderapp_jg-0.1.6/PKG-INFO
```

### Comparing `flightfinderapp_jg-0.1.5/Example.py` & `flightfinderapp_jg-0.1.6/Example.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 from FlightFinderApp_JG.FlightManager import RyanairFlights
 
 table = PrettyTable()
 ryanairFlights = RyanairFlights()
 
 
 _departure_airport = "KUN"
-_arrival_airport = "OPO"
+_arrival_airport = "BER"
 _includeReturnFlight = True
 _dateFrom = str(datetime.date.today())
 _price_value = 50
 
 result = ryanairFlights.find_flights(departure_airport_code=_departure_airport,
                                      arrival_airport_code=_arrival_airport,
                                      is_return_trip=_includeReturnFlight,
                                      outbound_date=_dateFrom,
                                      date_flexibility_in_days=10,
                                      trip_duration_in_days=10)
 
 if result is not None:
     if not _includeReturnFlight:
-        table.field_names = ["Total Trip Price", "Flight From", "Flight To", "Departure date", "Arrival date"]
+        table.field_names = ["Total Trip Price", "Flight From", "Flight To", "Departure date", "Arrival date", "Link"]
 
         for item in result:
             data = json.loads(item)
             if "toConnecting" in data["outbound"]:
                 table.add_row([
                     str(data["outbound"]["toConnecting"]["price"])+" ("+data["outbound"]["toConnecting"]["currency"]+")",
                     data["outbound"]["toConnecting"]["departureCity"]+" ("+data["outbound"]["toConnecting"]["departureIataCode"]+")",
@@ -41,18 +41,19 @@
                     data["outbound"]["fromConnecting"]["arrivalDate"]], divider=True)
             else:
                 table.add_row([
                     str(data["outbound"]["price"])+" ("+data["outbound"]["currency"]+")",
                     data["outbound"]["departureCity"]+" ("+data["outbound"]["departureIATACode"]+")",
                     data["outbound"]["arrivalCity"]+" ("+data["outbound"]["arrivalIATACode"]+")",
                     data["outbound"]["departureDate"],
-                    data["outbound"]["arrivalDate"]])
+                    data["outbound"]["arrivalDate"],
+                    data["summary"]["link"]])
 
     else:
-        table.field_names = ["Total Trip Price", "Trip Duration", "Outbound Flight", "Outbound Departure Date", "Outbound Arrival Date", "Outbound Flight Price", "Inbound Flight", "Inbound Departure Date", "Inbound Arrival Date", "Inbound Flight Price"]
+        table.field_names = ["Total Trip Price", "Trip Duration", "Outbound Flight", "Outbound Departure Date", "Outbound Arrival Date", "Outbound Flight Price", "Inbound Flight", "Inbound Departure Date", "Inbound Arrival Date", "Inbound Flight Price", "Link"]
 
         for item in result:
             data = json.loads(item)
 
             if "toConnecting" in data["outbound"]:
                 table.add_row([
                     str(data["tripSummary"]["totalPrice"]),
@@ -91,10 +92,11 @@
                     data["outbound"]["departureCity"]+" ("+data["outbound"]["departureIATACode"]+")",
                     data["outbound"]["departureDate"],
                     data["outbound"]["arrivalDate"],
                     str(data["outbound"]["price"])+" ("+data["outbound"]["currency"]+")",
                     data["inbound"]["departureCity"]+" ("+data["inbound"]["departureIATACode"]+")",
                     data["inbound"]["departureDate"],
                     data["inbound"]["arrivalDate"],
-                    str(data["inbound"]["price"])+" ("+data["inbound"]["currency"]+")"])
+                    str(data["inbound"]["price"])+" ("+data["inbound"]["currency"]+")",
+                    data["summary"]["link"]])
 
     print(table)
```

### Comparing `flightfinderapp_jg-0.1.5/src/FlightFinderApp_JG/DestinationManager.py` & `flightfinderapp_jg-0.1.6/src/FlightFinderApp_JG/DestinationManager.py`

 * *Files identical despite different names*

### Comparing `flightfinderapp_jg-0.1.5/src/FlightFinderApp_JG/FlightManager.py` & `flightfinderapp_jg-0.1.6/src/FlightFinderApp_JG/FlightManager.py`

 * *Files identical despite different names*

### Comparing `flightfinderapp_jg-0.1.5/src/FlightFinderApp_JG/__Parsers.py` & `flightfinderapp_jg-0.1.6/src/FlightFinderApp_JG/__Parsers.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,15 +15,28 @@
             "departureDate": item["outbound"]["departureDate"],
             "arrivalDate": item["outbound"]["arrivalDate"],
             "price": item["outbound"]["price"]["value"],
             "currency": item["outbound"]["price"]["currencyCode"],
             "priceUpdatedOn": item["outbound"]["priceUpdated"]},
             "summary": {
                 "price": item["summary"]["price"]["value"],
-                "currency": item["summary"]["price"]["currencyCode"]
+                "currency": item["summary"]["price"]["currencyCode"],
+                "link": "https://www.ryanair.com/gb/en/trip/flights/select?adults=1"
+                        +"&teens=0&children=0&infants=0&dateOut="
+                        +str(datetime.datetime.strptime(item["outbound"]["departureDate"], "%Y-%m-%dT%H:%M:%S").date())
+                        +"&dateIn=&isConnectedFlight=false&discount=0&promoCode=&isReturn=false&originIata="
+                        +item["outbound"]["departureAirport"]["iataCode"]
+                        +"&destinationIata="
+                        +item["outbound"]["arrivalAirport"]["iataCode"]
+                        +"&tpAdults=1&tpTeens=0&tpChildren=0&tpInfants=0&tpStartDate="
+                        +str(datetime.datetime.strptime(item["outbound"]["departureDate"], "%Y-%m-%dT%H:%M:%S").date())
+                        +"&tpEndDate=&tpDiscount=0&tpPromoCode=&tpOriginIata="
+                        +item["outbound"]["departureAirport"]["iataCode"]
+                        +"&tpDestinationIata="
+                        +item["outbound"]["arrivalAirport"]["iataCode"]
             }
         }
         if return_trip:
             data.update({"inbound": {
                 "departureCountry": item["inbound"]["departureAirport"]["countryName"],
                 "departureCity": item["inbound"]["departureAirport"]["city"]["name"],
                 "departureIATACode": item["inbound"]["departureAirport"]["iataCode"],
@@ -34,15 +47,32 @@
                 "arrivalDate": item["inbound"]["arrivalDate"],
                 "price": item["inbound"]["price"]["value"],
                 "currency": item["inbound"]["price"]["currencyCode"],
                 "priceUpdatedOn": item["inbound"]["priceUpdated"]},
                 "summary": {
                     "price": item["summary"]["price"]["value"],
                     "currency": item["summary"]["price"]["currencyCode"],
-                    "tripDuration": item["summary"]["tripDurationDays"]
+                    "tripDuration": item["summary"]["tripDurationDays"],
+                    "link": "https://www.ryanair.com/gb/en/trip/flights/select?adults=1"
+                            +"&teens=0&children=0&infants=0&dateOut="
+                            +str(datetime.datetime.strptime(item["outbound"]["departureDate"], "%Y-%m-%dT%H:%M:%S").date())
+                            +"&dateIn="
+                            +str(datetime.datetime.strptime(item["outbound"]["departureDate"], "%Y-%m-%dT%H:%M:%S").date())
+                            +"&isConnectedFlight=false&discount=0&promoCode=&isReturn=true&originIata="
+                            +item["outbound"]["departureAirport"]["iataCode"]
+                            +"&destinationIata="
+                            +item["outbound"]["arrivalAirport"]["iataCode"]
+                            +"&tpAdults=1&tpTeens=0&tpChildren=0&tpInfants=0&tpStartDate="
+                            +str(datetime.datetime.strptime(item["outbound"]["departureDate"], "%Y-%m-%dT%H:%M:%S").date())
+                            +"&tpEndDate="
+                            +str(datetime.datetime.strptime(item["inbound"]["arrivalDate"], "%Y-%m-%dT%H:%M:%S").date())
+                            +"&tpDiscount=0&tpPromoCode=&tpOriginIata="
+                            +item["outbound"]["departureAirport"]["iataCode"]
+                            +"&tpDestinationIata="
+                            +item["outbound"]["arrivalAirport"]["iataCode"]
                 }})
         flights.append(json.dumps(data))
 
     return flights
 
 def parse_connecting_flight_results(flights_to_connecting_airports, flights_from_connecting_airports):
 
@@ -161,8 +191,8 @@
                     "summary": {
                         "timeBetweenFlights": str(
                             datetime.datetime.strptime(flight_from["outbound"]["departureDate"], "%Y-%m-%dT%H:%M:%S")
                             - datetime.datetime.strptime(flight_to["outbound"]["arrivalDate"], "%Y-%m-%dT%H:%M:%S"))
                     }
                 }}
                 flight_data.append(json.dumps(data))
-    return flight_data
+    return flight_data
```

### Comparing `flightfinderapp_jg-0.1.5/src/FlightFinderApp_JG/cli.py` & `flightfinderapp_jg-0.1.6/src/FlightFinderApp_JG/cli.py`

 * *Files identical despite different names*

### Comparing `flightfinderapp_jg-0.1.5/LICENSE` & `flightfinderapp_jg-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flightfinderapp_jg-0.1.5/README.md` & `flightfinderapp_jg-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `flightfinderapp_jg-0.1.5/pyproject.toml` & `flightfinderapp_jg-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests", "prettytable", "click"]
 build-backend = "hatchling.build"
 
 [project]
 name = "FlightFinderApp_JG"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
     { name="Justinas Greibus" },
 ]
 description = "A helper that interacts with low-cost air carrier's API and helps to find cheap flights."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `flightfinderapp_jg-0.1.5/PKG-INFO` & `flightfinderapp_jg-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: FlightFinderApp_JG
-Version: 0.1.5
+Version: 0.1.6
 Summary: A helper that interacts with low-cost air carrier's API and helps to find cheap flights.
 Project-URL: Homepage, https://github.com/jgreibus/flight_finder
 Project-URL: Issues, https://github.com/jgreibus/flight_finder/issues
 Author: Justinas Greibus
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

