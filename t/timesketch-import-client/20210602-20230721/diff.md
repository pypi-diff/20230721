# Comparing `tmp/timesketch-import-client-20210602.tar.gz` & `tmp/timesketch-import-client-20230721.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/timesketch-import-client-20210602.tar", last modified: Fri Jun  4 12:21:46 2021, max compression
+gzip compressed data, was "timesketch-import-client-20230721.tar", last modified: Fri Jul 21 12:14:49 2023, max compression
```

## Comparing `timesketch-import-client-20210602.tar` & `timesketch-import-client-20230721.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-04 12:21:46.833992 timesketch-import-client-20210602/
--rw-r--r--   0 root         (0) root         (0)      477 2021-06-04 12:21:46.832992 timesketch-import-client-20210602/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2021-06-04 12:21:46.833992 timesketch-import-client-20210602/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1793 2021-06-04 12:16:25.000000 timesketch-import-client-20210602/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-04 12:21:46.829992 timesketch-import-client-20210602/timesketch_import_client/
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-04 12:16:25.000000 timesketch-import-client-20210602/timesketch_import_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-04 12:21:46.831992 timesketch-import-client-20210602/timesketch_import_client/data/
--rw-r--r--   0 root         (0) root         (0)     1973 2021-06-04 12:16:25.000000 timesketch-import-client-20210602/timesketch_import_client/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3022 2021-06-04 12:16:25.000000 timesketch-import-client-20210602/timesketch_import_client/data/formatter.yaml
--rw-r--r--   0 root         (0) root         (0)     5886 2021-06-04 12:16:25.000000 timesketch-import-client-20210602/timesketch_import_client/helper.py
--rw-r--r--   0 root         (0) root         (0)     4768 2021-06-04 12:16:25.000000 timesketch-import-client-20210602/timesketch_import_client/helper_test.py
--rw-r--r--   0 root         (0) root         (0)    30969 2021-06-04 12:16:25.000000 timesketch-import-client-20210602/timesketch_import_client/importer.py
--rw-r--r--   0 root         (0) root         (0)     6404 2021-06-04 12:16:25.000000 timesketch-import-client-20210602/timesketch_import_client/importer_test.py
--rw-r--r--   0 root         (0) root         (0)     4018 2021-06-04 12:16:25.000000 timesketch-import-client-20210602/timesketch_import_client/utils.py
--rw-r--r--   0 root         (0) root         (0)      765 2021-06-04 12:16:25.000000 timesketch-import-client-20210602/timesketch_import_client/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-04 12:21:46.831992 timesketch-import-client-20210602/timesketch_import_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      477 2021-06-04 12:21:46.000000 timesketch-import-client-20210602/timesketch_import_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2021-06-04 12:21:46.000000 timesketch-import-client-20210602/timesketch_import_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-06-04 12:21:46.000000 timesketch-import-client-20210602/timesketch_import_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2021-06-04 12:21:46.000000 timesketch-import-client-20210602/timesketch_import_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-06-04 12:21:46.000000 timesketch-import-client-20210602/timesketch_import_client.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       41 2021-06-04 12:21:46.000000 timesketch-import-client-20210602/timesketch_import_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2021-06-04 12:21:46.000000 timesketch-import-client-20210602/timesketch_import_client.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-04 12:21:46.832992 timesketch-import-client-20210602/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-04 12:16:25.000000 timesketch-import-client-20210602/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18952 2021-06-04 12:16:25.000000 timesketch-import-client-20210602/tools/timesketch_importer.py
+drwxr-x---   0 jbn      (190240) primarygroup (89939)        0 2023-07-21 12:14:49.049951 timesketch-import-client-20230721/
+-rw-r-----   0 jbn      (190240) primarygroup (89939)      438 2023-07-21 12:14:49.049951 timesketch-import-client-20230721/PKG-INFO
+-rw-r-----   0 jbn      (190240) primarygroup (89939)       38 2023-07-21 12:14:49.049951 timesketch-import-client-20230721/setup.cfg
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     1802 2022-05-04 12:34:04.000000 timesketch-import-client-20230721/setup.py
+drwxr-x---   0 jbn      (190240) primarygroup (89939)        0 2023-07-21 12:14:48.989946 timesketch-import-client-20230721/timesketch_import_client/
+-rw-r-----   0 jbn      (190240) primarygroup (89939)        0 2021-02-05 08:50:03.000000 timesketch-import-client-20230721/timesketch_import_client/__init__.py
+drwxr-x---   0 jbn      (190240) primarygroup (89939)        0 2023-07-21 12:14:49.021949 timesketch-import-client-20230721/timesketch_import_client/data/
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     1972 2022-05-04 12:34:04.000000 timesketch-import-client-20230721/timesketch_import_client/data/__init__.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     3022 2021-02-05 08:50:03.000000 timesketch-import-client-20230721/timesketch_import_client/data/formatter.yaml
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     5897 2023-05-26 10:36:03.000000 timesketch-import-client-20230721/timesketch_import_client/helper.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     4792 2022-05-04 12:34:04.000000 timesketch-import-client-20230721/timesketch_import_client/helper_test.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)    31713 2022-05-04 12:34:04.000000 timesketch-import-client-20230721/timesketch_import_client/importer.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     6646 2022-05-04 12:34:04.000000 timesketch-import-client-20230721/timesketch_import_client/importer_test.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)     4064 2022-05-04 12:34:04.000000 timesketch-import-client-20230721/timesketch_import_client/utils.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)      765 2023-07-21 11:58:10.000000 timesketch-import-client-20230721/timesketch_import_client/version.py
+drwxr-x---   0 jbn      (190240) primarygroup (89939)        0 2023-07-21 12:14:49.021949 timesketch-import-client-20230721/timesketch_import_client.egg-info/
+-rw-r--r--   0 jbn      (190240) primarygroup (89939)      438 2023-07-21 12:14:48.000000 timesketch-import-client-20230721/timesketch_import_client.egg-info/PKG-INFO
+-rw-r--r--   0 jbn      (190240) primarygroup (89939)      740 2023-07-21 12:14:48.000000 timesketch-import-client-20230721/timesketch_import_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jbn      (190240) primarygroup (89939)        1 2023-07-21 12:14:48.000000 timesketch-import-client-20230721/timesketch_import_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jbn      (190240) primarygroup (89939)       71 2023-07-21 12:14:48.000000 timesketch-import-client-20230721/timesketch_import_client.egg-info/entry_points.txt
+-rw-r--r--   0 jbn      (190240) primarygroup (89939)        1 2022-01-20 08:42:08.000000 timesketch-import-client-20230721/timesketch_import_client.egg-info/not-zip-safe
+-rw-r--r--   0 jbn      (190240) primarygroup (89939)       41 2023-07-21 12:14:48.000000 timesketch-import-client-20230721/timesketch_import_client.egg-info/requires.txt
+-rw-r--r--   0 jbn      (190240) primarygroup (89939)       31 2023-07-21 12:14:48.000000 timesketch-import-client-20230721/timesketch_import_client.egg-info/top_level.txt
+drwxr-x---   0 jbn      (190240) primarygroup (89939)        0 2023-07-21 12:14:49.049951 timesketch-import-client-20230721/tools/
+-rw-r-----   0 jbn      (190240) primarygroup (89939)        0 2021-02-05 08:50:03.000000 timesketch-import-client-20230721/tools/__init__.py
+-rw-r-----   0 jbn      (190240) primarygroup (89939)    20361 2023-05-26 10:36:03.000000 timesketch-import-client-20230721/tools/timesketch_importer.py
```

### Comparing `timesketch-import-client-20210602/setup.py` & `timesketch-import-client-20230721/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,37 +20,38 @@
 
 from setuptools import find_packages
 from setuptools import setup
 
 from timesketch_import_client import version
 
 setup(
-    name='timesketch-import-client',
+    name="timesketch-import-client",
     version=version.get_version(),
-    description='Timesketch Import Client',
-    license='Apache License, Version 2.0',
-    url='http://www.timesketch.org/',
-    maintainer='Timesketch development team',
-    maintainer_email='timesketch-dev@googlegroups.com',
+    description="Timesketch Import Client",
+    license="Apache License, Version 2.0",
+    url="http://www.timesketch.org/",
+    maintainer="Timesketch development team",
+    maintainer_email="timesketch-dev@googlegroups.com",
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Environment :: Console',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
+        "Development Status :: 4 - Beta",
+        "Environment :: Console",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
     ],
     data_files=[
-        ('data', glob.glob(
-            os.path.join('timesketch_import_client', 'data', '*.yaml'))),
+        ("data", glob.glob(os.path.join("timesketch_import_client", "data", "*.yaml"))),
     ],
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     entry_points={
-        'console_scripts': [
-            'timesketch_importer = tools.timesketch_importer:main']},
-    install_requires=frozenset([
-        'pandas',
-        'xlrd',
-        'timesketch-api-client',
-        'pyyaml',
-    ]),
-    )
+        "console_scripts": ["timesketch_importer = tools.timesketch_importer:main"]
+    },
+    install_requires=frozenset(
+        [
+            "pandas",
+            "xlrd",
+            "timesketch-api-client",
+            "pyyaml",
+        ]
+    ),
+)
```

### Comparing `timesketch-import-client-20210602/timesketch_import_client/data/__init__.py` & `timesketch-import-client-20230721/timesketch_import_client/data/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 import codecs
 import logging
 import os
 
 import yaml
 
 
