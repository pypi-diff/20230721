# Comparing `tmp/Bgolearn-2.2.1.tar.gz` & `tmp/Bgolearn-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bgolearn-2.2.1.tar", last modified: Mon Jul 17 03:33:33 2023, max compression
+gzip compressed data, was "Bgolearn-2.2.2.tar", last modified: Fri Jul 21 02:02:52 2023, max compression
```

## Comparing `Bgolearn-2.2.1.tar` & `Bgolearn-2.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 03:33:33.042426 Bgolearn-2.2.1/
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 03:33:33.041480 Bgolearn-2.2.1/Bgolearn/
--rwxr-xr-x   0 jacob      (501) staff       (20)    24206 2023-07-17 02:28:21.000000 Bgolearn-2.2.1/Bgolearn/BGO_eval.py
--rwxr-xr-x   0 jacob      (501) staff       (20)     3956 2023-07-17 03:25:17.000000 Bgolearn-2.2.1/Bgolearn/BGOclf.py
--rwxr-xr-x   0 jacob      (501) staff       (20)    18384 2023-07-17 02:35:43.000000 Bgolearn-2.2.1/Bgolearn/BGOmax.py
--rwxr-xr-x   0 jacob      (501) staff       (20)    18347 2023-07-17 02:40:08.000000 Bgolearn-2.2.1/Bgolearn/BGOmin.py
--rwxr-xr-x   0 jacob      (501) staff       (20)    21894 2023-07-17 03:26:08.000000 Bgolearn-2.2.1/Bgolearn/BGOsampling.py
--rwxr-xr-x   0 jacob      (501) staff       (20)     2472 2023-07-17 03:31:27.000000 Bgolearn-2.2.1/Bgolearn/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-17 03:33:33.042087 Bgolearn-2.2.1/Bgolearn.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-07-17 03:33:32.000000 Bgolearn-2.2.1/Bgolearn.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      300 2023-07-17 03:33:32.000000 Bgolearn-2.2.1/Bgolearn.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-07-17 03:33:32.000000 Bgolearn-2.2.1/Bgolearn.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       43 2023-07-17 03:33:32.000000 Bgolearn-2.2.1/Bgolearn.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        9 2023-07-17 03:33:32.000000 Bgolearn-2.2.1/Bgolearn.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-07-17 03:33:33.042283 Bgolearn-2.2.1/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)     1917 2022-11-06 12:06:03.000000 Bgolearn-2.2.1/README.md
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-07-17 03:33:33.042474 Bgolearn-2.2.1/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1366 2023-07-17 03:33:07.000000 Bgolearn-2.2.1/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-21 02:02:52.998887 Bgolearn-2.2.2/
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-21 02:02:52.998009 Bgolearn-2.2.2/Bgolearn/
+-rwxr-xr-x   0 jacob      (501) staff       (20)    24206 2023-07-17 02:28:21.000000 Bgolearn-2.2.2/Bgolearn/BGO_eval.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)     3956 2023-07-17 03:25:17.000000 Bgolearn-2.2.2/Bgolearn/BGOclf.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)    18384 2023-07-17 02:35:43.000000 Bgolearn-2.2.2/Bgolearn/BGOmax.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)    18347 2023-07-17 02:40:08.000000 Bgolearn-2.2.2/Bgolearn/BGOmin.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)    23554 2023-07-21 02:01:37.000000 Bgolearn-2.2.2/Bgolearn/BGOsampling.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)     1160 2023-07-21 02:01:52.000000 Bgolearn-2.2.2/Bgolearn/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-07-21 02:02:52.998593 Bgolearn-2.2.2/Bgolearn.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-07-21 02:02:52.000000 Bgolearn-2.2.2/Bgolearn.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      300 2023-07-21 02:02:52.000000 Bgolearn-2.2.2/Bgolearn.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-07-21 02:02:52.000000 Bgolearn-2.2.2/Bgolearn.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       43 2023-07-21 02:02:52.000000 Bgolearn-2.2.2/Bgolearn.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        9 2023-07-21 02:02:52.000000 Bgolearn-2.2.2/Bgolearn.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)     2478 2023-07-21 02:02:52.998754 Bgolearn-2.2.2/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)     1917 2022-11-06 12:06:03.000000 Bgolearn-2.2.2/README.md
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-07-21 02:02:52.998926 Bgolearn-2.2.2/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1366 2023-07-21 02:02:19.000000 Bgolearn-2.2.2/setup.py
```

### Comparing `Bgolearn-2.2.1/Bgolearn/BGO_eval.py` & `Bgolearn-2.2.2/Bgolearn/BGO_eval.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.2.1/Bgolearn/BGOclf.py` & `Bgolearn-2.2.2/Bgolearn/BGOclf.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.2.1/Bgolearn/BGOmax.py` & `Bgolearn-2.2.2/Bgolearn/BGOmax.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.2.1/Bgolearn/BGOmin.py` & `Bgolearn-2.2.2/Bgolearn/BGOmin.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.2.1/Bgolearn/BGOsampling.py` & `Bgolearn-2.2.2/Bgolearn/BGOsampling.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,17 +18,40 @@
 from sklearn.gaussian_process.kernels import  RBF, WhiteKernel
 from sklearn.model_selection import KFold
 
 class Bgolearn(object):
     def fit(self,data_matrix, Measured_response, virtual_samples, Mission ='Regression', Classifier = 'GaussianProcess',noise_std = None, Kriging_model = None, opt_num = 1 ,min_search = True, CV_test = False, ):
         
         """
-        PACKAGE: Bayesian global optimization learn .
+        ================================================================
+        PACKAGE: Bayesian global optimization-learn (Bgolearn) .
+        ================================================================
+        Thank you for choosing Bgolearn for material design. 
+        Bgolearn is developed to facilitate the application of machine learning in research.
+        Bgolearn is designed for optimizing single-target material properties. 
+        If you need to perform multi-target optimization, here are two important reminders:
+
+        1. Multi-tasks can be converted into a single task using domain knowledge. 
+        For example, you can use a weighted linear combination in the simplest situation. That is, y = w*y1 + y2...
+
+        2. Multi-tasks can be optimized using Pareto fronts. 
+        Bgolearn will return two arrays based on your dataset: 
+        the first array is a evaluation score for each virtual sample, 
+        while the second array is the recommended data considering only the current optimized target.
+
+        The first array is crucial for multi-task optimization. 
+        For instance, in a two-task optimization scenario, you can evaluate each candidate twice for the two separate targets. 
+        Then, plot the score of target 1 for each sample on the x-axis and the score of target 2 on the y-axis. 
+        The trade-off consideration is to select the data located in the front of the banana curve.
+
+        I am delighted to invite you to participate in the development of Bgolearn. 
+        If you have any issues or suggestions, please feel free to contact me at binjacobcao@gmail.com.
+        ================================================================
 
-        6 Apr 2023, version 1.4, Bin Cao, ZheJiang LAB, Hangzhou, CHINA. (MGI, SHU, Shanghai, CHINA).
+        Bin Cao, Advanced Materials Thrust, Hong Kong University of Science and Technology (Guangzhou).
 
         :param data_matrix: data matrix of training dataset, X .
 
         :param Measured_response: response of tarining dataset, y.
 
         :param virtual_samples: designed virtual samples.
 
@@ -77,23 +100,24 @@
         :param CV_test: 'LOOCV' or an int, default False (pass test) 
                 if CV_test = 'LOOCV', LOOCV will be applied,
                 elif CV_test = int, e.g., CV_test = 10, 10 folds cross validation will be applied.
         
         :return: 1: array; potential of each candidate. 2: array/float; recommended candidate(s).
 
         """
