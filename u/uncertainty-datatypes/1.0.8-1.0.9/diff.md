# Comparing `tmp/uncertainty-datatypes-1.0.8.tar.gz` & `tmp/uncertainty-datatypes-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uncertainty-datatypes-1.0.8.tar", last modified: Wed Jul 19 09:57:56 2023, max compression
+gzip compressed data, was "uncertainty-datatypes-1.0.9.tar", last modified: Wed Jul 19 10:09:00 2023, max compression
```

## Comparing `uncertainty-datatypes-1.0.8.tar` & `uncertainty-datatypes-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:57:56.890350 uncertainty-datatypes-1.0.8/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     1099 2023-07-17 07:54:55.000000 uncertainty-datatypes-1.0.8/LICENSE
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10699 2023-07-19 09:57:56.890185 uncertainty-datatypes-1.0.8/PKG-INFO
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     9928 2023-07-19 09:57:21.000000 uncertainty-datatypes-1.0.8/README.md
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      854 2023-07-19 09:57:40.000000 uncertainty-datatypes-1.0.8/pyproject.toml
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       38 2023-07-19 09:57:56.890391 uncertainty-datatypes-1.0.8/setup.cfg
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:57:56.888760 uncertainty-datatypes-1.0.8/test/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4429 2023-07-19 09:42:56.000000 uncertainty-datatypes-1.0.8/test/test_ubool.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    19029 2023-07-19 09:43:27.000000 uncertainty-datatypes-1.0.8/test/test_ufloat.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      717 2023-07-19 09:43:54.000000 uncertainty-datatypes-1.0.8/test/test_ufuncs.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    17973 2023-07-19 09:43:23.000000 uncertainty-datatypes-1.0.8/test/test_uint.py
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:57:56.889397 uncertainty-datatypes-1.0.8/uncertainty/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-14 08:59:58.000000 uncertainty-datatypes-1.0.8/uncertainty/__init__.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      328 2023-07-17 11:29:42.000000 uncertainty-datatypes-1.0.8/uncertainty/result.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4311 2023-07-19 09:11:10.000000 uncertainty-datatypes-1.0.8/uncertainty/ubool.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    20722 2023-07-19 09:45:39.000000 uncertainty-datatypes-1.0.8/uncertainty/unumbers.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4306 2023-07-19 09:44:37.000000 uncertainty-datatypes-1.0.8/uncertainty/utypes.py
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:57:56.890022 uncertainty-datatypes-1.0.8/uncertainty_datatypes.egg-info/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10699 2023-07-19 09:57:56.000000 uncertainty-datatypes-1.0.8/uncertainty_datatypes.egg-info/PKG-INFO
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      446 2023-07-19 09:57:56.000000 uncertainty-datatypes-1.0.8/uncertainty_datatypes.egg-info/SOURCES.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        1 2023-07-19 09:57:56.000000 uncertainty-datatypes-1.0.8/uncertainty_datatypes.egg-info/dependency_links.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       14 2023-07-19 09:57:56.000000 uncertainty-datatypes-1.0.8/uncertainty_datatypes.egg-info/requires.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       12 2023-07-19 09:57:56.000000 uncertainty-datatypes-1.0.8/uncertainty_datatypes.egg-info/top_level.txt
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 10:09:00.091582 uncertainty-datatypes-1.0.9/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     1099 2023-07-17 07:54:55.000000 uncertainty-datatypes-1.0.9/LICENSE
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10844 2023-07-19 10:09:00.091429 uncertainty-datatypes-1.0.9/PKG-INFO
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10073 2023-07-19 10:06:41.000000 uncertainty-datatypes-1.0.9/README.md
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      854 2023-07-19 10:08:53.000000 uncertainty-datatypes-1.0.9/pyproject.toml
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       38 2023-07-19 10:09:00.091617 uncertainty-datatypes-1.0.9/setup.cfg
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 10:09:00.090049 uncertainty-datatypes-1.0.9/test/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4429 2023-07-19 09:42:56.000000 uncertainty-datatypes-1.0.9/test/test_ubool.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    19029 2023-07-19 09:43:27.000000 uncertainty-datatypes-1.0.9/test/test_ufloat.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      717 2023-07-19 09:43:54.000000 uncertainty-datatypes-1.0.9/test/test_ufuncs.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    17973 2023-07-19 09:43:23.000000 uncertainty-datatypes-1.0.9/test/test_uint.py
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 10:09:00.090669 uncertainty-datatypes-1.0.9/uncertainty/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-14 08:59:58.000000 uncertainty-datatypes-1.0.9/uncertainty/__init__.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      328 2023-07-17 11:29:42.000000 uncertainty-datatypes-1.0.9/uncertainty/result.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4311 2023-07-19 09:11:10.000000 uncertainty-datatypes-1.0.9/uncertainty/ubool.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    20722 2023-07-19 09:45:39.000000 uncertainty-datatypes-1.0.9/uncertainty/unumbers.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4306 2023-07-19 09:44:37.000000 uncertainty-datatypes-1.0.9/uncertainty/utypes.py
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 10:09:00.091268 uncertainty-datatypes-1.0.9/uncertainty_datatypes.egg-info/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10844 2023-07-19 10:09:00.000000 uncertainty-datatypes-1.0.9/uncertainty_datatypes.egg-info/PKG-INFO
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      446 2023-07-19 10:09:00.000000 uncertainty-datatypes-1.0.9/uncertainty_datatypes.egg-info/SOURCES.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        1 2023-07-19 10:09:00.000000 uncertainty-datatypes-1.0.9/uncertainty_datatypes.egg-info/dependency_links.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       14 2023-07-19 10:09:00.000000 uncertainty-datatypes-1.0.9/uncertainty_datatypes.egg-info/requires.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       12 2023-07-19 10:09:00.000000 uncertainty-datatypes-1.0.9/uncertainty_datatypes.egg-info/top_level.txt
```

### Comparing `uncertainty-datatypes-1.0.8/LICENSE` & `uncertainty-datatypes-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.8/PKG-INFO` & `uncertainty-datatypes-1.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uncertainty-datatypes
-Version: 1.0.8
+Version: 1.0.9
 Summary: Uncertainty Datatypes Library
 Author: Atenea Research Group, University of Malaga, Spain
 Project-URL: Homepage, https://github.com/atenearesearchgroup/uncertainty
 Project-URL: Bug Tracker, https://github.com/atenearesearchgroup/uncertainty/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -78,24 +78,24 @@
 * Operator: ``` x & y ``` 
 * Special operator: ``` x |AND| y ``` 
 * The ubool method: ``` x.AND(y) ``` 
 * A function: ``` AND(x, y) ```
 
 The table below summarizes all the possible usages.
 
