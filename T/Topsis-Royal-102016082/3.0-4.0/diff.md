# Comparing `tmp/Topsis-Royal-102016082-3.0.tar.gz` & `tmp/Topsis-Royal-102016082-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Topsis-Royal-102016082-3.0.tar", last modified: Fri Jul 21 16:58:17 2023, max compression
+gzip compressed data, was "Topsis-Royal-102016082-4.0.tar", last modified: Fri Jul 21 17:30:56 2023, max compression
```

## Comparing `Topsis-Royal-102016082-3.0.tar` & `Topsis-Royal-102016082-4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 16:58:17.536733 Topsis-Royal-102016082-3.0/
--rw-rw-rw-   0        0        0     1067 2023-07-21 16:38:52.000000 Topsis-Royal-102016082-3.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2048 2023-07-21 16:58:17.536733 Topsis-Royal-102016082-3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1504 2023-07-21 16:52:50.000000 Topsis-Royal-102016082-3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 16:58:17.536733 Topsis-Royal-102016082-3.0/Topsis_Royal_102016082.egg-info/
--rw-rw-rw-   0        0        0     2048 2023-07-21 16:58:17.000000 Topsis-Royal-102016082-3.0/Topsis_Royal_102016082.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-07-21 16:58:17.000000 Topsis-Royal-102016082-3.0/Topsis_Royal_102016082.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 16:58:17.000000 Topsis-Royal-102016082-3.0/Topsis_Royal_102016082.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-07-21 16:58:17.000000 Topsis-Royal-102016082-3.0/Topsis_Royal_102016082.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-07-21 16:58:17.000000 Topsis-Royal-102016082-3.0/Topsis_Royal_102016082.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-21 16:58:17.000000 Topsis-Royal-102016082-3.0/Topsis_Royal_102016082.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-21 16:58:17.544758 Topsis-Royal-102016082-3.0/setup.cfg
--rw-rw-rw-   0        0        0     1126 2023-07-21 16:58:12.000000 Topsis-Royal-102016082-3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 16:58:17.536733 Topsis-Royal-102016082-3.0/topsis_assignment/
--rw-rw-rw-   0        0        0       17 2023-07-21 16:28:00.000000 Topsis-Royal-102016082-3.0/topsis_assignment/__init__.py
--rw-rw-rw-   0        0        0     2789 2023-07-21 16:33:51.000000 Topsis-Royal-102016082-3.0/topsis_assignment/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 17:30:56.503924 Topsis-Royal-102016082-4.0/
+-rw-rw-rw-   0        0        0     1067 2023-07-21 16:38:52.000000 Topsis-Royal-102016082-4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2138 2023-07-21 17:30:56.503924 Topsis-Royal-102016082-4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1633 2023-07-21 17:29:04.000000 Topsis-Royal-102016082-4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 17:30:56.479898 Topsis-Royal-102016082-4.0/Topsis_Royal_102016082.egg-info/
+-rw-rw-rw-   0        0        0     2138 2023-07-21 17:30:56.000000 Topsis-Royal-102016082-4.0/Topsis_Royal_102016082.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-07-21 17:30:56.000000 Topsis-Royal-102016082-4.0/Topsis_Royal_102016082.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 17:30:56.000000 Topsis-Royal-102016082-4.0/Topsis_Royal_102016082.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-21 17:30:56.000000 Topsis-Royal-102016082-4.0/Topsis_Royal_102016082.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2023-07-21 17:30:56.000000 Topsis-Royal-102016082-4.0/Topsis_Royal_102016082.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-21 17:30:56.000000 Topsis-Royal-102016082-4.0/Topsis_Royal_102016082.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-21 17:30:56.511931 Topsis-Royal-102016082-4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1126 2023-07-21 17:30:27.000000 Topsis-Royal-102016082-4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 17:30:56.503924 Topsis-Royal-102016082-4.0/topsis_assignment/
+-rw-rw-rw-   0        0        0       17 2023-07-21 17:30:39.000000 Topsis-Royal-102016082-4.0/topsis_assignment/__init__.py
+-rw-rw-rw-   0        0        0     2776 2023-07-21 17:28:29.000000 Topsis-Royal-102016082-4.0/topsis_assignment/__main__.py
```

### Comparing `Topsis-Royal-102016082-3.0/LICENSE.txt` & `Topsis-Royal-102016082-4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Topsis-Royal-102016082-3.0/PKG-INFO` & `Topsis-Royal-102016082-4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Topsis-Royal-102016082
-Version: 3.0
+Version: 4.0
 Summary: Topsis Assignment
 Home-page: https://github.com/RGarg2002/Topsis-Royal-102016082
 Author: Royal Garg
 Author-email: royalgarg36@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