+
         # Fit and transform the input data matrix
         virtual_samples = preprocess_data(virtual_samples)
         data_matrix = preprocess_data(data_matrix)
         Measured_response = preprocess_data(Measured_response)
 
         row_features = copy.deepcopy(virtual_samples)
         scaler = MinMaxScaler()
-        data_matrix = scaler.fit_transform(data_matrix)
-        virtual_samples = scaler.transform(virtual_samples)
+        virtual_samples = scaler.fit_transform(virtual_samples)
+        data_matrix = scaler.transform(data_matrix)
 
         timename = time.localtime(time.time())
         namey, nameM, named, nameh, namem = timename.tm_year, timename.tm_mon, timename.tm_mday, timename.tm_hour, timename.tm_min
 
         warnings.filterwarnings('ignore')
 
         if Mission == 'Classification':
@@ -112,15 +136,15 @@
             if Kriging_model == None:
                 kernel = 1 * RBF() 
                 if noise_std == None:
                     # call the default model;
                     class Kriging_model(object):
                         def fit_pre(self,xtrain,ytrain,xtest,):
                             # estimating Noise Level of training dataset
-                            noise_ker = WhiteKernel(noise_level_bounds=(0.01,0.5))
+                            noise_ker = WhiteKernel(noise_level_bounds=(0.001,0.5))
                             GPr = GaussianProcessRegressor(kernel= 1 * RBF()+noise_ker,normalize_y=True).fit(xtrain,ytrain)
                             noise_level = np.exp(GPr.kernel_.theta[1])
         
                             # ret_std is a placeholder for homogenous noise
                             # instantiated mode
                             mdoel = GaussianProcessRegressor(kernel=kernel,normalize_y=True,alpha = noise_level).fit(xtrain,ytrain)
                             # defined the attribute's outputs
```

### Comparing `Bgolearn-2.2.1/Bgolearn.egg-info/PKG-INFO` & `Bgolearn-2.2.2/Bgolearn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bgolearn
-Version: 2.2.1
+Version: 2.2.2
 Summary: A Bayesian global optimization package for material design
 Home-page: https://github.com/Bin-Cao/Bgolearn
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `Bgolearn-2.2.1/PKG-INFO` & `Bgolearn-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bgolearn
-Version: 2.2.1
+Version: 2.2.2
 Summary: A Bayesian global optimization package for material design
 Home-page: https://github.com/Bin-Cao/Bgolearn
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `Bgolearn-2.2.1/README.md` & `Bgolearn-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.2.1/setup.py` & `Bgolearn-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='Bgolearn',  # 包名
-    version='2.2.1',  # 版本
+    version='2.2.2',  # 版本
     description="A Bayesian global optimization package for material design",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='binjacobcao@gmail.com',  # 维护者邮件
```

