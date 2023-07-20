# Comparing `tmp/dotscanner-1.3.4.tar.gz` & `tmp/dotscanner-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dotscanner-1.3.4.tar", last modified: Wed Jun  7 06:19:21 2023, max compression
+gzip compressed data, was "dist/dotscanner-1.3.5.tar", last modified: Thu Jul 20 22:24:37 2023, max compression
```

## Comparing `dotscanner-1.3.4.tar` & `dotscanner-1.3.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 06:19:21.222840 dotscanner-1.3.4/
--rw-r--r--   0 holly      (501) staff       (20)     1103 2023-06-05 02:24:39.000000 dotscanner-1.3.4/LICENSE
--rw-r--r--   0 holly      (501) staff       (20)    13417 2023-06-07 06:19:21.222635 dotscanner-1.3.4/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)    12762 2023-06-07 06:18:08.000000 dotscanner-1.3.4/README.md
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 06:19:21.217968 dotscanner-1.3.4/dotscanner/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.4/dotscanner/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     2755 2023-06-07 06:04:06.000000 dotscanner-1.3.4/dotscanner/__main__.py
--rw-r--r--   0 holly      (501) staff       (20)    10277 2023-06-06 23:47:07.000000 dotscanner-1.3.4/dotscanner/dataprocessing.py
--rw-r--r--   0 holly      (501) staff       (20)    10147 2023-06-07 06:04:08.000000 dotscanner-1.3.4/dotscanner/density.py
--rw-r--r--   0 holly      (501) staff       (20)     6212 2023-06-07 06:04:08.000000 dotscanner-1.3.4/dotscanner/files.py
--rw-r--r--   0 holly      (501) staff       (20)    10595 2023-06-07 06:04:07.000000 dotscanner-1.3.4/dotscanner/lifetime.py
--rw-r--r--   0 holly      (501) staff       (20)     6692 2023-06-06 23:47:10.000000 dotscanner-1.3.4/dotscanner/strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 06:19:21.219983 dotscanner-1.3.4/dotscanner/ui/
--rw-r--r--   0 holly      (501) staff       (20)     5179 2023-06-06 23:47:11.000000 dotscanner-1.3.4/dotscanner/ui/DefaultUserSettingsEditor.py
--rw-r--r--   0 holly      (501) staff       (20)     1858 2023-06-06 23:47:12.000000 dotscanner-1.3.4/dotscanner/ui/DialogWindow.py
--rw-r--r--   0 holly      (501) staff       (20)     3510 2023-06-07 03:30:32.000000 dotscanner-1.3.4/dotscanner/ui/MicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     5764 2023-06-07 06:04:13.000000 dotscanner-1.3.4/dotscanner/ui/RegionSelector.py
--rw-r--r--   0 holly      (501) staff       (20)    16392 2023-06-07 06:12:10.000000 dotscanner-1.3.4/dotscanner/ui/ThresholdAdjuster.py
--rw-r--r--   0 holly      (501) staff       (20)    15070 2023-06-07 06:04:14.000000 dotscanner-1.3.4/dotscanner/ui/UserSettings.py
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.4/dotscanner/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     3097 2023-06-06 23:47:14.000000 dotscanner-1.3.4/dotscanner/ui/window.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 06:19:21.218858 dotscanner-1.3.4/dotscanner.egg-info/
--rw-r--r--   0 holly      (501) staff       (20)    13417 2023-06-07 06:19:21.000000 dotscanner-1.3.4/dotscanner.egg-info/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)     1050 2023-06-07 06:19:21.000000 dotscanner-1.3.4/dotscanner.egg-info/SOURCES.txt
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-06-07 06:19:21.000000 dotscanner-1.3.4/dotscanner.egg-info/dependency_links.txt
--rw-r--r--   0 holly      (501) staff       (20)       56 2023-06-07 06:19:21.000000 dotscanner-1.3.4/dotscanner.egg-info/entry_points.txt
--rw-r--r--   0 holly      (501) staff       (20)       17 2023-06-07 06:19:21.000000 dotscanner-1.3.4/dotscanner.egg-info/requires.txt
--rw-r--r--   0 holly      (501) staff       (20)       26 2023-06-07 06:19:21.000000 dotscanner-1.3.4/dotscanner.egg-info/top_level.txt
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 06:19:21.220538 dotscanner-1.3.4/settings/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.4/settings/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     6219 2023-06-06 20:41:22.000000 dotscanner-1.3.4/settings/config.py
--rw-r--r--   0 holly      (501) staff       (20)    11284 2023-06-05 02:24:39.000000 dotscanner-1.3.4/settings/configmanagement.py
--rw-r--r--   0 holly      (501) staff       (20)       38 2023-06-07 06:19:21.222900 dotscanner-1.3.4/setup.cfg
--rw-r--r--   0 holly      (501) staff       (20)     1444 2023-06-07 06:19:20.000000 dotscanner-1.3.4/setup.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 06:19:21.221579 dotscanner-1.3.4/tests/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.4/tests/__init__.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 06:19:21.221739 dotscanner-1.3.4/tests/data/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.4/tests/data/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)    10018 2023-06-05 02:24:39.000000 dotscanner-1.3.4/tests/test_dataprocessing.py
--rw-r--r--   0 holly      (501) staff       (20)     5619 2023-06-07 06:18:09.000000 dotscanner-1.3.4/tests/test_density.py
--rw-r--r--   0 holly      (501) staff       (20)    13472 2023-06-07 06:04:11.000000 dotscanner-1.3.4/tests/test_files.py
--rw-r--r--   0 holly      (501) staff       (20)     6341 2023-06-07 06:18:10.000000 dotscanner-1.3.4/tests/test_fullAnalysis.py
--rw-r--r--   0 holly      (501) staff       (20)    10886 2023-06-05 02:24:39.000000 dotscanner-1.3.4/tests/test_lifetime.py
--rw-r--r--   0 holly      (501) staff       (20)     5740 2023-06-07 03:30:33.000000 dotscanner-1.3.4/tests/test_strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-06-07 06:19:21.222383 dotscanner-1.3.4/tests/ui/
--rw-r--r--   0 holly      (501) staff       (20)      487 2023-06-07 03:30:33.000000 dotscanner-1.3.4/tests/ui/FakeMicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     1086 2023-06-07 06:04:14.000000 dotscanner-1.3.4/tests/ui/FakeUserSettings.py
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.4/tests/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     4099 2023-06-07 03:02:28.000000 dotscanner-1.3.4/tests/ui/test_MicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     8287 2023-06-07 06:12:11.000000 dotscanner-1.3.4/tests/ui/test_ThresholdAdjuster.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-07-20 22:24:37.410915 dotscanner-1.3.5/
+-rw-r--r--   0 holly      (501) staff       (20)     1103 2023-06-05 02:24:39.000000 dotscanner-1.3.5/LICENSE
+-rw-r--r--   0 holly      (501) staff       (20)    13629 2023-07-20 22:24:37.410735 dotscanner-1.3.5/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)    12974 2023-07-20 22:19:47.000000 dotscanner-1.3.5/README.md
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-07-20 22:24:37.405744 dotscanner-1.3.5/dotscanner/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.5/dotscanner/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     2755 2023-06-07 06:04:06.000000 dotscanner-1.3.5/dotscanner/__main__.py
+-rw-r--r--   0 holly      (501) staff       (20)    10277 2023-06-06 23:47:07.000000 dotscanner-1.3.5/dotscanner/dataprocessing.py
+-rw-r--r--   0 holly      (501) staff       (20)    10147 2023-06-07 06:04:08.000000 dotscanner-1.3.5/dotscanner/density.py
+-rw-r--r--   0 holly      (501) staff       (20)     6462 2023-07-20 21:39:52.000000 dotscanner-1.3.5/dotscanner/files.py
+-rw-r--r--   0 holly      (501) staff       (20)    10595 2023-06-07 06:04:07.000000 dotscanner-1.3.5/dotscanner/lifetime.py
+-rw-r--r--   0 holly      (501) staff       (20)     6867 2023-07-20 21:46:19.000000 dotscanner-1.3.5/dotscanner/strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-07-20 22:24:37.408101 dotscanner-1.3.5/dotscanner/ui/
+-rw-r--r--   0 holly      (501) staff       (20)     5179 2023-06-06 23:47:11.000000 dotscanner-1.3.5/dotscanner/ui/DefaultUserSettingsEditor.py
+-rw-r--r--   0 holly      (501) staff       (20)     1858 2023-06-06 23:47:12.000000 dotscanner-1.3.5/dotscanner/ui/DialogWindow.py
+-rw-r--r--   0 holly      (501) staff       (20)     3510 2023-06-07 03:30:32.000000 dotscanner-1.3.5/dotscanner/ui/MicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     5764 2023-06-07 06:04:13.000000 dotscanner-1.3.5/dotscanner/ui/RegionSelector.py
+-rw-r--r--   0 holly      (501) staff       (20)    16392 2023-06-07 06:12:10.000000 dotscanner-1.3.5/dotscanner/ui/ThresholdAdjuster.py
+-rw-r--r--   0 holly      (501) staff       (20)    15478 2023-07-20 22:12:44.000000 dotscanner-1.3.5/dotscanner/ui/UserSettings.py
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.5/dotscanner/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     3097 2023-06-06 23:47:14.000000 dotscanner-1.3.5/dotscanner/ui/window.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-07-20 22:24:37.406952 dotscanner-1.3.5/dotscanner.egg-info/
+-rw-r--r--   0 holly      (501) staff       (20)    13629 2023-07-20 22:24:37.000000 dotscanner-1.3.5/dotscanner.egg-info/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)     1050 2023-07-20 22:24:37.000000 dotscanner-1.3.5/dotscanner.egg-info/SOURCES.txt
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-20 22:24:37.000000 dotscanner-1.3.5/dotscanner.egg-info/dependency_links.txt
+-rw-r--r--   0 holly      (501) staff       (20)       56 2023-07-20 22:24:37.000000 dotscanner-1.3.5/dotscanner.egg-info/entry_points.txt
+-rw-r--r--   0 holly      (501) staff       (20)       17 2023-07-20 22:24:37.000000 dotscanner-1.3.5/dotscanner.egg-info/requires.txt
+-rw-r--r--   0 holly      (501) staff       (20)       26 2023-07-20 22:24:37.000000 dotscanner-1.3.5/dotscanner.egg-info/top_level.txt
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-07-20 22:24:37.408502 dotscanner-1.3.5/settings/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.5/settings/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     6219 2023-06-06 20:41:22.000000 dotscanner-1.3.5/settings/config.py
+-rw-r--r--   0 holly      (501) staff       (20)    11284 2023-06-05 02:24:39.000000 dotscanner-1.3.5/settings/configmanagement.py
+-rw-r--r--   0 holly      (501) staff       (20)       38 2023-07-20 22:24:37.410982 dotscanner-1.3.5/setup.cfg
+-rw-r--r--   0 holly      (501) staff       (20)     1444 2023-07-20 22:24:37.000000 dotscanner-1.3.5/setup.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-07-20 22:24:37.409651 dotscanner-1.3.5/tests/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.5/tests/__init__.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-07-20 22:24:37.409787 dotscanner-1.3.5/tests/data/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.5/tests/data/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)    10018 2023-06-05 02:24:39.000000 dotscanner-1.3.5/tests/test_dataprocessing.py
+-rw-r--r--   0 holly      (501) staff       (20)     5619 2023-06-07 06:18:09.000000 dotscanner-1.3.5/tests/test_density.py
+-rw-r--r--   0 holly      (501) staff       (20)    14518 2023-07-20 21:50:56.000000 dotscanner-1.3.5/tests/test_files.py
+-rw-r--r--   0 holly      (501) staff       (20)     7470 2023-06-16 00:50:00.000000 dotscanner-1.3.5/tests/test_fullAnalysis.py
+-rw-r--r--   0 holly      (501) staff       (20)    10886 2023-06-05 02:24:39.000000 dotscanner-1.3.5/tests/test_lifetime.py
+-rw-r--r--   0 holly      (501) staff       (20)     6051 2023-07-20 21:53:10.000000 dotscanner-1.3.5/tests/test_strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-07-20 22:24:37.410476 dotscanner-1.3.5/tests/ui/
+-rw-r--r--   0 holly      (501) staff       (20)      487 2023-06-07 03:30:33.000000 dotscanner-1.3.5/tests/ui/FakeMicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     1086 2023-06-07 06:04:14.000000 dotscanner-1.3.5/tests/ui/FakeUserSettings.py
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.5/tests/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     4099 2023-06-07 03:02:28.000000 dotscanner-1.3.5/tests/ui/test_MicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     8287 2023-06-07 06:12:11.000000 dotscanner-1.3.5/tests/ui/test_ThresholdAdjuster.py
```

### Comparing `dotscanner-1.3.4/LICENSE` & `dotscanner-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.4/PKG-INFO` & `dotscanner-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotscanner
-Version: 1.3.4
+Version: 1.3.5
 Summary: A program designed for analysis of microscope imaging data
 Home-page: https://github.com/bdavis222/dotscanner
 Author: Holly Allen and Brian Davis
 Author-email: holly.allen@colorado.edu
 Project-URL: Bug Reports, https://github.com/bdavis222/dotscanner/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/dotscanner
