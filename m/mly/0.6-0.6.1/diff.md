# Comparing `tmp/mly-0.6.tar.gz` & `tmp/mly-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mly-0.6.tar", last modified: Tue Jul 18 15:37:30 2023, max compression
+gzip compressed data, was "mly-0.6.1.tar", last modified: Fri Jul 21 10:11:37 2023, max compression
```

## Comparing `mly-0.6.tar` & `mly-0.6.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:37:30.291577 mly-0.6/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-10 08:55:19.000000 mly-0.6/LICENSE
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      495 2023-07-18 15:37:30.291577 mly-0.6/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2021-01-11 16:48:33.000000 mly-0.6/README.md
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:37:30.270577 mly-0.6/mly/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  1433718 2021-05-11 10:43:11.000000 mly-0.6/mly/SRD.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:15:39.000000 mly-0.6/mly/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10014 2023-07-18 09:16:42.000000 mly-0.6/mly/createFileSystem.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:37:30.282577 mly-0.6/mly/datatools/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      155 2023-07-18 09:16:42.000000 mly-0.6/mly/datatools/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22332 2023-07-18 09:16:42.000000 mly-0.6/mly/datatools/core.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28108 2023-07-18 09:16:42.000000 mly-0.6/mly/datatools/datatools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    91856 2023-07-18 15:30:16.000000 mly-0.6/mly/datatools/generator.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:37:30.286577 mly-0.6/mly/datatools/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-07-18 09:16:42.000000 mly-0.6/mly/datatools/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3438 2023-07-18 09:16:42.000000 mly-0.6/mly/datatools/tests/test_core.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      441 2023-07-18 09:16:42.000000 mly-0.6/mly/datatools/tests/test_datatools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4975 2023-07-18 09:16:42.000000 mly-0.6/mly/datatools/tests/test_generator.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    18633 2023-07-18 09:16:42.000000 mly-0.6/mly/exceptions.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7770 2022-08-17 15:08:03.000000 mly-0.6/mly/mlTools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6996 2021-01-11 16:48:33.000000 mly-0.6/mly/models.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7316 2023-07-18 09:16:42.000000 mly-0.6/mly/offlinefar.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7797 2023-07-18 09:16:42.000000 mly-0.6/mly/plugins.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10153 2023-07-18 09:16:42.000000 mly-0.6/mly/projectwave.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8913 2022-03-15 16:16:40.000000 mly-0.6/mly/simulateddetectornoise.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13856 2023-07-18 10:44:50.000000 mly-0.6/mly/skymap_utils.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:37:30.290577 mly-0.6/mly/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      728 2021-10-07 09:34:45.000000 mly-0.6/mly/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1601 2021-10-08 08:22:16.000000 mly-0.6/mly/tests/test_init.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5258 2022-03-02 09:58:19.000000 mly-0.6/mly/tests/test_tools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13037 2023-07-18 09:16:42.000000 mly-0.6/mly/tools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   126794 2023-07-18 15:30:30.000000 mly-0.6/mly/validators.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    34282 2023-07-18 09:16:42.000000 mly-0.6/mly/waveforms.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:37:30.278577 mly-0.6/mly.egg-info/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      495 2023-07-18 15:37:30.000000 mly-0.6/mly.egg-info/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      730 2023-07-18 15:37:30.000000 mly-0.6/mly.egg-info/SOURCES.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-07-18 15:37:30.000000 mly-0.6/mly.egg-info/dependency_links.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       96 2023-07-18 15:37:30.000000 mly-0.6/mly.egg-info/requires.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-07-18 15:37:30.000000 mly-0.6/mly.egg-info/top_level.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       79 2023-07-18 15:37:30.292577 mly-0.6/setup.cfg
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      952 2023-07-18 15:36:55.000000 mly-0.6/setup.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:11:37.096082 mly-0.6.1/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-10 08:55:19.000000 mly-0.6.1/LICENSE
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      497 2023-07-21 10:11:37.096082 mly-0.6.1/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2021-01-11 16:48:33.000000 mly-0.6.1/README.md
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:11:37.080082 mly-0.6.1/mly/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  1433718 2021-05-11 10:43:11.000000 mly-0.6.1/mly/SRD.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:15:39.000000 mly-0.6.1/mly/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10014 2023-07-18 09:16:42.000000 mly-0.6.1/mly/createFileSystem.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:11:37.087082 mly-0.6.1/mly/datatools/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      155 2023-07-18 09:16:42.000000 mly-0.6.1/mly/datatools/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22332 2023-07-18 09:16:42.000000 mly-0.6.1/mly/datatools/core.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28108 2023-07-20 14:51:05.000000 mly-0.6.1/mly/datatools/datatools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    91859 2023-07-20 15:33:40.000000 mly-0.6.1/mly/datatools/generator.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:11:37.091082 mly-0.6.1/mly/datatools/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-07-18 09:16:42.000000 mly-0.6.1/mly/datatools/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3438 2023-07-18 09:16:42.000000 mly-0.6.1/mly/datatools/tests/test_core.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      441 2023-07-18 09:16:42.000000 mly-0.6.1/mly/datatools/tests/test_datatools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4975 2023-07-18 09:16:42.000000 mly-0.6.1/mly/datatools/tests/test_generator.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    18633 2023-07-18 09:16:42.000000 mly-0.6.1/mly/exceptions.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7770 2022-08-17 15:08:03.000000 mly-0.6.1/mly/mlTools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6996 2021-01-11 16:48:33.000000 mly-0.6.1/mly/models.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7316 2023-07-18 09:16:42.000000 mly-0.6.1/mly/offlinefar.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7797 2023-07-18 09:16:42.000000 mly-0.6.1/mly/plugins.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10153 2023-07-18 09:16:42.000000 mly-0.6.1/mly/projectwave.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8913 2022-03-15 16:16:40.000000 mly-0.6.1/mly/simulateddetectornoise.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13856 2023-07-20 14:53:35.000000 mly-0.6.1/mly/skymap_utils.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:11:37.095082 mly-0.6.1/mly/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      728 2021-10-07 09:34:45.000000 mly-0.6.1/mly/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1601 2021-10-08 08:22:16.000000 mly-0.6.1/mly/tests/test_init.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5258 2022-03-02 09:58:19.000000 mly-0.6.1/mly/tests/test_tools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13037 2023-07-18 09:16:42.000000 mly-0.6.1/mly/tools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   126788 2023-07-20 15:40:17.000000 mly-0.6.1/mly/validators.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    34282 2023-07-18 09:16:42.000000 mly-0.6.1/mly/waveforms.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-21 10:11:37.084082 mly-0.6.1/mly.egg-info/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      497 2023-07-21 10:11:37.000000 mly-0.6.1/mly.egg-info/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      730 2023-07-21 10:11:37.000000 mly-0.6.1/mly.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-07-21 10:11:37.000000 mly-0.6.1/mly.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       96 2023-07-21 10:11:37.000000 mly-0.6.1/mly.egg-info/requires.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-07-21 10:11:37.000000 mly-0.6.1/mly.egg-info/top_level.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       79 2023-07-21 10:11:37.097082 mly-0.6.1/setup.cfg
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      954 2023-07-21 09:44:55.000000 mly-0.6.1/setup.py
```

### Comparing `mly-0.6/LICENSE` & `mly-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mly-0.6/mly/SRD.py` & `mly-0.6.1/mly/SRD.py`

 * *Files identical despite different names*

### Comparing `mly-0.6/mly/createFileSystem.py` & `mly-0.6.1/mly/createFileSystem.py`

 * *Files identical despite different names*

### Comparing `mly-0.6/mly/datatools/core.py` & `mly-0.6.1/mly/datatools/core.py`

 * *Files identical despite different names*

### Comparing `mly-0.6/mly/datatools/datatools.py` & `mly-0.6.1/mly/datatools/datatools.py`

 * *Files identical despite different names*

### Comparing `mly-0.6/mly/datatools/generator.py` & `mly-0.6.1/mly/datatools/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,15 +362,15 @@
                 and all(len(el)==2 for el in noiseSourceFile)):
 
             noiseFormat='gwdatafind'
 
         # Loading noise using file paths of txt files (different for each detector)
         elif (isinstance(noiseSourceFile,list) 
               and len(noiseSourceFile)==len(detectors) 
-              and all(isisntance(path_,str) for path_ in noiseSourceFile)
+              and all(isinstance(path_,str) for path_ in noiseSourceFile)
               and all(path_[-4:]=='.txt' for path_ in noiseSourceFile)):
 
             noiseFormat='txtD'
 
         # Loading noise using file paths of txt files (one with all detectors)
         elif (isinstance(noiseSourceFile,str) 
               and noiseSourceFile[-4:]=='.txt'):