@@ -18,23 +18,28 @@
 The Technique for Order of Preference by Similarity to Ideal Solution (TOPSIS) is a multi-criteria decision analysis method. TOPSIS is based on the concept that the chosen alternative should have the shortest geometric distance from the positive ideal solution (PIS) and the longest geometric distance from the negative ideal solution
 
 ## The Method
 - Step 1 
 Calculating Normalized Matrix and weighted Normalize matrix. We normalize each value by making it: where m is the number of rows in the dataset and n is the number of columns. I vary along rows and j varies along the column.
 
 - Step 2
-Calculating Ideal Best and Ideal worst and Euclidean distance for each row from ideal worst and ideal best value. First, we will find out the ideal best and ideal worst value: Now here we need to see the impact, i.e. is it â€˜+â€™ or â€˜-â€˜ impact. If â€˜+â€™ impact Ideal best for a column is the maximum value in that column and the ideal worst is the minimum value in that column, and vice versa for the â€˜-â€˜ impact.
+Calculating Ideal Best and Ideal worst and Euclidean distance for each row from ideal worst and ideal best value. First, we will find out the ideal best and ideal worst value: Now here we need to see the impact, i.e. is it '+' or '-' impact. If '+' impact Ideal best for a column is the maximum value in that column and the ideal worst is the minimum value in that column, and vice versa for the '-' impact.
 
 - Step 3
-    Calculating Topsis Score and Ranking. Now we have Distance positive and distance negative with us, letâ€™s calculate the Topsis score for each row on basis of them.
+    Calculating Topsis Score and Ranking. Now we have Distance positive and distance negative with us, let's calculate the Topsis score for each row on basis of them.
     TOPSIS Score = diw / (dib + diw)  for each row
     Now rank according to the TOPSIS score, i.e. higher the score, better the rank
 
 ## Installation
 
 On the Python console, run 'pip install Topsis-Royal-102016082'
 
+## Usage
+
+On the python console run 'topsis InputDataFile Weights Impacts ResultFileName'
+Ex: topsis data.csv "1,1,2,2" "+,-,-,+" result.csv
+
 ## License
 
 MIT
 
 **Free Software, Hell Yeah!**
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Topsis-Royal-102016082-3.0/README.md` & `Topsis-Royal-102016082-4.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -3,23 +3,28 @@
 The Technique for Order of Preference by Similarity to Ideal Solution (TOPSIS) is a multi-criteria decision analysis method. TOPSIS is based on the concept that the chosen alternative should have the shortest geometric distance from the positive ideal solution (PIS) and the longest geometric distance from the negative ideal solution
 
 ## The Method
 - Step 1 
 Calculating Normalized Matrix and weighted Normalize matrix. We normalize each value by making it: where m is the number of rows in the dataset and n is the number of columns. I vary along rows and j varies along the column.
 
 - Step 2
-Calculating Ideal Best and Ideal worst and Euclidean distance for each row from ideal worst and ideal best value. First, we will find out the ideal best and ideal worst value: Now here we need to see the impact, i.e. is it ‘+’ or ‘-‘ impact. If ‘+’ impact Ideal best for a column is the maximum value in that column and the ideal worst is the minimum value in that column, and vice versa for the ‘-‘ impact.
+Calculating Ideal Best and Ideal worst and Euclidean distance for each row from ideal worst and ideal best value. First, we will find out the ideal best and ideal worst value: Now here we need to see the impact, i.e. is it '+' or '-' impact. If '+' impact Ideal best for a column is the maximum value in that column and the ideal worst is the minimum value in that column, and vice versa for the '-' impact.
 
 - Step 3
