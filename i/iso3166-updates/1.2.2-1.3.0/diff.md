# Comparing `tmp/iso3166-updates-1.2.2.tar.gz` & `tmp/iso3166-updates-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iso3166-updates-1.2.2.tar", last modified: Mon May 22 19:21:57 2023, max compression
+gzip compressed data, was "iso3166-updates-1.3.0.tar", last modified: Fri Jun 23 23:41:25 2023, max compression
```

## Comparing `iso3166-updates-1.2.2.tar` & `iso3166-updates-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:21:57.542352 iso3166-updates-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-22 19:21:34.000000 iso3166-updates-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19683 2023-05-22 19:21:57.542352 iso3166-updates-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-05-22 19:21:34.000000 iso3166-updates-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:21:57.538352 iso3166-updates-1.2.2/iso3166_updates/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 19:21:34.000000 iso3166-updates-1.2.2/iso3166_updates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25218 2023-05-22 19:21:34.000000 iso3166-updates-1.2.2/iso3166_updates/iso3166_updates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:21:57.542352 iso3166-updates-1.2.2/iso3166_updates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19683 2023-05-22 19:21:57.000000 iso3166-updates-1.2.2/iso3166_updates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-22 19:21:57.000000 iso3166-updates-1.2.2/iso3166_updates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:21:57.000000 iso3166-updates-1.2.2/iso3166_updates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:21:48.000000 iso3166-updates-1.2.2/iso3166_updates.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-22 19:21:57.000000 iso3166-updates-1.2.2/iso3166_updates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 19:21:57.000000 iso3166-updates-1.2.2/iso3166_updates.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-22 19:21:57.542352 iso3166-updates-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-22 19:21:34.000000 iso3166-updates-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:41:25.484483 iso3166-updates-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-23 23:41:05.000000 iso3166-updates-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18983 2023-06-23 23:41:25.484483 iso3166-updates-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17369 2023-06-23 23:41:05.000000 iso3166-updates-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:41:25.480483 iso3166-updates-1.3.0/iso3166_updates/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-23 23:41:05.000000 iso3166-updates-1.3.0/iso3166_updates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35367 2023-06-23 23:41:05.000000 iso3166-updates-1.3.0/iso3166_updates/iso3166_updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:41:25.484483 iso3166-updates-1.3.0/iso3166_updates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18983 2023-06-23 23:41:25.000000 iso3166-updates-1.3.0/iso3166_updates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-23 23:41:25.000000 iso3166-updates-1.3.0/iso3166_updates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 23:41:25.000000 iso3166-updates-1.3.0/iso3166_updates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 23:41:18.000000 iso3166-updates-1.3.0/iso3166_updates.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-23 23:41:25.000000 iso3166-updates-1.3.0/iso3166_updates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 23:41:25.000000 iso3166-updates-1.3.0/iso3166_updates.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-23 23:41:25.484483 iso3166-updates-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-23 23:41:05.000000 iso3166-updates-1.3.0/setup.py
```

### Comparing `iso3166-updates-1.2.2/PKG-INFO` & `iso3166-updates-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,261 +1,18 @@
 Metadata-Version: 2.1
 Name: iso3166-updates
