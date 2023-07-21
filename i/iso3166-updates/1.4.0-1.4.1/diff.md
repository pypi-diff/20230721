# Comparing `tmp/iso3166-updates-1.4.0.tar.gz` & `tmp/iso3166-updates-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iso3166-updates-1.4.0.tar", last modified: Thu Jul 20 19:26:12 2023, max compression
+gzip compressed data, was "iso3166-updates-1.4.1.tar", last modified: Fri Jul 21 15:13:27 2023, max compression
```

## Comparing `iso3166-updates-1.4.0.tar` & `iso3166-updates-1.4.1.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:26:12.312900 iso3166-updates-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-20 19:25:42.000000 iso3166-updates-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21765 2023-07-20 19:26:12.312900 iso3166-updates-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20201 2023-07-20 19:25:42.000000 iso3166-updates-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:26:12.312900 iso3166-updates-1.4.0/iso3166_updates/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-20 19:25:42.000000 iso3166-updates-1.4.0/iso3166_updates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14799 2023-07-20 19:25:42.000000 iso3166-updates-1.4.0/iso3166_updates/iso3166_updates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:26:12.312900 iso3166-updates-1.4.0/iso3166_updates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21765 2023-07-20 19:26:12.000000 iso3166-updates-1.4.0/iso3166_updates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-20 19:26:12.000000 iso3166-updates-1.4.0/iso3166_updates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:26:12.000000 iso3166-updates-1.4.0/iso3166_updates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:26:11.000000 iso3166-updates-1.4.0/iso3166_updates.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-20 19:26:12.000000 iso3166-updates-1.4.0/iso3166_updates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 19:26:12.000000 iso3166-updates-1.4.0/iso3166_updates.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-20 19:26:12.312900 iso3166-updates-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-20 19:25:42.000000 iso3166-updates-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:13:27.693669 iso3166-updates-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-21 15:12:51.000000 iso3166-updates-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-21 15:12:51.000000 iso3166-updates-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    22890 2023-07-21 15:13:27.693669 iso3166-updates-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-07-21 15:12:51.000000 iso3166-updates-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:13:27.689669 iso3166-updates-1.4.1/iso3166_updates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-21 15:12:51.000000 iso3166-updates-1.4.1/iso3166_updates/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-21 15:12:51.000000 iso3166-updates-1.4.1/iso3166_updates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   318079 2023-07-21 15:12:51.000000 iso3166-updates-1.4.1/iso3166_updates/iso3166-updates.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14910 2023-07-21 15:12:51.000000 iso3166-updates-1.4.1/iso3166_updates/iso3166_updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:13:27.693669 iso3166-updates-1.4.1/iso3166_updates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22890 2023-07-21 15:13:27.000000 iso3166-updates-1.4.1/iso3166_updates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-21 15:13:27.000000 iso3166-updates-1.4.1/iso3166_updates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:13:27.000000 iso3166-updates-1.4.1/iso3166_updates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:13:26.000000 iso3166-updates-1.4.1/iso3166_updates.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-21 15:13:27.000000 iso3166-updates-1.4.1/iso3166_updates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 15:13:27.000000 iso3166-updates-1.4.1/iso3166_updates.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-21 15:13:27.693669 iso3166-updates-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-21 15:12:51.000000 iso3166-updates-1.4.1/setup.py
```

### Comparing `iso3166-updates-1.4.0/LICENSE` & `iso3166-updates-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iso3166-updates-1.4.0/PKG-INFO` & `iso3166-updates-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: iso3166-updates
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 Home-page: https://github.com/amckenna41/iso3166-updates
 Author: AJ McKenna, https://github.com/amckenna41
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
-Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,csv,iso3166-2,iso3166-1,alpha-2,alpha-3
+Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,csv,iso3166-2,iso3166-1,alpha-2,alpha-3,selenium,chromedriver
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
@@ -46,76 +46,87 @@
 <!-- [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-updates)](https://github.com/iso3166-updates) -->
 
 <div alt="images" style="justify-content: center; display:flex; margin-left=50px;">
   <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="200" width="500"/>
   <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="200" width="300"/>
 </div>
 
-> Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a lightweight Python software package and API; a demo of both is available [here][demo].
+> Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a lightweight Python software package and API; a demo of both is available [here][demo]. There is also a demo of the script used to pull and export all the latest updates, available [here][demo_2].
 
 Table of Contents
 -----------------
   * [Introduction](#introduction)
   * [API](#api)
   * [Staying up to date](#staying-up-to-date)
   * [Requirements](#requirements)
   * [Installation](#installation)
-  * [Usage](#usage)
+  * [Usage (iso3166-updates-Python-package)](#usage-iso3166-updates-Python-package)
+  * [Usage (get_all_iso3166_updates.py script)](#usage-get_all_iso3166_updates.py-script)
   * [Directories](#Directories)
   * [Issues](#Issues)
   * [Contact](#contact)
   * [References](#references)
 
 Introduction
 ------------
-`iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
+`iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
 
 The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations [[1]](#references). The ISO 3166-2 was first published in 1998 and as of 29 November 2022 there are 5,043 codes defined in it [[2]](#references).
 
 ### Problem Statement:
 
-The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
+The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Typically these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
 
 This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of country's ISO 3166-2 codes for free, with an easy-to-use interface and Python package and API, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
 
-<strong> The earliest date for any ISO 3166 updates is 2000-06-21, and the most recent is 2022-11-29. </strong>
+<strong> The earliest date for any ISO 3166-2 update is 2000-06-21, and the most recent is 2022-11-29. </strong>
 
 ### Intended Audience:
 
 This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (excluding 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API (https://iso3166-updates.com). 
 
 API
 ---
-An API is available that can be used to extract any applicable updates for a country via a URL. The API is available at the URL:
+An API is available that can be used to extract any applicable updates for a country via an API endpoint. The API is available at the URL:
 
 > https://www.iso3166-updates.com/api
 
-Three query string parameters are available in the API - `alpha2`, `year` and `months`. 
+The other endpoints available in the API are:
 
-* The 2 letter alpha-2 country code can be appended to the url as a query string parameter or as its own path ("?alpha2=JP" or /alpha2/JP). A single alpha-2 or list of them can be passed to the API (e.g "?alpha2="FR, DE, HU, ID, MA" or /alpha2/FR,DE,HU,ID,MA). The 3 letter alpha-3 counterpart for each country's alpha-2 code can also be passed into the `alpha2` parameter (e.g "?alpha2="FRA, DEU, HUN, IDN, MAR" or /alpha2/FRA,DEU,HUN,IDN,MAR). 
+* https://iso3166-updates.com/api/alpha2/<input_alpha2>
+* https://iso3166-updates.com/api/name/<input_name>
+* https://iso3166-updates.com/api/year/<year>
+* https://iso3166-updates.com/api/alpha2/<input_alpha2>/year/<input_year>
+* https://iso3166-updates.com/api/month/<month>
 
-* The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "/year/2017", "2010-2015", "<2009", ">2002"). 
+Four query string parameters/paths are available in the API - `alpha2`, `name`, `year` and `months`. 
 
-* Finally, the months parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g "?months=2", "/months/6", "/months/48").
+* The 2 letter `alpha2` country code can be appended to the url as a query string parameter or as its own path (e.g ?alpha2=JP or /alpha2/JP). A single alpha-2 or list of them can be passed to the API (e.g ?alpha2=FR, DE, HU, ID, MA or /alpha2/FR,DE,HU,ID,MA). For redudancy, the 3 letter alpha-3 counterpart for each country's alpha-2 code can also be passed into the `alpha2` parameter (e.g ?alpha2=FRA, DEU, HUN, IDN, MAR or /alpha2/FRA,DEU,HUN,IDN,MAR). 
 
-* If no input parameter values specified then all ISO 3166-2 updates for all countries and years will be gotten.
+* The `name` parameter takes in a country's name as it is commonly known in English (e.g France, Moldova, Benin). A closeness function is used to get the most approximate available country from the one the user input. If one is not found then an error is raised.
 
-The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure, the hosting was switched to Vercel (https://vercel.com/).
+* The `year` parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g /year/2017, /year/2010-2015, /year/<2009, /year/>2002). 
+
+* Finally, the `months` parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g /months/2, /months/6, /months/48).
+
+* If no input parameter values specified then all ISO 3166-2 updates for all countries and years will be returned.
+
+The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. A complete diagram of the architecture is shown below. <i>Although, due to the cost of infrastructure, the hosting was switched to Vercel (https://vercel.com/).</i>
 
 The API documentation and usage with all useful commands and examples to the API is available on the [README](https://github.com/amckenna41/iso3166-updates/blob/main/iso3166-updates-api/README.md) of the iso3166-updates-api folder. 
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_arch.png" alt="gcp_arch" height="200" width="400"/>
+  <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_architecture.png" alt="gcp_arch" height="200" width="400"/>
 </p>
 
 Staying up to date
 ------------------
 The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>.
 
-The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Run microservice ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The application is built using a custom Docker container that uses the `iso3166-updates` Python software to pull all the latest updates/changes, from all ISO 3166-2 wiki's and each country's ISO website page, to check for the latest updates within a certain period e.g. the past 3-6 months. The app compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data. A Cloud Scheduler is used to periodically call the application.
+The object storing all updates, both locally (iso3166_updates/iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Run microservice ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The application is built using a custom Docker container that uses the `iso3166-updates` Python software to pull all the latest updates/changes, from all ISO 3166-2 wiki's and each country's ISO website page, to check for the latest updates within a certain period e.g. the past 3-6 months. The app compares the generated output with that of the updates JSON currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found, such that the API will have the most up-to-date data. A Cloud Scheduler is used to periodically call the application.
 
 Additionally, a GitHub Issue in the custom-built `iso3166-updates`, `iso3166-2` and `iso3166-flag-icons` repositories will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-updates`, `iso3166-2` and `iso3166-flag-icons` JSONs and repos.
 
 Ultimately, this Cloud Run microservice ensures that the software and assoicated APIs are up-to-date with the latest ISO 3166-2 information for all countries/territories/subdivisions etc.
 
 Requirements
 ------------
@@ -135,15 +146,15 @@
 git clone -b master https://github.com/amckenna41/iso3166-updates.git
 cd iso3166_updates
 python3 setup.py install
 ```
 
 Usage (iso3166-updates Python package)
 --------------------------------------
-Below are some examples of using the custom-built iso3166-updates Python package. 
+Below are some examples of using the custom-built `iso3166-updates` Python package. 
 
 **Import package:**
 ```python
 import iso3166_updates as iso
 ```
 
 **Get all listed changes/updates for all countries and years:**
@@ -162,77 +173,78 @@
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Ireland, between years 2012 and 2021:**
 ```python
 iso.updates.year("2012-2021")["IE"]
 ```
 
-**Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >=2015":**
+**Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >= 2015:**
 ```python
 iso.updates.year(">2015")["TA"]
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Yemen, with updates with year < 2010:**
 ```python
 iso.updates.year("<2010")["YE"]
 ```
-Usage get_all_iso3166_updates.py script
----------------------------------------
-Below are some examples of using the get_all_iso3166_updates.py script which is used to pull all the ISO 3166 updates
+Usage (get_all_iso3166_updates.py script)
+-----------------------------------------
+Below are some examples of using the `get_all_iso3166_updates.py` script which is used to pull all the ISO 3166 updates
 from the various data sources.
 
 **Requirements:**
 * [python][python] >= 3.8
 * [iso3166-updates][iso3166-updates] >= 1.3.0
 * [pandas][pandas] >= 1.4.3
 * [numpy][numpy] >= 1.23.2
 * [requests][requests] >= 2.28.1
 * [beautifulsoup4][beautifulsoup4] >= 4.11.1
 * [iso3166][iso3166] >= 2.1.1
 * [google-auth][google-auth] >= 2.17.3
 * [google-cloud-storage][google-cloud-storage] >= 2.8.0
 * [google-api-python-client][google-api-python-client] >= 2.86.0
 * [emoji-country-flag][emoji-country-flag] == 1.3.0
-* [selenium][seleniumn] >= 4.10.0
+* [selenium][selenium] >= 4.10.0
 * [flask][flask] >= 2.3.2
 * [gunicorn][gunicorn] >= 21.2.0
 <!-- * [webdriver-manager][webdriver-manager] >= 3.8.6 -->
 <!-- * [lxml][lxml] >=  4.9.3 -->
 
 **Input parameters to get_updates function:**
 ```python
   # -alpha2 ALPHA2, --alpha2 ALPHA2
   #                       Alpha-2 code/s of ISO 3166 countries to check for updates.
   # -export_filename EXPORT_FILENAME, --export_filename EXPORT_FILENAME
   #                       Filename for exported ISO 3166 updates for CSV and JSON files.
   # -export_folder EXPORT_FOLDER, --export_folder EXPORT_FOLDER
-  #                       Folder where to store exported ISO files.
+  #                       Folder where to store exported ISO 3166 files.
   # -export_json, --export_json
   #                       Whether to export all found updates to json.
   # -export_csv, --export_csv
   #                       Whether to export all found updates to csv files in export folder.
   # -year YEAR, --year YEAR
   #                       Selected year/years, year ranges or year to check for updates greater
-  #                       than or less than specified year
+  #                       than or less than specified year.
   # -concat_updates, --concat_updates
-  #                       Whether to concatenate updates of individual countrys into the same json file or seperate.
+  #                       Whether to concatenate updates of individual countrys into the same json file or seperate
+  #                       into seperate files
   # -verbose, --verbose
   #                       Set to 1 to print out progress of updates function, 0 will not print progress.
   # -use_selenium, --use_selenium
   #                       Gather all data for each country from its official page on the ISO website which 
   #                       requires Python Selenium and chromedriver. If False then just use country data
   #                       from its wiki page.
 ```
 **Get all the latest updates for all ISO 3166 countries**
 ```bash
 ./get_all_updates.sh 
 
 '''
---export_filename     Filename for exported JSON/CSVs files containing updates data (default="iso3166-updates.json").
---export_folder       Folder name to store exported JSON/CSVs files containing updates data (default="test-iso3166-updates).
+--export_filename     Filename for exported JSON/CSV files containing updates data (default="iso3166-updates.json").
+--export_folder       Folder name to store exported JSON/CSV files containing updates data (default="test-iso3166-updates).
 '''
 ```
 
 **Import module:**
 ```python
 import get_all_iso3166_updates as iso3166_updates
 ```
@@ -251,15 +263,15 @@
 
 **Get any listed ISO 3166-2 changes/updates for Ireland, between years 2012 and 2021, use default parameters (export to json but not csv):**
 ```python
 iso3166_updates.get_updates("IE", year="2012-2021")
 #exported files: /iso3166-updates/iso3166-updates-IE_2012-2021.json
 ```
 
-**Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >=2015, export only to CSV with filename iso3166-output":**
+**Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >= 2015, export only to CSV with filename iso3166-output":**
 ```python
 iso3166_updates.get_updates("TA", year=">2015", export_filename="iso3166-output", export_json=0, export_csv=1)
 #exported files: /iso3166-updates/iso3166-output-TA_>2015.csv
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Yemen, with updates with year < 2010, use default parameters (export to json but not csv):**
 ```python
@@ -275,17 +287,17 @@
 * Code/Subdivision change: Overall summary of change/update made.
 * Description of change in newsletter: More in-depth info about the change/update that was made.
 
 E.g. The output format of the exported <b>CSV</b> for AD (Andorra) is:
 
 | Edition/Newsletter | Date Issued | Code/Subdivision change | Description of change in newsletter |   
 |:-------------------|:------------|------------------------------------:|------------------------:|
-| Newsletter I-8     | 2007-04-17  | Subdivisions added: 7 parishes...   | Addition of the administrative subdivisions...                 | 
-| Online Browsing Platform (OBP) | 2014-11-03 | No subdivision changes listed | Update List Source |
-| Online Browsing Platform (OBP) | 2015-11-27 | No subdivision changes listed | Update List Source | 
+| Newsletter I-8.    | 2007-04-17  | Subdivisions added: 7 parishes.   | Addition of the administrative subdivisions and of their code elements.                 | 
+| Online Browsing Platform (OBP). | 2014-11-03 | | Update List Source |
+| Online Browsing Platform (OBP). | 2015-11-27 | | Update List Source | 
 
 E.g. The output format of the exported <b>JSON</b> for AD (Andorra) is:
 ```javascript
 {
   AD: [
       {
         "Code/Subdivision change": "",
@@ -310,18 +322,18 @@
 ```
 
 Directories
 -----------
 * `/docs` - documentation for `iso3166-updates` Python package.
 * `/iso3166_updates` - source code for `iso3166-updates` Python package.
 * `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the `iso3166-updates` API, including the main.py, requirements.txt and API config file.
-* `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Function for the check-for-updates function which is a periodically called Cloud Function that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date. Includes the main.py and requirements.txt files.
-* `/tests` - unit and integration tests for `iso3166-updates`.
+* `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Run microservice for the check-for-updates function which is a periodically called Cloud Run app that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date.
+* `/tests` - unit and integration tests for `iso3166-updates` software and API.
 * `get_all_iso3166_updates.py` - python module that pulls and exports all the latest ISO 3166 data from the various data sources.
-* `get_all_iso3166-updates.sh` - shell script created to call the get_all..py script to introduce some pseudo randomness required when using Python Selenium. 
+* `get_all_iso3166-updates.sh` - shell script created to call the get_all_iso3166_updates.py script to introduce some pseudo randomness required when using Python Selenium. 
 
 Issues
 ------
 Any issues, errors or bugs can be raised via the [Issues](Issues) tab in the repository.
 
 Contact
 -------
@@ -340,14 +352,15 @@
 Support
 -------
 <a href="https://www.buymeacoffee.com/amckenna41" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
 [Back to top](#TOP)
 
 [demo]: https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing
+[demo_2]: https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing
 [python]: https://www.python.org/downloads/release/python-360/
 [iso3166-updates]: https://github.com/amckenna41/iso3166-updates
 [pandas]: https://pandas.pydata.org/
 [numpy]: https://numpy.org/
 [requests]: https://requests.readthedocs.io/
 [beautifulsoup4]: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
 [google-auth]: https://cloud.google.com/python/docs/reference
```

### Comparing `iso3166-updates-1.4.0/README.md` & `iso3166-updates-1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,76 +11,87 @@
 <!-- [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-updates)](https://github.com/iso3166-updates) -->
 
 <div alt="images" style="justify-content: center; display:flex; margin-left=50px;">
   <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="200" width="500"/>
   <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="200" width="300"/>
 </div>
 
-> Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a lightweight Python software package and API; a demo of both is available [here][demo].
+> Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a lightweight Python software package and API; a demo of both is available [here][demo]. There is also a demo of the script used to pull and export all the latest updates, available [here][demo_2].
 
 Table of Contents
 -----------------
   * [Introduction](#introduction)
   * [API](#api)
   * [Staying up to date](#staying-up-to-date)
   * [Requirements](#requirements)
   * [Installation](#installation)
-  * [Usage](#usage)
+  * [Usage (iso3166-updates-Python-package)](#usage-iso3166-updates-Python-package)
+  * [Usage (get_all_iso3166_updates.py script)](#usage-get_all_iso3166_updates.py-script)
   * [Directories](#Directories)
   * [Issues](#Issues)
   * [Contact](#contact)
   * [References](#references)
 
 Introduction
 ------------
-`iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
+`iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
 
 The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations [[1]](#references). The ISO 3166-2 was first published in 1998 and as of 29 November 2022 there are 5,043 codes defined in it [[2]](#references).
 
 ### Problem Statement:
 
-The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
+The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Typically these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
 
 This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of country's ISO 3166-2 codes for free, with an easy-to-use interface and Python package and API, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
 
-<strong> The earliest date for any ISO 3166 updates is 2000-06-21, and the most recent is 2022-11-29. </strong>
+<strong> The earliest date for any ISO 3166-2 update is 2000-06-21, and the most recent is 2022-11-29. </strong>
 
 ### Intended Audience:
 
 This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (excluding 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API (https://iso3166-updates.com). 
 
 API
 ---
-An API is available that can be used to extract any applicable updates for a country via a URL. The API is available at the URL:
+An API is available that can be used to extract any applicable updates for a country via an API endpoint. The API is available at the URL:
 
 > https://www.iso3166-updates.com/api
 
-Three query string parameters are available in the API - `alpha2`, `year` and `months`. 
+The other endpoints available in the API are:
 
-* The 2 letter alpha-2 country code can be appended to the url as a query string parameter or as its own path ("?alpha2=JP" or /alpha2/JP). A single alpha-2 or list of them can be passed to the API (e.g "?alpha2="FR, DE, HU, ID, MA" or /alpha2/FR,DE,HU,ID,MA). The 3 letter alpha-3 counterpart for each country's alpha-2 code can also be passed into the `alpha2` parameter (e.g "?alpha2="FRA, DEU, HUN, IDN, MAR" or /alpha2/FRA,DEU,HUN,IDN,MAR). 
+* https://iso3166-updates.com/api/alpha2/<input_alpha2>
+* https://iso3166-updates.com/api/name/<input_name>
+* https://iso3166-updates.com/api/year/<year>
+* https://iso3166-updates.com/api/alpha2/<input_alpha2>/year/<input_year>
+* https://iso3166-updates.com/api/month/<month>
 
-* The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "/year/2017", "2010-2015", "<2009", ">2002"). 
+Four query string parameters/paths are available in the API - `alpha2`, `name`, `year` and `months`. 
 
-* Finally, the months parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g "?months=2", "/months/6", "/months/48").
+* The 2 letter `alpha2` country code can be appended to the url as a query string parameter or as its own path (e.g ?alpha2=JP or /alpha2/JP). A single alpha-2 or list of them can be passed to the API (e.g ?alpha2=FR, DE, HU, ID, MA or /alpha2/FR,DE,HU,ID,MA). For redudancy, the 3 letter alpha-3 counterpart for each country's alpha-2 code can also be passed into the `alpha2` parameter (e.g ?alpha2=FRA, DEU, HUN, IDN, MAR or /alpha2/FRA,DEU,HUN,IDN,MAR). 
 
-* If no input parameter values specified then all ISO 3166-2 updates for all countries and years will be gotten.
+* The `name` parameter takes in a country's name as it is commonly known in English (e.g France, Moldova, Benin). A closeness function is used to get the most approximate available country from the one the user input. If one is not found then an error is raised.
 
-The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure, the hosting was switched to Vercel (https://vercel.com/).
+* The `year` parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g /year/2017, /year/2010-2015, /year/<2009, /year/>2002). 
+
+* Finally, the `months` parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g /months/2, /months/6, /months/48).
+
+* If no input parameter values specified then all ISO 3166-2 updates for all countries and years will be returned.
+
+The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. A complete diagram of the architecture is shown below. <i>Although, due to the cost of infrastructure, the hosting was switched to Vercel (https://vercel.com/).</i>
 
 The API documentation and usage with all useful commands and examples to the API is available on the [README](https://github.com/amckenna41/iso3166-updates/blob/main/iso3166-updates-api/README.md) of the iso3166-updates-api folder. 
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_arch.png" alt="gcp_arch" height="200" width="400"/>
+  <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_architecture.png" alt="gcp_arch" height="200" width="400"/>
 </p>
 
 Staying up to date
 ------------------
 The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>.
 
-The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Run microservice ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The application is built using a custom Docker container that uses the `iso3166-updates` Python software to pull all the latest updates/changes, from all ISO 3166-2 wiki's and each country's ISO website page, to check for the latest updates within a certain period e.g. the past 3-6 months. The app compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data. A Cloud Scheduler is used to periodically call the application.
+The object storing all updates, both locally (iso3166_updates/iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Run microservice ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The application is built using a custom Docker container that uses the `iso3166-updates` Python software to pull all the latest updates/changes, from all ISO 3166-2 wiki's and each country's ISO website page, to check for the latest updates within a certain period e.g. the past 3-6 months. The app compares the generated output with that of the updates JSON currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found, such that the API will have the most up-to-date data. A Cloud Scheduler is used to periodically call the application.
 
 Additionally, a GitHub Issue in the custom-built `iso3166-updates`, `iso3166-2` and `iso3166-flag-icons` repositories will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-updates`, `iso3166-2` and `iso3166-flag-icons` JSONs and repos.
 
 Ultimately, this Cloud Run microservice ensures that the software and assoicated APIs are up-to-date with the latest ISO 3166-2 information for all countries/territories/subdivisions etc.
 
 Requirements
 ------------
@@ -100,15 +111,15 @@
 git clone -b master https://github.com/amckenna41/iso3166-updates.git
 cd iso3166_updates
 python3 setup.py install
 ```
 
 Usage (iso3166-updates Python package)
 --------------------------------------
-Below are some examples of using the custom-built iso3166-updates Python package. 
+Below are some examples of using the custom-built `iso3166-updates` Python package. 
 
 **Import package:**
 ```python
 import iso3166_updates as iso
 ```
 
 **Get all listed changes/updates for all countries and years:**
@@ -127,77 +138,78 @@
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Ireland, between years 2012 and 2021:**
 ```python
 iso.updates.year("2012-2021")["IE"]
 ```
 
-**Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >=2015":**
+**Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >= 2015:**
 ```python
 iso.updates.year(">2015")["TA"]
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Yemen, with updates with year < 2010:**
 ```python
 iso.updates.year("<2010")["YE"]
 ```
-Usage get_all_iso3166_updates.py script
----------------------------------------
-Below are some examples of using the get_all_iso3166_updates.py script which is used to pull all the ISO 3166 updates
+Usage (get_all_iso3166_updates.py script)
+-----------------------------------------
+Below are some examples of using the `get_all_iso3166_updates.py` script which is used to pull all the ISO 3166 updates
 from the various data sources.
 
 **Requirements:**
 * [python][python] >= 3.8
 * [iso3166-updates][iso3166-updates] >= 1.3.0
 * [pandas][pandas] >= 1.4.3
 * [numpy][numpy] >= 1.23.2
 * [requests][requests] >= 2.28.1
 * [beautifulsoup4][beautifulsoup4] >= 4.11.1
 * [iso3166][iso3166] >= 2.1.1
 * [google-auth][google-auth] >= 2.17.3
 * [google-cloud-storage][google-cloud-storage] >= 2.8.0
 * [google-api-python-client][google-api-python-client] >= 2.86.0
 * [emoji-country-flag][emoji-country-flag] == 1.3.0
-* [selenium][seleniumn] >= 4.10.0
+* [selenium][selenium] >= 4.10.0
 * [flask][flask] >= 2.3.2
 * [gunicorn][gunicorn] >= 21.2.0
 <!-- * [webdriver-manager][webdriver-manager] >= 3.8.6 -->
 <!-- * [lxml][lxml] >=  4.9.3 -->
 
 **Input parameters to get_updates function:**
 ```python
   # -alpha2 ALPHA2, --alpha2 ALPHA2
   #                       Alpha-2 code/s of ISO 3166 countries to check for updates.
   # -export_filename EXPORT_FILENAME, --export_filename EXPORT_FILENAME
   #                       Filename for exported ISO 3166 updates for CSV and JSON files.
   # -export_folder EXPORT_FOLDER, --export_folder EXPORT_FOLDER
-  #                       Folder where to store exported ISO files.
+  #                       Folder where to store exported ISO 3166 files.
   # -export_json, --export_json
   #                       Whether to export all found updates to json.
   # -export_csv, --export_csv
   #                       Whether to export all found updates to csv files in export folder.
   # -year YEAR, --year YEAR
   #                       Selected year/years, year ranges or year to check for updates greater
-  #                       than or less than specified year
+  #                       than or less than specified year.
   # -concat_updates, --concat_updates
-  #                       Whether to concatenate updates of individual countrys into the same json file or seperate.
+  #                       Whether to concatenate updates of individual countrys into the same json file or seperate
+  #                       into seperate files
   # -verbose, --verbose
   #                       Set to 1 to print out progress of updates function, 0 will not print progress.
   # -use_selenium, --use_selenium
   #                       Gather all data for each country from its official page on the ISO website which 
   #                       requires Python Selenium and chromedriver. If False then just use country data
   #                       from its wiki page.
 ```
 **Get all the latest updates for all ISO 3166 countries**
 ```bash
 ./get_all_updates.sh 
 
 '''
---export_filename     Filename for exported JSON/CSVs files containing updates data (default="iso3166-updates.json").
---export_folder       Folder name to store exported JSON/CSVs files containing updates data (default="test-iso3166-updates).
+--export_filename     Filename for exported JSON/CSV files containing updates data (default="iso3166-updates.json").
+--export_folder       Folder name to store exported JSON/CSV files containing updates data (default="test-iso3166-updates).
 '''
 ```
 
 **Import module:**
 ```python
 import get_all_iso3166_updates as iso3166_updates
 ```
@@ -216,15 +228,15 @@
 
 **Get any listed ISO 3166-2 changes/updates for Ireland, between years 2012 and 2021, use default parameters (export to json but not csv):**
 ```python
 iso3166_updates.get_updates("IE", year="2012-2021")
 #exported files: /iso3166-updates/iso3166-updates-IE_2012-2021.json
 ```
 
-**Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >=2015, export only to CSV with filename iso3166-output":**
+**Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >= 2015, export only to CSV with filename iso3166-output":**
 ```python
 iso3166_updates.get_updates("TA", year=">2015", export_filename="iso3166-output", export_json=0, export_csv=1)
 #exported files: /iso3166-updates/iso3166-output-TA_>2015.csv
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Yemen, with updates with year < 2010, use default parameters (export to json but not csv):**
 ```python
@@ -240,17 +252,17 @@
 * Code/Subdivision change: Overall summary of change/update made.
 * Description of change in newsletter: More in-depth info about the change/update that was made.
 
 E.g. The output format of the exported <b>CSV</b> for AD (Andorra) is:
 
 | Edition/Newsletter | Date Issued | Code/Subdivision change | Description of change in newsletter |   
 |:-------------------|:------------|------------------------------------:|------------------------:|
-| Newsletter I-8     | 2007-04-17  | Subdivisions added: 7 parishes...   | Addition of the administrative subdivisions...                 | 
-| Online Browsing Platform (OBP) | 2014-11-03 | No subdivision changes listed | Update List Source |
-| Online Browsing Platform (OBP) | 2015-11-27 | No subdivision changes listed | Update List Source | 
+| Newsletter I-8.    | 2007-04-17  | Subdivisions added: 7 parishes.   | Addition of the administrative subdivisions and of their code elements.                 | 
+| Online Browsing Platform (OBP). | 2014-11-03 | | Update List Source |
+| Online Browsing Platform (OBP). | 2015-11-27 | | Update List Source | 
 
 E.g. The output format of the exported <b>JSON</b> for AD (Andorra) is:
 ```javascript
 {
   AD: [
       {
         "Code/Subdivision change": "",
@@ -275,18 +287,18 @@
 ```
 
 Directories
 -----------
 * `/docs` - documentation for `iso3166-updates` Python package.
 * `/iso3166_updates` - source code for `iso3166-updates` Python package.
 * `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the `iso3166-updates` API, including the main.py, requirements.txt and API config file.
-* `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Function for the check-for-updates function which is a periodically called Cloud Function that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date. Includes the main.py and requirements.txt files.
-* `/tests` - unit and integration tests for `iso3166-updates`.
+* `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Run microservice for the check-for-updates function which is a periodically called Cloud Run app that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date.
+* `/tests` - unit and integration tests for `iso3166-updates` software and API.
 * `get_all_iso3166_updates.py` - python module that pulls and exports all the latest ISO 3166 data from the various data sources.
-* `get_all_iso3166-updates.sh` - shell script created to call the get_all..py script to introduce some pseudo randomness required when using Python Selenium. 
+* `get_all_iso3166-updates.sh` - shell script created to call the get_all_iso3166_updates.py script to introduce some pseudo randomness required when using Python Selenium. 
 
 Issues
 ------
 Any issues, errors or bugs can be raised via the [Issues](Issues) tab in the repository.
 
 Contact
 -------
@@ -305,14 +317,15 @@
 Support
 -------
 <a href="https://www.buymeacoffee.com/amckenna41" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
 [Back to top](#TOP)
 
 [demo]: https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing
+[demo_2]: https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing
 [python]: https://www.python.org/downloads/release/python-360/
 [iso3166-updates]: https://github.com/amckenna41/iso3166-updates
 [pandas]: https://pandas.pydata.org/
 [numpy]: https://numpy.org/
 [requests]: https://requests.readthedocs.io/
 [beautifulsoup4]: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
 [google-auth]: https://cloud.google.com/python/docs/reference
```

### Comparing `iso3166-updates-1.4.0/iso3166_updates/__init__.py` & `iso3166-updates-1.4.1/iso3166_updates/__init__.py`

 * *Files identical despite different names*

### Comparing `iso3166-updates-1.4.0/iso3166_updates/iso3166_updates.py` & `iso3166-updates-1.4.1/iso3166_updates/iso3166_updates.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,16 @@
         self.iso3166_updates_json_filename = "iso3166-updates.json"
         
         #get module path
         self.iso3166_updates_module_path = os.path.dirname(os.path.abspath(sys.modules[self.__module__].__file__))
         
         #raise error if iso3166-upates json doesnt exist in folder
         if not (os.path.isfile(os.path.join(self.iso3166_updates_module_path, self.iso3166_updates_json_filename))):
-            raise OSError("Issue finding iso3166-updates.json in dir.")
+            raise OSError("Issue finding iso3166-updates.json in dir: {}".format(
+                os.path.join(self.iso3166_updates_module_path, self.iso3166_updates_json_filename)))
 
         #open iso3166-updates json file and load it into class variable
         with open(os.path.join(self.iso3166_updates_module_path, self.iso3166_updates_json_filename)) as iso3166_updates_json:
             self.all = json.load(iso3166_updates_json)
 
         #get list of all countries by 2 letter alpha3 code
         self.alpha2 = sorted(list(iso3166.countries_by_alpha2.keys()))
```

### Comparing `iso3166-updates-1.4.0/iso3166_updates.egg-info/PKG-INFO` & `iso3166-updates-1.4.1/iso3166_updates.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: iso3166-updates
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 Home-page: https://github.com/amckenna41/iso3166-updates
 Author: AJ McKenna, https://github.com/amckenna41
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
-Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,csv,iso3166-2,iso3166-1,alpha-2,alpha-3
+Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,csv,iso3166-2,iso3166-1,alpha-2,alpha-3,selenium,chromedriver
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
@@ -46,76 +46,87 @@
 <!-- [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-updates)](https://github.com/iso3166-updates) -->
 
 <div alt="images" style="justify-content: center; display:flex; margin-left=50px;">
   <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="200" width="500"/>
   <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="200" width="300"/>
 </div>
 
-> Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a lightweight Python software package and API; a demo of both is available [here][demo].
+> Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a lightweight Python software package and API; a demo of both is available [here][demo]. There is also a demo of the script used to pull and export all the latest updates, available [here][demo_2].
 
 Table of Contents
 -----------------
   * [Introduction](#introduction)
   * [API](#api)
   * [Staying up to date](#staying-up-to-date)
   * [Requirements](#requirements)
   * [Installation](#installation)
-  * [Usage](#usage)
+  * [Usage (iso3166-updates-Python-package)](#usage-iso3166-updates-Python-package)
+  * [Usage (get_all_iso3166_updates.py script)](#usage-get_all_iso3166_updates.py-script)
   * [Directories](#Directories)
   * [Issues](#Issues)
   * [Contact](#contact)
   * [References](#references)
 
 Introduction
 ------------
-`iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
+`iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
 
 The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations [[1]](#references). The ISO 3166-2 was first published in 1998 and as of 29 November 2022 there are 5,043 codes defined in it [[2]](#references).
 
 ### Problem Statement:
 
-The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
+The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Typically these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
 
 This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of country's ISO 3166-2 codes for free, with an easy-to-use interface and Python package and API, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
 
-<strong> The earliest date for any ISO 3166 updates is 2000-06-21, and the most recent is 2022-11-29. </strong>
+<strong> The earliest date for any ISO 3166-2 update is 2000-06-21, and the most recent is 2022-11-29. </strong>
 
 ### Intended Audience:
 
 This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (excluding 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API (https://iso3166-updates.com). 
 
 API
 ---
-An API is available that can be used to extract any applicable updates for a country via a URL. The API is available at the URL:
+An API is available that can be used to extract any applicable updates for a country via an API endpoint. The API is available at the URL:
 
 > https://www.iso3166-updates.com/api
 
-Three query string parameters are available in the API - `alpha2`, `year` and `months`. 
+The other endpoints available in the API are:
 
-* The 2 letter alpha-2 country code can be appended to the url as a query string parameter or as its own path ("?alpha2=JP" or /alpha2/JP). A single alpha-2 or list of them can be passed to the API (e.g "?alpha2="FR, DE, HU, ID, MA" or /alpha2/FR,DE,HU,ID,MA). The 3 letter alpha-3 counterpart for each country's alpha-2 code can also be passed into the `alpha2` parameter (e.g "?alpha2="FRA, DEU, HUN, IDN, MAR" or /alpha2/FRA,DEU,HUN,IDN,MAR). 
+* https://iso3166-updates.com/api/alpha2/<input_alpha2>
+* https://iso3166-updates.com/api/name/<input_name>
+* https://iso3166-updates.com/api/year/<year>
+* https://iso3166-updates.com/api/alpha2/<input_alpha2>/year/<input_year>
+* https://iso3166-updates.com/api/month/<month>
 
-* The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "/year/2017", "2010-2015", "<2009", ">2002"). 
+Four query string parameters/paths are available in the API - `alpha2`, `name`, `year` and `months`. 
 
-* Finally, the months parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g "?months=2", "/months/6", "/months/48").
+* The 2 letter `alpha2` country code can be appended to the url as a query string parameter or as its own path (e.g ?alpha2=JP or /alpha2/JP). A single alpha-2 or list of them can be passed to the API (e.g ?alpha2=FR, DE, HU, ID, MA or /alpha2/FR,DE,HU,ID,MA). For redudancy, the 3 letter alpha-3 counterpart for each country's alpha-2 code can also be passed into the `alpha2` parameter (e.g ?alpha2=FRA, DEU, HUN, IDN, MAR or /alpha2/FRA,DEU,HUN,IDN,MAR). 
 
-* If no input parameter values specified then all ISO 3166-2 updates for all countries and years will be gotten.
+* The `name` parameter takes in a country's name as it is commonly known in English (e.g France, Moldova, Benin). A closeness function is used to get the most approximate available country from the one the user input. If one is not found then an error is raised.
 
-The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure, the hosting was switched to Vercel (https://vercel.com/).
+* The `year` parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g /year/2017, /year/2010-2015, /year/<2009, /year/>2002). 
+
+* Finally, the `months` parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g /months/2, /months/6, /months/48).
+
+* If no input parameter values specified then all ISO 3166-2 updates for all countries and years will be returned.
+
+The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. A complete diagram of the architecture is shown below. <i>Although, due to the cost of infrastructure, the hosting was switched to Vercel (https://vercel.com/).</i>
 
 The API documentation and usage with all useful commands and examples to the API is available on the [README](https://github.com/amckenna41/iso3166-updates/blob/main/iso3166-updates-api/README.md) of the iso3166-updates-api folder. 
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_arch.png" alt="gcp_arch" height="200" width="400"/>
+  <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_architecture.png" alt="gcp_arch" height="200" width="400"/>
 </p>
 
 Staying up to date
 ------------------
 The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>.
 
-The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Run microservice ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The application is built using a custom Docker container that uses the `iso3166-updates` Python software to pull all the latest updates/changes, from all ISO 3166-2 wiki's and each country's ISO website page, to check for the latest updates within a certain period e.g. the past 3-6 months. The app compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data. A Cloud Scheduler is used to periodically call the application.
+The object storing all updates, both locally (iso3166_updates/iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Run microservice ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The application is built using a custom Docker container that uses the `iso3166-updates` Python software to pull all the latest updates/changes, from all ISO 3166-2 wiki's and each country's ISO website page, to check for the latest updates within a certain period e.g. the past 3-6 months. The app compares the generated output with that of the updates JSON currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found, such that the API will have the most up-to-date data. A Cloud Scheduler is used to periodically call the application.
 
 Additionally, a GitHub Issue in the custom-built `iso3166-updates`, `iso3166-2` and `iso3166-flag-icons` repositories will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-updates`, `iso3166-2` and `iso3166-flag-icons` JSONs and repos.
 
 Ultimately, this Cloud Run microservice ensures that the software and assoicated APIs are up-to-date with the latest ISO 3166-2 information for all countries/territories/subdivisions etc.
 
 Requirements
 ------------
@@ -135,15 +146,15 @@
 git clone -b master https://github.com/amckenna41/iso3166-updates.git
 cd iso3166_updates
 python3 setup.py install
 ```
 
 Usage (iso3166-updates Python package)
 --------------------------------------
-Below are some examples of using the custom-built iso3166-updates Python package. 
+Below are some examples of using the custom-built `iso3166-updates` Python package. 
 
 **Import package:**
 ```python
 import iso3166_updates as iso
 ```
 
 **Get all listed changes/updates for all countries and years:**
@@ -162,77 +173,78 @@
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Ireland, between years 2012 and 2021:**
 ```python
 iso.updates.year("2012-2021")["IE"]
 ```
 
-**Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >=2015":**
+**Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >= 2015:**
 ```python
 iso.updates.year(">2015")["TA"]
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Yemen, with updates with year < 2010:**
 ```python
 iso.updates.year("<2010")["YE"]
 ```
-Usage get_all_iso3166_updates.py script
----------------------------------------
-Below are some examples of using the get_all_iso3166_updates.py script which is used to pull all the ISO 3166 updates
+Usage (get_all_iso3166_updates.py script)
+-----------------------------------------
+Below are some examples of using the `get_all_iso3166_updates.py` script which is used to pull all the ISO 3166 updates
 from the various data sources.
 
 **Requirements:**
 * [python][python] >= 3.8
 * [iso3166-updates][iso3166-updates] >= 1.3.0
 * [pandas][pandas] >= 1.4.3
 * [numpy][numpy] >= 1.23.2
 * [requests][requests] >= 2.28.1
 * [beautifulsoup4][beautifulsoup4] >= 4.11.1
 * [iso3166][iso3166] >= 2.1.1
 * [google-auth][google-auth] >= 2.17.3
 * [google-cloud-storage][google-cloud-storage] >= 2.8.0
 * [google-api-python-client][google-api-python-client] >= 2.86.0
 * [emoji-country-flag][emoji-country-flag] == 1.3.0
-* [selenium][seleniumn] >= 4.10.0
+* [selenium][selenium] >= 4.10.0
 * [flask][flask] >= 2.3.2
 * [gunicorn][gunicorn] >= 21.2.0
 <!-- * [webdriver-manager][webdriver-manager] >= 3.8.6 -->
 <!-- * [lxml][lxml] >=  4.9.3 -->
 
 **Input parameters to get_updates function:**
 ```python
   # -alpha2 ALPHA2, --alpha2 ALPHA2
   #                       Alpha-2 code/s of ISO 3166 countries to check for updates.
   # -export_filename EXPORT_FILENAME, --export_filename EXPORT_FILENAME
   #                       Filename for exported ISO 3166 updates for CSV and JSON files.
   # -export_folder EXPORT_FOLDER, --export_folder EXPORT_FOLDER
-  #                       Folder where to store exported ISO files.
+  #                       Folder where to store exported ISO 3166 files.
   # -export_json, --export_json
   #                       Whether to export all found updates to json.
   # -export_csv, --export_csv
   #                       Whether to export all found updates to csv files in export folder.
   # -year YEAR, --year YEAR
   #                       Selected year/years, year ranges or year to check for updates greater
-  #                       than or less than specified year
+  #                       than or less than specified year.
   # -concat_updates, --concat_updates
-  #                       Whether to concatenate updates of individual countrys into the same json file or seperate.
+  #                       Whether to concatenate updates of individual countrys into the same json file or seperate
+  #                       into seperate files
   # -verbose, --verbose
   #                       Set to 1 to print out progress of updates function, 0 will not print progress.
   # -use_selenium, --use_selenium
   #                       Gather all data for each country from its official page on the ISO website which 
   #                       requires Python Selenium and chromedriver. If False then just use country data
   #                       from its wiki page.
 ```
 **Get all the latest updates for all ISO 3166 countries**
 ```bash
 ./get_all_updates.sh 
 
 '''
---export_filename     Filename for exported JSON/CSVs files containing updates data (default="iso3166-updates.json").
---export_folder       Folder name to store exported JSON/CSVs files containing updates data (default="test-iso3166-updates).
+--export_filename     Filename for exported JSON/CSV files containing updates data (default="iso3166-updates.json").
+--export_folder       Folder name to store exported JSON/CSV files containing updates data (default="test-iso3166-updates).
 '''
 ```
 
 **Import module:**
 ```python
 import get_all_iso3166_updates as iso3166_updates
 ```
@@ -251,15 +263,15 @@
 
 **Get any listed ISO 3166-2 changes/updates for Ireland, between years 2012 and 2021, use default parameters (export to json but not csv):**
 ```python
 iso3166_updates.get_updates("IE", year="2012-2021")
 #exported files: /iso3166-updates/iso3166-updates-IE_2012-2021.json
 ```
 
-**Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >=2015, export only to CSV with filename iso3166-output":**
+**Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >= 2015, export only to CSV with filename iso3166-output":**
 ```python
 iso3166_updates.get_updates("TA", year=">2015", export_filename="iso3166-output", export_json=0, export_csv=1)
 #exported files: /iso3166-updates/iso3166-output-TA_>2015.csv
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Yemen, with updates with year < 2010, use default parameters (export to json but not csv):**
 ```python
@@ -275,17 +287,17 @@
 * Code/Subdivision change: Overall summary of change/update made.
 * Description of change in newsletter: More in-depth info about the change/update that was made.
 
 E.g. The output format of the exported <b>CSV</b> for AD (Andorra) is:
 
 | Edition/Newsletter | Date Issued | Code/Subdivision change | Description of change in newsletter |   
 |:-------------------|:------------|------------------------------------:|------------------------:|
-| Newsletter I-8     | 2007-04-17  | Subdivisions added: 7 parishes...   | Addition of the administrative subdivisions...                 | 
-| Online Browsing Platform (OBP) | 2014-11-03 | No subdivision changes listed | Update List Source |
-| Online Browsing Platform (OBP) | 2015-11-27 | No subdivision changes listed | Update List Source | 
+| Newsletter I-8.    | 2007-04-17  | Subdivisions added: 7 parishes.   | Addition of the administrative subdivisions and of their code elements.                 | 
+| Online Browsing Platform (OBP). | 2014-11-03 | | Update List Source |
+| Online Browsing Platform (OBP). | 2015-11-27 | | Update List Source | 
 
 E.g. The output format of the exported <b>JSON</b> for AD (Andorra) is:
 ```javascript
 {
   AD: [
       {
         "Code/Subdivision change": "",
@@ -310,18 +322,18 @@
 ```
 
 Directories
 -----------
 * `/docs` - documentation for `iso3166-updates` Python package.
 * `/iso3166_updates` - source code for `iso3166-updates` Python package.
 * `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the `iso3166-updates` API, including the main.py, requirements.txt and API config file.
-* `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Function for the check-for-updates function which is a periodically called Cloud Function that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date. Includes the main.py and requirements.txt files.
-* `/tests` - unit and integration tests for `iso3166-updates`.
+* `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Run microservice for the check-for-updates function which is a periodically called Cloud Run app that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date.
+* `/tests` - unit and integration tests for `iso3166-updates` software and API.
 * `get_all_iso3166_updates.py` - python module that pulls and exports all the latest ISO 3166 data from the various data sources.
-* `get_all_iso3166-updates.sh` - shell script created to call the get_all..py script to introduce some pseudo randomness required when using Python Selenium. 
+* `get_all_iso3166-updates.sh` - shell script created to call the get_all_iso3166_updates.py script to introduce some pseudo randomness required when using Python Selenium. 
 
 Issues
 ------
 Any issues, errors or bugs can be raised via the [Issues](Issues) tab in the repository.
 
 Contact
 -------
@@ -340,14 +352,15 @@
 Support
 -------
 <a href="https://www.buymeacoffee.com/amckenna41" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
 [Back to top](#TOP)
 
 [demo]: https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing
+[demo_2]: https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing
 [python]: https://www.python.org/downloads/release/python-360/
 [iso3166-updates]: https://github.com/amckenna41/iso3166-updates
 [pandas]: https://pandas.pydata.org/
 [numpy]: https://numpy.org/
 [requests]: https://requests.readthedocs.io/
 [beautifulsoup4]: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
 [google-auth]: https://cloud.google.com/python/docs/reference
```

### Comparing `iso3166-updates-1.4.0/setup.cfg` & `iso3166-updates-1.4.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iso3166-updates
-version = 1.4.0
+version = 1.4.1
 description = A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = AJ McKenna
 author_email = amckenna41@qub.ac.uk
 url = https://github.com/amckenna41/iso3166-updates
 download_url = https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
```

### Comparing `iso3166-updates-1.4.0/setup.py` & `iso3166-updates-1.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 import pathlib
 from setuptools import setup, find_packages
 import sys
 
 #software metadata
 __name__ = 'iso3166-updates'
-__version__ = "1.4.0"
+__version__ = "1.4.1"
 __description__ = "A Python package that pulls the latest updates & changes to all ISO3166 listed countries."
 __author__ = 'AJ McKenna, https://github.com/amckenna41'
 __authorEmail__ = 'amckenna41@qub.ac.uk'
 __license__ = 'MIT'
 __url__ = 'https://github.com/amckenna41/iso3166-updates'
 __download_url__ = "https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip"
 __status__ = 'Development'
 __maintainer__ = "AJ McKenna"
 __keywords__ = ["iso", "iso3166", "beautifulsoup", "python", "pypi", "countries", "country codes", "csv", \
-            "iso3166-2", "iso3166-1", "alpha-2", "alpha-3"]
+            "iso3166-2", "iso3166-1", "alpha-2", "alpha-3", "selenium", "chromedriver"]
 __test_suite__ = "tests"
  
 #ensure python version is greater than 3
 if (sys.version_info[0] < 3):
     sys.exit('Python 3 is the minimum version requirement.')
 
 #get path to README file
```

