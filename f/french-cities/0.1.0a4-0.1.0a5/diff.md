# Comparing `tmp/french_cities-0.1.0a4.tar.gz` & `tmp/french_cities-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "french_cities-0.1.0a4.tar", max compression
+gzip compressed data, was "french_cities-0.1.0a5.tar", max compression
```

## Comparing `french_cities-0.1.0a4.tar` & `french_cities-0.1.0a5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      520 2023-07-20 15:31:44.641685 french_cities-0.1.0a4/french_cities/__init__.py
--rw-r--r--   0        0        0    20106 2023-07-20 15:30:53.459607 french_cities-0.1.0a4/french_cities/city_finder.py
--rw-r--r--   0        0        0     4654 2023-07-17 15:18:48.886858 french_cities-0.1.0a4/french_cities/departement_finder.py
--rw-r--r--   0        0        0      335 2023-07-17 15:15:52.270285 french_cities-0.1.0a4/french_cities/utils.py
--rw-r--r--   0        0        0     7791 2023-07-20 14:20:02.786838 french_cities-0.1.0a4/french_cities/vintage.py
--rw-r--r--   0        0        0     1235 2023-07-20 15:31:47.476493 french_cities-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0     8785 2023-07-20 12:28:33.096467 french_cities-0.1.0a4/README.fr.md
--rw-r--r--   0        0        0     7355 2023-07-20 12:27:35.807255 french_cities-0.1.0a4/README.md
--rw-r--r--   0        0        0    17157 1970-01-01 00:00:00.000000 french_cities-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0      349 2023-07-21 09:11:11.383937 french_cities-0.1.0a5/french_cities/__init__.py
+-rw-r--r--   0        0        0    19353 2023-07-21 09:20:08.502684 french_cities-0.1.0a5/french_cities/city_finder.py
+-rw-r--r--   0        0        0     4654 2023-07-17 15:18:48.886858 french_cities-0.1.0a5/french_cities/departement_finder.py
+-rw-r--r--   0        0        0      335 2023-07-17 15:15:52.270285 french_cities-0.1.0a5/french_cities/utils.py
+-rw-r--r--   0        0        0     7791 2023-07-20 14:20:02.786838 french_cities-0.1.0a5/french_cities/vintage.py
+-rw-r--r--   0        0        0     1235 2023-07-21 09:11:19.186649 french_cities-0.1.0a5/pyproject.toml
+-rw-r--r--   0        0        0     8785 2023-07-20 12:28:33.096467 french_cities-0.1.0a5/README.fr.md
+-rw-r--r--   0        0        0     7355 2023-07-20 12:27:35.807255 french_cities-0.1.0a5/README.md
+-rw-r--r--   0        0        0    17157 1970-01-01 00:00:00.000000 french_cities-0.1.0a5/PKG-INFO
```

### Comparing `french_cities-0.1.0a4/french_cities/city_finder.py` & `french_cities-0.1.0a5/french_cities/city_finder.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,108 +6,97 @@
 import io
 import logging
 from requests_cache import CachedSession
 from requests import Session
 from rapidfuzz import fuzz
 from unidecode import unidecode
 from pynsee.geodata import get_geodata
+from pynsee.localdata import get_area_list
 import geopandas as gpd
 from pyproj import Transformer
 from datetime import date, timedelta
 from typing import Union
 import numpy as np
 from pebble import ThreadPool
 from tqdm import tqdm
 
 from french_cities.vintage import set_vintage
 from french_cities.departement_finder import find_departements
 from french_cities.utils import init_pynsee
-from french_cities import LAST_INSEE_HISTO_CITIES
 
 
 logger = logging.getLogger(__name__)
 
 