-| Operation  | Operator       | Special Operator         | Method                  | Function                 |
-|:----------:|:--------------:|:------------------------:|:-----------------------:|:------------------------:|
-| AND        | ``` x & y ```  | ``` x |AND| y ```        | ``` x.AND(y) ```        | ``` AND(x, y) ```        |
-| OR         | ``` x | y ```  | ``` x |OR| y ```         | ``` x.OR(y) ```         | ``` OR(x, y) ```         |
-| XOR        | ``` x ^ y ```  | ``` x |XOR| y ```        | ``` x.XOR(y) ```        | ``` XOR(x, y) ```        |
-| NOT        | ``` ~ x ```    |                          | ``` x.NOT() ```         | ``` NOT(x) ```           |
-| IMPLIES    | ``` x >> y ``` | ``` x |IMPLIES| y ```    | ``` x.IMPLIES(y) ```    | ``` IMPLIES(x, y) ```    |
-| EQUIVALENT | ``` x == y ``` | ``` x |EQUIVALENT| y ``` | ``` x.EQUIVALENT(y) ``` | ``` EQUIVALENT(x, y) ``` |
-| EQUALS     | ``` x == y ``` |  ``` x |EQUALS| y ```    | ``` x.EQUALS(y) ```     | ``` EQUALS(x, y) ```     |
-| DISTINCT   | ``` x != y ``` | ``` x |DISTINCT| y ```   | ``` x.DISTINCT(y) ```   | ``` DISTINCT(x, y) ```   |
+| Operation  | Operator        | Special Operator           | Method                  | Function                 |
+|:----------:|:---------------:|:--------------------------:|:-----------------------:|:------------------------:|
+| AND        | ``` x & y ```   | ``` x \|AND\| y ```        | ``` x.AND(y) ```        | ``` AND(x, y) ```        |
+| OR         | ``` x \| y ```  | ``` x \|OR\| y ```         | ``` x.OR(y) ```         | ``` OR(x, y) ```         |
+| XOR        | ``` x ^ y ```   | ``` x \|XOR\| y ```        | ``` x.XOR(y) ```        | ``` XOR(x, y) ```        |
+| NOT        | ``` ~ x ```     |                            | ``` x.NOT() ```         | ``` NOT(x) ```           |
+| IMPLIES    | ``` x >> y ```  | ``` x \|IMPLIES\| y ```    | ``` x.IMPLIES(y) ```    | ``` IMPLIES(x, y) ```    |
+| EQUIVALENT | ``` x == y ```  | ``` x \|EQUIVALENT\| y ``` | ``` x.EQUIVALENT(y) ``` | ``` EQUIVALENT(x, y) ``` |
+| EQUALS     | ``` x == y ```  | ``` x \|EQUALS\| y ```     | ``` x.EQUALS(y) ```     | ``` EQUALS(x, y) ```     |
+| DISTINCT   | ``` x != y ```  | ``` x \|DISTINCT\| y ```   | ``` x.DISTINCT(y) ```   | ``` DISTINCT(x, y) ```   |
 
 <sub> Operators or special operators must be surrounded by parentheses due operator precedence. Meanwhile, using a method or the function provides the highest precedence. </sub>
 
 *ubool Code example:*
 ```python
 x = ubool(0.3)
 y = ubool(0.8)
@@ -301,8 +301,11 @@
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Atenea Research Group
-For more information, please visit our research group's websites: http://atenea.lcc.uma.es/projects/UncertainOCLTypes.html and http://atenea.lcc.uma.es/projects/SubjectiveLogic.html
+For more information, please visit our research group's websites: 
+- [Atenea Research Group](http://atenea.lcc.uma.es/) 
+- [Atenea: Uncertain OCL Types](http://atenea.lcc.uma.es/projects/UncertainOCLTypes.html) 
+- [Atenea: Subjective Logic](http://atenea.lcc.uma.es/projects/SubjectiveLogic.html)
```

