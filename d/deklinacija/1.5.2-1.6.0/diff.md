# Comparing `tmp/deklinacija-1.5.2.tar.gz` & `tmp/deklinacija-1.6.0.tar.gz`

## Comparing `deklinacija-1.5.2.tar` & `deklinacija-1.6.0.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.5.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deklinacija-1.5.2/deklinacija/__init__.py
--rw-r--r--   0        0        0    21641 2020-02-02 00:00:00.000000 deklinacija-1.5.2/deklinacija/module.py
--rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 deklinacija-1.5.2/deklinacija/utils.py
--rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 deklinacija-1.5.2/deklinacija/vokativ_database.csv
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 deklinacija-1.5.2/tests/names_female.txt
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 deklinacija-1.5.2/tests/names_male.txt
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 deklinacija-1.5.2/tests/test_names.py
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 deklinacija-1.5.2/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.5.2/LICENSE
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 deklinacija-1.5.2/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 deklinacija-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 deklinacija-1.6.0/main.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.6.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 deklinacija-1.6.0/deklinacija/__init__.py
+-rw-r--r--   0        0        0    30068 2020-02-02 00:00:00.000000 deklinacija-1.6.0/deklinacija/main.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 deklinacija-1.6.0/deklinacija/notes.txt
+-rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 deklinacija-1.6.0/deklinacija/utils.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 deklinacija-1.6.0/deklinacija/vokativ_database.csv
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 deklinacija-1.6.0/tests/names_female.txt
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 deklinacija-1.6.0/tests/names_female_posessive.txt
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 deklinacija-1.6.0/tests/names_male.txt
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 deklinacija-1.6.0/tests/names_male_posessive.txt
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 deklinacija-1.6.0/tests/test_names.py
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 deklinacija-1.6.0/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.6.0/LICENSE
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 deklinacija-1.6.0/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 deklinacija-1.6.0/PKG-INFO
```

### Comparing `deklinacija-1.5.2/.github/workflows/python-package.yml` & `deklinacija-1.6.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `deklinacija-1.5.2/deklinacija/module.py` & `deklinacija-1.6.0/deklinacija/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import deklinacija.utils as utils
 
 VOWELS = ["а", "е", "и", "о", "у"]  # used for identifying consonants
 
 # the last and second to last characters in names ending in these characters switch places during declension
 NEP_A = ["тар", "ац", "рај", "рађ", "рак", "нак", "ндар", "чак"]
 NEP_A_EXCEPT = []  # names which have one of the above suffixes but the last and the 2nd to last characters don't switch places during declension
-INSTRUMENTAL_LETTERS = ["ј", "љ", "њ", "ђ", "ћ", "ч", "џ", "ш", "ж"]
+ZADNJONEPCANI = ["ј", "љ", "њ", "ђ", "ћ", "ч", "џ", "ш", "ж"]
 PALATALIZACIJA = {"к": "ч", "г": "ж", "х": "ш", }
-
+POSSESIVE_SUFFIXES = {"male_singular":"","male_plural":"и","female_singular":"а","female_plural":"е","neutral_singular":"о","neutral_plural":"а"}
+MALE_EXCEPTIONS = ["тата","газда","судија","ага"]
+FEMALE_EXCEPTIONS = ["пећ","чађ","кћер","ствар","љубав","радост"]
 
 def genitiv(name, gender):
     """
     OD KOGA, OD ČEGA? FROM WHOM?
 
     Returns the genitive form of the provided name. If a last name is present, it must be separated with a whitespace.
     
@@ -104,17 +106,21 @@
     name: The name that should be declined
     gender: The gender of the person, param value must be either "male" or "female"
     """
     utils.check(name, gender)
     name = name.strip()
     fullName = name.split()
     returnName = []
-
+    n = 0
     for i in fullName:
-        changedName = __vokativ(i, gender)
+        if n == 0: 
+            changedName = __vokativ(i, gender,False)
+            n += 1
+        else:
+            changedName = __vokativ(i, gender,True)
         returnName.append(changedName)
 
     return " ".join(returnName)
 
 def instrumental(name, gender):
     """
     S KIM? ČIM? WITH WHOM? WITH WHAT?
@@ -139,15 +145,15 @@
         changedName = __instrumental(i, gender)
         returnName.append(changedName)
 
     return " ".join(returnName)
 
 def lokativ(name, gender):
     """
-    O KOME? O ČEMU? U KOJOJ LOKACIJI? ABOUT WHO? ABOUT WHAT? IN WHAT LOCATION?
+    O KOME? O ČEMU? NA KOJOJ LOKACIJI? ABOUT WHO? ABOUT WHAT? IN WHAT LOCATION?
 
     Returns the locative form of the provided name. If a last name is present, it must be separated with a whitespace.
     
     Context in a sentence:
     "Marko je trenutno u Beogradu."
     Translation:
     "Marko is currently in Belgrade."
@@ -163,14 +169,202 @@
 
     for i in fullName:
         changedName = __lokativ(i, gender)
         returnName.append(changedName)
 
     return " ".join(returnName)
 
+def possesive(name,gender,object_gender,grammatical_number="singular"):
+    """
+    ČIJI? WHOSE?
+
+    Returns the possesive form of the provided name. Depends on the object_gender and grammatical_number parameters to add the appropriate suffix to the name.
+    
+    Parameters:
+    name: The name of the person that posseses something
+    gender: The gender of the person that posesses something, param value must be either "male" or "female"
+    object_gender: Can either be the gender of the object that the person posesses (value must be "male", "female" or "neutral") or the object itself, in which case the gender will be automatically detected provided that the grammatical_number param is correct
+    grammatical_number: The grammatical number of the object that the person posesses. Param value must be either "singular" or "plural". Default: singular
+    """
+    utils.checkPosessive(name,gender,grammatical_number)
+    object_gender = object_gender.strip().lower()
+
+    if object_gender not in ["male", "female", "neutral"]:
+        object_gender = utils.toCyrillic(object_gender)
+        if object_gender[-1] == "е":
+            if grammatical_number == "singular":
+                object_gender = "neutral"
+            else:
+                object_gender = "female"
+        elif object_gender[-1] == "а":
+            if object_gender in MALE_EXCEPTIONS:
+                object_gender = "male"
+            else:
+                object_gender = "female"
+        elif object_gender[-1] == "и" and grammatical_number == "plural":
+            test = object_gender[:-1]
+            if test in FEMALE_EXCEPTIONS:
+                object_gender = "female"
+            else:
+                object_gender = "male"
+        else:
+            if object_gender in FEMALE_EXCEPTIONS:
+                object_gender = "female"
+            else:
+                object_gender = "male"
+    
+    #name = name.strip()
+
+    lastChar = name[-1]
+    if lastChar.isupper():
+        if utils.isLatin(lastChar) == True:
+            suffix = utils.toLatin(POSSESIVE_SUFFIXES[object_gender+"_"+grammatical_number]).upper()
+        else:
+            suffix = POSSESIVE_SUFFIXES[object_gender+"_"+grammatical_number].upper()
+    else:
+        if utils.isLatin(lastChar) == True:
+            suffix = utils.toLatin(POSSESIVE_SUFFIXES[object_gender+"_"+grammatical_number])
+        else:
+            suffix = POSSESIVE_SUFFIXES[object_gender+"_"+grammatical_number]
+    return __possesive(name,gender)+suffix
+
+def posessiveAll(name,gender):
+    """
+    Creates all possible posessive forms (male, female and neutral in plural and singular) of the provided name and returns a dictionary where the keys are in the "GENDER_NUMBER" format.
+
+    Parameters:
+    name: The name that should be transformed
+    gender: The gender of the person, param value must be either "male" or "female"
+    """
+    utils.check(name, gender)
+    name = name.strip()
+    
+    return {"name":name,"male_singular":possesive(name,gender,"male","singular"),"male_plural":possesive(name,gender,"male","plural"),"female_singular":possesive(name,gender,"female","singular"),"female_plural":possesive(name,gender,"female","plural"),"neutral_singular":possesive(name,gender,"neutral","singular"),"neutral_plural":possesive(name,gender,"neutral","plural")}
+
+def __possesive(name,gender):
+    utils.check(name, gender)
+    name = utils.separateLetters(__genitiv(name.strip(),gender))
+    lastChar = name[-1]
+    secToLastChar = name[-2]
+    lastThree = name[-3]+name[-2]+name[-1]
+    lastTwo = name[-2]+name[-1]
+
+    if gender.lower() == "female" and utils.toCyrillic(name[-1].lower()) not in ['е','e']:
+        if lastChar.isupper():
+            if utils.isLatin(lastChar) == True:
+                if utils.toCyrillic(lastChar.lower()) in ['и','i']:
+                    name[-1] = "IJIN"
+                    return "".join(name)
+
+                name.append("IN")
+                return "".join(name)
+            else:
+                if utils.toCyrillic(lastChar.lower()) in ['и','i']:
+                    name[-1] = "ИЈИН"
+                    return "".join(name)
+                
+                name.append("ИН")
+                return "".join(name)
+        else:
+            if utils.isLatin(lastChar) == True:
+                if utils.toCyrillic(lastChar.lower()) in ['и','i']:
+                    name[-1] = "ijin"
+                    return "".join(name)
+                if lastThree.lower() == 'ice':
+                    name[-2] = "č"
+
+                name.append("in")
+                return "".join(name)
+            else:
+                if utils.toCyrillic(lastChar.lower()) in ['и','i']:
+                    name[-1] = "ијин"
+                    return "".join(name)
+
+                name.append("ин")
+                return "".join(name)
+            
+    if name[-1].lower() in ['е','e']:
+        if lastChar.isupper():
+            if utils.isLatin(lastChar) == True:
+                if utils.toCyrillic(lastChar.lower()) in ['и','i']:
+                    name[-1] = "IJIN"
+                    return "".join(name)
+                elif lastThree.lower() == 'ice':
+                    name[-2] = "Č"
+
+                name[-1] = "IN"
+                return "".join(name)
+            else:
+                if utils.toCyrillic(lastChar.lower()) in ['и','i']:
+                    name[-1] = "ИЈИН"
+                    return "".join(name)
+                elif lastThree.lower() == 'ице':
+                    name[-2] = "Ч"
+                
+                name[-1] = "ИН"
+                return "".join(name)
+        else:
+            if utils.isLatin(lastChar) == True:
+                if utils.toCyrillic(lastChar.lower()) in ['и','i']:
+                    name[-1] = "ijin"
+                    return "".join(name)
+                if lastThree.lower() == 'ice':
+                    name[-2] = "č"
+
+                name[-1] = "in"
+                return "".join(name)
+            else:
+                if utils.toCyrillic(lastChar.lower()) in ['и','i']:
+                    name[-1] = "ијин"
+                    return "".join(name)
+                elif lastThree.lower() == 'ице':
+                    name[-2] = "ч"
+
+                name[-1] = "ин"
+                return "".join(name)
+    
+    if name[-1].lower() in ['а','a','г','g']:
+        if lastChar.isupper():
+            if utils.isLatin(lastChar) == True:
+                if utils.toCyrillic(secToLastChar.lower()) in ZADNJONEPCANI:
+                    name[-1] = "EV"
+                    return "".join(name)
+                if utils.toCyrillic(lastTwo.lower()) == "ог":
+                    name = name[:-1]
+
+                name[-1] = "OV"
+                return "".join(name)
+            else:
+                if utils.toCyrillic(secToLastChar.lower()) in ZADNJONEPCANI:
+                    name[-1] = "ЕВ"
+                    return "".join(name)
+                
+                name[-1] = "ОВ"
+                return "".join(name)
+        else:
+            if utils.isLatin(lastChar) == True:
+                if utils.toCyrillic(secToLastChar.lower()) in ZADNJONEPCANI:
+                    name[-1] = "ev"
+                    return "".join(name)
+                if utils.toCyrillic(lastTwo.lower()) == "ог":
+                    name = name[:-1]
+                
+                name[-1] = "ov"
+                return "".join(name)
+            else:
+                if utils.toCyrillic(secToLastChar.lower()) in ZADNJONEPCANI:
+                    name[-1] = "ев"
+                    return "".join(name)
+                if utils.toCyrillic(lastTwo.lower()) == "ог":
+                    name = name[:-1]
+                
+                name[-1] = "ов"
+                return "".join(name)
+    
+
 def __genitiv(name, gender):
     utils.check(name, gender)
     name = utils.separateLetters(name.strip())
 
     lastChar = name[-1]
     secToLastChar = name[-2]
     trdToLastChar = name[-3]
@@ -398,29 +592,29 @@
             if utils.isLatin(lastChar) == True:
                 name[-1] = "u"
             else:
                 name[-1] = "у"
 
     return "".join(name)
 
-def __vokativ(name, gender):
+def __vokativ(name, gender, last_name):
     utils.check(name, gender)
     name = name.strip()
     nameGenitiv = list(genitiv(name, gender))
     name = list(name)
     nameSep = utils.separateLetters(name)
     rest = "".join(name[:-1])
 
     if gender.lower() == "female" and name[-1].lower() not in ["а", "a"]:
         return "".join(name)
 
     if name[-2].lower()+name[-1].lower() in ["ia", "иа"]:
         return "".join(name)
 
-    if utils.toCyrillic(name[-1].lower()) in ["к", "ц"] and (utils.toCyrillic((nameSep[-3]+nameSep[-2]+nameSep[-1]).lower()) in NEP_A or utils.toCyrillic(nameSep[-2]+nameSep[-1]).lower() in NEP_A):
+    if utils.toCyrillic(name[-1].lower()) in ["к", "ц"] and (utils.toCyrillic((nameSep[-3]+nameSep[-2]+nameSep[-1]).lower()) in NEP_A or utils.toCyrillic(nameSep[-2]+nameSep[-1]).lower() in NEP_A or last_name == True):
         if nameGenitiv[-1].islower():
             if utils.isLatin(nameGenitiv[-1]) == True:
                 nameGenitiv[-1] = "u"
             else:
                 nameGenitiv[-1] = "у"
         else:
             if utils.isLatin(nameGenitiv[-1]) == True:
@@ -455,15 +649,15 @@
                     PALATALIZACIJA[utils.toCyrillic(nameGenitiv[-2].lower())].upper())
             else:
                 nameGenitiv[-2] = PALATALIZACIJA[nameGenitiv[-2].lower()
                                                  ].upper()
 
             return "".join(nameGenitiv)
 
-    if utils.toCyrillic(name[-1].lower()) in INSTRUMENTAL_LETTERS:
+    if utils.toCyrillic(name[-1].lower()) in ZADNJONEPCANI:
         if nameGenitiv[-1].islower():
             if utils.isLatin(nameGenitiv[-1]) == True:
                 nameGenitiv[-1] = "u"
             else:
                 nameGenitiv[-1] = "у"
         else:
             if utils.isLatin(nameGenitiv[-1]) == True:
@@ -562,15 +756,15 @@
         else:
             if utils.isLatin(lastChar) == True:
                 name[-1] = "im"
             else:
                 name[-1] = "им"
         return "".join(name)
 
-    if gender.lower() == "male" and utils.toCyrillic(nameGenitiv)[-1].lower() in INSTRUMENTAL_LETTERS and name[-1].lower() not in ["а", "a"]:
+    if gender.lower() == "male" and utils.toCyrillic(nameGenitiv)[-1].lower() in ZADNJONEPCANI and name[-1].lower() not in ["а", "a"]:
         if lastChar.isupper():
             if utils.isLatin(lastChar):
                 nameGenitiv.append("EM")
             else:
                 nameGenitiv.append("ЕМ")
             return "".join(nameGenitiv)
         else:
```

