# Comparing `tmp/iso3166-updates-1.3.0.tar.gz` & `tmp/iso3166-updates-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iso3166-updates-1.3.0.tar", last modified: Fri Jun 23 23:41:25 2023, max compression
+gzip compressed data, was "iso3166-updates-1.3.1.tar", last modified: Sat Jun 24 13:15:40 2023, max compression
```

## Comparing `iso3166-updates-1.3.0.tar` & `iso3166-updates-1.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:41:25.484483 iso3166-updates-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-23 23:41:05.000000 iso3166-updates-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18983 2023-06-23 23:41:25.484483 iso3166-updates-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17369 2023-06-23 23:41:05.000000 iso3166-updates-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:41:25.480483 iso3166-updates-1.3.0/iso3166_updates/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-23 23:41:05.000000 iso3166-updates-1.3.0/iso3166_updates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35367 2023-06-23 23:41:05.000000 iso3166-updates-1.3.0/iso3166_updates/iso3166_updates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:41:25.484483 iso3166-updates-1.3.0/iso3166_updates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18983 2023-06-23 23:41:25.000000 iso3166-updates-1.3.0/iso3166_updates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-23 23:41:25.000000 iso3166-updates-1.3.0/iso3166_updates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 23:41:25.000000 iso3166-updates-1.3.0/iso3166_updates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 23:41:18.000000 iso3166-updates-1.3.0/iso3166_updates.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-23 23:41:25.000000 iso3166-updates-1.3.0/iso3166_updates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 23:41:25.000000 iso3166-updates-1.3.0/iso3166_updates.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-23 23:41:25.484483 iso3166-updates-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-23 23:41:05.000000 iso3166-updates-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:15:40.728347 iso3166-updates-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-24 13:15:14.000000 iso3166-updates-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-06-24 13:15:40.728347 iso3166-updates-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18162 2023-06-24 13:15:14.000000 iso3166-updates-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:15:40.728347 iso3166-updates-1.3.1/iso3166_updates/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-24 13:15:14.000000 iso3166-updates-1.3.1/iso3166_updates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35367 2023-06-24 13:15:14.000000 iso3166-updates-1.3.1/iso3166_updates/iso3166_updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:15:40.728347 iso3166-updates-1.3.1/iso3166_updates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-06-24 13:15:40.000000 iso3166-updates-1.3.1/iso3166_updates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-24 13:15:40.000000 iso3166-updates-1.3.1/iso3166_updates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 13:15:40.000000 iso3166-updates-1.3.1/iso3166_updates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 13:15:40.000000 iso3166-updates-1.3.1/iso3166_updates.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-24 13:15:40.000000 iso3166-updates-1.3.1/iso3166_updates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-24 13:15:40.000000 iso3166-updates-1.3.1/iso3166_updates.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-24 13:15:40.728347 iso3166-updates-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-24 13:15:14.000000 iso3166-updates-1.3.1/setup.py
```

### Comparing `iso3166-updates-1.3.0/LICENSE` & `iso3166-updates-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iso3166-updates-1.3.0/PKG-INFO` & `iso3166-updates-1.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,7 @@
-Metadata-Version: 2.1
-Name: iso3166-updates
-Version: 1.3.0
-Summary: A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
-Home-page: https://github.com/amckenna41/iso3166-updates
-Author: AJ McKenna, https://github.com/amckenna41
-Author-email: amckenna41@qub.ac.uk
-Maintainer: AJ McKenna
-License: MIT
-Download-URL: https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
-Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,csv,iso3166-2,iso3166-1,alpha-2,alpha-3
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License
-Classifier: License :: Free For Educational Use
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: docs
-License-File: LICENSE
-
 # iso3166-updates
 
 [![iso3166_updates](https://img.shields.io/pypi/v/iso3166-updates)](https://pypi.org/project/iso3166-updates/)
 [![pytest](https://github.com/amckenna41/iso3166-updates/workflows/Building%20and%20Testing/badge.svg)](https://github.com/amckenna41/iso3166-updates/actions?query=workflowBuilding%20and%20Testing)
 [![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/iso3166-updates/)
 [![License: MIT](https://img.shields.io/github/license/amckenna41/iso3166-updates)](https://opensource.org/licenses/MIT)
 <!-- [![CircleCI](https://circleci.com/gh/amckenna41/iso3166-updates.svg?style=svg&circle-token=d860bb64668be19d44f106841b80eb47a8b7e7e8)](https://app.circleci.com/pipelines/github/amckenna41/iso3166-updates) -->
@@ -85,30 +49,38 @@
 
 API
 ---
 An API is available that can be used to extract any applicable updates for a country via a URL. The API is available at the URL:
 
 > https://www.iso3166-updates.com/api
 
-Three query string parameters/paths are available in the API - `alpha2`, `year` and `months`. The 2 letter alpha-2 country code can be appeneded to the url as a query string parameter - "?alpha2=JP". A single alpha-2 or list of them can be passed to the API (e.g "FR", "DE", "HU, ID, MA"). The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "?year=2017", "2010-2015", "<2009", ">2002"). Finally, the months parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g "?month=6", "?month=48").
+Three query string parameters are available in the API - `alpha2`, `year` and `months`. 
+
+* The 2 letter alpha-2 country code can be appended to the url as a query string parameter or as its own path ("?alpha2=JP" or /alpha2/JP). A single alpha-2 or list of them can be passed to the API (e.g "?alpha2="FR, DE, HU, ID, MA" or /alpha2/FR,DE,HU,ID,MA). The 3 letter alpha-3 counterpart for each country's alpha-2 code can also be passed into the `alpha2` parameter (e.g "?alpha2="FRA, DEU, HUN, IDN, MAR" or /alpha2/FRA,DEU,HUN,IDN,MAR). 
+
+* The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "/year/2017", "2010-2015", "<2009", ">2002"). 
+
+* Finally, the months parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g "?months=2", "/months/6", "/months/48").
 
-The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON with all ISO 3166 updates. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure the hosting was switched to Vercel (https://vercel.com/).
+* If no input parameter values specified then all ISO 3166-2 updates for all countries and years will be gotten.
+
+The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure the hosting was switched to Vercel (https://vercel.com/).
 
 The API documentation and usage with all useful commands and examples to the API is available on the [README](https://github.com/amckenna41/iso3166-updates/blob/main/iso3166-updates-api/README.md) of the iso3166-updates-api folder. 
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_arch.png" alt="gcp_arch" height="200" width="400"/>
 </p>
 
 Staying up to date
 ------------------
 The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. 
-The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO 3166-2 wiki's to check for the latest updates within a certain period e.g the past 3-6 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data.
+The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO 3166-2 wiki's to check for the latest updates within a certain period e.g. the past 3-6 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data.
 
-Additionally, a GitHub Issue in the `iso3166-2` and `iso3166-flag-icons` repositories will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-2` and `iso3166-flag-icons` JSONs and repos.
+Additionally, a GitHub Issue in the custom-built `iso3166-updates`, `iso3166-2` and `iso3166-flag-icons` repositories will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-updates`, `iso3166-2` and `iso3166-flag-icons` JSONs and repos.
 
 Ultimately, this Cloud Function ensures that the software and assoicated APIs are up-to-date with the latest ISO 3166-2 information for all countries/territories/subdivisions etc.
 
 Requirements
 ------------
 * [python][python] >= 3.7
 * [pandas][pandas] >= 1.4.3
@@ -138,99 +110,102 @@
 ```python
 import iso3166_updates as iso3166_updates
 ```
 
 **Input parameters to get_updates function:**
 ```python
   # -alpha2 ALPHA2, --alpha2 ALPHA2
-  #                       Alpha-2 code/s of ISO3166 countries to check for updates.
+  #                       Alpha-2 code/s of ISO 3166 countries to check for updates.
   # -export_filename EXPORT_FILENAME, --export_filename EXPORT_FILENAME
-  #                       Filename for exported ISO3166 updates for CSV and JSON files.
+  #                       Filename for exported ISO 3166 updates for CSV and JSON files.
   # -export_folder EXPORT_FOLDER, --export_folder EXPORT_FOLDER
   #                       Folder where to store exported ISO files.
   # -export_json, --export_json
   #                       Whether to export all found updates to json.
   # -export_csv, --export_csv
   #                       Whether to export all found updates to csv files in export folder.
   # -year YEAR, --year YEAR
-  #                       Selected year to check for updates.
+  #                       Selected year/years, year ranges or year to check for updates greater
+  #                       than or less than specified year
   # -concat_updates, --concat_updates
   #                       Whether to concatenate updates of individual countrys into the same json file or seperate.
 ```
 
-**Get all listed changes/updates for all countries which happens by default if no alpha-2 codes specified in input param, export csv and json to folder "iso3166-updates":**
+**Get all listed changes/updates for all countries and years which happens by default if no alpha-2 codes or years specified in input paramaters, export csv and json to folder "iso3166-updates", print progress via verbose flag:**
 ```python
-iso3166_updates.get_updates(export_folder="iso3166-updates", export_json=1, export_csv=1)
-#exported files: /iso3166-updates/iso3166-updates.json and /iso3166-updates/iso3166-updates.csv
+iso3166_updates.get_updates(export_folder="iso3166-updates", export_json=1, export_csv=1, verbose=1)
+#exported files: /iso3166-updates.json and /iso3166-updates/iso3166-updates.csv
 ```
 
-**Get all listed changes/updates for Andorra from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:AD), export csv and json to folder "iso3166-updates":**
+**Get all listed ISO 3166-2 changes/updates for Andorra, export csv and json to folder "iso3166-updates":**
 ```python
 iso3166_updates.get_updates("AD", export_folder="iso3166-updates", export_json=1, export_csv=1)
-#exported files: /iso3166-updates/iso3166-updates-AD.json and /iso3166-updates/iso3166-updates-AD.csv
+#exported files: /iso3166-updates-AD.json and /iso3166-updates/iso3166-updates-AD.csv
 ```
 
-**Get all listed changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates":**
+**Get all listed ISO 3166-2 changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates", print progress using verbose flag:**
 ```python
-iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=0)
+iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=0, verbose=1)
 #exported files: /iso3166-updates/iso3166-updates-BA,DE,FR,HU,PY.json
 ```
 
-**Get any listed changes/updates for HU, IT, JA, KE from wiki, in the year 2018, export only to JSON with filename "iso3166-updates.json" and seperate updates into sepetate JSON files:**
+**Get any listed ISO 3166-2 changes/updates for HU, IT, JA, KE, in the year 2018, export only to JSON with filename "iso3166-updates.json" and seperate updates into sepetate JSON files (concat_updates=False):**
 ```python
 iso3166_updates.get_updates("HU, IT, JA, KE", year="2018", export_json=1, export_csv=0, export_filename="iso3166-updates", concat_updates=0)
 #exported files: /iso3166-updates/iso3166-updates-HU,IT,JA,KE-2018.json
 ```
 
-**Get any listed changes/updates for Ireland from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:IE), between years of 2012 and 2021, use default parameters:**
+**Get any listed ISO 3166-2 changes/updates for Ireland, between years 2012 and 2021, use default parameters (export to json but not csv):**
 ```python
 iso3166_updates.get_updates("IE", year="2012-2021")
 #exported files: /iso3166-updates/iso3166-updates-IE_2012-2021.json
 ```
 
-**Get any listed changes/updates for Tanzania from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:TZ), with updates years >=2015, export only to CSV with filename iso3166-output":**
+**Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >=2015, export only to CSV with filename iso3166-output":**
 ```python
 iso3166_updates.get_updates("TA", year=">2015", export_filename="iso3166-output", export_json=0, export_csv=1)
 #exported files: /iso3166-updates/iso3166-output-TA_>2015.csv
 ```
 
-**Get any listed changes/updates for Yemen from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:YE), with updates years < 2010, use default parameters:**
+**Get any listed ISO 3166-2 changes/updates for Yemen, with updates with year < 2010, use default parameters (export to json but not csv):**
 ```python
 iso3166_updates.get_updates("YE", year="<2010")
 #exported files: /iso3166-updates/iso3166-output-YE_<2010.json
 ```
 ## Terminal/Command Line
 
-**Get all listed changes/updates for all countries, export csv and json to folder "iso3166-updates", print progress using verbose parameter:** 
+The software functions can also be run from the cmd/terminal interface, when the script is called the get_updates() function will be called. The script accepts the same parameter names as the get_updates() function.
+
+**Get all listed ISO 3166-2 changes/updates for all countries, export csv and json to folder "iso3166-updates", print progress using verbose flag:** 
 ```bash
 python3 iso3166_updates.py --export_folder="iso3166-updates" --export_csv --export_json --verbose
 ```
 
-**Get all listed changes/updates for BY, DJ, ET, LY, PA for year range 2005-2010, export only CSV of updates to export folder "iso3166-updates", print progress using verbose parameter:**
+**Get all listed ISO 3166-2 changes/updates for BY, DJ, ET, LY, PA for year range 2005-2010, export only CSV of updates to export folder "iso3166-updates", print progress using verbose flag:**
 ```bash
 python3 iso3166_updates.py --alpha2="BY, DJ, ET, LY, PA" --year="2005-2010" --export_folder="iso3166-updates" --export_csv --no-export_json --verbose
 ```
 
-The output to the above functions for the updates/changes to a ISO 3166-2 country returns 4 columns: 
-<b>Edition/Newsletter, Date Issued, Code/Subdivision change</b> and <b>Description of change in newsletter.</b> For the CSV export, if more than one country input then an addition primary key column <b>Country Code</b> will be prepended to the first column, which will be the 2 letter ISO 3166-1 country code. 
+The output to the above functions for the updates/changes to an ISO 3166-2 country returns 4 columns: 
+<b>Edition/Newsletter, Date Issued, Code/Subdivision change</b> and <b>Description of change in newsletter.</b> For the CSV export, if more than one country input, then an additional primary key column <b>Country Code</b> will be prepended to the first column, which will be the 2 letter ISO 3166-1 country code. 
 
-* Edition/Newsletter: Name and or edition of newsletter that ISO 3166-2 change/update was communicated in.
+* Edition/Newsletter: Name and or edition of newsletter that the ISO 3166-2 change/update was communicated in.
 * Date Issued: Date that the change was communicated.
 * Code/Subdivision change: Overall summary of change/update made.
 * Description of change in newsletter: More in-depth info about the change/update that was made.
 
-E.g. The output format of the exported CSV for AD (Andorra) is:
+E.g. The output format of the exported <b>CSV</b> for AD (Andorra) is:
 
 | Edition/Newsletter | Date Issued | Code/Subdivision change | Description of change in newsletter |   
 |:-------------------|:------------|------------------------------------:|------------------------:|
 | Newsletter I-8     | 2007-04-17  | Subdivisions added: 7 parishes...   | Addition of the administrative subdivisions...                 | 
 | Online Browsing Platform (OBP) | 2014-11-03 | No subdivision changes listed | Update List Source |
 | Online Browsing Platform (OBP) | 2015-11-27 | No subdivision changes listed | Update List Source | 
 
-E.g. The output format of the exported JSON for AD (Andorra) is:
+E.g. The output format of the exported <b>JSON</b> for AD (Andorra) is:
 ```javascript
 {
   AD: [
       {
         "Code/Subdivision change": "",
         "Date Issued": "2015-11-27",
         "Description of change in newsletter": "Update List Source",
@@ -288,9 +263,8 @@
 [python]: https://www.python.org/downloads/release/python-360/
 [pandas]: https://pandas.pydata.org/
 [numpy]: https://numpy.org/
 [requests]: https://requests.readthedocs.io/
 [beautifulsoup4]: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
 [iso3166]: https://github.com/deactivated/python-iso3166
 [PyPi]: https://pypi.org/project/iso3166-updates/
-[Issues]: https://github.com/amckenna41/iso3166-updates/issues
-
+[Issues]: https://github.com/amckenna41/iso3166-updates/issues
```

### Comparing `iso3166-updates-1.3.0/README.md` & `iso3166-updates-1.3.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,42 @@
+Metadata-Version: 2.1
+Name: iso3166-updates
+Version: 1.3.1
+Summary: A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
+Home-page: https://github.com/amckenna41/iso3166-updates
+Author: AJ McKenna, https://github.com/amckenna41
+Author-email: amckenna41@qub.ac.uk
+Maintainer: AJ McKenna
+License: MIT
+Download-URL: https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
+Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,csv,iso3166-2,iso3166-1,alpha-2,alpha-3
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Free For Educational Use
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: docs
+License-File: LICENSE
+
 # iso3166-updates
 
 [![iso3166_updates](https://img.shields.io/pypi/v/iso3166-updates)](https://pypi.org/project/iso3166-updates/)
 [![pytest](https://github.com/amckenna41/iso3166-updates/workflows/Building%20and%20Testing/badge.svg)](https://github.com/amckenna41/iso3166-updates/actions?query=workflowBuilding%20and%20Testing)
 [![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/iso3166-updates/)
 [![License: MIT](https://img.shields.io/github/license/amckenna41/iso3166-updates)](https://opensource.org/licenses/MIT)
 <!-- [![CircleCI](https://circleci.com/gh/amckenna41/iso3166-updates.svg?style=svg&circle-token=d860bb64668be19d44f106841b80eb47a8b7e7e8)](https://app.circleci.com/pipelines/github/amckenna41/iso3166-updates) -->
@@ -49,30 +84,38 @@
 
 API
 ---
 An API is available that can be used to extract any applicable updates for a country via a URL. The API is available at the URL:
 
 > https://www.iso3166-updates.com/api
 
-Three query string parameters/paths are available in the API - `alpha2`, `year` and `months`. The 2 letter alpha-2 country code can be appeneded to the url as a query string parameter - "?alpha2=JP". A single alpha-2 or list of them can be passed to the API (e.g "FR", "DE", "HU, ID, MA"). The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "?year=2017", "2010-2015", "<2009", ">2002"). Finally, the months parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g "?month=6", "?month=48").
+Three query string parameters are available in the API - `alpha2`, `year` and `months`. 
+
+* The 2 letter alpha-2 country code can be appended to the url as a query string parameter or as its own path ("?alpha2=JP" or /alpha2/JP). A single alpha-2 or list of them can be passed to the API (e.g "?alpha2="FR, DE, HU, ID, MA" or /alpha2/FR,DE,HU,ID,MA). The 3 letter alpha-3 counterpart for each country's alpha-2 code can also be passed into the `alpha2` parameter (e.g "?alpha2="FRA, DEU, HUN, IDN, MAR" or /alpha2/FRA,DEU,HUN,IDN,MAR). 
+
+* The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "/year/2017", "2010-2015", "<2009", ">2002"). 
+
+* Finally, the months parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g "?months=2", "/months/6", "/months/48").
 
-The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON with all ISO 3166 updates. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure the hosting was switched to Vercel (https://vercel.com/).
+* If no input parameter values specified then all ISO 3166-2 updates for all countries and years will be gotten.
+
+The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure the hosting was switched to Vercel (https://vercel.com/).
 
 The API documentation and usage with all useful commands and examples to the API is available on the [README](https://github.com/amckenna41/iso3166-updates/blob/main/iso3166-updates-api/README.md) of the iso3166-updates-api folder. 
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_arch.png" alt="gcp_arch" height="200" width="400"/>
 </p>
 
 Staying up to date
 ------------------
 The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. 
-The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO 3166-2 wiki's to check for the latest updates within a certain period e.g the past 3-6 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data.
+The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO 3166-2 wiki's to check for the latest updates within a certain period e.g. the past 3-6 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data.
 
-Additionally, a GitHub Issue in the `iso3166-2` and `iso3166-flag-icons` repositories will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-2` and `iso3166-flag-icons` JSONs and repos.
+Additionally, a GitHub Issue in the custom-built `iso3166-updates`, `iso3166-2` and `iso3166-flag-icons` repositories will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-updates`, `iso3166-2` and `iso3166-flag-icons` JSONs and repos.
 
 Ultimately, this Cloud Function ensures that the software and assoicated APIs are up-to-date with the latest ISO 3166-2 information for all countries/territories/subdivisions etc.
 
 Requirements
 ------------
 * [python][python] >= 3.7
 * [pandas][pandas] >= 1.4.3
@@ -102,99 +145,102 @@
 ```python
 import iso3166_updates as iso3166_updates
 ```
 
 **Input parameters to get_updates function:**
 ```python
   # -alpha2 ALPHA2, --alpha2 ALPHA2
-  #                       Alpha-2 code/s of ISO3166 countries to check for updates.
+  #                       Alpha-2 code/s of ISO 3166 countries to check for updates.
   # -export_filename EXPORT_FILENAME, --export_filename EXPORT_FILENAME
-  #                       Filename for exported ISO3166 updates for CSV and JSON files.
+  #                       Filename for exported ISO 3166 updates for CSV and JSON files.
   # -export_folder EXPORT_FOLDER, --export_folder EXPORT_FOLDER
   #                       Folder where to store exported ISO files.
   # -export_json, --export_json
   #                       Whether to export all found updates to json.
   # -export_csv, --export_csv
   #                       Whether to export all found updates to csv files in export folder.
   # -year YEAR, --year YEAR
-  #                       Selected year to check for updates.
+  #                       Selected year/years, year ranges or year to check for updates greater
+  #                       than or less than specified year
   # -concat_updates, --concat_updates
   #                       Whether to concatenate updates of individual countrys into the same json file or seperate.
 ```
 
-**Get all listed changes/updates for all countries which happens by default if no alpha-2 codes specified in input param, export csv and json to folder "iso3166-updates":**
+**Get all listed changes/updates for all countries and years which happens by default if no alpha-2 codes or years specified in input paramaters, export csv and json to folder "iso3166-updates", print progress via verbose flag:**
 ```python
-iso3166_updates.get_updates(export_folder="iso3166-updates", export_json=1, export_csv=1)
-#exported files: /iso3166-updates/iso3166-updates.json and /iso3166-updates/iso3166-updates.csv
+iso3166_updates.get_updates(export_folder="iso3166-updates", export_json=1, export_csv=1, verbose=1)
+#exported files: /iso3166-updates.json and /iso3166-updates/iso3166-updates.csv
 ```
 
-**Get all listed changes/updates for Andorra from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:AD), export csv and json to folder "iso3166-updates":**
+**Get all listed ISO 3166-2 changes/updates for Andorra, export csv and json to folder "iso3166-updates":**
 ```python
 iso3166_updates.get_updates("AD", export_folder="iso3166-updates", export_json=1, export_csv=1)
-#exported files: /iso3166-updates/iso3166-updates-AD.json and /iso3166-updates/iso3166-updates-AD.csv
+#exported files: /iso3166-updates-AD.json and /iso3166-updates/iso3166-updates-AD.csv
 ```
 
-**Get all listed changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates":**
+**Get all listed ISO 3166-2 changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates", print progress using verbose flag:**
 ```python
-iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=0)
+iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=0, verbose=1)
 #exported files: /iso3166-updates/iso3166-updates-BA,DE,FR,HU,PY.json
 ```
 
-**Get any listed changes/updates for HU, IT, JA, KE from wiki, in the year 2018, export only to JSON with filename "iso3166-updates.json" and seperate updates into sepetate JSON files:**
+**Get any listed ISO 3166-2 changes/updates for HU, IT, JA, KE, in the year 2018, export only to JSON with filename "iso3166-updates.json" and seperate updates into sepetate JSON files (concat_updates=False):**
 ```python
 iso3166_updates.get_updates("HU, IT, JA, KE", year="2018", export_json=1, export_csv=0, export_filename="iso3166-updates", concat_updates=0)
 #exported files: /iso3166-updates/iso3166-updates-HU,IT,JA,KE-2018.json
 ```
 
-**Get any listed changes/updates for Ireland from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:IE), between years of 2012 and 2021, use default parameters:**
+**Get any listed ISO 3166-2 changes/updates for Ireland, between years 2012 and 2021, use default parameters (export to json but not csv):**
 ```python
 iso3166_updates.get_updates("IE", year="2012-2021")
 #exported files: /iso3166-updates/iso3166-updates-IE_2012-2021.json
 ```
 
-**Get any listed changes/updates for Tanzania from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:TZ), with updates years >=2015, export only to CSV with filename iso3166-output":**
+**Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >=2015, export only to CSV with filename iso3166-output":**
 ```python
 iso3166_updates.get_updates("TA", year=">2015", export_filename="iso3166-output", export_json=0, export_csv=1)
 #exported files: /iso3166-updates/iso3166-output-TA_>2015.csv
 ```
 
-**Get any listed changes/updates for Yemen from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:YE), with updates years < 2010, use default parameters:**
+**Get any listed ISO 3166-2 changes/updates for Yemen, with updates with year < 2010, use default parameters (export to json but not csv):**
 ```python
 iso3166_updates.get_updates("YE", year="<2010")
 #exported files: /iso3166-updates/iso3166-output-YE_<2010.json
 ```
 ## Terminal/Command Line
 
-**Get all listed changes/updates for all countries, export csv and json to folder "iso3166-updates", print progress using verbose parameter:** 
+The software functions can also be run from the cmd/terminal interface, when the script is called the get_updates() function will be called. The script accepts the same parameter names as the get_updates() function.
+
+**Get all listed ISO 3166-2 changes/updates for all countries, export csv and json to folder "iso3166-updates", print progress using verbose flag:** 
 ```bash
 python3 iso3166_updates.py --export_folder="iso3166-updates" --export_csv --export_json --verbose
 ```
 
-**Get all listed changes/updates for BY, DJ, ET, LY, PA for year range 2005-2010, export only CSV of updates to export folder "iso3166-updates", print progress using verbose parameter:**
+**Get all listed ISO 3166-2 changes/updates for BY, DJ, ET, LY, PA for year range 2005-2010, export only CSV of updates to export folder "iso3166-updates", print progress using verbose flag:**
 ```bash
 python3 iso3166_updates.py --alpha2="BY, DJ, ET, LY, PA" --year="2005-2010" --export_folder="iso3166-updates" --export_csv --no-export_json --verbose
 ```
 
-The output to the above functions for the updates/changes to a ISO 3166-2 country returns 4 columns: 
-<b>Edition/Newsletter, Date Issued, Code/Subdivision change</b> and <b>Description of change in newsletter.</b> For the CSV export, if more than one country input then an addition primary key column <b>Country Code</b> will be prepended to the first column, which will be the 2 letter ISO 3166-1 country code. 
+The output to the above functions for the updates/changes to an ISO 3166-2 country returns 4 columns: 
+<b>Edition/Newsletter, Date Issued, Code/Subdivision change</b> and <b>Description of change in newsletter.</b> For the CSV export, if more than one country input, then an additional primary key column <b>Country Code</b> will be prepended to the first column, which will be the 2 letter ISO 3166-1 country code. 
 
-* Edition/Newsletter: Name and or edition of newsletter that ISO 3166-2 change/update was communicated in.
+* Edition/Newsletter: Name and or edition of newsletter that the ISO 3166-2 change/update was communicated in.
 * Date Issued: Date that the change was communicated.
 * Code/Subdivision change: Overall summary of change/update made.
 * Description of change in newsletter: More in-depth info about the change/update that was made.
 
-E.g. The output format of the exported CSV for AD (Andorra) is:
+E.g. The output format of the exported <b>CSV</b> for AD (Andorra) is:
 
 | Edition/Newsletter | Date Issued | Code/Subdivision change | Description of change in newsletter |   
 |:-------------------|:------------|------------------------------------:|------------------------:|
 | Newsletter I-8     | 2007-04-17  | Subdivisions added: 7 parishes...   | Addition of the administrative subdivisions...                 | 
 | Online Browsing Platform (OBP) | 2014-11-03 | No subdivision changes listed | Update List Source |
 | Online Browsing Platform (OBP) | 2015-11-27 | No subdivision changes listed | Update List Source | 
 
-E.g. The output format of the exported JSON for AD (Andorra) is:
+E.g. The output format of the exported <b>JSON</b> for AD (Andorra) is:
 ```javascript
 {
   AD: [
       {
         "Code/Subdivision change": "",
         "Date Issued": "2015-11-27",
         "Description of change in newsletter": "Update List Source",
@@ -252,8 +298,9 @@
 [python]: https://www.python.org/downloads/release/python-360/
 [pandas]: https://pandas.pydata.org/
 [numpy]: https://numpy.org/
 [requests]: https://requests.readthedocs.io/
 [beautifulsoup4]: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
 [iso3166]: https://github.com/deactivated/python-iso3166
 [PyPi]: https://pypi.org/project/iso3166-updates/
-[Issues]: https://github.com/amckenna41/iso3166-updates/issues
+[Issues]: https://github.com/amckenna41/iso3166-updates/issues
+
```

### Comparing `iso3166-updates-1.3.0/iso3166_updates/iso3166_updates.py` & `iso3166-updates-1.3.1/iso3166_updates/iso3166_updates.py`

 * *Files identical despite different names*

### Comparing `iso3166-updates-1.3.0/iso3166_updates.egg-info/PKG-INFO` & `iso3166-updates-1.3.1/iso3166_updates.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iso3166-updates
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 Home-page: https://github.com/amckenna41/iso3166-updates
 Author: AJ McKenna, https://github.com/amckenna41
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
@@ -14,15 +14,14 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Free For Educational Use
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
@@ -85,30 +84,38 @@
 
 API
 ---
 An API is available that can be used to extract any applicable updates for a country via a URL. The API is available at the URL:
 
 > https://www.iso3166-updates.com/api
 
-Three query string parameters/paths are available in the API - `alpha2`, `year` and `months`. The 2 letter alpha-2 country code can be appeneded to the url as a query string parameter - "?alpha2=JP". A single alpha-2 or list of them can be passed to the API (e.g "FR", "DE", "HU, ID, MA"). The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "?year=2017", "2010-2015", "<2009", ">2002"). Finally, the months parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g "?month=6", "?month=48").
+Three query string parameters are available in the API - `alpha2`, `year` and `months`. 
 
-The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON with all ISO 3166 updates. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure the hosting was switched to Vercel (https://vercel.com/).
+* The 2 letter alpha-2 country code can be appended to the url as a query string parameter or as its own path ("?alpha2=JP" or /alpha2/JP). A single alpha-2 or list of them can be passed to the API (e.g "?alpha2="FR, DE, HU, ID, MA" or /alpha2/FR,DE,HU,ID,MA). The 3 letter alpha-3 counterpart for each country's alpha-2 code can also be passed into the `alpha2` parameter (e.g "?alpha2="FRA, DEU, HUN, IDN, MAR" or /alpha2/FRA,DEU,HUN,IDN,MAR). 
+
+* The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "/year/2017", "2010-2015", "<2009", ">2002"). 
+
+* Finally, the months parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g "?months=2", "/months/6", "/months/48").
+
+* If no input parameter values specified then all ISO 3166-2 updates for all countries and years will be gotten.
+
+The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure the hosting was switched to Vercel (https://vercel.com/).
 
 The API documentation and usage with all useful commands and examples to the API is available on the [README](https://github.com/amckenna41/iso3166-updates/blob/main/iso3166-updates-api/README.md) of the iso3166-updates-api folder. 
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_arch.png" alt="gcp_arch" height="200" width="400"/>
 </p>
 
 Staying up to date
 ------------------
 The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. 
-The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO 3166-2 wiki's to check for the latest updates within a certain period e.g the past 3-6 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data.
+The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO 3166-2 wiki's to check for the latest updates within a certain period e.g. the past 3-6 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data.
 
-Additionally, a GitHub Issue in the `iso3166-2` and `iso3166-flag-icons` repositories will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-2` and `iso3166-flag-icons` JSONs and repos.
+Additionally, a GitHub Issue in the custom-built `iso3166-updates`, `iso3166-2` and `iso3166-flag-icons` repositories will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-updates`, `iso3166-2` and `iso3166-flag-icons` JSONs and repos.
 
 Ultimately, this Cloud Function ensures that the software and assoicated APIs are up-to-date with the latest ISO 3166-2 information for all countries/territories/subdivisions etc.
 
 Requirements
 ------------
 * [python][python] >= 3.7
 * [pandas][pandas] >= 1.4.3
@@ -138,99 +145,102 @@
 ```python
 import iso3166_updates as iso3166_updates
 ```
 
 **Input parameters to get_updates function:**
 ```python
   # -alpha2 ALPHA2, --alpha2 ALPHA2
-  #                       Alpha-2 code/s of ISO3166 countries to check for updates.
+  #                       Alpha-2 code/s of ISO 3166 countries to check for updates.
   # -export_filename EXPORT_FILENAME, --export_filename EXPORT_FILENAME
-  #                       Filename for exported ISO3166 updates for CSV and JSON files.
+  #                       Filename for exported ISO 3166 updates for CSV and JSON files.
   # -export_folder EXPORT_FOLDER, --export_folder EXPORT_FOLDER
   #                       Folder where to store exported ISO files.
   # -export_json, --export_json
   #                       Whether to export all found updates to json.
   # -export_csv, --export_csv
   #                       Whether to export all found updates to csv files in export folder.
   # -year YEAR, --year YEAR
-  #                       Selected year to check for updates.
+  #                       Selected year/years, year ranges or year to check for updates greater
+  #                       than or less than specified year
   # -concat_updates, --concat_updates
   #                       Whether to concatenate updates of individual countrys into the same json file or seperate.
 ```
 
-**Get all listed changes/updates for all countries which happens by default if no alpha-2 codes specified in input param, export csv and json to folder "iso3166-updates":**
+**Get all listed changes/updates for all countries and years which happens by default if no alpha-2 codes or years specified in input paramaters, export csv and json to folder "iso3166-updates", print progress via verbose flag:**
 ```python
-iso3166_updates.get_updates(export_folder="iso3166-updates", export_json=1, export_csv=1)
-#exported files: /iso3166-updates/iso3166-updates.json and /iso3166-updates/iso3166-updates.csv
+iso3166_updates.get_updates(export_folder="iso3166-updates", export_json=1, export_csv=1, verbose=1)
+#exported files: /iso3166-updates.json and /iso3166-updates/iso3166-updates.csv
 ```
 
-**Get all listed changes/updates for Andorra from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:AD), export csv and json to folder "iso3166-updates":**
+**Get all listed ISO 3166-2 changes/updates for Andorra, export csv and json to folder "iso3166-updates":**
 ```python
 iso3166_updates.get_updates("AD", export_folder="iso3166-updates", export_json=1, export_csv=1)
-#exported files: /iso3166-updates/iso3166-updates-AD.json and /iso3166-updates/iso3166-updates-AD.csv
+#exported files: /iso3166-updates-AD.json and /iso3166-updates/iso3166-updates-AD.csv
 ```
 
-**Get all listed changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates":**
+**Get all listed ISO 3166-2 changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates", print progress using verbose flag:**
 ```python
-iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=0)
+iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=0, verbose=1)
 #exported files: /iso3166-updates/iso3166-updates-BA,DE,FR,HU,PY.json
 ```
 
-**Get any listed changes/updates for HU, IT, JA, KE from wiki, in the year 2018, export only to JSON with filename "iso3166-updates.json" and seperate updates into sepetate JSON files:**
+**Get any listed ISO 3166-2 changes/updates for HU, IT, JA, KE, in the year 2018, export only to JSON with filename "iso3166-updates.json" and seperate updates into sepetate JSON files (concat_updates=False):**
 ```python
 iso3166_updates.get_updates("HU, IT, JA, KE", year="2018", export_json=1, export_csv=0, export_filename="iso3166-updates", concat_updates=0)
 #exported files: /iso3166-updates/iso3166-updates-HU,IT,JA,KE-2018.json
 ```
 
-**Get any listed changes/updates for Ireland from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:IE), between years of 2012 and 2021, use default parameters:**
+**Get any listed ISO 3166-2 changes/updates for Ireland, between years 2012 and 2021, use default parameters (export to json but not csv):**
 ```python
 iso3166_updates.get_updates("IE", year="2012-2021")
 #exported files: /iso3166-updates/iso3166-updates-IE_2012-2021.json
 ```
 
-**Get any listed changes/updates for Tanzania from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:TZ), with updates years >=2015, export only to CSV with filename iso3166-output":**
+**Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >=2015, export only to CSV with filename iso3166-output":**
 ```python
 iso3166_updates.get_updates("TA", year=">2015", export_filename="iso3166-output", export_json=0, export_csv=1)
 #exported files: /iso3166-updates/iso3166-output-TA_>2015.csv
 ```
 
-**Get any listed changes/updates for Yemen from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:YE), with updates years < 2010, use default parameters:**
+**Get any listed ISO 3166-2 changes/updates for Yemen, with updates with year < 2010, use default parameters (export to json but not csv):**
 ```python
 iso3166_updates.get_updates("YE", year="<2010")
 #exported files: /iso3166-updates/iso3166-output-YE_<2010.json
 ```
 ## Terminal/Command Line
 
-**Get all listed changes/updates for all countries, export csv and json to folder "iso3166-updates", print progress using verbose parameter:** 
+The software functions can also be run from the cmd/terminal interface, when the script is called the get_updates() function will be called. The script accepts the same parameter names as the get_updates() function.
+
+**Get all listed ISO 3166-2 changes/updates for all countries, export csv and json to folder "iso3166-updates", print progress using verbose flag:** 
 ```bash
 python3 iso3166_updates.py --export_folder="iso3166-updates" --export_csv --export_json --verbose
 ```
 
-**Get all listed changes/updates for BY, DJ, ET, LY, PA for year range 2005-2010, export only CSV of updates to export folder "iso3166-updates", print progress using verbose parameter:**
+**Get all listed ISO 3166-2 changes/updates for BY, DJ, ET, LY, PA for year range 2005-2010, export only CSV of updates to export folder "iso3166-updates", print progress using verbose flag:**
 ```bash
 python3 iso3166_updates.py --alpha2="BY, DJ, ET, LY, PA" --year="2005-2010" --export_folder="iso3166-updates" --export_csv --no-export_json --verbose
 ```
 
-The output to the above functions for the updates/changes to a ISO 3166-2 country returns 4 columns: 
-<b>Edition/Newsletter, Date Issued, Code/Subdivision change</b> and <b>Description of change in newsletter.</b> For the CSV export, if more than one country input then an addition primary key column <b>Country Code</b> will be prepended to the first column, which will be the 2 letter ISO 3166-1 country code. 
+The output to the above functions for the updates/changes to an ISO 3166-2 country returns 4 columns: 
+<b>Edition/Newsletter, Date Issued, Code/Subdivision change</b> and <b>Description of change in newsletter.</b> For the CSV export, if more than one country input, then an additional primary key column <b>Country Code</b> will be prepended to the first column, which will be the 2 letter ISO 3166-1 country code. 
 
-* Edition/Newsletter: Name and or edition of newsletter that ISO 3166-2 change/update was communicated in.
+* Edition/Newsletter: Name and or edition of newsletter that the ISO 3166-2 change/update was communicated in.
 * Date Issued: Date that the change was communicated.
 * Code/Subdivision change: Overall summary of change/update made.
 * Description of change in newsletter: More in-depth info about the change/update that was made.
 
-E.g. The output format of the exported CSV for AD (Andorra) is:
+E.g. The output format of the exported <b>CSV</b> for AD (Andorra) is:
 
 | Edition/Newsletter | Date Issued | Code/Subdivision change | Description of change in newsletter |   
 |:-------------------|:------------|------------------------------------:|------------------------:|
 | Newsletter I-8     | 2007-04-17  | Subdivisions added: 7 parishes...   | Addition of the administrative subdivisions...                 | 
 | Online Browsing Platform (OBP) | 2014-11-03 | No subdivision changes listed | Update List Source |
 | Online Browsing Platform (OBP) | 2015-11-27 | No subdivision changes listed | Update List Source | 
 
-E.g. The output format of the exported JSON for AD (Andorra) is:
+E.g. The output format of the exported <b>JSON</b> for AD (Andorra) is:
 ```javascript
 {
   AD: [
       {
         "Code/Subdivision change": "",
         "Date Issued": "2015-11-27",
         "Description of change in newsletter": "Update List Source",
```

### Comparing `iso3166-updates-1.3.0/setup.cfg` & `iso3166-updates-1.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iso3166-updates
-version = 1.3.0
+version = 1.3.1
 description = A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = AJ McKenna
 author_email = amckenna41@qub.ac.uk
 url = https://github.com/amckenna41/iso3166-updates
 download_url = https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
```

### Comparing `iso3166-updates-1.3.0/setup.py` & `iso3166-updates-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pathlib
 from setuptools import setup, find_packages
 import sys
 
 #software metadata
 __name__ = 'iso3166-updates'
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 __description__ = "A Python package that pulls the latest updates & changes to all ISO3166 listed countries."
 __author__ = 'AJ McKenna, https://github.com/amckenna41'
 __authorEmail__ = 'amckenna41@qub.ac.uk'
 __license__ = 'MIT'
 __url__ = 'https://github.com/amckenna41/iso3166-updates'
 __download_url__ = "https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip"
 __status__ = 'Development'
@@ -46,15 +46,14 @@
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Information Technology',
         'License :: OSI Approved :: MIT License',
         'License :: Free For Educational Use',
         'Natural Language :: English',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',	
         'Programming Language :: Python :: Implementation :: PyPy',
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Scientific/Engineering',
```