### Comparing `uncertainty-datatypes-1.0.8/README.md` & `uncertainty-datatypes-1.0.9/uncertainty_datatypes.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: uncertainty-datatypes
+Version: 1.0.9
+Summary: Uncertainty Datatypes Library
+Author: Atenea Research Group, University of Malaga, Spain
+Project-URL: Homepage, https://github.com/atenearesearchgroup/uncertainty
+Project-URL: Bug Tracker, https://github.com/atenearesearchgroup/uncertainty/issues
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Education
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Uncertainty Python Library
 
 Uncertainty is a Python library providing uncertainty datatypes including u-type, a-type and s-type: 
 1. **u-type** datatypes: ubool, uint, ufloat, ustr, uenum.
     Type U is a pair (x, u), noted x ± u, that represents a random variable whose average is x and standard deviation is u.
 2. **a-type** datatypes: abool, aint, afloat.
     Type A, maintain the set of the measured values as X = {x1,...,xn}, x ± u could be calculated as the mean and standard deviation.
@@ -59,24 +78,24 @@
 * Operator: ``` x & y ``` 
 * Special operator: ``` x |AND| y ``` 
 * The ubool method: ``` x.AND(y) ``` 
 * A function: ``` AND(x, y) ```
 
 The table below summarizes all the possible usages.
 
