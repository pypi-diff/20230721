# Comparing `tmp/gmltools-0.0.92.tar.gz` & `tmp/gmltools-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.92.tar", last modified: Fri Jul 21 10:01:56 2023, max compression
+gzip compressed data, was "gmltools-0.0.93.tar", last modified: Fri Jul 21 11:51:40 2023, max compression
```

## Comparing `gmltools-0.0.92.tar` & `gmltools-0.0.93.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 10:01:56.036728 gmltools-0.0.92/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.92/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.92/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-07-21 10:01:56.035728 gmltools-0.0.92/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.92/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 10:01:56.014726 gmltools-0.0.92/dist/
--rw-rw-rw-   0        0        0    78901 2023-06-14 08:50:22.000000 gmltools-0.0.92/dist/gmltools-0.0.80.tar.gz
--rw-rw-rw-   0        0        0    78864 2023-06-14 08:54:29.000000 gmltools-0.0.92/dist/gmltools-0.0.81.tar.gz
--rw-rw-rw-   0        0        0    79689 2023-06-26 15:34:26.000000 gmltools-0.0.92/dist/gmltools-0.0.82.tar.gz
--rw-rw-rw-   0        0        0      483 2023-04-27 11:36:50.000000 gmltools-0.0.92/environment.txt
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.92/gmltools.yml
--rw-rw-rw-   0        0        0    17997 2023-04-17 10:10:38.000000 gmltools-0.0.92/gmltools2.yml
--rw-rw-rw-   0        0        0    17200 2023-04-24 08:57:47.000000 gmltools-0.0.92/gmltools3.yml
--rw-rw-rw-   0        0        0     4638 2023-04-26 09:14:46.000000 gmltools-0.0.92/gmltools4.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.92/mltools.yml
--rw-rw-rw-   0        0        0      618 2023-07-21 10:01:38.000000 gmltools-0.0.92/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-21 10:01:56.036728 gmltools-0.0.92/setup.cfg
--rw-rw-rw-   0        0        0     1746 2023-07-21 10:01:32.000000 gmltools-0.0.92/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:01:55.997729 gmltools-0.0.92/src/
-drwxrwxrwx   0        0        0        0 2023-07-21 10:01:56.016728 gmltools-0.0.92/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.92/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.92/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:01:56.022727 gmltools-0.0.92/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.92/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    50752 2023-07-21 10:01:19.000000 gmltools-0.0.92/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:01:56.028733 gmltools-0.0.92/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.92/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.92/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.92/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.92/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   165893 2023-07-20 07:49:43.000000 gmltools-0.0.92/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     7529 2023-07-20 07:31:38.000000 gmltools-0.0.92/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    33623 2023-07-06 11:21:54.000000 gmltools-0.0.92/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:01:56.031730 gmltools-0.0.92/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.92/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.92/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.92/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:01:56.034728 gmltools-0.0.92/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.92/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.92/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.92/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.92/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:01:56.021727 gmltools-0.0.92/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-07-21 10:01:55.000000 gmltools-0.0.92/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1048 2023-07-21 10:01:55.000000 gmltools-0.0.92/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 10:01:55.000000 gmltools-0.0.92/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2023-07-21 10:01:55.000000 gmltools-0.0.92/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 10:01:55.000000 gmltools-0.0.92/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 11:51:40.274074 gmltools-0.0.93/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.93/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.93/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-07-21 11:51:40.273080 gmltools-0.0.93/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.93/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 11:51:40.241894 gmltools-0.0.93/dist/
+-rw-rw-rw-   0        0        0    78901 2023-06-14 08:50:22.000000 gmltools-0.0.93/dist/gmltools-0.0.80.tar.gz
+-rw-rw-rw-   0        0        0    78864 2023-06-14 08:54:29.000000 gmltools-0.0.93/dist/gmltools-0.0.81.tar.gz
+-rw-rw-rw-   0        0        0    79689 2023-06-26 15:34:26.000000 gmltools-0.0.93/dist/gmltools-0.0.82.tar.gz
+-rw-rw-rw-   0        0        0      483 2023-04-27 11:36:50.000000 gmltools-0.0.93/environment.txt
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.93/gmltools.yml
+-rw-rw-rw-   0        0        0    17997 2023-04-17 10:10:38.000000 gmltools-0.0.93/gmltools2.yml
+-rw-rw-rw-   0        0        0    17200 2023-04-24 08:57:47.000000 gmltools-0.0.93/gmltools3.yml
+-rw-rw-rw-   0        0        0     4638 2023-04-26 09:14:46.000000 gmltools-0.0.93/gmltools4.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.93/mltools.yml
+-rw-rw-rw-   0        0        0      618 2023-07-21 11:51:13.000000 gmltools-0.0.93/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-21 11:51:40.274074 gmltools-0.0.93/setup.cfg
+-rw-rw-rw-   0        0        0     1746 2023-07-21 11:51:06.000000 gmltools-0.0.93/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:51:40.222853 gmltools-0.0.93/src/
+drwxrwxrwx   0        0        0        0 2023-07-21 11:51:40.244854 gmltools-0.0.93/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.93/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.93/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:51:40.253895 gmltools-0.0.93/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.93/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    50755 2023-07-21 11:50:50.000000 gmltools-0.0.93/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:51:40.264082 gmltools-0.0.93/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.93/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.93/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.93/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.93/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   165893 2023-07-20 07:49:43.000000 gmltools-0.0.93/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     7529 2023-07-20 07:31:38.000000 gmltools-0.0.93/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    33623 2023-07-06 11:21:54.000000 gmltools-0.0.93/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:51:40.267081 gmltools-0.0.93/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.93/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.93/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.93/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:51:40.272082 gmltools-0.0.93/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.93/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.93/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.93/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.93/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:51:40.251894 gmltools-0.0.93/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-07-21 11:51:39.000000 gmltools-0.0.93/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1048 2023-07-21 11:51:40.000000 gmltools-0.0.93/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 11:51:39.000000 gmltools-0.0.93/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-07-21 11:51:39.000000 gmltools-0.0.93/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-21 11:51:39.000000 gmltools-0.0.93/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.92/LICENSE` & `gmltools-0.0.93/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/Models.ipynb` & `gmltools-0.0.93/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/PKG-INFO` & `gmltools-0.0.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.92
+Version: 0.0.93
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.92/README.md` & `gmltools-0.0.93/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/dist/gmltools-0.0.80.tar.gz` & `gmltools-0.0.93/dist/gmltools-0.0.80.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/dist/gmltools-0.0.81.tar.gz` & `gmltools-0.0.93/dist/gmltools-0.0.81.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/dist/gmltools-0.0.82.tar.gz` & `gmltools-0.0.93/dist/gmltools-0.0.82.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/gmltools.yml` & `gmltools-0.0.93/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/gmltools2.yml` & `gmltools-0.0.93/gmltools2.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/gmltools3.yml` & `gmltools-0.0.93/gmltools3.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/gmltools4.yml` & `gmltools-0.0.93/gmltools4.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/mltools.yml` & `gmltools-0.0.93/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/pyproject.toml` & `gmltools-0.0.93/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.92"
+version = "0.0.93"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.92/setup.py` & `gmltools-0.0.93/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0', 'lightgbm>=3.3.5', 'linear-tree>=0.3.5', 'scikit-learn>=1.2.1']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.92',
+    'version': '0.0.93',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.92/src/gmltools/To_Do.txt` & `gmltools-0.0.93/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/src/gmltools/eda/eda.py` & `gmltools-0.0.93/src/gmltools/eda/eda.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,15 +447,15 @@
 #--------------------------------------------------------PLOT DATA--------------------------------------------------------#
 class ExploreManager:
     def __init__(self,df):
         self.df=df
 
 
 