@@ -101,15 +101,15 @@
 #### Skips allowed
 This sets the number of consecutive images that are allowed to be skipped in a lifetime calculation. This can be useful for dimmer dots where an image or two in a series are relatively out of focus, resulting in an unwanted non-detection for those frames. By increasing the number of skips allowed, these particles will be retained as long as they are back in focus and bright enough for detection in subsequent frames.
       
 #### Remove edge frames
 This dictates whether edge frames should be removed from a lifetime calculation. If a particle is detected in the first frame of an image, for example, it cannot be determined whether the particle existed before the first image was taken, so it might not make sense to include this in a lifetime calculation (and the same may also be true for particles in the last frame). If the number of skips allowed in the lifetime calculation is greater than zero, this will increase how many edge frames are removed from analysis.
 
 ## The Threshold Adjustment Window
-This window shows the image data with the dots and blobs identified, and features several button groups on the left sidebar:
+Clicking the **Next** button, or pressing the **return** key on the keyboard, from the Configurations Window saves the configuration settings selected by the user and advances to the Threshold Adjustment Window. This window shows the image data with the dots and blobs identified, and features several button groups on the left sidebar:
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/7.png)
 
 From top to bottom, these button groups perform the following actions:
 
 #### View
 These buttons allow four different viewing options: zooming in on the top left, top right, bottom left, bottom right, or zooming back out to show the full image. The user can also press the **spacebar** on the keyboard to cycle through these different views.
 
