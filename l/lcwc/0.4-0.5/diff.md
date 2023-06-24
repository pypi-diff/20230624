# Comparing `tmp/lcwc-0.4.tar.gz` & `tmp/lcwc-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcwc-0.4.tar", last modified: Wed Apr 19 17:07:00 2023, max compression
+gzip compressed data, was "lcwc-0.5.tar", last modified: Sat Jun 24 15:02:46 2023, max compression
```

## Comparing `lcwc-0.4.tar` & `lcwc-0.5.tar`

### file list

```diff
@@ -1,22 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 17:07:00.560031 lcwc-0.4/
--rw-rw-rw-   0        0        0     1058 2023-01-16 14:14:04.000000 lcwc-0.4/LICENSE
--rw-rw-rw-   0        0        0     1764 2023-04-19 17:07:00.559031 lcwc-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1110 2023-04-15 17:56:28.000000 lcwc-0.4/README.md
--rw-rw-rw-   0        0        0      789 2023-04-19 17:05:56.000000 lcwc-0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 17:07:00.560031 lcwc-0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-19 17:07:00.538030 lcwc-0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 17:07:00.552031 lcwc-0.4/src/lcwc/
--rw-rw-rw-   0        0        0        0 2023-04-19 15:24:37.000000 lcwc-0.4/src/lcwc/__init__.py
--rw-rw-rw-   0        0        0      324 2023-01-28 13:09:14.000000 lcwc-0.4/src/lcwc/category.py
--rw-rw-rw-   0        0        0      915 2023-04-08 10:55:17.000000 lcwc-0.4/src/lcwc/client.py
--rw-rw-rw-   0        0        0     5023 2023-04-19 17:04:26.000000 lcwc-0.4/src/lcwc/feedclient.py
--rw-rw-rw-   0        0        0     2314 2023-04-15 17:45:56.000000 lcwc-0.4/src/lcwc/incident.py
-drwxrwxrwx   0        0        0        0 2023-04-19 17:07:00.558034 lcwc-0.4/src/lcwc/utils/
--rw-rw-rw-   0        0        0     1794 2023-04-19 17:04:57.000000 lcwc-0.4/src/lcwc/utils/__init__.py
--rw-rw-rw-   0        0        0     3609 2023-04-15 17:56:04.000000 lcwc-0.4/src/lcwc/webclient.py
-drwxrwxrwx   0        0        0        0 2023-04-19 17:07:00.557031 lcwc-0.4/src/lcwc.egg-info/
--rw-rw-rw-   0        0        0     1764 2023-04-19 17:07:00.000000 lcwc-0.4/src/lcwc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-04-19 17:07:00.000000 lcwc-0.4/src/lcwc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 17:07:00.000000 lcwc-0.4/src/lcwc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-19 17:07:00.000000 lcwc-0.4/src/lcwc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-19 17:07:00.000000 lcwc-0.4/src/lcwc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 15:02:46.139338 lcwc-0.5/
+-rw-rw-rw-   0        0        0     1058 2023-01-16 14:14:04.000000 lcwc-0.5/LICENSE
+-rw-rw-rw-   0        0        0     2325 2023-06-24 15:02:46.137840 lcwc-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1671 2023-06-10 14:58:54.000000 lcwc-0.5/README.md
+-rw-rw-rw-   0        0        0      789 2023-06-24 15:01:35.000000 lcwc-0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-24 15:02:46.139338 lcwc-0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-24 15:02:46.101343 lcwc-0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-24 15:02:46.114838 lcwc-0.5/src/lcwc/
+-rw-rw-rw-   0        0        0       20 2023-06-24 15:01:21.000000 lcwc-0.5/src/lcwc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:02:46.124839 lcwc-0.5/src/lcwc/arcgis/
+-rw-rw-rw-   0        0        0       60 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/arcgis/__init__.py
+-rw-rw-rw-   0        0        0     6050 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/arcgis/client.py
+-rw-rw-rw-   0        0        0     1592 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/arcgis/incident.py
+-rw-rw-rw-   0        0        0      326 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/category.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:02:46.129839 lcwc-0.5/src/lcwc/feed/
+-rw-rw-rw-   0        0        0       64 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/feed/__init__.py
+-rw-rw-rw-   0        0        0     4201 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/feed/client.py
+-rw-rw-rw-   0        0        0      889 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/feed/incident.py
+-rw-rw-rw-   0        0        0     2344 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/incident.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:02:46.133339 lcwc-0.5/src/lcwc/utils/
+-rw-rw-rw-   0        0        0     2925 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/utils/__init__.py
+-rw-rw-rw-   0        0        0     4162 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/utils/restadapter.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:02:46.136839 lcwc-0.5/src/lcwc/web/
+-rw-rw-rw-   0        0        0       27 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/web/__init__.py
+-rw-rw-rw-   0        0        0     3681 2023-06-24 14:32:45.000000 lcwc-0.5/src/lcwc/web/client.py
+drwxrwxrwx   0        0        0        0 2023-06-24 15:02:46.120844 lcwc-0.5/src/lcwc.egg-info/
+-rw-rw-rw-   0        0        0     2325 2023-06-24 15:02:46.000000 lcwc-0.5/src/lcwc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2023-06-24 15:02:46.000000 lcwc-0.5/src/lcwc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 15:02:46.000000 lcwc-0.5/src/lcwc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-24 15:02:46.000000 lcwc-0.5/src/lcwc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-24 15:02:46.000000 lcwc-0.5/src/lcwc.egg-info/top_level.txt
```

### Comparing `lcwc-0.4/LICENSE` & `lcwc-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lcwc-0.4/PKG-INFO` & `lcwc-0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcwc
-Version: 0.4
+Version: 0.5
 Summary: Python library for fetching the Lancaster County-Wide Communications live incident list.
 Author-email: Nate Shoffner <nate.shoffner@gmail.com>
 Project-URL: Homepage, https://github.com/NateShoffner/python-lcwc
 Project-URL: Bug Tracker, https://github.com/NateShoffner/python-lcwc/issues
 Keywords: lcwc,lancaster,police,fire,ems,dispatch,911,incident
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,33 +13,42 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-lcwc
 
 python-lcwc is a Python library for the [LCWC](https://www.lcwc911.us/live-incident-list) incident feed.
 
-The library features both a web scraper and a RSS feed parser. The web scraper client is more reliable due to the RSS feed not categorizing incidents so we have to attempt to extrapolate the category from the incident description/units assigned. Functionally, it should be mostly accurate but edge cases may pop up. Addtionally, the feed parser offers a GUID. This is a unique identifier for each incident. The web client does not offer this.
+The library features multiple clients for retrieving incidents: a web scraper, an RSS feed parser, and an ArcGIS REST client. See notes below for more information.
 
 ## Installation
 
     pip install lcwc
 
 ## Example
 
 ```python
 
 import aiohttp
-from lcwc import feedclient
+from lcwc.feed import Client
 
-client = feedclient.IncidentFeedClient()
+client = Client()
 
 async with aiohttp.ClientSession() as session:
-    incidents = await client.fetch_and_parse(session)
+    incidents = await client.get_incidents(session)
 
     for incident in incidents:
         print(f'{incident.date} - {incident.description}')
 ```
 
-## TODO
+## Notes
 
-- [ ] Identify potential duplicate incidents reported under multiple categories (e.g. "Fire" and "Traffic" for vehicle fire)
-- [ ] Backing store and event emitter
+### Web Client
+
+The web client uses web-scraping which can be a bit limited for identification purposes but is the most reliable. The web client is the recommended client for use unless you need more granular information such as static identifers.
+
+### Feed Client
+
+The feed client uses the RSS feed and is similar to the web client except it overs an (admittedly arbitrary) GUID for each incident. Categorization can be a bit off since the feed doesn't supply that in formation so we have to attempt to extrapolate the category from the incident description/units assigned. Use the web client if you need more accurate categorization.
+
+### ArcGIS REST Client
+
+The ArcGIS REST client uses the ArcGIS REST API to retrieve incidents. This is the most accurate client since it uses the same data source as the LCWC website. This is still a bit of a prototype and may be subject to change. The ArcGIS REST client is the recommended client if you need more granular information such as static identifiers and coordinates.
```

### Comparing `lcwc-0.4/README.md` & `lcwc-0.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 # python-lcwc
 
 python-lcwc is a Python library for the [LCWC](https://www.lcwc911.us/live-incident-list) incident feed.
 
-The library features both a web scraper and a RSS feed parser. The web scraper client is more reliable due to the RSS feed not categorizing incidents so we have to attempt to extrapolate the category from the incident description/units assigned. Functionally, it should be mostly accurate but edge cases may pop up. Addtionally, the feed parser offers a GUID. This is a unique identifier for each incident. The web client does not offer this.
+The library features multiple clients for retrieving incidents: a web scraper, an RSS feed parser, and an ArcGIS REST client. See notes below for more information.
 
 ## Installation
 
     pip install lcwc
 
 ## Example
 
 ```python
 
 import aiohttp
-from lcwc import feedclient
+from lcwc.feed import Client
 
-client = feedclient.IncidentFeedClient()
+client = Client()
 
 async with aiohttp.ClientSession() as session:
-    incidents = await client.fetch_and_parse(session)
+    incidents = await client.get_incidents(session)
 
     for incident in incidents:
         print(f'{incident.date} - {incident.description}')
 ```
 
-## TODO
+## Notes
 
-- [ ] Identify potential duplicate incidents reported under multiple categories (e.g. "Fire" and "Traffic" for vehicle fire)
-- [ ] Backing store and event emitter
+### Web Client
+
+The web client uses web-scraping which can be a bit limited for identification purposes but is the most reliable. The web client is the recommended client for use unless you need more granular information such as static identifers.
+
+### Feed Client
+
+The feed client uses the RSS feed and is similar to the web client except it overs an (admittedly arbitrary) GUID for each incident. Categorization can be a bit off since the feed doesn't supply that in formation so we have to attempt to extrapolate the category from the incident description/units assigned. Use the web client if you need more accurate categorization.
+
+### ArcGIS REST Client
+
+The ArcGIS REST client uses the ArcGIS REST API to retrieve incidents. This is the most accurate client since it uses the same data source as the LCWC website. This is still a bit of a prototype and may be subject to change. The ArcGIS REST client is the recommended client if you need more granular information such as static identifiers and coordinates.
```

### Comparing `lcwc-0.4/pyproject.toml` & `lcwc-0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lcwc"
-version = "0.4"
+version = "0.5"
 authors = [
   { name="Nate Shoffner", email="nate.shoffner@gmail.com" },
 ]
 description = "Python library for fetching the Lancaster County-Wide Communications live incident list."
 keywords = ["lcwc", "lancaster", "police", "fire", "ems", "dispatch", "911", "incident"]
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `lcwc-0.4/src/lcwc/feedclient.py` & `lcwc-0.5/src/lcwc/feed/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,92 +1,91 @@
 import aiohttp
 import datetime
-import email.utils 
 import feedparser
-from lcwc.category import IncidentCategory
-from lcwc.client import Client
-from lcwc.incident import Incident
-from lcwc.utils import FIRE_UNIT_NAMES, LOCATION_NAMES, MEDICAL_UNIT_NAMES, determine_category
+import pytz
+from lcwc.feed.incident import FeedIncident
+from lcwc.utils import (
+    FIRE_UNIT_NAMES,
+    LOCATION_NAMES,
+    MEDICAL_UNIT_NAMES,
+    determine_category,
+)
 
-'''
+"""
 Example entry:
 
 <item>
     <title>MEDICAL EMERGENCY</title>
     <link>http://www.lcwc911.us/lcwc/lcwc/publiccad.asp</link>
     <description>MARTIC TOWNSHIP; BRIDGE VALLEY RD & LAKE ALDRED TER; MEDIC 56-1; </description>
     <pubDate>Wed, 25 Jan 2023 15:22:54 GMT</pubDate>
     <guid isPermaLink="false">792d7e14-34ef-4907-bb50-86c43cd3d570</guid>
 </item>
-'''
+"""
 
-# custom class to handle the guid attribute
-# a bit usless on its own but might be useful for statically identifying incidents
-# since apparently every detail is subject to change except maybe the timestamp
-class FeedIncident(Incident):
-    """ Represents an incident from the live incident feed """
-
-    def __init__(self, category: IncidentCategory, date: datetime, description: str, township: str, intersection: str, units: list[str] = [], guid: str = None) -> None:
-        super().__init__(category, date, description, township, intersection, units)
-        self._guid = guid
-
-    @property
-    def guid(self) -> str:
-        """ Returns the guid of the incident """
-        return self._guid
 
-class IncidentFeedClient(Client):
+class Client:
+    """Client for the incident RSS feed"""
 
-    URL = 'https://webcad.lcwc911.us/Pages/Public/LiveIncidentsFeed.aspx'
+    URL = "https://webcad.lcwc911.us/Pages/Public/LiveIncidentsFeed.aspx"
     """ The URL of the live incident feed """
 
-    def __init__(self):
-        super().__init__()
-
-    async def fetch(self, session: aiohttp.ClientSession, timeout: int = 10) -> bytes:
-        """ Gets the live incident feed and returns the xml as bytes
+    async def get_incidents(
+        self, session: aiohttp.ClientSession, timeout: int = 10
+    ) -> list[FeedIncident]:
+        """Gets the live incident feed and returns a list of incidents
 
         :param session: The aiohttp session to use
-        :param timeout: The timeout in seconds
-        :return: The xml of the live incident feed
-        :rtype: bytes
+        :param timeout: The timeout for the request
+        :return: A list of incidents
+        :rtype: list[Incident]
         """
-        async with session:
-            html = await super().fetch(session, timeout)
-            return html
+        response = None
+        async with session.get(self.URL, timeout=timeout) as resp:
+            if resp.status == 200:
+                response = await resp.read()
+            else:
+                raise Exception(f"Unable to fetch live incident feed: {resp.status}")
 
-    def parse(self, contents: bytes) -> list[FeedIncident]:
-        """ Parses the live incident feed and returns a list of incidents
+        active_incidents = self.__parse(response)
+        return active_incidents
+
+    def __parse(self, contents: bytes) -> list[FeedIncident]:
+        """Parses the live incident feed and returns a list of incidents
 
         :param contents: The xml of the live incident feed
         :return: A list of incidents
         :rtype: list[Incident]
         """
         incidents = []
 
         d = feedparser.parse(contents)
 
         def has_intersection(details_segment: str) -> bool:
             return any(k in details_segment for k in LOCATION_NAMES)
-            
+
         def has_unit_names(details_segment: str) -> bool:
-            return any(k in details_segment for k in FIRE_UNIT_NAMES + MEDICAL_UNIT_NAMES)
+            return any(
+                k in details_segment for k in FIRE_UNIT_NAMES + MEDICAL_UNIT_NAMES
+            )
 
         for entry in d.entries:
-
             guid = entry.guid
-            date = datetime.datetime.fromtimestamp( email.utils.mktime_tz(email.utils.parsedate_tz(entry.published)))
+            gmt_date = datetime.datetime.strptime(
+                entry.published, "%a, %d %b %Y %H:%M:%S %Z"
+            )
+            date = gmt_date.replace(tzinfo=datetime.timezone.utc).astimezone(pytz.utc)
             description = entry.title
 
             # Possible formats:
             # [township];[intersection];[units assigned]
             # [township];[intersection]
             # [township];[units assigned]
             # [township]
-            details_split = entry['description'].strip().split(';', maxsplit=3)
+            details_split = entry["description"].strip().split(";", maxsplit=3)
 
             # first item is always the township
             township = details_split[0].strip()
 
             intersection = None
             units = []
 
@@ -98,34 +97,26 @@
                     if has_intersection(details_split[1]):
                         intersection = details_split[1].strip()
                     if len(details_split) > 2 and has_unit_names(details_split[2]):
                         units = self.__extract_units(details_split[2])
 
             category = determine_category(description, units)
 
-            incidents.append(FeedIncident(category, date, description, township, intersection, units, guid))
+            incidents.append(
+                FeedIncident(
+                    category, date, description, township, intersection, units, guid
+                )
+            )
 
         return incidents
 
-    async def fetch_and_parse(self, session: aiohttp.ClientSession, timeout: int = 10) -> list[FeedIncident]:
-        """ Gets the live incident feed and returns a list of incidents
-
-        :param session: The aiohttp session to use
-        :param timeout: The timeout for the request
-        :return: A list of incidents
-        :rtype: list[Incident]
-        """
-        result = await self.fetch(session, timeout)
-        active_incidents = self.parse(result)
-        return active_incidents
-    
     def __extract_units(self, units_data: str) -> list[str]:
-        """ Extracts the units from the data string
+        """Extracts the units from the data string
 
         :param units_data: The data string containing the units
         :return: A list of units
         :rtype: list[str]
         """
         units_data = units_data.strip()
-        if units_data == '':
+        if units_data == "":
             return []
-        return [u.strip() for u in units_data.strip().split('<br />')]
+        return [u.strip() for u in units_data.strip().split("<br />")]
```

### Comparing `lcwc-0.4/src/lcwc/incident.py` & `lcwc-0.5/src/lcwc/incident.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 import datetime
 from lcwc.category import IncidentCategory
 
+
 class Incident:
-    """ Represents an incident"""
+    """Represents an incident"""
 
-    def __init__(self, category: IncidentCategory, date: datetime, description: str, township: str, intersection: str, units: list[str] = []) -> None:
+    def __init__(
+        self,
+        category: IncidentCategory,
+        date: datetime,
+        description: str,
+        township: str,
+        intersection: str,
+        units: list[str] = [],
+    ) -> None:
         """Constructor.
 
         :param IncidentCategory category: The category of the incident
-        
+
         :param datetime date: The date and time of the incident in local time (EST)
 
         :param str description: The description of the incident
 
         :param str township: The location of the incident location
 
         :param str intersection: The intersection of the incident location
@@ -25,47 +34,47 @@
         self._description = description
         self._township = township
         self._intersection = intersection
         self._units = units
 
     @property
     def category(self) -> IncidentCategory:
-        """ Returns the category of the incident """
+        """Returns the category of the incident"""
         return self._category
 
     @property
     def date(self) -> datetime:
-        """ Returns the date and time of the incident in local time (EST) """
+        """Returns the date and time of the incident"""
         return self._date
 
     @property
     def description(self) -> str:
-        """ Returns the incident description """
+        """Returns the incident description"""
         return self._description
 
     @property
     def township(self) -> str:
-        """ Returns the township of the incident location """
+        """Returns the township of the incident location"""
         return self._township
 
     @property
     def intersection(self) -> str:
-        """ Returns the intersection of the incident location """
+        """Returns the intersection of the incident location"""
         return self._intersection
 
     @property
     def location(self) -> str:
-        """ Returns the full location of the incident """
+        """Returns the full location of the incident"""
         if self._intersection is None:
             return self._township
         else:
-            return '\n'.join([self._intersection, self._township])
+            return "\n".join([self._intersection, self._township])
 
     @property
     def units(self) -> list[str]:
-        """ Returns a list of units responding to the incident """
+        """Returns a list of units responding to the incident"""
         return self._units
 
     @property
     def units_pending(self) -> bool:
-        """ Returns true if the incident has units pending """
-        return any([unit == 'PENDING' for unit in self._units])
+        """Returns true if the incident has units pending"""
+        return any([unit == "PENDING" for unit in self._units])
```

### Comparing `lcwc-0.4/src/lcwc/webclient.py` & `lcwc-0.5/src/lcwc/web/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,104 @@
 import datetime
 import aiohttp
+import pytz
 from bs4 import BeautifulSoup
 from lcwc.category import IncidentCategory
 from lcwc.incident import Incident
-from lcwc.client import Client
 
-TIMEZONE = 'US/Eastern'
-""" The timezone used on the LCWC website """
-
-DATE_FORMAT = '%a, %b %d, %Y %H:%M'
+DATE_FORMAT = "%a, %b %d, %Y %H:%M"
 """ The date format used on the LCWC website """
 
-class IncidentWebClient(Client):
-    """ Parses the live incident page from the LCWC website """
 
-    URL = 'https://www.lcwc911.us/live-incident-list'
-    """ The URL of the live incident page """
+class Client:
+    """Client for scraping the live incident page"""
 
-    def __init__(self):
-        super().__init__()
+    URL = "https://www.lcwc911.us/live-incident-list"
+    """ The URL of the live incident page """
 
-    async def fetch(self, session: aiohttp.ClientSession, timeout: int = 10) -> bytes:
-        """ Gets the live incident page and returns the html as bytes
+    async def get_incidents(
+        self, session: aiohttp.ClientSession, timeout: int = 10
+    ) -> list[Incident]:
+        """Fetches the live incident page and returns a list of incidents
 
         :param session: The aiohttp session to use
         :param timeout: The timeout in seconds
-        :return: The html of the live incident page
-        :rtype: bytes
+        :return: A list of incidents
+        :rtype: list[Incident]
         """
-        async with session:
-            html = await super().fetch(session, timeout)
-            return html
+        html = None
+        async with session.get(self.URL, timeout=timeout) as resp:
+            if resp.status == 200:
+                html = await resp.read()
+            else:
+                raise Exception(f"Unable to fetch live incident page: {resp.status}")
 
-    def parse(self, page_html: bytes) -> list[Incident]:
-        """ Parses the live incident page and returns a list of incidents
+        active_incidents = self.__parse(html)
+        return active_incidents
+
+    def __parse(self, page_html: bytes) -> list[Incident]:
+        """Parses the live incident page and returns a list of incidents
 
         :param page_html: The html of the live incident page
         :return: A list of incidents
         :rtype: list[Incident]
         """
 
         incidents = []
-        
-        soup = BeautifulSoup(page_html, 'html.parser')
-        containers = soup.find_all('div', class_='live-incident-container')
+
+        soup = BeautifulSoup(page_html, "html.parser")
+        containers = soup.find_all("div", class_="live-incident-container")
 
         for container in containers:
-            header = container.find('h2').text
+            header = container.find("h2").text
             category = IncidentCategory[header.split()[1].upper()]
 
-            table = container.find('table', class_='live-incidents')
+            table = container.find("table", class_="live-incidents")
 
-            rows = table.find_all('tr')
+            rows = table.find_all("tr")
 
             for row in rows:
-
-                date_row = row.find('td', class_='date-row')
-                incident_row = row.find('td', class_='incident-row')
-                location_row = row.find('td', class_='location-row')
-                units_row = row.find('td', class_='units-row')
-
-                if not date_row or not incident_row or not location_row or not units_row:
+                date_row = row.find("td", class_="date-row")
+                incident_row = row.find("td", class_="incident-row")
+                location_row = row.find("td", class_="location-row")
+                units_row = row.find("td", class_="units-row")
+
+                if (
+                    not date_row
+                    or not incident_row
+                    or not location_row
+                    or not units_row
+                ):
                     continue
 
-                date = datetime.datetime.strptime(date_row.text.strip(), DATE_FORMAT)
+                # convert date to UTC
+                local_tz = pytz.timezone("America/New_York")
+                raw_date = datetime.datetime.strptime(
+                    date_row.text.strip(), DATE_FORMAT
+                )
+                local_dt = local_tz.localize(raw_date, is_dst=None)
+                date = local_dt.astimezone(pytz.utc)
+
                 description = incident_row.text.strip().strip()
 
                 # split location by street(s) and township (if applicable)
-                location = [l.strip() for l in location_row.text.strip().split('\n')]
+                location = [l.strip() for l in location_row.text.strip().split("\n")]
 
                 if len(location) == 1:
                     intersection = None
                     township = location[0]
                 else:
                     intersection = location[0]
                     township = location[1]
 
                 # we have to decode manually because of internal <br/> tags
-                units = [u.strip() for u in units_row.decode_contents().strip().split('<br/>')]
-    
-                incident = Incident(category, date, description, township, intersection, units)
+                units = [
+                    u.strip()
+                    for u in units_row.decode_contents().strip().split("<br/>")
+                ]
+
+                incident = Incident(
+                    category, date, description, township, intersection, units
+                )
                 incidents.append(incident)
 
         return incidents
-
-    async def fetch_and_parse(self, session: aiohttp.ClientSession, timeout: int = 10) -> list[Incident]:
-        """ Gets the live incident page and returns a list of incidents
-
-        :param session: The aiohttp session to use
-        :param timeout: The timeout in seconds
-        :return: A list of incidents
-        :rtype: list[Incident]
-        """
-        result = await self.fetch(session)
-        active_incidents = self.parse(result)
-        return active_incidents
```

### Comparing `lcwc-0.4/src/lcwc.egg-info/PKG-INFO` & `lcwc-0.5/src/lcwc.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcwc
-Version: 0.4
+Version: 0.5
 Summary: Python library for fetching the Lancaster County-Wide Communications live incident list.
 Author-email: Nate Shoffner <nate.shoffner@gmail.com>
 Project-URL: Homepage, https://github.com/NateShoffner/python-lcwc
 Project-URL: Bug Tracker, https://github.com/NateShoffner/python-lcwc/issues
 Keywords: lcwc,lancaster,police,fire,ems,dispatch,911,incident
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,33 +13,42 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-lcwc
 
 python-lcwc is a Python library for the [LCWC](https://www.lcwc911.us/live-incident-list) incident feed.
 
-The library features both a web scraper and a RSS feed parser. The web scraper client is more reliable due to the RSS feed not categorizing incidents so we have to attempt to extrapolate the category from the incident description/units assigned. Functionally, it should be mostly accurate but edge cases may pop up. Addtionally, the feed parser offers a GUID. This is a unique identifier for each incident. The web client does not offer this.
+The library features multiple clients for retrieving incidents: a web scraper, an RSS feed parser, and an ArcGIS REST client. See notes below for more information.
 
 ## Installation
 
     pip install lcwc
 
 ## Example
 
 ```python
 
 import aiohttp
-from lcwc import feedclient
+from lcwc.feed import Client
 
-client = feedclient.IncidentFeedClient()
+client = Client()
 
 async with aiohttp.ClientSession() as session:
-    incidents = await client.fetch_and_parse(session)
+    incidents = await client.get_incidents(session)
 
     for incident in incidents:
         print(f'{incident.date} - {incident.description}')
 ```
 
-## TODO
+## Notes
 
-- [ ] Identify potential duplicate incidents reported under multiple categories (e.g. "Fire" and "Traffic" for vehicle fire)
-- [ ] Backing store and event emitter
+### Web Client
+
+The web client uses web-scraping which can be a bit limited for identification purposes but is the most reliable. The web client is the recommended client for use unless you need more granular information such as static identifers.
+
+### Feed Client
+
+The feed client uses the RSS feed and is similar to the web client except it overs an (admittedly arbitrary) GUID for each incident. Categorization can be a bit off since the feed doesn't supply that in formation so we have to attempt to extrapolate the category from the incident description/units assigned. Use the web client if you need more accurate categorization.
+
+### ArcGIS REST Client
+
+The ArcGIS REST client uses the ArcGIS REST API to retrieve incidents. This is the most accurate client since it uses the same data source as the LCWC website. This is still a bit of a prototype and may be subject to change. The ArcGIS REST client is the recommended client if you need more granular information such as static identifiers and coordinates.
```

