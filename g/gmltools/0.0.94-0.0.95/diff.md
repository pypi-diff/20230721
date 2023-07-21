# Comparing `tmp/gmltools-0.0.94.tar.gz` & `tmp/gmltools-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.94.tar", last modified: Fri Jul 21 12:05:27 2023, max compression
+gzip compressed data, was "gmltools-0.0.95.tar", last modified: Fri Jul 21 12:08:33 2023, max compression
```

## Comparing `gmltools-0.0.94.tar` & `gmltools-0.0.95.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 12:05:27.264617 gmltools-0.0.94/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.94/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.94/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-07-21 12:05:27.263623 gmltools-0.0.94/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.94/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 12:05:27.182034 gmltools-0.0.94/dist/
--rw-rw-rw-   0        0        0    78901 2023-06-14 08:50:22.000000 gmltools-0.0.94/dist/gmltools-0.0.80.tar.gz
--rw-rw-rw-   0        0        0    78864 2023-06-14 08:54:29.000000 gmltools-0.0.94/dist/gmltools-0.0.81.tar.gz
--rw-rw-rw-   0        0        0    79689 2023-06-26 15:34:26.000000 gmltools-0.0.94/dist/gmltools-0.0.82.tar.gz
--rw-rw-rw-   0        0        0      483 2023-04-27 11:36:50.000000 gmltools-0.0.94/environment.txt
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.94/gmltools.yml
--rw-rw-rw-   0        0        0    17997 2023-04-17 10:10:38.000000 gmltools-0.0.94/gmltools2.yml
--rw-rw-rw-   0        0        0    17200 2023-04-24 08:57:47.000000 gmltools-0.0.94/gmltools3.yml
--rw-rw-rw-   0        0        0     4638 2023-04-26 09:14:46.000000 gmltools-0.0.94/gmltools4.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.94/mltools.yml
--rw-rw-rw-   0        0        0      618 2023-07-21 12:04:43.000000 gmltools-0.0.94/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-21 12:05:27.264617 gmltools-0.0.94/setup.cfg
--rw-rw-rw-   0        0        0     1746 2023-07-21 12:04:36.000000 gmltools-0.0.94/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 12:05:27.131019 gmltools-0.0.94/src/
-drwxrwxrwx   0        0        0        0 2023-07-21 12:05:27.190100 gmltools-0.0.94/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.94/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.94/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 12:05:27.206079 gmltools-0.0.94/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.94/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    50781 2023-07-21 12:05:12.000000 gmltools-0.0.94/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-07-21 12:05:27.232615 gmltools-0.0.94/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.94/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.94/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.94/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.94/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   165893 2023-07-20 07:49:43.000000 gmltools-0.0.94/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     7529 2023-07-20 07:31:38.000000 gmltools-0.0.94/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    33623 2023-07-06 11:21:54.000000 gmltools-0.0.94/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-07-21 12:05:27.244622 gmltools-0.0.94/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.94/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.94/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.94/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-07-21 12:05:27.261618 gmltools-0.0.94/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.94/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.94/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.94/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.94/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-07-21 12:05:27.194996 gmltools-0.0.94/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-07-21 12:05:26.000000 gmltools-0.0.94/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1048 2023-07-21 12:05:26.000000 gmltools-0.0.94/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 12:05:26.000000 gmltools-0.0.94/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2023-07-21 12:05:26.000000 gmltools-0.0.94/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 12:05:26.000000 gmltools-0.0.94/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 12:08:33.188786 gmltools-0.0.95/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.95/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.95/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-07-21 12:08:33.188786 gmltools-0.0.95/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.95/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 12:08:33.164773 gmltools-0.0.95/dist/
+-rw-rw-rw-   0        0        0    78901 2023-06-14 08:50:22.000000 gmltools-0.0.95/dist/gmltools-0.0.80.tar.gz
+-rw-rw-rw-   0        0        0    78864 2023-06-14 08:54:29.000000 gmltools-0.0.95/dist/gmltools-0.0.81.tar.gz
+-rw-rw-rw-   0        0        0    79689 2023-06-26 15:34:26.000000 gmltools-0.0.95/dist/gmltools-0.0.82.tar.gz
+-rw-rw-rw-   0        0        0      483 2023-04-27 11:36:50.000000 gmltools-0.0.95/environment.txt
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.95/gmltools.yml
+-rw-rw-rw-   0        0        0    17997 2023-04-17 10:10:38.000000 gmltools-0.0.95/gmltools2.yml
+-rw-rw-rw-   0        0        0    17200 2023-04-24 08:57:47.000000 gmltools-0.0.95/gmltools3.yml
+-rw-rw-rw-   0        0        0     4638 2023-04-26 09:14:46.000000 gmltools-0.0.95/gmltools4.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.95/mltools.yml
+-rw-rw-rw-   0        0        0      618 2023-07-21 12:08:13.000000 gmltools-0.0.95/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-21 12:08:33.189778 gmltools-0.0.95/setup.cfg
+-rw-rw-rw-   0        0        0     1746 2023-07-21 12:08:07.000000 gmltools-0.0.95/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:08:33.148774 gmltools-0.0.95/src/
+drwxrwxrwx   0        0        0        0 2023-07-21 12:08:33.166774 gmltools-0.0.95/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.95/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.95/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:08:33.173774 gmltools-0.0.95/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.95/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    50777 2023-07-21 12:07:59.000000 gmltools-0.0.95/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:08:33.181779 gmltools-0.0.95/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.95/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.95/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.95/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.95/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   165893 2023-07-20 07:49:43.000000 gmltools-0.0.95/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     7529 2023-07-20 07:31:38.000000 gmltools-0.0.95/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    33623 2023-07-06 11:21:54.000000 gmltools-0.0.95/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:08:33.183786 gmltools-0.0.95/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.95/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.95/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.95/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:08:33.187778 gmltools-0.0.95/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.95/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.95/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.95/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.95/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-07-21 12:08:33.171775 gmltools-0.0.95/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-07-21 12:08:32.000000 gmltools-0.0.95/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1048 2023-07-21 12:08:33.000000 gmltools-0.0.95/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 12:08:32.000000 gmltools-0.0.95/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-07-21 12:08:32.000000 gmltools-0.0.95/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-21 12:08:32.000000 gmltools-0.0.95/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.94/LICENSE` & `gmltools-0.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/Models.ipynb` & `gmltools-0.0.95/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/PKG-INFO` & `gmltools-0.0.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.94
+Version: 0.0.95
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.94/README.md` & `gmltools-0.0.95/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/dist/gmltools-0.0.80.tar.gz` & `gmltools-0.0.95/dist/gmltools-0.0.80.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/dist/gmltools-0.0.81.tar.gz` & `gmltools-0.0.95/dist/gmltools-0.0.81.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/dist/gmltools-0.0.82.tar.gz` & `gmltools-0.0.95/dist/gmltools-0.0.82.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/gmltools.yml` & `gmltools-0.0.95/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/gmltools2.yml` & `gmltools-0.0.95/gmltools2.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/gmltools3.yml` & `gmltools-0.0.95/gmltools3.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/gmltools4.yml` & `gmltools-0.0.95/gmltools4.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/mltools.yml` & `gmltools-0.0.95/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/pyproject.toml` & `gmltools-0.0.95/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.94"
+version = "0.0.95"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.94/setup.py` & `gmltools-0.0.95/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0', 'lightgbm>=3.3.5', 'linear-tree>=0.3.5', 'scikit-learn>=1.2.1']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.94',
+    'version': '0.0.95',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.94/src/gmltools/To_Do.txt` & `gmltools-0.0.95/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/src/gmltools/eda/eda.py` & `gmltools-0.0.95/src/gmltools/eda/eda.py`

 * *Files 0% similar despite different names*

```diff
@@ -519,15 +519,15 @@
                 # If the directory does not exist, create it
                 os.makedirs(save_path)
 
             # Save the figure
             
             pio.write_image(fig, save_path + f'{title}_correlation_heatmap.png')
 
-            return fig
+        return fig
 
 
 
 
 
     def plot_distribution(self, bins:int=50, figsize:tuple=(600, 400), save_name="", category_column=None, x_range=None, shared_yaxes:bool=False, shared_xaxes:bool=False, histnorm=None, label_size:int=14, tick_size:int=12, title_size:int=16):
         """
```

### Comparing `gmltools-0.0.94/src/gmltools/models/bayes.py` & `gmltools-0.0.95/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.95/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/src/gmltools/models/dummy_model.py` & `gmltools-0.0.95/src/gmltools/models/dummy_model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/src/gmltools/models/model.py` & `gmltools-0.0.95/src/gmltools/models/model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/src/gmltools/models/models_info.py` & `gmltools-0.0.95/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.95/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.95/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.95/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.95/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.95/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.95/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.94/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.95/src/gmltools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.94
+Version: 0.0.95
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.94/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.95/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