-logger = logging.getLogger('timesketch_importer.config_loader')
+logger = logging.getLogger("timesketch_importer.config_loader")
 
-DEFAULT_FILE = 'formatter.yaml'
+DEFAULT_FILE = "formatter.yaml"
 
 
-def load_config(file_path=''):
+def load_config(file_path=""):
     """Loads YAML config and returns a list of dict with the results.
 
     Args:
         file_path (str): path to the YAML config file. This is optional
             and if not defined the default formatter.yaml file will be
             used that comes with the tool.
 
@@ -38,24 +38,24 @@
         dict: a dict with the key being a config file identifier and the value
         being another dict with the configuration items.
     """
     if not file_path:
         base_path = os.path.dirname(__file__)
         file_path = os.path.join(base_path, DEFAULT_FILE)
 
-    if not file_path.endswith('.yaml'):
-        logger.error('Can\'t load a config that is not a YAML file.')
+    if not file_path.endswith(".yaml"):
+        logger.error("Can't load a config that is not a YAML file.")
         return {}
 
     if not os.path.isfile(file_path):
-        logger.error('File path does not exist, unable to load YAML config.')
+        logger.error("File path does not exist, unable to load YAML config.")
         return {}
 
-    with codecs.open(file_path, 'r') as fh:
+    with codecs.open(file_path, "r") as fh:
         try:
             data = yaml.safe_load(fh)
             return data
         except (AttributeError, yaml.parser.ParserError) as e:
-            logger.error('Unable to parse YAML file, with error: %s', e)
+            logger.error("Unable to parse YAML file, with error: %s", e)
             return {}
 
     return {}
```

### Comparing `timesketch-import-client-20210602/timesketch_import_client/data/formatter.yaml` & `timesketch-import-client-20230721/timesketch_import_client/data/formatter.yaml`

 * *Files identical despite different names*

### Comparing `timesketch-import-client-20210602/timesketch_import_client/helper.py` & `timesketch-import-client-20230721/timesketch_import_client/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import logging
 import os
 
 from timesketch_import_client import data as data_config
 
 
-logger = logging.getLogger('timesketch_importer.ts_import_helper')
+logger = logging.getLogger("timesketch_importer.ts_import_helper")
 
 
 class ImportHelper:
     """Import helper class."""
 
     def __init__(self, load_default=True):
         """Initialize the helper class."""
@@ -37,31 +37,31 @@
         """Sets up the streamer based on a configuration dict.
 
         Args:
             streamer (ImportStreamer): an import streamer object.
             config_dict (dict): A dictionary that contains
                 configuration details for the streamer.
         """
-        message = config_dict.get('message')
+        message = config_dict.get("message")
         if message:
             streamer.set_message_format_string(message)
 
-        timestamp_desc = config_dict.get('timestamp_desc')
+        timestamp_desc = config_dict.get("timestamp_desc")
         if timestamp_desc:
             streamer.set_timestamp_description(timestamp_desc)
 
-        separator = config_dict.get('separator')
+        separator = config_dict.get("separator")
         if separator:
             streamer.set_csv_delimiter(separator)
 
-        encoding = config_dict.get('encoding')
+        encoding = config_dict.get("encoding")
         if encoding:
             streamer.set_text_encoding(encoding)
 
-        datetime_string = config_dict.get('datetime')
+        datetime_string = config_dict.get("datetime")
         if datetime_string:
             streamer.set_datetime_column(datetime_string)
 
     def add_config(self, file_path):
         """Loads a YAML config file describing the log file config.
 
         This function reads a YAML config file, and adds the config
@@ -73,47 +73,48 @@
 
         Raises:
             ValueError: if the file path does not exist or if the config
                         is not valid or cannot be read.
         """
         if not os.path.isfile(file_path):
             raise ValueError(
-                'Unable to open file: [{0:s}], it does not exist.'.format(
-                    file_path))
+                "Unable to open file: [{0:s}], it does not exist.".format(file_path)
+            )
 
         if not os.access(file_path, os.R_OK):
             raise ValueError(
-                'Unable to open file: [{0:s}], cannot open it for '
-                'read, please check permissions.'.format(file_path))
-
+                "Unable to open file: [{0:s}], cannot open it for "
+                "read, please check permissions.".format(file_path)
+            )
 
         config = data_config.load_config(file_path)
         if not isinstance(config, dict):
             raise ValueError(
-                'Unable to read config file since it does not produce a dict')
+                "Unable to read config file since it does not produce a dict"
+            )
 
         if not all([isinstance(x, dict) for x in config.values()]):
             raise ValueError(
-                'The config needs to a dict that contains other dict '
-                'attributes.')
+                "The config needs to a dict that contains other dict attributes."
+            )
 
         self._data.update(config)
 
-    def add_config_dict(self, config, config_name='manual'):
+    def add_config_dict(self, config, config_name="manual"):
         """Add a config dict describing the log file config.
 
         Args:
             config (dict): a single dict with the config needed for setting
                 up the streamer.
             config_name (str): the name of the config to be added. This is
                 optional, with the default value set to "manual".
         """
         self._data[config_name] = config
 
-    def configure_streamer(self, streamer, data_type='', columns=None):
+    def configure_streamer(self, streamer, data_type="", columns=None):
         """Go through loaded config and setup a streamer if there is a match.
 
         This function takes a streamer object and compares the loaded config
         to see if there is a match to the data_type and/or columns that are
         supplied to the function and sets the streamer up if a matching
         config is discovered.
 
@@ -123,33 +124,33 @@
         Args:
             streamer (ImportStreamer): an import streamer object.
             data_type (str): optional data type that is used for matching
                 with the loaded config.
             columns (List[str]): optional list of strings with column names.
         """
         for config_name, config in self._data.items():
-            conf_data_type = config.get('data_type')
+            conf_data_type = config.get("data_type")
             if data_type and conf_data_type and conf_data_type == data_type:
-                logger.info('Using config %s for streamer.', config_name)
+                logger.info("Using config %s for streamer.", config_name)
                 self._configure_streamer(streamer, config)
                 return
 
             if not columns:
                 continue
 
             column_set = set(columns)
-            column_string = config.get('columns', '')
-            column_subset_string = config.get('columns_subset', '')
+            column_string = config.get("columns", "")
+            column_subset_string = config.get("columns_subset", "")
             if not any([column_string, column_subset_string]):
                 continue
 
-            conf_columns = set(column_string.split(','))
+            conf_columns = set(column_string.split(","))
             if conf_columns and column_set == conf_columns:
-                logger.info('Using config %s for streamer.', config_name)
+                logger.info("Using config %s for streamer.", config_name)
                 self._configure_streamer(streamer, config)
                 return
 
-            columns_subset = set(column_subset_string.split(','))
+            columns_subset = set(column_subset_string.split(","))
             if columns_subset and columns_subset.issubset(column_set):
-                logger.info('Using config %s for streamer.', config_name)
+                logger.info("Using config %s for streamer.", config_name)
                 self._configure_streamer(streamer, config)
                 return
