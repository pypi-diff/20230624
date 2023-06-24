# Comparing `tmp/FlightRadarAPI-1.2.8.tar.gz` & `tmp/FlightRadarAPI-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlightRadarAPI-1.2.8.tar", last modified: Sun May 28 20:11:57 2023, max compression
+gzip compressed data, was "FlightRadarAPI-1.3.0.tar", last modified: Sat Jun 24 16:18:36 2023, max compression
```

## Comparing `FlightRadarAPI-1.2.8.tar` & `FlightRadarAPI-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 20:11:57.943747 FlightRadarAPI-1.2.8/
-drwxrwxrwx   0        0        0        0 2023-05-28 20:11:57.928744 FlightRadarAPI-1.2.8/FlightRadar24/
--rw-rw-rw-   0        0        0      469 2023-05-28 19:59:55.000000 FlightRadarAPI-1.2.8/FlightRadar24/__init__.py
--rw-rw-rw-   0        0        0     5840 2023-05-28 19:59:55.000000 FlightRadarAPI-1.2.8/FlightRadar24/api.py
--rw-rw-rw-   0        0        0     2048 2023-05-28 19:59:55.000000 FlightRadarAPI-1.2.8/FlightRadar24/core.py
--rw-rw-rw-   0        0        0     9199 2023-03-19 22:45:09.000000 FlightRadarAPI-1.2.8/FlightRadar24/flight.py
--rw-rw-rw-   0        0        0     1753 2023-03-19 22:52:21.000000 FlightRadarAPI-1.2.8/FlightRadar24/request.py
-drwxrwxrwx   0        0        0        0 2023-05-28 20:11:57.942740 FlightRadarAPI-1.2.8/FlightRadarAPI.egg-info/
--rw-rw-rw-   0        0        0     3138 2023-05-28 20:11:57.000000 FlightRadarAPI-1.2.8/FlightRadarAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-05-28 20:11:57.000000 FlightRadarAPI-1.2.8/FlightRadarAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 20:11:57.000000 FlightRadarAPI-1.2.8/FlightRadarAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-28 20:11:57.000000 FlightRadarAPI-1.2.8/FlightRadarAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-28 20:11:57.000000 FlightRadarAPI-1.2.8/FlightRadarAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1110 2023-01-13 23:16:02.000000 FlightRadarAPI-1.2.8/LICENSE
--rw-rw-rw-   0        0        0     3138 2023-05-28 20:11:57.942740 FlightRadarAPI-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     2467 2023-01-29 02:09:37.000000 FlightRadarAPI-1.2.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-28 20:11:57.943747 FlightRadarAPI-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1053 2023-05-28 19:59:55.000000 FlightRadarAPI-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 16:18:36.674620 FlightRadarAPI-1.3.0/
+drwxrwxrwx   0        0        0        0 2023-06-24 16:18:36.644915 FlightRadarAPI-1.3.0/FlightRadar24/
+-rw-rw-rw-   0        0        0      469 2023-06-24 16:16:53.000000 FlightRadarAPI-1.3.0/FlightRadar24/__init__.py
+-rw-rw-rw-   0        0        0     6731 2023-06-24 16:06:24.000000 FlightRadarAPI-1.3.0/FlightRadar24/api.py
+-rw-rw-rw-   0        0        0     2048 2023-05-28 15:31:59.000000 FlightRadarAPI-1.3.0/FlightRadar24/core.py
+-rw-rw-rw-   0        0        0     9199 2023-04-03 15:49:14.000000 FlightRadarAPI-1.3.0/FlightRadar24/flight.py
+-rw-rw-rw-   0        0        0     1753 2023-05-28 15:37:24.000000 FlightRadarAPI-1.3.0/FlightRadar24/request.py
+drwxrwxrwx   0        0        0        0 2023-06-24 16:18:36.672711 FlightRadarAPI-1.3.0/FlightRadarAPI.egg-info/
+-rw-rw-rw-   0        0        0     3138 2023-06-24 16:18:36.000000 FlightRadarAPI-1.3.0/FlightRadarAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-06-24 16:18:36.000000 FlightRadarAPI-1.3.0/FlightRadarAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 16:18:36.000000 FlightRadarAPI-1.3.0/FlightRadarAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-24 16:18:36.000000 FlightRadarAPI-1.3.0/FlightRadarAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-24 16:18:36.000000 FlightRadarAPI-1.3.0/FlightRadarAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1110 2023-04-03 15:49:14.000000 FlightRadarAPI-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     3138 2023-06-24 16:18:36.673620 FlightRadarAPI-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2467 2023-04-03 15:49:14.000000 FlightRadarAPI-1.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 16:18:36.674620 FlightRadarAPI-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2023-04-03 15:50:42.000000 FlightRadarAPI-1.3.0/setup.py
```

### Comparing `FlightRadarAPI-1.2.8/FlightRadar24/api.py` & `FlightRadarAPI-1.3.0/FlightRadar24/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from .core import Core
 from .flight import Flight
 from .request import APIRequest
 
 from deprecated import deprecated