### Comparing `deklinacija-1.5.2/deklinacija/utils.py` & `deklinacija-1.6.0/deklinacija/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,28 +98,41 @@
             word[n] = i
         n += 1
 
     return "".join(word)
 
 
 def check(name, gender):
-    if type(name) != str or type(name) != str or type(gender) != str:
+    if type(name) != str or type(gender) != str:
         raise TypeError(
-            "name and gender params must be a string, param latin must be a boolean")
+            "name and gender params must be a string")
 
-    gender = gender.strip()
     name = name.strip()
 
     if gender.lower() not in ["male", "female"]:
         raise ValueError('gender param must be either "male" or "female"')
 
     if len(name) < 3:
         raise ValueError("name param must be at least 3 characters long")
 
 
+def checkPosessive(name,gender,grammatical_number):
+    if type(name) != str or type(gender) != str or type(grammatical_number) != str:
+        raise TypeError(
+            "all params must be strings")
+    
+    if gender.lower() not in ["male", "female"]:
+        raise ValueError('gender param must be either "male" or "female"')
+    
+    if grammatical_number.lower() not in ["singular", "plural"]:
+        raise ValueError('grammatical_number param must be either "singular" or "plural"')
+
+    if len(name) < 3:
+        raise ValueError("name param must be at least 3 characters long")
+    
 def separateLetters(word):
     word = list(word)
     wordText = "".join(word)
     wordArray = []
 
     n = 0
     while n <= (len(word)-1):