```

### Comparing `timesketch-import-client-20210602/timesketch_import_client/helper_test.py` & `timesketch-import-client-20230721/timesketch_import_client/helper_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,24 +36,25 @@
 
 vindur:
         message: 'Vedrid i dag er: {vedur}, med typiskri {auka}'
         timestamp_desc: 'Thu Veist Thad'
         columns: 'vedur,magn,auka,rigning'
 """
 
+
 class MockStreamer:
     """Mock streamer object for testing."""
 
     def __init__(self):
         """Initialize."""
-        self.format_string = ''
-        self.timestamp_description = ''
-        self.csv_delimiter = ''
-        self.text_encoding = ''
-        self.datetime_column = ''
+        self.format_string = ""
+        self.timestamp_description = ""
+        self.csv_delimiter = ""
+        self.text_encoding = ""
+        self.datetime_column = ""
 
     def set_message_format_string(self, message):
         self.format_string = message
 
     def set_timestamp_description(self, timestamp_desc):
         self.timestamp_description = timestamp_desc
 
@@ -69,67 +70,70 @@
 
 class TimesketchHelperTest(unittest.TestCase):
     """Test Timesketch import helper."""
 
     def setUp(self):
         """Set up the test."""
         self._helper = helper.ImportHelper()
-        with tempfile.NamedTemporaryFile('w', suffix='.yaml') as fw:
+        with tempfile.NamedTemporaryFile("w", suffix=".yaml") as fw:
             fw.write(MOCK_CONFIG)
             fw.seek(0)
             self._helper.add_config(fw.name)
 
     def test_not_config(self):
         """Test a helper that does not match."""
         streamer = MockStreamer()
-        self._helper.configure_streamer(streamer, data_type='foo:no')
+        self._helper.configure_streamer(streamer, data_type="foo:no")
 
-        self.assertEqual(streamer.format_string, '')
-        self.assertEqual(streamer.timestamp_description, '')
-        self.assertEqual(streamer.csv_delimiter, '')
-        self.assertEqual(streamer.text_encoding, '')
-        self.assertEqual(streamer.datetime_column, '')
+        self.assertEqual(streamer.format_string, "")
+        self.assertEqual(streamer.timestamp_description, "")
+        self.assertEqual(streamer.csv_delimiter, "")
+        self.assertEqual(streamer.text_encoding, "")
+        self.assertEqual(streamer.datetime_column, "")
 
     def test_sub_column(self):
         """Test a helper that matches on sub columns."""
         streamer = MockStreamer()
         self._helper.configure_streamer(
-            streamer, data_type='foo:no',
-            columns=['cA', 'cB', 'cC', 'cD', 'cE', 'cF', 'cG'])
+            streamer,
+            data_type="foo:no",
+            columns=["cA", "cB", "cC", "cD", "cE", "cF", "cG"],
+        )
 
         self.assertEqual(
             streamer.format_string,
-            'The {cA} went bananas with {cC}, but without letting {cD} know.')
-        self.assertEqual(streamer.timestamp_description, 'Event Logged')
-        self.assertEqual(streamer.csv_delimiter, '')
-        self.assertEqual(streamer.text_encoding, '')
-        self.assertEqual(streamer.datetime_column, 'cB')
+            "The {cA} went bananas with {cC}, but without letting {cD} know.",
+        )
+        self.assertEqual(streamer.timestamp_description, "Event Logged")
+        self.assertEqual(streamer.csv_delimiter, "")
+        self.assertEqual(streamer.text_encoding, "")
+        self.assertEqual(streamer.datetime_column, "cB")
 
     def test_columns(self):
         """Test a helper that matches on columns."""
         streamer = MockStreamer()
         self._helper.configure_streamer(
-            streamer, data_type='foo:no',
-            columns=['vedur', 'magn', 'auka', 'rigning'])
+            streamer, data_type="foo:no", columns=["vedur", "magn", "auka", "rigning"]
+        )
 
         self.assertEqual(
-            streamer.format_string,
-            'Vedrid i dag er: {vedur}, med typiskri {auka}')
-        self.assertEqual(streamer.timestamp_description, 'Thu Veist Thad')
-        self.assertEqual(streamer.csv_delimiter, '')
-        self.assertEqual(streamer.text_encoding, '')
-        self.assertEqual(streamer.datetime_column, '')
+            streamer.format_string, "Vedrid i dag er: {vedur}, med typiskri {auka}"
+        )
+        self.assertEqual(streamer.timestamp_description, "Thu Veist Thad")
+        self.assertEqual(streamer.csv_delimiter, "")
+        self.assertEqual(streamer.text_encoding, "")
+        self.assertEqual(streamer.datetime_column, "")
 
     def test_data_type(self):
         """Test a helper that matches on data_type."""
         streamer = MockStreamer()
         self._helper.configure_streamer(
-            streamer, data_type='data:secret:message',
-            columns=['vedur', 'auka', 'rigning'])
-
-        self.assertEqual(
-            streamer.format_string,
-            'Some people {stuff}, with {other}')
-        self.assertEqual(streamer.timestamp_description, 'Stuff Happened')
-        self.assertEqual(streamer.csv_delimiter, '>')
-        self.assertEqual(streamer.text_encoding, 'secret-formula')
-        self.assertEqual(streamer.datetime_column, '')
+            streamer,
+            data_type="data:secret:message",
+            columns=["vedur", "auka", "rigning"],
+        )
+
+        self.assertEqual(streamer.format_string, "Some people {stuff}, with {other}")
+        self.assertEqual(streamer.timestamp_description, "Stuff Happened")
+        self.assertEqual(streamer.csv_delimiter, ">")
+        self.assertEqual(streamer.text_encoding, "secret-formula")
+        self.assertEqual(streamer.datetime_column, "")
```

### Comparing `timesketch-import-client-20210602/timesketch_import_client/importer.py` & `timesketch-import-client-20230721/timesketch_import_client/importer.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,55 +26,55 @@
 import numpy
 import pandas
 
 from timesketch_api_client import timeline
 from timesketch_api_client import definitions
 from timesketch_import_client import utils
 
-logger = logging.getLogger('timesketch_importer.importer')
+logger = logging.getLogger("timesketch_importer.importer")
 
 
 class ImportStreamer(object):
     """Upload object used to stream results to Timesketch."""
 
     # The number of entries before automatically flushing
     # the streamer.
     DEFAULT_ENTRY_THRESHOLD = 50000
 
     # Number of bytes in a binary file before automatically
     # chunking it up into smaller pieces.
     DEFAULT_FILESIZE_THRESHOLD = 104857600  # 100 Mb.
 
     # Define default values.
-    DEFAULT_TEXT_ENCODING = 'utf-8'
-    DEFAULT_TIMESTAMP_DESC = 'Time Logged'
+    DEFAULT_TEXT_ENCODING = "utf-8"
+    DEFAULT_TIMESTAMP_DESC = "Time Logged"
 
     # Define the maximum amount of retries for a file/chunk upload.
     DEFAULT_RETRY_LIMIT = 3
 
     def __init__(self):
         """Initialize the upload streamer."""
-        self._celery_task_id = ''
+        self._celery_task_id = ""
         self._count = 0
         self._config_helper = None
-        self._data_label = ''
+        self._data_label = ""
         self._dict_config_loaded = False
         self._csv_delimiter = None
         self._data_lines = []
         self._data_type = None
         self._datetime_field = None
         self._format_string = None
-        self._index = ''
+        self._index = ""
         self._last_response = None
-        self._provider = 'Importer library'
-        self._resource_url = ''
+        self._provider = "Importer library"
+        self._resource_url = ""
         self._sketch = None
         self._timeline_id = None
         self._timeline_name = None
-        self._upload_context = ''
+        self._upload_context = ""
 
         self._chunk = 1
 
         self._text_encoding = self.DEFAULT_TEXT_ENCODING
         self._timestamp_desc = self.DEFAULT_TIMESTAMP_DESC
         self._threshold_entry = self.DEFAULT_ENTRY_THRESHOLD
         self._threshold_filesize = self.DEFAULT_FILESIZE_THRESHOLD
@@ -91,135 +91,143 @@
               is added.
           * All keys that start with an underscore ("_") are removed.
 
         Args:
             my_dict: a dictionary that may be missing few fields needed
                     for Timesketch.
         """
-        if 'message' not in my_dict:
-            format_string = (
-                self._format_string or utils.get_combined_message_string(
-                    mydict=my_dict))
-            my_dict['message'] = format_string.format(**my_dict)
+        if "message" not in my_dict:
+            format_string = self._format_string or utils.get_combined_message_string(
+                mydict=my_dict
+            )
+            my_dict["message"] = format_string.format(**my_dict)
 
-        _ = my_dict.setdefault('timestamp_desc', self._timestamp_desc)
+        _ = my_dict.setdefault("timestamp_desc", self._timestamp_desc)
         if self._data_type:
-            _ = my_dict.setdefault('data_type', self._data_type)
+            _ = my_dict.setdefault("data_type", self._data_type)
 