@@ -148,15 +148,15 @@
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
-* 1.3.4
+* 1.3.5
      * Bug fixes
 * 1.3.0
      * Added option to re-analyze data without redrawing regions
      * Added particle displacement tracking during lifetime measurement
      * Added histogram output for lifetimes measurements
 * 1.2.0
      * Added options for editing the configuration file
```

### Comparing `dotscanner-1.3.4/README.md` & `dotscanner-1.3.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 #### Skips allowed
 This sets the number of consecutive images that are allowed to be skipped in a lifetime calculation. This can be useful for dimmer dots where an image or two in a series are relatively out of focus, resulting in an unwanted non-detection for those frames. By increasing the number of skips allowed, these particles will be retained as long as they are back in focus and bright enough for detection in subsequent frames.
       
 #### Remove edge frames
 This dictates whether edge frames should be removed from a lifetime calculation. If a particle is detected in the first frame of an image, for example, it cannot be determined whether the particle existed before the first image was taken, so it might not make sense to include this in a lifetime calculation (and the same may also be true for particles in the last frame). If the number of skips allowed in the lifetime calculation is greater than zero, this will increase how many edge frames are removed from analysis.
 
 ## The Threshold Adjustment Window
-This window shows the image data with the dots and blobs identified, and features several button groups on the left sidebar:
+Clicking the **Next** button, or pressing the **return** key on the keyboard, from the Configurations Window saves the configuration settings selected by the user and advances to the Threshold Adjustment Window. This window shows the image data with the dots and blobs identified, and features several button groups on the left sidebar:
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/7.png)
 
 From top to bottom, these button groups perform the following actions:
 
 #### View
 These buttons allow four different viewing options: zooming in on the top left, top right, bottom left, bottom right, or zooming back out to show the full image. The user can also press the **spacebar** on the keyboard to cycle through these different views.
 
