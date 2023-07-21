# Comparing `tmp/sound-extraction-2.0.1.tar.gz` & `tmp/sound-extraction-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sound-extraction-2.0.1.tar", last modified: Fri Jul 21 00:20:52 2023, max compression
+gzip compressed data, was "dist\sound-extraction-2.1.2.tar", last modified: Thu Jul 20 13:02:59 2023, max compression
```

## Comparing `sound-extraction-2.0.1.tar` & `sound-extraction-2.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 00:20:52.502227 sound-extraction-2.0.1/
--rw-rw-rw-   0        0        0     1087 2023-06-12 17:14:00.000000 sound-extraction-2.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     8682 2023-07-21 00:20:52.501224 sound-extraction-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     8176 2023-07-20 13:20:13.000000 sound-extraction-2.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-21 00:20:52.503236 sound-extraction-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1334 2023-07-21 00:18:51.000000 sound-extraction-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 00:20:52.475412 sound-extraction-2.0.1/sound_extraction.egg-info/
--rw-rw-rw-   0        0        0     8682 2023-07-21 00:20:52.000000 sound-extraction-2.0.1/sound_extraction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-07-21 00:20:52.000000 sound-extraction-2.0.1/sound_extraction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 00:20:52.000000 sound-extraction-2.0.1/sound_extraction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      126 2023-07-21 00:20:52.000000 sound-extraction-2.0.1/sound_extraction.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      219 2023-07-21 00:20:52.000000 sound-extraction-2.0.1/sound_extraction.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-21 00:20:52.000000 sound-extraction-2.0.1/sound_extraction.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 00:20:52.498386 sound-extraction-2.0.1/src/
--rw-rw-rw-   0        0        0        0 2023-07-18 16:09:50.000000 sound-extraction-2.0.1/src/__init__.py
--rw-rw-rw-   0        0        0    10890 2023-07-21 00:14:28.000000 sound-extraction-2.0.1/src/recording_times_generator.py
--rw-rw-rw-   0        0        0    18955 2023-07-21 00:18:33.000000 sound-extraction-2.0.1/src/sound_extraction.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:02:59.863448 sound-extraction-2.1.2/
+-rw-rw-rw-   0        0        0     1087 2023-06-12 17:14:00.000000 sound-extraction-2.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     8537 2023-07-20 13:02:59.861407 sound-extraction-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8031 2023-07-20 12:50:30.000000 sound-extraction-2.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-20 13:02:59.864400 sound-extraction-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1334 2023-07-20 13:02:20.000000 sound-extraction-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:02:59.849439 sound-extraction-2.1.2/sound_extraction.egg-info/
+-rw-rw-rw-   0        0        0     8537 2023-07-20 13:02:59.000000 sound-extraction-2.1.2/sound_extraction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-07-20 13:02:59.000000 sound-extraction-2.1.2/sound_extraction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 13:02:59.000000 sound-extraction-2.1.2/sound_extraction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      126 2023-07-20 13:02:59.000000 sound-extraction-2.1.2/sound_extraction.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      219 2023-07-20 13:02:59.000000 sound-extraction-2.1.2/sound_extraction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-20 13:02:59.000000 sound-extraction-2.1.2/sound_extraction.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 13:02:59.858418 sound-extraction-2.1.2/src/
+-rw-rw-rw-   0        0        0        0 2023-07-18 16:09:50.000000 sound-extraction-2.1.2/src/__init__.py
+-rw-rw-rw-   0        0        0    10907 2023-07-19 20:33:31.000000 sound-extraction-2.1.2/src/recording_times_generator.py
+-rw-rw-rw-   0        0        0    18955 2023-07-20 12:53:44.000000 sound-extraction-2.1.2/src/sound_extraction.py
```

### Comparing `sound-extraction-2.0.1/LICENSE.txt` & `sound-extraction-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sound-extraction-2.0.1/PKG-INFO` & `sound-extraction-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: sound-extraction
-Version: 2.0.1
+Version: 2.1.2
 Home-page: https://github.com/prayagnshah/Sound-Extraction
 Author: Prayag Shah
 Author-email: prayagshah07@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Audio-File Extraction
 
