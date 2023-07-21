# Comparing `tmp/PythonQueryLanguage-0.1.6.tar.gz` & `tmp/pythonquerylanguage-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonQueryLanguage-0.1.6.tar", max compression
+gzip compressed data, was "pythonquerylanguage-0.1.8.tar", max compression
```

## Comparing `PythonQueryLanguage-0.1.6.tar` & `pythonquerylanguage-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rwxr-xr-x   0        0        0      455 2022-08-22 12:31:00.049547 PythonQueryLanguage-0.1.6/pyproject.toml
--rwxr-xr-x   0        0        0        0 2022-08-22 12:22:59.796524 PythonQueryLanguage-0.1.6/pythonquerylanguage/__init__.py
--rwxr-xr-x   0        0        0    23085 2022-08-22 12:25:16.313928 PythonQueryLanguage-0.1.6/pythonquerylanguage/pql.py
--rwxr-xr-x   0        0        0     2866 2022-02-25 14:04:00.907483 PythonQueryLanguage-0.1.6/readme.md
--rw-r--r--   0        0        0     3736 2022-08-22 12:31:04.311988 PythonQueryLanguage-0.1.6/setup.py
--rw-r--r--   0        0        0     3528 2022-08-22 12:31:04.312703 PythonQueryLanguage-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-21 12:05:56.004611 pythonquerylanguage-0.1.8/PythonQueryLanguage/__init__.py
+-rwxr-xr-x   0        0        0    23085 2022-08-22 12:25:16.000000 pythonquerylanguage-0.1.8/PythonQueryLanguage/pql.py
+-rw-r--r--   0        0        0      508 2023-07-21 12:31:32.742791 pythonquerylanguage-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2866 2023-07-21 12:05:56.008611 pythonquerylanguage-0.1.8/readme.md
+-rw-r--r--   0        0        0     3569 1970-01-01 00:00:00.000000 pythonquerylanguage-0.1.8/PKG-INFO
```

### Comparing `PythonQueryLanguage-0.1.6/pythonquerylanguage/pql.py` & `pythonquerylanguage-0.1.8/PythonQueryLanguage/pql.py`

 * *Files identical despite different names*

### Comparing `PythonQueryLanguage-0.1.6/readme.md` & `pythonquerylanguage-0.1.8/readme.md`

 * *Files identical despite different names*

### Comparing `PythonQueryLanguage-0.1.6/setup.py` & `pythonquerylanguage-0.1.8/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,98 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pythonquerylanguage
+Version: 0.1.8
+Summary: Python SQL wrapper based on pandas and SQLalchemy
+License: MIT
+Author: Pablo Ruiz
+Author-email: pablo.r.c@live.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: SQLAlchemy (>=1.4.31,<2.0.0)
+Requires-Dist: ipython (>=8.0.1,<9.0.0)
+Requires-Dist: numpy (>=1.22.2,<2.0.0)
+Requires-Dist: pandas
+Description-Content-Type: text/markdown
 
-packages = \
-['pythonquerylanguage']
 
-package_data = \
-{'': ['*']}
+# <b>Python Query Language PQL</b>
 
