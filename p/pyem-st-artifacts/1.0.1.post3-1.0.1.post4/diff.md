# Comparing `tmp/pyem_st_artifacts-1.0.1.post3.tar.gz` & `tmp/pyem_st_artifacts-1.0.1.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyem_st_artifacts-1.0.1.post3.tar", last modified: Wed Jul 12 15:47:14 2023, max compression
+gzip compressed data, was "dist\pyem_st_artifacts-1.0.1.post4.tar", last modified: Fri Jul 21 12:45:41 2023, max compression
```

## Comparing `pyem_st_artifacts-1.0.1.post3.tar` & `pyem_st_artifacts-1.0.1.post4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/
--rw-rw-rw-   0        0        0     1090 2023-04-19 10:44:40.000000 pyem_st_artifacts-1.0.1.post3/LICENSE
--rw-rw-rw-   0        0        0     9699 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/PKG-INFO
--rw-rw-rw-   0        0        0     9145 2023-07-12 15:47:03.000000 pyem_st_artifacts-1.0.1.post3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/
--rw-rw-rw-   0        0        0        0 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/__init__.py
--rw-rw-rw-   0        0        0    23999 2023-07-12 15:29:15.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/emotional_math.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/
-drwxrwxrwx   0        0        0        0 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x64/
--rw-rw-rw-   0        0        0    73216 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x64/artifacts-x64.dll
--rw-rw-rw-   0        0        0   174080 2023-06-07 09:52:32.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x64/em_st_artifacts-x64.dll
--rw-rw-rw-   0        0        0   320512 2023-02-09 11:55:16.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x64/filters.dll
-drwxrwxrwx   0        0        0        0 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x86/
--rw-rw-rw-   0        0        0    56320 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x86/artifacts-x86.dll
--rw-rw-rw-   0        0        0   133632 2023-06-07 09:53:04.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x86/em_st_artifacts-x86.dll
--rw-rw-rw-   0        0        0   268288 2023-02-09 11:55:16.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x86/filters.dll
--rw-rw-rw-   0        0        0     3448 2023-06-07 13:09:40.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/sample.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/utils/
--rw-rw-rw-   0        0        0      193 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/utils/EmotionalMathException.py
--rw-rw-rw-   0        0        0        0 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/utils/__init__.py
--rw-rw-rw-   0        0        0      944 2023-06-06 14:04:47.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/utils/lib_settings.py
--rw-rw-rw-   0        0        0      655 2023-06-06 13:59:02.000000 pyem_st_artifacts-1.0.1.post3/em_st_artifacts/utils/support_classes.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/pyem_st_artifacts.egg-info/
--rw-rw-rw-   0        0        0     9699 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/pyem_st_artifacts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/pyem_st_artifacts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/pyem_st_artifacts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/pyem_st_artifacts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 15:47:14.000000 pyem_st_artifacts-1.0.1.post3/setup.cfg
--rw-rw-rw-   0        0        0     1414 2023-07-12 15:43:13.000000 pyem_st_artifacts-1.0.1.post3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/
+-rw-rw-rw-   0        0        0     1090 2023-04-19 10:44:40.000000 pyem_st_artifacts-1.0.1.post4/LICENSE
+-rw-rw-rw-   0        0        0     9699 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/PKG-INFO
+-rw-rw-rw-   0        0        0     9145 2023-07-12 15:47:03.000000 pyem_st_artifacts-1.0.1.post4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/
+-rw-rw-rw-   0        0        0        0 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/__init__.py
+-rw-rw-rw-   0        0        0    24174 2023-07-21 12:39:50.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/emotional_math.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/
+drwxrwxrwx   0        0        0        0 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x64/
+-rw-rw-rw-   0        0        0    73216 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x64/artifacts-x64.dll
+-rw-rw-rw-   0        0        0   174080 2023-06-07 09:52:32.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x64/em_st_artifacts-x64.dll
+-rw-rw-rw-   0        0        0   320512 2023-02-09 11:55:16.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x64/filters.dll
+drwxrwxrwx   0        0        0        0 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x86/
+-rw-rw-rw-   0        0        0    56320 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x86/artifacts-x86.dll
+-rw-rw-rw-   0        0        0   133632 2023-06-07 09:53:04.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x86/em_st_artifacts-x86.dll
+-rw-rw-rw-   0        0        0   268288 2023-02-09 11:55:16.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x86/filters.dll
+-rw-rw-rw-   0        0        0     3448 2023-06-07 13:09:40.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/sample.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/utils/
+-rw-rw-rw-   0        0        0      193 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/utils/EmotionalMathException.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/utils/__init__.py
+-rw-rw-rw-   0        0        0      945 2023-07-21 12:40:14.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/utils/lib_settings.py
+-rw-rw-rw-   0        0        0      655 2023-06-06 13:59:02.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/utils/support_classes.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/pyem_st_artifacts.egg-info/
+-rw-rw-rw-   0        0        0     9699 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/pyem_st_artifacts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/pyem_st_artifacts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/pyem_st_artifacts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/pyem_st_artifacts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/setup.cfg
+-rw-rw-rw-   0        0        0     1414 2023-07-21 12:41:12.000000 pyem_st_artifacts-1.0.1.post4/setup.py
```

### Comparing `pyem_st_artifacts-1.0.1.post3/LICENSE` & `pyem_st_artifacts-1.0.1.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post3/PKG-INFO` & `pyem_st_artifacts-1.0.1.post4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyem_st_artifacts
-Version: 1.0.1.post3
+Version: 1.0.1.post4
 Summary: Python wrapper for Emotions library
 Home-page: https://gitlab.com/neurosdk2/neurosamples/-/tree/main/python
 Author: Brainbit Inc.
 Author-email: support@brainbit.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyem_st_artifacts-1.0.1.post3/README.md` & `pyem_st_artifacts-1.0.1.post4/README.md`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post3/em_st_artifacts/emotional_math.py` & `pyem_st_artifacts-1.0.1.post4/em_st_artifacts/emotional_math.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,17 @@
                                                         mls.bipolar_mode,
                                                         mls.channels_number,
                                                         mls.channel_for_analysis)
 
         native_art_setting = self._NativeArtifactDetectSetting(ads.art_bord,
                                                                ads.allowed_percent_artpoints,
                                                                ads.raw_betap_limit,
+                                                               ads.total_pow_border,
                                                                ads.global_artwin_sec,
+                                                               ads.spect_art_by_totalp,
                                                                ads.hanning_win_spectrum,
                                                                ads.hamming_win_spectrum,
                                                                ads.num_wins_for_quality_avg)
 
         native_short_art_setting = self._NativeShortArtifactDetectSetting(sads.ampl_art_detect_win_size,
                                                                           sads.ampl_art_zerod_area,
                                                                           sads.ampl_art_extremum_border)
```

