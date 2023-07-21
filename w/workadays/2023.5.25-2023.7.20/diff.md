# Comparing `tmp/workadays-2023.5.25.tar.gz` & `tmp/workadays-2023.7.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workadays-2023.5.25.tar", last modified: Thu May 25 22:36:50 2023, max compression
+gzip compressed data, was "workadays-2023.7.20.tar", last modified: Fri Jul 21 01:56:01 2023, max compression
```

## Comparing `workadays-2023.5.25.tar` & `workadays-2023.7.20.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 22:36:50.536721 workadays-2023.5.25/
--rw-rw-rw-   0        0        0      395 2022-07-24 01:31:47.000000 workadays-2023.5.25/.gitattributes
--rw-rw-rw-   0        0        0      306 2023-05-23 20:16:32.000000 workadays-2023.5.25/.gitignore
--rw-rw-rw-   0        0        0     1090 2022-07-24 01:31:47.000000 workadays-2023.5.25/LICENSE
--rw-rw-rw-   0        0        0     3236 2023-05-25 22:36:50.536721 workadays-2023.5.25/PKG-INFO
--rw-rw-rw-   0        0        0     2483 2023-05-25 22:34:35.000000 workadays-2023.5.25/README.md
--rw-rw-rw-   0        0        0      111 2023-05-25 22:36:50.551726 workadays-2023.5.25/Setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-05-25 22:32:50.000000 workadays-2023.5.25/Setup.py
--rw-rw-rw-   0        0        0       67 2023-05-23 20:15:53.000000 workadays-2023.5.25/Tests.py
--rw-rw-rw-   0        0        0       26 2023-05-25 22:35:49.000000 workadays-2023.5.25/commit
-drwxrwxrwx   0        0        0        0 2023-05-25 22:36:50.520711 workadays-2023.5.25/workadays/
-drwxrwxrwx   0        0        0        0 2023-05-25 22:36:50.536721 workadays-2023.5.25/workadays/.idea/
--rw-rw-rw-   0        0        0       50 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/.idea/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-25 22:36:50.536721 workadays-2023.5.25/workadays/.idea/inspectionProfiles/
--rw-rw-rw-   0        0        0     1413 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/.idea/inspectionProfiles/Project_Default.xml
--rw-rw-rw-   0        0        0      179 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0        0        0      188 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/.idea/misc.xml
--rw-rw-rw-   0        0        0      277 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/.idea/modules.xml
--rw-rw-rw-   0        0        0      452 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/.idea/workadays.iml
--rw-rw-rw-   0        0        0       84 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:36:50.536721 workadays-2023.5.25/workadays/__pycache__/
--rw-rw-rw-   0        0        0      185 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     4918 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/__pycache__/brazil.cpython-38.pyc
--rw-rw-rw-   0        0        0      326 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/__pycache__/constants.cpython-38.pyc
--rw-rw-rw-   0        0        0      579 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/__pycache__/countries.cpython-38.pyc
--rw-rw-rw-   0        0        0     6029 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/__pycache__/holiday_base.cpython-38.pyc
--rw-rw-rw-   0        0        0     1183 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/__pycache__/holidays.cpython-38.pyc
--rw-rw-rw-   0        0        0     1764 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/__pycache__/luxembourg.cpython-38.pyc
--rw-rw-rw-   0        0        0      267 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/__pycache__/main.cpython-38.pyc
--rw-rw-rw-   0        0        0     5829 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/__pycache__/united_kingdom.cpython-38.pyc
--rw-rw-rw-   0        0        0    11834 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/__pycache__/united_states.cpython-38.pyc
--rw-rw-rw-   0        0        0     3478 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/__pycache__/workdays.cpython-38.pyc
--rw-rw-rw-   0        0        0     5294 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/__pycache__/workdays_tests.cpython-38.pyc
--rw-rw-rw-   0        0        0     6841 2023-05-23 20:15:53.000000 workadays-2023.5.25/workadays/brazil.py
--rw-rw-rw-   0        0        0      172 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/constants.py
--rw-rw-rw-   0        0        0      280 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/countries.py
--rw-rw-rw-   0        0        0     7571 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/holiday_base.py
--rw-rw-rw-   0        0        0      850 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/holidays.py
--rw-rw-rw-   0        0        0     2010 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/luxembourg.py
--rw-rw-rw-   0        0        0      148 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/main.py
--rw-rw-rw-   0        0        0     8507 2022-07-24 01:31:47.000000 workadays-2023.5.25/workadays/united_kingdom.py
--rw-rw-rw-   0        0        0    23951 2022-08-08 22:43:01.000000 workadays-2023.5.25/workadays/united_states.py
--rw-rw-rw-   0        0        0     6653 2023-05-25 22:26:38.000000 workadays-2023.5.25/workadays/workdays.py
--rw-rw-rw-   0        0        0     8922 2023-05-25 22:32:16.000000 workadays-2023.5.25/workadays/workdays_tests.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:36:50.535714 workadays-2023.5.25/workadays.egg-info/
--rw-rw-rw-   0        0        0     3236 2023-05-25 22:36:50.000000 workadays-2023.5.25/workadays.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1337 2023-05-25 22:36:50.000000 workadays-2023.5.25/workadays.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 22:36:50.000000 workadays-2023.5.25/workadays.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-05-25 22:36:50.000000 workadays-2023.5.25/workadays.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-25 22:36:50.000000 workadays-2023.5.25/workadays.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 01:56:01.699044 workadays-2023.7.20/
+-rw-rw-rw-   0        0        0      395 2022-07-24 01:31:47.000000 workadays-2023.7.20/.gitattributes
+-rw-rw-rw-   0        0        0      306 2023-05-23 20:16:32.000000 workadays-2023.7.20/.gitignore
+-rw-rw-rw-   0        0        0     1090 2022-07-24 01:31:47.000000 workadays-2023.7.20/LICENSE
+-rw-rw-rw-   0        0        0     3236 2023-07-21 01:56:01.699044 workadays-2023.7.20/PKG-INFO
+-rw-rw-rw-   0        0        0     2483 2023-05-25 22:34:35.000000 workadays-2023.7.20/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-21 01:56:01.699044 workadays-2023.7.20/Setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-07-21 01:52:41.000000 workadays-2023.7.20/Setup.py
+-rw-rw-rw-   0        0        0       67 2023-05-23 20:15:53.000000 workadays-2023.7.20/Tests.py
+-rw-rw-rw-   0        0        0       26 2023-05-25 22:35:49.000000 workadays-2023.7.20/commit
+drwxrwxrwx   0        0        0        0 2023-07-21 01:56:01.667132 workadays-2023.7.20/workadays/
+drwxrwxrwx   0        0        0        0 2023-07-21 01:56:01.682757 workadays-2023.7.20/workadays/.idea/
+-rw-rw-rw-   0        0        0       50 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/.idea/.gitignore
+drwxrwxrwx   0        0        0        0 2023-07-21 01:56:01.682757 workadays-2023.7.20/workadays/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0     1413 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/.idea/inspectionProfiles/Project_Default.xml
+-rw-rw-rw-   0        0        0      179 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      188 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/.idea/misc.xml
+-rw-rw-rw-   0        0        0      277 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/.idea/modules.xml
+-rw-rw-rw-   0        0        0      452 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/.idea/workadays.iml
+-rw-rw-rw-   0        0        0       84 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 01:56:01.699044 workadays-2023.7.20/workadays/__pycache__/
+-rw-rw-rw-   0        0        0      185 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0     4918 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/__pycache__/brazil.cpython-38.pyc
+-rw-rw-rw-   0        0        0      326 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/__pycache__/constants.cpython-38.pyc
+-rw-rw-rw-   0        0        0      579 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/__pycache__/countries.cpython-38.pyc
+-rw-rw-rw-   0        0        0     6029 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/__pycache__/holiday_base.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1183 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/__pycache__/holidays.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1764 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/__pycache__/luxembourg.cpython-38.pyc
+-rw-rw-rw-   0        0        0      267 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/__pycache__/main.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5829 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/__pycache__/united_kingdom.cpython-38.pyc
+-rw-rw-rw-   0        0        0    11834 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/__pycache__/united_states.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3478 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/__pycache__/workdays.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5294 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/__pycache__/workdays_tests.cpython-38.pyc
+-rw-rw-rw-   0        0        0     6841 2023-05-23 20:15:53.000000 workadays-2023.7.20/workadays/brazil.py
+-rw-rw-rw-   0        0        0      172 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/constants.py
+-rw-rw-rw-   0        0        0      280 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/countries.py
+-rw-rw-rw-   0        0        0     7571 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/holiday_base.py
+-rw-rw-rw-   0        0        0      850 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/holidays.py
+-rw-rw-rw-   0        0        0     2010 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/luxembourg.py
+-rw-rw-rw-   0        0        0      148 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/main.py
+-rw-rw-rw-   0        0        0     8507 2022-07-24 01:31:47.000000 workadays-2023.7.20/workadays/united_kingdom.py
+-rw-rw-rw-   0        0        0    23951 2022-08-08 22:43:01.000000 workadays-2023.7.20/workadays/united_states.py
+-rw-rw-rw-   0        0        0     6655 2023-07-21 01:49:46.000000 workadays-2023.7.20/workadays/workdays.py
+-rw-rw-rw-   0        0        0     9071 2023-07-21 01:52:41.000000 workadays-2023.7.20/workadays/workdays_tests.py
+drwxrwxrwx   0        0        0        0 2023-07-21 01:56:01.682757 workadays-2023.7.20/workadays.egg-info/
+-rw-rw-rw-   0        0        0     3236 2023-07-21 01:56:01.000000 workadays-2023.7.20/workadays.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1337 2023-07-21 01:56:01.000000 workadays-2023.7.20/workadays.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 01:56:01.000000 workadays-2023.7.20/workadays.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-21 01:56:01.000000 workadays-2023.7.20/workadays.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-21 01:56:01.000000 workadays-2023.7.20/workadays.egg-info/top_level.txt
```

### Comparing `workadays-2023.5.25/LICENSE` & `workadays-2023.7.20/LICENSE`

 * *Files identical despite different names*

### Comparing `workadays-2023.5.25/PKG-INFO` & `workadays-2023.7.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workadays
-Version: 2023.5.25
+Version: 2023.7.20
 Summary: Calendário de dias úteis, dias corridos e dias 360 (30/360).
 Home-page: https://github.com/mfhorita
 Author: Marcelo Horita
 Author-email: mfhorita@gmail.com.br
 License: MIT License
 Keywords: workdays workadays feriados holidays diasuteis uteis,dias360,days360,days
 Classifier: License :: Freeware
