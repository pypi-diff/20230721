# Comparing `tmp/idftools-0.1.7.tar.gz` & `tmp/idftools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idftools-0.1.7.tar", last modified: Fri Jul 14 20:57:27 2023, max compression
+gzip compressed data, was "idftools-0.1.8.tar", last modified: Fri Jul 21 13:26:17 2023, max compression
```

## Comparing `idftools-0.1.7.tar` & `idftools-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,11 @@
-drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 20:57:27.835754 idftools-0.1.7/
--rw-rw-r--   0 enio      (1000) enio      (1000)     6293 2023-07-14 20:57:27.835754 idftools-0.1.7/PKG-INFO
--rw-rw-r--   0 enio      (1000) enio      (1000)     4261 2023-07-14 20:37:31.000000 idftools-0.1.7/README.md
-drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 20:57:27.835754 idftools-0.1.7/idftools/
--rw-rw-r--   0 enio      (1000) enio      (1000)    34945 2023-05-25 18:44:21.000000 idftools-0.1.7/idftools/certificate.py
--rwxrwxr-x   0 enio      (1000) enio      (1000)    22099 2023-07-13 20:03:14.000000 idftools-0.1.7/idftools/driversfactory.py
-drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 20:57:27.835754 idftools-0.1.7/idftools/idftools.egg-info/
--rw-rw-r--   0 enio      (1000) enio      (1000)     6293 2023-07-14 20:57:27.000000 idftools-0.1.7/idftools/idftools.egg-info/PKG-INFO
--rw-rw-r--   0 enio      (1000) enio      (1000)      255 2023-07-14 20:57:27.000000 idftools-0.1.7/idftools/idftools.egg-info/SOURCES.txt
--rw-rw-r--   0 enio      (1000) enio      (1000)        1 2023-07-14 20:57:27.000000 idftools-0.1.7/idftools/idftools.egg-info/dependency_links.txt
--rw-rw-r--   0 enio      (1000) enio      (1000)       37 2023-07-14 20:57:27.000000 idftools-0.1.7/idftools/idftools.egg-info/top_level.txt
--rwxrwxr-x   0 enio      (1000) enio      (1000)    70637 2023-07-13 20:10:20.000000 idftools-0.1.7/idftools/utilities.py
--rw-rw-r--   0 enio      (1000) enio      (1000)       38 2023-07-14 20:57:27.835754 idftools-0.1.7/setup.cfg
--rw-rw-r--   0 enio      (1000) enio      (1000)      919 2023-07-14 20:57:17.000000 idftools-0.1.7/setup.py
+drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-21 13:26:17.048066 idftools-0.1.8/
+-rw-rw-r--   0 enio      (1000) enio      (1000)     6306 2023-07-21 13:26:17.048066 idftools-0.1.8/PKG-INFO
+-rw-rw-r--   0 enio      (1000) enio      (1000)     4258 2023-07-14 21:10:47.000000 idftools-0.1.8/README.md
+drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-21 13:26:17.048066 idftools-0.1.8/modules_idftools/
+drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-21 13:26:17.048066 idftools-0.1.8/modules_idftools/idftools.egg-info/
+-rw-rw-r--   0 enio      (1000) enio      (1000)     6306 2023-07-21 13:26:17.000000 idftools-0.1.8/modules_idftools/idftools.egg-info/PKG-INFO
+-rw-rw-r--   0 enio      (1000) enio      (1000)      214 2023-07-21 13:26:17.000000 idftools-0.1.8/modules_idftools/idftools.egg-info/SOURCES.txt
+-rw-rw-r--   0 enio      (1000) enio      (1000)        1 2023-07-21 13:26:17.000000 idftools-0.1.8/modules_idftools/idftools.egg-info/dependency_links.txt
+-rw-rw-r--   0 enio      (1000) enio      (1000)       37 2023-07-21 13:26:17.000000 idftools-0.1.8/modules_idftools/idftools.egg-info/top_level.txt
+-rw-rw-r--   0 enio      (1000) enio      (1000)       38 2023-07-21 13:26:17.048066 idftools-0.1.8/setup.cfg
+-rw-rw-r--   0 enio      (1000) enio      (1000)      962 2023-07-21 13:26:11.000000 idftools-0.1.8/setup.py
```

### Comparing `idftools-0.1.7/PKG-INFO` & `idftools-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idftools
-Version: 0.1.7
+Version: 0.1.8
 Summary: Um pacote com alguns utilitarios uteis
 Home-page: https://github.com/eniodefarias/pypi-idftools
 Author: eniodefarias
 Author-email: eniodefarias@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img src="http://ideiadofuturo.com.br/img/logo_ideia.png" width="120" title="supervisão"  alt="Supervisao Contabilidade e Consultoria">  
