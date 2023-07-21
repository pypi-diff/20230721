# Comparing `tmp/geocode-adi-2.0.0.tar.gz` & `tmp/geocode-adi-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\geocode-adi-2.0.0.tar", last modified: Tue Feb  9 09:26:03 2021, max compression
+gzip compressed data, was "geocode-adi-2.1.0.tar", last modified: Fri Jul 21 05:16:31 2023, max compression
```

## Comparing `geocode-adi-2.0.0.tar` & `geocode-adi-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2021-02-09 09:26:03.077931 geocode-adi-2.0.0/
--rw-rw-rw-   0        0        0       33 2021-02-09 08:45:34.000000 geocode-adi-2.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5990 2021-02-09 09:26:03.075935 geocode-adi-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4816 2021-02-09 09:25:14.000000 geocode-adi-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2021-02-09 09:26:02.974901 geocode-adi-2.0.0/geocode-adi/
--rw-rw-rw-   0        0        0        0 2021-02-08 14:21:57.000000 geocode-adi-2.0.0/geocode-adi/__init__.py
--rw-rw-rw-   0        0        0     2156 2021-02-09 07:44:10.000000 geocode-adi-2.0.0/geocode-adi/__main__.py
--rw-rw-rw-   0        0        0    35301 2021-02-09 08:53:17.000000 geocode-adi-2.0.0/geocode-adi/geocodeadi.py
-drwxrwxrwx   0        0        0        0 2021-02-09 09:26:02.998693 geocode-adi-2.0.0/geocode-adi/resources/
--rw-rw-rw-   0        0        0  4254762 2021-02-08 14:21:57.000000 geocode-adi-2.0.0/geocode-adi/resources/BlockGroupToADI.feather
--rw-rw-rw-   0        0        0        0 2021-02-08 14:21:57.000000 geocode-adi-2.0.0/geocode-adi/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2021-02-09 09:26:03.073177 geocode-adi-2.0.0/geocode_adi.egg-info/
--rw-rw-rw-   0        0        0     5990 2021-02-09 09:26:02.000000 geocode-adi-2.0.0/geocode_adi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2021-02-09 09:26:02.000000 geocode-adi-2.0.0/geocode_adi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-02-09 09:26:02.000000 geocode-adi-2.0.0/geocode_adi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2021-02-09 09:26:02.000000 geocode-adi-2.0.0/geocode_adi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2021-02-09 09:26:02.000000 geocode-adi-2.0.0/geocode_adi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-02-09 09:26:03.079007 geocode-adi-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1045 2021-02-09 09:18:00.000000 geocode-adi-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 05:16:31.639588 geocode-adi-2.1.0/
+-rw-rw-rw-   0        0        0     1089 2023-07-20 20:05:55.000000 geocode-adi-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-07-20 20:05:55.000000 geocode-adi-2.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5472 2023-07-21 05:16:31.639588 geocode-adi-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5014 2023-07-21 03:38:54.000000 geocode-adi-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 05:16:31.603252 geocode-adi-2.1.0/geocode-adi/
+-rw-rw-rw-   0        0        0        0 2023-07-20 20:05:55.000000 geocode-adi-2.1.0/geocode-adi/__init__.py
+-rw-rw-rw-   0        0        0     2156 2023-07-20 20:05:55.000000 geocode-adi-2.1.0/geocode-adi/__main__.py
+-rw-rw-rw-   0        0        0    35735 2023-07-21 02:42:39.000000 geocode-adi-2.1.0/geocode-adi/geocodeadi.py
+drwxrwxrwx   0        0        0        0 2023-07-21 05:16:31.626719 geocode-adi-2.1.0/geocode-adi/resources/
+-rw-rw-rw-   0        0        0  9849810 2023-07-21 00:51:50.000000 geocode-adi-2.1.0/geocode-adi/resources/BlockGroupToADI.feather
+-rw-rw-rw-   0        0        0        0 2023-07-20 20:05:55.000000 geocode-adi-2.1.0/geocode-adi/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 05:16:31.636311 geocode-adi-2.1.0/geocode_adi.egg-info/
+-rw-rw-rw-   0        0        0     5472 2023-07-21 05:16:31.000000 geocode-adi-2.1.0/geocode_adi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-07-21 05:16:31.000000 geocode-adi-2.1.0/geocode_adi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 05:16:31.000000 geocode-adi-2.1.0/geocode_adi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-07-21 05:16:31.000000 geocode-adi-2.1.0/geocode_adi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-21 05:16:31.000000 geocode-adi-2.1.0/geocode_adi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 05:16:31.639588 geocode-adi-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1041 2023-07-21 05:05:51.000000 geocode-adi-2.1.0/setup.py
```

### Comparing `geocode-adi-2.0.0/PKG-INFO` & `geocode-adi-2.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,97 +1,101 @@
 Metadata-Version: 2.1
 Name: geocode-adi