-    def plot_correlation(self, method='pearson', figsize=(1000,1000), colorscale='agsunset', title=None, title_size=24, label_size=14, annotation_font_size=10, save=False, save_path="./imgs/correlations/"):
+    def plot_correlation(self, method='pearson', figsize=(1000,1000), colorscale='agsunset', title=None, title_size=24, label_size=14, annotation_font_size=10, save=False, save_path="./imgs/correlations/",show=True):
         """
         Plotly heatmap of the correlation matrix of a dataframe
 
         Parameters
         ----------
         df : pd.DataFrame
 
@@ -505,15 +505,16 @@
         fig.update_traces(colorscale='agsunset')
 
         # Increase annotation font size
         for i in range(len(fig.layout.annotations)):
             fig.layout.annotations[i].font.size = annotation_font_size
 
         fig.update_layout(width=figsize[0], height=figsize[1])
-        fig.show()
+        if show:
+            fig.show()
 
         # Check if save is set to True
         if save:
             # Check if the directory exists
             if not os.path.exists(save_path):
                 # If the directory does not exist, create it
                 os.makedirs(save_path)
@@ -1021,15 +1022,15 @@
             date : str
                 Date to plot similar pattern
             """
             patrons=self.get_similar_pattern(date)
             patrons=patrons.iloc[:5]
             patrons_date=patrons.iloc[:,0].apply(lambda x: x.strftime('%Y-%m-%d')).values
 
-            print(patrons_date)
+  
             #drop on eif its duplicated
             
             self.patron=patrons
             self.patron_date=patrons_date
             height_adjuts= len(patrons)
     
             patron_profile= [str(row[0].date()) + " , Euclidian Distance Value: " + str(round(row[1],2)) for index, row in patrons.iterrows()]
```

### Comparing `gmltools-0.0.92/src/gmltools/models/bayes.py` & `gmltools-0.0.93/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.93/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/src/gmltools/models/dummy_model.py` & `gmltools-0.0.93/src/gmltools/models/dummy_model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/src/gmltools/models/model.py` & `gmltools-0.0.93/src/gmltools/models/model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/src/gmltools/models/models_info.py` & `gmltools-0.0.93/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.93/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.93/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.93/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.93/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.93/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.93/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.92/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.93/src/gmltools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.92
+Version: 0.0.93
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.92/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.93/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

