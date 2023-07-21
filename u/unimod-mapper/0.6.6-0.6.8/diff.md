# Comparing `tmp/unimod_mapper-0.6.6-py3-none-any.whl.zip` & `tmp/unimod_mapper-0.6.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 12023 bytes, number of entries: 8
--rw-r--r--  2.0 unx       40 b- defN 22-May-27 12:50 unimod_mapper/__init__.py
--rw-r--r--  2.0 unx    49866 b- defN 22-May-27 12:50 unimod_mapper/unimod_mapper.py
--rw-r--r--  2.0 unx        6 b- defN 22-May-27 12:50 unimod_mapper/version.txt
--rw-r--r--  2.0 unx     1088 b- defN 22-May-27 12:50 unimod_mapper-0.6.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     1301 b- defN 22-May-27 12:50 unimod_mapper-0.6.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-May-27 12:50 unimod_mapper-0.6.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 22-May-27 12:50 unimod_mapper-0.6.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      663 b- defN 22-May-27 12:50 unimod_mapper-0.6.6.dist-info/RECORD
-8 files, 53070 bytes uncompressed, 10855 bytes compressed:  79.5%
+Zip file size: 12299 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       40 b- defN 23-Jul-21 12:28 unimod_mapper/__init__.py
+-rw-r--r--  2.0 unx    50891 b- defN 23-Jul-21 12:28 unimod_mapper/unimod_mapper.py
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-21 12:28 unimod_mapper/version.txt
+-rw-r--r--  2.0 unx     1088 b- defN 23-Jul-21 12:29 unimod_mapper-0.6.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1300 b- defN 23-Jul-21 12:29 unimod_mapper-0.6.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 12:29 unimod_mapper-0.6.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-21 12:29 unimod_mapper-0.6.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      663 b- defN 23-Jul-21 12:29 unimod_mapper-0.6.8.dist-info/RECORD
+8 files, 54094 bytes uncompressed, 11131 bytes compressed:  79.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: unimod_mapper/unimod_mapper.py
 Comment: 
 
 Filename: unimod_mapper/version.txt
 Comment: 
 
-Filename: unimod_mapper-0.6.6.dist-info/LICENSE
+Filename: unimod_mapper-0.6.8.dist-info/LICENSE
 Comment: 
 
-Filename: unimod_mapper-0.6.6.dist-info/METADATA
+Filename: unimod_mapper-0.6.8.dist-info/METADATA
 Comment: 
 
-Filename: unimod_mapper-0.6.6.dist-info/WHEEL
+Filename: unimod_mapper-0.6.8.dist-info/WHEEL
 Comment: 
 
-Filename: unimod_mapper-0.6.6.dist-info/top_level.txt
+Filename: unimod_mapper-0.6.8.dist-info/top_level.txt
 Comment: 
 
-Filename: unimod_mapper-0.6.6.dist-info/RECORD
+Filename: unimod_mapper-0.6.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## unimod_mapper/unimod_mapper.py

```diff
@@ -364,15 +364,14 @@
         Returns:
             list: list of tuples with combined and single masses
         """
         mass_list = []
         for combo in itertools.combinations_with_replacement(
             self.df[["mono_mass", "Name"]].drop_duplicates().to_numpy(), 2
         ):
-
             combo_mass = np.sum(np.fromiter((c[0] for c in combo), float))
             combo_name = [c[1] for c in combo]
             mass_list.append((combo_mass, combo_name))
         return sorted(mass_list)
 
     def _extract_elements(self, element):
         """Extract xml elements with the name 'element'.
@@ -446,15 +445,14 @@
                         neutral_loss_mass = 0
                         if len(element) > 0:
                             for sub_element in element.iter():
                                 if (
                                     sub_element.tag.endswith("}NeutralLoss")
                                     and len(sub_element) > 0
                                 ):
-
                                     neutral_loss_elements = self._extract_elements(
                                         sub_element
                                     )
                                     neutral_loss_mass = float(
                                         sub_element.attrib["mono_mass"]
                                     )
                         tmp["specificity"].append(
@@ -1169,14 +1167,39 @@
         self._reparseXML(xml_file_list=xml_list)
         return
 
     def _reparseXML(self, xml_file_list=[]):
         self._data_list = self._parseXML(xml_file_list=xml_file_list)
         self._mapper = self._initialize_mapper()
 
+    def read_mapped_mods_as_df(self, mapped_mods):
+        """
+        Read in results (rdict) of the map_mods function and turn them into a pandas data frame.
+        This allows for using the mapping functions without requiring modifications to be part
+        of the xml files.
+
+        Args:
+            mapped_mods (dict): dictionary that is returned by the mapped_mods function
+
+        Returns:
+            df (pandas data frame): pandas data frame containing all modifications used as input.
+                                    Importantly, this df replaces self._df as well!
+        """
+        mod_list = []
+        for mod_type in ["fix", "opt"]:
+            for m in mapped_mods[mod_type]:
+                mod_list.append(m)
+        df = pd.DataFrame(mod_list)
+        df = df.rename(columns={"id": "Accession"})
+        df = df.rename(columns={"mass": "mono_mass"})
+        df = df.rename(columns={"composition": "elements"})
+        df = df.rename(columns={"name": "Name"})
+        self._df = df
+        return df
+
     def map_mods(self, mod_list):
         """
         Maps modifications defined in params["modification"] using unimods or user-defined modifications. Using the
         dict format for the mods, the dict can be adjusted depending on the purpose of
         the mapping. Moreover, it can have the minimal amount of items (i.e.: engine-specific ones).
         At the end the mapped values will be updated to the original dict.
         Note:
@@ -1205,15 +1228,14 @@
                 }
             ]
 
         """
 
         rdict = {"fix": [], "opt": []}
         for index, mod in enumerate(mod_list):
-
             # Generate a default mod_dict with minimal required keys
 
             mod_dict = {
                 "aa": None,
                 "type": None,
                 "position": None,
                 "name": None,
@@ -1322,15 +1344,14 @@
                     )
                     chemical_composition = ChemicalComposition()
                     chemical_composition.use(formula=cc_string)
                     mass = chemical_composition.mass()
 
             neutral_loss = []
             if mod_dict["neutral_loss"] == "unimod":
-
                 for nl_item in self.name_to_neutral_loss(unimod_name):
                     if nl_item[0] == mod_dict["aa"]:
                         neutral_loss.append(nl_item[1])
             else:
                 neutral_loss.append(mod_dict["neutral_loss"])
 
             mapped_dict = {
```