@@ -698,16 +698,16 @@
 
                 ind=internalLags(detectors = detectors
                                    ,lags = timeSlides
                                    ,duration = duration
                                    ,fs = 1
                                    ,size = len(file_)
                                    ,start_from_sec=startingPoint)
-                for det in detectors:
-                    print("det",gps0[det]+np.array(ind[det])+(windowSize-duration)/2)
+                #for det in detectors:
+                    #print("det",gps0[det]+np.array(ind[det])+(windowSize-duration)/2)
 
                 if size > len(file_):
                     print("Requested size is bigger that the noise sourse data"
                                      +" can provide. Background will be used multiple times")
 
                     indexRepetition = ceil(size/len(file_))
 
@@ -771,14 +771,15 @@
 #             print(len(ind['H']),len(ind['L']))
 #             print(len(noise_segDict['H'])/fs,len(noise_segDict['L'])/fs)
 
 
 
     thetime = time.time()
     DATA=DataSet(name = name)
+
     for I in range(size):
 
 
         t0=time.time()
 
         detKeys = list(injectionFileDict.keys())
```

### Comparing `mly-0.6/mly/datatools/tests/test_core.py` & `mly-0.6.1/mly/datatools/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `mly-0.6/mly/datatools/tests/test_generator.py` & `mly-0.6.1/mly/datatools/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `mly-0.6/mly/exceptions.py` & `mly-0.6.1/mly/exceptions.py`

 * *Files identical despite different names*

### Comparing `mly-0.6/mly/mlTools.py` & `mly-0.6.1/mly/mlTools.py`

 * *Files identical despite different names*

### Comparing `mly-0.6/mly/models.py` & `mly-0.6.1/mly/models.py`

 * *Files identical despite different names*

### Comparing `mly-0.6/mly/offlinefar.py` & `mly-0.6.1/mly/offlinefar.py`

 * *Files identical despite different names*

### Comparing `mly-0.6/mly/plugins.py` & `mly-0.6.1/mly/plugins.py`

 * *Files identical despite different names*

### Comparing `mly-0.6/mly/projectwave.py` & `mly-0.6.1/mly/projectwave.py`

 * *Files identical despite different names*

### Comparing `mly-0.6/mly/simulateddetectornoise.py` & `mly-0.6.1/mly/simulateddetectornoise.py`

 * *Files identical despite different names*

### Comparing `mly-0.6/mly/skymap_utils.py` & `mly-0.6.1/mly/skymap_utils.py`

 * *Files identical despite different names*

### Comparing `mly-0.6/mly/tests/__init__.py` & `mly-0.6.1/mly/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mly-0.6/mly/tests/test_init.py` & `mly-0.6.1/mly/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `mly-0.6/mly/tests/test_tools.py` & `mly-0.6.1/mly/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `mly-0.6/mly/tools.py` & `mly-0.6.1/mly/tools.py`

 * *Files identical despite different names*

### Comparing `mly-0.6/mly/validators.py` & `mly-0.6.1/mly/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,29 +187,28 @@
 
             
             if 'stackDetectorDict' in kwargs:
                 DATA = stackDetector(DATA, **kwargs['stackDetectorDict'])
                 
             #random.shuffle(DATA.dataPods)
 