-        if 'datetime' not in my_dict:
-            date = ''
+        if "datetime" not in my_dict:
+            date = ""
             if self._datetime_field:
                 value = my_dict.get(self._datetime_field)
                 if value:
                     date = utils.get_datestring_from_value(value)
             if not date:
                 for key in my_dict:
                     key_string = key.lower()
-                    if 'time' not in key_string:
+                    if "time" not in key_string:
                         continue
 
-                    if key_string == 'timestamp_desc':
+                    if key_string == "timestamp_desc":
                         continue
 
                     value = my_dict[key]
                     date = utils.get_datestring_from_value(value)
                     if date:
                         break
 
             if date:
-                my_dict['datetime'] = date
+                my_dict["datetime"] = date
         else:
-            my_dict['datetime'] = utils.get_datestring_from_value(
-                my_dict['datetime'])
+            my_dict["datetime"] = utils.get_datestring_from_value(my_dict["datetime"])
 
         # We don't want to include any columns that start with an underscore.
-        underscore_columns = [x for x in my_dict if x.startswith('_')]
+        underscore_columns = [x for x in my_dict if x.startswith("_")]
         if underscore_columns:
             for column in underscore_columns:
                 del my_dict[column]
 
     def _fix_data_frame(self, data_frame):
         """Returns a data frame with added columns for Timesketch upload.
 
         Args:
             data_frame: a pandas data frame.
 
         Returns:
             A pandas data frame with added columns needed for Timesketch.
         """
-        if 'message' not in data_frame:
-            format_string = (
-                self._format_string or utils.get_combined_message_string(
-                    dataframe=data_frame))
+        if "message" not in data_frame:
+            format_string = self._format_string or utils.get_combined_message_string(
+                dataframe=data_frame
+            )
             utils.format_data_frame(data_frame, format_string)
 
-        if 'timestamp_desc' not in data_frame:
-            data_frame['timestamp_desc'] = self._timestamp_desc
+        if "timestamp_desc" not in data_frame:
+            data_frame["timestamp_desc"] = self._timestamp_desc
 
-        if self._data_type and 'data_type' not in data_frame:
-            data_frame['data_type'] = self._data_type
+        if self._data_type and "data_type" not in data_frame:
+            data_frame["data_type"] = self._data_type
 
-        if 'datetime' not in data_frame:
+        if "datetime" not in data_frame:
             if self._datetime_field and self._datetime_field in data_frame:
                 try:
-                    data_frame['timestamp'] = pandas.to_datetime(
-                        data_frame[self._datetime_field], utc=True)
+                    data_frame["timestamp"] = pandas.to_datetime(
+                        data_frame[self._datetime_field], utc=True
+                    )
                 except ValueError as e:
                     logger.info(
-                        'Unable to convert timestamp in column: %s, error %s',
-                        self._datetime_field, e)
+                        "Unable to convert timestamp in column: %s, error %s",
+                        self._datetime_field,
+                        e,
+                    )
             else:
                 for column in data_frame.columns[
-                        data_frame.columns.str.contains('time', case=False)]:
-                    if column.lower() == 'timestamp_desc':
+                    data_frame.columns.str.contains("time", case=False)
+                ]:
+                    if column.lower() == "timestamp_desc":
                         continue
                     try:
-                        data_frame['timestamp'] = pandas.to_datetime(
-                            data_frame[column], utc=True)
+                        data_frame["timestamp"] = pandas.to_datetime(
+                            data_frame[column], utc=True
+                        )
                         # We want the first successful timestamp value.
                         break
                     except ValueError as e:
                         logger.info(
-                            'Unable to convert timestamp in column: '
-                            '%s, error %s', column, e)
-
-            if 'timestamp' in data_frame:
-                data_frame['datetime'] = data_frame['timestamp'].dt.strftime(
-                    '%Y-%m-%dT%H:%M:%S%z')
-                data_frame['timestamp'] = data_frame[
-                    'timestamp'].astype(numpy.int64) / 1e9
+                            "Unable to convert timestamp in column: " "%s, error %s",
+                            column,
+                            e,
+                        )
+
+            if "timestamp" in data_frame:
+                data_frame["datetime"] = data_frame["timestamp"].dt.strftime(
+                    "%Y-%m-%dT%H:%M:%S%z"
+                )
+                data_frame["timestamp"] = (
+                    data_frame["timestamp"].astype(numpy.int64) / 1e9
+                )
         else:
             try:
-                date = pandas.to_datetime(data_frame['datetime'], utc=True)
-                data_frame['datetime'] = date.dt.strftime('%Y-%m-%dT%H:%M:%S%z')
+                date = pandas.to_datetime(data_frame["datetime"], utc=True)
+                data_frame["datetime"] = date.dt.strftime("%Y-%m-%dT%H:%M:%S%z")
             except Exception:  # pylint: disable=broad-except
                 logger.error(
-                    'Unable to change datetime, is it badly formed?',
-                    exc_info=True)
+                    "Unable to change datetime, is it badly formed?", exc_info=True
+                )
 
         # TODO: Support labels in uploads/imports.
-        if 'label' in data_frame:
-            del data_frame['label']
+        if "label" in data_frame:
+            del data_frame["label"]
             logger.warning(
-                'Labels cannot be imported at this time. Therefore the '
-                'label column was dropped from the dataset.')
+                "Labels cannot be imported at this time. Therefore the "
+                "label column was dropped from the dataset."
+            )
 
         # We don't want to include any columns that start with an underscore.
-        columns = list(
-            data_frame.columns[~data_frame.columns.str.contains('^_')])
+        columns = list(data_frame.columns[~data_frame.columns.str.contains("^_")])
         return data_frame[columns]
 
     def _ready(self):
         """Check whether all variables have been set.
 
         Raises:
             ValueError: if the streamer has not yet been fully configured.
         """
         if self._sketch is None:
-            raise ValueError('Sketch has not yet been set.')
+            raise ValueError("Sketch has not yet been set.")
 
     def _reset(self):
         """Reset the buffer."""
         self._count = 0
         self._data_lines = []
 
     def _upload_data_buffer(self, end_stream, retry_count=0):
@@ -235,66 +243,76 @@
             RuntimeError: If the data buffer is not successfully uploaded.
         """
         if not self._data_lines:
             return None
 
         start_time = time.time()
         data = {
-            'name': self._timeline_name,
-            'sketch_id': self._sketch.id,
-            'enable_stream': not end_stream,
-            'data_label': self._data_label,
-            'provider': self._provider,
-            'events': '\n'.join([json.dumps(x) for x in self._data_lines]),
+            "name": self._timeline_name,
+            "sketch_id": self._sketch.id,
+            "enable_stream": not end_stream,
+            "data_label": self._data_label,
+            "provider": self._provider,
+            "events": "\n".join([json.dumps(x) for x in self._data_lines]),
         }
         if self._index:
-            data['index_name'] = self._index
+            data["index_name"] = self._index
 
         if self._upload_context:
-            data['context'] = self._upload_context
+            data["context"] = self._upload_context
 
         logger.debug(
-            'Data buffer ready for upload, took {0:.2f} seconds to '
-            'prepare.'.format(time.time() - start_time))
+            "Data buffer ready for upload, took {0:.2f} seconds to "
+            "prepare.".format(time.time() - start_time)
+        )
 
         response = self._sketch.api.session.post(self._resource_url, data=data)
 
         # TODO: Investigate why the sleep is needed, fix the underlying issue
         # and get rid of it here.
         # To prevent unexpected errors with connection refusal adding a quick
         # sleep.
         time.sleep(2)
 
         if response.status_code not in definitions.HTTP_STATUS_CODE_20X:
             if retry_count >= self.DEFAULT_RETRY_LIMIT:
                 raise RuntimeError(
-                    'Error uploading data: [{0:d}] {1!s} {2!s}, '
-                    'index {3:s}'.format(
-                        response.status_code, response.reason, response.text,
-                        self._index))
+                    "Error uploading data: [{0:d}] {1!s} {2!s}, "
+                    "index {3:s}".format(
+                        response.status_code,
+                        response.reason,
+                        response.text,
+                        self._index,
+                    )
+                )
 
             logger.warning(
-                'Unable to upload data buffer: {0:d}, retrying (attempt '
-                '{1:d}/{2:d})'.format(
-                    self._chunk, retry_count + 1, self.DEFAULT_RETRY_LIMIT))
+                "Unable to upload data buffer: {0:d}, retrying (attempt "
+                "{1:d}/{2:d})".format(
+                    self._chunk, retry_count + 1, self.DEFAULT_RETRY_LIMIT
+                )
+            )
 
             return self._upload_data_buffer(
-                end_stream=end_stream, retry_count=retry_count + 1)
+                end_stream=end_stream, retry_count=retry_count + 1
+            )
 
         logger.debug(
-            'Data buffer nr. {0:d} uploaded, total time: {1:.2f}s'.format(
-                self._chunk, time.time() - start_time))
+            "Data buffer nr. {0:d} uploaded, total time: {1:.2f}s".format(
+                self._chunk, time.time() - start_time
+            )
+        )
         self._chunk += 1
         response_dict = response.json()
-        object_dict = response_dict.get('objects', [{}])[0]
-        meta_dict = response_dict.get('meta', {})
-        self._celery_task_id = meta_dict.get('task_id', '')
+        object_dict = response_dict.get("objects", [{}])[0]
+        meta_dict = response_dict.get("meta", {})
+        self._celery_task_id = meta_dict.get("task_id", "")
 
-        self._timeline_id = object_dict.get('id')
-        self._index = object_dict.get('searchindex', {}).get('index_name')
+        self._timeline_id = object_dict.get("id")
+        self._index = object_dict.get("searchindex", {}).get("index_name")
         self._last_response = response_dict
 
         return None
 
     def _upload_data_frame(self, data_frame, end_stream, retry_count=0):
         """Upload data to Timesketch.
 
