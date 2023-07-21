# Comparing `tmp/idftools-0.1.8.tar.gz` & `tmp/idftools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idftools-0.1.8.tar", last modified: Fri Jul 21 13:26:17 2023, max compression
+gzip compressed data, was "idftools-0.1.9.tar", last modified: Fri Jul 21 14:26:07 2023, max compression
```

## Comparing `idftools-0.1.8.tar` & `idftools-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-21 13:26:17.048066 idftools-0.1.8/
--rw-rw-r--   0 enio      (1000) enio      (1000)     6306 2023-07-21 13:26:17.048066 idftools-0.1.8/PKG-INFO
--rw-rw-r--   0 enio      (1000) enio      (1000)     4258 2023-07-14 21:10:47.000000 idftools-0.1.8/README.md
-drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-21 13:26:17.048066 idftools-0.1.8/modules_idftools/
-drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-21 13:26:17.048066 idftools-0.1.8/modules_idftools/idftools.egg-info/
--rw-rw-r--   0 enio      (1000) enio      (1000)     6306 2023-07-21 13:26:17.000000 idftools-0.1.8/modules_idftools/idftools.egg-info/PKG-INFO
--rw-rw-r--   0 enio      (1000) enio      (1000)      214 2023-07-21 13:26:17.000000 idftools-0.1.8/modules_idftools/idftools.egg-info/SOURCES.txt
--rw-rw-r--   0 enio      (1000) enio      (1000)        1 2023-07-21 13:26:17.000000 idftools-0.1.8/modules_idftools/idftools.egg-info/dependency_links.txt
--rw-rw-r--   0 enio      (1000) enio      (1000)       37 2023-07-21 13:26:17.000000 idftools-0.1.8/modules_idftools/idftools.egg-info/top_level.txt
--rw-rw-r--   0 enio      (1000) enio      (1000)       38 2023-07-21 13:26:17.048066 idftools-0.1.8/setup.cfg
--rw-rw-r--   0 enio      (1000) enio      (1000)      962 2023-07-21 13:26:11.000000 idftools-0.1.8/setup.py
+drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-21 14:26:07.795535 idftools-0.1.9/
+-rw-rw-r--   0 enio      (1000) enio      (1000)     6306 2023-07-21 14:26:07.795535 idftools-0.1.9/PKG-INFO
+-rw-rw-r--   0 enio      (1000) enio      (1000)     4258 2023-07-14 21:10:47.000000 idftools-0.1.9/README.md
+drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-21 14:26:07.795535 idftools-0.1.9/idftools.egg-info/
+-rw-rw-r--   0 enio      (1000) enio      (1000)     6306 2023-07-21 14:26:07.000000 idftools-0.1.9/idftools.egg-info/PKG-INFO
+-rw-rw-r--   0 enio      (1000) enio      (1000)      146 2023-07-21 14:26:07.000000 idftools-0.1.9/idftools.egg-info/SOURCES.txt
+-rw-rw-r--   0 enio      (1000) enio      (1000)        1 2023-07-21 14:26:07.000000 idftools-0.1.9/idftools.egg-info/dependency_links.txt
+-rw-rw-r--   0 enio      (1000) enio      (1000)       37 2023-07-21 14:26:07.000000 idftools-0.1.9/idftools.egg-info/top_level.txt
+-rw-rw-r--   0 enio      (1000) enio      (1000)       38 2023-07-21 14:26:07.795535 idftools-0.1.9/setup.cfg
+-rw-rw-r--   0 enio      (1000) enio      (1000)     1017 2023-07-21 14:25:56.000000 idftools-0.1.9/setup.py
```

### Comparing `idftools-0.1.8/PKG-INFO` & `idftools-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idftools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Um pacote com alguns utilitarios uteis
 Home-page: https://github.com/eniodefarias/pypi-idftools
 Author: eniodefarias
 Author-email: eniodefarias@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img src="http://ideiadofuturo.com.br/img/logo_ideia.png" width="120" title="supervisão"  alt="Supervisao Contabilidade e Consultoria">
```

### Comparing `idftools-0.1.8/README.md` & `idftools-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `idftools-0.1.8/modules_idftools/idftools.egg-info/PKG-INFO` & `idftools-0.1.9/idftools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idftools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Um pacote com alguns utilitarios uteis
 Home-page: https://github.com/eniodefarias/pypi-idftools
 Author: eniodefarias
 Author-email: eniodefarias@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img src="http://ideiadofuturo.com.br/img/logo_ideia.png" width="120" title="supervisão"  alt="Supervisao Contabilidade e Consultoria">
```

### Comparing `idftools-0.1.8/setup.py` & `idftools-0.1.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 print(f'long_description={long_description}')
 
 setup(
-    version="0.1.8",
+    version="0.1.9",
     long_description=long_description,
     long_description_content_type='text/markdown',
     # install_requires=requirements,
     name="idftools",
     author_email="eniodefarias@gmail.com",
     author="eniodefarias",
     url="https://github.com/eniodefarias/pypi-idftools",
     description="Um pacote com alguns utilitarios uteis",
     py_modules=["utilities", "driversfactory", "certificate"],
     # package_dir={"": "idftools"}
-    package_dir={"": "modules_idftools"}
+    package_dir={"idftools": "modules_idftools", "idffonts": "modules_idftools/idftools/fonts"}
 )
 
 # .venv/bin/python3 setup.py sdist bdist_wheel
 # twine upload --skip-existing dist/*
```

