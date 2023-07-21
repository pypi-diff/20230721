# Comparing `tmp/Metrics_Miscellany-0.2-py2.py3-none-any.whl.zip` & `tmp/Metrics_Miscellany-0.2.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6804 bytes, number of entries: 10
+Zip file size: 6855 bytes, number of entries: 10
 -rw-rw----  2.0 unx       45 b- defN 22-Nov-08 18:06 metrics_miscellany/__init__.py
 -rw-rw----  2.0 unx     1799 b- defN 23-Apr-30 18:18 metrics_miscellany/estimators.py
 -rw-rw----  2.0 unx      606 b- defN 23-Apr-30 18:18 metrics_miscellany/random.py
--rw-rw----  2.0 unx     6099 b- defN 23-Jul-21 18:11 metrics_miscellany/tests.py
+-rw-rw----  2.0 unx     6229 b- defN 23-Jul-21 18:39 metrics_miscellany/tests.py
 -rw-rw----  2.0 unx     1588 b- defN 23-Jun-01 18:39 metrics_miscellany/utils.py
--rw-rw----  2.0 unx      282 b- defN 23-Jul-21 18:15 Metrics_Miscellany-0.2.dist-info/LICENSE.txt
--rw-rw----  2.0 unx      394 b- defN 23-Jul-21 18:15 Metrics_Miscellany-0.2.dist-info/METADATA
--rw-rw----  2.0 unx      110 b- defN 23-Jul-21 18:15 Metrics_Miscellany-0.2.dist-info/WHEEL
--rw-rw----  2.0 unx       19 b- defN 23-Jul-21 18:15 Metrics_Miscellany-0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      860 b- defN 23-Jul-21 18:15 Metrics_Miscellany-0.2.dist-info/RECORD
-10 files, 11802 bytes uncompressed, 5318 bytes compressed:  54.9%
+-rw-rw----  2.0 unx      282 b- defN 23-Jul-21 19:00 Metrics_Miscellany-0.2.1.dist-info/LICENSE.txt
+-rw-rw----  2.0 unx      396 b- defN 23-Jul-21 19:00 Metrics_Miscellany-0.2.1.dist-info/METADATA
+-rw-rw----  2.0 unx      110 b- defN 23-Jul-21 19:00 Metrics_Miscellany-0.2.1.dist-info/WHEEL
+-rw-rw----  2.0 unx       19 b- defN 23-Jul-21 19:00 Metrics_Miscellany-0.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      870 b- defN 23-Jul-21 19:00 Metrics_Miscellany-0.2.1.dist-info/RECORD
+10 files, 11944 bytes uncompressed, 5349 bytes compressed:  55.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: metrics_miscellany/tests.py
 Comment: 
 
 Filename: metrics_miscellany/utils.py
 Comment: 
 
-Filename: Metrics_Miscellany-0.2.dist-info/LICENSE.txt
+Filename: Metrics_Miscellany-0.2.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: Metrics_Miscellany-0.2.dist-info/METADATA
+Filename: Metrics_Miscellany-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: Metrics_Miscellany-0.2.dist-info/WHEEL
+Filename: Metrics_Miscellany-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: Metrics_Miscellany-0.2.dist-info/top_level.txt
+Filename: Metrics_Miscellany-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: Metrics_Miscellany-0.2.dist-info/RECORD
+Filename: Metrics_Miscellany-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## metrics_miscellany/tests.py

```diff
@@ -60,15 +60,15 @@
         """
         Once we have ranks, construct SM statistic
         """
         # Fill missing ranks with (k_i+1)/2
         R = R.where(~np.isnan(R),(kay+1)/2,axis=1)
 
         # Construct adjusted observation matrix
-        A = R.subtract((kay+1)/2,axis=1)@np.sqrt(12/(kay+1))
+        A = R.subtract((kay.values+1)/2,axis=1)@np.sqrt(12/(kay.values+1))
 
         # Count of observations in both columns k and l
         O = ~np.isnan(X)+0.
 
         Sigma = np.eye(O.shape[0]) - O@O.T
 
         # Delete diagonal
@@ -104,15 +104,18 @@
 
         SE = 0
         lastSE = np.inf
         its = 0
         sms = []
         while (its < 30) or (np.abs(SE-lastSE) > tol):
             lastSE = SE
-            sms.append(construct_statistic(pd.DataFrame(np.apply_along_axis(np.random.permutation,axis=0,arr=R.values)),kay))
+            scrambled = pd.DataFrame(np.apply_along_axis(np.random.permutation,axis=0,arr=R.values),
+                                     index=R.index,columns=R.columns)
+           
+            sms.append(construct_statistic(scrambled,kay))
             SE = np.std(sms)
             its += 1
         p = np.mean(sms>SM)
 
     return SM,p
 
 friedman = skillings_mack
```

