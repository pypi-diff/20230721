# Comparing `tmp/uk_geo_utils-0.8.1.tar.gz` & `tmp/uk_geo_utils-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/uk_geo_utils-0.8.1.tar", last modified: Wed Oct 16 19:12:02 2019, max compression
+gzip compressed data, was "dist/uk_geo_utils-0.9.0.tar", last modified: Thu Feb  6 15:29:46 2020, max compression
```

## Comparing `uk_geo_utils-0.8.1.tar` & `uk_geo_utils-0.9.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2019-10-16 19:12:02.000000 uk_geo_utils-0.8.1/
--rw-rw-r--   0 chris     (1000) chris     (1000)      956 2019-10-16 19:10:58.000000 uk_geo_utils-0.8.1/README.md
--rw-rw-r--   0 chris     (1000) chris     (1000)       55 2018-05-22 17:05:07.000000 uk_geo_utils-0.8.1/MANIFEST.in
--rw-rw-r--   0 chris     (1000) chris     (1000)     2045 2019-10-16 19:12:02.000000 uk_geo_utils-0.8.1/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     1585 2019-10-16 19:10:58.000000 uk_geo_utils-0.8.1/setup.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2019-10-16 19:12:02.000000 uk_geo_utils-0.8.1/uk_geo_utils/
--rw-rw-r--   0 chris     (1000) chris     (1000)     7564 2019-10-16 19:10:58.000000 uk_geo_utils-0.8.1/uk_geo_utils/models.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2019-10-16 19:12:02.000000 uk_geo_utils-0.8.1/uk_geo_utils/management/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2019-10-16 19:12:02.000000 uk_geo_utils-0.8.1/uk_geo_utils/management/commands/
--rw-rw-r--   0 chris     (1000) chris     (1000)     3188 2019-10-16 19:10:58.000000 uk_geo_utils-0.8.1/uk_geo_utils/management/commands/clean_addressbase.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2217 2019-10-16 19:10:58.000000 uk_geo_utils-0.8.1/uk_geo_utils/management/commands/import_onsud.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1693 2019-10-16 19:10:58.000000 uk_geo_utils-0.8.1/uk_geo_utils/management/commands/import_cleaned_addresses.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2778 2019-10-16 19:10:58.000000 uk_geo_utils-0.8.1/uk_geo_utils/management/commands/import_onspd.py
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2017-10-03 12:23:49.000000 uk_geo_utils-0.8.1/uk_geo_utils/management/commands/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2017-10-03 12:23:49.000000 uk_geo_utils-0.8.1/uk_geo_utils/management/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4370 2019-10-16 19:10:58.000000 uk_geo_utils-0.8.1/uk_geo_utils/geocoders.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7106 2019-10-16 19:10:58.000000 uk_geo_utils-0.8.1/uk_geo_utils/helpers.py
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2017-10-03 12:23:49.000000 uk_geo_utils-0.8.1/uk_geo_utils/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2019-10-16 19:12:02.000000 uk_geo_utils-0.8.1/uk_geo_utils/migrations/
--rw-rw-r--   0 chris     (1000) chris     (1000)      515 2019-10-16 19:10:58.000000 uk_geo_utils-0.8.1/uk_geo_utils/migrations/0003_auto_20171030_1504.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3097 2019-10-16 19:10:58.000000 uk_geo_utils-0.8.1/uk_geo_utils/migrations/0001_initial.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      270 2019-10-16 19:10:58.000000 uk_geo_utils-0.8.1/uk_geo_utils/migrations/0007_remove_onsud_ctry_flag.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      759 2019-10-16 19:10:58.000000 uk_geo_utils-0.8.1/uk_geo_utils/migrations/0006_auto_20180612_1655.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4989 2019-10-16 19:10:58.000000 uk_geo_utils-0.8.1/uk_geo_utils/migrations/0002_onspd.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      446 2019-10-16 19:10:58.000000 uk_geo_utils-0.8.1/uk_geo_utils/migrations/0005_onsud_ced.py
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2017-10-03 12:23:49.000000 uk_geo_utils-0.8.1/uk_geo_utils/migrations/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1349 2019-10-16 19:10:58.000000 uk_geo_utils-0.8.1/uk_geo_utils/migrations/0004_auto_20180228_1553.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2019-10-16 19:12:02.000000 uk_geo_utils-0.8.1/uk_geo_utils.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)       13 2019-10-16 19:12:02.000000 uk_geo_utils-0.8.1/uk_geo_utils.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      965 2019-10-16 19:12:02.000000 uk_geo_utils-0.8.1/uk_geo_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     2045 2019-10-16 19:12:02.000000 uk_geo_utils-0.8.1/uk_geo_utils.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)       73 2019-10-16 19:12:02.000000 uk_geo_utils-0.8.1/uk_geo_utils.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2019-10-16 19:12:02.000000 uk_geo_utils-0.8.1/uk_geo_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2019-10-16 19:12:02.000000 uk_geo_utils-0.8.1/setup.cfg
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2020-02-06 15:29:46.000000 uk_geo_utils-0.9.0/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      956 2019-10-16 19:10:58.000000 uk_geo_utils-0.9.0/README.md
+-rw-rw-r--   0 chris     (1000) chris     (1000)       55 2018-05-22 17:05:07.000000 uk_geo_utils-0.9.0/MANIFEST.in
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2045 2020-02-06 15:29:46.000000 uk_geo_utils-0.9.0/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1578 2020-02-06 15:29:05.000000 uk_geo_utils-0.9.0/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2020-02-06 15:29:46.000000 uk_geo_utils-0.9.0/uk_geo_utils/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7633 2020-02-06 15:29:05.000000 uk_geo_utils-0.9.0/uk_geo_utils/models.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2020-02-06 15:29:46.000000 uk_geo_utils-0.9.0/uk_geo_utils/management/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2020-02-06 15:29:46.000000 uk_geo_utils-0.9.0/uk_geo_utils/management/commands/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2217 2019-10-16 19:10:58.000000 uk_geo_utils-0.9.0/uk_geo_utils/management/commands/import_onsud.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6405 2020-02-06 15:29:05.000000 uk_geo_utils-0.9.0/uk_geo_utils/management/commands/clean_addressbase_plus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1712 2020-02-06 15:29:05.000000 uk_geo_utils-0.9.0/uk_geo_utils/management/commands/import_cleaned_addresses.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2778 2019-10-16 19:10:58.000000 uk_geo_utils-0.9.0/uk_geo_utils/management/commands/import_onspd.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2017-10-03 12:23:49.000000 uk_geo_utils-0.9.0/uk_geo_utils/management/commands/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3423 2020-02-06 15:29:05.000000 uk_geo_utils-0.9.0/uk_geo_utils/management/commands/clean_addressbase_standard.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2017-10-03 12:23:49.000000 uk_geo_utils-0.9.0/uk_geo_utils/management/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4527 2020-02-06 15:29:05.000000 uk_geo_utils-0.9.0/uk_geo_utils/geocoders.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10131 2020-02-06 15:29:05.000000 uk_geo_utils-0.9.0/uk_geo_utils/helpers.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2017-10-03 12:23:49.000000 uk_geo_utils-0.9.0/uk_geo_utils/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2020-02-06 15:29:46.000000 uk_geo_utils-0.9.0/uk_geo_utils/migrations/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      515 2019-10-16 19:10:58.000000 uk_geo_utils-0.9.0/uk_geo_utils/migrations/0003_auto_20171030_1504.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      438 2020-02-06 15:29:05.000000 uk_geo_utils-0.9.0/uk_geo_utils/migrations/0008_address_addressbase_postal.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3097 2019-10-16 19:10:58.000000 uk_geo_utils-0.9.0/uk_geo_utils/migrations/0001_initial.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      270 2019-10-16 19:10:58.000000 uk_geo_utils-0.9.0/uk_geo_utils/migrations/0007_remove_onsud_ctry_flag.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      759 2019-10-16 19:10:58.000000 uk_geo_utils-0.9.0/uk_geo_utils/migrations/0006_auto_20180612_1655.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4989 2019-10-16 19:10:58.000000 uk_geo_utils-0.9.0/uk_geo_utils/migrations/0002_onspd.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      446 2019-10-16 19:10:58.000000 uk_geo_utils-0.9.0/uk_geo_utils/migrations/0005_onsud_ced.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2017-10-03 12:23:49.000000 uk_geo_utils-0.9.0/uk_geo_utils/migrations/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1349 2019-10-16 19:10:58.000000 uk_geo_utils-0.9.0/uk_geo_utils/migrations/0004_auto_20180228_1553.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2020-02-06 15:29:46.000000 uk_geo_utils-0.9.0/uk_geo_utils.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       13 2020-02-06 15:29:46.000000 uk_geo_utils-0.9.0/uk_geo_utils.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1092 2020-02-06 15:29:46.000000 uk_geo_utils-0.9.0/uk_geo_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2045 2020-02-06 15:29:46.000000 uk_geo_utils-0.9.0/uk_geo_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)       66 2020-02-06 15:29:46.000000 uk_geo_utils-0.9.0/uk_geo_utils.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2020-02-06 15:29:46.000000 uk_geo_utils-0.9.0/uk_geo_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2020-02-06 15:29:46.000000 uk_geo_utils-0.9.0/setup.cfg
```

### Comparing `uk_geo_utils-0.8.1/README.md` & `uk_geo_utils-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `uk_geo_utils-0.8.1/PKG-INFO` & `uk_geo_utils-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uk_geo_utils
-Version: 0.8.1
+Version: 0.9.0
 Summary: Django app for working with OS Addressbase, ONSUD and ONSPD
 Home-page: https://github.com/DemocracyClub/uk-geo-utils
 Author: chris48s
 License: MIT
 Project-URL: Documentation, https://democracyclub.github.io/uk-geo-utils/
 Project-URL: Source, https://github.com/DemocracyClub/uk-geo-utils
 Description: # Django UK Geo Utils
```