-
             result[loopname].append(val)
 
             
             for m in range(len(trained_models)):
                 dataList=[]
                 input_shape=trained_models[m].input_shape
                 if isinstance(input_shape,tuple): input_shape=[input_shape]
                 for i in range(len(models[1][m])):
-                    print(input_shape[i],models[1][m][i])
-                    print(DATA[0].__getattribute__(models[1][m][i]).shape)
+                    # print(input_shape[i],models[1][m][i])
+                    # print(DATA[0].__getattribute__(models[1][m][i]).shape)
                     dataList.append(DATA.exportData(models[1][m][i],shape=input_shape[i]))
 
                 if len(dataList)==1: dataList=dataList[0]
-                scores = trained_models[m].predict(dataList, batch_size=1, verbose=0)[:,columns[m]]
+                scores = trained_models[m](dataList, training=False).numpy()[:,columns[m]]
 
                 if 'scores'+str(m+1) in list(result.keys()):
                     result['scores'+str(m+1)].append(scores.tolist())
                 else:
                     result['scores'+str(m+1)]=[scores.tolist()]
 
         if savePath==None:
```

### Comparing `mly-0.6/mly/waveforms.py` & `mly-0.6.1/mly/waveforms.py`

 * *Files identical despite different names*

### Comparing `mly-0.6/mly.egg-info/SOURCES.txt` & `mly-0.6.1/mly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mly-0.6/setup.py` & `mly-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mly",
-    version="0.6",
+    version="0.6.1",
     author="Vasileios Skliris",
     author_email='vas.skliris@gmail.com',
     description='This tool helps you create training and testing data for ML to use for gravitational wave detection.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://pypi.python.org/pypi/mly/',
     packages=setuptools.find_packages(),
```