@@ -128,15 +128,15 @@
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
-* 1.3.4
+* 1.3.5
      * Bug fixes
 * 1.3.0
      * Added option to re-analyze data without redrawing regions
      * Added particle displacement tracking during lifetime measurement
      * Added histogram output for lifetimes measurements
 * 1.2.0
      * Added options for editing the configuration file
```

### Comparing `dotscanner-1.3.4/dotscanner/__main__.py` & `dotscanner-1.3.5/dotscanner/__main__.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.4/dotscanner/dataprocessing.py` & `dotscanner-1.3.5/dotscanner/dataprocessing.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.4/dotscanner/density.py` & `dotscanner-1.3.5/dotscanner/density.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.4/dotscanner/files.py` & `dotscanner-1.3.5/dotscanner/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -205,7 +205,15 @@
 	
 	figurePath = f"{directory}{figureDirectoryName}/"
 	
 	if not os.path.exists(figurePath):
 		os.mkdir(figurePath)
 	
 	return figurePath
+
+def getExtensionIndexFromDensityAnalysisFileLineArray(lineArray):
+	for index, element in enumerate(lineArray):
+		if "." in element:
+			periodIndex = element.find(".")
+			if not element[periodIndex + 1].isdigit():
+				return index
+	return -1
```

### Comparing `dotscanner-1.3.4/dotscanner/lifetime.py` & `dotscanner-1.3.5/dotscanner/lifetime.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.4/dotscanner/strings.py` & `dotscanner-1.3.5/dotscanner/strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,18 @@
 	return f"\nFile {filename} skipped"
 
 def invalidAnalysisFileWarning(filepath):
 	filename = filepath.split("/")[-1]
 	return f'\nInvalid analysis file selected: "{filename}". A valid file has a .txt extension \
 and contains density or lifetime data.'
 