```

### Comparing `deklinacija-1.5.2/deklinacija/vokativ_database.csv` & `deklinacija-1.6.0/deklinacija/vokativ_database.csv`

 * *Files identical despite different names*

### Comparing `deklinacija-1.5.2/tests/names_female.txt` & `deklinacija-1.6.0/tests/names_female.txt`

 * *Files identical despite different names*

### Comparing `deklinacija-1.5.2/tests/names_male.txt` & `deklinacija-1.6.0/tests/names_male.txt`

 * *Files identical despite different names*

### Comparing `deklinacija-1.5.2/tests/test_names.py` & `deklinacija-1.6.0/tests/test_names.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,21 +6,28 @@
 namesMale = ["Predrag","Minja","Relja","Uroš","Petrović","Petar","Mačak","Božidar","Đurađ","Djuradj","Miki","Dario","Čuperak","Đorđe","Djordje","Pablo","Juraj","Aleksandar","Opanak","Vlah","Subotički","Niški","Srpski","Dario Subotički","Minja Niški","Miki Srpski"]
 namesFemale = ["Jana","Milica","Mia","Ines","Tea","Ina","Petrović","Daria","Anžujska","Subotički","Petka","Lana Petrović","Sandra Anžujska","Milica Tabova","Milica Releva"]
 
 module_path = os.path.abspath(__file__)
 module_directory = os.path.dirname(module_path)
 file_path_male = os.path.join(module_directory, 'names_male.txt')
 file_path_female = os.path.join(module_directory, 'names_female.txt')