## unimod_mapper/version.txt

```diff
@@ -1 +1 @@
-0.6.6
+0.6.8
```

## Comparing `unimod_mapper-0.6.6.dist-info/LICENSE` & `unimod_mapper-0.6.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `unimod_mapper-0.6.6.dist-info/METADATA` & `unimod_mapper-0.6.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unimod-mapper
-Version: 0.6.6
+Version: 0.6.8
 Summary: unimod_mapper
 Home-page: https://github.com/computational-ms/unimod-mapper
 Author: Christian Fufezan, Manuel Kösters, Johannes Leufken, Stefan Schulze
 Author-email: ursgal.team@gmail.com
 License: MIT
 Platform: Any that supports python 3.7
 Classifier: Development Status :: 4 - Beta
@@ -28,8 +28,7 @@
 Requires-Dist: requests
 Requires-Dist: loguru
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: chemical-composition
 
 Unimod Mapper for Proteomics Tools
-
```

## Comparing `unimod_mapper-0.6.6.dist-info/RECORD` & `unimod_mapper-0.6.8.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 unimod_mapper/__init__.py,sha256=1AtvsTpzn5w1FRZEHWAPKeWM-w7VPVoBa5TmrR66q7M,40
-unimod_mapper/unimod_mapper.py,sha256=mBWv9FZ-zTTG_TCff5ZgA_rQnJ8124ge6h4oQY4Ty6A,49866
-unimod_mapper/version.txt,sha256=mG2VqS0VOK16dV5ndue_YukObeucJsWuzEDjoDRtruY,6
-unimod_mapper-0.6.6.dist-info/LICENSE,sha256=034M0-369w46yGNUZ3w7VrBOrLdflqy5pA1qA9s_v9E,1088
-unimod_mapper-0.6.6.dist-info/METADATA,sha256=_MoZec6kWkRwfJf3WzCGc55YfwdT3GDHvVjfE4zTEbY,1301
-unimod_mapper-0.6.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-unimod_mapper-0.6.6.dist-info/top_level.txt,sha256=jrtWb2jaqwk_GlIPNLPXWDq3uH_UZejh-bcYAGIraSw,14
-unimod_mapper-0.6.6.dist-info/RECORD,,
+unimod_mapper/unimod_mapper.py,sha256=9fpXEKTyPufjNKn0SQCVKeKKM8VKUcNl_NOawAv10qA,50891
+unimod_mapper/version.txt,sha256=eYqNGfKt8g-HEbPJO2sxI2mxHXp-cEP-UzwTwmiseL4,6
+unimod_mapper-0.6.8.dist-info/LICENSE,sha256=034M0-369w46yGNUZ3w7VrBOrLdflqy5pA1qA9s_v9E,1088
+unimod_mapper-0.6.8.dist-info/METADATA,sha256=p3BOhm-7U_-2fmAIRUCdplgIZpNz3EVa8RyHgrSDRnQ,1300
+unimod_mapper-0.6.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+unimod_mapper-0.6.8.dist-info/top_level.txt,sha256=jrtWb2jaqwk_GlIPNLPXWDq3uH_UZejh-bcYAGIraSw,14
+unimod_mapper-0.6.8.dist-info/RECORD,,
```