@@ -305,53 +323,59 @@
             retry_count: optional int that is only set if this is a retry
                 of the upload.
 
         Raises:
             RuntimeError: If the dataframe is not successfully uploaded.
         """
         data = {
-            'name': self._timeline_name,
-            'sketch_id': self._sketch.id,
-            'enable_stream': not end_stream,
-            'data_label': self._data_label,
-            'provider': self._provider,
-            'events': data_frame.to_json(orient='records', lines=True),
+            "name": self._timeline_name,
+            "sketch_id": self._sketch.id,
+            "enable_stream": not end_stream,
+            "data_label": self._data_label,
+            "provider": self._provider,
+            "events": data_frame.to_json(orient="records", lines=True),
         }
         if self._index:
-            data['index_name'] = self._index
+            data["index_name"] = self._index
 
         if self._upload_context:
-            data['context'] = self._upload_context
+            data["context"] = self._upload_context
 
         response = self._sketch.api.session.post(self._resource_url, data=data)
         if response.status_code not in definitions.HTTP_STATUS_CODE_20X:
             if retry_count >= self.DEFAULT_RETRY_LIMIT:
                 raise RuntimeError(
-                    'Error uploading data: [{0:d}] {1!s} {2!s}, '
-                    'index {3:s}'.format(
-                        response.status_code, response.reason, response.text,
-                        self._index))
+                    "Error uploading data: [{0:d}] {1!s} {2!s}, "
+                    "index {3:s}".format(
+                        response.status_code,
+                        response.reason,
+                        response.text,
+                        self._index,
+                    )
+                )
 
             logger.warning(
-                'Unable to upload dataframe, retrying (attempt '
-                '{0:d}/{1:d})'.format(
-                    retry_count + 1, self.DEFAULT_RETRY_LIMIT))
+                "Unable to upload dataframe, retrying (attempt "
+                "{0:d}/{1:d})".format(retry_count + 1, self.DEFAULT_RETRY_LIMIT)
+            )
 
             return self._upload_data_frame(
-                data_frame=data_frame, end_stream=end_stream,
-                retry_count=retry_count + 1)
+                data_frame=data_frame,
+                end_stream=end_stream,
+                retry_count=retry_count + 1,
+            )
 
         self._chunk += 1
         response_dict = response.json()
-        object_dict = response_dict.get('objects', [{}])[0]
-        meta_dict = response_dict.get('meta', {})
-        self._celery_task_id = meta_dict.get('task_id', '')
+        object_dict = response_dict.get("objects", [{}])[0]
+        meta_dict = response_dict.get("meta", {})
+        self._celery_task_id = meta_dict.get("task_id", "")
 
-        self._timeline_id = object_dict.get('id')
-        self._index = object_dict.get('searchindex', {}).get('index_name')
+        self._timeline_id = object_dict.get("id")
+        self._index = object_dict.get("searchindex", {}).get("index_name")
         self._last_response = response_dict
         return None
 
     def _upload_binary_file(self, file_path):
         """Upload binary data to Timesketch, potentially chunking it up.
 
         Args:
@@ -359,88 +383,99 @@
         """
         file_size = os.path.getsize(file_path)
 
         if self._timeline_name:
             timeline_name = self._timeline_name
         else:
             file_name = os.path.basename(file_path)
-            file_name_no_ext, _, _ = file_name.rpartition('.')
+            file_name_no_ext, _, _ = file_name.rpartition(".")
             timeline_name = file_name_no_ext
 
         data = {
-            'name': timeline_name,
-            'sketch_id': self._sketch.id,
-            'total_file_size': file_size,
-            'provider': self._provider,
-            'data_label': self._data_label,
+            "name": timeline_name,
+            "sketch_id": self._sketch.id,
+            "total_file_size": file_size,
+            "provider": self._provider,
+            "data_label": self._data_label,
         }
         if self._index:
-            data['index_name'] = self._index
+            data["index_name"] = self._index
 
         if self._upload_context:
-            data['context'] = self._upload_context
+            data["context"] = self._upload_context
 
         if file_size <= self._threshold_filesize:
-            file_dict = {
-                'file': open(file_path, 'rb')}
+            file_dict = {"file": open(file_path, "rb")}
             response = self._sketch.api.session.post(
-                self._resource_url, files=file_dict, data=data)
+                self._resource_url, files=file_dict, data=data
+            )
         else:
-            chunks = int(
-                math.ceil(float(file_size) / self._threshold_filesize))
-            data['chunk_total_chunks'] = chunks
-            data['chunk_index_name'] = uuid.uuid4().hex
+            chunks = int(math.ceil(float(file_size) / self._threshold_filesize))
+            data["chunk_total_chunks"] = chunks
+            data["chunk_index_name"] = uuid.uuid4().hex
 
             for index in range(0, chunks):
-                data['chunk_index'] = index
+                data["chunk_index"] = index
                 start = self._threshold_filesize * index
-                data['chunk_byte_offset'] = start
-                fh = open(file_path, 'rb')
+                data["chunk_byte_offset"] = start
+                fh = open(file_path, "rb")
                 fh.seek(start)
                 binary_data = fh.read(self._threshold_filesize)
                 file_stream = io.BytesIO(binary_data)
                 file_stream.name = file_path
-                file_dict = {'file': file_stream}
+                file_dict = {"file": file_stream}
 
                 retry_count = 0
                 while True:
                     if retry_count >= self.DEFAULT_RETRY_LIMIT:
                         raise RuntimeError(
-                            'Error uploading data chunk: {0:d}/{1:d}. Status '
-                            'code: {2:d} - {3!s} {4!s}'.format(
-                                index, chunks, response.status_code,
-                                response.reason, response.text))
+                            "Error uploading data chunk: {0:d}/{1:d}. Status "
+                            "code: {2:d} - {3!s} {4!s}".format(
+                                index,
+                                chunks,
+                                response.status_code,
+                                response.reason,
+                                response.text,
+                            )
+                        )
 
                     response = self._sketch.api.session.post(
-                        self._resource_url, files=file_dict, data=data)
+                        self._resource_url, files=file_dict, data=data
+                    )
 
                     if response.status_code in definitions.HTTP_STATUS_CODE_20X:
                         break
 
                     retry_count += 1
                     logger.warning(
-                        'Error uploading data chunk {0:d}/{1:d}, retry '
-                        'attempt {2:d}/{3:d}'.format(
-                            index, chunks, retry_count,
-                            self.DEFAULT_RETRY_LIMIT))
+                        "Error uploading data chunk {0:d}/{1:d}, retry "
+                        "attempt {2:d}/{3:d}".format(
+                            index, chunks, retry_count, self.DEFAULT_RETRY_LIMIT
+                        )
+                    )
 
         if response.status_code not in definitions.HTTP_STATUS_CODE_20X:
             raise RuntimeError(
-                'Error uploading data: [{0:d}] {1!s} {2!s}, file: {3:s}, '
-                'index {4:s}'.format(
-                    response.status_code, response.reason, response.text,
-                    file_path, self._index))
+                "Error uploading data: [{0:d}] {1!s} {2!s}, file: {3:s}, "
+                "index {4:s}".format(
+                    response.status_code,
+                    response.reason,
+                    response.text,
+                    file_path,
+                    self._index,
+                )
+            )
 
         response_dict = response.json()
-        object_dict = response_dict.get('objects', [{}])[0]
-        meta_dict = response_dict.get('meta', {})
-        self._celery_task_id = meta_dict.get('task_id', '')
+        object_dict = response_dict.get("objects", [{}])[0]
+        meta_dict = response_dict.get("meta", {})
+        self._celery_task_id = meta_dict.get("task_id", "")
 
-        self._timeline_id = object_dict.get('id')
-        self._index = object_dict.get('searchindex', {}).get('index_name')
+        self._timeline_id = object_dict.get("id")
+        self._index = object_dict.get("searchindex", {}).get("index_name")
         self._last_response = response_dict
 
     def add_data_frame(self, data_frame, part_of_iter=False):
         """Add a data frame into the buffer.
 
         Args:
               data_frame: a pandas data frame object to add to the buffer.
