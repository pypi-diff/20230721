# Comparing `tmp/fsrs4anki_optimizer-4.3.0.tar.gz` & `tmp/fsrs4anki_optimizer-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-4.3.0.tar", last modified: Fri Jul 21 04:19:01 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-4.3.1.tar", last modified: Fri Jul 21 08:36:27 2023, max compression
```

## Comparing `fsrs4anki_optimizer-4.3.0.tar` & `fsrs4anki_optimizer-4.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:19:01.332590 fsrs4anki_optimizer-4.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-21 04:19:01.332590 fsrs4anki_optimizer-4.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:19:01.332590 fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 04:18:50.000000 fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-21 04:18:50.000000 fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50825 2023-07-21 04:18:50.000000 fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:19:01.332590 fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-21 04:19:01.000000 fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-21 04:19:01.000000 fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 04:19:01.000000 fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-21 04:19:01.000000 fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-21 04:19:01.000000 fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-21 04:18:50.000000 fsrs4anki_optimizer-4.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 04:19:01.332590 fsrs4anki_optimizer-4.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 04:18:50.000000 fsrs4anki_optimizer-4.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:36:27.560448 fsrs4anki_optimizer-4.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-21 08:36:27.560448 fsrs4anki_optimizer-4.3.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:36:27.556448 fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 08:36:12.000000 fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-21 08:36:12.000000 fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51134 2023-07-21 08:36:12.000000 fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:36:27.560448 fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-21 08:36:27.000000 fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-21 08:36:27.000000 fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:36:27.000000 fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-21 08:36:27.000000 fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-21 08:36:27.000000 fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-21 08:36:12.000000 fsrs4anki_optimizer-4.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 08:36:27.560448 fsrs4anki_optimizer-4.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 08:36:12.000000 fsrs4anki_optimizer-4.3.1/setup.py
```

### Comparing `fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-4.3.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -492,23 +492,24 @@
         rating_stability = {}
         rating_count = {}
         average_recall = self.dataset['y'].mean()
 
         for first_rating in ("1", "2", "3", "4"):
             group = self.S0_dataset_group[self.S0_dataset_group['r_history'] == first_rating]
             if group.empty:
+                tqdm.write(f'Not enough data for first rating {first_rating}. Expected at least 100, got 0.')
                 continue
             delta_t = group['delta_t']
             recall = (group['y']['mean'] * group['y']['count'] + average_recall * 1) / (group['y']['count'] + 1)
             count = group['y']['count']
             total_count = sum(count)
             if total_count < 100:
                 tqdm.write(f'Not enough data for first rating {first_rating}. Expected at least 100, got {total_count}.')
                 continue
-            params, _ = curve_fit(power_forgetting_curve, delta_t, recall, sigma=1/np.sqrt(count), bounds=((0.1), (60 if total_count < 1000 else 365)))
+            params, _ = curve_fit(power_forgetting_curve, delta_t, recall, sigma=1/np.sqrt(count), bounds=((0.1), (15 if total_count < 1000 else 365)))
             stability = params[0]
             rating_stability[int(first_rating)] = stability
             rating_count[int(first_rating)] = total_count
             predict_recall = power_forgetting_curve(delta_t, *params)
             rmse = mean_squared_error(recall, predict_recall, sample_weight=count, squared=False)
 
             if verbose:
@@ -522,16 +523,20 @@
                 plt.xlim(0, 30)
                 plt.xlabel('Interval')
                 plt.ylabel('Recall')
                 plt.title(f'Forgetting curve for first rating {first_rating} (n={total_count}, s={stability:.2f})')
                 plt.show()
                 tqdm.write(str(rating_stability))
 
-        if len(rating_stability) < 2:
+        if len(rating_stability) == 0:
             raise Exception("Not enough data for pretraining!")
+        elif len(rating_stability) == 1:
+            init_stability = round(list(rating_stability.values())[0], 2)
+            for i in (0, 1, 2, 3):
+                self.init_w[i] = init_stability
         elif len(rating_stability) == 4:
             for rating, stability in rating_stability.items():
                 self.init_w[rating-1] = round(stability, 2)
             tqdm.write(f"Pretrain finished!")
             return
 
         def S0_rating_curve(rating, a, b, c):
@@ -549,15 +554,15 @@
             plt.grid(True)
             plt.xlabel('First rating')
             plt.ylabel('Stability')
             plt.title('Stability for first rating')
             plt.show()
 
         for rating in (1, 2, 3, 4):
-            again_extrap = max(min(S0_rating_curve(1, *params), 60), 0.1)
+            again_extrap = max(min(S0_rating_curve(1, *params), 15), 0.1)
             # if there isn't enough data to calculate the value for "Again" exactly
             if 1 not in rating_stability:
                 # then check if there exists an exact value for "Hard"
                 if 2 in rating_stability:
                     # if it exists, then check whether the extrapolation breaks monotonicity
                     # Again > Hard is possible, but we should allow it only for exact values, otherwise we should assume monotonicity
                     if again_extrap > rating_stability[2]:
@@ -566,15 +571,15 @@
                     else:
                         # if it doesn't break monotonicity, then use the extrapolated value
                         rating_stability[1] = again_extrap
                 # if an exact value for "Hard" doesn't exist, then just use the extrapolation, there's nothing else we can do
                 else:
                     rating_stability[1] = again_extrap
             elif rating not in rating_stability:
-                rating_stability[rating] = max(min(S0_rating_curve(rating, *params), 60), 0.1)
+                rating_stability[rating] = max(min(S0_rating_curve(rating, *params), 15), 0.1)
 
         rating_stability = {k: round(v, 2) for k, v in sorted(rating_stability.items(), key=lambda item: item[0])}
         for rating, stability in rating_stability.items():
             self.init_w[rating-1] = stability
         tqdm.write(f"Pretrain finished!")
 
     def train(self, lr: float = 4e-2, n_epoch: int = 5, n_splits: int = 5, batch_size: int = 512, verbose: bool = True):
```