-from typing import Dict, List
+from typing import Any, Dict, List, Optional, Tuple
 
 
 class FlightRadar24API(object):
     """
     Flight Radar 24 API
     """
 
@@ -40,67 +40,95 @@
 
         request = APIRequest(Core.user_login_url, headers = Core.json_headers, data = data)
         self.__real_time_flight_tracker_config["enc"] = request.get_cookie("_frPl")
 
         return request.get_content()
 
     def get_airlines(self) -> List[Dict]:
-        # Get the data from Flightradar24.
+        """
+        Return a list with all airlines.
+        """
         request = APIRequest(Core.airlines_data_url, headers = Core.json_headers)
         return request.get_content()["rows"]
 
-    def get_airline_logo(self, iata: str, icao: str) -> str:
-        # Get the first airline logo URL.
+    def get_airline_logo(self, iata: str, icao: str) -> Optional[Tuple[bytes, str]]:
+        """
+        Download the logo of an airline from FlightRadar24 and return it as bytes.
+        """
         first_logo_url = Core.airline_logo_url.format(iata, icao)
 
-        # Check if there was a problem with the request. If not, the URL is returned.
-        first_status_code = APIRequest(first_logo_url, headers = Core.image_headers).get_status_code()
-        if not str(first_status_code).startswith("4"): return first_logo_url
+        # Try to get the image by the first URL option.
+        response = APIRequest(first_logo_url, headers = Core.image_headers)
+        status_code = response.get_status_code()
 
-        # Get the second airline logo URL.
+        if not str(status_code).startswith("4"):
+            return response.get_content(), first_logo_url.split(".")[-1]
+
+        # Get the image by the second airline logo URL.
         second_logo_url = Core.alternative_airline_logo_url.format(icao)
 
-        # Check if there was a problem with the request. If not, the URL is returned.
-        second_status_code = APIRequest(second_logo_url, headers = Core.image_headers).get_status_code()
-        if not str(second_status_code).startswith("4"): return second_logo_url
+        response = APIRequest(second_logo_url, headers = Core.image_headers)
+        status_code = response.get_status_code()
+
+        if not str(status_code).startswith("4"):
+            return response.get_content(), second_logo_url.split(".")[-1]
 
     def get_airport(self, code: str) -> Dict:
-        # Get the airport data from Flightradar24.
+        """
+        Return detailed information about an airport.
+
+        :param code: ICAO or IATA of the airport.
+        """
         request = APIRequest(Core.airport_data_url.format(code), headers = Core.json_headers)
         return request.get_content()["details"]
 
     def get_airports(self) -> List[Dict]:
-        # Get the airports data from Flightradar24.
+        """
+        Return a list with all airports.
+        """
         request = APIRequest(Core.airports_data_url, headers = Core.json_headers)
         return request.get_content()["rows"]
 
     def get_bounds(self, zone: Dict[str, float]) -> str:
-        # Convert coordinate dictionary (tl_y, tl_x, br_y, br_x) to string "y1, y2, x1, x2".
+        """
+        Convert coordinate dictionary to a string "y1, y2, x1, x2".
+
+        :param zone: Dictionary containing the following keys: tl_y, tl_x, br_y, br_x
+        """
         return "{},{},{},{}".format(zone["tl_y"], zone["br_y"] , zone["tl_x"], zone["br_x"])
 
-    def get_country_flag(self, country: str) -> str:
-        # Get the country flag image URL.
-        flag_url = Core.country_flag_url.format(country.lower().replace(" ", "-"))
+    def get_country_flag(self, country: str) -> Optional[Tuple[bytes, str]]:
+        """
+        Download the flag of a country from FlightRadar24 and return it as bytes.
 
+        :param country: Country name
+        """
+        flag_url = Core.country_flag_url.format(country.lower().replace(" ", "-"))
         headers = Core.image_headers.copy()
         
         if "origin" in headers:
-            headers.pop("origin") # Doesn't work for this request
+            headers.pop("origin")  # Does not work for this request.
 
-        # Check if there is a problem with the request. If not, the URL is returned.
-        status_code = APIRequest(flag_url, headers = headers).get_status_code()
-        if not str(status_code).startswith("4"): return flag_url
+        response = APIRequest(flag_url, headers = headers)
+        status_code = response.get_status_code()
 
-    def get_flight_details(self, flight_id: str) -> Dict:
-        # Get the flight details from Data Live Flightradar24.
+        if not str(status_code).startswith("4"):
+            return response.get_content(), flag_url.split(".")[-1]
+
+    def get_flight_details(self, flight_id: str) -> Dict[Any, Any]:
+        """
+        Return the flight details from Data Live Flightradar24.
+        """
         request = APIRequest(Core.flight_data_url.format(flight_id), headers = Core.json_headers)
         return request.get_content()
 
     def get_flights(self, airline: str = None, bounds: str = None, registration: str = None, aircraft_type: str = None) -> List[Flight]:
         """
+        Return a list of flights. See more options at set_real_time_flight_tracker_config() method.
+
         :param airline: the airline ICAO. Ex: "DAL"
         :param bounds: coordinates (y1, y2 ,x1, x2). Ex: "75.78,-75.78,-427.56,427.56"
         :param registration: aircraft registration
         :param aircraft_type: aircraft model code. Ex: "B737"
         """
 
         request_params = self.__real_time_flight_tracker_config.copy()
@@ -122,26 +150,33 @@
             # Get flights only.
             if flight_id[0].isnumeric():
                 flights.append(Flight(flight_id, flight_info))
 
         return flights
 
     def get_real_time_flight_tracker_config(self) -> Dict[str, str]:
+        """
+        Return the current config of the real time flight tracker, used by get_flights() method.
+        """
         return self.__real_time_flight_tracker_config.copy()
 
-    def get_zones(self) -> Dict:
-
-        # Get the zones data from Flightradar24.
+    def get_zones(self) -> Dict[str, Dict]:
+        """
+        Returns all major zones on the globe.
+        """
         request = APIRequest(Core.zones_data_url, headers = Core.json_headers)
         zones = request.get_content()
 
-        # Remove version information.
-        zones.pop("version")
+        if "version" in zones:
+            zones.pop("version")
+
         return zones
 
     def set_real_time_flight_tracker_config(self, **config: str) -> None:
-
+        """
+        Set config for the real time flight tracker, used by get_flights() method.
+        """
         for key, value in config.items():
 
             # Check if the parameter exists and if the value is numeric.
             if key in self.__real_time_flight_tracker_config and value.isnumeric():
                 self.__real_time_flight_tracker_config[key] = value
```

### Comparing `FlightRadarAPI-1.2.8/FlightRadar24/core.py` & `FlightRadarAPI-1.3.0/FlightRadar24/core.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.2.8/FlightRadar24/flight.py` & `FlightRadarAPI-1.3.0/FlightRadar24/flight.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.2.8/FlightRadar24/request.py` & `FlightRadarAPI-1.3.0/FlightRadar24/request.py`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.2.8/FlightRadarAPI.egg-info/PKG-INFO` & `FlightRadarAPI-1.3.0/FlightRadarAPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlightRadarAPI
-Version: 1.2.8
+Version: 1.3.0
 Summary: API for FlightRadar24
 Home-page: https://github.com/JeanExtreme002/FlightRadarAPI
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: flightradar24 api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `FlightRadarAPI-1.2.8/LICENSE` & `FlightRadarAPI-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.2.8/PKG-INFO` & `FlightRadarAPI-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlightRadarAPI
-Version: 1.2.8
+Version: 1.3.0
 Summary: API for FlightRadar24
 Home-page: https://github.com/JeanExtreme002/FlightRadarAPI
 Author: Jean Loui Bernard Silva de Jesus
 License: MIT
 Keywords: flightradar24 api
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `FlightRadarAPI-1.2.8/README.md` & `FlightRadarAPI-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `FlightRadarAPI-1.2.8/setup.py` & `FlightRadarAPI-1.3.0/setup.py`

 * *Files identical despite different names*