@@ -451,83 +486,87 @@
         Raises:
               ValueError: if the data frame does not contain the correct
                   columns for Timesketch upload.
         """
         self._ready()
 
         if not isinstance(data_frame, pandas.DataFrame):
-            raise TypeError('Entry object needs to be a DataFrame')
+            raise TypeError("Entry object needs to be a DataFrame")
 
         size = data_frame.shape[0]
 
         if self._config_helper:
-            data_type = ''
-            if 'data_type' in data_frame:
+            data_type = ""
+            if "data_type" in data_frame:
                 data_types = data_frame.data_type.unique()
                 if len(data_types) == 1:
                     data_type = data_types[0]
 
             df_columns = list(data_frame.columns)
             self._config_helper.configure_streamer(
-                self, data_type=data_type, columns=df_columns)
+                self, data_type=data_type, columns=df_columns
+            )
 
         data_frame_use = self._fix_data_frame(data_frame)
 
-        if 'datetime' not in data_frame_use:
+        if "datetime" not in data_frame_use:
             raise ValueError(
-                'Need a field called datetime in the data frame that is '
-                'formatted according using this format string: '
-                '%Y-%m-%dT%H:%M:%S%z. If that is not provided the data frame '
+                "Need a field called datetime in the data frame that is "
+                "formatted according using this format string: "
+                "%Y-%m-%dT%H:%M:%S%z. If that is not provided the data frame "
                 'needs to have a column that has the word "time" in it, '
-                'that can be used to convert to a datetime field.')
+                "that can be used to convert to a datetime field."
+            )
 
-        if 'message' not in data_frame_use:
+        if "message" not in data_frame_use:
             raise ValueError(
-                'Need a field called message in the data frame, use the '
-                'formatting string to generate one automatically.')
+                "Need a field called message in the data frame, use the "
+                "formatting string to generate one automatically."
+            )
 
-        if 'timestamp_desc' not in data_frame_use:
-            raise ValueError(
-                'Need a field called timestamp_desc in the data frame.')
+        if "timestamp_desc" not in data_frame_use:
+            raise ValueError("Need a field called timestamp_desc in the data frame.")
 
         if size <= self._threshold_entry:
             end_stream = not part_of_iter
             self._upload_data_frame(data_frame_use, end_stream=end_stream)
             return
 
         chunks = int(math.ceil(float(size) / self._threshold_entry))
         for index in range(0, chunks):
             chunk_start = index * self._threshold_entry
             data_chunk = data_frame_use[
-                chunk_start:chunk_start + self._threshold_entry]
+                chunk_start : chunk_start + self._threshold_entry
+            ]
             end_stream = bool(index == chunks - 1)
             self._upload_data_frame(data_chunk, end_stream=end_stream)
 
     def add_dict(self, entry):
         """Add an entry into the buffer.
 
         Args:
             entry: a dict object to add to the buffer.
 
         Raises:
             TypeError: if the entry is not a dict.
         """
         self._ready()
         if not isinstance(entry, dict):
-            raise TypeError('Entry object needs to be a dict.')
+            raise TypeError("Entry object needs to be a dict.")
 
         if self._count >= self._threshold_entry:
             self.flush(end_stream=False)
             self._reset()
 
         if self._config_helper and not self._dict_config_loaded:
-            data_type = entry.get('data_type', '')
+            data_type = entry.get("data_type", "")
             columns = entry.keys()
             self._config_helper.configure_streamer(
-                self, data_type=data_type, columns=columns)
+                self, data_type=data_type, columns=columns
+            )
             self._dict_config_loaded = True
 
         # Changing the dictionary to add fields, such as timestamp description,
         # message field, etc. See function docstring for further details.
         self._fix_dict(entry)
         self._data_lines.append(entry)
         self._count += 1
@@ -562,79 +601,79 @@
                     ``usecols``, index_col is based on the subset.
 
         Raises:
             TypeError: if the entry is not an Excel sheet.
         """
         self._ready()
         if not os.path.isfile(filepath):
-            raise TypeError('File path is not a real file.')
+            raise TypeError("File path is not a real file.")
 
-        file_ending = filepath.lower().split('.')[-1]
-        if file_ending not in ['xls', 'xlsx']:
-            raise TypeError('File name needs to end with xls or xlsx')
+        file_ending = filepath.lower().split(".")[-1]
+        if file_ending not in ["xls", "xlsx"]:
+            raise TypeError("File name needs to end with xls or xlsx")
 
         data_frame = pandas.read_excel(filepath, **kwargs)
         if data_frame.empty:
-            raise TypeError('Not able to read any rows from sheet.')
+            raise TypeError("Not able to read any rows from sheet.")
 
         self.add_data_frame(data_frame)
 
-    def add_file(self, filepath, delimiter=','):
+    def add_file(self, filepath, delimiter=","):
         """Add a CSV, JSONL or a PLASO file to the buffer.
 
         Args:
             filepath: the path to the file to add.
             delimiter: if this is a CSV file then a delimiter can be defined.
 
         Raises:
             TypeError: if the entry does not fulfill requirements.
         """
         self._ready()
 
         if not os.path.isfile(filepath):
-            raise TypeError('Entry object needs to be a file that exists.')
+            raise TypeError("Entry object needs to be a file that exists.")
 
         if not self._timeline_name:
             base_path = os.path.basename(filepath)
-            default_timeline_name, _, _ = base_path.rpartition('.')
+            default_timeline_name, _, _ = base_path.rpartition(".")
             self.set_timeline_name(default_timeline_name)
 
-        file_ending = filepath.lower().split('.')[-1]
+        file_ending = filepath.lower().split(".")[-1]
 
         if not self._data_label:
             self._data_label = file_ending
 
-        if file_ending == 'csv':
+        if file_ending == "csv":
             if self._csv_delimiter:
                 delimiter = self._csv_delimiter
 
             with codecs.open(
-                    filepath, 'r', encoding=self._text_encoding,
-                    errors='replace') as fh:
+                filepath, "r", encoding=self._text_encoding, errors="replace"
+            ) as fh:
                 for chunk_frame in pandas.read_csv(
-                        fh, delimiter=delimiter,
-                        chunksize=self._threshold_entry):
+                    fh, delimiter=delimiter, chunksize=self._threshold_entry
+                ):
                     self.add_data_frame(chunk_frame, part_of_iter=True)
-        elif file_ending == 'plaso':
+        elif file_ending == "plaso":
             self._upload_binary_file(filepath)
 
-        elif file_ending == 'jsonl':
+        elif file_ending == "jsonl":
             with codecs.open(
-                    filepath, 'r', encoding=self._text_encoding,
-                    errors='replace') as fh:
+                filepath, "r", encoding=self._text_encoding, errors="replace"
+            ) as fh:
                 for line in fh:
                     try:
                         self.add_json(line.strip())
                     except TypeError as e:
-                        logger.error('Unable to decode line: {0!s}'.format(e))
+                        logger.error("Unable to decode line: {0!s}".format(e))
 
         else:
             raise TypeError(
-                'File needs to have a file extension of: .csv, .jsonl, mans or '
-                '.plaso')
+                "File needs to have a file extension of: .csv, .jsonl or " ".plaso"
+            )
 
     def add_json(self, json_entry, column_names=None):
         """Add an entry that is in a JSON format.
 
         Args:
             json_entry: a single entry encoded in JSON.
             column_names: a list of column names if the JSON object
@@ -642,33 +681,37 @@
 
         Raises:
             TypeError: if the entry is not JSON or in the wrong JSON format.
         """
         try:
             json_obj = json.loads(json_entry)
         except json.JSONDecodeError as e:
