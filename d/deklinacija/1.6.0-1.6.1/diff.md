# Comparing `tmp/deklinacija-1.6.0.tar.gz` & `tmp/deklinacija-1.6.1.tar.gz`

## Comparing `deklinacija-1.6.0.tar` & `deklinacija-1.6.1.tar`

### file list

```diff
@@ -1,17 +1,15 @@
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 deklinacija-1.6.0/main.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.6.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 deklinacija-1.6.0/deklinacija/__init__.py
--rw-r--r--   0        0        0    30068 2020-02-02 00:00:00.000000 deklinacija-1.6.0/deklinacija/main.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 deklinacija-1.6.0/deklinacija/notes.txt
--rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 deklinacija-1.6.0/deklinacija/utils.py
--rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 deklinacija-1.6.0/deklinacija/vokativ_database.csv
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 deklinacija-1.6.0/tests/names_female.txt
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 deklinacija-1.6.0/tests/names_female_posessive.txt
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 deklinacija-1.6.0/tests/names_male.txt
--rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 deklinacija-1.6.0/tests/names_male_posessive.txt
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 deklinacija-1.6.0/tests/test_names.py
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 deklinacija-1.6.0/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.6.0/LICENSE
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 deklinacija-1.6.0/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 deklinacija-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.6.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 deklinacija-1.6.1/deklinacija/__init__.py
+-rw-r--r--   0        0        0    30068 2020-02-02 00:00:00.000000 deklinacija-1.6.1/deklinacija/main.py
+-rw-r--r--   0        0        0     6626 2020-02-02 00:00:00.000000 deklinacija-1.6.1/deklinacija/utils.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 deklinacija-1.6.1/deklinacija/vokativ_database.csv
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 deklinacija-1.6.1/tests/names_female.txt
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 deklinacija-1.6.1/tests/names_female_posessive.txt
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 deklinacija-1.6.1/tests/names_male.txt
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 deklinacija-1.6.1/tests/names_male_posessive.txt
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 deklinacija-1.6.1/tests/test_names.py
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 deklinacija-1.6.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.6.1/LICENSE
+-rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 deklinacija-1.6.1/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 deklinacija-1.6.1/PKG-INFO
```

### Comparing `deklinacija-1.6.0/.github/workflows/python-package.yml` & `deklinacija-1.6.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `deklinacija-1.6.0/deklinacija/main.py` & `deklinacija-1.6.1/deklinacija/main.py`

 * *Files identical despite different names*

### Comparing `deklinacija-1.6.0/deklinacija/utils.py` & `deklinacija-1.6.1/deklinacija/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,24 +13,29 @@
 
 ZVUCNI = ["б", "д", "г", "ђ", "ж", "з", "џ"]
 
 latExceptions = []
 
 
 def isLatin(word):
+    """
+    Returns a boolean indicating whether the last character of the input string is in the Latin script. Raises an error if the character isn't neither in Latin or Cyrillic.
+    """
     if word[-1].lower() in alphabet:
         return True
     elif word[-1].lower() in alphabet_latin:
         return False
     else:
         raise ValueError("word contains illegal characters")
 
 
 def toCyrillic(word):
-
+    """
+    Converts input string into Cyrillic. Works with Serbian Latin letter pairs (lj, nj, dž, etc.)
+    """
     wordArray = []
     word = list(word)
     wordText = "".join(word)
 
     if wordText.lower() not in latExceptions:
         n = 0
         while n <= (len(word)-1):
@@ -76,14 +81,17 @@
 
     word = "".join(wordArray)
 
     return word
 
 
 def toLatin(word):
+    """
+    Converts input string into Cyrillic. Works with Serbian Latin letter pairs (lj, nj, dž etc.)
+    """
     word = list(word)
 
     n = 0
     for i in word:
         if i.lower() in alphabet_latin:
             if i[0].isupper() and i.lower() in ['љ', 'њ', 'џ']:
                 letter = alphabet_latin[i.lower()][0].upper(
@@ -124,16 +132,20 @@
         raise ValueError('gender param must be either "male" or "female"')
     
     if grammatical_number.lower() not in ["singular", "plural"]:
         raise ValueError('grammatical_number param must be either "singular" or "plural"')
 
     if len(name) < 3:
         raise ValueError("name param must be at least 3 characters long")
-    
+
+
 def separateLetters(word):
+    """
+    Separates letters from word, while making sure that certain letter pairs in Serbian Latin (lj, nj, dž etc.) stay together. Returns a list.
+    """
     word = list(word)
     wordText = "".join(word)
     wordArray = []
 
     n = 0
     while n <= (len(word)-1):
```

### Comparing `deklinacija-1.6.0/deklinacija/vokativ_database.csv` & `deklinacija-1.6.1/deklinacija/vokativ_database.csv`

 * *Files identical despite different names*

### Comparing `deklinacija-1.6.0/tests/names_female.txt` & `deklinacija-1.6.1/tests/names_female.txt`

 * *Files identical despite different names*

### Comparing `deklinacija-1.6.0/tests/names_female_posessive.txt` & `deklinacija-1.6.1/tests/names_female_posessive.txt`

 * *Files identical despite different names*

### Comparing `deklinacija-1.6.0/tests/names_male.txt` & `deklinacija-1.6.1/tests/names_male.txt`

 * *Files identical despite different names*

### Comparing `deklinacija-1.6.0/tests/names_male_posessive.txt` & `deklinacija-1.6.1/tests/names_male_posessive.txt`

 * *Files identical despite different names*

### Comparing `deklinacija-1.6.0/tests/test_names.py` & `deklinacija-1.6.1/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `deklinacija-1.6.0/.gitignore` & `deklinacija-1.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `deklinacija-1.6.0/LICENSE` & `deklinacija-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deklinacija-1.6.0/pyproject.toml` & `deklinacija-1.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "deklinacija"
-version = "1.6.0"
+version = "1.6.1"
 authors = [
   { name="urelja", email="code.relja@gmail.com" },
 ]
 description = "A Python library for declension of personal names in Serbian"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

