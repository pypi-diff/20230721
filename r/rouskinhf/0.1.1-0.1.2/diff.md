# Comparing `tmp/rouskinhf-0.1.1.tar.gz` & `tmp/rouskinhf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rouskinhf-0.1.1.tar", last modified: Thu Jul 20 04:02:10 2023, max compression
+gzip compressed data, was "rouskinhf-0.1.2.tar", last modified: Fri Jul 21 17:26:44 2023, max compression
```

## Comparing `rouskinhf-0.1.1.tar` & `rouskinhf-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-20 04:02:10.780282 rouskinhf-0.1.1/
--rw-r--r--   0 ymdt       (501) staff       (20)     1141 2023-06-30 22:14:56.000000 rouskinhf-0.1.1/LICENSE
--rw-r--r--   0 ymdt       (501) staff       (20)        3 2023-07-01 06:33:39.000000 rouskinhf-0.1.1/MANIFEST.in
--rw-r--r--   0 ymdt       (501) staff       (20)     5140 2023-07-20 04:02:10.780106 rouskinhf-0.1.1/PKG-INFO
--rw-r--r--   0 ymdt       (501) staff       (20)     4689 2023-07-20 03:54:37.000000 rouskinhf-0.1.1/README.md
--rw-r--r--   0 ymdt       (501) staff       (20)      813 2023-07-20 04:01:38.000000 rouskinhf-0.1.1/pyproject.toml
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-20 04:02:10.778783 rouskinhf-0.1.1/rouskinhf/
--rw-r--r--   0 ymdt       (501) staff       (20)     2433 2023-07-20 01:01:23.000000 rouskinhf-0.1.1/rouskinhf/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)    14888 2023-07-20 00:54:02.000000 rouskinhf-0.1.1/rouskinhf/datafolder.py
--rw-r--r--   0 ymdt       (501) staff       (20)     5620 2023-07-07 18:09:01.000000 rouskinhf-0.1.1/rouskinhf/datapoint.py
--rw-r--r--   0 ymdt       (501) staff       (20)      556 2023-07-20 03:42:13.000000 rouskinhf-0.1.1/rouskinhf/env.py
--rw-r--r--   0 ymdt       (501) staff       (20)     3136 2023-07-01 05:56:29.000000 rouskinhf-0.1.1/rouskinhf/info_file.py
--rw-r--r--   0 ymdt       (501) staff       (20)     9593 2023-07-13 17:48:12.000000 rouskinhf-0.1.1/rouskinhf/list_datapoints.py
--rw-r--r--   0 ymdt       (501) staff       (20)     3672 2023-07-20 00:05:00.000000 rouskinhf-0.1.1/rouskinhf/parsers.py
--rw-r--r--   0 ymdt       (501) staff       (20)     2608 2023-07-20 00:54:02.000000 rouskinhf-0.1.1/rouskinhf/path.py
--rw-r--r--   0 ymdt       (501) staff       (20)     6222 2023-07-20 00:54:02.000000 rouskinhf-0.1.1/rouskinhf/rnastructure.py
--rw-r--r--   0 ymdt       (501) staff       (20)     3493 2023-07-20 00:54:02.000000 rouskinhf-0.1.1/rouskinhf/util.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-20 04:02:10.779723 rouskinhf-0.1.1/rouskinhf.egg-info/
--rw-r--r--   0 ymdt       (501) staff       (20)     5140 2023-07-20 04:02:10.000000 rouskinhf-0.1.1/rouskinhf.egg-info/PKG-INFO
--rw-r--r--   0 ymdt       (501) staff       (20)      438 2023-07-20 04:02:10.000000 rouskinhf-0.1.1/rouskinhf.egg-info/SOURCES.txt
--rw-r--r--   0 ymdt       (501) staff       (20)        1 2023-07-20 04:02:10.000000 rouskinhf-0.1.1/rouskinhf.egg-info/dependency_links.txt
--rw-r--r--   0 ymdt       (501) staff       (20)      136 2023-07-20 04:02:10.000000 rouskinhf-0.1.1/rouskinhf.egg-info/requires.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       10 2023-07-20 04:02:10.000000 rouskinhf-0.1.1/rouskinhf.egg-info/top_level.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       38 2023-07-20 04:02:10.780332 rouskinhf-0.1.1/setup.cfg
--rw-r--r--   0 ymdt       (501) staff       (20)      429 2023-07-20 04:01:49.000000 rouskinhf-0.1.1/setup.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-21 17:26:44.035824 rouskinhf-0.1.2/
+-rw-r--r--   0 ymdt       (501) staff       (20)     1141 2023-06-30 22:14:56.000000 rouskinhf-0.1.2/LICENSE
+-rw-r--r--   0 ymdt       (501) staff       (20)        3 2023-07-01 06:33:39.000000 rouskinhf-0.1.2/MANIFEST.in
+-rw-r--r--   0 ymdt       (501) staff       (20)     5839 2023-07-21 17:26:44.035668 rouskinhf-0.1.2/PKG-INFO
+-rw-r--r--   0 ymdt       (501) staff       (20)     5388 2023-07-21 17:26:25.000000 rouskinhf-0.1.2/README.md
+-rw-r--r--   0 ymdt       (501) staff       (20)      813 2023-07-21 17:26:41.000000 rouskinhf-0.1.2/pyproject.toml
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-21 17:26:44.034415 rouskinhf-0.1.2/rouskinhf/
+-rw-r--r--   0 ymdt       (501) staff       (20)     2433 2023-07-20 01:01:23.000000 rouskinhf-0.1.2/rouskinhf/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    15276 2023-07-21 17:26:25.000000 rouskinhf-0.1.2/rouskinhf/datafolder.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     5620 2023-07-07 18:09:01.000000 rouskinhf-0.1.2/rouskinhf/datapoint.py
+-rw-r--r--   0 ymdt       (501) staff       (20)      556 2023-07-20 03:42:13.000000 rouskinhf-0.1.2/rouskinhf/env.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     3136 2023-07-01 05:56:29.000000 rouskinhf-0.1.2/rouskinhf/info_file.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    10753 2023-07-21 17:26:25.000000 rouskinhf-0.1.2/rouskinhf/list_datapoints.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     3672 2023-07-20 00:05:00.000000 rouskinhf-0.1.2/rouskinhf/parsers.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     2608 2023-07-20 00:54:02.000000 rouskinhf-0.1.2/rouskinhf/path.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     6222 2023-07-20 00:54:02.000000 rouskinhf-0.1.2/rouskinhf/rnastructure.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     3493 2023-07-20 00:54:02.000000 rouskinhf-0.1.2/rouskinhf/util.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-21 17:26:44.035417 rouskinhf-0.1.2/rouskinhf.egg-info/
+-rw-r--r--   0 ymdt       (501) staff       (20)     5839 2023-07-21 17:26:44.000000 rouskinhf-0.1.2/rouskinhf.egg-info/PKG-INFO
+-rw-r--r--   0 ymdt       (501) staff       (20)      438 2023-07-21 17:26:44.000000 rouskinhf-0.1.2/rouskinhf.egg-info/SOURCES.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)        1 2023-07-21 17:26:44.000000 rouskinhf-0.1.2/rouskinhf.egg-info/dependency_links.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)      136 2023-07-21 17:26:44.000000 rouskinhf-0.1.2/rouskinhf.egg-info/requires.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       10 2023-07-21 17:26:44.000000 rouskinhf-0.1.2/rouskinhf.egg-info/top_level.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       38 2023-07-21 17:26:44.035879 rouskinhf-0.1.2/setup.cfg
+-rw-r--r--   0 ymdt       (501) staff       (20)      430 2023-07-20 04:08:01.000000 rouskinhf-0.1.2/setup.py
```

### Comparing `rouskinhf-0.1.1/LICENSE` & `rouskinhf-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.1/PKG-INFO` & `rouskinhf-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,18 @@
-Metadata-Version: 2.1
-Name: rouskinhf
-Version: 0.1.1
-Summary: A library to manipulate data for our DMS prediction models.
-Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
 
 
+# Download your RNA data from HuggingFace with rouskinhf!
 