-            raise TypeError('Data not as JSON, error: {0!s}'.format(e)) from e
+            raise TypeError("Data not as JSON, error: {0!s}".format(e)) from e
 
         json_dict = {}
         if isinstance(json_obj, (list, tuple)):
             if not column_names:
                 raise TypeError(
-                    'Data is a list, but there are no defined column names.')
+                    "Data is a list, but there are no defined column names."
+                )
             if not len(json_obj) != len(column_names):
                 raise TypeError(
-                    'The number of columns ({0:d}) does not match the number '
-                    'of columns in the JSON list ({1:d})'.format(
-                        len(column_names), len(json_obj)))
+                    "The number of columns ({0:d}) does not match the number "
+                    "of columns in the JSON list ({1:d})".format(
+                        len(column_names), len(json_obj)
+                    )
+                )
             json_dict = dict(zip(column_names, json_obj))
         elif isinstance(json_obj, dict):
             json_dict = json_obj
         else:
             raise TypeError(
-                'The JSON object needs to be either a dict or a list with '
-                'defined column names.')
+                "The JSON object needs to be either a dict or a list with "
+                "defined column names."
+            )
 
         self.add_dict(json_dict)
 
     @property
     def celery_task_id(self):
         """Return the celery task identification for the upload."""
         return self._celery_task_id
@@ -680,19 +723,18 @@
         except ValueError:
             return
 
         if self._data_lines:
             self.flush(end_stream=True)
 
         # Trigger auto analyzer pipeline to kick in.
-        pipe_resource = '{0:s}/sketches/{1:d}/analyzer/'.format(
-            self._sketch.api.api_root, self._sketch.id)
-        data = {
-            'index_name': self._index
-        }
+        pipe_resource = "{0:s}/sketches/{1:d}/analyzer/".format(
+            self._sketch.api.api_root, self._sketch.id
+        )
+        data = {"index_name": self._index}
         _ = self._sketch.api.session.post(pipe_resource, json=data)
 
     def flush(self, end_stream=True):
         """Flushes the buffer and uploads to timesketch.
 
         Args:
             end_stream: boolean that determines whether this is the final
@@ -765,15 +807,15 @@
         """Set a client for the streamer.
 
         Args:
             sketch: an instance of Sketch that is used to communicate
                 with the API to upload data.
         """
         self._sketch = sketch
-        self._resource_url = '{0:s}/upload/'.format(sketch.api.api_root)
+        self._resource_url = "{0:s}/upload/".format(sketch.api.api_root)
 
     def set_text_encoding(self, encoding):
         """Set the default encoding for reading text files."""
         self._text_encoding = encoding
 
     def set_timeline_name(self, name):
         """Set the timeline name."""
@@ -783,40 +825,40 @@
         """Set the timestamp description field."""
         self._timestamp_desc = description
 
     @property
     def state(self):
         """Returns a state string for the indexing process."""
         if not self._celery_task_id:
-            return 'Unknown'
+            return "Unknown"
 
-        tasks = self._sketch.api.check_celery_status(
-            job_id=self._celery_task_id)
+        tasks = self._sketch.api.check_celery_status(job_id=self._celery_task_id)
 
         if len(tasks) > 1:
             for task in tasks:
-                if task.get('task_id', '') ==  self._celery_task_id:
-                    return task.get('state', 'Unknown')
+                if task.get("task_id", "") == self._celery_task_id:
+                    return task.get("state", "Unknown")
 
         task = tasks[0]
-        return task.get('state', 'Unknown')
+        return task.get("state", "Unknown")
 
     @property
     def timeline(self):
         """Returns a timeline object."""
         if not self._timeline_id:
-            logger.warning('No timeline ID has been stored as of yet.')
+            logger.warning("No timeline ID has been stored as of yet.")
             return None
 
         timeline_obj = timeline.Timeline(
             timeline_id=self._timeline_id,
             sketch_id=self._sketch.id,
             api=self._sketch.api,
             name=self._timeline_name,
-            searchindex=self._index)
+            searchindex=self._index,
+        )
         return timeline_obj
 
     def __enter__(self):
         """Make it possible to use "with" statement."""
         self._reset()
         return self
```

### Comparing `timesketch-import-client-20210602/timesketch_import_client/importer_test.py` & `timesketch-import-client-20230721/timesketch_import_client/importer_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,172 +24,186 @@
 
 
 class MockSketch(object):
     """Mock sketch object."""
 
     def __init__(self):
         self.api = mock.Mock()
-        self.api.api_root = 'foo_root'
+        self.api.api_root = "foo_root"
         self.id = 1
 
 
 class MockStreamer(importer.ImportStreamer):
     """Mock the import streamer."""
 
     def __init__(self):
-        super(MockStreamer, self).__init__()
+        super().__init__()
         self.lines = []
 
     @property
     def columns(self):
         columns = set()
         for line in self.lines:
             columns.update(line.keys())
         return list(columns)
 
-    def _upload_data_buffer(self, end_stream):
+    def _upload_data_buffer(self, end_stream, retry_count=0):
         self.lines.extend(self._data_lines)
 
-    def _upload_data_frame(self, data_frame, end_stream):
-        self.lines.extend(
-            json.loads(data_frame.to_json(orient='records')))
+    def _upload_data_frame(self, data_frame, end_stream, retry_count=0):
+        self.lines.extend(json.loads(data_frame.to_json(orient="records")))
 
     def close(self):
         pass
 
 
 class TimesketchImporterTest(unittest.TestCase):
     """Test Timesketch importer."""
 
     def setUp(self):
         """Set up the test data frame."""
         self.lines = []
 
         dict_one = {
-            'timestamp': '2019-02-23T12:51:52',
-            'stuff': 'from bar to foobar',
-            'correct': False,
-            'random_number': 13245,
-            'vital_stats': 'gangverk'
+            "timestamp": "2019-02-23T12:51:52",
+            "stuff": "from bar to foobar",
+            "correct": False,
+            "random_number": 13245,
+            "vital_stats": "gangverk",
         }
         self.lines.append(dict_one)
 
         dict_two = {
-            'timestamp': '2019-06-17T20:11:23',
-            'stuff': 'fra sjalfstaedi til sjalfstaedis',
-            'correct': True,
-            'random_number': 52,
-            'vital_stats': 'stolt'
+            "timestamp": "2019-06-17T20:11:23",
+            "stuff": "fra sjalfstaedi til sjalfstaedis",
+            "correct": True,
+            "random_number": 52,
+            "vital_stats": "stolt",
         }
         self.lines.append(dict_two)
 
         dict_three = {
-            'timestamp': '2019-01-03T02:39:42',
-            'stuff': 'stordagur',
-            'correct': True,
-            'random_number': 59913,
-            'vital_stats': 'elli'
+            "timestamp": "2019-01-03T02:39:42",
+            "stuff": "stordagur",
+            "correct": True,
+            "random_number": 59913,
+            "vital_stats": "elli",
         }
         self.lines.append(dict_three)
 
         dict_four = {
-            'timestamp': '2019-12-23T23:00:03',
-            'stuff': 'sidasti sens ad kaupa gjof',
-            'correct': True,
-            'random_number': 5231134324,
-            'vital_stats': 'stress'
+            "timestamp": "2019-12-23T23:00:03",
+            "stuff": "sidasti sens ad kaupa gjof",
+            "correct": True,
+            "random_number": 5231134324,
+            "vital_stats": "stress",
         }
         self.lines.append(dict_four)
 
         dict_five = {
-            'timestamp': '2019-10-31T17:12:44',
-            'stuff': 'hraeda hraedur',
-            'correct': True,
-            'random_number': 420,
-            'vital_stats': 'grasker'
+            "timestamp": "2019-10-31T17:12:44",
+            "stuff": "hraeda hraedur",
+            "correct": True,
+            "random_number": 420,
+            "vital_stats": "grasker",
         }
         self.lines.append(dict_five)
 
         self.frame = pandas.DataFrame(self.lines)
 
     def test_adding_data_frames(self):
         """Test adding a data frame to the importer."""
         with MockStreamer() as streamer:
             streamer.set_sketch(MockSketch())
-            streamer.set_timestamp_description('Log Entries')
-            streamer.set_timeline_name('Test Entries')
+            streamer.set_timestamp_description("Log Entries")
+            streamer.set_timeline_name("Test Entries")
             streamer.set_message_format_string(
-                '{stuff:s} -> {correct!s} [{random_number:d}]')
+                "{stuff:s} -> {correct!s} [{random_number:d}]"
+            )
 
             streamer.add_data_frame(self.frame)
             self._run_all_tests(streamer.columns, streamer.lines)
             self.assertEqual(len(streamer.lines), 5)
 
         # Test by splitting up the dataset into chunks.
         lines = None
         columns = None
         with MockStreamer() as streamer:
             streamer.set_sketch(MockSketch())
-            streamer.set_timestamp_description('Log Entries')
-            streamer.set_timeline_name('Test Entries')
+            streamer.set_timestamp_description("Log Entries")
+            streamer.set_timeline_name("Test Entries")
             streamer.set_entry_threshold(2)
             streamer.set_message_format_string(
-                '{stuff:s} -> {correct!s} [{random_number:d}]')
+                "{stuff:s} -> {correct!s} [{random_number:d}]"
+            )
 
             streamer.add_data_frame(self.frame)
             lines = streamer.lines
             columns = streamer.columns
         self._run_all_tests(columns, lines)
         self.assertEqual(len(lines), 5)
 
     def test_adding_dict(self):
         """Test adding a dict to the importer."""
         with MockStreamer() as streamer:
             streamer.set_sketch(MockSketch())
-            streamer.set_timestamp_description('Log Entries')
-            streamer.set_timeline_name('Test Entries')
+            streamer.set_timestamp_description("Log Entries")
+            streamer.set_timeline_name("Test Entries")
             streamer.set_message_format_string(
-                '{stuff:s} -> {correct!s} [{random_number:d}]')
+                "{stuff:s} -> {correct!s} [{random_number:d}]"
+            )
 
             for entry in self.lines:
                 streamer.add_dict(entry)
 
             streamer.flush()
             self._run_all_tests(streamer.columns, streamer.lines)
 
     def test_adding_json(self):
         """Test adding a JSON to the importer."""
         with MockStreamer() as streamer:
             streamer.set_sketch(MockSketch())
-            streamer.set_timestamp_description('Log Entries')
-            streamer.set_timeline_name('Test Entries')
+            streamer.set_timestamp_description("Log Entries")
+            streamer.set_timeline_name("Test Entries")
             streamer.set_message_format_string(
-                '{stuff:s} -> {correct!s} [{random_number:d}]')
+                "{stuff:s} -> {correct!s} [{random_number:d}]"
+            )
 
             for entry in self.lines:
                 json_string = json.dumps(entry)
                 streamer.add_json(json_string)
 
             streamer.flush()
             self._run_all_tests(streamer.columns, streamer.lines)
 
     def _run_all_tests(self, columns, lines):
         """Run all tests on the result set of a streamer."""
         # The first line is the column line.
         self.assertEqual(len(lines), 5)
 
         column_set = set(columns)
-        correct_set = set([
-            'message', 'timestamp_desc', 'datetime', 'timestamp',
-            'vital_stats', 'random_number', 'correct', 'stuff'])
+        correct_set = set(
+            [
+                "message",
+                "timestamp_desc",
+                "datetime",
+                "timestamp",
+                "vital_stats",
+                "random_number",
+                "correct",
+                "stuff",
+            ]
+        )
 
         self.assertSetEqual(column_set, correct_set)
 
-        messages = [x.get('message', 'N/A') for x in lines]
-        message_correct = set([
-            'fra sjalfstaedi til sjalfstaedis -> True [52]',
-            'from bar to foobar -> False [13245]',
-            'sidasti sens ad kaupa gjof -> True [5231134324]',
-            'stordagur -> True [59913]',
-            'hraeda hraedur -> True [420]',
-        ])
+        messages = [x.get("message", "N/A") for x in lines]
+        message_correct = set(
+            [
+                "fra sjalfstaedi til sjalfstaedis -> True [52]",
+                "from bar to foobar -> False [13245]",
+                "sidasti sens ad kaupa gjof -> True [5231134324]",
+                "stordagur -> True [59913]",
+                "hraeda hraedur -> True [420]",
+            ]
+        )
         self.assertSetEqual(set(messages), message_correct)
```

### Comparing `timesketch-import-client-20210602/timesketch_import_client/utils.py` & `timesketch-import-client-20230721/timesketch_import_client/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,42 +20,51 @@
 import dateutil.parser
 
 
 # When there is no defined format message string a default one is used
 # that is generated using the available columns or keys in the dataset.
 # This constant defines what columns or keys should be skipped while
 # generating this message field.
-FIELDS_TO_SKIP_IN_FORMAT_STRING = frozenset([
-    'timestamp_desc', 'time', 'timestamp', 'data_type', 'datetime',
-    'source_short', 'source_long', 'source'
-])
+FIELDS_TO_SKIP_IN_FORMAT_STRING = frozenset(
+    [
+        "timestamp_desc",
+        "time",
+        "timestamp",
+        "data_type",
+        "datetime",
+        "source_short",
+        "source_long",
+        "source",
+    ]
+)
 # This constant defines patterns that are used to skip columns or keys
 # that start with the strings defined here.
-FIELDS_TO_SKIP_STARTSWITH = frozenset([
-    '_',
-])
+FIELDS_TO_SKIP_STARTSWITH = frozenset(
+    [
+        "_",
+    ]
+)
 
 
 def format_data_frame(dataframe, format_message_string):
     """Add a message field to a data frame using a format message string.
 
     Args:
         dataframe (pandas.DataFrame): the data frame containing the data.
         format_message_String (str): the format string used to generate
             a message column.
     """
-    dataframe['message'] = ''
+    dataframe["message"] = ""
 
     formatter = string.Formatter()
     for literal_text, field, _, _ in formatter.parse(format_message_string):
-        dataframe['message'] = dataframe['message'] + literal_text
+        dataframe["message"] = dataframe["message"] + literal_text
 
         if field:
-            dataframe['message'] = dataframe[
-                'message'] + dataframe[field].astype(str)
+            dataframe["message"] = dataframe["message"] + dataframe[field].astype(str)
 
 
 def get_combined_message_string(dataframe=None, mydict=None):
     """Returns a message string by combining all columns from a DataFrame/dict.
 
     Args:
         dataframe (pandas.DataFrame): the data frame containing the data. Used