-| Operation  | Operator       | Special Operator         | Method                  | Function                 |
-|:----------:|:--------------:|:------------------------:|:-----------------------:|:------------------------:|
-| AND        | ``` x & y ```  | ``` x |AND| y ```        | ``` x.AND(y) ```        | ``` AND(x, y) ```        |
-| OR         | ``` x | y ```  | ``` x |OR| y ```         | ``` x.OR(y) ```         | ``` OR(x, y) ```         |
-| XOR        | ``` x ^ y ```  | ``` x |XOR| y ```        | ``` x.XOR(y) ```        | ``` XOR(x, y) ```        |
-| NOT        | ``` ~ x ```    |                          | ``` x.NOT() ```         | ``` NOT(x) ```           |
-| IMPLIES    | ``` x >> y ``` | ``` x |IMPLIES| y ```    | ``` x.IMPLIES(y) ```    | ``` IMPLIES(x, y) ```    |
-| EQUIVALENT | ``` x == y ``` | ``` x |EQUIVALENT| y ``` | ``` x.EQUIVALENT(y) ``` | ``` EQUIVALENT(x, y) ``` |
-| EQUALS     | ``` x == y ``` |  ``` x |EQUALS| y ```    | ``` x.EQUALS(y) ```     | ``` EQUALS(x, y) ```     |
-| DISTINCT   | ``` x != y ``` | ``` x |DISTINCT| y ```   | ``` x.DISTINCT(y) ```   | ``` DISTINCT(x, y) ```   |
+| Operation  | Operator        | Special Operator           | Method                  | Function                 |
+|:----------:|:---------------:|:--------------------------:|:-----------------------:|:------------------------:|
+| AND        | ``` x & y ```   | ``` x \|AND\| y ```        | ``` x.AND(y) ```        | ``` AND(x, y) ```        |
+| OR         | ``` x \| y ```  | ``` x \|OR\| y ```         | ``` x.OR(y) ```         | ``` OR(x, y) ```         |
+| XOR        | ``` x ^ y ```   | ``` x \|XOR\| y ```        | ``` x.XOR(y) ```        | ``` XOR(x, y) ```        |
+| NOT        | ``` ~ x ```     |                            | ``` x.NOT() ```         | ``` NOT(x) ```           |
+| IMPLIES    | ``` x >> y ```  | ``` x \|IMPLIES\| y ```    | ``` x.IMPLIES(y) ```    | ``` IMPLIES(x, y) ```    |
+| EQUIVALENT | ``` x == y ```  | ``` x \|EQUIVALENT\| y ``` | ``` x.EQUIVALENT(y) ``` | ``` EQUIVALENT(x, y) ``` |
+| EQUALS     | ``` x == y ```  | ``` x \|EQUALS\| y ```     | ``` x.EQUALS(y) ```     | ``` EQUALS(x, y) ```     |
+| DISTINCT   | ``` x != y ```  | ``` x \|DISTINCT\| y ```   | ``` x.DISTINCT(y) ```   | ``` DISTINCT(x, y) ```   |
 
 <sub> Operators or special operators must be surrounded by parentheses due operator precedence. Meanwhile, using a method or the function provides the highest precedence. </sub>
 
 *ubool Code example:*
 ```python
 x = ubool(0.3)
 y = ubool(0.8)
@@ -282,8 +301,11 @@
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Atenea Research Group
-For more information, please visit our research group's websites: http://atenea.lcc.uma.es/projects/UncertainOCLTypes.html and http://atenea.lcc.uma.es/projects/SubjectiveLogic.html
+For more information, please visit our research group's websites: 
+- [Atenea Research Group](http://atenea.lcc.uma.es/) 
+- [Atenea: Uncertain OCL Types](http://atenea.lcc.uma.es/projects/UncertainOCLTypes.html) 
+- [Atenea: Subjective Logic](http://atenea.lcc.uma.es/projects/SubjectiveLogic.html)
```

