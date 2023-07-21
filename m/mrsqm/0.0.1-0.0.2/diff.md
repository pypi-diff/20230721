# Comparing `tmp/mrsqm-0.0.1.tar.gz` & `tmp/mrsqm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrsqm-0.0.1.tar", last modified: Wed Feb 15 23:58:05 2023, max compression
+gzip compressed data, was "mrsqm-0.0.2.tar", last modified: Fri Jul 21 17:57:28 2023, max compression
```

## Comparing `mrsqm-0.0.1.tar` & `mrsqm-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 23:58:05.201147 mrsqm-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-15 23:57:50.000000 mrsqm-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-15 23:57:50.000000 mrsqm-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-15 23:58:05.201147 mrsqm-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-02-15 23:57:50.000000 mrsqm-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-02-15 23:57:50.000000 mrsqm-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 23:58:05.201147 mrsqm-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-02-15 23:57:50.000000 mrsqm-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 23:58:05.197147 mrsqm-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 23:58:05.197147 mrsqm-0.0.1/src/mrsqm/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-15 23:57:50.000000 mrsqm-0.0.1/src/mrsqm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-02-15 23:57:50.000000 mrsqm-0.0.1/src/mrsqm/common.h
--rw-r--r--   0 runner    (1001) docker     (123)   863383 2023-02-15 23:58:04.000000 mrsqm-0.0.1/src/mrsqm/mrsqm_wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19013 2023-02-15 23:57:50.000000 mrsqm-0.0.1/src/mrsqm/mrsqm_wrapper.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-02-15 23:57:50.000000 mrsqm-0.0.1/src/mrsqm/sax_converter.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 23:58:05.201147 mrsqm-0.0.1/src/mrsqm/sfa/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1478 2023-02-15 23:57:50.000000 mrsqm-0.0.1/src/mrsqm/sfa/DFT.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-02-15 23:57:50.000000 mrsqm-0.0.1/src/mrsqm/sfa/DFT.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     7383 2023-02-15 23:57:50.000000 mrsqm-0.0.1/src/mrsqm/sfa/MFT.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)      924 2023-02-15 23:57:50.000000 mrsqm-0.0.1/src/mrsqm/sfa/MFT.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     4766 2023-02-15 23:57:50.000000 mrsqm-0.0.1/src/mrsqm/sfa/SFA.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-02-15 23:57:50.000000 mrsqm-0.0.1/src/mrsqm/sfa/SFA.h
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-02-15 23:57:50.000000 mrsqm-0.0.1/src/mrsqm/sfa/SFAWrapper.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     4103 2023-02-15 23:57:50.000000 mrsqm-0.0.1/src/mrsqm/sfa/TimeSeries.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     1055 2023-02-15 23:57:50.000000 mrsqm-0.0.1/src/mrsqm/sfa/TimeSeries.h
--rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-02-15 23:57:50.000000 mrsqm-0.0.1/src/mrsqm/sqminer.h
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-02-15 23:57:50.000000 mrsqm-0.0.1/src/mrsqm/strie.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 23:58:05.197147 mrsqm-0.0.1/src/mrsqm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-15 23:58:05.000000 mrsqm-0.0.1/src/mrsqm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-15 23:58:05.000000 mrsqm-0.0.1/src/mrsqm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 23:58:05.000000 mrsqm-0.0.1/src/mrsqm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-15 23:58:05.000000 mrsqm-0.0.1/src/mrsqm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:57:28.904968 mrsqm-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 17:57:16.000000 mrsqm-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-21 17:57:16.000000 mrsqm-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-21 17:57:28.904968 mrsqm-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-21 17:57:16.000000 mrsqm-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-21 17:57:16.000000 mrsqm-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 17:57:28.904968 mrsqm-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-21 17:57:16.000000 mrsqm-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:57:28.900968 mrsqm-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:57:28.904968 mrsqm-0.0.2/src/mrsqm/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-21 17:57:16.000000 mrsqm-0.0.2/src/mrsqm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-21 17:57:16.000000 mrsqm-0.0.2/src/mrsqm/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)  1158333 2023-07-21 17:57:28.000000 mrsqm-0.0.2/src/mrsqm/mrsqm_wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21629 2023-07-21 17:57:16.000000 mrsqm-0.0.2/src/mrsqm/mrsqm_wrapper.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-07-21 17:57:16.000000 mrsqm-0.0.2/src/mrsqm/sax_converter.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:57:28.904968 mrsqm-0.0.2/src/mrsqm/sfa/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1478 2023-07-21 17:57:16.000000 mrsqm-0.0.2/src/mrsqm/sfa/DFT.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-07-21 17:57:16.000000 mrsqm-0.0.2/src/mrsqm/sfa/DFT.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7383 2023-07-21 17:57:16.000000 mrsqm-0.0.2/src/mrsqm/sfa/MFT.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)      924 2023-07-21 17:57:16.000000 mrsqm-0.0.2/src/mrsqm/sfa/MFT.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4766 2023-07-21 17:57:16.000000 mrsqm-0.0.2/src/mrsqm/sfa/SFA.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-21 17:57:16.000000 mrsqm-0.0.2/src/mrsqm/sfa/SFA.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-21 17:57:16.000000 mrsqm-0.0.2/src/mrsqm/sfa/SFAWrapper.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4103 2023-07-21 17:57:16.000000 mrsqm-0.0.2/src/mrsqm/sfa/TimeSeries.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1055 2023-07-21 17:57:16.000000 mrsqm-0.0.2/src/mrsqm/sfa/TimeSeries.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-07-21 17:57:16.000000 mrsqm-0.0.2/src/mrsqm/sqminer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-21 17:57:16.000000 mrsqm-0.0.2/src/mrsqm/strie.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:57:28.904968 mrsqm-0.0.2/src/mrsqm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-21 17:57:28.000000 mrsqm-0.0.2/src/mrsqm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-21 17:57:28.000000 mrsqm-0.0.2/src/mrsqm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 17:57:28.000000 mrsqm-0.0.2/src/mrsqm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 17:57:28.000000 mrsqm-0.0.2/src/mrsqm.egg-info/top_level.txt
```

### Comparing `mrsqm-0.0.1/LICENSE` & `mrsqm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mrsqm-0.0.1/README.md` & `mrsqm-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,19 @@
 ```
 cython >= 0.29
 numpy >= 1.18
 pandas >= 1.0.3
 scikit-learn >= 0.22
 fftw3 (http://www.fftw.org/)
 ```