-def _get_old_cities_names(
-    year: str,
-    look_for: pd.DataFrame,
-    alias: str,
-    session: Session = None,
-    last_insee_histo_cities: str = LAST_INSEE_HISTO_CITIES,
+def _fuzzy_match_cities_names(
+    year: str, look_for: pd.DataFrame, alias: str
 ) -> pd.DataFrame:
     """
-    Get old city names directly from INSEE's website (hardcoded URL to update
-    annually in french_cities.__init__) and use fuzzy matching inside the same
-    departement to find best candidates.
+    Use fuzzy matching to retrieve cities from their names to find best
+    candidates.
 
     Parameters
     ----------
     year : str
         Desired vintage ("last" or castable to int)
     look_for : pd.DataFrame
         DataFrame cities (expected columns are "city_cleaned" & "dep") we are
         trying to find a match to
     alias : str
         field to use to store the positive matches' codes into the returned
         datafram
-    session : Session, optional
-        Requests Session to use for web queries to APIs. Note that pynsee
-        (used under the hood for geolocation recognition) uses it's own
-        session. The default is None (and will use a CachedSession with
-        **NO** expiration retrieving the INSEE's complete file)
-    last_insee_histo_cities : str, optional
-        Path to INSEE's "all cities since 1943" file.
-        Defaults to french_cities.LAST_INSEE_HISTO_CITIES
-        Currently found here:
-            https://www.insee.fr/fr/information/6800675#communes_1943
 
     Returns
     -------
     match : pd.DataFrame
         DataFrame of positive matches (ie look_for + one mor column under the
         label `alias`)
 
     """
-    if not session:
-        session = CachedSession(allowable_methods=("GET", "POST"))
-
-    r = session.get(last_insee_histo_cities)
-    obj = io.BytesIO(r.content)
-    df = pd.read_csv(obj)
+    init_pynsee()
 
-    ix = df[df.DATE_FIN.isnull() == False].index
-    df = df.loc[ix, ["NCC", "COM"]].reset_index(drop=True)
-    df = df.drop_duplicates("NCC")
+    df = get_area_list("communes", date="*")
+    df["TITLE_SHORT"] = (
+        df["TITLE_SHORT"]
+        .str.upper()
+        .apply(unidecode)
+        .str.split(r"\W+")
+        .str.join(" ")
+        .str.strip(" ")
+    )
+    df = df.loc[:, ["TITLE_SHORT", "CODE"]]
 
-    df = find_departements(df, source="COM", alias="dep", type_code="insee")
+    df = find_departements(df, source="CODE", alias="dep", type_code="insee")
+    df = df.drop_duplicates(["TITLE_SHORT", "dep"])
+    df = df.reset_index(drop=False)
 
     # fuzzy matching df / look_for
-    match = look_for.merge(df, on="dep", how="inner")
-    match["fuzzy_match"] = match[["city_cleaned", "NCC"]].apply(
+    match_ = look_for.merge(df, on="dep", how="inner")
+    match_["fuzzy_match"] = match_[["city_cleaned", "TITLE_SHORT"]].apply(
         lambda xy: fuzz.token_set_ratio(*xy), axis=1
     )
 
-    ix = match[match.fuzzy_match > 80].index
-    match = match.loc[ix].drop("fuzzy_match", axis=1)
+    ix = match_[match_.fuzzy_match > 80].index
+    match_ = match_.loc[ix].drop("fuzzy_match", axis=1)
 
     # Keep matches only if there is no ambiguity
-    match = match.drop_duplicates("city_cleaned", keep=False)
+    match_ = match_.drop_duplicates("city_cleaned", keep=False)
 
     try:
         year = int(year)
     except ValueError:
         year = date.today().year
-    match = set_vintage(match, year, "COM")
-    match = look_for.merge(
-        match[["city_cleaned", "dep", "COM"]],
+    match_ = set_vintage(match_, year, "CODE")
+    match_ = look_for.merge(
+        match_[["city_cleaned", "dep", "CODE"]],
         on=["city_cleaned", "dep"],
         how="left",
     )
-    match = match.rename({"COM": alias}, axis=1)
-    return match
+    match_ = match_.rename({"CODE": alias}, axis=1)
+    return match_
 
 
 def _find_from_geoloc(
     epsg: int,
     df: pd.DataFrame,
     year: str = "last",
     x: str = "x",
@@ -543,17 +532,15 @@
     )
 
     # Where still no results, check directly from INSEE's website for obsolete
     # cities (using dep & city)
     ix = df[df[field_output].isnull()].index
     if len(ix) > 0:
         missing = df.loc[ix, [dep, "city_cleaned"]]
-        missing = _get_old_cities_names(
-            year, missing, "candidat_missing", session
-        )
+        missing = _fuzzy_match_cities_names(year, missing, "candidat_missing")
         df = df.merge(missing, on=[dep, "city_cleaned"], how="left")
 
         candidats = [field_output, "candidat_missing"]
         df[field_output] = combine(df, candidats)
         df = df.drop("candidat_missing", axis=1)
 
     df = df.drop("city_cleaned", axis=1)
```

### Comparing `french_cities-0.1.0a4/french_cities/departement_finder.py` & `french_cities-0.1.0a5/french_cities/departement_finder.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.0a4/french_cities/vintage.py` & `french_cities-0.1.0a5/french_cities/vintage.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.0a4/pyproject.toml` & `french_cities-0.1.0a5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "french-cities"
-version = "0.1.0a4"
+version = "0.1.0a5"
 description = "Toolbox on french cities: set vintage, find departments, find cities..."
 authors = ["thomas.grandjean <thomas.grandjean@developpement-durable.gouv.fr>"]
 license = "etalab-2.0"
 readme = ["README.md", "README.fr.md"]
 homepage = "https://github.com/tgrandje/french-cities/"
 repository = "https://github.com/tgrandje/french-cities/"
 documentation = "https://github.com/tgrandje/french-cities/"
```

### Comparing `french_cities-0.1.0a4/README.fr.md` & `french_cities-0.1.0a5/README.fr.md`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.0a4/README.md` & `french_cities-0.1.0a5/README.md`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.0a4/PKG-INFO` & `french_cities-0.1.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: french-cities
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: Toolbox on french cities: set vintage, find departments, find cities...
 Home-page: https://github.com/tgrandje/french-cities/
 License: etalab-2.0
 Keywords: france,cities
 Author: thomas.grandjean
 Author-email: thomas.grandjean@developpement-durable.gouv.fr
 Requires-Python: >=3.8,<4.0
```