+def invalidFilenameInDensityAnalysisFile(lineArray):
+	return f"Filename with valid extension not found in the following line in densities file:\n\
+{' '.join(lineArray)}"
+
 def lifetimeOutputFileHeader(microscopeImage, userSettings):
 	verticesStringList = []
 	for vertex in microscopeImage.polygon[:-1]:
 		y, x = vertex
 		verticesStringList.append(f"({x}, {y})")
 	verticesString = ", ".join(verticesStringList)
```

### Comparing `dotscanner-1.3.4/dotscanner/ui/DefaultUserSettingsEditor.py` & `dotscanner-1.3.5/dotscanner/ui/DefaultUserSettingsEditor.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.4/dotscanner/ui/DialogWindow.py` & `dotscanner-1.3.5/dotscanner/ui/DialogWindow.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.4/dotscanner/ui/MicroscopeImage.py` & `dotscanner-1.3.5/dotscanner/ui/MicroscopeImage.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.4/dotscanner/ui/RegionSelector.py` & `dotscanner-1.3.5/dotscanner/ui/RegionSelector.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.4/dotscanner/ui/ThresholdAdjuster.py` & `dotscanner-1.3.5/dotscanner/ui/ThresholdAdjuster.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.4/dotscanner/ui/UserSettings.py` & `dotscanner-1.3.5/dotscanner/ui/UserSettings.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,34 +320,41 @@
 						return
 					else:
 						self.program = ProgramType.LIFETIME
 						self.parseLifetimeFile(chosenFile)
 						return
 		
 		print(strings.invalidAnalysisFileWarning(chosenFile))
+		return
 	
 	def parseDensityFile(self, chosenFile):
 		self.filepath = os.path.dirname(chosenFile)
 		with open(chosenFile, "r") as file:
 			for line in file:
 				if line.startswith("#"):
 					continue
 				
 				splitLine = line.split()
 				if splitLine[1] == "skipped":
 					continue
 				