+## Installation using pip
+pip install mrsqm
 
+
+## Installation from source
 Download the repository: 
 ```
 git clone https://github.com/mlgig/mrsqm.git
 ```
 Move into the code directory of the repository: 
 ```
 cd mrsqm/mrsqm
@@ -36,15 +40,15 @@
 Load data from arff files
 ```
 X_train,y_train = util.load_from_arff_to_dataframe("data/Coffee/Coffee_TRAIN.arff")
 X_test,y_test = util.load_from_arff_to_dataframe("data/Coffee/Coffee_TEST.arff")
 ```
 Train with MrSQM
 ```
-clf = MrSQMClassifier()
+clf = MrSQMClassifier(nsax=0, nsfa=5)
 clf.fit(X_train,y_train)
 ```
 
 Make predictions
 ```
 predicted = clf.predict(X_test)
 ```
```

### Comparing `mrsqm-0.0.1/setup.py` & `mrsqm-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
                    sources=["src/mrsqm/mrsqm_wrapper.pyx","src/mrsqm/sfa/MFT.cpp","src/mrsqm/sfa/DFT.cpp","src/mrsqm/sfa/SFA.cpp","src/mrsqm/sfa/TimeSeries.cpp"],
                    extra_compile_args=["-Wall", "-Ofast", "-g", "-std=c++11", "-ffast-math"],
                    extra_link_args=["-lfftw3", "-lm", "-L/opt/local/lib"],           
                    include_dirs=['src/mrsqm'])
 
 setup(
     name='mrsqm',
-    version="0.0.1",
+    version="0.0.2",
     author='Thach Le Nguyen',
     author_email='thalng@protonmail.com',
     setup_requires=[
         'setuptools',  # first version to support pyx in Extension
         'cython',
     ],
     packages=find_packages(where='src'),
```

### Comparing `mrsqm-0.0.1/src/mrsqm/common.h` & `mrsqm-0.0.2/src/mrsqm/common.h`

 * *Files identical despite different names*

### Comparing `mrsqm-0.0.1/src/mrsqm/mrsqm_wrapper.pyx` & `mrsqm-0.0.2/src/mrsqm/mrsqm_wrapper.pyx`

 * *Files 12% similar despite different names*

```diff
@@ -202,18 +202,16 @@
         self.thisptr = new SQMiner(selection,threshold)
     def __dealloc__(self):
         del self.thisptr
 
     def mine(self, vector[string] sequences, vector[int] labels):
         return self.thisptr.mine(sequences, labels)     
 
-
-######################### MrSQM Classifier #########################
-
-class MrSQMClassifier:    
+######################### MrSQM Transformer #########################
+class MrSQMTransformer:
     '''     
     Overview: MrSQM is an efficient time series classifier utilizing symbolic representations of time series. MrSQM implements four different feature selection strategies (R,S,RS,SR) that can quickly select subsequences from multiple symbolic representations of time series data.
     def __init__(self, strat = 'RS', features_per_rep = 500, selection_per_rep = 2000, nsax = 1, nsfa = 0, custom_config=None, random_state = None, sfa_norm = True):
 
     Parameters
     ----------
     
@@ -455,75 +453,116 @@
         debug_logging("Search for subsequences.")        
         mr_seqs = self.transform_time_series(X)
         
         
         
         for rep in mr_seqs:
             mined = self.mine(rep,int_y)
-            self.sequences.append(mined)
-
-
-    
-        # first computing the feature vectors
-        # then fit the new data to a logistic regression model
+            self.sequences.append(mined)  
         
-        debug_logging("Compute feature vectors.")
-        train_x = self.feature_selection_on_train(mr_seqs, int_y)
         
-        debug_logging("Fit logistic regression model.")
-        self.clf = LogisticRegression(solver='newton-cg',multi_class = 'multinomial', class_weight='balanced').fit(train_x, y)        
-        # self.clf = RidgeClassifierCV(alphas = np.logspace(-3, 3, 10), normalize = True).fit(train_x, y)        
-        self.classes_ = self.clf.classes_ # shouldn't matter  
+        self.feature_selection_on_train(mr_seqs, int_y)       
 
         return self
+    
+    def fit_transform(self, X, y):
+        debug_logging("Fit training data.")
+        self.classes_ = np.unique(y) #because sklearn also uses np.unique
 
+        int_y = [np.where(self.classes_ == c)[0][0] for c in y]
 
-    def predict_proba(self, X): 
-        mr_seqs = self.transform_time_series(X)       
-        test_x = self.feature_selection_on_test(mr_seqs)
-        return self.clf.predict_proba(test_x) 
+        self.sequences = []
 
-    def predict(self, X):
-        mr_seqs = self.transform_time_series(X)       
-        test_x = self.feature_selection_on_test(mr_seqs)
-        return self.clf.predict(test_x)
+        debug_logging("Search for subsequences.")        
+        mr_seqs = self.transform_time_series(X)
+        
+        
+        
+        for rep in mr_seqs:
+            mined = self.mine(rep,int_y)
+            self.sequences.append(mined)
+    
+        
+        
+        debug_logging("Compute feature vectors.")
+        train_x = self.feature_selection_on_train(mr_seqs, int_y)       
+
+        return train_x
 
-    def decision_function(self, X):
+    def transform(self,X):
         mr_seqs = self.transform_time_series(X)       
-        test_x = self.feature_selection_on_test(mr_seqs)
-        return self.clf.decision_function(test_x)
+        X_transform = self.feature_selection_on_test(mr_seqs)
+        return X_transform
 
-    def get_saliency_map(self, ts):        
+    
+    def get_saliency_map(self, ts, coefs):        
 
         is_multiclass = len(self.classes_) > 2
         weighted_ts = np.zeros((len(self.classes_), len(ts)))
 
         fi = 0
         for cfg, features in zip(self.config, self.sequences):
             if cfg['method'] == 'sax':
                 ps = PySAX(cfg['window'], cfg['word'], cfg['alphabet'])
                 if is_multiclass:
                     for ci, cl in enumerate(self.classes_):
                         weighted_ts[ci, :] += ps.map_weighted_patterns(
-                            ts, features, self.clf.coef_[ci, fi:(fi+len(features))])
+                            ts, features, coefs[ci, fi:(fi+len(features))])
                 else:
                     # because classes_[1] is the positive class
                     weighted_ts[1, :] += ps.map_weighted_patterns(
-                        ts, features, self.clf.coef_[0, fi:(fi+len(features))])
+                        ts, features, coefs[0, fi:(fi+len(features))])
 
             fi += len(features)
         if not is_multiclass:
             weighted_ts[0, :] = -weighted_ts[1, :]
         return weighted_ts
-        
 
 
 
+######################### MrSQM Classifier #########################
+
+class MrSQMClassifier:
+    '''     
+    Overview: MrSQM is an efficient time series classifier utilizing symbolic representations of time series. MrSQM implements four different feature selection strategies (R,S,RS,SR) that can quickly select subsequences from multiple symbolic representations of time series data.
+    def __init__(self, strat = 'RS', features_per_rep = 500, selection_per_rep = 2000, nsax = 1, nsfa = 0, custom_config=None, random_state = None, sfa_norm = True):
+
+    Parameters
+    ----------
+    
+    strat               : str, feature selection strategy, either 'R','S','SR', or 'RS'. R and S are single-stage filters while RS and SR are two-stage filters. By default set to 'RS'.
+    features_per_rep    : int, (maximum) number of features selected per representation. By deafault set to 500.
+    selection_per_rep   : int, (maximum) number of candidate features selected per representation. Only applied in two stages strategies (RS and SR). By deafault set to 2000.
+    nsax                : int, control the number of representations produced by sax transformation.
+    nsfa                : int, control the number of representations produced by sfa transformation.
+    custom_config       : dict, customized parameters for the symbolic transformation.
+    random_state        : set random seed for classifier. By default 'none'.
+    ts_norm             : time series normalisation (standardisation). By default set to 'True'.
 
+    '''
+    def __init__(self, strat = 'RS', features_per_rep = 500, selection_per_rep = 2000, nsax = 1, nsfa = 0, custom_config=None, random_state = None, sfa_norm = True):        
+        self.transformer = MrSQMTransformer(strat = strat, features_per_rep = features_per_rep, selection_per_rep = selection_per_rep, nsax = nsax, nsfa = nsfa, custom_config = custom_config, random_state = random_state, sfa_norm = sfa_norm)
+    
+    def fit(self, X, y):
+        debug_logging("Fit training data.")        
+        train_x = self.transformer.fit_transform(X,y)
+        debug_logging("Fit logistic regression model.")
+        self.clf = LogisticRegression(solver='newton-cg',multi_class = 'multinomial', class_weight='balanced').fit(train_x, y)        
+        # self.clf = RidgeClassifierCV(alphas = np.logspace(-3, 3, 10), normalize = True).fit(train_x, y)        
+        self.classes_ = self.clf.classes_ # shouldn't matter  
 
- 
+        return self
 
 
+    def predict_proba(self, X):         
+        return self.clf.predict_proba(self.transformer.transform(X)) 
 
+    def predict(self, X):        
+        return self.clf.predict(self.transformer.transform(X))
 
+    def decision_function(self, X):        
+        return self.clf.decision_function(self.transformer.transform(X))
 
+    def get_saliency_map(self, ts):
+        return self.transformer.get_saliency_map(ts,self.clf.coef_)
 
+
```

### Comparing `mrsqm-0.0.1/src/mrsqm/sax_converter.h` & `mrsqm-0.0.2/src/mrsqm/sax_converter.h`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 { -1.69062162958, -1.33517773612, -1.09680356209, -0.908457868537, -0.747858594763, -0.604585346583, -0.472789120992, -0.348755695517, -0.229884117579, -0.114185294321, 0.0, 0.114185294321, 0.229884117579, 0.348755695517, 0.472789120992, 0.604585346583, 0.747858594763, 0.908457868537, 1.09680356209, 1.33517773612, 1.69062162958 };
 { -1.71167530651, -1.35973738394, -1.12433823157, -0.938814316877, -0.781033811523, -0.640666889919, -0.511936213871, -0.391196258189, -0.275921063108, -0.164210777079, -0.0545189148481, 0.0545189148481, 0.164210777079, 0.275921063108, 0.391196258189, 0.511936213871, 0.640666889919, 0.781033811523, 0.938814316877, 1.12433823157, 1.35973738394, 1.71167530651 };
 		 */
 	}
 
 	
 
-	std::string segment2SAX(std::vector<double> &timeseries, int cur_pos, char char_start){
+	std::string segment2SAX(std::vector<double> timeseries, int cur_pos, char char_start){
 		int window_end = cur_pos + (window_size-1)*dilation;
 		
 		
 
 		// calculate mean and std
 		double mean_wd = 0.0;
 		double var_wd = 0.0;
@@ -235,15 +235,15 @@
 		}
 
 		return sax_word;
 
 	}
 
 	//main function to convert a vector of double to a vector of SAX sequences
-	std::vector<std::string> timeseries2SAX(std::vector<double> &timeseries, char char_start){
+	std::vector<std::string> timeseries2SAX(std::vector<double> timeseries, char char_start){
 
 		// length of the time series
 		int ts_length = timeseries.size();
 		std::vector<std::string>  sax_seqc;
 		// sliding windows
 
 		for (int cur_pos = 0; cur_pos < ts_length - (window_size-1)*dilation; cur_pos += step_size){
@@ -277,15 +277,15 @@
 				break;
 			}
 		}
 		return sax_seqc;
 	}
 
 	// same but always use 'abc..' for the alphabet
-	std::vector<std::string> timeseries2SAX(std::vector<double> &timeseries){
+	std::vector<std::string> timeseries2SAX(std::vector<double> timeseries){
 		char char_start = 'a';
 		return timeseries2SAX(timeseries,char_start);
 	}
 
 
 
 	// set of patterns instead of a single pattern
```

### Comparing `mrsqm-0.0.1/src/mrsqm/sfa/DFT.cpp` & `mrsqm-0.0.2/src/mrsqm/sfa/DFT.cpp`

 * *Files identical despite different names*

### Comparing `mrsqm-0.0.1/src/mrsqm/sfa/MFT.cpp` & `mrsqm-0.0.2/src/mrsqm/sfa/MFT.cpp`

 * *Files identical despite different names*

### Comparing `mrsqm-0.0.1/src/mrsqm/sfa/MFT.h` & `mrsqm-0.0.2/src/mrsqm/sfa/MFT.h`

 * *Files identical despite different names*

### Comparing `mrsqm-0.0.1/src/mrsqm/sfa/SFA.cpp` & `mrsqm-0.0.2/src/mrsqm/sfa/SFA.cpp`

 * *Files identical despite different names*

### Comparing `mrsqm-0.0.1/src/mrsqm/sfa/SFA.h` & `mrsqm-0.0.2/src/mrsqm/sfa/SFA.h`

 * *Files identical despite different names*

### Comparing `mrsqm-0.0.1/src/mrsqm/sfa/SFAWrapper.cpp` & `mrsqm-0.0.2/src/mrsqm/sfa/SFAWrapper.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         this->windowSize = window_size;
         this->maxFeatures = word_length;
         this->maxSymbols = alphabet_size;
         this->normMean = normalization;
         this->normTS = normTimeSeries;
 
     }
-    void fit(std::vector<std::vector<double>> &X)
+    void fit(std::vector<std::vector<double>> X)
     {
         std::vector<std::shared_ptr<TimeSeries>> samples = toTimeSeriesData(X);
 
         sfa = new SFA(SFA::EQUI_DEPTH, windowSize, maxFeatures, maxSymbols, normMean);
 
         // create histogramm + distribution
         std::vector<std::shared_ptr<TimeSeries>> windows;
@@ -85,15 +85,15 @@
                 windows.emplace_back(t2);
             }
         }
 
         sfa->divideHistogram(windows, 0);
     }
 
-    std::vector<std::string> transform(std::vector<std::vector<double>> &X)
+    std::vector<std::string> transform(std::vector<std::vector<double>> X)
     {
         std::vector<std::shared_ptr<TimeSeries>> samples = toTimeSeriesData(X);
         std::vector<std::string> seqs;
         MFT fft(windowSize, normMean, sfa);
 
         for (auto ts : samples)
         {
```

### Comparing `mrsqm-0.0.1/src/mrsqm/sfa/TimeSeries.cpp` & `mrsqm-0.0.2/src/mrsqm/sfa/TimeSeries.cpp`

 * *Files identical despite different names*

### Comparing `mrsqm-0.0.1/src/mrsqm/sfa/TimeSeries.h` & `mrsqm-0.0.2/src/mrsqm/sfa/TimeSeries.h`

 * *Files identical despite different names*

### Comparing `mrsqm-0.0.1/src/mrsqm/sqminer.h` & `mrsqm-0.0.2/src/mrsqm/sqminer.h`

 * *Files identical despite different names*

### Comparing `mrsqm-0.0.1/src/mrsqm/strie.cpp` & `mrsqm-0.0.2/src/mrsqm/strie.cpp`

 * *Files identical despite different names*

### Comparing `mrsqm-0.0.1/src/mrsqm.egg-info/SOURCES.txt` & `mrsqm-0.0.2/src/mrsqm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