+file_path_male_p = os.path.join(module_directory, 'names_male_posessive.txt')
+file_path_female_p = os.path.join(module_directory, 'names_female_posessive.txt')
 
 with open(file_path_male, "r", encoding="utf-8") as fileM:
     read_content_male = fileM.readlines()
 
 with open(file_path_female, "r", encoding="utf-8") as fileF:
     read_content_female = fileF.readlines()
 
+with open(file_path_male_p, "r", encoding="utf-8") as fileMP:
+    read_content_male_p = fileMP.readlines()
+
+with open(file_path_female_p, "r", encoding="utf-8") as fileFP:
+    read_content_female_p = fileFP.readlines()
 
 def testMaleNames():
     n = 0
     for i in read_content_male:
         nameDict = ast.literal_eval(read_content_male[n].strip())
         name = nameDict['nominativ']
         compare = dek.declineAll(name,"male")
@@ -30,8 +37,26 @@
 def testFemaleNames():
     n = 0
     for i in read_content_female:
         nameDict = ast.literal_eval(read_content_female[n].strip())
         name = nameDict['nominativ']
         compare = dek.declineAll(name,"female")
         assert compare == nameDict
+        n += 1
+
+def testPosessiveMaleNames():
+    n = 0
+    for i in read_content_male_p:
+        nameDict = ast.literal_eval(read_content_male_p[n].strip())
+        name = nameDict['name']
+        compare = dek.posessiveAll(name,"male")
+        assert compare == nameDict
+        n += 1
+
+def testPosessiveFemaleNames():
+    n = 0
+    for i in read_content_female_p:
+        nameDict = ast.literal_eval(read_content_female_p[n].strip())
+        name = nameDict['name']
+        compare = dek.posessiveAll(name,"female")
+        assert compare == nameDict
         n += 1
