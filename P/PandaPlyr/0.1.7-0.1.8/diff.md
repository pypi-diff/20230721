# Comparing `tmp/PandaPlyr-0.1.7.tar.gz` & `tmp/PandaPlyr-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PandaPlyr-0.1.7.tar", last modified: Thu Jul 20 05:12:25 2023, max compression
+gzip compressed data, was "PandaPlyr-0.1.8.tar", last modified: Thu Jul 20 22:34:49 2023, max compression
```

## Comparing `PandaPlyr-0.1.7.tar` & `PandaPlyr-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 05:12:25.623316 PandaPlyr-0.1.7/
--rw-rw-rw-   0        0        0    15728 2023-07-20 05:12:25.623316 PandaPlyr-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-20 05:12:25.607316 PandaPlyr-0.1.7/PandaPlyr.egg-info/
--rw-rw-rw-   0        0        0    15728 2023-07-20 05:12:25.000000 PandaPlyr-0.1.7/PandaPlyr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-07-20 05:12:25.000000 PandaPlyr-0.1.7/PandaPlyr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 05:12:25.000000 PandaPlyr-0.1.7/PandaPlyr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-20 05:12:25.000000 PandaPlyr-0.1.7/PandaPlyr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-20 05:12:25.000000 PandaPlyr-0.1.7/PandaPlyr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14572 2023-07-20 05:05:29.000000 PandaPlyr-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-20 05:12:25.624316 PandaPlyr-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      840 2023-07-20 05:11:53.000000 PandaPlyr-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 05:12:25.614317 PandaPlyr-0.1.7/src/
--rw-rw-rw-   0        0        0      170 2023-07-20 05:11:56.000000 PandaPlyr-0.1.7/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 05:12:25.617316 PandaPlyr-0.1.7/src/data/
--rw-rw-rw-   0        0        0      369 2023-07-18 22:08:45.000000 PandaPlyr-0.1.7/src/data/student_grades.csv
--rw-rw-rw-   0        0        0      114 2023-07-18 21:53:36.000000 PandaPlyr-0.1.7/src/data/subject_categories.csv
--rw-rw-rw-   0        0        0    57910 2023-07-18 16:51:59.000000 PandaPlyr-0.1.7/src/data/titanic.csv
--rw-rw-rw-   0        0        0    23671 2023-07-20 04:49:06.000000 PandaPlyr-0.1.7/src/pandaplyr.py
--rw-rw-rw-   0        0        0     1273 2023-07-19 20:45:03.000000 PandaPlyr-0.1.7/src/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-20 05:12:25.617316 PandaPlyr-0.1.7/tests/
--rw-rw-rw-   0        0        0     8347 2023-07-20 04:49:51.000000 PandaPlyr-0.1.7/tests/test_pyplyr.py
+drwxrwxrwx   0        0        0        0 2023-07-20 22:34:49.756265 PandaPlyr-0.1.8/
+-rw-rw-rw-   0        0        0     1090 2023-07-20 21:36:47.000000 PandaPlyr-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0    15885 2023-07-20 22:34:49.755264 PandaPlyr-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-20 22:34:49.728267 PandaPlyr-0.1.8/PandaPlyr.egg-info/
+-rw-rw-rw-   0        0        0    15885 2023-07-20 22:34:49.000000 PandaPlyr-0.1.8/PandaPlyr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-07-20 22:34:49.000000 PandaPlyr-0.1.8/PandaPlyr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 22:34:49.000000 PandaPlyr-0.1.8/PandaPlyr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-20 22:34:49.000000 PandaPlyr-0.1.8/PandaPlyr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-20 22:34:49.000000 PandaPlyr-0.1.8/PandaPlyr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14705 2023-07-20 21:35:02.000000 PandaPlyr-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-20 22:34:49.756265 PandaPlyr-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      840 2023-07-20 22:33:23.000000 PandaPlyr-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 22:34:49.730265 PandaPlyr-0.1.8/src/
+-rw-rw-rw-   0        0        0      170 2023-07-20 22:33:19.000000 PandaPlyr-0.1.8/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 22:34:49.749265 PandaPlyr-0.1.8/src/data/
+-rw-rw-rw-   0        0        0      369 2023-07-18 22:08:45.000000 PandaPlyr-0.1.8/src/data/student_grades.csv
+-rw-rw-rw-   0        0        0    51243 2023-07-20 22:29:22.000000 PandaPlyr-0.1.8/src/data/student_grades_by_year.csv
+-rw-rw-rw-   0        0        0      114 2023-07-18 21:53:36.000000 PandaPlyr-0.1.8/src/data/subject_categories.csv
+-rw-rw-rw-   0        0        0    57910 2023-07-18 16:51:59.000000 PandaPlyr-0.1.8/src/data/titanic.csv
+-rw-rw-rw-   0        0        0    23666 2023-07-20 15:28:21.000000 PandaPlyr-0.1.8/src/pandaplyr.py
+-rw-rw-rw-   0        0        0     1620 2023-07-20 22:30:01.000000 PandaPlyr-0.1.8/src/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-20 22:34:49.750266 PandaPlyr-0.1.8/tests/
+-rw-rw-rw-   0        0        0     8347 2023-07-20 04:49:51.000000 PandaPlyr-0.1.8/tests/test_pyplyr.py
```

### Comparing `PandaPlyr-0.1.7/PKG-INFO` & `PandaPlyr-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: PandaPlyr
-Version: 0.1.7
+Version: 0.1.8
 Summary: The purpose of PandaPlyr is to make chained operations on pandas DataFrames easier and more readable.
 Home-page: https://github.com/OlivierNDO/PandaPlyr/
 Author: Nick Olivier
 Author-email: Olivier_N@lynchburg.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ## <img src="images/PyPlyr_Icon.png" alt="Project Logo" width="80" height="80"> PandaPlyr
 
 [![PyPI version](https://badge.fury.io/py/pandaplyr.svg)](https://badge.fury.io/py/pandaplyr)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 PandaPlyr is a Python package designed to provide a familiar and efficient data manipulation experience similar to the popular dplyr package in R. It aims to simplify and streamline the process of working with tabular data by providing a concise and intuitive syntax. The purpose of pandaplyr is to make chained operations on pandas DataFrames easier and more readable.
 
 ## Table of Contents
 
 - [Installing](#installing)
 - [Features](#features)
@@ -657,14 +659,14 @@
 
 </td></tr> 
 </table>
 
 
 
 ## Future features
-
+- [ ] Benchmarking module
 - [ ] Polars backend
 - [ ] Intelligent multiprocessing
 
 
 ## Contact
 [![LinkedIn Badge](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/oliviernicholas/)
```

### Comparing `PandaPlyr-0.1.7/PandaPlyr.egg-info/PKG-INFO` & `PandaPlyr-0.1.8/PandaPlyr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: PandaPlyr
-Version: 0.1.7
+Version: 0.1.8
 Summary: The purpose of PandaPlyr is to make chained operations on pandas DataFrames easier and more readable.
 Home-page: https://github.com/OlivierNDO/PandaPlyr/
 Author: Nick Olivier
 Author-email: Olivier_N@lynchburg.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ## <img src="images/PyPlyr_Icon.png" alt="Project Logo" width="80" height="80"> PandaPlyr
 
 [![PyPI version](https://badge.fury.io/py/pandaplyr.svg)](https://badge.fury.io/py/pandaplyr)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 PandaPlyr is a Python package designed to provide a familiar and efficient data manipulation experience similar to the popular dplyr package in R. It aims to simplify and streamline the process of working with tabular data by providing a concise and intuitive syntax. The purpose of pandaplyr is to make chained operations on pandas DataFrames easier and more readable.
 
 ## Table of Contents
 
 - [Installing](#installing)
 - [Features](#features)
@@ -657,14 +659,14 @@
 
 </td></tr> 
 </table>
 
 
 
 ## Future features
-
+- [ ] Benchmarking module
 - [ ] Polars backend
 - [ ] Intelligent multiprocessing
 
 
 ## Contact
 [![LinkedIn Badge](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/oliviernicholas/)
```

### Comparing `PandaPlyr-0.1.7/README.md` & `PandaPlyr-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ## <img src="images/PyPlyr_Icon.png" alt="Project Logo" width="80" height="80"> PandaPlyr
 
 [![PyPI version](https://badge.fury.io/py/pandaplyr.svg)](https://badge.fury.io/py/pandaplyr)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 PandaPlyr is a Python package designed to provide a familiar and efficient data manipulation experience similar to the popular dplyr package in R. It aims to simplify and streamline the process of working with tabular data by providing a concise and intuitive syntax. The purpose of pandaplyr is to make chained operations on pandas DataFrames easier and more readable.
 
 ## Table of Contents
 
 - [Installing](#installing)
 - [Features](#features)
@@ -644,14 +645,14 @@
 
 </td></tr> 
 </table>
 
 
 
 ## Future features
-
+- [ ] Benchmarking module
 - [ ] Polars backend
 - [ ] Intelligent multiprocessing
 
 
 ## Contact
 [![LinkedIn Badge](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/oliviernicholas/)
```

### Comparing `PandaPlyr-0.1.7/setup.py` & `PandaPlyr-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="PandaPlyr",
-    version="0.1.7",
+    version="0.1.8",
     author="Nick Olivier",
     author_email="Olivier_N@lynchburg.edu",
     description="The purpose of PandaPlyr is to make chained operations on pandas DataFrames easier and more readable.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/OlivierNDO/PandaPlyr/",
     packages=['PandaPlyr'],
```

### Comparing `PandaPlyr-0.1.7/src/data/titanic.csv` & `PandaPlyr-0.1.8/src/data/titanic.csv`

 * *Files identical despite different names*

### Comparing `PandaPlyr-0.1.7/src/pandaplyr.py` & `PandaPlyr-0.1.8/src/pandaplyr.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         group_columns = args[0]
     else:
         group_columns = list(args)
         
     # Ensure group columns are present in the DataFrame
     for gc in group_columns:
         if gc not in df.columns:
-            raise KeyError(f"Column '{col}' does not exist in the DataFrame")
+            raise KeyError(f"Column '{gc}' does not exist in the DataFrame")
     return df.groupby(group_columns, **kwargs)
 
 
 @Pipe
 def summarise(df, *args, **kwargs):
     """
     Function to aggregate a pandas DataFrame.
@@ -155,16 +155,14 @@
                 # if operation is not a string or a function, assign it to the column directly
                 df_copy[column] = operation
         except Exception as e:
             raise ValueError(f"Error processing operation '{operation}' for column '{column}': {str(e)}")
     return df_copy
 
 
-
-
 @Pipe
 def where(df, condition):
     """
     Function to filter rows of a pandas DataFrame based on a condition.
 
     Parameters:
     -----------
```

### Comparing `PandaPlyr-0.1.7/src/utils.py` & `PandaPlyr-0.1.8/src/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,26 @@
     -------
     pandas.DataFrame:
         The loaded Grades dataset.
     """
     data_path = pkg_resources.resource_filename('PandaPlyr', 'data/student_grades.csv')
     return pd.read_csv(data_path)
 
+def read_grades_by_year_dataset():
+    """
+    Read the Grades dataset from the CSV file into a pandas Dataframe
+
+    Returns:
+    -------
+    pandas.DataFrame:
+        The loaded Grades dataset.
+    """
+    data_path = pkg_resources.resource_filename('PandaPlyr', 'data/student_grades_by_year.csv')
+    return pd.read_csv(data_path)
+
 def read_subject_dataset():
     """
     Read the Subject dataset from the CSV file into a pandas Dataframe
 
     Returns:
     -------
     pandas.DataFrame:
```

### Comparing `PandaPlyr-0.1.7/tests/test_pyplyr.py` & `PandaPlyr-0.1.8/tests/test_pyplyr.py`

 * *Files identical despite different names*