-				filename = splitLine[0]
-				lowerDotThreshScale = round(float(splitLine[5]), 1)
-				upperDotThreshScale = round(float(splitLine[6]), 1)
-				lowerBlobThreshScale = round(float(splitLine[7]), 1)
-				blobSize = int(splitLine[8])
-				dotSize = int(splitLine[9])
-				lowerContrast = round(float(splitLine[10]), 1)
-				upperContrast = round(float(splitLine[11]), 1)
+				# Handle filenames with spaces in them
+				extensionIndex = files.getExtensionIndexFromDensityAnalysisFileLineArray(splitLine)
+				if extensionIndex == -1:
+					print(strings.invalidFilenameInDensityAnalysisFile(splitLine))
+					return
+				filename = " ".join(splitLine[:extensionIndex + 1])
+				
+				lowerDotThreshScale = round(float(splitLine[extensionIndex + 5]), 1)
+				upperDotThreshScale = round(float(splitLine[extensionIndex + 6]), 1)
+				lowerBlobThreshScale = round(float(splitLine[extensionIndex + 7]), 1)
+				blobSize = int(splitLine[extensionIndex + 8])
+				dotSize = int(splitLine[extensionIndex + 9])
+				lowerContrast = round(float(splitLine[extensionIndex + 10]), 1)
+				upperContrast = round(float(splitLine[extensionIndex + 11]), 1)
 				polygonString = line.split("(")[1:]
 				polygonPairsStringArray = [item.split(")")[0] for item in polygonString]
 				polygon = []
 				for pair in polygonPairsStringArray:
 					x, y = pair.split(",")
 					polygon.append([int(y), int(x)])
 				polygon.append([polygon[0][0], polygon[0][1]])
```

### Comparing `dotscanner-1.3.4/dotscanner/ui/window.py` & `dotscanner-1.3.5/dotscanner/ui/window.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.4/dotscanner.egg-info/PKG-INFO` & `dotscanner-1.3.5/dotscanner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotscanner
-Version: 1.3.4
+Version: 1.3.5
 Summary: A program designed for analysis of microscope imaging data
 Home-page: https://github.com/bdavis222/dotscanner
 Author: Holly Allen and Brian Davis
 Author-email: holly.allen@colorado.edu
 Project-URL: Bug Reports, https://github.com/bdavis222/dotscanner/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/dotscanner
@@ -101,15 +101,15 @@
 #### Skips allowed
 This sets the number of consecutive images that are allowed to be skipped in a lifetime calculation. This can be useful for dimmer dots where an image or two in a series are relatively out of focus, resulting in an unwanted non-detection for those frames. By increasing the number of skips allowed, these particles will be retained as long as they are back in focus and bright enough for detection in subsequent frames.
       
 #### Remove edge frames
 This dictates whether edge frames should be removed from a lifetime calculation. If a particle is detected in the first frame of an image, for example, it cannot be determined whether the particle existed before the first image was taken, so it might not make sense to include this in a lifetime calculation (and the same may also be true for particles in the last frame). If the number of skips allowed in the lifetime calculation is greater than zero, this will increase how many edge frames are removed from analysis.
 
 ## The Threshold Adjustment Window
-This window shows the image data with the dots and blobs identified, and features several button groups on the left sidebar:
+Clicking the **Next** button, or pressing the **return** key on the keyboard, from the Configurations Window saves the configuration settings selected by the user and advances to the Threshold Adjustment Window. This window shows the image data with the dots and blobs identified, and features several button groups on the left sidebar:
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/7.png)
 
 From top to bottom, these button groups perform the following actions:
 
 #### View
 These buttons allow four different viewing options: zooming in on the top left, top right, bottom left, bottom right, or zooming back out to show the full image. The user can also press the **spacebar** on the keyboard to cycle through these different views.
 
@@ -148,15 +148,15 @@
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
-* 1.3.4
+* 1.3.5
      * Bug fixes
 * 1.3.0
      * Added option to re-analyze data without redrawing regions
      * Added particle displacement tracking during lifetime measurement
      * Added histogram output for lifetimes measurements
 * 1.2.0
      * Added options for editing the configuration file