```

### Comparing `workadays-2023.5.25/README.md` & `workadays-2023.7.20/README.md`

 * *Files identical despite different names*

### Comparing `workadays-2023.5.25/Setup.py` & `workadays-2023.7.20/Setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='workadays',
-    version='2023.05.25',
+    version='2023.07.20',
     author='Marcelo Horita',
     author_email='mfhorita@gmail.com.br',
     packages=['workadays'],
     description="Calendário de dias úteis, dias corridos e dias 360 (30/360).",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mfhorita',
```

### Comparing `workadays-2023.5.25/workadays/.idea/inspectionProfiles/Project_Default.xml` & `workadays-2023.7.20/workadays/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `workadays-2023.5.25/workadays/__pycache__/brazil.cpython-38.pyc` & `workadays-2023.7.20/workadays/__pycache__/brazil.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `workadays-2023.5.25/workadays/__pycache__/countries.cpython-38.pyc` & `workadays-2023.7.20/workadays/__pycache__/countries.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `workadays-2023.5.25/workadays/__pycache__/holiday_base.cpython-38.pyc` & `workadays-2023.7.20/workadays/__pycache__/holiday_base.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `workadays-2023.5.25/workadays/__pycache__/holidays.cpython-38.pyc` & `workadays-2023.7.20/workadays/__pycache__/holidays.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `workadays-2023.5.25/workadays/__pycache__/luxembourg.cpython-38.pyc` & `workadays-2023.7.20/workadays/__pycache__/luxembourg.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `workadays-2023.5.25/workadays/__pycache__/united_kingdom.cpython-38.pyc` & `workadays-2023.7.20/workadays/__pycache__/united_kingdom.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `workadays-2023.5.25/workadays/__pycache__/united_states.cpython-38.pyc` & `workadays-2023.7.20/workadays/__pycache__/united_states.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `workadays-2023.5.25/workadays/__pycache__/workdays.cpython-38.pyc` & `workadays-2023.7.20/workadays/__pycache__/workdays.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `workadays-2023.5.25/workadays/__pycache__/workdays_tests.cpython-38.pyc` & `workadays-2023.7.20/workadays/__pycache__/workdays_tests.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `workadays-2023.5.25/workadays/brazil.py` & `workadays-2023.7.20/workadays/brazil.py`

 * *Files identical despite different names*

### Comparing `workadays-2023.5.25/workadays/holiday_base.py` & `workadays-2023.7.20/workadays/holiday_base.py`

 * *Files identical despite different names*

### Comparing `workadays-2023.5.25/workadays/holidays.py` & `workadays-2023.7.20/workadays/holidays.py`

 * *Files identical despite different names*

### Comparing `workadays-2023.5.25/workadays/luxembourg.py` & `workadays-2023.7.20/workadays/luxembourg.py`

 * *Files identical despite different names*

### Comparing `workadays-2023.5.25/workadays/united_kingdom.py` & `workadays-2023.7.20/workadays/united_kingdom.py`

 * *Files identical despite different names*

### Comparing `workadays-2023.5.25/workadays/united_states.py` & `workadays-2023.7.20/workadays/united_states.py`

 * *Files identical despite different names*

### Comparing `workadays-2023.5.25/workadays/workdays.py` & `workadays-2023.7.20/workadays/workdays.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         holidays = get_holidays(years=years, expand=expand, observed=observed,
                                 country=country, prov=prov, state=state)
 
     # Diferença de dias corridos
     ndc = days(start_date, end_date)
     ndu = ndc   # Contador de dias úteis
 
