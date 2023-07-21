# Comparing `tmp/monitorVW-1.4.0.tar.gz` & `tmp/monitorVW-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monitorVW-1.4.0.tar", last modified: Mon Nov 21 14:55:41 2022, max compression
+gzip compressed data, was "monitorVW-1.4.1.tar", last modified: Fri Jul 21 17:31:24 2023, max compression
```

## Comparing `monitorVW-1.4.0.tar` & `monitorVW-1.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-21 14:55:41.441254 monitorVW-1.4.0/
--rw-r--r--   0 root         (0) root         (0)     1063 2022-11-05 17:36:53.000000 monitorVW-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       31 2022-11-08 17:32:47.000000 monitorVW-1.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13004 2022-11-21 14:55:41.441254 monitorVW-1.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12337 2022-11-21 14:40:32.000000 monitorVW-1.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-21 14:55:41.433254 monitorVW-1.4.0/data/
--rw-r--r--   0 root         (0) root         (0)     1242 2022-11-21 14:26:10.000000 monitorVW-1.4.0/data/monitorVW.json
--rw-r--r--   0 root         (0) root         (0)      315 2022-11-08 17:22:26.000000 monitorVW-1.4.0/data/monitorVW.service
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-21 14:55:41.437254 monitorVW-1.4.0/monitorVW/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-05 22:04:06.000000 monitorVW-1.4.0/monitorVW/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26646 2022-11-21 14:29:47.000000 monitorVW-1.4.0/monitorVW/monitorVW.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-21 14:55:41.441254 monitorVW-1.4.0/monitorVW/weconnect/
--rw-r--r--   0 root         (0) root         (0)    34344 2022-11-06 18:46:17.000000 monitorVW-1.4.0/monitorVW/weconnect/NativeAPI.py
--rw-r--r--   0 root         (0) root         (0)      125 2022-11-05 23:43:41.000000 monitorVW-1.4.0/monitorVW/weconnect/__init__.py
--rw-r--r--   0 root         (0) root         (0)       27 2022-11-05 22:08:24.000000 monitorVW-1.4.0/monitorVW/weconnect/_version.py
--rw-r--r--   0 root         (0) root         (0)    10933 2022-11-07 10:12:19.000000 monitorVW-1.4.0/monitorVW/weconnect/vsr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-21 14:55:41.437254 monitorVW-1.4.0/monitorVW.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13004 2022-11-21 14:55:41.000000 monitorVW-1.4.0/monitorVW.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      414 2022-11-21 14:55:41.000000 monitorVW-1.4.0/monitorVW.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-21 14:55:41.000000 monitorVW-1.4.0/monitorVW.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      790 2022-11-21 14:55:41.000000 monitorVW-1.4.0/monitorVW.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-11-21 14:55:41.000000 monitorVW-1.4.0/monitorVW.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-21 14:55:41.441254 monitorVW-1.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    10191 2022-11-21 14:30:24.000000 monitorVW-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 17:31:24.686851 monitorVW-1.4.1/
+-rw-r--r--   0 root         (0) root         (0)     1063 2022-11-05 17:36:53.000000 monitorVW-1.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       31 2022-11-08 17:32:47.000000 monitorVW-1.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    13049 2023-07-21 17:31:24.686851 monitorVW-1.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12382 2023-03-22 10:55:32.000000 monitorVW-1.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 17:31:24.678851 monitorVW-1.4.1/data/
+-rw-r--r--   0 root         (0) root         (0)     1242 2022-11-21 14:26:10.000000 monitorVW-1.4.1/data/monitorVW.json
+-rw-r--r--   0 root         (0) root         (0)      315 2022-11-08 17:22:26.000000 monitorVW-1.4.1/data/monitorVW.service
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 17:31:24.678851 monitorVW-1.4.1/monitorVW/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-05 22:04:06.000000 monitorVW-1.4.1/monitorVW/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26646 2022-11-21 16:20:42.000000 monitorVW-1.4.1/monitorVW/monitorVW.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 17:31:24.682851 monitorVW-1.4.1/monitorVW/weconnect/
+-rw-r--r--   0 root         (0) root         (0)    34513 2023-07-21 17:15:32.000000 monitorVW-1.4.1/monitorVW/weconnect/NativeAPI.py
+-rw-r--r--   0 root         (0) root         (0)      125 2022-11-05 23:43:41.000000 monitorVW-1.4.1/monitorVW/weconnect/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       27 2022-11-05 22:08:24.000000 monitorVW-1.4.1/monitorVW/weconnect/_version.py
+-rw-r--r--   0 root         (0) root         (0)    10933 2022-11-07 10:12:19.000000 monitorVW-1.4.1/monitorVW/weconnect/vsr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 17:31:24.682851 monitorVW-1.4.1/monitorVW.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13049 2023-07-21 17:31:24.000000 monitorVW-1.4.1/monitorVW.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      414 2023-07-21 17:31:24.000000 monitorVW-1.4.1/monitorVW.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 17:31:24.000000 monitorVW-1.4.1/monitorVW.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      790 2023-07-21 17:31:24.000000 monitorVW-1.4.1/monitorVW.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-21 17:31:24.000000 monitorVW-1.4.1/monitorVW.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 17:31:24.686851 monitorVW-1.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    10191 2023-07-21 17:28:08.000000 monitorVW-1.4.1/setup.py
```

### Comparing `monitorVW-1.4.0/LICENSE` & `monitorVW-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `monitorVW-1.4.0/PKG-INFO` & `monitorVW-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monitorVW
-Version: 1.4.0
+Version: 1.4.1
 Summary: Read VW car data from We Connect and store in Influx DB
 Home-page: https://github.com/signag/monitorVW
 Author: signag
 Author-email: siegfried.nagel@t-online.de
 Project-URL: Source, https://github.com/signag/fritzToInfluxHA/
 Keywords: RaspberryPi InfluxDB
 Classifier: Development Status :: 3 - Alpha
@@ -19,15 +19,15 @@
 
 # monitorVW
 
 The program periodically reads car data from Volkswagen WeConnect and stores these as measurements in an InfluxDB database.
 
 For WeConnect, see: <https://www.volkswagen-nutzfahrzeuge.de/de/digitale-dienste-und-apps/we-connect.html>
 
-As interface to WeConnect Web ervices, I use <https://github.com/trocotronic/weconnect>
+As interface to WeConnect Web Services, I use <https://github.com/trocotronic/weconnect>
 
 In order to use the program you need
 - A registration at WeConnect
 - An Influx DB V2.4 or later running on the same or another machine
 - A Grafana instance vor visualization
 
 InfluxDB (<https://www.influxdata.com/products/influxdb-overview/>) is a time series database which can be used as cloud version or local installation on various platforms.
@@ -100,14 +100,15 @@
     "weconSPin": "weconPin",
     "weconCarId": "weconCarID",
     "InfluxOutput": true,
     "InfluxURL": "influxURL",
     "InfluxOrg": "inflixOrg",
     "InfluxToken": "influxToken",
     "InfluxBucket": "influxBucket",
+    "InfluxTripBucket": "influxTripBucket",
     "csvOutput": true,
     "csvFile": "tests/output/monitorVW.csv",
     "carData": {
         "tripDataShortTerm": {
             "InfluxOutput": true,
             "InfluxMeasurement": "tripShortTerm",
             "InfluxTimeStart": "",
```

