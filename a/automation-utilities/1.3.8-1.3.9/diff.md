# Comparing `tmp/automation-utilities-1.3.8.tar.gz` & `tmp/automation-utilities-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-utilities-1.3.8.tar", last modified: Wed Jul 19 15:42:12 2023, max compression
+gzip compressed data, was "automation-utilities-1.3.9.tar", last modified: Fri Jul 21 18:11:34 2023, max compression
```

## Comparing `automation-utilities-1.3.8.tar` & `automation-utilities-1.3.9.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 15:42:12.069236 automation-utilities-1.3.8/
-drwxrwxrwx   0        0        0        0 2023-07-19 15:42:12.068225 automation-utilities-1.3.8/Automation_Utilities.egg-info/
--rw-rw-rw-   0        0        0      134 2023-07-19 15:42:11.000000 automation-utilities-1.3.8/Automation_Utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      596 2023-07-19 15:42:11.000000 automation-utilities-1.3.8/Automation_Utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 15:42:11.000000 automation-utilities-1.3.8/Automation_Utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-19 15:42:11.000000 automation-utilities-1.3.8/Automation_Utilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-19 15:42:11.000000 automation-utilities-1.3.8/Automation_Utilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2023-07-19 15:42:12.069236 automation-utilities-1.3.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-19 15:42:12.062144 automation-utilities-1.3.8/automation_utilities/
--rw-rw-rw-   0        0        0     1452 2023-07-16 17:33:33.000000 automation-utilities-1.3.8/automation_utilities/Data.py
--rw-rw-rw-   0        0        0      936 2023-07-18 19:42:13.000000 automation-utilities-1.3.8/automation_utilities/Files.py
--rw-rw-rw-   0        0        0      456 2023-07-04 17:58:58.000000 automation-utilities-1.3.8/automation_utilities/Generator.py
--rw-rw-rw-   0        0        0      147 2023-07-02 15:43:12.000000 automation-utilities-1.3.8/automation_utilities/Input.py
--rw-rw-rw-   0        0        0      835 2023-06-27 20:34:27.000000 automation-utilities-1.3.8/automation_utilities/PhoneNumbers.py
--rw-rw-rw-   0        0        0        0 2023-06-26 15:36:31.000000 automation-utilities-1.3.8/automation_utilities/__init__.py
--rw-rw-rw-   0        0        0       42 2023-07-19 15:42:12.070459 automation-utilities-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0      271 2023-07-19 15:41:56.000000 automation-utilities-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 18:11:34.689264 automation-utilities-1.3.9/
+drwxrwxrwx   0        0        0        0 2023-07-21 18:11:34.684251 automation-utilities-1.3.9/Automation_Utilities.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-07-21 18:11:34.000000 automation-utilities-1.3.9/Automation_Utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      694 2023-07-21 18:11:34.000000 automation-utilities-1.3.9/Automation_Utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 18:11:34.000000 automation-utilities-1.3.9/Automation_Utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-21 18:11:34.000000 automation-utilities-1.3.9/Automation_Utilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-21 18:11:34.000000 automation-utilities-1.3.9/Automation_Utilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2023-07-21 18:11:34.689264 automation-utilities-1.3.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 18:11:34.678762 automation-utilities-1.3.9/automation_utilities/
+-rw-rw-rw-   0        0        0      186 2023-07-19 17:03:31.000000 automation-utilities-1.3.9/automation_utilities/Control.py
+-rw-rw-rw-   0        0        0     1575 2023-07-20 11:40:18.000000 automation-utilities-1.3.9/automation_utilities/Data.py
+-rw-rw-rw-   0        0        0       82 2023-07-20 19:25:23.000000 automation-utilities-1.3.9/automation_utilities/Exceptions.py
+-rw-rw-rw-   0        0        0      936 2023-07-18 19:42:13.000000 automation-utilities-1.3.9/automation_utilities/Files.py
+-rw-rw-rw-   0        0        0        0 2023-07-20 19:11:30.000000 automation-utilities-1.3.9/automation_utilities/Generator.py
+-rw-rw-rw-   0        0        0      147 2023-07-02 15:43:12.000000 automation-utilities-1.3.9/automation_utilities/Input.py
+-rw-rw-rw-   0        0        0      835 2023-06-27 20:34:27.000000 automation-utilities-1.3.9/automation_utilities/PhoneNumbers.py
+-rw-rw-rw-   0        0        0      525 2023-07-20 19:11:30.000000 automation-utilities-1.3.9/automation_utilities/__init__.py
+-rw-rw-rw-   0        0        0     2195 2023-07-21 18:11:32.000000 automation-utilities-1.3.9/automation_utilities/mailtm.py
+-rw-rw-rw-   0        0        0       42 2023-07-21 18:11:34.689264 automation-utilities-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      307 2023-07-21 18:11:32.000000 automation-utilities-1.3.9/setup.py
```

### Comparing `automation-utilities-1.3.8/Automation_Utilities.egg-info/SOURCES.txt` & `automation-utilities-1.3.9/Automation_Utilities.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 setup.py
 Automation_Utilities.egg-info/PKG-INFO
 Automation_Utilities.egg-info/SOURCES.txt
 Automation_Utilities.egg-info/dependency_links.txt
 Automation_Utilities.egg-info/top_level.txt
+automation_utilities/Control.py
 automation_utilities/Data.py
+automation_utilities/Exceptions.py
 automation_utilities/Files.py
 automation_utilities/Generator.py
 automation_utilities/Input.py
 automation_utilities/PhoneNumbers.py
 automation_utilities/__init__.py
+automation_utilities/mailtm.py
 automation_utilities.egg-info/PKG-INFO
 automation_utilities.egg-info/SOURCES.txt
 automation_utilities.egg-info/dependency_links.txt
 automation_utilities.egg-info/requires.txt
 automation_utilities.egg-info/top_level.txt
```

### Comparing `automation-utilities-1.3.8/automation_utilities/Data.py` & `automation-utilities-1.3.9/automation_utilities/Data.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,17 @@
         self.file_name = file_name
         try:
             self.data = json.load(open(file_name, 'r', encoding='utf-8'))
         except FileNotFoundError:
             self.data = {}
         self._privte = 15
 
+    def __call__(self, key, from_list: list = None, loop: bool = False):
+        return self.get(key, from_list, loop)
+
     def get(self, key, from_list: list = None, loop: bool = False):
         if key not in self.data.keys():
             self.data[key] = 0
         if isinstance(self.data[key], int):
             Data.lock.acquire()
             self.data[key] += 1
             json.dump(self.data, open(self.file_name, 'w', encoding='utf-8'), indent=2, ensure_ascii=False)
```

### Comparing `automation-utilities-1.3.8/automation_utilities/Files.py` & `automation-utilities-1.3.9/automation_utilities/Files.py`

 * *Files identical despite different names*

### Comparing `automation-utilities-1.3.8/automation_utilities/PhoneNumbers.py` & `automation-utilities-1.3.9/automation_utilities/PhoneNumbers.py`

 * *Files identical despite different names*