-install_requires = \
-['SQLAlchemy>=1.4.31,<2.0.0',
- 'ipython==8.0.1',
- 'numpy>=1.22.2,<2.0.0',
- 'pandas>=1.4.1,<2.0.0']
-
-setup_kwargs = {
-    'name': 'pythonquerylanguage',
-    'version': '0.1.6',
-    'description': 'Python SQL wrapper based on pandas and SQLalchemy',
-    'long_description': '\n# <b>Python Query Language PQL</b>\n\n<b>PQL</b> is a python wrapper of the sql sintax based in SQLalchemy and pandas, this code introduces a new syntax to use \nin your code when calling a database table.\n\n## Requirements\n\nYou only need a distribution of python3 installed.\n\n## ⚙️Installation:\n\nYou can install the requirements (preferably in an environment) using:\n\n> pip install PythonQueryLanguage\n\n## Basic Usage:\n\nPQL is managed by a class called SQLManager, to instanciated you will need to pass your connection strings in a dictionary\nand the enviroment you are willoing to use\n\n`\nconnection_dict = {\'test_env\': \'connection string from engine\',\n                   \'prod_env\': \'mssql+pyodbc://ur@prod.com/url2?driver=ODBC+Driver+17+for+SQL+Server\'\n                  }\nenv = \'test_env\'\npql = SQLManager(connection_dict,env)\n`\n\nOnce you have instanciated the class you can use it with his convenient functions that will wrap SQL expresions.\n\n> pql.select_all(\'tableA\',\'id\',\'myid\')  =  SELECT * FROM tableA WHERE id = \'myid\n\nPQL supports searchs in arrays:\n\n> pql.select_all(\'tableA\',\'id\',[\'myid\',\'myid2\'])  =  SELECT * FROM tableA WHERE id IN (\'myid\',\'myid2\')\n\nPQL cast the data in a inteligent manner:\n\n> pql.select_all(\'tableA\',[\'id\',\'name\'],[\'myid\',\'myName\'])  =  SELECT * FROM tableA WHERE id = \'myid\' AND myName = \'myid2\'\n\nPQL accepts adiotional arguments:\n\n> pql.select(\'column\',\'tableA\',[\'id\',\'name\'],[\'myid\',\'myName\'],\'OR\')  =  SELECT column FROM tableA WHERE id = \'myid\' OR myName = \'myid2\'\n\nPQL accepts direct evaluation or raw sql expressions (thougt only recommended in edge cases)\n\n> pql.query("SELECT * FROM tableA WHERE id = \'myid")  =  SELECT * FROM tableA WHERE id = \'myid\'\n\nPQL accepst function and Store procedure evaluations.\n\n## Multy enviroment usage.\n\nPQL is built to support working with different db environments at the same time, this multi enviroment work can be done in different ways:\n\n- 1. Instanciate the PQLmanager with different enviroments and run them.\n- 2. Changing the enviroment of the class with the change_enviroment method.\n- 3. Using scoped functions.\n\nExample of scoped functions:\n\nYou are working in a database test enviroment but you need to extract some data from the production enviroment without changing the enviroment of the PQLmanager\nThen you can query the table at producion using a scope:\n\n> pql.select_all(\'TableA\',env=\'prod\')\n\nThis function will run in the production environment and retrieve the information from it without changing your global environment.\n\n## IUD\n\nPQL supports Insert Update Delete Operations, all these operations are based in pandas dataframes.\n\n## Interactive.\n\nPQL is thought to be used in a jupyter notebook as well as used in real code. PQL contains different functionalities that allows the user\nto know what query will be executed in the database and confirmation security.\n\n',
-    'author': 'Pablo Ruiz',
-    'author_email': 'pablo.r.c@live.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+<b>PQL</b> is a python wrapper of the sql sintax based in SQLalchemy and pandas, this code introduces a new syntax to use 
+in your code when calling a database table.
+
+## Requirements
+
+You only need a distribution of python3 installed.
+
+## ⚙️Installation:
+
+You can install the requirements (preferably in an environment) using:
+
+> pip install PythonQueryLanguage
+
+## Basic Usage:
+
+PQL is managed by a class called SQLManager, to instanciated you will need to pass your connection strings in a dictionary
+and the enviroment you are willoing to use
+
+`
+connection_dict = {'test_env': 'connection string from engine',
+                   'prod_env': 'mssql+pyodbc://ur@prod.com/url2?driver=ODBC+Driver+17+for+SQL+Server'
+                  }
+env = 'test_env'
+pql = SQLManager(connection_dict,env)
+`
+
+Once you have instanciated the class you can use it with his convenient functions that will wrap SQL expresions.
+
+> pql.select_all('tableA','id','myid')  =  SELECT * FROM tableA WHERE id = 'myid
+
+PQL supports searchs in arrays:
+
+> pql.select_all('tableA','id',['myid','myid2'])  =  SELECT * FROM tableA WHERE id IN ('myid','myid2')
+
+PQL cast the data in a inteligent manner:
+
+> pql.select_all('tableA',['id','name'],['myid','myName'])  =  SELECT * FROM tableA WHERE id = 'myid' AND myName = 'myid2'
+
+PQL accepts adiotional arguments:
+
+> pql.select('column','tableA',['id','name'],['myid','myName'],'OR')  =  SELECT column FROM tableA WHERE id = 'myid' OR myName = 'myid2'
+
+PQL accepts direct evaluation or raw sql expressions (thougt only recommended in edge cases)
+
+> pql.query("SELECT * FROM tableA WHERE id = 'myid")  =  SELECT * FROM tableA WHERE id = 'myid'
+
+PQL accepst function and Store procedure evaluations.
+
+## Multy enviroment usage.
+
+PQL is built to support working with different db environments at the same time, this multi enviroment work can be done in different ways:
+
+- 1. Instanciate the PQLmanager with different enviroments and run them.
+- 2. Changing the enviroment of the class with the change_enviroment method.
+- 3. Using scoped functions.
+
+Example of scoped functions:
+
+You are working in a database test enviroment but you need to extract some data from the production enviroment without changing the enviroment of the PQLmanager
+Then you can query the table at producion using a scope:
+
+> pql.select_all('TableA',env='prod')
+
+This function will run in the production environment and retrieve the information from it without changing your global environment.
+
+## IUD
+
+PQL supports Insert Update Delete Operations, all these operations are based in pandas dataframes.
+
+## Interactive.
+
+PQL is thought to be used in a jupyter notebook as well as used in real code. PQL contains different functionalities that allows the user
+to know what query will be executed in the database and confirmation security.
 
 
-setup(**setup_kwargs)
```