-# Download your RNA data from huggingface with rouskinhf!
-
-A repo to manipulate the data for our RNA structure prediction model. The data is stored on HuggingFace and pulled locally for training models.
+A repo to manipulate the data for our RNA structure prediction model. This repo allows you to:
+- pull datasets from the Rouskinlab's HuggingFace
+- create datasets from local files and push them to HuggingFace, from the formats:
+    - `.fasta`
+    - `.ct`
+    - `.json` (DREEM output format)
+    - `.json` (Rouskinlab's huggingface format)
 
 ## Installation
 
 ### Get a HuggingFace token
 
 Go to [HuggingFace](https://huggingface.co/) and create an account. Then go to your profile and copy your token ([huggingface.co/settings/tokens](https://huggingface.co/settings/tokens)).
 
@@ -68,14 +61,31 @@
 
 ### Create a datafolder from local files and push it to HuggingFace
 
 See the [tutorial](https://github.com/rouskinlab/rouskinhf/blob/main/tutorials/create_push_pull.ipynb).
 
 ## About
 
+### Sourcing the environment and keeping your environment variable secret
+
+The variables defined in the `env` file are required by `rouskinhf`. Make that before you use `rouskinhf`, you run in a terminal:
+
+```bash
+source env
+``` 
+ or, in a Jupyter notebook:
+
+```python
+!pip install python-dotenv
+%load_ext dotenv
+%dotenv env
+```
+ 
+ The point of using environment variables is to ensure the privacy of your huggingface token. Make sure to add your `env` file to your `.gitignore`, so your HuggingFace token doesn't get pushed to any public repository.
+
 ### Import data with ``import_dataset``
 
 This repo provides a function ``import_dataset``, which allows your to pull a dataset from HuggingFace and store it locally. If the data is already stored locally, it will be loaded from the local folder. The type of data available is the DMS signal and the structure, under the shape of paired bases tuples. The function has the following signature:
 
 ```python
 def import_dataset(name:str, data:str, force_download:bool=False)->np.ndarray:
 
@@ -96,22 +106,22 @@
 
     ndarray
         The dataset with the given name for the given type of data.
 
     Example
     -------
 
-    >>> import_dataset(name='for_testing', data='structure', hf_token=os.environ['os.environ['HUGGINGFACE_TOKEN'],']).shape
-    (2,)
-    >>> import_dataset(name='for_testing', data='DMS', hf_token=os.environ['os.environ['HUGGINGFACE_TOKEN'],']).shape
-    (2,)
-    >>> import_dataset(name='for_testing', data='structure', hf_token=os.environ['os.environ['HUGGINGFACE_TOKEN'],'], force_download=True).shape
-    (2,)
-    >>> import_dataset(name='for_testing', data='DMS', hf_token=os.environ['os.environ['HUGGINGFACE_TOKEN'],'], force_download=True).shape
-    (2,)
+    >>> import_dataset(name='for_testing', data='structure').keys()
+    dict_keys(['references', 'sequences', 'structure'])
+    >>> import_dataset(name='for_testing', data='DMS').keys()
+    dict_keys(['references', 'sequences', 'DMS'])
+    >>> import_dataset(name='for_testing', data='structure', force_download=True).keys()
+    dict_keys(['references', 'sequences', 'structure'])
+    >>> import_dataset(name='for_testing', data='DMS', force_download=True).keys()
+    dict_keys(['references', 'sequences', 'DMS'])
 ```
 
 ### FYI, the datafolder object
 
 The datafolder object is a wrapper around your local folder and HuggingFace API, to keep a consistent datastructure across your datasets. It contains multiple methods to create datasets from various input formats, store the data and metadata in a systematic way, and push / pull from HuggingFace.
 
 On HuggingFace, the datafolder stores the data under the following structure:
```

### Comparing `rouskinhf-0.1.1/README.md` & `rouskinhf-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,31 @@
+Metadata-Version: 2.1
+Name: rouskinhf
+Version: 0.1.2
+Summary: A library to manipulate data for our DMS prediction models.
+Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
-# Download your RNA data from huggingface with rouskinhf!
 
-A repo to manipulate the data for our RNA structure prediction model. The data is stored on HuggingFace and pulled locally for training models.
+# Download your RNA data from HuggingFace with rouskinhf!
+
+A repo to manipulate the data for our RNA structure prediction model. This repo allows you to:
+- pull datasets from the Rouskinlab's HuggingFace
+- create datasets from local files and push them to HuggingFace, from the formats:
+    - `.fasta`
+    - `.ct`
+    - `.json` (DREEM output format)
+    - `.json` (Rouskinlab's huggingface format)
 
 ## Installation
 
 ### Get a HuggingFace token
 
 Go to [HuggingFace](https://huggingface.co/) and create an account. Then go to your profile and copy your token ([huggingface.co/settings/tokens](https://huggingface.co/settings/tokens)).
 
@@ -55,14 +74,31 @@
 
 ### Create a datafolder from local files and push it to HuggingFace
 
 See the [tutorial](https://github.com/rouskinlab/rouskinhf/blob/main/tutorials/create_push_pull.ipynb).
 
 ## About
 
+### Sourcing the environment and keeping your environment variable secret
+
+The variables defined in the `env` file are required by `rouskinhf`. Make that before you use `rouskinhf`, you run in a terminal:
+
+```bash
+source env
+``` 
+ or, in a Jupyter notebook:
+
+```python
+!pip install python-dotenv
+%load_ext dotenv
+%dotenv env
+```
+ 
+ The point of using environment variables is to ensure the privacy of your huggingface token. Make sure to add your `env` file to your `.gitignore`, so your HuggingFace token doesn't get pushed to any public repository.
+
 ### Import data with ``import_dataset``
 
 This repo provides a function ``import_dataset``, which allows your to pull a dataset from HuggingFace and store it locally. If the data is already stored locally, it will be loaded from the local folder. The type of data available is the DMS signal and the structure, under the shape of paired bases tuples. The function has the following signature:
 
 ```python
 def import_dataset(name:str, data:str, force_download:bool=False)->np.ndarray:
 
@@ -83,22 +119,22 @@
 
     ndarray
         The dataset with the given name for the given type of data.
 
     Example
     -------
 
-    >>> import_dataset(name='for_testing', data='structure', hf_token=os.environ['os.environ['HUGGINGFACE_TOKEN'],']).shape
-    (2,)
-    >>> import_dataset(name='for_testing', data='DMS', hf_token=os.environ['os.environ['HUGGINGFACE_TOKEN'],']).shape
-    (2,)
-    >>> import_dataset(name='for_testing', data='structure', hf_token=os.environ['os.environ['HUGGINGFACE_TOKEN'],'], force_download=True).shape
-    (2,)
-    >>> import_dataset(name='for_testing', data='DMS', hf_token=os.environ['os.environ['HUGGINGFACE_TOKEN'],'], force_download=True).shape
-    (2,)
+    >>> import_dataset(name='for_testing', data='structure').keys()
+    dict_keys(['references', 'sequences', 'structure'])
+    >>> import_dataset(name='for_testing', data='DMS').keys()
+    dict_keys(['references', 'sequences', 'DMS'])
+    >>> import_dataset(name='for_testing', data='structure', force_download=True).keys()
+    dict_keys(['references', 'sequences', 'structure'])
+    >>> import_dataset(name='for_testing', data='DMS', force_download=True).keys()
+    dict_keys(['references', 'sequences', 'DMS'])
 ```
 
 ### FYI, the datafolder object
 
 The datafolder object is a wrapper around your local folder and HuggingFace API, to keep a consistent datastructure across your datasets. It contains multiple methods to create datasets from various input formats, store the data and metadata in a systematic way, and push / pull from HuggingFace.
 
 On HuggingFace, the datafolder stores the data under the following structure:
```

### Comparing `rouskinhf-0.1.1/pyproject.toml` & `rouskinhf-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = ['rouskinhf']
 
 [project]
 name =  "rouskinhf"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     {name = "Yves Martin", email = "yves@martin.yt"},
     {name = "Alberic de Lajarte", email = "albericlajarte@gmail.com"},
 ]
 description = "A library to manipulate data for our DMS prediction models."
 readme = "README.md"
 classifiers = [
```

### Comparing `rouskinhf-0.1.1/rouskinhf/__init__.py` & `rouskinhf-0.1.2/rouskinhf/__init__.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.1/rouskinhf/datafolder.py` & `rouskinhf-0.1.2/rouskinhf/datafolder.py`

 * *Files 3% similar despite different names*

```diff
@@ -162,16 +162,15 @@
 
 
 
 
     def dump_datapoints(self, generate_npy):
         """Dump the datapoints to a json file."""
 
-        if not os.path.exists(self.get_json()):
-            self.datapoints.to_json(self.get_json())
+        self.datapoints.to_json(self.get_json())
 
         if generate_npy:
             self.generate_npy()
 
 
 
 class CreateDatafolderFromDreemOutput(CreateDatafolderTemplate):
@@ -189,31 +188,34 @@
 
     predict_structure : bool, optional
         If True, the structure of the RNA is predicted. Default is True.
 
     generate_npy : bool, optional
         If True, the npy files are generated. Default is True.
 
+    tqdm : bool, optional
+        If True, a progress bar is displayed. Default is True.
+
 
     Examples
     --------
 
     >>> datafolder = DataFolder.from_dreem_output(path_in='data/input_files_for_testing/dreem_output.json', generate_npy=True)
     >>> datafolder.name
     'dreem_output'
     >>> print(str(datafolder).split(' ')[0])
     CreateDatafolderFromDreemOutput
     >>> os.path.isfile(datafolder.get_json())
     True
     """
 
-    def __init__(self, path_in, path_out, name, predict_structure, generate_npy) -> None:
+    def __init__(self, path_in, path_out, name, predict_structure, generate_npy, tqdm=True) -> None:
         super().__init__(path_in, path_out, name, source = 'dreem_output', predict_structure = predict_structure, predict_dms = False)
 
-        self.datapoints = ListofDatapoints.from_dreem_output(path_in, predict_structure = predict_structure)
+        self.datapoints = ListofDatapoints.from_dreem_output(path_in, predict_structure = predict_structure, tqdm=tqdm)
         self.dump_datapoints(generate_npy)
 
 
 class CreateDatafolderFromFasta(CreateDatafolderTemplate):
 
     """ Create a datafolder from a fasta file.
 
@@ -244,18 +246,18 @@
     'sequences'
     >>> print(str(datafolder).split(' ')[0])
     CreateDatafolderFromFasta
     >>> os.path.isfile(datafolder.get_json())
     True
     """
 
-    def __init__(self, path_in, path_out, name, predict_structure, predict_dms, generate_npy) -> None:
+    def __init__(self, path_in, path_out, name, predict_structure, predict_dms, generate_npy, tqdm) -> None:
         super().__init__(path_in, path_out, name, source = 'fasta', predict_structure = predict_structure, predict_dms = predict_dms)
 
-        self.datapoints = ListofDatapoints.from_fasta(path_in, predict_structure = predict_structure, predict_dms = predict_dms)
+        self.datapoints = ListofDatapoints.from_fasta(path_in, predict_structure = predict_structure, predict_dms = predict_dms, tqdm=tqdm)
         self.dump_datapoints(generate_npy)
 
 
 
 class CreateDatafolderFromCTfolder(CreateDatafolderTemplate):
 
     """ Create a datafolder from a folder of ct files.
@@ -271,32 +273,35 @@
 
     predict_dms : bool, optional
         If True, the dms of the RNA is predicted. Default is True.
 
     generate_npy : bool, optional
         If True, the npy files are generated. Default is True.
 
+    tqdm : bool, optional
+        If True, a progress bar is displayed. Default is True.
+
 
     Examples
     --------
 
     >>> datafolder = DataFolder.from_ct_folder(path_in='data/input_files_for_testing/ct_files', generate_npy=True)
     >>> datafolder.name
     'ct_files'
     >>> print(str(datafolder).split(' ')[0])
     CreateDatafolderFromCTfolder
     >>> os.path.isfile(datafolder.get_json())
     True
     """
 
-    def __init__(self, path_in, path_out, name, predict_dms, generate_npy) -> None:
+    def __init__(self, path_in, path_out, name, predict_dms, generate_npy, tqdm=True) -> None:
         super().__init__(path_in, path_out, name, source = 'ct', predict_structure = False, predict_dms = predict_dms)
 
         ct_files = [os.path.join(path_in, f) for f in os.listdir(path_in) if f.endswith('.ct') or f.endswith('.txt')]
-        self.datapoints = ListofDatapoints.from_ct(ct_files, predict_dms = predict_dms)
+        self.datapoints = ListofDatapoints.from_ct(ct_files, predict_dms = predict_dms, tqdm=tqdm)
         self.datapoints.filter_duplicates()
         self.dump_datapoints(generate_npy)
 
 
 class LoadDatafolder(DataFolderTemplate):
 
     def __init__(self, name, root) -> None:
@@ -323,15 +328,15 @@
     --------
 
     >>> datafolder = LoadDatafolderFromHF(name='for_testing', path_out='data/datafolders')
     >>> datafolder.name
     'for_testing'
     """
 
-    def __init__(self, name, path_out, revision='main') -> None:
+    def __init__(self, name, path_out, revision='main', tqdm=True) -> None:
         super().__init__(name, path_out)
 
         # Download the datafolder #TODO : check if the datafolder is already downloaded
         snapshot_download(
             repo_id = ROUSKINLAB+self.name,
             repo_type='dataset',
             local_dir=self.get_main_folder(),
@@ -339,15 +344,15 @@
             token=HUGGINGFACE_TOKEN,
             allow_patterns=['info.json', 'data.json']
             )
 
         assert os.path.isdir(self.get_main_folder()), f'No folder found in {self.get_main_folder()}'
         assert os.path.isfile(self.get_json()), f'No json file found in {self.get_main_folder()}'
 
-        self.datapoints = ListofDatapoints.from_json(self.get_json())
+        self.datapoints = ListofDatapoints.from_json(self.get_json(), tqdm=tqdm)
 
 
 class LoadDatafolderFromLocal(LoadDatafolder):
     """Load a datafolder from local.
 
     Parameters
     ----------
@@ -391,37 +396,39 @@
 
     predict_structure : bool, optional
         If True, the structure is predicted. Default is True.
 
     predict_dms : bool, optional
         If True, the dms is predicted. Default is True.
 
+    tqdm : bool, optional
+        If True, a progress bar is displayed. Default is True.
 
     Example
     -------
 
     >>> datafolder = DataFolder.from_fasta('data/input_files_for_testing/sequences.fasta')
     >>> datafolder = DataFolder.from_dreem_output('data/input_files_for_testing/dreem_output.json')
     >>> datafolder = DataFolder.from_ct_folder('data/input_files_for_testing/ct_files')
     >>> datafolder = DataFolder.from_huggingface('for_testing')
     >>> datafolder = DataFolder.from_local('for_testing')
     """
 
-    def from_fasta(path_in, path_out=DATA_FOLDER, name = None, predict_structure = PREDICT_STRUCTURE, predict_dms = PREDICT_DMS, generate_npy = GENERATE_NPY)->CreateDatafolderFromFasta:
+    def from_fasta(path_in, path_out=DATA_FOLDER, name = None, predict_structure = PREDICT_STRUCTURE, predict_dms = PREDICT_DMS, generate_npy = GENERATE_NPY, tqdm=True)->CreateDatafolderFromFasta:
         """Create a datafolder from a fasta file. See CreateDatafolderFromFasta for more details."""
-        return CreateDatafolderFromFasta(path_in, path_out, name, predict_structure, predict_dms, generate_npy)
+        return CreateDatafolderFromFasta(path_in, path_out, name, predict_structure, predict_dms, generate_npy, tqdm=tqdm)
 
-    def from_dreem_output(path_in, path_out=DATA_FOLDER, name = None, predict_structure = PREDICT_STRUCTURE, generate_npy = GENERATE_NPY)->CreateDatafolderFromDreemOutput:
+    def from_dreem_output(path_in, path_out=DATA_FOLDER, name = None, predict_structure = PREDICT_STRUCTURE, generate_npy = GENERATE_NPY, tqdm=True)->CreateDatafolderFromDreemOutput:
         """Create a datafolder from a dreem output file. See CreateDatafolderFromDreemOutput for more details."""
-        return CreateDatafolderFromDreemOutput(path_in, path_out, name, predict_structure, generate_npy)
+        return CreateDatafolderFromDreemOutput(path_in, path_out, name, predict_structure, generate_npy, tqdm=tqdm)
 
     def from_local(name, path=DATA_FOLDER)->LoadDatafolderFromLocal:
         """Load a datafolder from local. See LoadDatafolderFromLocal for more details."""
         return LoadDatafolderFromLocal(name, path)
 
-    def from_ct_folder(path_in, path_out=DATA_FOLDER, name = None, predict_dms = PREDICT_DMS, generate_npy = GENERATE_NPY)->CreateDatafolderFromCTfolder:
+    def from_ct_folder(path_in, path_out=DATA_FOLDER, name = None, predict_dms = PREDICT_DMS, generate_npy = GENERATE_NPY, tqdm=True)->CreateDatafolderFromCTfolder:
         """Create a datafolder from a folder of ct files. See CreateDatafolderFromCTfolder for more details."""
-        return CreateDatafolderFromCTfolder(path_in, path_out, name, predict_dms, generate_npy)
+        return CreateDatafolderFromCTfolder(path_in, path_out, name, predict_dms, generate_npy, tqdm=tqdm)
 
-    def from_huggingface(name, path_out=DATA_FOLDER)->LoadDatafolderFromHF:
+    def from_huggingface(name, path_out=DATA_FOLDER, tqdm=True)->LoadDatafolderFromHF:
         """Load a datafolder from HuggingFace. See LoadDatafolderFromHF for more details."""
-        return LoadDatafolderFromHF(name, path_out)
+        return LoadDatafolderFromHF(name, path_out, tqdm=tqdm)
```

### Comparing `rouskinhf-0.1.1/rouskinhf/datapoint.py` & `rouskinhf-0.1.2/rouskinhf/datapoint.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.1/rouskinhf/env.py` & `rouskinhf-0.1.2/rouskinhf/env.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.1/rouskinhf/info_file.py` & `rouskinhf-0.1.2/rouskinhf/info_file.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.1/rouskinhf/list_datapoints.py` & `rouskinhf-0.1.2/rouskinhf/list_datapoints.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,45 +3,58 @@
 import numpy as np
 import json
 import re
 from .datapoint import Datapoint, DatapointFactory
 from typing import List, Tuple, Union, Optional
 from .parsers import Fasta, DreemOutput
 import pandas as pd
+from tqdm import tqdm as tqdm_parser
 
 class ListofDatapoints:
 
     def __init__(self, datapoints):
         self.datapoints = datapoints
 
     def __call__(self) -> List[Datapoint]:
         return self.datapoints
 
     @classmethod
-    def from_fasta(cls, fasta_file, predict_structure, predict_dms):
+    def from_fasta(cls, fasta_file, predict_structure, predict_dms, tqdm=True):
         """Create a list of datapoint from a fasta file. The structure and dms will be predicted if predict_structure and predict_dms are True."""
         sequences, references = Fasta.parse(fasta_file)
+        if tqdm:
+            return cls([DatapointFactory.from_fasta(sequence, reference, predict_structure, predict_dms)
+                    for sequence, reference in tqdm_parser(zip(sequences, references), total=len(sequences), desc='Parsing fasta file')])
         return cls([DatapointFactory.from_fasta(sequence, reference, predict_structure, predict_dms)
                     for sequence, reference in zip(sequences, references)])
 
     @classmethod
-    def from_ct(cls, ct_files, predict_dms):
+    def from_ct(cls, ct_files, predict_dms, tqdm=True):
         """Create a list of datapoint from a ct file. The dms will be predicted if predict_dms is True."""
+        if tqdm:
+            return cls([DatapointFactory.from_ct(ct_file, predict_dms) for ct_file in tqdm_parser(ct_files, total=len(ct_files), desc='Parsing ct files')])
         return cls([DatapointFactory.from_ct(ct_file, predict_dms) for ct_file in ct_files])
 
     @classmethod
-    def from_dreem_output(cls, dreem_output_file, predict_structure):
+    def from_dreem_output(cls, dreem_output_file, predict_structure, tqdm):
         """Create a list of datapoint from a dreem output file. The structure and dms will be predicted if predict_structure and predict_dms are True."""
+        print('Parsing dreem output file')
+        if tqdm:
+            n_lines = len(list(DreemOutput.parse(dreem_output_file)))
+            return cls([DatapointFactory.from_dreem_output(reference, sequence, mutation_rate, predict_structure)
+            for reference, sequence, mutation_rate in tqdm_parser(DreemOutput.parse(dreem_output_file), total=n_lines, desc='Parsing dreem output file')])
         return cls([DatapointFactory.from_dreem_output(reference, sequence, mutation_rate, predict_structure)
             for reference, sequence, mutation_rate in DreemOutput.parse(dreem_output_file)])
 
     @classmethod
-    def from_json(cls, json_file):
+    def from_json(cls, json_file, tqdm=True):
         """Create a list of datapoint from a json file."""
         with open(json_file) as f:
+            if tqdm:
+                return cls([DatapointFactory.from_json_line(line) for line in tqdm_parser(f, total=sum(1 for line in open(json_file) if line.strip() not in ['{', '}']), desc='Parsing json file') if line.strip() not in ['{', '}']])
             return cls([DatapointFactory.from_json_line(line) for line in f if line.strip() not in ['{', '}']])
 
 
     def to_base_pairs_npy(self, path):
         """Writes the structure npy file from the list of datapoints.
 
         Args:
```

### Comparing `rouskinhf-0.1.1/rouskinhf/parsers.py` & `rouskinhf-0.1.2/rouskinhf/parsers.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.1/rouskinhf/path.py` & `rouskinhf-0.1.2/rouskinhf/path.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.1/rouskinhf/rnastructure.py` & `rouskinhf-0.1.2/rouskinhf/rnastructure.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.1/rouskinhf/util.py` & `rouskinhf-0.1.2/rouskinhf/util.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.1/rouskinhf.egg-info/PKG-INFO` & `rouskinhf-0.1.2/rouskinhf.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 Metadata-Version: 2.1
 Name: rouskinhf
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library to manipulate data for our DMS prediction models.
 Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 
-# Download your RNA data from huggingface with rouskinhf!
+# Download your RNA data from HuggingFace with rouskinhf!
 
-A repo to manipulate the data for our RNA structure prediction model. The data is stored on HuggingFace and pulled locally for training models.
+A repo to manipulate the data for our RNA structure prediction model. This repo allows you to:
+- pull datasets from the Rouskinlab's HuggingFace
+- create datasets from local files and push them to HuggingFace, from the formats:
+    - `.fasta`
+    - `.ct`
+    - `.json` (DREEM output format)
+    - `.json` (Rouskinlab's huggingface format)
 
 ## Installation
 
 ### Get a HuggingFace token
 
 Go to [HuggingFace](https://huggingface.co/) and create an account. Then go to your profile and copy your token ([huggingface.co/settings/tokens](https://huggingface.co/settings/tokens)).
 
@@ -68,14 +74,31 @@
 
 ### Create a datafolder from local files and push it to HuggingFace
 
 See the [tutorial](https://github.com/rouskinlab/rouskinhf/blob/main/tutorials/create_push_pull.ipynb).
 
 ## About
 
+### Sourcing the environment and keeping your environment variable secret
+
+The variables defined in the `env` file are required by `rouskinhf`. Make that before you use `rouskinhf`, you run in a terminal:
+
+```bash
+source env
+``` 
+ or, in a Jupyter notebook:
+
+```python
+!pip install python-dotenv
+%load_ext dotenv
+%dotenv env
+```
+ 
+ The point of using environment variables is to ensure the privacy of your huggingface token. Make sure to add your `env` file to your `.gitignore`, so your HuggingFace token doesn't get pushed to any public repository.
+
 ### Import data with ``import_dataset``
 
 This repo provides a function ``import_dataset``, which allows your to pull a dataset from HuggingFace and store it locally. If the data is already stored locally, it will be loaded from the local folder. The type of data available is the DMS signal and the structure, under the shape of paired bases tuples. The function has the following signature:
 
 ```python
 def import_dataset(name:str, data:str, force_download:bool=False)->np.ndarray:
 
@@ -96,22 +119,22 @@
 
     ndarray
         The dataset with the given name for the given type of data.
 
     Example
     -------
 
-    >>> import_dataset(name='for_testing', data='structure', hf_token=os.environ['os.environ['HUGGINGFACE_TOKEN'],']).shape
-    (2,)
-    >>> import_dataset(name='for_testing', data='DMS', hf_token=os.environ['os.environ['HUGGINGFACE_TOKEN'],']).shape
-    (2,)
-    >>> import_dataset(name='for_testing', data='structure', hf_token=os.environ['os.environ['HUGGINGFACE_TOKEN'],'], force_download=True).shape
-    (2,)
-    >>> import_dataset(name='for_testing', data='DMS', hf_token=os.environ['os.environ['HUGGINGFACE_TOKEN'],'], force_download=True).shape
-    (2,)
+    >>> import_dataset(name='for_testing', data='structure').keys()
+    dict_keys(['references', 'sequences', 'structure'])
+    >>> import_dataset(name='for_testing', data='DMS').keys()
+    dict_keys(['references', 'sequences', 'DMS'])
+    >>> import_dataset(name='for_testing', data='structure', force_download=True).keys()
+    dict_keys(['references', 'sequences', 'structure'])
+    >>> import_dataset(name='for_testing', data='DMS', force_download=True).keys()
+    dict_keys(['references', 'sequences', 'DMS'])
 ```
 
 ### FYI, the datafolder object
 
 The datafolder object is a wrapper around your local folder and HuggingFace API, to keep a consistent datastructure across your datasets. It contains multiple methods to create datasets from various input formats, store the data and metadata in a systematic way, and push / pull from HuggingFace.
 
 On HuggingFace, the datafolder stores the data under the following structure:
```