@@ -66,35 +75,33 @@
     Raises:
         ValueError if neither dataframe nor a dictionary is supplied.
 
     Returns:
         A string that can be used as a default message string.
     """
     if dataframe is None and mydict is None:
-        raise ValueError('Need to define either a dict or a DataFrame')
+        raise ValueError("Need to define either a dict or a DataFrame")
 
     if mydict:
         my_list = list(mydict.keys())
     else:
         my_list = list(dataframe.columns)
 
-    fields_to_delete = list(set(my_list).intersection(
-        FIELDS_TO_SKIP_IN_FORMAT_STRING))
+    fields_to_delete = list(set(my_list).intersection(FIELDS_TO_SKIP_IN_FORMAT_STRING))
     for field in fields_to_delete:
         index = my_list.index(field)
         _ = my_list.pop(index)
 
     for del_field in FIELDS_TO_SKIP_STARTSWITH:
         for index, field in enumerate(my_list):
             if field.startswith(del_field):
                 _ = my_list.pop(index)
 
-    string_values = [
-        '[{0:s}] = {{{0:s}}}'.format(x) for x in my_list]
-    return ', '.join(string_values)
+    string_values = ["[{0:s}] = {{{0:s}}}".format(x) for x in my_list]
+    return ", ".join(string_values)
 
 
 def get_datestring_from_value(value):
     """Returns an empty string or a date value.
 
     Args:
         value (any): A string or an int/float that contains a timestamp
@@ -113,8 +120,8 @@
 
     if isinstance(value, (int, float)):
         try:
             date = datetime.datetime.utcfromtimestamp(value / 1e6)
             return date.isoformat()
         except ValueError:
             pass
-    return ''
+    return ""
```

### Comparing `timesketch-import-client-20210602/timesketch_import_client/version.py` & `timesketch-import-client-20230721/timesketch_import_client/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,13 +9,13 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Version information for Timesketch Import Client."""
 
-__version__ = '20210602'
+__version__ = "20230721"
 
 
 def get_version():
     """Returns the version information."""
     return __version__
```

### Comparing `timesketch-import-client-20210602/timesketch_import_client.egg-info/SOURCES.txt` & `timesketch-import-client-20230721/timesketch_import_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