### Comparing `uncertainty-datatypes-1.0.8/pyproject.toml` & `uncertainty-datatypes-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uncertainty-datatypes"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Atenea Research Group, University of Malaga, Spain" },
 ]
 description = "Uncertainty Datatypes Library"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers=[
```

### Comparing `uncertainty-datatypes-1.0.8/test/test_ubool.py` & `uncertainty-datatypes-1.0.9/test/test_ubool.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.8/test/test_ufloat.py` & `uncertainty-datatypes-1.0.9/test/test_ufloat.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.8/test/test_ufuncs.py` & `uncertainty-datatypes-1.0.9/test/test_ufuncs.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.8/test/test_uint.py` & `uncertainty-datatypes-1.0.9/test/test_uint.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.8/uncertainty/ubool.py` & `uncertainty-datatypes-1.0.9/uncertainty/ubool.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.8/uncertainty/unumbers.py` & `uncertainty-datatypes-1.0.9/uncertainty/unumbers.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.8/uncertainty/utypes.py` & `uncertainty-datatypes-1.0.9/uncertainty/utypes.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.8/uncertainty_datatypes.egg-info/PKG-INFO` & `uncertainty-datatypes-1.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: uncertainty-datatypes
-Version: 1.0.8
-Summary: Uncertainty Datatypes Library
-Author: Atenea Research Group, University of Malaga, Spain
-Project-URL: Homepage, https://github.com/atenearesearchgroup/uncertainty
-Project-URL: Bug Tracker, https://github.com/atenearesearchgroup/uncertainty/issues
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Education
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Uncertainty Python Library
 
 Uncertainty is a Python library providing uncertainty datatypes including u-type, a-type and s-type: 
 1. **u-type** datatypes: ubool, uint, ufloat, ustr, uenum.
     Type U is a pair (x, u), noted x ± u, that represents a random variable whose average is x and standard deviation is u.
 2. **a-type** datatypes: abool, aint, afloat.
     Type A, maintain the set of the measured values as X = {x1,...,xn}, x ± u could be calculated as the mean and standard deviation.
@@ -78,24 +59,24 @@
 * Operator: ``` x & y ``` 
 * Special operator: ``` x |AND| y ``` 
 * The ubool method: ``` x.AND(y) ``` 
 * A function: ``` AND(x, y) ```
 
 The table below summarizes all the possible usages.
 
-| Operation  | Operator       | Special Operator         | Method                  | Function                 |
-|:----------:|:--------------:|:------------------------:|:-----------------------:|:------------------------:|
-| AND        | ``` x & y ```  | ``` x |AND| y ```        | ``` x.AND(y) ```        | ``` AND(x, y) ```        |
-| OR         | ``` x | y ```  | ``` x |OR| y ```         | ``` x.OR(y) ```         | ``` OR(x, y) ```         |
-| XOR        | ``` x ^ y ```  | ``` x |XOR| y ```        | ``` x.XOR(y) ```        | ``` XOR(x, y) ```        |
-| NOT        | ``` ~ x ```    |                          | ``` x.NOT() ```         | ``` NOT(x) ```           |
-| IMPLIES    | ``` x >> y ``` | ``` x |IMPLIES| y ```    | ``` x.IMPLIES(y) ```    | ``` IMPLIES(x, y) ```    |
-| EQUIVALENT | ``` x == y ``` | ``` x |EQUIVALENT| y ``` | ``` x.EQUIVALENT(y) ``` | ``` EQUIVALENT(x, y) ``` |
-| EQUALS     | ``` x == y ``` |  ``` x |EQUALS| y ```    | ``` x.EQUALS(y) ```     | ``` EQUALS(x, y) ```     |
-| DISTINCT   | ``` x != y ``` | ``` x |DISTINCT| y ```   | ``` x.DISTINCT(y) ```   | ``` DISTINCT(x, y) ```   |
+| Operation  | Operator        | Special Operator           | Method                  | Function                 |
+|:----------:|:---------------:|:--------------------------:|:-----------------------:|:------------------------:|
+| AND        | ``` x & y ```   | ``` x \|AND\| y ```        | ``` x.AND(y) ```        | ``` AND(x, y) ```        |
+| OR         | ``` x \| y ```  | ``` x \|OR\| y ```         | ``` x.OR(y) ```         | ``` OR(x, y) ```         |
+| XOR        | ``` x ^ y ```   | ``` x \|XOR\| y ```        | ``` x.XOR(y) ```        | ``` XOR(x, y) ```        |
+| NOT        | ``` ~ x ```     |                            | ``` x.NOT() ```         | ``` NOT(x) ```           |
+| IMPLIES    | ``` x >> y ```  | ``` x \|IMPLIES\| y ```    | ``` x.IMPLIES(y) ```    | ``` IMPLIES(x, y) ```    |
+| EQUIVALENT | ``` x == y ```  | ``` x \|EQUIVALENT\| y ``` | ``` x.EQUIVALENT(y) ``` | ``` EQUIVALENT(x, y) ``` |
+| EQUALS     | ``` x == y ```  | ``` x \|EQUALS\| y ```     | ``` x.EQUALS(y) ```     | ``` EQUALS(x, y) ```     |
+| DISTINCT   | ``` x != y ```  | ``` x \|DISTINCT\| y ```   | ``` x.DISTINCT(y) ```   | ``` DISTINCT(x, y) ```   |
 
 <sub> Operators or special operators must be surrounded by parentheses due operator precedence. Meanwhile, using a method or the function provides the highest precedence. </sub>
 
 *ubool Code example:*
 ```python
 x = ubool(0.3)
 y = ubool(0.8)
@@ -301,8 +282,11 @@
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Atenea Research Group
-For more information, please visit our research group's websites: http://atenea.lcc.uma.es/projects/UncertainOCLTypes.html and http://atenea.lcc.uma.es/projects/SubjectiveLogic.html
+For more information, please visit our research group's websites: 
+- [Atenea Research Group](http://atenea.lcc.uma.es/) 
+- [Atenea: Uncertain OCL Types](http://atenea.lcc.uma.es/projects/UncertainOCLTypes.html) 
+- [Atenea: Subjective Logic](http://atenea.lcc.uma.es/projects/SubjectiveLogic.html)
```