-    Calculating Topsis Score and Ranking. Now we have Distance positive and distance negative with us, let’s calculate the Topsis score for each row on basis of them.
+    Calculating Topsis Score and Ranking. Now we have Distance positive and distance negative with us, let's calculate the Topsis score for each row on basis of them.
     TOPSIS Score = diw / (dib + diw)  for each row
     Now rank according to the TOPSIS score, i.e. higher the score, better the rank
 
 ## Installation
 
 On the Python console, run 'pip install Topsis-Royal-102016082'
 
+## Usage
+
+On the python console run 'topsis InputDataFile Weights Impacts ResultFileName'
+Ex: topsis data.csv "1,1,2,2" "+,-,-,+" result.csv
+
 ## License
 
 MIT
 
 **Free Software, Hell Yeah!**
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Topsis-Royal-102016082-3.0/Topsis_Royal_102016082.egg-info/PKG-INFO` & `Topsis-Royal-102016082-4.0/Topsis_Royal_102016082.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Topsis-Royal-102016082
-Version: 3.0
+Version: 4.0
 Summary: Topsis Assignment
 Home-page: https://github.com/RGarg2002/Topsis-Royal-102016082
 Author: Royal Garg
 Author-email: royalgarg36@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
@@ -18,23 +18,28 @@
 The Technique for Order of Preference by Similarity to Ideal Solution (TOPSIS) is a multi-criteria decision analysis method. TOPSIS is based on the concept that the chosen alternative should have the shortest geometric distance from the positive ideal solution (PIS) and the longest geometric distance from the negative ideal solution
 
 ## The Method
 - Step 1 
 Calculating Normalized Matrix and weighted Normalize matrix. We normalize each value by making it: where m is the number of rows in the dataset and n is the number of columns. I vary along rows and j varies along the column.
 
 - Step 2
-Calculating Ideal Best and Ideal worst and Euclidean distance for each row from ideal worst and ideal best value. First, we will find out the ideal best and ideal worst value: Now here we need to see the impact, i.e. is it â€˜+â€™ or â€˜-â€˜ impact. If â€˜+â€™ impact Ideal best for a column is the maximum value in that column and the ideal worst is the minimum value in that column, and vice versa for the â€˜-â€˜ impact.
+Calculating Ideal Best and Ideal worst and Euclidean distance for each row from ideal worst and ideal best value. First, we will find out the ideal best and ideal worst value: Now here we need to see the impact, i.e. is it '+' or '-' impact. If '+' impact Ideal best for a column is the maximum value in that column and the ideal worst is the minimum value in that column, and vice versa for the '-' impact.
 
 - Step 3
-    Calculating Topsis Score and Ranking. Now we have Distance positive and distance negative with us, letâ€™s calculate the Topsis score for each row on basis of them.
+    Calculating Topsis Score and Ranking. Now we have Distance positive and distance negative with us, let's calculate the Topsis score for each row on basis of them.
     TOPSIS Score = diw / (dib + diw)  for each row
     Now rank according to the TOPSIS score, i.e. higher the score, better the rank
 
 ## Installation
 
 On the Python console, run 'pip install Topsis-Royal-102016082'
 
+## Usage
+
+On the python console run 'topsis InputDataFile Weights Impacts ResultFileName'
+Ex: topsis data.csv "1,1,2,2" "+,-,-,+" result.csv
+
 ## License
 
 MIT
 
 **Free Software, Hell Yeah!**
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Topsis-Royal-102016082-3.0/setup.py` & `Topsis-Royal-102016082-4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="Topsis-Royal-102016082",
-    version="3.0",
+    version="4.0",
     description="Topsis Assignment",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/RGarg2002/Topsis-Royal-102016082",
     author="Royal Garg",
     author_email="royalgarg36@gmail.com",
     license="MIT",
```

### Comparing `Topsis-Royal-102016082-3.0/topsis_assignment/__main__.py` & `Topsis-Royal-102016082-4.0/topsis_assignment/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import math
 import numpy as np
 import sys
 import logging
 
 def main():  
   if (len(sys.argv) != 5):
-    logging.warning("Usages: python <program.py> <InputDataFile> <Weights> <Impacts> <ResultFileName>")
+    logging.warning("Usages: topsis <InputDataFile> <Weights> <Impacts> <ResultFileName>")
     exit()
   try:
       data = pd.DataFrame(pd.read_csv(str(sys.argv[1])))
   except FileNotFoundError:
       logging.warning("Wrong input data file or file path")
       exit()
   data1 = data.copy()
```