### Comparing `monitorVW-1.4.0/README.md` & `monitorVW-1.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # monitorVW
 
 The program periodically reads car data from Volkswagen WeConnect and stores these as measurements in an InfluxDB database.
 
 For WeConnect, see: <https://www.volkswagen-nutzfahrzeuge.de/de/digitale-dienste-und-apps/we-connect.html>
 
-As interface to WeConnect Web ervices, I use <https://github.com/trocotronic/weconnect>
+As interface to WeConnect Web Services, I use <https://github.com/trocotronic/weconnect>
 
 In order to use the program you need
 - A registration at WeConnect
 - An Influx DB V2.4 or later running on the same or another machine
 - A Grafana instance vor visualization
 
 InfluxDB (<https://www.influxdata.com/products/influxdb-overview/>) is a time series database which can be used as cloud version or local installation on various platforms.
@@ -81,14 +81,15 @@
     "weconSPin": "weconPin",
     "weconCarId": "weconCarID",
     "InfluxOutput": true,
     "InfluxURL": "influxURL",
     "InfluxOrg": "inflixOrg",
     "InfluxToken": "influxToken",
     "InfluxBucket": "influxBucket",
+    "InfluxTripBucket": "influxTripBucket",
     "csvOutput": true,
     "csvFile": "tests/output/monitorVW.csv",
     "carData": {
         "tripDataShortTerm": {
             "InfluxOutput": true,
             "InfluxMeasurement": "tripShortTerm",
             "InfluxTimeStart": "",
```

### Comparing `monitorVW-1.4.0/data/monitorVW.json` & `monitorVW-1.4.1/data/monitorVW.json`

 * *Files identical despite different names*

### Comparing `monitorVW-1.4.0/monitorVW/monitorVW.py` & `monitorVW-1.4.1/monitorVW/monitorVW.py`

 * *Files identical despite different names*

### Comparing `monitorVW-1.4.0/monitorVW/weconnect/NativeAPI.py` & `monitorVW-1.4.1/monitorVW/weconnect/NativeAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,14 +305,16 @@
             soup = BeautifulSoup(r.text, 'html.parser')
             scripts = soup.find_all('script')
             for script in scripts:
                 if script.string and 'window._IDK' in script.string:
                     try:
                         idk_txt = '{'+re.search(r'\{(.*)\}',script.string,re.M|re.S).group(1)+'}'
                         idk_txt = re.sub(r'([\{\s,])(\w+)(:)', r'\1"\2"\3', idk_txt.replace('\'','"'))
+                        ### response contained invalid JSON
+                        idk_txt = idk_txt.replace('"isFooterEnabled": false,', '"isFooterEnabled": false')
                         idk = json.loads(idk_txt)
                         break
                     except json.decoder.JSONDecodeError:
                         raise VWError('Cannot find IDK credentials')
 
             post['hmac'] = idk['templateModel']['hmac']
             post['password'] = self.__credentials['password']
```

### Comparing `monitorVW-1.4.0/monitorVW/weconnect/vsr.py` & `monitorVW-1.4.1/monitorVW/weconnect/vsr.py`

 * *Files identical despite different names*

### Comparing `monitorVW-1.4.0/monitorVW.egg-info/PKG-INFO` & `monitorVW-1.4.1/monitorVW.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monitorVW
-Version: 1.4.0
+Version: 1.4.1
 Summary: Read VW car data from We Connect and store in Influx DB
 Home-page: https://github.com/signag/monitorVW
 Author: signag
 Author-email: siegfried.nagel@t-online.de
 Project-URL: Source, https://github.com/signag/fritzToInfluxHA/
 Keywords: RaspberryPi InfluxDB
 Classifier: Development Status :: 3 - Alpha
@@ -19,15 +19,15 @@
 
 # monitorVW
 
 The program periodically reads car data from Volkswagen WeConnect and stores these as measurements in an InfluxDB database.
 
 For WeConnect, see: <https://www.volkswagen-nutzfahrzeuge.de/de/digitale-dienste-und-apps/we-connect.html>
 
-As interface to WeConnect Web ervices, I use <https://github.com/trocotronic/weconnect>
+As interface to WeConnect Web Services, I use <https://github.com/trocotronic/weconnect>
 
 In order to use the program you need
 - A registration at WeConnect
 - An Influx DB V2.4 or later running on the same or another machine
 - A Grafana instance vor visualization
 
 InfluxDB (<https://www.influxdata.com/products/influxdb-overview/>) is a time series database which can be used as cloud version or local installation on various platforms.
@@ -100,14 +100,15 @@
     "weconSPin": "weconPin",
     "weconCarId": "weconCarID",
     "InfluxOutput": true,
     "InfluxURL": "influxURL",
     "InfluxOrg": "inflixOrg",
     "InfluxToken": "influxToken",
     "InfluxBucket": "influxBucket",
+    "InfluxTripBucket": "influxTripBucket",
     "csvOutput": true,
     "csvFile": "tests/output/monitorVW.csv",
     "carData": {
         "tripDataShortTerm": {
             "InfluxOutput": true,
             "InfluxMeasurement": "tripShortTerm",
             "InfluxTimeStart": "",
```

### Comparing `monitorVW-1.4.0/monitorVW.egg-info/requires.txt` & `monitorVW-1.4.1/monitorVW.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `monitorVW-1.4.0/setup.py` & `monitorVW-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     name="monitorVW",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="1.4.0",  # Required
+    version="1.4.1",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Read VW car data from We Connect and store in Influx DB",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