### Comparing `uk_geo_utils-0.8.1/setup.py` & `uk_geo_utils-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,25 +13,25 @@
             return f.read()
     except IOError:
         return ""
 
 
 setup(
     name="uk_geo_utils",
-    version="0.8.1",
+    version="0.9.0",
     author="chris48s",
     license="MIT",
     url="https://github.com/DemocracyClub/uk-geo-utils",
     packages=find_packages(),
     include_package_data=True,
     description="Django app for working with OS Addressbase, ONSUD and ONSPD",
     long_description=_get_description(),
     long_description_content_type="text/markdown",
     install_requires=["Django>=1.11,<2.3", "psycopg2-binary"],
-    extras_require={"development": ["python-coveralls", "mkdocs"]},
+    extras_require={"development": ["coveralls", "mkdocs"]},
     classifiers=[
         "Framework :: Django",
         "Framework :: Django :: 1.11",
         "Framework :: Django :: 2.1",
         "Framework :: Django :: 2.2",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
```

### Comparing `uk_geo_utils-0.8.1/uk_geo_utils/models.py` & `uk_geo_utils-0.9.0/uk_geo_utils/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 
 class AbstractAddress(models.Model):
     uprn = models.CharField(primary_key=True, max_length=100)
     address = models.TextField(blank=True)
     postcode = models.CharField(blank=True, max_length=15, db_index=True)
     location = models.PointField(null=True, blank=True)
+    addressbase_postal = models.CharField(blank=False, max_length=1)
     objects = AbstractAddressManager()
 
     class Meta:
         abstract = True
 
 
 class Address(AbstractAddress):
```

### Comparing `uk_geo_utils-0.8.1/uk_geo_utils/management/commands/clean_addressbase.py` & `uk_geo_utils-0.9.0/uk_geo_utils/management/commands/clean_addressbase_standard.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import csv
 import os
 import glob
-from uk_geo_utils.helpers import AddressFormatter
+from uk_geo_utils.helpers import PAFAddressFormatter
 from django.core.management.base import BaseCommand
 
 
 class Command(BaseCommand):
     def add_arguments(self, parser):
         parser.add_argument(
             "ab_path", help="The path to the folder containing the AddressBase CSVs"
@@ -49,28 +49,35 @@
             raise FileNotFoundError("No CSV files found in %s" % (self.base_path))
 
         with open(out_path, "w") as out_file:
             for csv_path in files:
                 if csv_path.endswith("cleaned.csv"):
                     continue
                 self.out_csv = csv.DictWriter(
-                    out_file, fieldnames=["UPRN", "address", "postcode", "location"]
+                    out_file,
+                    fieldnames=[
+                        "UPRN",
+                        "address",
+                        "postcode",
+                        "location",
+                        "addressbase_postal",
+                    ],
                 )
                 self.stdout.write(csv_path)
                 self.clean_csv(csv_path)
                 out_file.flush()
 
-    def line_filer(self, csv_path):
+    def line_filter(self, csv_path):
         with open(csv_path) as csv_file:
             for line in csv.DictReader(csv_file, fieldnames=self.fieldnames):
                 # Do any filtering we might need to do here
                 yield line
 
     def clean_csv(self, csv_path):
-        for line in self.line_filer(csv_path):
+        for line in self.line_filter(csv_path):
             self.out_csv.writerow(self.clean_output_line(line))
 
     def clean_address(self, line):
         address_fields = [
             "ORGANISATION_NAME",
             "DEPARTMENT_NAME",
             "PO_BOX_NUMBER",
@@ -80,18 +87,19 @@
             "DEPENDENT_THOROUGHFARE",
             "THOROUGHFARE",
             "DOUBLE_DEPENDENT_LOCALITY",
             "DEPENDENT_LOCALITY",
             "POST_TOWN",
         ]
         kwargs = {k.lower(): line[k] for k in line if k in address_fields}
-        return AddressFormatter(**kwargs).generate_address_label()
+        return PAFAddressFormatter(**kwargs).generate_address_label()
 
     def clean_output_line(self, line):
         data = {}
         data["UPRN"] = line["UPRN"]
         data["address"] = self.clean_address(line)
         data["postcode"] = line["POSTCODE"]
         data["location"] = "SRID=4326;POINT({} {})".format(
             line["LONGITUDE"], line["LATITUDE"]
         )
+        data["addressbase_postal"] = "D"
         return data
```

### Comparing `uk_geo_utils-0.8.1/uk_geo_utils/management/commands/import_onsud.py` & `uk_geo_utils-0.9.0/uk_geo_utils/management/commands/import_onsud.py`

 * *Files identical despite different names*

### Comparing `uk_geo_utils-0.8.1/uk_geo_utils/management/commands/import_cleaned_addresses.py` & `uk_geo_utils-0.9.0/uk_geo_utils/management/commands/import_cleaned_addresses.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             cursor = connection.cursor()
             self.stdout.write("clearing existing data..")
             cursor.execute("TRUNCATE TABLE %s;" % (self.table_name))
 
             self.stdout.write("importing from %s.." % (cleaned_file_path))
             cursor.copy_expert(
                 """
-                COPY %s (UPRN,address,postcode,location)
+                COPY %s (UPRN,address,postcode,location,addressbase_postal)
                 FROM STDIN (FORMAT CSV, DELIMITER ',', quote '"');
             """
                 % (self.table_name),
                 fp,
             )
 
         self.stdout.write("...done")
```

### Comparing `uk_geo_utils-0.8.1/uk_geo_utils/management/commands/import_onspd.py` & `uk_geo_utils-0.9.0/uk_geo_utils/management/commands/import_onspd.py`

 * *Files identical despite different names*

### Comparing `uk_geo_utils-0.8.1/uk_geo_utils/geocoders.py` & `uk_geo_utils-0.9.0/uk_geo_utils/geocoders.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,14 +85,17 @@
 
     @property
     def uprns(self):
         return [a.uprn for a in self._addresses]
 
     @property
     def centroid(self):
+        type_d_addresses = self._addresses.filter(addressbase_postal="D")
+        if len(type_d_addresses) > 0:
+            return type_d_addresses.centroid
         return self._addresses.centroid
 
     @property
     def addresses(self):
         sorter = AddressSorter(self._addresses)
         return sorter.natural_sort()
```

### Comparing `uk_geo_utils-0.8.1/uk_geo_utils/migrations/0003_auto_20171030_1504.py` & `uk_geo_utils-0.9.0/uk_geo_utils/migrations/0003_auto_20171030_1504.py`

 * *Files identical despite different names*

### Comparing `uk_geo_utils-0.8.1/uk_geo_utils/migrations/0001_initial.py` & `uk_geo_utils-0.9.0/uk_geo_utils/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `uk_geo_utils-0.8.1/uk_geo_utils/migrations/0006_auto_20180612_1655.py` & `uk_geo_utils-0.9.0/uk_geo_utils/migrations/0006_auto_20180612_1655.py`

 * *Files identical despite different names*

### Comparing `uk_geo_utils-0.8.1/uk_geo_utils/migrations/0002_onspd.py` & `uk_geo_utils-0.9.0/uk_geo_utils/migrations/0002_onspd.py`

 * *Files identical despite different names*

### Comparing `uk_geo_utils-0.8.1/uk_geo_utils/migrations/0004_auto_20180228_1553.py` & `uk_geo_utils-0.9.0/uk_geo_utils/migrations/0004_auto_20180228_1553.py`

 * *Files identical despite different names*

### Comparing `uk_geo_utils-0.8.1/uk_geo_utils.egg-info/SOURCES.txt` & `uk_geo_utils-0.9.0/uk_geo_utils.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 uk_geo_utils.egg-info/PKG-INFO
 uk_geo_utils.egg-info/SOURCES.txt
 uk_geo_utils.egg-info/dependency_links.txt
 uk_geo_utils.egg-info/requires.txt
 uk_geo_utils.egg-info/top_level.txt
 uk_geo_utils/management/__init__.py
 uk_geo_utils/management/commands/__init__.py
-uk_geo_utils/management/commands/clean_addressbase.py
+uk_geo_utils/management/commands/clean_addressbase_plus.py
+uk_geo_utils/management/commands/clean_addressbase_standard.py
 uk_geo_utils/management/commands/import_cleaned_addresses.py
 uk_geo_utils/management/commands/import_onspd.py
 uk_geo_utils/management/commands/import_onsud.py
 uk_geo_utils/migrations/0001_initial.py
 uk_geo_utils/migrations/0002_onspd.py
 uk_geo_utils/migrations/0003_auto_20171030_1504.py
 uk_geo_utils/migrations/0004_auto_20180228_1553.py
 uk_geo_utils/migrations/0005_onsud_ced.py
 uk_geo_utils/migrations/0006_auto_20180612_1655.py
 uk_geo_utils/migrations/0007_remove_onsud_ctry_flag.py
+uk_geo_utils/migrations/0008_address_addressbase_postal.py
 uk_geo_utils/migrations/__init__.py
```

### Comparing `uk_geo_utils-0.8.1/uk_geo_utils.egg-info/PKG-INFO` & `uk_geo_utils-0.9.0/uk_geo_utils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uk-geo-utils
-Version: 0.8.1
+Version: 0.9.0
 Summary: Django app for working with OS Addressbase, ONSUD and ONSPD
 Home-page: https://github.com/DemocracyClub/uk-geo-utils
 Author: chris48s
 License: MIT
 Project-URL: Documentation, https://democracyclub.github.io/uk-geo-utils/
 Project-URL: Source, https://github.com/DemocracyClub/uk-geo-utils
 Description: # Django UK Geo Utils
```