-    for d in range(1, ndc):
+    for d in range(0, ndc+1):
         dt_aux = start_date + dt.timedelta(d)
         ndu -= 1 if is_weekend(dt_aux) or dt_aux in holidays else 0
 
     return ndu * (-1 if inverte_sinal else 1)
 
 
 # É ano bissexto
```

### Comparing `workadays-2023.5.25/workadays/workdays_tests.py` & `workadays-2023.7.20/workadays/workdays_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,20 @@
 
 import os
 import datetime as dt
 from workadays import workdays as wd
 
 
 def exec_tests():
-    dt_ini = dt.date(2020, 12, 25)
-    dt_fim = dt.date(2026, 12, 25)
+    dt_fim = dt.date(2021, 5, 1)
+    for dia in range(1, 31):
+        print(dt.date(2021, 4, dia), wd.networkdays(dt.date(2021, 4, dia), dt_fim))
+
+    dt_ini = dt.date(2021, 4, 11)
+    dt_fim = dt.date(2021, 4, 30)
     print(wd.networkdays(dt_ini, dt_fim))
 
     dt_ini = dt.date(2023, 5, 22)
     print(wd.workdays(dt_ini, 2520))
 
     dt_ini = dt.date(2023, 5, 22)
     data_hora = dt.datetime.combine(dt_ini, dt.time())
```

### Comparing `workadays-2023.5.25/workadays.egg-info/PKG-INFO` & `workadays-2023.7.20/workadays.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workadays
-Version: 2023.5.25
+Version: 2023.7.20
 Summary: Calendário de dias úteis, dias corridos e dias 360 (30/360).
 Home-page: https://github.com/mfhorita
 Author: Marcelo Horita
 Author-email: mfhorita@gmail.com.br
 License: MIT License
 Keywords: workdays workadays feriados holidays diasuteis uteis,dias360,days360,days
 Classifier: License :: Freeware
```

### Comparing `workadays-2023.5.25/workadays.egg-info/SOURCES.txt` & `workadays-2023.7.20/workadays.egg-info/SOURCES.txt`

 * *Files identical despite different names*