@@ -81,21 +81,23 @@
         ## atualizando
         ```bash
         pip install --upgrade pip
         pip install --upgrade idftools
         ```
         
         ## importando
+        
         ```python
-        import idftools
+        
+        from modules_idftools import idftools
         
         # use as funções do seu pacote
-        idftools.utilities.some_function()
-        idftools.driversfactory.some_other_function()
-        idftools.certificate.another_function()
+        utilities.some_function()
+        driversfactory.some_other_function()
+        certificate.another_function()
         ```
         
         ---
         
         ---
         
         ---
```

### Comparing `idftools-0.1.7/README.md` & `idftools-0.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -73,21 +73,23 @@
 ## atualizando
 ```bash
 pip install --upgrade pip
 pip install --upgrade idftools
 ```
 
 ## importando
+
 ```python
-import idftools
+
+from modules_idftools import idftools
 
 # use as funções do seu pacote
-idftools.utilities.some_function()
-idftools.driversfactory.some_other_function()
-idftools.certificate.another_function()
+utilities.some_function()
+driversfactory.some_other_function()
+certificate.another_function()
 ```
 
 ---
 
 ---
 
 ---
```

### Comparing `idftools-0.1.7/idftools/idftools.egg-info/PKG-INFO` & `idftools-0.1.8/modules_idftools/idftools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idftools
-Version: 0.1.7
+Version: 0.1.8
 Summary: Um pacote com alguns utilitarios uteis
 Home-page: https://github.com/eniodefarias/pypi-idftools
 Author: eniodefarias
 Author-email: eniodefarias@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img src="http://ideiadofuturo.com.br/img/logo_ideia.png" width="120" title="supervisão"  alt="Supervisao Contabilidade e Consultoria">  
@@ -81,21 +81,23 @@
         ## atualizando
         ```bash
         pip install --upgrade pip
         pip install --upgrade idftools
         ```
         
         ## importando
+        
         ```python
-        import idftools
+        
+        from modules_idftools import idftools
         
         # use as funções do seu pacote
-        idftools.utilities.some_function()
-        idftools.driversfactory.some_other_function()
-        idftools.certificate.another_function()
+        utilities.some_function()
+        driversfactory.some_other_function()
+        certificate.another_function()
         ```
         
         ---
         
         ---
         
         ---
```

### Comparing `idftools-0.1.7/setup.py` & `idftools-0.1.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,22 +12,23 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 print(f'long_description={long_description}')
 
 setup(
-    version="0.1.7",
+    version="0.1.8",
     long_description=long_description,
     long_description_content_type='text/markdown',
     # install_requires=requirements,
     name="idftools",
     author_email="eniodefarias@gmail.com",
     author="eniodefarias",
     url="https://github.com/eniodefarias/pypi-idftools",
     description="Um pacote com alguns utilitarios uteis",
     py_modules=["utilities", "driversfactory", "certificate"],
-    package_dir={"": "idftools"}
+    # package_dir={"": "idftools"}
+    package_dir={"": "modules_idftools"}
 )
 
 # .venv/bin/python3 setup.py sdist bdist_wheel
 # twine upload --skip-existing dist/*
```