```

### Comparing `deklinacija-1.5.2/.gitignore` & `deklinacija-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `deklinacija-1.5.2/LICENSE` & `deklinacija-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deklinacija-1.5.2/README.md` & `deklinacija-1.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,8 +56,8 @@
 
 ## Todo
 The following features are on the roadmap:
 - Possessive forms
 
 
 ## Attribution
-[Vokativi](https://github.com/startitrs/vokativi) by [Startit](https://github.com/startitrs) is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) / Modifications: converted to Cyrillic and filtered out names longer than 4 characters
+[Vokativi](https://github.com/startitrs/vokativi) by [Startit](https://github.com/startitrs) is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) / Modifications: converted to Cyrillic and filtered out names longer than 6 characters
```

### Comparing `deklinacija-1.5.2/pyproject.toml` & `deklinacija-1.6.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "deklinacija"
-version = "1.5.2"
+version = "1.6.0"
 authors = [
   { name="urelja", email="code.relja@gmail.com" },
 ]
 description = "A Python library for declension of personal names in Serbian"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `deklinacija-1.5.2/PKG-INFO` & `deklinacija-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deklinacija
-Version: 1.5.2
+Version: 1.6.0
 Summary: A Python library for declension of personal names in Serbian
 Project-URL: Homepage, https://github.com/urelja/deklinacija
 Project-URL: Bug Tracker, https://github.com/urelja/deklinacija/issues
 Author-email: urelja <code.relja@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -70,8 +70,8 @@
 
 ## Todo
 The following features are on the roadmap:
 - Possessive forms
 
 
 ## Attribution
-[Vokativi](https://github.com/startitrs/vokativi) by [Startit](https://github.com/startitrs) is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) / Modifications: converted to Cyrillic and filtered out names longer than 4 characters
+[Vokativi](https://github.com/startitrs/vokativi) by [Startit](https://github.com/startitrs) is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) / Modifications: converted to Cyrillic and filtered out names longer than 6 characters
```