-Version: 1.2.2
+Version: 1.3.0
 Summary: A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 Home-page: https://github.com/amckenna41/iso3166-updates
 Author: AJ McKenna, https://github.com/amckenna41
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
-Description: # iso3166-updates
-        
-        [![iso3166_updates](https://img.shields.io/pypi/v/iso3166-updates)](https://pypi.org/project/iso3166-updates/)
-        [![pytest](https://github.com/amckenna41/iso3166-updates/workflows/Building%20and%20Testing/badge.svg)](https://github.com/amckenna41/iso3166-updates/actions?query=workflowBuilding%20and%20Testing)
-        [![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/iso3166-updates/)
-        [![License: MIT](https://img.shields.io/github/license/amckenna41/iso3166-updates)](https://opensource.org/licenses/MIT)
-        <!-- [![CircleCI](https://circleci.com/gh/amckenna41/iso3166-updates.svg?style=svg&circle-token=d860bb64668be19d44f106841b80eb47a8b7e7e8)](https://app.circleci.com/pipelines/github/amckenna41/iso3166-updates) -->
-        [![Issues](https://img.shields.io/github/issues/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates/issues)
-        [![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates)
-        <!-- [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-updates)](https://github.com/iso3166-updates) -->
-        
-        <div alt="images" style="justify-content: center; display:flex; margin-left=50px;">
-          <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="200" width="500"/>
-          <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="200" width="300"/>
-        </div>
-        
-        > Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here][demo].
-        
-        Table of Contents
-        -----------------
-          * [Introduction](#introduction)
-          * [API](#api)
-          * [Staying up to date](#staying-up-to-date)
-          * [Requirements](#requirements)
-          * [Installation](#installation)
-          * [Usage](#usage)
-          * [Directories](#Directories)
-          * [Issues](#Issues)
-          * [Contact](#contact)
-          * [References](#references)
-        
-        Introduction
-        ------------
-        `iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
-        
-        The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations [[1]](#references). The ISO 3166-2 was first published in 1998 and as of 29 November 2022 there are 5,043 codes defined in it [[2]](#references).
-        
-        ### Problem Statement:
-        
-        The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
-        
-        This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of country's ISO 3166-2 codes for free, with an easy-to-use interface and Python package and API, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
-        
-        <strong> The earliest date for any ISO 3166 updates is 2000-06-21, and the most recent is 2022-11-29. </strong>
-        
-        ### Intended Audience:
-        
-        This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (excluding 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API (https://iso3166-updates.com). 
-        
-        API
-        ---
-        An API is available that can be used to extract any applicable updates for a country via a URL. The API is available at the URL:
-        
-        > https://www.iso3166-updates.com/api
-        
-        Three query string parameters/paths are available in the API - `alpha2`, `year` and `months`. The 2 letter alpha-2 country code can be appeneded to the url as a query string parameter - "?alpha2=JP". A single alpha-2 or list of them can be passed to the API (e.g "FR", "DE", "HU, ID, MA"). The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "?year=2017", "2010-2015", "<2009", ">2002"). Finally, the months parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g "?month=6", "?month=48").
-        
-        The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON with all ISO 3166 updates. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure the hosting was switched to Vercel (https://vercel.com/).
-        
-        The API documentation and usage with all useful commands and examples to the API is available on the [README](https://github.com/amckenna41/iso3166-updates/blob/main/iso3166-updates-api/README.md) of the iso3166-updates-api folder. 
-        
-        <p align="center">
-          <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_arch.png" alt="gcp_arch" height="200" width="400"/>
-        </p>
-        
-        Staying up to date
-        ------------------
-        The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. 
-        The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO 3166-2 wiki's to check for the latest updates within a certain period e.g the past 3-6 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data.
-        
-        Additionally, a GitHub Issue in the `iso3166-2` and `iso3166-flag-icons` repositories will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-2` and `iso3166-flag-icons` JSONs and repos.
-        
-        Ultimately, this Cloud Function ensures that the software and assoicated APIs are up-to-date with the latest ISO 3166-2 information for all countries/territories/subdivisions etc.
-        
-        Requirements
-        ------------
-        * [python][python] >= 3.7
-        * [pandas][pandas] >= 1.4.3
-        * [numpy][numpy] >= 1.23.2
-        * [requests][requests] >= 2.28.1
-        * [beautifulsoup4][beautifulsoup4] >= 4.11.1
-        * [iso3166][iso3166] >= 2.1.1
-        
-        Installation
-        ------------
-        Install the latest version of `iso3166-updates` via [PyPi][PyPi] using pip:
-        
-        ```bash
-        pip3 install iso3166-updates --upgrade
-        ```
-        
-        Installation from source:
-        ```bash
-        git clone -b master https://github.com/amckenna41/iso3166-updates.git
-        cd iso3166_updates
-        python3 setup.py install
-        ```
-        
-        Usage
-        -----
-        **Import package:**
-        ```python
-        import iso3166_updates as iso3166_updates
-        ```
-        
-        **Input parameters to get_updates function:**
-        ```python
-          # -alpha2 ALPHA2, --alpha2 ALPHA2
-          #                       Alpha-2 code/s of ISO3166 countries to check for updates.
-          # -export_filename EXPORT_FILENAME, --export_filename EXPORT_FILENAME
-          #                       Filename for exported ISO3166 updates csv file.
-          # -export_json_filename EXPORT_JSON_FILENAME, --export_json_filename EXPORT_JSON_FILENAME
-          #                       Filename for exported ISO3166 updates json file.
-          # -export_folder EXPORT_FOLDER, --export_folder EXPORT_FOLDER
-          #                       Folder where to store exported ISO files.
-          # -export_json, --export_json
-          #                       Whether to export all found updates to json.
-          # -export_csv, --export_csv
-          #                       Whether to export all found updates to csv files in export folder.
-          # -year YEAR, --year YEAR
-          #                       Selected year to check for updates.
-          # -concat_updates, --concat_updates
-          #                       Whether to concatenate updates of individual countrys into the same json file or seperate.
-        ```
-        
-        **Get all listed changes/updates for all countries which happens by default if no alpha-2 codes specified in input param, export csv and json to folder "iso3166-updates":**
-        ```python
-        iso3166_updates.get_updates(export_folder="iso3166-updates", export_json=1, export_csv=1)
-        ```
-        
-        **Get all listed changes/updates for Andorra from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:AD), export csv and json to folder "iso3166-updates":**
-        ```python
-        iso3166_updates.get_updates("AD", export_folder="iso3166-updates", export_json=1, export_csv=1)
-        ```
-        
-        **Get all listed changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates":**
-        ```python
-        iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=0))
-        ```
-        
-        **Get any listed changes/updates for HU, IT, JA, KE from wiki, in the year 2018, export only to JSON with filename "iso3166-updates.json" and seperate updates into sepetate JSON files:**
-        ```python
-        iso3166_updates.get_updates("HU, IT, JA, KE", year="2018", export_json=1, export_csv=0, export_json_filename="iso3166-updates", concat_updates=0)
-        ```
-        
-        **Get any listed changes/updates for Ireland from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:IE), between years of 2012 and 2021, use default parameters:**
-        ```python
-        iso3166_updates.get_updates("IE", year="2012-2021")
-        ```
-        
-        **Get any listed changes/updates for Tanzania from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:TZ), with updates years >=2015, export only to CSV with filename "iso3166-output.csv":**
-        ```python
-        iso3166_updates.get_updates("TA", year=">2015", export_filename="iso3166-output.csv")
-        ```
-        
-        **Get any listed changes/updates for Yemen from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:YE), with updates years < 2010, use default parameters:**
-        ```python
-        iso3166_updates.get_updates("YE", year="<2010")
-        ```
-        
-        The output to the above functions for the updates/changes to a ISO 3166-2 country returns 4 columns: 
-        <b>Edition/Newsletter, Date Issued, Code/Subdivision change</b> and <b>Description of change in newsletter.</b> 
-        
-        * Edition/Newsletter: Name and or edition of newsletter that ISO 3166-2 change/update was communicated in.
-        * Date Issued: Date that the change was communicated.
-        * Code/Subdivision change: Overall summary of change/update made.
-        * Description of change in newsletter: More in-depth info about the change/update that was made.
-        
-        E.g. The output format of the exported CSV for AD (Andorra) is:
-        
-        | Edition/Newsletter | Date Issued | Code/Subdivision change | Description of change in newsletter |   
-        |:-------------------|:------------|------------------------------------:|------------------------:|
-        | Newsletter I-8     | 2007-04-17  | Subdivisions added: 7 parishes...   | Addition of the administrative subdivisions...                 | 
-        | Online Browsing Platform (OBP) | 2014-11-03 | No subdivision changes listed | Update List Source |
-        | Online Browsing Platform (OBP) | 2015-11-27 | No subdivision changes listed | Update List Source | 
-        
-        E.g. The output format of the exported JSON for AD (Andorra) is:
-        ```javascript
-        {
-          AD: [
-              {
-                "Code/Subdivision change": "",
-                "Date Issued": "2015-11-27",
-                "Description of change in newsletter": "Update List Source",
-                "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)"
-              },
-              {
-                "Code/Subdivision change": "",
-                "Date Issued": "2014-11-03",
-                "Description of change in newsletter": "Update List Source",
-                "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)"
-              },
-              {
-                "Code/Subdivision change:" "Subdivisions added:7 parishes",
-                "Date Issued": "2007-04-17",
-                "Description of change in newsletter": "Addition of the administrative subdivisions and of their code elements",
-                "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)"
-              }
-          ]
-        }
-        ```
-        
-        Directories
-        -----------
-        * `/docs` - documentation for `iso3166-updates` Python package.
-        * `/iso3166_updates` - source code for `iso3166-updates` Python package.
-        * `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the `iso3166-updates` API, including the main.py, requirements.txt and API config file.
-        * `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Function for the check-for-updates function which is a periodically called Cloud Function that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date. Includes the main.py and requirements.txt files.
-        * `/tests` - unit and integration tests for `iso3166-updates`.
-        
-        Issues
-        ------
-        Any issues, errors or bugs can be raised via the [Issues](Issues) tab in the repository. Also if there are any missing or incorrect data in the updates json, this should also be raised by creating an issue. 
-        
-        Contact
-        -------
-        If you have any questions or comments, please contact amckenna41@qub.ac.uk or raise an issue on the [Issues][Issues] tab. <br><br>
-        [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/)
-        
-        References
-        ----------
-        \[1\]: ISO3166-1: https://en.wikipedia.org/wiki/ISO_3166-1 <br>
-        \[2\]: ISO3166-2: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
-        \[3\]: ISO Country Codes Collection: https://www.iso.org/publication/PUB500001 <br>
-        \[4\]: ISO Country Codes: https://www.iso.org/iso-3166-country-codes.html <br>
-        \[5\]: ISO3166-1 flag-icons repo: https://github.com/lipis/flag-icons <br>
-        \[6\]: ISO3166-2 flag-icons repo: https://github.com/amckenna41/iso3166-flag-icons <br>
-        
-        Support
-        -------
-        <a href="https://www.buymeacoffee.com/amckenna41" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
-        
-        [Back to top](#TOP)
-        
-        [demo]: https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing
-        [python]: https://www.python.org/downloads/release/python-360/
-        [pandas]: https://pandas.pydata.org/
-        [numpy]: https://numpy.org/
-        [requests]: https://requests.readthedocs.io/
-        [beautifulsoup4]: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
-        [iso3166]: https://github.com/deactivated/python-iso3166
-        [PyPi]: https://pypi.org/project/iso3166-updates/
-        [Issues]: https://github.com/amckenna41/iso3166-updates/issues
-Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,csviso3166-2,iso3166-1,alpha2,alpha3
+Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,csv,iso3166-2,iso3166-1,alpha-2,alpha-3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
@@ -271,7 +28,269 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
+License-File: LICENSE
+
+# iso3166-updates
+
+[![iso3166_updates](https://img.shields.io/pypi/v/iso3166-updates)](https://pypi.org/project/iso3166-updates/)
+[![pytest](https://github.com/amckenna41/iso3166-updates/workflows/Building%20and%20Testing/badge.svg)](https://github.com/amckenna41/iso3166-updates/actions?query=workflowBuilding%20and%20Testing)
+[![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/iso3166-updates/)
+[![License: MIT](https://img.shields.io/github/license/amckenna41/iso3166-updates)](https://opensource.org/licenses/MIT)
+<!-- [![CircleCI](https://circleci.com/gh/amckenna41/iso3166-updates.svg?style=svg&circle-token=d860bb64668be19d44f106841b80eb47a8b7e7e8)](https://app.circleci.com/pipelines/github/amckenna41/iso3166-updates) -->
+[![Issues](https://img.shields.io/github/issues/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates/issues)
+[![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates)
+<!-- [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-updates)](https://github.com/iso3166-updates) -->
+
+<div alt="images" style="justify-content: center; display:flex; margin-left=50px;">
+  <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="200" width="500"/>
+  <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="200" width="300"/>
+</div>
+
+> Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here][demo].
+
+Table of Contents
+-----------------
+  * [Introduction](#introduction)
+  * [API](#api)
+  * [Staying up to date](#staying-up-to-date)
+  * [Requirements](#requirements)
+  * [Installation](#installation)
+  * [Usage](#usage)
+  * [Directories](#Directories)
+  * [Issues](#Issues)
+  * [Contact](#contact)
+  * [References](#references)
+
+Introduction
+------------
+`iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
+
+The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations [[1]](#references). The ISO 3166-2 was first published in 1998 and as of 29 November 2022 there are 5,043 codes defined in it [[2]](#references).
+
+### Problem Statement:
+
+The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
+
+This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of country's ISO 3166-2 codes for free, with an easy-to-use interface and Python package and API, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
+
+<strong> The earliest date for any ISO 3166 updates is 2000-06-21, and the most recent is 2022-11-29. </strong>
+
+### Intended Audience:
+
+This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (excluding 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API (https://iso3166-updates.com). 
+
+API
+---
+An API is available that can be used to extract any applicable updates for a country via a URL. The API is available at the URL:
+
+> https://www.iso3166-updates.com/api
+
+Three query string parameters/paths are available in the API - `alpha2`, `year` and `months`. The 2 letter alpha-2 country code can be appeneded to the url as a query string parameter - "?alpha2=JP". A single alpha-2 or list of them can be passed to the API (e.g "FR", "DE", "HU, ID, MA"). The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "?year=2017", "2010-2015", "<2009", ">2002"). Finally, the months parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g "?month=6", "?month=48").
+
+The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON with all ISO 3166 updates. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure the hosting was switched to Vercel (https://vercel.com/).
+
+The API documentation and usage with all useful commands and examples to the API is available on the [README](https://github.com/amckenna41/iso3166-updates/blob/main/iso3166-updates-api/README.md) of the iso3166-updates-api folder. 
+
+<p align="center">
+  <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_arch.png" alt="gcp_arch" height="200" width="400"/>
+</p>
+
+Staying up to date
+------------------
+The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. 
+The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO 3166-2 wiki's to check for the latest updates within a certain period e.g the past 3-6 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data.
+
+Additionally, a GitHub Issue in the `iso3166-2` and `iso3166-flag-icons` repositories will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-2` and `iso3166-flag-icons` JSONs and repos.
+
+Ultimately, this Cloud Function ensures that the software and assoicated APIs are up-to-date with the latest ISO 3166-2 information for all countries/territories/subdivisions etc.
+
+Requirements
+------------
+* [python][python] >= 3.7
+* [pandas][pandas] >= 1.4.3
+* [numpy][numpy] >= 1.23.2
+* [requests][requests] >= 2.28.1
+* [beautifulsoup4][beautifulsoup4] >= 4.11.1
+* [iso3166][iso3166] >= 2.1.1
+
+Installation
+------------
+Install the latest version of `iso3166-updates` via [PyPi][PyPi] using pip:
+
+```bash
+pip3 install iso3166-updates --upgrade
+```
+
+Installation from source:
+```bash
+git clone -b master https://github.com/amckenna41/iso3166-updates.git
+cd iso3166_updates
+python3 setup.py install
+```
+
+Usage
+-----
+**Import package:**
+```python
+import iso3166_updates as iso3166_updates
+```
+
+**Input parameters to get_updates function:**
+```python
+  # -alpha2 ALPHA2, --alpha2 ALPHA2
+  #                       Alpha-2 code/s of ISO3166 countries to check for updates.
+  # -export_filename EXPORT_FILENAME, --export_filename EXPORT_FILENAME
+  #                       Filename for exported ISO3166 updates for CSV and JSON files.
+  # -export_folder EXPORT_FOLDER, --export_folder EXPORT_FOLDER
+  #                       Folder where to store exported ISO files.
+  # -export_json, --export_json
+  #                       Whether to export all found updates to json.
+  # -export_csv, --export_csv
+  #                       Whether to export all found updates to csv files in export folder.
+  # -year YEAR, --year YEAR
+  #                       Selected year to check for updates.
+  # -concat_updates, --concat_updates
+  #                       Whether to concatenate updates of individual countrys into the same json file or seperate.
+```
+
+**Get all listed changes/updates for all countries which happens by default if no alpha-2 codes specified in input param, export csv and json to folder "iso3166-updates":**
+```python
+iso3166_updates.get_updates(export_folder="iso3166-updates", export_json=1, export_csv=1)
+#exported files: /iso3166-updates/iso3166-updates.json and /iso3166-updates/iso3166-updates.csv
+```
+
+**Get all listed changes/updates for Andorra from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:AD), export csv and json to folder "iso3166-updates":**
+```python
+iso3166_updates.get_updates("AD", export_folder="iso3166-updates", export_json=1, export_csv=1)
+#exported files: /iso3166-updates/iso3166-updates-AD.json and /iso3166-updates/iso3166-updates-AD.csv
+```
+
+**Get all listed changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates":**
+```python
+iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=0)
+#exported files: /iso3166-updates/iso3166-updates-BA,DE,FR,HU,PY.json
+```
+
+**Get any listed changes/updates for HU, IT, JA, KE from wiki, in the year 2018, export only to JSON with filename "iso3166-updates.json" and seperate updates into sepetate JSON files:**
+```python
+iso3166_updates.get_updates("HU, IT, JA, KE", year="2018", export_json=1, export_csv=0, export_filename="iso3166-updates", concat_updates=0)
+#exported files: /iso3166-updates/iso3166-updates-HU,IT,JA,KE-2018.json
+```
+
+**Get any listed changes/updates for Ireland from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:IE), between years of 2012 and 2021, use default parameters:**
+```python
+iso3166_updates.get_updates("IE", year="2012-2021")
+#exported files: /iso3166-updates/iso3166-updates-IE_2012-2021.json
+```
+
+**Get any listed changes/updates for Tanzania from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:TZ), with updates years >=2015, export only to CSV with filename iso3166-output":**
+```python
+iso3166_updates.get_updates("TA", year=">2015", export_filename="iso3166-output", export_json=0, export_csv=1)
+#exported files: /iso3166-updates/iso3166-output-TA_>2015.csv
+```
+
+**Get any listed changes/updates for Yemen from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:YE), with updates years < 2010, use default parameters:**
+```python
+iso3166_updates.get_updates("YE", year="<2010")
+#exported files: /iso3166-updates/iso3166-output-YE_<2010.json
+```
+## Terminal/Command Line
+
+**Get all listed changes/updates for all countries, export csv and json to folder "iso3166-updates", print progress using verbose parameter:** 
+```bash
+python3 iso3166_updates.py --export_folder="iso3166-updates" --export_csv --export_json --verbose
+```
+
+**Get all listed changes/updates for BY, DJ, ET, LY, PA for year range 2005-2010, export only CSV of updates to export folder "iso3166-updates", print progress using verbose parameter:**
+```bash
+python3 iso3166_updates.py --alpha2="BY, DJ, ET, LY, PA" --year="2005-2010" --export_folder="iso3166-updates" --export_csv --no-export_json --verbose
+```
+
+The output to the above functions for the updates/changes to a ISO 3166-2 country returns 4 columns: 
+<b>Edition/Newsletter, Date Issued, Code/Subdivision change</b> and <b>Description of change in newsletter.</b> For the CSV export, if more than one country input then an addition primary key column <b>Country Code</b> will be prepended to the first column, which will be the 2 letter ISO 3166-1 country code. 
+
+* Edition/Newsletter: Name and or edition of newsletter that ISO 3166-2 change/update was communicated in.
+* Date Issued: Date that the change was communicated.
+* Code/Subdivision change: Overall summary of change/update made.
+* Description of change in newsletter: More in-depth info about the change/update that was made.
+
+E.g. The output format of the exported CSV for AD (Andorra) is:
+
+| Edition/Newsletter | Date Issued | Code/Subdivision change | Description of change in newsletter |   
+|:-------------------|:------------|------------------------------------:|------------------------:|
+| Newsletter I-8     | 2007-04-17  | Subdivisions added: 7 parishes...   | Addition of the administrative subdivisions...                 | 
+| Online Browsing Platform (OBP) | 2014-11-03 | No subdivision changes listed | Update List Source |
+| Online Browsing Platform (OBP) | 2015-11-27 | No subdivision changes listed | Update List Source | 
+
+E.g. The output format of the exported JSON for AD (Andorra) is:
+```javascript
+{
+  AD: [
+      {
+        "Code/Subdivision change": "",
+        "Date Issued": "2015-11-27",
+        "Description of change in newsletter": "Update List Source",
+        "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)"
+      },
+      {
+        "Code/Subdivision change": "",
+        "Date Issued": "2014-11-03",
+        "Description of change in newsletter": "Update List Source",
+        "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)"
+      },
+      {
+        "Code/Subdivision change:" "Subdivisions added:7 parishes",
+        "Date Issued": "2007-04-17",
+        "Description of change in newsletter": "Addition of the administrative subdivisions and of their code elements",
+        "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)"
+      }
+  ]
+}
+```
+
+Directories
+-----------
+* `/docs` - documentation for `iso3166-updates` Python package.
+* `/iso3166_updates` - source code for `iso3166-updates` Python package.
+* `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the `iso3166-updates` API, including the main.py, requirements.txt and API config file.
+* `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Function for the check-for-updates function which is a periodically called Cloud Function that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date. Includes the main.py and requirements.txt files.
+* `/tests` - unit and integration tests for `iso3166-updates`.
+
+Issues
+------
+Any issues, errors or bugs can be raised via the [Issues](Issues) tab in the repository. Also if there are any missing or incorrect data in the updates json, this should also be raised by creating an issue. 
+
+Contact
+-------
+If you have any questions or comments, please contact amckenna41@qub.ac.uk or raise an issue on the [Issues][Issues] tab. <br><br>
+[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/)
+
+References
+----------
+\[1\]: ISO3166-1: https://en.wikipedia.org/wiki/ISO_3166-1 <br>
+\[2\]: ISO3166-2: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
+\[3\]: ISO Country Codes Collection: https://www.iso.org/publication/PUB500001 <br>
+\[4\]: ISO Country Codes: https://www.iso.org/iso-3166-country-codes.html <br>
+\[5\]: ISO3166-1 flag-icons repo: https://github.com/lipis/flag-icons <br>
+\[6\]: ISO3166-2 flag-icons repo: https://github.com/amckenna41/iso3166-flag-icons <br>
+
+Support
+-------
+<a href="https://www.buymeacoffee.com/amckenna41" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
+
+[Back to top](#TOP)
+
+[demo]: https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing
+[python]: https://www.python.org/downloads/release/python-360/
+[pandas]: https://pandas.pydata.org/
+[numpy]: https://numpy.org/
+[requests]: https://requests.readthedocs.io/
+[beautifulsoup4]: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
+[iso3166]: https://github.com/deactivated/python-iso3166
+[PyPi]: https://pypi.org/project/iso3166-updates/
+[Issues]: https://github.com/amckenna41/iso3166-updates/issues
+
```

### Comparing `iso3166-updates-1.2.2/README.md` & `iso3166-updates-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -104,17 +104,15 @@
 ```
 
 **Input parameters to get_updates function:**
 ```python
   # -alpha2 ALPHA2, --alpha2 ALPHA2
   #                       Alpha-2 code/s of ISO3166 countries to check for updates.
   # -export_filename EXPORT_FILENAME, --export_filename EXPORT_FILENAME
-  #                       Filename for exported ISO3166 updates csv file.
-  # -export_json_filename EXPORT_JSON_FILENAME, --export_json_filename EXPORT_JSON_FILENAME
-  #                       Filename for exported ISO3166 updates json file.
+  #                       Filename for exported ISO3166 updates for CSV and JSON files.
   # -export_folder EXPORT_FOLDER, --export_folder EXPORT_FOLDER
   #                       Folder where to store exported ISO files.
   # -export_json, --export_json
   #                       Whether to export all found updates to json.
   # -export_csv, --export_csv
   #                       Whether to export all found updates to csv files in export folder.
   # -year YEAR, --year YEAR
@@ -122,48 +120,66 @@
   # -concat_updates, --concat_updates
   #                       Whether to concatenate updates of individual countrys into the same json file or seperate.
 ```
 
 **Get all listed changes/updates for all countries which happens by default if no alpha-2 codes specified in input param, export csv and json to folder "iso3166-updates":**
 ```python
 iso3166_updates.get_updates(export_folder="iso3166-updates", export_json=1, export_csv=1)
+#exported files: /iso3166-updates/iso3166-updates.json and /iso3166-updates/iso3166-updates.csv
 ```
 
 **Get all listed changes/updates for Andorra from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:AD), export csv and json to folder "iso3166-updates":**
 ```python
 iso3166_updates.get_updates("AD", export_folder="iso3166-updates", export_json=1, export_csv=1)
+#exported files: /iso3166-updates/iso3166-updates-AD.json and /iso3166-updates/iso3166-updates-AD.csv
 ```
 
 **Get all listed changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates":**
 ```python
-iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=0))
+iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=0)
+#exported files: /iso3166-updates/iso3166-updates-BA,DE,FR,HU,PY.json
 ```
 
 **Get any listed changes/updates for HU, IT, JA, KE from wiki, in the year 2018, export only to JSON with filename "iso3166-updates.json" and seperate updates into sepetate JSON files:**
 ```python
-iso3166_updates.get_updates("HU, IT, JA, KE", year="2018", export_json=1, export_csv=0, export_json_filename="iso3166-updates", concat_updates=0)
+iso3166_updates.get_updates("HU, IT, JA, KE", year="2018", export_json=1, export_csv=0, export_filename="iso3166-updates", concat_updates=0)
+#exported files: /iso3166-updates/iso3166-updates-HU,IT,JA,KE-2018.json
 ```
 
 **Get any listed changes/updates for Ireland from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:IE), between years of 2012 and 2021, use default parameters:**
 ```python
 iso3166_updates.get_updates("IE", year="2012-2021")
+#exported files: /iso3166-updates/iso3166-updates-IE_2012-2021.json
 ```
 
-**Get any listed changes/updates for Tanzania from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:TZ), with updates years >=2015, export only to CSV with filename "iso3166-output.csv":**
+**Get any listed changes/updates for Tanzania from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:TZ), with updates years >=2015, export only to CSV with filename iso3166-output":**
 ```python
-iso3166_updates.get_updates("TA", year=">2015", export_filename="iso3166-output.csv")
+iso3166_updates.get_updates("TA", year=">2015", export_filename="iso3166-output", export_json=0, export_csv=1)
+#exported files: /iso3166-updates/iso3166-output-TA_>2015.csv
 ```
 
 **Get any listed changes/updates for Yemen from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:YE), with updates years < 2010, use default parameters:**
 ```python
 iso3166_updates.get_updates("YE", year="<2010")
+#exported files: /iso3166-updates/iso3166-output-YE_<2010.json
+```
+## Terminal/Command Line
+
+**Get all listed changes/updates for all countries, export csv and json to folder "iso3166-updates", print progress using verbose parameter:** 
+```bash
+python3 iso3166_updates.py --export_folder="iso3166-updates" --export_csv --export_json --verbose
+```
+
+**Get all listed changes/updates for BY, DJ, ET, LY, PA for year range 2005-2010, export only CSV of updates to export folder "iso3166-updates", print progress using verbose parameter:**
+```bash
+python3 iso3166_updates.py --alpha2="BY, DJ, ET, LY, PA" --year="2005-2010" --export_folder="iso3166-updates" --export_csv --no-export_json --verbose
 ```
 
 The output to the above functions for the updates/changes to a ISO 3166-2 country returns 4 columns: 
-<b>Edition/Newsletter, Date Issued, Code/Subdivision change</b> and <b>Description of change in newsletter.</b> 
+<b>Edition/Newsletter, Date Issued, Code/Subdivision change</b> and <b>Description of change in newsletter.</b> For the CSV export, if more than one country input then an addition primary key column <b>Country Code</b> will be prepended to the first column, which will be the 2 letter ISO 3166-1 country code. 
 
 * Edition/Newsletter: Name and or edition of newsletter that ISO 3166-2 change/update was communicated in.
 * Date Issued: Date that the change was communicated.
 * Code/Subdivision change: Overall summary of change/update made.
 * Description of change in newsletter: More in-depth info about the change/update that was made.
 
 E.g. The output format of the exported CSV for AD (Andorra) is:
```

### Comparing `iso3166-updates-1.2.2/iso3166_updates/iso3166_updates.py` & `iso3166-updates-1.3.0/iso3166_updates/iso3166_updates.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,155 +2,167 @@
 import argparse
 import pandas as pd
 import requests
 import iso3166
 import os
 import getpass
 import json
-import logging
 import re
-from bs4 import BeautifulSoup
+from bs4 import BeautifulSoup, Tag
 from importlib import metadata
 import datetime
 
-#initialise logging library 
+#get current software version
 __version__ = metadata.metadata('iso3166_updates')['version']
-log = logging.getLogger(__name__)
 
 #initalise User-agent header for requests library 
 USER_AGENT_HEADER = {'User-Agent': 'iso3166-updates/{} ({}; {})'.format(__version__,
                                        'https://github.com/amckenna41/iso3166-updates', getpass.getuser())}
 
 #base URL for ISO3166-2 wiki
 wiki_base_url = "https://en.wikipedia.org/wiki/ISO_3166-2:"
 
-
-def get_updates(alpha2_codes=[], year=[], export_filename="iso3166-updates",
-        export_json_filename="iso3166-updates", export_folder="test_iso3166-updates", 
-        concat_updates=True, export_json=True, export_csv=False):
+def get_updates(alpha2_codes=[], year=[], export_filename="iso3166-updates", export_folder="test_iso3166-updates", 
+        concat_updates=True, export_json=True, export_csv=False, verbose=True):
     """
-    Get all listed updates to a country/country's ISO3166-2 subdivision codes/names 
+    Get all listed changes/updates to a country/country's ISO 3166-2 subdivision codes/names 
     via the "Changes" section on its wiki page. All wiki pages follow the convention
     https://en.wikipedia.org/wiki/ISO_3166-2:XX where XX is the 2 letter alpha-2 code
-    for a country. The "Changes" section lists updates or changes to any ISO3166-2 codes 
-    according to the ISO newsletter which is realeased peridically by the ISO as well as 
-    its Online Browsing Platform (OBP). The ISO newsletters are not easily discoverable 
-    and accessinle online and may require a subscription to the ISO3166-2 database 
-    (https://www.iso.org/iso/updating_information.pdf).
-
-    The changes/updates table is converted to a DataFrame and then exported to a 
-    CSV for further analysis. You can also get the updates from a particular year, 
-    list of years, year range or updates greater than or less than specified year, 
-    using the Year parameter. All of the updates are ordered alphabetically by there
-    2 letter country code and exported to a JSON and or CSV file.
+    for a country listed in the ISO 3166-1. The "Changes" section lists updates or changes 
+    to any ISO 3166-2 codes, including historical changes, according to the ISO newsletter 
+    which is released peridically by the ISO as well as its Online Browsing Platform (OBP). 
+    The ISO newsletters are not easily discoverable and accessinle online and may require a 
+    subscription to the ISO 3166-2 database (https://www.iso.org/iso/updating_information.pdf). 
+    The earliest available changes are from the year 2000 and the latest changes are from 2023.
+
+    The changes/updates table is converted to a DataFrame and then exported to a CSV and or 
+    JSON for further analysis. You can also get the updates from a particular year, list of 
+    years, year range or updates greater than or less than a specified year, using the year 
+    parameter. All of the updates are ordered alphabetically by their 2 letter ISO 3166-1 
+    country code and exported to a JSON and or CSV file.
 
     Parameters
     ----------
     :alpha2_codes : str / list (default=[])
-        single string or list of alpha-2 ISO3166 codes to get the latest ISO3166-2 updates from. If
-        single alpha-2 code passed in then it is converted to an iterable list. If no value passed
-        into param then all updates for all ISO3166 gotten. 
+        single string or list of alpha-2 ISO 3166-1 codes to get the latest ISO 3166-2 updates 
+        from. If a single alpha-2 code passed in then it is converted to an iterable list. If 
+        no value passed into param then all updates for all ISO 3166-1 countries are retrieved. 
     :year : list (default = [])
-        list of 1 or more years to get the specific ISO3166-2 updates from, per country. By default, 
-        the year param will be empty meaning all changes/updates for all years will be gotten.
-    :export_filename : str (default = "iso3166-updates")
-        filename for csv output of inputted country's ISO3166-2 updates. 
-    :export_json_filename : str (default = "iso3166-updates")
-        filename for json output of all country's ISO3166-2 updates. 
-    :export_folder : str (default = "../iso3166-updates")
-        folder name to store all csv outputs for all country's ISO3166-2 updates. 
-    :concat_updates : bool (default = True)
-        if multiple alpha-2 codes input, concatenate updates into one JSOn file or into seperately
-        named files in export folder. Not available for csv output.
-    :export_json : bool (default = True)
-        export all ISO3166 updates for inputted country's into json format. 
-    :export_csv : bool (default = False)
-        export all ISO3166 updates for inputted country's to csv files in export folder.
+        list of 1 or more years to get the specific ISO 3166-2 updates from, per country. By 
+        default, the year param will be empty meaning all changes/updates for all years will be 
+        retrieved. You can also pass in a year range (e.g 2010-2015) or a year to get all updates 
+        less than or greater than that specified year (e.g >2007, <2021).
+    :export_filename : str (default="iso3166-updates")
+        filename for JSON and CSV output files of inputted country's ISO 3166-2 updates. 
+    :export_folder : str (default="../iso3166-updates")
+        folder name to store all csv and json outputs for all country's ISO 3166-2 updates. 
+    :concat_updates : bool (default=True)
+        if multiple alpha-2 codes input, concatenate updates into one JSON and or CSV file 
+        (concat_updates=True) or into seperately named files in export folder 
+        (concat_updates=False). By default all country's updates will be compiled into the 
+        same file.
+    :export_json : bool (default=True)
+        export all ISO 3166 updates for inputted countries into json format in export folder. 
+    :export_csv : bool (default=False)
+        export all ISO 3166 updates for inputted countries into csv format in export folder. 
+    :verbose: int (default=1)
+        Set to 1 to print out progress of updates functionality, 0 will not print progress.
 
     Returns
     -------
     :all_changes : dict
-        dictionary of all found ISO3166 updates from users inputted alpha2 codes and or year
+        dictionary of all found ISO 3166 updates from user's inputted alpha2 codes and or year
         parameter values.
     """
     year_range = False
     greater_than = False
     less_than = False
-    
+    all_updates = False #set to True if gathering all ISO 3166 updates
+
     #if alpha-2 codes input param isn't str or list raise type error
     if not isinstance(alpha2_codes, str) and not isinstance(alpha2_codes, list):
         raise TypeError('alpha2_codes input param should be a 2 letter '
-            'ISO3166 alpha-2 code or a list of the same, got input of type {}.'.format(type(alpha2_codes)))
+            'ISO 3166-1 alpha-2 code or a list of the same, got input of type {}.'.format(type(alpha2_codes)))
 
-    #if single str input for alpha-2 codes param then convert to array, remove whitespace
+    #if single str of 1 or more alpha-2 codes input then convert to array, remove whitespace, seperate using comma
     if (isinstance(alpha2_codes, str)):
         alpha2_codes = alpha2_codes.replace(' ', '').split(',')
 
+    #convert year str to array
+    if not (isinstance(year, list)):
+        year = [year]
+    
+    #raise error if invalid data types input for year parameter
+    for year_ in year:
+        if not isinstance(year_, str):
+            raise TypeError("Invalid data type for year parameter, expected str, got {}.".format(type(year_)))
+
     #if list with 1 string of multiple alpha-2 codes, convert to multiple list elements e.g ['HI, LA'] will be converted to ['HI', 'LA']
     if (isinstance(alpha2_codes, list) and len(alpha2_codes) == 1 and ',' in alpha2_codes[0]):
         alpha2_codes = alpha2_codes[0].replace(' ', '').split(',')
 
-    #if single str input for Year param then convert to array, remove whitespace
+    #if single str of 1 or more years input then convert to array, remove whitespace, seperate using comma
     if (isinstance(year, str)):
         year = year.replace(' ', '').split(',')
-
+    
     def convert_to_alpha2(alpha3_code):
         """ 
-        Convert an ISO3166 country's 3 letter alpha-3 code into its 2 letter
+        Convert an ISO 3166 country's 3 letter alpha-3 code into its 2 letter
         alpha-2 counterpart. 
 
         Parameters 
         ----------
         :alpha3_code: str
-            3 letter ISO3166 country code.
+            3 letter ISO 3166-1 country code.
         
         Returns
         -------
         :iso3166.countries_by_alpha3[alpha3_code].alpha2: str
-            2 letter ISO3166 country code. 
+            2 letter ISO 3166 country code. 
         """
-        #return error if 3 letter alpha-3 code not found
+        #return None if 3 letter alpha-3 code not found
         if not (alpha3_code in list(iso3166.countries_by_alpha3.keys())):
             return None
         else:
             #use iso3166 package to find corresponding alpha-2 code from its alpha-3
             return iso3166.countries_by_alpha3[alpha3_code].alpha2
     
     #if 3 letter alpha-3 codes input then convert to corresponding alpha-2, else raise error
-    if (alpha2_codes != []):
+    if (alpha2_codes != ['']):
         for code in range(0, len(alpha2_codes)):
             if (len(alpha2_codes[code]) == 3): 
                 temp_alpha2_code = convert_to_alpha2(alpha2_codes[code])
                 if not (temp_alpha2_code is None):
                     alpha2_codes[code] = temp_alpha2_code
                 else:
                     raise ValueError("Invalid alpha-3 code input, cannot convert into corresponding alpha-2 code: {}.".format(alpha2_codes[code]))
+    
+    input_alpha2_codes = alpha2_codes
 
-    #use all ISO3166 codes if invalid alpha-2 code input, otherwise convert alpha-2 to array
-    if (alpha2_codes == []):
+    #use all ISO 3166-1 codes if no input alpha-2 parameter input, set all_updates to True
+    if ((alpha2_codes == [''] or alpha2_codes == [])):
         alpha2_codes = sorted(list(iso3166.countries_by_alpha2.keys()))
+        all_updates = True
 
-    #sort codes in alphabetical order
+    #sort codes in alphabetical order, uppercase each
     alpha2_codes.sort()
     alpha2_codes = [code.upper() for code in alpha2_codes]
 
-    #'-' seperating 2 years implies a year range of sought country updates, validate format of years in range
-    #'>' before year means get all country updates greater than or equal to specified year
-    #'<' before year means get all country updates less than to specified year
+    #a '-' seperating 2 years implies a year range of sought country updates, validate format of years in range
+    #a ',' seperating 2 year implies a list of years
+    #a '>' before year means get all country updates greater than or equal to specified year
+    #a '<' before year means get all country updates less than specified year
     if (year != []):
         if ('-' in year[0]):
             year_range = True
             year = year[0].split('-')
             #only 2 years should be included in input parameter
             if (len(year) > 2):
                 year = []
                 year_range = False
-        elif (',' in year[0]):
-            #split years into multiple years, if multiple are input
-            year = year[0].split(',')
         #parse array for using greater than symbol
         elif ('>' in year[0]):
             year = list(year[0].rpartition(">")[1:])
             greater_than = True
             year.remove('>')
             if (len(year) > 2):
                 year = []
@@ -159,43 +171,103 @@
         elif ('<' in year[0]):
             year = list(year[0].rpartition("<")[1:])
             less_than = True
             year.remove('<')
             if (len(year) > 2):
                 year = []
                 less_than = False
+        elif (',' in year[0]):
+            #split years into multiple years, if multiple are input
+            year = year[0].split(',')
+    #validate each year's format using regex
     for year_ in year:
         #skip to next iteration if < or > symbol
-        if (year_ == '<' or year_ == '>'):
+        if (year_ == '<' or year_ == '>' or year_ == '-'):
             continue
-        #validate year format using regex
-        if not (bool(re.match(r"^1|^2[0-9][0-9][0-9]", year_))):
+        if not (bool(re.match(r"^1[0-9][0-9][0-9]$|^2[0-9][0-9][0-9]$", year_))):
             year = []
             year_range = False 
             break 
 
     #object to store all country updates/changes
     all_changes = {}
+    
+    #temp filename export var
+    temp_filename = os.path.splitext(export_filename)[0]
+    
+    ### Get JSON and CSV filenames based on alpha-2 and year input parameters - concat_updates=True ###
+
+    #append 2 letter alpha-2 codes to export filenames if less than 10 input, append year as well if applicable
+    if (len(alpha2_codes) <= 10 and not (any(code in export_filename for code in alpha2_codes)) and \
+        concat_updates==True and (year != [''] and year != []) and len(year) <= 10 and not \
+            (greater_than or less_than or year_range)):
+
+        #seperate alpha-2 codes and years into comma seperated lists
+        alpha2_str = ','.join(alpha2_codes) 
+        year_str = ','.join(year) 
+
+        #append list of alpha-2 codes and or years to json and csv filenames
+        temp_filename = temp_filename + "-" + alpha2_str + "_" + year_str
+    else:
+        #append 2 letter alpha-2 codes to export filename, year parameter not appended
+        if (len(alpha2_codes) <= 10 and not (any(code in export_filename for code in alpha2_codes)) \
+                and (year == [''] or year == []) and concat_updates==True):
+            
+            #seperate alpha-2 codes into comma seperated lists
+            alpha2_str = ','.join(alpha2_codes) 
+
+            #append list of alpha-2 codes to json and csv filenames
+            temp_filename = temp_filename + "-" + alpha2_str
+        #append greater than/less than/year range symbols to filenames
+        elif ((greater_than or less_than or year_range) and concat_updates==True):
+            
+            #seperate alpha-2 codes and years into comma seperated lists
+            alpha2_str = ','.join(alpha2_codes) 
+            year_str = ','.join(year) 
+            #append alpha-2 codes to filename if less than 10 input
+            if (len(alpha2_codes) <= 10):
+                temp_filename = temp_filename + "-" + alpha2_str
+            
+            #append list of years and gt/lt/year range symbols to json and csv filenames, if applicable
+            if (greater_than):
+                temp_filename = temp_filename + "_>" + year_str
+            elif (less_than):
+                temp_filename = temp_filename + "_<" + year_str
+            elif (year_range):
+                temp_filename = temp_filename + "_" + year[0] + "-" + year[1]
+
+        elif ((input_alpha2_codes == [] or input_alpha2_codes == ['']) and (year != [] and year != ['']) and \
+              concat_updates==True and len(year) <= 10 and not (greater_than or less_than or year_range)):
+            
+            #seperate years into comma seperated lists
+            year_str = ','.join(year) 
 
-    export_fname = export_filename + '-'
+            #append list of years to json and csv filenames
+            temp_filename = temp_filename + "-" + year_str
 
-    #iterate over all input ISO country codes
+    #file export filename   
+    export_filename_concat_updates = temp_filename
+
+    #dataframe for csv export                
+    csv_iso3166_df = pd.DataFrame()
+
+    #iterate over all input ISO 3166-1 country codes
     for alpha2 in alpha2_codes:
         
-        export_fname = export_filename + '-' + alpha2  
-
         #skip to next iteration if alpha-2 not valid
         if (alpha2 not in list(iso3166.countries_by_alpha2.keys())):
             continue
 
-        print("ISO 3166 Code: {} ({})".format(alpha2, wiki_base_url + alpha2))
+        #print out progress of function
+        if (verbose):
+            print("ISO 3166-1 Code: {} ({})".format(alpha2, wiki_base_url + alpha2))
 
         all_changes[alpha2] = {}
 
-        #get html content from wiki of ISO3166 page, raise exception if status code != 200
+        #get html content from wiki of ISO 3166 page, raise exception if status code != 200
         try:
             page = requests.get(wiki_base_url + alpha2, headers=USER_AGENT_HEADER)
             page.raise_for_status()
         except requests.exceptions.HTTPError as err:
             raise SystemExit(err)
 
         #convert html content into BS4 object
@@ -207,174 +279,265 @@
         #skip to next iteration if no changes for ISO code found
         if (changesSection is None):
             continue
 
         #get table element in Changes Section 
         table = changesSection.findNext('table')
         
-        #convert html to 2D array 
+        #convert html table to 2D array 
         iso3166_table = table_to_array(table)
         
         #convert updates html table/2D array to dataframe 
         iso3166_df = get_updates_df(iso3166_table, year, year_range, less_than, greater_than)
 
         #some wiki's have two updates tables  
         iso3166_table_2 = table.findNext('table', {"class": "wikitable"})
 
-        #concat both updates table to 1 df, if applicable 
+        #concatenate both updates table to 1 dataframe, if applicable 
         if (iso3166_table_2 != None):
             #convert secondary table into 2D array
             temp_iso3166_table = table_to_array(iso3166_table_2)
             #several tables have extra unwanted cols meaning we ignore those tables
             if ('former code' not in [col.lower() for col in temp_iso3166_table[0]] and 
                 'in region' not in [col.lower() for col in temp_iso3166_table[0]] and 
                 'before' not in [col.lower() for col in temp_iso3166_table[0]]): 
-                temp_iso3166_df = get_updates_df(temp_iso3166_table, year)
+                temp_iso3166_df = get_updates_df(temp_iso3166_table, year, year_range, less_than, greater_than)
 
-                #concat two dataframes
+                #concat two dataframes together
                 iso3166_df = pd.concat([iso3166_df, temp_iso3166_df], axis=0)
-
+        
         #set Edition/Newsletter to OBP if no value/empty string
         if ((iso3166_df["Edition/Newsletter"] == "").any()):
           iso3166_df["Edition/Newsletter"] = iso3166_df["Edition/Newsletter"].replace('', 
             "Online Browsing Platform (OBP)", regex=True)
 
         #seperate 'Browsing' and 'Platform' string if they are concatenated in column
         iso3166_df["Edition/Newsletter"] = iso3166_df["Edition/Newsletter"].str.replace('BrowsingPlatform', "Browsing Platform")
 
-        #append year onto filename, if not empty
-        export_fname = export_fname + (("-" + str(year)) if year != [] else '')  #potentially need to add strip to export_fname
-        
-        #create output folder if doesn't exist and files are set to be exported
-        if (export_csv or export_json) and not (os.path.isdir(export_folder)):
-            os.mkdir(export_folder)
-
         #only export non-empty dataframes         
         if not (iso3166_df.empty):
             
             #convert date column to datetime object
             iso3166_df['Date Issued'] = pd.to_datetime(iso3166_df["Date Issued"])
             #sort and order by date, newest to oldest
             iso3166_df = iso3166_df.sort_values(by=['Date Issued'], ascending=False)
             #convert date column back to string 
             iso3166_df['Date Issued'] = iso3166_df['Date Issued'].astype(str)
 
-            #export to csv, append extension if applicable
-            if (export_csv): 
-                if (os.path.splitext(export_json_filename)[1] != ".csv"):
-                    export_fname = export_fname + ".csv"
-                iso3166_df.to_csv(os.path.join(export_folder, export_fname), index=False)
-        
-            #add ISO updates to object of all ISO3166 updates, convert to json 
+            #create dataframe for csv export with updates concatenated in same file
+            if (export_csv and concat_updates):
+                if len(alpha2_codes) > 1:
+                    #insert Country Code primary key column in dataframe if more than 1 country exported
+                    iso3166_df.insert(0, "Country Code", alpha2, True)
+                    #concatenate original dataframe with csv dataframe with new primary key column
+                    csv_iso3166_df = pd.concat([iso3166_df, csv_iso3166_df], axis=0)
+                    #drop Country Code column from original dataframe
+                    iso3166_df.drop('Country Code', axis=1, inplace=True)  
+                else:
+                    csv_iso3166_df = iso3166_df
+
+            #add ISO updates to object of all ISO 3166 updates, convert to json 
             all_changes[alpha2] = json.loads(iso3166_df.to_json(orient='records'))
 
-        #reset export filename var 
-        export_fname = export_filename
+    #create output folder if doesn't exist and files are set to be exported
+    if (export_csv or export_json) and not (os.path.isdir(export_folder)):
+        os.mkdir(export_folder)
+            
+    #auxillary function to remove all empty nested dicts within object
+    def _del(_d):
+        return {a:_del(b) if isinstance(b, dict) else b for a, b in _d.items() if b and not a.startswith('_')}
+    
+    #remove any empty country updates dict if year parameter input set and no alpha-2 codes passed into parameter
+    if year != [] and (input_alpha2_codes == [] or input_alpha2_codes == ['']):
+        all_changes = _del(all_changes)
 
-    #append list of alpha-2 codes to exported json filename if 10 or less codes input,
-    #and codes are not already in filename and the multiple outputs are to be concatenated (concat_updates=True)
-    if (len(alpha2_codes) <= 10 and not (any(code in export_json_filename for code in alpha2_codes)) and concat_updates==True):
-        alpha2_str = ','.join(alpha2_codes)
-        if (os.path.splitext(export_json_filename)[1] == ".json"):
-            export_json_filename = os.path.splitext(export_json_filename)[0]
-        export_json_filename = export_json_filename + "-" + alpha2_str + ".json"
-
-    #append extension to json filename, if applicable 
-    if (os.path.splitext(export_json_filename)[1] != ".json"):
-        export_json_filename = export_json_filename + ".json"
-        
-    #export all ISO3166 updates to json, store in export folder dir
+    #temp filename export var
+    temp_filename = os.path.splitext(export_filename)[0]
+    
+    #export all ISO 3166 updates to json, store in export folder dir
     if (export_json):
-        if (all_changes):   #checking if all_changes obj isn't empty
+        all_changes_json = all_changes
+        #checking if all_changes object isn't empty
+        if (all_changes_json):  
+            #if singular country code input and it's contents are empty, set to empty dict
+            if (len(alpha2_codes) == 1 and not (any(all_changes_json.values()))):
+                all_changes_json = {}
             if (concat_updates):
-                #concatenate updates into the same json
-                with open(os.path.join(export_folder, export_json_filename), "w") as write_file:
-                    json.dump(all_changes, write_file, indent=4, ensure_ascii=False)
+                #export updates into the same json
+                with open(os.path.join(export_folder, os.path.splitext(export_filename_concat_updates)[0] + ".json"), "w") as write_file:
+                    json.dump(all_changes_json, write_file, indent=4, ensure_ascii=False)
             else:
                 #seperate country updates into individual json files
-                for update in all_changes:
-                    with open(os.path.join(export_folder, os.path.splitext(export_json_filename)[0] + "-" + update + ".json"), "w") as write_file:
-                        json.dump(all_changes[update], write_file, indent=4, ensure_ascii=False)
+                for update in all_changes_json:
+                    #append alpha-2 codes and list of years or gt/lt/year range symbols, if applicable, to seperate exported json files
+                    if (year != [] and year != ['']):
+                        if (greater_than):
+                            export_filename_no_concat_updates = temp_filename + "-" + update + "_>" + ','.join(year) + ".json"
+                        elif (less_than):
+                            export_filename_no_concat_updates = temp_filename + "-" + update + "_<" + ','.join(year) + ".json"
+                        elif (year_range):
+                            export_filename_no_concat_updates = temp_filename+ "-" + update + "_" + year[0] + "-" + year[1] + ".json"
+                        else:
+                            export_filename_no_concat_updates = temp_filename + "-" + update + "-" + ','.join(year) + ".json"
+                    else:
+                        export_filename_no_concat_updates = temp_filename + "-" + update + ".json"
+
+                    #export updates object to seperate json files
+                    with open(os.path.join(export_folder, export_filename_no_concat_updates), "w") as write_file:
+                        json.dump(all_changes_json[update], write_file, indent=4, ensure_ascii=False)
             
-            print("All ISO3166 changes exported to folder {}.".format(export_folder))
-    
+            #if verbose flag set, print export completion message
+            if (verbose):
+                print("All ISO 3166 updates exported to folder {}.".format(export_folder))
+
+    #export all ISO 3166 updates to csv, store in export folder dir
+    if (export_csv):
+        #checking if all_changes object isn't empty
+        if (all_changes):  
+            #validate all_changes object contains at least one non-empty dict, don't export if all empty dicts
+            if (any(all_changes.values())):
+                if (concat_updates):
+                    #append Country Code column if more than one country input
+                    if len(alpha2_codes) > 1:
+                        #sort dataframe alphabetically using country code column
+                        csv_iso3166_df.sort_values('Country Code', inplace=True)
+                    #export updates object to same concatenated csv file
+                    csv_iso3166_df.to_csv(os.path.join(export_folder, os.path.splitext(export_filename_concat_updates)[0] + ".csv"), index=False)
+                else:
+                    #seperate country updates into individual csv files
+                    for update in all_changes:
+                        #convert updates object into dataframe
+                        temp_updates = pd.DataFrame(all_changes[update])
+                        #skip to next updates object if dataframe is empty
+                        if (temp_updates.empty):
+                            continue
+                        #append alpha-2 codes and list of years or gt/lt/year range symbol, if applicable, to seperate exported csv files
+                        if (year != [] and year != ['']):
+                            if (greater_than):
+                                export_filename_no_concat_updates = temp_filename + "-" + update + "_>" + ','.join(year) + ".csv"
+                            elif (less_than):
+                                export_filename_no_concat_updates = temp_filename + "-" + update + "_<" + ','.join(year) + ".csv"
+                            elif (year_range):
+                                export_filename_no_concat_updates = temp_filename + "-" + update + "_" + year[0] + "-" + year[1] + ".csv"
+                            else:
+                                export_filename_no_concat_updates = temp_filename + "-" + update + "_" + ','.join(year) + ".csv"        
+                        else:
+                            export_filename_no_concat_updates = temp_filename + "-" + update + ".csv"
+                        
+                        #export updates object to seperate csv files
+                        temp_updates.to_csv(os.path.join(export_folder, export_filename_no_concat_updates), index=False)
+
     return all_changes
 
 def get_updates_df(iso3166_updates_table, year=[], year_range=False, less_than=False, greater_than=False):
     """
-    Convert parsed html table, from the Changes Section in the respective ISO3166-2 wiki
-    page, into a pandas dataframe. Convert columns/headers using correct naming 
-    conventions. If year param not empty then remove any rows that don't have 
-    specified year(s) or year range.
+    Convert parsed html table, from the Changes/Updates Section in the respective 
+    ISO 3166-2 wiki page, into a pandas dataframe. Convert columns/headers using 
+    correct naming conventions, correct Date column into correct format and 
+    translate any unicode arrows in the text to normal arrow (->). If year param 
+    not empty then remove any rows that don't have specified year(s). If year 
+    range, less than or greater than parameters set to True then get all updates 
+    from year range or all updates less than or all updates greater than a year, 
+    respectively. 
 
     Parameters
     ----------
     :iso3166_updates_table : array
-        2D array of ISO3166-2 updates from Changes section in wiki.
+        2D array of ISO 3166-2 updates from Changes/Updates section in wiki.
     :year : array
-        array/list of year(s). If not empty only the ISO3166 updates for the selected
+        array/list of year(s). If not empty only the ISO 3166 updates for the selected
         year for a particular country will be returned. If empty then all years of 
         updates are returned.
-
+    :year_range: bool
+        set to True if a range of years are input into year parameter e.g "2002-2010" etc.
+        Function will remove all rows in Dataframe that aren't in specified year range.
+    :less_than: bool
+        set to True if less than symbol is input into year parameter e.g "<2018" etc.
+        Function will remove all rows in Dataframe that are greater than specified year.
+    :greater_than: bool
+        set to True if greater than symbol is input into year parameter e.g ">2005" etc.
+        Function will remove all rows in Dataframe that are less than specified year.
     Returns
     -------
     :iso3166_df : pd.DataFrame
-        converted pandas dataframe of all ISO3166-2 changes for particular country
+        converted pandas dataframe of all ISO 3166-2 changes for particular country/countries
         from 2D input array.
     """
+    #raise error if input updates table isnt an array/list
+    if not isinstance(iso3166_updates_table, list):
+        raise TypeError("Input ISO 3166 updates table parameter must be a array/list, got {}.".format(type(iso3166_updates_table)))
+
     #update column names to correct naming conventions
     cols = correct_columns(iso3166_updates_table[0])
 
+    #lambda function to translate any occurences of unicode arrow → to normal arrow ->
+    correct_arrow_lambda = lambda table: [[elem.replace('→', '->') for elem in entry if isinstance(elem, str)] for entry in table]
+
+    #translate unicode arrow → to normal arrow -> in table text
+    iso3166_updates_table = correct_arrow_lambda(iso3166_updates_table)
+
     #convert 2D array into dataframe    
     iso3166_df = pd.DataFrame(iso3166_updates_table[1:], columns=cols)
 
     #get index and name of Date column in DataFrame, i.e the column that has 'date' in it
     date_col_index = [idx for idx, s in enumerate(list(map(lambda x: x.lower(), iso3166_df.columns))) if 'date' in s]
     date_col_name = list(iso3166_df.columns)[date_col_index[0]]
 
-    def correct_date(row):
+    def corrected_date(row):
         """ parse new date from row if date of changes has been "corrected". """
         if ("corrected" in row):
             return row[row.index("corrected") + len("corrected"):].strip().replace(')', '')
         else:
             return row 
-
+        
+    #reformat date column if date has been corrected
+    iso3166_df[date_col_name] = iso3166_df[date_col_name].apply(corrected_date)
+    
     def get_year(row):
         """ convert string date in rows of df into yyyy-mm-dd data format from date object. """
         return datetime.datetime.strptime(row, '%Y-%m-%d').year
 
-    #reformat date column if date has been corrected
-    iso3166_df[date_col_name] = iso3166_df[date_col_name].apply(correct_date)
-    
-    #only include rows of dataframe where date updated is same as year parameter, drop year col
+    #drop rows of dataframe where Date Issued column isn't same as year parameter, if greater_than, 
+    #less_than or year_range bools set then drop any rows that don't meet condition
     if (year != []): 
-        #create temp year column to get year of updates from date column 
-        iso3166_df['Year'] = iso3166_df[date_col_name].apply(get_year)         
-        temp_iso3166_df_array = []
-        for year_ in year:
-            temp_iso3166_df = iso3166_df[iso3166_df.Year == int(year_)]
-            temp_iso3166_df_array.append(temp_iso3166_df)
+        #create temp year column to get year of updates from date column, convert to str
+        iso3166_df['Year'] = iso3166_df[date_col_name].apply(get_year)     
+        iso3166_df['Year'] = iso3166_df['Year'].astype(str)    
+
+        #drop all rows in dataframe that are less than input year
+        if (greater_than):
+            iso3166_df = iso3166_df.drop(iso3166_df[iso3166_df.Year < year[0]].index)
+        #drop all rows in dataframe that are greater than or equal to input year
+        elif (less_than):
+            iso3166_df = iso3166_df.drop(iso3166_df[iso3166_df.Year >= year[0]].index)
+        #drop all rows in dataframe that are not within input year range
+        elif (year_range):
+            iso3166_df = iso3166_df.drop(iso3166_df[iso3166_df.Year < year[0]].index)
+            iso3166_df = iso3166_df.drop(iso3166_df[iso3166_df.Year > year[1]].index)
+        else:
+            #drop all rows in dataframe that aren't equal to year/list of years in year parameter
+            for year_ in year:
+                iso3166_df = iso3166_df.drop(iso3166_df[iso3166_df.Year != year_].index)
 
-        #concatenate list of correct rows, drop temp year column from dataframe
-        iso3166_df = pd.concat(temp_iso3166_df_array)
+        #drop Year column
         iso3166_df = iso3166_df.drop('Year', axis=1)
 
-    #add below columns if not present so all DF's follow same format
+    #add below columns if not present so all dataframes follow same format
     if ("Edition/Newsletter" not in iso3166_df):
         iso3166_df["Edition/Newsletter"] = ""
 
     if ("Code/Subdivision change" not in iso3166_df):
         iso3166_df["Code/Subdivision change"] = ""
 
-    #reindex/reorder columns in df
+    #reindex/reorder columns in dataframe
     iso3166_df = iso3166_df.reindex(columns=['Date Issued', 'Edition/Newsletter', 
         'Code/Subdivision change', 'Description of change in newsletter'])
 
     #replace all null/nan with empty string
-    iso3166_df.fillna("", inplace = True)
+    iso3166_df.fillna("", inplace=True)
 
     return iso3166_df
 
 def correct_columns(cols):
     """ 
     Update column names so all dataframes follow the column format of:
     ["Date Issued", "Edition/Newsletter", "Code/Subdivision change",
@@ -407,28 +570,32 @@
     Convert html table into 2D array. Much of the function code was inspired from [1] which 
     provides an optimal and working solution for handling tables with different rowspans & 
     colspans. 
 
     Parameters
     ----------
     :table_tag : bs4.element.Tag
-      bs4 object of table element.
+      bs4 Tag object of table element.
     
     Returns
     -------
     :table : tuple
-      tuple of parsed data from html table in Changes section of ISO3166 wiki.
+      tuple of parsed data from html table in Changes section of ISO 3166 wiki.
     
     Reference
     ---------
     [1]: https://stackoverflow.com/questions/48393253/how-to-parse-table-with-rowspan-and-colspan
     """
     #if invalid table tag input return empty array
     if (table_tag is None):
         return []
+    
+    #raise type error if input parameter not a BS4 tag type
+    if not isinstance(table_tag, Tag):
+        raise TypeError("Input table object must be of type bs4.element.Tag, got {}.".format(type(table_tag)))
 
     rowspans = []  #track pending rowspans
     rows = table_tag.find_all('tr') #all table rows
 
     #count columns (including spanned).
     #add active rowspans from preceding rows
     #we *ignore* the colspan value on the last cell, to prevent
@@ -448,14 +615,15 @@
 
     #it doesn't matter if there are still rowspan numbers 'active'; no extra
     #rows to show in the table means the larger than 1 rowspan numbers in the
     #last table row are ignored.
 
     #build an empty matrix for all possible cells
     table = [[None] * colcount for row in rows]
+
     #fill matrix from row data
     rowspans = {}  #track pending rowspans, column number mapping to count
     for row, row_elem in enumerate(rows):
         span_offset = 0  #how many columns are skipped due to row and colspans 
         for col, cell in enumerate(row_elem.find_all(['td', 'th'], recursive=False)):
             #adjust for preceding row and colspans
             col += span_offset
@@ -494,58 +662,45 @@
         #update rowspan bookkeeping
         rowspans = {c: s - 1 for c, s in rowspans.items() if s > 1}
 
     #iterate through converted table, removing any newline characters
     for row in range(0, len(table)):
         for col in range(0, len(table[row])):
             if not (table[row][col] is None):
-                table[row][col] = table[row][col].replace('\n', '')
+                table[row][col] = table[row][col].replace('\n', "")
 
     return table
 
 if __name__ == '__main__':
 
-    parser = argparse.ArgumentParser(description='Get latest changes/updates of ISO3166-2 country codes.')
+    parser = argparse.ArgumentParser(description='Get latest changes/updates for all countries in the ISO 3166-1/3166-2 standard.')
     parser.add_argument('-alpha2', '--alpha2', type=str, required=False, default="", 
-        help='Alpha-2 code/s of ISO3166 countries to check for updates.')
+        help='2 letter alpha-2 code(s) of ISO 3166-1 countries to check for updates.')
     parser.add_argument('-year', '--year', type=str, required=False, default="", 
-        help='Selected year to check for updates.')
+        help='Selected year(s) to check for updates, can also be a year range or greater than/less than specific year.')
     parser.add_argument('-export_filename', '--export_filename', type=str, required=False, default="iso3166-updates", 
-        help='Filename for exported ISO3166 updates csv file.')
-    parser.add_argument('-export_json_filename', '--export_json_filename', type=str, required=False, default="iso3166-updates", 
-        help='Filename for exported ISO3166 updates json file.')
+        help='Filename for exported ISO 3166 updates CSV and JSON files.')
     parser.add_argument('-export_folder', '--export_folder', type=str, required=False, default="test-iso3166-updates", 
         help='Folder where to store exported ISO files.')
-    parser.add_argument('-export_json', '--export_json', action="store_false", required=False, 
+    parser.add_argument('-export_json', '--export_json', required=False, action=argparse.BooleanOptionalAction, default=1,
         help='Whether to export all found updates to json.')
-    parser.add_argument('-export_csv', '--export_csv', required=False, action="store_true", 
+    parser.add_argument('-export_csv', '--export_csv', required=False, action=argparse.BooleanOptionalAction, default=0,
         help='Whether to export all found updates to csv files in export folder.')
-    parser.add_argument('-concat_updates', '--concat_updates', action="store_true", default=True, required=False, 
-        help='Whether to concatenate updates of individual countrys into the same json file or individual. Only applies to JSON files, not CSVs.')
+    parser.add_argument('-concat_updates', '--concat_updates', required=False, action=argparse.BooleanOptionalAction, default=1,
+        help='Whether to concatenate updates of individual countrys into the same json or csv files or individual files.')
+    parser.add_argument('-verbose', '--verbose', type=int, required=False, action=argparse.BooleanOptionalAction, default=1, 
+        help='Set to 1 to print out progress of updates function, 0 will not print progress.')
 
     #parse input args
     args = parser.parse_args()
-    alpha2_codes = [args.alpha2]
-    if (',' in alpha2_codes[0]):
-        alpha2_codes = alpha2_codes[0].split(',')
-    export_filename = args.export_filename
-    export_json_filename = args.export_json_filename
+    alpha2_codes = args.alpha2
     export_folder = args.export_folder
     concat_updates = args.concat_updates
     export_json = args.export_json
     export_csv = args.export_csv
-    year = [args.year]
-    if (',' in year[0]):
-        year = year[0].split(',')
-    alpha_codes = []
-
-    #use all ISO3166 codes if invalid alpha-2 code input, otherwise convert alpha-2 to array
-    if (alpha2_codes == [''] or not isinstance(alpha2_codes, list)):
-        alpha2_codes = sorted(list(iso3166.countries_by_alpha2.keys()))
-
-    #sort codes in alphabetical order
-    alpha2_codes.sort()
-    alpha2_codes = [code.upper() for code in alpha2_codes]
+    year = args.year
+    verbose = args.verbose
+    export_filename = args.export_filename
     
-    #output ISO3166 updates/changes for selected alpha-2 code/s
-    get_updates(alpha2_codes, year, export_filename, export_json_filename,
-        export_folder, concat_updates, export_json, export_csv)
+    #output ISO 3166 updates/changes for selected alpha-2 code(s) and year(s)
+    get_updates(alpha2_codes, year, export_filename, export_folder, 
+        concat_updates, export_json, export_csv, verbose)
```

### Comparing `iso3166-updates-1.2.2/iso3166_updates.egg-info/PKG-INFO` & `iso3166-updates-1.3.0/iso3166_updates.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,261 +1,18 @@
 Metadata-Version: 2.1
 Name: iso3166-updates
-Version: 1.2.2
+Version: 1.3.0
 Summary: A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 Home-page: https://github.com/amckenna41/iso3166-updates
 Author: AJ McKenna, https://github.com/amckenna41
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
-Description: # iso3166-updates
-        
-        [![iso3166_updates](https://img.shields.io/pypi/v/iso3166-updates)](https://pypi.org/project/iso3166-updates/)
-        [![pytest](https://github.com/amckenna41/iso3166-updates/workflows/Building%20and%20Testing/badge.svg)](https://github.com/amckenna41/iso3166-updates/actions?query=workflowBuilding%20and%20Testing)
-        [![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/iso3166-updates/)
-        [![License: MIT](https://img.shields.io/github/license/amckenna41/iso3166-updates)](https://opensource.org/licenses/MIT)
-        <!-- [![CircleCI](https://circleci.com/gh/amckenna41/iso3166-updates.svg?style=svg&circle-token=d860bb64668be19d44f106841b80eb47a8b7e7e8)](https://app.circleci.com/pipelines/github/amckenna41/iso3166-updates) -->
-        [![Issues](https://img.shields.io/github/issues/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates/issues)
-        [![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates)
-        <!-- [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-updates)](https://github.com/iso3166-updates) -->
-        
-        <div alt="images" style="justify-content: center; display:flex; margin-left=50px;">
-          <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="200" width="500"/>
-          <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="200" width="300"/>
-        </div>
-        
-        > Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here][demo].
-        
-        Table of Contents
-        -----------------
-          * [Introduction](#introduction)
-          * [API](#api)
-          * [Staying up to date](#staying-up-to-date)
-          * [Requirements](#requirements)
-          * [Installation](#installation)
-          * [Usage](#usage)
-          * [Directories](#Directories)
-          * [Issues](#Issues)
-          * [Contact](#contact)
-          * [References](#references)
-        
-        Introduction
-        ------------
-        `iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
-        
-        The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations [[1]](#references). The ISO 3166-2 was first published in 1998 and as of 29 November 2022 there are 5,043 codes defined in it [[2]](#references).
-        
-        ### Problem Statement:
-        
-        The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
-        
-        This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of country's ISO 3166-2 codes for free, with an easy-to-use interface and Python package and API, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
-        
-        <strong> The earliest date for any ISO 3166 updates is 2000-06-21, and the most recent is 2022-11-29. </strong>
-        
-        ### Intended Audience:
-        
-        This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (excluding 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API (https://iso3166-updates.com). 
-        
-        API
-        ---
-        An API is available that can be used to extract any applicable updates for a country via a URL. The API is available at the URL:
-        
-        > https://www.iso3166-updates.com/api
-        
-        Three query string parameters/paths are available in the API - `alpha2`, `year` and `months`. The 2 letter alpha-2 country code can be appeneded to the url as a query string parameter - "?alpha2=JP". A single alpha-2 or list of them can be passed to the API (e.g "FR", "DE", "HU, ID, MA"). The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "?year=2017", "2010-2015", "<2009", ">2002"). Finally, the months parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g "?month=6", "?month=48").
-        
-        The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON with all ISO 3166 updates. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure the hosting was switched to Vercel (https://vercel.com/).
-        
-        The API documentation and usage with all useful commands and examples to the API is available on the [README](https://github.com/amckenna41/iso3166-updates/blob/main/iso3166-updates-api/README.md) of the iso3166-updates-api folder. 
-        
-        <p align="center">
-          <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_arch.png" alt="gcp_arch" height="200" width="400"/>
-        </p>
-        
-        Staying up to date
-        ------------------
-        The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. 
-        The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO 3166-2 wiki's to check for the latest updates within a certain period e.g the past 3-6 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data.
-        
-        Additionally, a GitHub Issue in the `iso3166-2` and `iso3166-flag-icons` repositories will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-2` and `iso3166-flag-icons` JSONs and repos.
-        
-        Ultimately, this Cloud Function ensures that the software and assoicated APIs are up-to-date with the latest ISO 3166-2 information for all countries/territories/subdivisions etc.
-        
-        Requirements
-        ------------
-        * [python][python] >= 3.7
-        * [pandas][pandas] >= 1.4.3
-        * [numpy][numpy] >= 1.23.2
-        * [requests][requests] >= 2.28.1
-        * [beautifulsoup4][beautifulsoup4] >= 4.11.1
-        * [iso3166][iso3166] >= 2.1.1
-        
-        Installation
-        ------------
-        Install the latest version of `iso3166-updates` via [PyPi][PyPi] using pip:
-        
-        ```bash
-        pip3 install iso3166-updates --upgrade
-        ```
-        
-        Installation from source:
-        ```bash
-        git clone -b master https://github.com/amckenna41/iso3166-updates.git
-        cd iso3166_updates
-        python3 setup.py install
-        ```
-        
-        Usage
-        -----
-        **Import package:**
-        ```python
-        import iso3166_updates as iso3166_updates
-        ```
-        
-        **Input parameters to get_updates function:**
-        ```python
-          # -alpha2 ALPHA2, --alpha2 ALPHA2
-          #                       Alpha-2 code/s of ISO3166 countries to check for updates.
-          # -export_filename EXPORT_FILENAME, --export_filename EXPORT_FILENAME
-          #                       Filename for exported ISO3166 updates csv file.
-          # -export_json_filename EXPORT_JSON_FILENAME, --export_json_filename EXPORT_JSON_FILENAME
-          #                       Filename for exported ISO3166 updates json file.
-          # -export_folder EXPORT_FOLDER, --export_folder EXPORT_FOLDER
-          #                       Folder where to store exported ISO files.
-          # -export_json, --export_json
-          #                       Whether to export all found updates to json.
-          # -export_csv, --export_csv
-          #                       Whether to export all found updates to csv files in export folder.
-          # -year YEAR, --year YEAR
-          #                       Selected year to check for updates.
-          # -concat_updates, --concat_updates
-          #                       Whether to concatenate updates of individual countrys into the same json file or seperate.
-        ```
-        
-        **Get all listed changes/updates for all countries which happens by default if no alpha-2 codes specified in input param, export csv and json to folder "iso3166-updates":**
-        ```python
-        iso3166_updates.get_updates(export_folder="iso3166-updates", export_json=1, export_csv=1)
-        ```
-        
-        **Get all listed changes/updates for Andorra from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:AD), export csv and json to folder "iso3166-updates":**
-        ```python
-        iso3166_updates.get_updates("AD", export_folder="iso3166-updates", export_json=1, export_csv=1)
-        ```
-        
-        **Get all listed changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates":**
-        ```python
-        iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=0))
-        ```
-        
-        **Get any listed changes/updates for HU, IT, JA, KE from wiki, in the year 2018, export only to JSON with filename "iso3166-updates.json" and seperate updates into sepetate JSON files:**
-        ```python
-        iso3166_updates.get_updates("HU, IT, JA, KE", year="2018", export_json=1, export_csv=0, export_json_filename="iso3166-updates", concat_updates=0)
-        ```
-        
-        **Get any listed changes/updates for Ireland from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:IE), between years of 2012 and 2021, use default parameters:**
-        ```python
-        iso3166_updates.get_updates("IE", year="2012-2021")
-        ```
-        
-        **Get any listed changes/updates for Tanzania from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:TZ), with updates years >=2015, export only to CSV with filename "iso3166-output.csv":**
-        ```python
-        iso3166_updates.get_updates("TA", year=">2015", export_filename="iso3166-output.csv")
-        ```
-        
-        **Get any listed changes/updates for Yemen from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:YE), with updates years < 2010, use default parameters:**
-        ```python
-        iso3166_updates.get_updates("YE", year="<2010")
-        ```
-        
-        The output to the above functions for the updates/changes to a ISO 3166-2 country returns 4 columns: 
-        <b>Edition/Newsletter, Date Issued, Code/Subdivision change</b> and <b>Description of change in newsletter.</b> 
-        
-        * Edition/Newsletter: Name and or edition of newsletter that ISO 3166-2 change/update was communicated in.
-        * Date Issued: Date that the change was communicated.
-        * Code/Subdivision change: Overall summary of change/update made.
-        * Description of change in newsletter: More in-depth info about the change/update that was made.
-        
-        E.g. The output format of the exported CSV for AD (Andorra) is:
-        
-        | Edition/Newsletter | Date Issued | Code/Subdivision change | Description of change in newsletter |   
-        |:-------------------|:------------|------------------------------------:|------------------------:|
-        | Newsletter I-8     | 2007-04-17  | Subdivisions added: 7 parishes...   | Addition of the administrative subdivisions...                 | 
-        | Online Browsing Platform (OBP) | 2014-11-03 | No subdivision changes listed | Update List Source |
-        | Online Browsing Platform (OBP) | 2015-11-27 | No subdivision changes listed | Update List Source | 
-        
-        E.g. The output format of the exported JSON for AD (Andorra) is:
-        ```javascript
-        {
-          AD: [
-              {
-                "Code/Subdivision change": "",
-                "Date Issued": "2015-11-27",
-                "Description of change in newsletter": "Update List Source",
-                "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)"
-              },
-              {
-                "Code/Subdivision change": "",
-                "Date Issued": "2014-11-03",
-                "Description of change in newsletter": "Update List Source",
-                "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)"
-              },
-              {
-                "Code/Subdivision change:" "Subdivisions added:7 parishes",
-                "Date Issued": "2007-04-17",
-                "Description of change in newsletter": "Addition of the administrative subdivisions and of their code elements",
-                "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)"
-              }
-          ]
-        }
-        ```
-        
-        Directories
-        -----------
-        * `/docs` - documentation for `iso3166-updates` Python package.
-        * `/iso3166_updates` - source code for `iso3166-updates` Python package.
-        * `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the `iso3166-updates` API, including the main.py, requirements.txt and API config file.
-        * `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Function for the check-for-updates function which is a periodically called Cloud Function that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date. Includes the main.py and requirements.txt files.
-        * `/tests` - unit and integration tests for `iso3166-updates`.
-        
-        Issues
-        ------
-        Any issues, errors or bugs can be raised via the [Issues](Issues) tab in the repository. Also if there are any missing or incorrect data in the updates json, this should also be raised by creating an issue. 
-        
-        Contact
-        -------
-        If you have any questions or comments, please contact amckenna41@qub.ac.uk or raise an issue on the [Issues][Issues] tab. <br><br>
-        [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/)
-        
-        References
-        ----------
-        \[1\]: ISO3166-1: https://en.wikipedia.org/wiki/ISO_3166-1 <br>
-        \[2\]: ISO3166-2: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
-        \[3\]: ISO Country Codes Collection: https://www.iso.org/publication/PUB500001 <br>
-        \[4\]: ISO Country Codes: https://www.iso.org/iso-3166-country-codes.html <br>
-        \[5\]: ISO3166-1 flag-icons repo: https://github.com/lipis/flag-icons <br>
-        \[6\]: ISO3166-2 flag-icons repo: https://github.com/amckenna41/iso3166-flag-icons <br>
-        
-        Support
-        -------
-        <a href="https://www.buymeacoffee.com/amckenna41" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
-        
-        [Back to top](#TOP)
-        
-        [demo]: https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing
-        [python]: https://www.python.org/downloads/release/python-360/
-        [pandas]: https://pandas.pydata.org/
-        [numpy]: https://numpy.org/
-        [requests]: https://requests.readthedocs.io/
-        [beautifulsoup4]: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
-        [iso3166]: https://github.com/deactivated/python-iso3166
-        [PyPi]: https://pypi.org/project/iso3166-updates/
-        [Issues]: https://github.com/amckenna41/iso3166-updates/issues
-Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,csviso3166-2,iso3166-1,alpha2,alpha3
+Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,csv,iso3166-2,iso3166-1,alpha-2,alpha-3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
@@ -271,7 +28,269 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
+License-File: LICENSE
+
+# iso3166-updates
+
+[![iso3166_updates](https://img.shields.io/pypi/v/iso3166-updates)](https://pypi.org/project/iso3166-updates/)
+[![pytest](https://github.com/amckenna41/iso3166-updates/workflows/Building%20and%20Testing/badge.svg)](https://github.com/amckenna41/iso3166-updates/actions?query=workflowBuilding%20and%20Testing)
+[![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/iso3166-updates/)
+[![License: MIT](https://img.shields.io/github/license/amckenna41/iso3166-updates)](https://opensource.org/licenses/MIT)
+<!-- [![CircleCI](https://circleci.com/gh/amckenna41/iso3166-updates.svg?style=svg&circle-token=d860bb64668be19d44f106841b80eb47a8b7e7e8)](https://app.circleci.com/pipelines/github/amckenna41/iso3166-updates) -->
+[![Issues](https://img.shields.io/github/issues/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates/issues)
+[![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates)
+<!-- [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-updates)](https://github.com/iso3166-updates) -->
+
+<div alt="images" style="justify-content: center; display:flex; margin-left=50px;">
+  <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="200" width="500"/>
+  <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="200" width="300"/>
+</div>
+
+> Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here][demo].
+
+Table of Contents
+-----------------
+  * [Introduction](#introduction)
+  * [API](#api)
+  * [Staying up to date](#staying-up-to-date)
+  * [Requirements](#requirements)
+  * [Installation](#installation)
+  * [Usage](#usage)
+  * [Directories](#Directories)
+  * [Issues](#Issues)
+  * [Contact](#contact)
+  * [References](#references)
+
+Introduction
+------------
+`iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
+
+The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations [[1]](#references). The ISO 3166-2 was first published in 1998 and as of 29 November 2022 there are 5,043 codes defined in it [[2]](#references).
+
+### Problem Statement:
+
+The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
+
+This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of country's ISO 3166-2 codes for free, with an easy-to-use interface and Python package and API, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
+
+<strong> The earliest date for any ISO 3166 updates is 2000-06-21, and the most recent is 2022-11-29. </strong>
+
+### Intended Audience:
+
+This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (excluding 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API (https://iso3166-updates.com). 
+
+API
+---
+An API is available that can be used to extract any applicable updates for a country via a URL. The API is available at the URL:
+
+> https://www.iso3166-updates.com/api
+
+Three query string parameters/paths are available in the API - `alpha2`, `year` and `months`. The 2 letter alpha-2 country code can be appeneded to the url as a query string parameter - "?alpha2=JP". A single alpha-2 or list of them can be passed to the API (e.g "FR", "DE", "HU, ID, MA"). The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "?year=2017", "2010-2015", "<2009", ">2002"). Finally, the months parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g "?month=6", "?month=48").
+
+The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON with all ISO 3166 updates. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure the hosting was switched to Vercel (https://vercel.com/).
+
+The API documentation and usage with all useful commands and examples to the API is available on the [README](https://github.com/amckenna41/iso3166-updates/blob/main/iso3166-updates-api/README.md) of the iso3166-updates-api folder. 
+
+<p align="center">
+  <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_arch.png" alt="gcp_arch" height="200" width="400"/>
+</p>
+
+Staying up to date
+------------------
+The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. 
+The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO 3166-2 wiki's to check for the latest updates within a certain period e.g the past 3-6 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data.
+
+Additionally, a GitHub Issue in the `iso3166-2` and `iso3166-flag-icons` repositories will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-2` and `iso3166-flag-icons` JSONs and repos.
+
+Ultimately, this Cloud Function ensures that the software and assoicated APIs are up-to-date with the latest ISO 3166-2 information for all countries/territories/subdivisions etc.
+
+Requirements
+------------
+* [python][python] >= 3.7
+* [pandas][pandas] >= 1.4.3
+* [numpy][numpy] >= 1.23.2
+* [requests][requests] >= 2.28.1
+* [beautifulsoup4][beautifulsoup4] >= 4.11.1
+* [iso3166][iso3166] >= 2.1.1
+
+Installation
+------------
+Install the latest version of `iso3166-updates` via [PyPi][PyPi] using pip:
+
+```bash
+pip3 install iso3166-updates --upgrade
+```
+
+Installation from source:
+```bash
+git clone -b master https://github.com/amckenna41/iso3166-updates.git
+cd iso3166_updates
+python3 setup.py install
+```
+
+Usage
+-----
+**Import package:**
+```python
+import iso3166_updates as iso3166_updates
+```
+
+**Input parameters to get_updates function:**
+```python
+  # -alpha2 ALPHA2, --alpha2 ALPHA2
+  #                       Alpha-2 code/s of ISO3166 countries to check for updates.
+  # -export_filename EXPORT_FILENAME, --export_filename EXPORT_FILENAME
+  #                       Filename for exported ISO3166 updates for CSV and JSON files.
+  # -export_folder EXPORT_FOLDER, --export_folder EXPORT_FOLDER
+  #                       Folder where to store exported ISO files.
+  # -export_json, --export_json
+  #                       Whether to export all found updates to json.
+  # -export_csv, --export_csv
+  #                       Whether to export all found updates to csv files in export folder.
+  # -year YEAR, --year YEAR
+  #                       Selected year to check for updates.
+  # -concat_updates, --concat_updates
+  #                       Whether to concatenate updates of individual countrys into the same json file or seperate.
+```
+
+**Get all listed changes/updates for all countries which happens by default if no alpha-2 codes specified in input param, export csv and json to folder "iso3166-updates":**
+```python
+iso3166_updates.get_updates(export_folder="iso3166-updates", export_json=1, export_csv=1)
+#exported files: /iso3166-updates/iso3166-updates.json and /iso3166-updates/iso3166-updates.csv
+```
+
+**Get all listed changes/updates for Andorra from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:AD), export csv and json to folder "iso3166-updates":**
+```python
+iso3166_updates.get_updates("AD", export_folder="iso3166-updates", export_json=1, export_csv=1)
+#exported files: /iso3166-updates/iso3166-updates-AD.json and /iso3166-updates/iso3166-updates-AD.csv
+```
+
+**Get all listed changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates":**
+```python
+iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=0)
+#exported files: /iso3166-updates/iso3166-updates-BA,DE,FR,HU,PY.json
+```
+
+**Get any listed changes/updates for HU, IT, JA, KE from wiki, in the year 2018, export only to JSON with filename "iso3166-updates.json" and seperate updates into sepetate JSON files:**
+```python
+iso3166_updates.get_updates("HU, IT, JA, KE", year="2018", export_json=1, export_csv=0, export_filename="iso3166-updates", concat_updates=0)
+#exported files: /iso3166-updates/iso3166-updates-HU,IT,JA,KE-2018.json
+```
+
+**Get any listed changes/updates for Ireland from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:IE), between years of 2012 and 2021, use default parameters:**
+```python
+iso3166_updates.get_updates("IE", year="2012-2021")
+#exported files: /iso3166-updates/iso3166-updates-IE_2012-2021.json
+```
+
+**Get any listed changes/updates for Tanzania from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:TZ), with updates years >=2015, export only to CSV with filename iso3166-output":**
+```python
+iso3166_updates.get_updates("TA", year=">2015", export_filename="iso3166-output", export_json=0, export_csv=1)
+#exported files: /iso3166-updates/iso3166-output-TA_>2015.csv
+```
+
+**Get any listed changes/updates for Yemen from wiki (https://en.wikipedia.org/wiki/ISO_3166-2:YE), with updates years < 2010, use default parameters:**
+```python
+iso3166_updates.get_updates("YE", year="<2010")
+#exported files: /iso3166-updates/iso3166-output-YE_<2010.json
+```
+## Terminal/Command Line
+
+**Get all listed changes/updates for all countries, export csv and json to folder "iso3166-updates", print progress using verbose parameter:** 
+```bash
+python3 iso3166_updates.py --export_folder="iso3166-updates" --export_csv --export_json --verbose
+```
+
+**Get all listed changes/updates for BY, DJ, ET, LY, PA for year range 2005-2010, export only CSV of updates to export folder "iso3166-updates", print progress using verbose parameter:**
+```bash
+python3 iso3166_updates.py --alpha2="BY, DJ, ET, LY, PA" --year="2005-2010" --export_folder="iso3166-updates" --export_csv --no-export_json --verbose
+```
+
+The output to the above functions for the updates/changes to a ISO 3166-2 country returns 4 columns: 
+<b>Edition/Newsletter, Date Issued, Code/Subdivision change</b> and <b>Description of change in newsletter.</b> For the CSV export, if more than one country input then an addition primary key column <b>Country Code</b> will be prepended to the first column, which will be the 2 letter ISO 3166-1 country code. 
+
+* Edition/Newsletter: Name and or edition of newsletter that ISO 3166-2 change/update was communicated in.
+* Date Issued: Date that the change was communicated.
+* Code/Subdivision change: Overall summary of change/update made.
+* Description of change in newsletter: More in-depth info about the change/update that was made.
+
+E.g. The output format of the exported CSV for AD (Andorra) is:
+
+| Edition/Newsletter | Date Issued | Code/Subdivision change | Description of change in newsletter |   
+|:-------------------|:------------|------------------------------------:|------------------------:|
+| Newsletter I-8     | 2007-04-17  | Subdivisions added: 7 parishes...   | Addition of the administrative subdivisions...                 | 
+| Online Browsing Platform (OBP) | 2014-11-03 | No subdivision changes listed | Update List Source |
+| Online Browsing Platform (OBP) | 2015-11-27 | No subdivision changes listed | Update List Source | 
+
+E.g. The output format of the exported JSON for AD (Andorra) is:
+```javascript
+{
+  AD: [
+      {
+        "Code/Subdivision change": "",
+        "Date Issued": "2015-11-27",
+        "Description of change in newsletter": "Update List Source",
+        "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)"
+      },
+      {
+        "Code/Subdivision change": "",
+        "Date Issued": "2014-11-03",
+        "Description of change in newsletter": "Update List Source",
+        "Edition/Newsletter": "Online Browsing Platform (OBP) (https://www.iso.org/obp/ui/#iso:code:3166:AD)"
+      },
+      {
+        "Code/Subdivision change:" "Subdivisions added:7 parishes",
+        "Date Issued": "2007-04-17",
+        "Description of change in newsletter": "Addition of the administrative subdivisions and of their code elements",
+        "Edition/Newsletter": "Newsletter I-8 (https://web.archive.org/web/20120330105926/http://www.iso.org/iso/iso_3166-2_newsletter_i-8_en.pdf)"
+      }
+  ]
+}
+```
+
+Directories
+-----------
+* `/docs` - documentation for `iso3166-updates` Python package.
+* `/iso3166_updates` - source code for `iso3166-updates` Python package.
+* `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the `iso3166-updates` API, including the main.py, requirements.txt and API config file.
+* `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Function for the check-for-updates function which is a periodically called Cloud Function that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date. Includes the main.py and requirements.txt files.
+* `/tests` - unit and integration tests for `iso3166-updates`.
+
+Issues
+------
+Any issues, errors or bugs can be raised via the [Issues](Issues) tab in the repository. Also if there are any missing or incorrect data in the updates json, this should also be raised by creating an issue. 
+
+Contact
+-------
+If you have any questions or comments, please contact amckenna41@qub.ac.uk or raise an issue on the [Issues][Issues] tab. <br><br>
+[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/)
+
+References
+----------
+\[1\]: ISO3166-1: https://en.wikipedia.org/wiki/ISO_3166-1 <br>
+\[2\]: ISO3166-2: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
+\[3\]: ISO Country Codes Collection: https://www.iso.org/publication/PUB500001 <br>
+\[4\]: ISO Country Codes: https://www.iso.org/iso-3166-country-codes.html <br>
+\[5\]: ISO3166-1 flag-icons repo: https://github.com/lipis/flag-icons <br>
+\[6\]: ISO3166-2 flag-icons repo: https://github.com/amckenna41/iso3166-flag-icons <br>
+
+Support
+-------
+<a href="https://www.buymeacoffee.com/amckenna41" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
+
+[Back to top](#TOP)
+
+[demo]: https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing
+[python]: https://www.python.org/downloads/release/python-360/
+[pandas]: https://pandas.pydata.org/
+[numpy]: https://numpy.org/
+[requests]: https://requests.readthedocs.io/
+[beautifulsoup4]: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
+[iso3166]: https://github.com/deactivated/python-iso3166
+[PyPi]: https://pypi.org/project/iso3166-updates/
+[Issues]: https://github.com/amckenna41/iso3166-updates/issues
+
```

### Comparing `iso3166-updates-1.2.2/setup.cfg` & `iso3166-updates-1.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iso3166-updates
-version = 1.2.2
+version = 1.3.0
 description = A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = AJ McKenna
 author_email = amckenna41@qub.ac.uk
 url = https://github.com/amckenna41/iso3166-updates
 download_url = https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
```

### Comparing `iso3166-updates-1.2.2/setup.py` & `iso3166-updates-1.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 ###############################################################################
 #####   Setup.py - installs all the required packages and dependancies    #####
 ###############################################################################
 
 import pathlib
 from setuptools import setup, find_packages
 import sys
-# import iso3166_updates
 
 #software metadata
 __name__ = 'iso3166-updates'
-__version__ = "1.2.2"
+__version__ = "1.3.0"
 __description__ = "A Python package that pulls the latest updates & changes to all ISO3166 listed countries."
 __author__ = 'AJ McKenna, https://github.com/amckenna41'
 __authorEmail__ = 'amckenna41@qub.ac.uk'
 __license__ = 'MIT'
 __url__ = 'https://github.com/amckenna41/iso3166-updates'
 __download_url__ = "https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip"
 __status__ = 'Development'
 __maintainer__ = "AJ McKenna"
-__keywords__ = ["iso", "iso3166", "beautifulsoup", "python", "pypi", "countries", "country codes", "csv" \
-            "iso3166-2", "iso3166-1", "alpha2", "alpha3"]
+__keywords__ = ["iso", "iso3166", "beautifulsoup", "python", "pypi", "countries", "country codes", "csv", \
+            "iso3166-2", "iso3166-1", "alpha-2", "alpha-3"]
 __test_suite__ = "tests"
  
 #ensure python version is greater than 3
 if (sys.version_info[0] < 3):
     sys.exit('Python 3 is the minimum version requirement.')
 
 #get path to README file
```