### Comparing `pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x64/artifacts-x64.dll` & `pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x64/artifacts-x64.dll`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x64/em_st_artifacts-x64.dll` & `pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x64/em_st_artifacts-x64.dll`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x64/filters.dll` & `pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x64/filters.dll`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x86/artifacts-x86.dll` & `pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x86/artifacts-x86.dll`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x86/em_st_artifacts-x86.dll` & `pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x86/em_st_artifacts-x86.dll`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post3/em_st_artifacts/libs/x86/filters.dll` & `pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x86/filters.dll`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post3/em_st_artifacts/sample.py` & `pyem_st_artifacts-1.0.1.post4/em_st_artifacts/sample.py`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post3/em_st_artifacts/utils/lib_settings.py` & `pyem_st_artifacts-1.0.1.post4/em_st_artifacts/utils/lib_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 @dataclass
 class ArtifactDetectSetting:
     art_bord: int = 70
     allowed_percent_artpoints: int = 50
     raw_betap_limit: int = 800000
-    total_pow_border: int = 3 * 1e7
+    total_pow_border: int = 30000000
     global_artwin_sec: int = 4
     spect_art_by_totalp: int = False
     hanning_win_spectrum: int = False
     hamming_win_spectrum: int = False
     num_wins_for_quality_avg: int = 100
```

### Comparing `pyem_st_artifacts-1.0.1.post3/em_st_artifacts/utils/support_classes.py` & `pyem_st_artifacts-1.0.1.post4/em_st_artifacts/utils/support_classes.py`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post3/pyem_st_artifacts.egg-info/PKG-INFO` & `pyem_st_artifacts-1.0.1.post4/pyem_st_artifacts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyem-st-artifacts
-Version: 1.0.1.post3
+Version: 1.0.1.post4
 Summary: Python wrapper for Emotions library
 Home-page: https://gitlab.com/neurosdk2/neurosamples/-/tree/main/python
 Author: Brainbit Inc.
 Author-email: support@brainbit.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyem_st_artifacts-1.0.1.post3/pyem_st_artifacts.egg-info/SOURCES.txt` & `pyem_st_artifacts-1.0.1.post4/pyem_st_artifacts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post3/setup.py` & `pyem_st_artifacts-1.0.1.post4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pyem_st_artifacts',
-    version='1.0.1.post3',
+    version='1.0.1.post4',
     py_modules=[
         'em_st_artifacts.emotional_math',
         'em_st_artifacts.utils.lib_settings',
         'em_st_artifacts.utils.support_classes',
         'em_st_artifacts.utils.EmotionalMathException'],
     packages=['em_st_artifacts'],
     url='https://gitlab.com/neurosdk2/neurosamples/-/tree/main/python',
```