-Version: 2.0.0
+Version: 2.1.0
 Summary: Map addresses to Area Deprivation Index through U.S. Census Block Groups
 Home-page: https://github.com/AyushDoshi/geocode-adi
 Author: Ayush Doshi
 Author-email: ayushdoshi1@gmail.com
 License: MIT
-Description: # geocode-adi
-        
-        ## What is it?
-        
-        **geocode-adi** is a Python package that allows for the mapping of address information to Gopal K. Singh's 
-        [**Area Deprivation Index (ADI)**][adi-paper] at the U.S. Census Block Group level, which was calculated by the 
-        [**Applied Population Lab at UW-Madison**][pop-lab] and made available on 
-        [**UW-Madison's Neighborhood Atlas**][neigh-atlas].
-        
-        ## Where to get it?
-        The source code is currently hosted on GitHub at:
-        https://github.com/AyushDoshi/geocode-adi.
-        
-        Binary installers for released versions are available at the 
-        [Python Package Index (PyPI)][geocode-adi-pypi].
-        ```
-        pip install geocode-adi
-        ```
-        
-        ### Dependencies
-        - [Pandas](https://pandas.pydata.org/) - Required for reading in address data, manipulating it, and exporting it back 
-        out.
-        - [Numpy](https://www.numpy.org) - Required for chunking address data and adding "Not A Number" values.
-        - [Requests](https://requests.readthedocs.io) - Required for making GET requests to Google.
-        - [Geopy](https://geopy.readthedocs.io) - Required for making geocoding API calls to Nominatim/OpenStreetMaps.
-        - [Census Geocode](https://github.com/fitnr/censusgeocode) - Required for making geocoding API calls to the 
-        [U.S. Census Geocoder][us-geocoder].
-        - [tqdm](https://tqdm.github.io/) - Required for making progress bars.
-        
-        If **geocode-adi** is installed using a binary installer, such as through [PyPI][geocode-adi-pypi], the required 
-        dependencies should automatically be installed.
-        
-        ## How to use it?
-        This package is meant to be run as a script in the command-line/terminal, although the individual functions found in the
-        [*geocodeadi.py*](geocode-adi/geocodeadi.py) file may be imported as a module.
-        
-        The script takes in a comma-delimited file, such as a .CSV, that contains the address information. Specifically, the 
-        file must contain at least 4 columns: *'Address'*, *'City'*, *'State'*, *'ZIP Code'*. These columns must also be 
-        labeled as such. The *'Address'* column must contain at least the street number and name. Other information, such as 
-        apartment or suite number, is optional. An example of a correctly formatted file of addresses is the
-        [*AddressSample.csv*](AddressSample.csv) file in the repository.
-        
-        Once installed, **geocode-adi** can be simply called in the command-line/terminal in the following way:
-        ```
-        python -m geocode-adi [PATH_TO_ADDRESS_FILE]
-        ```
-        For example, using the file [*AddressSample.csv*](AddressSample.csv):
-        ```
-        python -m geocode-adi AddressSample.csv
-        ```
-        ## How does it work?
-        
-        **geocode-adi** works in mapping addresses to ADI in 4 overarching steps:
-        1. It imports the addresses into a Pandas DataFrame.
-        2. It converts the addresses into U.S. Census Block Groups, which itself occurs in 6 steps:
-            1. It filters out the majority of P.O. and Route boxes from the address list and puts them to the side.
-            2. Then it does a first-pass conversion of the filtered addresses directly to U.S. Census Block Groups using the 
-            [U.S. Census Geocoder][us-geocoder].
-            3. The addresses that failed to be directly converted to U.S. Census Block Groups are then tried to be converted to 
-            coordinates using Google.
-            4. The addresses that failed at being converted to coordinates by Google are then tried to be converted to 
-            coordinates using [Nominatim/OpenStreetMaps](https://nominatim.org/).
-            5. The addresses that were successfully converted to coordinates, either by Google or Nominatim/OpenStreetMaps, are 
-            then tried at a second-pass conversion to U.S. Census Block Groups with the U.S. Census Geocoder again, but this 
-            time using the coordinates instead of the addresses directly.
-            6. Addresses that were successfully converted to U.S. Census Blocks, either in the first or second pass, are then 
-            combined. Addresses that failed to be converted, due to being a PO/Route Box, failing to be converted to 
-            coordinates, or failing to have their coordinates converted to U.S. Census Block Groups, are also combined.
-        3. Addresses that were successfully converted to U.S. Census Block Groups then have an ADI value mapped to it based on 
-        its U.S. Census Block Group.
-        4. The addresses that were mapped to ADI values through their U.S. Census Block Group are exported to a .CSV file 
-        labeled ***successful.csv***. Addresses that failed to be converted to Census Block Groups are exported to a .CSV file 
-        labeled ***failed.csv***.
-        
-        ## License
-        [MIT](LICENSE)
-        
-        [adi-paper]: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1447923/
-        [neigh-atlas]: https://www.neighborhoodatlas.medicine.wisc.edu/
-        [geocode-adi-pypi]: https://pypi.org/project/geocode-adi
-        [pop-lab]: https://apl.wisc.edu/
-        [us-geocoder]: https://geocoding.geo.census.gov/
-        [geocode-adi-pypi]: https://pypi.org/project/geocode-adi/
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# geocode-adi
+
+## What is it?
+
+**geocode-adi** is a Python package that allows for the mapping of address information to Gopal K. Singh's 
+[**Area Deprivation Index (ADI)**][adi-paper] at the U.S. Census Block Group level, which was calculated by the 
+[**Applied Population Lab at UW-Madison**][pop-lab] and made available on 
+[**UW-Madison's Neighborhood Atlas**][neigh-atlas]. For a given address, it will map to the ADI National
+Percentiles and State Deciles for the following years/versions:
+- 2021
+- 2020
+- 2015
+
+## Where to get it?
+The source code is currently hosted on GitHub at:
+https://github.com/AyushDoshi/geocode-adi.
+
+Binary installers for released versions are available at the 
+[Python Package Index (PyPI)][geocode-adi-pypi]. To run the script, Python 3.6 or greater is required.
+```
+pip install geocode-adi
+```
+
+### Dependencies
+- [Pandas](https://pandas.pydata.org/) - Required for reading in address data, manipulating it, and exporting it back 
+out.
+- [Numpy](https://www.numpy.org) - Required for chunking address data and adding "Not A Number" values.
+- [Requests](https://requests.readthedocs.io) - Required for making GET requests to Google.
+- [Geopy](https://geopy.readthedocs.io) - Required for making geocoding API calls to Nominatim/OpenStreetMaps.
+- [Census Geocode](https://github.com/fitnr/censusgeocode) - Required for making geocoding API calls to the 
+[U.S. Census Geocoder][us-geocoder].
+- [tqdm](https://tqdm.github.io/) - Required for making progress bars.
+
+If **geocode-adi** is installed using a binary installer, such as through [PyPI][geocode-adi-pypi], the required 
+dependencies should automatically be installed.
+
+## How to use it?
+This package is meant to be run as a script in the command-line/terminal, although the individual functions found in the
+[*geocodeadi.py*](geocode-adi/geocodeadi.py) file may be imported as a module.
+
+The script takes in a comma-delimited file, such as a .CSV, that contains the address information. Specifically, the 
+file must contain at least 4 columns: *'Address'*, *'City'*, *'State'*, *'ZIP Code'*. These columns must also be 
+labeled as such. The *'Address'* column must contain at least the street number and name. Other information, such as 
+apartment or suite number, is optional. An example of a correctly formatted file of addresses is the
+[*AddressSample.csv*](AddressSample.csv) file in the repository.
+
+Once installed, **geocode-adi** can be simply called in the command-line/terminal in the following way:
+```
+python -m geocode-adi [PATH_TO_ADDRESS_FILE]
+```
+For example, using the file [*AddressSample.csv*](AddressSample.csv):
+```
+python -m geocode-adi AddressSample.csv
+```
+## How does it work?
+
+**geocode-adi** works in mapping addresses to ADI in 4 overarching steps:
+1. It imports the addresses into a Pandas DataFrame.
+2. It converts the addresses into U.S. Census Block Groups, which itself occurs in 6 steps:
+    1. It filters out the majority of P.O. and Route boxes from the address list and puts them to the side.
+    2. Then it does a first-pass conversion of the filtered addresses directly to U.S. Census Block Groups using the 
+    [U.S. Census Geocoder][us-geocoder].
+    3. The addresses that failed to be directly converted to U.S. Census Block Groups are then tried to be converted to 
+    coordinates using Google.
+    4. The addresses that failed at being converted to coordinates by Google are then tried to be converted to 
+    coordinates using [Nominatim/OpenStreetMaps](https://nominatim.org/).
+    5. The addresses that were successfully converted to coordinates, either by Google or Nominatim/OpenStreetMaps, are 
+    then tried at a second-pass conversion to U.S. Census Block Groups with the U.S. Census Geocoder again, but this 
+    time using the coordinates instead of the addresses directly.
+    6. Addresses that were successfully converted to U.S. Census Blocks, either in the first or second pass, are then 
+    combined. Addresses that failed to be converted, due to being a PO/Route Box, failing to be converted to 
+    coordinates, or failing to have their coordinates converted to U.S. Census Block Groups, are also combined.
+3. Addresses that were successfully converted to U.S. Census Block Groups then have an ADI value mapped to it based on 
+its U.S. Census Block Group.
+4. The addresses that were mapped to ADI values through their U.S. Census Block Group are exported to a .CSV file 
+labeled ***successful.csv***. Addresses that failed to be converted to Census Block Groups are exported to a .CSV file 
+labeled ***failed.csv***.
+
+## License
+[MIT](LICENSE)
+
+[adi-paper]: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1447923/
+[neigh-atlas]: https://www.neighborhoodatlas.medicine.wisc.edu/
+[geocode-adi-pypi]: https://pypi.org/project/geocode-adi
+[pop-lab]: https://apl.wisc.edu/
+[us-geocoder]: https://geocoding.geo.census.gov/
+[geocode-adi-pypi]: https://pypi.org/project/geocode-adi/
```

### Comparing `geocode-adi-2.0.0/README.md` & `geocode-adi-2.1.0/geocode_adi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,40 @@
+Metadata-Version: 2.1
+Name: geocode-adi
+Version: 2.1.0
+Summary: Map addresses to Area Deprivation Index through U.S. Census Block Groups
+Home-page: https://github.com/AyushDoshi/geocode-adi
+Author: Ayush Doshi
+Author-email: ayushdoshi1@gmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # geocode-adi
 
 ## What is it?
 
 **geocode-adi** is a Python package that allows for the mapping of address information to Gopal K. Singh's 
 [**Area Deprivation Index (ADI)**][adi-paper] at the U.S. Census Block Group level, which was calculated by the 
 [**Applied Population Lab at UW-Madison**][pop-lab] and made available on 
-[**UW-Madison's Neighborhood Atlas**][neigh-atlas].
+[**UW-Madison's Neighborhood Atlas**][neigh-atlas]. For a given address, it will map to the ADI National
+Percentiles and State Deciles for the following years/versions:
+- 2021
+- 2020
+- 2015
 
 ## Where to get it?
 The source code is currently hosted on GitHub at:
 https://github.com/AyushDoshi/geocode-adi.
 
 Binary installers for released versions are available at the 
-[Python Package Index (PyPI)][geocode-adi-pypi].
+[Python Package Index (PyPI)][geocode-adi-pypi]. To run the script, Python 3.6 or greater is required.
 ```
 pip install geocode-adi
 ```
 
 ### Dependencies
 - [Pandas](https://pandas.pydata.org/) - Required for reading in address data, manipulating it, and exporting it back 
 out.
@@ -76,8 +94,8 @@
 [MIT](LICENSE)
 
 [adi-paper]: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1447923/
 [neigh-atlas]: https://www.neighborhoodatlas.medicine.wisc.edu/
 [geocode-adi-pypi]: https://pypi.org/project/geocode-adi
 [pop-lab]: https://apl.wisc.edu/
 [us-geocoder]: https://geocoding.geo.census.gov/
-[geocode-adi-pypi]: https://pypi.org/project/geocode-adi/
+[geocode-adi-pypi]: https://pypi.org/project/geocode-adi/
```

### Comparing `geocode-adi-2.0.0/geocode-adi/__main__.py` & `geocode-adi-2.1.0/geocode-adi/__main__.py`

 * *Files identical despite different names*

### Comparing `geocode-adi-2.0.0/geocode-adi/geocodeadi.py` & `geocode-adi-2.1.0/geocode-adi/geocodeadi.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,20 +20,26 @@
 import geopy.exc
 import geopy.extra.rate_limiter
 import numpy
 import pandas
 import requests
 import tqdm
 
-# Dictionary that contains pairs of benchmarks and vintages needed to acquire U.S. Census Block Group information from
-# addresses and coordinates.
-benchmark_vintage_pairs_dict = {
-    'Public_AR_Current': ['Census2010_Current', 'ACS2019_Current', 'ACS2018_Current', 'ACS2017_Current'],
-    'Public_AR_TAB2020': ['ACS2019_TAB2020', 'ACS2018_TAB2020', 'ACS2017_TAB2020', 'Census2010_TAB2020'],
-    'Public_AR_Census2020': ['Census2010_Census2020']}
+
+# Build a dictionary that contains the benchmarks and associated vintages that are available by the U.S. Census Block
+# Group to get geographic data from addresses and coordinates
+benchmark_vintage_pairs_dict = dict()
+benchmarks_dict_list = requests.get('https://geocoding.geo.census.gov/geocoder/benchmarks').json()['benchmarks']
+for benchmark_dict in benchmarks_dict_list:
+    vintages_request_URL = 'https://geocoding.geo.census.gov/geocoder/vintages?benchmark=' + benchmark_dict['id']
+    vintages_dict_list = requests.get(vintages_request_URL).json()['vintages']
+    vintages_dict_list.reverse()
+    vintages_dict_list = vintages_dict_list[-1:] + vintages_dict_list[:-1]
+    vintages_list = [vintage_dict['vintageName'] for vintage_dict in vintages_dict_list]
+    benchmark_vintage_pairs_dict[benchmark_dict['benchmarkName']] = vintages_list
 
 # Convert dictionary of benchmark and vintage pairs to a list of tuples.
 benchmark_vintage_tuple_list = [(benchmark, vintage)
                                 for benchmark, vintages in benchmark_vintage_pairs_dict.items()
                                 for vintage in vintages]
 
 # Ignore FutureWarnings in regards to tqdm Panel. TODO: Fix tqdm panel concerns to remove filter warnings
@@ -630,9 +636,9 @@
 
     # Merge the address data back to the patient data to recreate the original data that was provided, now with geocode
     # and ADI information.
     successful_df = patient_data_df.merge(successful_df, on='data_id').drop(columns='data_id')
     failed_df = patient_data_df.merge(failed_df, on='data_id').drop(columns='data_id')
 
     # Export the successfully and unsuccessfully geocoded DataFrames to CSV.
-    successful_df.to_csv('successful.csv', index=False)
-    failed_df.to_csv('failed.csv', index=False)
+    successful_df.to_csv('successful.csv', index=False, na_rep='NaN')
+    failed_df.to_csv('failed.csv', index=False, na_rep='NaN')
```

### Comparing `geocode-adi-2.0.0/geocode_adi.egg-info/PKG-INFO` & `geocode-adi-2.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,87 @@
-Metadata-Version: 2.1
-Name: geocode-adi
-Version: 2.0.0
-Summary: Map addresses to Area Deprivation Index through U.S. Census Block Groups
-Home-page: https://github.com/AyushDoshi/geocode-adi
-Author: Ayush Doshi
-Author-email: ayushdoshi1@gmail.com
-License: MIT
-Description: # geocode-adi
-        
-        ## What is it?
-        
-        **geocode-adi** is a Python package that allows for the mapping of address information to Gopal K. Singh's 
-        [**Area Deprivation Index (ADI)**][adi-paper] at the U.S. Census Block Group level, which was calculated by the 
-        [**Applied Population Lab at UW-Madison**][pop-lab] and made available on 
-        [**UW-Madison's Neighborhood Atlas**][neigh-atlas].
-        
-        ## Where to get it?
-        The source code is currently hosted on GitHub at:
-        https://github.com/AyushDoshi/geocode-adi.
-        
-        Binary installers for released versions are available at the 
-        [Python Package Index (PyPI)][geocode-adi-pypi].
-        ```
-        pip install geocode-adi
-        ```
-        
-        ### Dependencies
-        - [Pandas](https://pandas.pydata.org/) - Required for reading in address data, manipulating it, and exporting it back 
-        out.
-        - [Numpy](https://www.numpy.org) - Required for chunking address data and adding "Not A Number" values.
-        - [Requests](https://requests.readthedocs.io) - Required for making GET requests to Google.
-        - [Geopy](https://geopy.readthedocs.io) - Required for making geocoding API calls to Nominatim/OpenStreetMaps.
-        - [Census Geocode](https://github.com/fitnr/censusgeocode) - Required for making geocoding API calls to the 
-        [U.S. Census Geocoder][us-geocoder].
-        - [tqdm](https://tqdm.github.io/) - Required for making progress bars.
-        
-        If **geocode-adi** is installed using a binary installer, such as through [PyPI][geocode-adi-pypi], the required 
-        dependencies should automatically be installed.
-        
-        ## How to use it?
-        This package is meant to be run as a script in the command-line/terminal, although the individual functions found in the
-        [*geocodeadi.py*](geocode-adi/geocodeadi.py) file may be imported as a module.
-        
-        The script takes in a comma-delimited file, such as a .CSV, that contains the address information. Specifically, the 
-        file must contain at least 4 columns: *'Address'*, *'City'*, *'State'*, *'ZIP Code'*. These columns must also be 
-        labeled as such. The *'Address'* column must contain at least the street number and name. Other information, such as 
-        apartment or suite number, is optional. An example of a correctly formatted file of addresses is the
-        [*AddressSample.csv*](AddressSample.csv) file in the repository.
-        
-        Once installed, **geocode-adi** can be simply called in the command-line/terminal in the following way:
-        ```
-        python -m geocode-adi [PATH_TO_ADDRESS_FILE]
-        ```
-        For example, using the file [*AddressSample.csv*](AddressSample.csv):
-        ```
-        python -m geocode-adi AddressSample.csv
-        ```
-        ## How does it work?
-        
-        **geocode-adi** works in mapping addresses to ADI in 4 overarching steps:
-        1. It imports the addresses into a Pandas DataFrame.
-        2. It converts the addresses into U.S. Census Block Groups, which itself occurs in 6 steps:
-            1. It filters out the majority of P.O. and Route boxes from the address list and puts them to the side.
-            2. Then it does a first-pass conversion of the filtered addresses directly to U.S. Census Block Groups using the 
-            [U.S. Census Geocoder][us-geocoder].
-            3. The addresses that failed to be directly converted to U.S. Census Block Groups are then tried to be converted to 
-            coordinates using Google.
-            4. The addresses that failed at being converted to coordinates by Google are then tried to be converted to 
-            coordinates using [Nominatim/OpenStreetMaps](https://nominatim.org/).
-            5. The addresses that were successfully converted to coordinates, either by Google or Nominatim/OpenStreetMaps, are 
-            then tried at a second-pass conversion to U.S. Census Block Groups with the U.S. Census Geocoder again, but this 
-            time using the coordinates instead of the addresses directly.
-            6. Addresses that were successfully converted to U.S. Census Blocks, either in the first or second pass, are then 
-            combined. Addresses that failed to be converted, due to being a PO/Route Box, failing to be converted to 
-            coordinates, or failing to have their coordinates converted to U.S. Census Block Groups, are also combined.
-        3. Addresses that were successfully converted to U.S. Census Block Groups then have an ADI value mapped to it based on 
-        its U.S. Census Block Group.
-        4. The addresses that were mapped to ADI values through their U.S. Census Block Group are exported to a .CSV file 
-        labeled ***successful.csv***. Addresses that failed to be converted to Census Block Groups are exported to a .CSV file 
-        labeled ***failed.csv***.
-        
-        ## License
-        [MIT](LICENSE)
-        
-        [adi-paper]: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1447923/
-        [neigh-atlas]: https://www.neighborhoodatlas.medicine.wisc.edu/
-        [geocode-adi-pypi]: https://pypi.org/project/geocode-adi
-        [pop-lab]: https://apl.wisc.edu/
-        [us-geocoder]: https://geocoding.geo.census.gov/
-        [geocode-adi-pypi]: https://pypi.org/project/geocode-adi/
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+# geocode-adi
+
+## What is it?
+
+**geocode-adi** is a Python package that allows for the mapping of address information to Gopal K. Singh's 
+[**Area Deprivation Index (ADI)**][adi-paper] at the U.S. Census Block Group level, which was calculated by the 
+[**Applied Population Lab at UW-Madison**][pop-lab] and made available on 
+[**UW-Madison's Neighborhood Atlas**][neigh-atlas]. For a given address, it will map to the ADI National
+Percentiles and State Deciles for the following years/versions:
+- 2021
+- 2020
+- 2015
+
+## Where to get it?
+The source code is currently hosted on GitHub at:
+https://github.com/AyushDoshi/geocode-adi.
+
+Binary installers for released versions are available at the 
+[Python Package Index (PyPI)][geocode-adi-pypi]. To run the script, Python 3.6 or greater is required.
+```
+pip install geocode-adi
+```
+
+### Dependencies
+- [Pandas](https://pandas.pydata.org/) - Required for reading in address data, manipulating it, and exporting it back 
+out.
+- [Numpy](https://www.numpy.org) - Required for chunking address data and adding "Not A Number" values.
+- [Requests](https://requests.readthedocs.io) - Required for making GET requests to Google.
+- [Geopy](https://geopy.readthedocs.io) - Required for making geocoding API calls to Nominatim/OpenStreetMaps.
+- [Census Geocode](https://github.com/fitnr/censusgeocode) - Required for making geocoding API calls to the 
+[U.S. Census Geocoder][us-geocoder].
+- [tqdm](https://tqdm.github.io/) - Required for making progress bars.
+
+If **geocode-adi** is installed using a binary installer, such as through [PyPI][geocode-adi-pypi], the required 
+dependencies should automatically be installed.
+
+## How to use it?
+This package is meant to be run as a script in the command-line/terminal, although the individual functions found in the
+[*geocodeadi.py*](geocode-adi/geocodeadi.py) file may be imported as a module.
+
+The script takes in a comma-delimited file, such as a .CSV, that contains the address information. Specifically, the 
+file must contain at least 4 columns: *'Address'*, *'City'*, *'State'*, *'ZIP Code'*. These columns must also be 
+labeled as such. The *'Address'* column must contain at least the street number and name. Other information, such as 
+apartment or suite number, is optional. An example of a correctly formatted file of addresses is the
+[*AddressSample.csv*](AddressSample.csv) file in the repository.
+
+Once installed, **geocode-adi** can be simply called in the command-line/terminal in the following way:
+```
+python -m geocode-adi [PATH_TO_ADDRESS_FILE]
+```
+For example, using the file [*AddressSample.csv*](AddressSample.csv):
+```
+python -m geocode-adi AddressSample.csv
+```
+## How does it work?
+
+**geocode-adi** works in mapping addresses to ADI in 4 overarching steps:
+1. It imports the addresses into a Pandas DataFrame.
+2. It converts the addresses into U.S. Census Block Groups, which itself occurs in 6 steps:
+    1. It filters out the majority of P.O. and Route boxes from the address list and puts them to the side.
+    2. Then it does a first-pass conversion of the filtered addresses directly to U.S. Census Block Groups using the 
+    [U.S. Census Geocoder][us-geocoder].
+    3. The addresses that failed to be directly converted to U.S. Census Block Groups are then tried to be converted to 
+    coordinates using Google.
+    4. The addresses that failed at being converted to coordinates by Google are then tried to be converted to 
+    coordinates using [Nominatim/OpenStreetMaps](https://nominatim.org/).
+    5. The addresses that were successfully converted to coordinates, either by Google or Nominatim/OpenStreetMaps, are 
+    then tried at a second-pass conversion to U.S. Census Block Groups with the U.S. Census Geocoder again, but this 
+    time using the coordinates instead of the addresses directly.
+    6. Addresses that were successfully converted to U.S. Census Blocks, either in the first or second pass, are then 
+    combined. Addresses that failed to be converted, due to being a PO/Route Box, failing to be converted to 
+    coordinates, or failing to have their coordinates converted to U.S. Census Block Groups, are also combined.
+3. Addresses that were successfully converted to U.S. Census Block Groups then have an ADI value mapped to it based on 
+its U.S. Census Block Group.
+4. The addresses that were mapped to ADI values through their U.S. Census Block Group are exported to a .CSV file 
+labeled ***successful.csv***. Addresses that failed to be converted to Census Block Groups are exported to a .CSV file 
+labeled ***failed.csv***.
+
+## License
+[MIT](LICENSE)
+
+[adi-paper]: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1447923/
+[neigh-atlas]: https://www.neighborhoodatlas.medicine.wisc.edu/
+[geocode-adi-pypi]: https://pypi.org/project/geocode-adi
+[pop-lab]: https://apl.wisc.edu/
+[us-geocoder]: https://geocoding.geo.census.gov/
+[geocode-adi-pypi]: https://pypi.org/project/geocode-adi/
```

### Comparing `geocode-adi-2.0.0/setup.py` & `geocode-adi-2.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="geocode-adi",
-    version="2.0.0",
+    version="2.1.0",
     description="Map addresses to Area Deprivation Index through U.S. Census Block Groups",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/AyushDoshi/geocode-adi",
     author="Ayush Doshi",
     author_email="ayushdoshi1@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3"
     ],
     python_requires='>=3.8',
     packages=["geocode-adi"],
     include_package_data=True,
-    install_requires=["requests", "tqdm", "censusgeocode", "geopy", "pandas", "numpy", "pyarrow"]
+    install_requires=["requests==2.29.0", "tqdm", "censusgeocode", "geopy", "pandas", "numpy", "pyarrow"],
+    package_dir={'/': 'geocode-adi'}
 )
```