-[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI](https://img.shields.io/pypi/v/sound-extraction)
+[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/pypromice.svg)](https://pypi.org/project/sound-extraction/)
 
 ## About
 
 Use this tool to segment (i.e., clip or slice), copy, and extract short-duration recordings, from long-duration WAV or FLAC files. Segmenting audio files into smaller parts can make recordings compatible for certain analytical workflows and allow for easier manipulation and sharing. Segment and extracting recordings based on a list of recording start times (date times) and a desired duration. This allows for applications such as the extraction of stratified audio samples, among others.
 
 ## Types of Installation and you only have to use *one* of them
 
@@ -130,16 +130,14 @@
 
 1. Try to have your original audio files in subfolder of root directory and once you provide path of root folder then code will search for all the files in all subfolders as well as in root folder.
 
 2. Original files should be in the format `20220611T202300.wav` or `20220611T202300.flac`. Sample files in CSV should be in the format `20220611_202300.wav` or `20220611_202300.flac` under the heading `sampleFile`. For instance,
 
    ![Sample Image](data/image.png)
 
-3. If you do not have the CSV file with sample times then you can generate the CSV file by following this [README](https://github.com/prayagnshah/Sound-Extraction/blob/main/src/README.md)
-
 ## Changelog
 
 1. All the version changes are mentioned in the [CHANGELOG.md](https://github.com/prayagnshah/Sound-Extraction/blob/main/CHANGELOG.md) file.
 
 ## Contributing
 
 Contributions are welcomed and appreciated. Here are some ways to get involved:
```

### Comparing `sound-extraction-2.0.1/README.md` & `sound-extraction-2.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Audio-File Extraction
 
-[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI](https://img.shields.io/pypi/v/sound-extraction)
+[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/pypromice.svg)](https://pypi.org/project/sound-extraction/)
 
 ## About
 
 Use this tool to segment (i.e., clip or slice), copy, and extract short-duration recordings, from long-duration WAV or FLAC files. Segmenting audio files into smaller parts can make recordings compatible for certain analytical workflows and allow for easier manipulation and sharing. Segment and extracting recordings based on a list of recording start times (date times) and a desired duration. This allows for applications such as the extraction of stratified audio samples, among others.
 
 ## Types of Installation and you only have to use *one* of them
 
@@ -116,16 +116,14 @@
 
 1. Try to have your original audio files in subfolder of root directory and once you provide path of root folder then code will search for all the files in all subfolders as well as in root folder.
 
 2. Original files should be in the format `20220611T202300.wav` or `20220611T202300.flac`. Sample files in CSV should be in the format `20220611_202300.wav` or `20220611_202300.flac` under the heading `sampleFile`. For instance,
 
    ![Sample Image](data/image.png)
 
-3. If you do not have the CSV file with sample times then you can generate the CSV file by following this [README](https://github.com/prayagnshah/Sound-Extraction/blob/main/src/README.md)
-
 ## Changelog
 
 1. All the version changes are mentioned in the [CHANGELOG.md](https://github.com/prayagnshah/Sound-Extraction/blob/main/CHANGELOG.md) file.
 
 ## Contributing
 
 Contributions are welcomed and appreciated. Here are some ways to get involved:
```

### Comparing `sound-extraction-2.0.1/setup.py` & `sound-extraction-2.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="sound-extraction",
-    version="2.0.1",
+    version="2.1.2",
     packages=["src"],
     install_requires=[
         "certifi==2023.5.7",
         "cffi==1.15.1",
         "load-dotenv==0.1.0",
         "numpy==1.24.3",
         "pycparser==2.21",
```

### Comparing `sound-extraction-2.0.1/sound_extraction.egg-info/PKG-INFO` & `sound-extraction-2.1.2/sound_extraction.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: sound-extraction
-Version: 2.0.1
+Version: 2.1.2
 Home-page: https://github.com/prayagnshah/Sound-Extraction
 Author: Prayag Shah
 Author-email: prayagshah07@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Audio-File Extraction
 
-[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI](https://img.shields.io/pypi/v/sound-extraction)
+[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/pypromice.svg)](https://pypi.org/project/sound-extraction/)
 
 ## About
 
 Use this tool to segment (i.e., clip or slice), copy, and extract short-duration recordings, from long-duration WAV or FLAC files. Segmenting audio files into smaller parts can make recordings compatible for certain analytical workflows and allow for easier manipulation and sharing. Segment and extracting recordings based on a list of recording start times (date times) and a desired duration. This allows for applications such as the extraction of stratified audio samples, among others.
 
 ## Types of Installation and you only have to use *one* of them
 
@@ -130,16 +130,14 @@
 
 1. Try to have your original audio files in subfolder of root directory and once you provide path of root folder then code will search for all the files in all subfolders as well as in root folder.
 
 2. Original files should be in the format `20220611T202300.wav` or `20220611T202300.flac`. Sample files in CSV should be in the format `20220611_202300.wav` or `20220611_202300.flac` under the heading `sampleFile`. For instance,
 
    ![Sample Image](data/image.png)
 
-3. If you do not have the CSV file with sample times then you can generate the CSV file by following this [README](https://github.com/prayagnshah/Sound-Extraction/blob/main/src/README.md)
-
 ## Changelog
 
 1. All the version changes are mentioned in the [CHANGELOG.md](https://github.com/prayagnshah/Sound-Extraction/blob/main/CHANGELOG.md) file.
 
 ## Contributing
 
 Contributions are welcomed and appreciated. Here are some ways to get involved:
```

### Comparing `sound-extraction-2.0.1/src/recording_times_generator.py` & `sound-extraction-2.1.2/src/recording_times_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,17 +240,17 @@
     # Writing the list of dictionaries to a CSV file
     fieldnames = ["site", "sampleFile", "sunrise", "sunset", "category"]
     
     # Check if the output path is a directory or a file
     file_path = args.output
     
     if os.path.isdir(file_path):
-        file_path = os.path.join(file_path, "samples.csv")
-    elif not file_path.endswith(".csv"):
-        file_path += ".csv"
+        file_path = os.path.join(args.output + "samples.csv")
+    elif os.path.splitext(file_path)[1] == ".csv":
+        file_path = args.output
     
     
     with open(file_path, "w", newline='') as f:
         writer = csv.DictWriter(f, fieldnames=fieldnames)
         writer.writeheader()
         writer.writerows(random_samples)
```

### Comparing `sound-extraction-2.0.1/src/sound_extraction.py` & `sound-extraction-2.1.2/src/sound_extraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 load_dotenv()
 
 # Get the sentry DSN from the environment variables
 sentry_dsn = os.getenv("sentry_dsn")
 
 sentry_sdk.init(
     dsn=sentry_dsn,
-    release="v2.0.1",
+    release="v2.1.2",
     # Set traces_sample_rate to 1.0 to capture 100%
     # of transactions for performance monitoring.
     traces_sample_rate=1.0,
 )
 
 def main():
     def get_directories(root_directory):
```