```

### Comparing `dotscanner-1.3.4/dotscanner.egg-info/SOURCES.txt` & `dotscanner-1.3.5/dotscanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.4/settings/config.py` & `dotscanner-1.3.5/settings/config.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.4/settings/configmanagement.py` & `dotscanner-1.3.5/settings/configmanagement.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.4/setup.py` & `dotscanner-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='dotscanner',
-    version='1.3.4', # Required 
+    version='1.3.5', # Required 
     description='A program designed for analysis of microscope imaging data',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/bdavis222/dotscanner',
     author='Holly Allen and Brian Davis',
     author_email='holly.allen@colorado.edu',
     classifiers=[
```

### Comparing `dotscanner-1.3.4/tests/test_dataprocessing.py` & `dotscanner-1.3.5/tests/test_dataprocessing.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.4/tests/test_density.py` & `dotscanner-1.3.5/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.4/tests/test_files.py` & `dotscanner-1.3.5/tests/test_files.py`

 * *Files 8% similar despite different names*

```diff
@@ -281,10 +281,28 @@
         
         self.assertEqual(newFilename, "filename65.txt")
         self.assertEqual(newFilename2, "filename3.txt")
     
     def test_incrementTargetPathName(self):
         self.assertEqual(files.incrementTargetPathName("path/to/file2.txt"), "path/to/file3.txt")
         self.assertEqual(files.incrementTargetPathName("path/to/file66.txt"), "path/to/file67.txt")
+    
+    def test_getExtensionIndexFromDensityAnalysisFileLineArray(self):
+        line1 = "SD-RFP-2.tif 290 20247 0.0143231 0.0008411 1.5 5.0 2.0 5 2 0.0 5.0 (168, 425), \
+(151, 392), (62, 148), (112, 109), (230, 379)"
+        line2 = "SD 525-2.tif 195 11325 0.0172185 0.001233 1.5 5.0 2.0 5 2 0.0 5.0 (88, 198), \
+(128, 187), (154, 165), (224, 353), (184, 411)"
+        line3 = "SD 525-2tif 210 13151 0.0159684 0.0011019 1.5 5.0 2.0 5 2 0.0 5.0 (125, 438), \
+(95, 213), (148, 192), (214, 368)"
+        lineArray1 = line1.split()
+        lineArray2 = line2.split()
+        lineArray3 = line3.split()
+        extensionIndex1 = files.getExtensionIndexFromDensityAnalysisFileLineArray(lineArray1)
+        extensionIndex2 = files.getExtensionIndexFromDensityAnalysisFileLineArray(lineArray2)
+        extensionIndex3 = files.getExtensionIndexFromDensityAnalysisFileLineArray(lineArray3)
+        
+        self.assertEqual(extensionIndex1, 0)
+        self.assertEqual(extensionIndex2, 1)
+        self.assertEqual(extensionIndex3, -1)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dotscanner-1.3.4/tests/test_lifetime.py` & `dotscanner-1.3.5/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.4/tests/test_strings.py` & `dotscanner-1.3.5/tests/test_strings.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,21 @@
     def test_invalidAnalysisFileWarning(self):
         self.assertEqual(
             strings.invalidAnalysisFileWarning("test_file.png"),
             f'\nInvalid analysis file selected: "test_file.png". A valid file has a .txt extension \
 and contains density or lifetime data.'
         )
     
+    def test_invalidFilenameInDensityAnalysisFile(self):
+        self.assertEqual(
+            strings.invalidFilenameInDensityAnalysisFile(["file", "array", "example"]),
+            f"Filename with valid extension not found in the following line in densities file:\n\
+file array example"
+        )
+    
     def test_outputFileTopHeader(self):
         self.assertEqual(
             strings.outputFileTopHeader(strings.ProgramType.DENSITY),
             f"# Dot Scanner (https://github.com/bdavis222/dotscanner)\n\
 # Generated output file for density measurement\n#"
         )
         self.assertEqual(
```

### Comparing `dotscanner-1.3.4/tests/ui/FakeUserSettings.py` & `dotscanner-1.3.5/tests/ui/FakeUserSettings.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.4/tests/ui/test_MicroscopeImage.py` & `dotscanner-1.3.5/tests/ui/test_MicroscopeImage.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.4/tests/ui/test_ThresholdAdjuster.py` & `dotscanner-1.3.5/tests/ui/test_ThresholdAdjuster.py`

 * *Files identical despite different names*

